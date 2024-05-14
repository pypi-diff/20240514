# Comparing `tmp/maptasker-4.0.2.tar.gz` & `tmp/maptasker-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maptasker-4.0.2.tar", max compression
+gzip compressed data, was "maptasker-4.0.5.tar", max compression
```

## Comparing `maptasker-4.0.2.tar` & `maptasker-4.0.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1079 2024-02-16 16:36:22.405000 maptasker-4.0.2/LICENSE.txt
--rw-r--r--   0        0        0      536 2024-03-04 15:40:38.700000 maptasker-4.0.2/README_PyPl.md
--rw-r--r--   0        0        0        0 2024-03-10 15:08:20.218081 maptasker-4.0.2/maptasker/__init__.py
--rw-r--r--   0        0        0     9216 2024-02-22 20:13:00.839000 maptasker-4.0.2/maptasker/assets/Thumbs.db
--rw-r--r--   0        0        0      390 2024-03-25 17:21:31.285000 maptasker-4.0.2/maptasker/assets/icons/arrow.png
--rw-r--r--   0        0        0   104984 2023-11-21 17:46:03.716000 maptasker-4.0.2/maptasker/assets/maptasker_logo_dark.png
--rw-r--r--   0        0        0   104904 2023-11-21 17:46:03.717000 maptasker-4.0.2/maptasker/assets/maptasker_logo_light.png
--rw-r--r--   0        0        0     1782 2024-01-08 16:34:50.197000 maptasker-4.0.2/maptasker/main.py
--rw-r--r--   0        0        0       17 2024-02-02 20:14:04.969000 maptasker-4.0.2/maptasker/src/__init__.py
--rw-r--r--   0        0        0    13403 2024-04-25 15:06:44.558922 maptasker-4.0.2/maptasker/src/actargs.py
--rw-r--r--   0        0        0    22348 2024-04-25 15:06:44.559256 maptasker-4.0.2/maptasker/src/action.py
--rw-r--r--   0        0        0   124439 2024-04-22 17:26:35.331982 maptasker-4.0.2/maptasker/src/actionc.py
--rw-r--r--   0        0        0     8377 2024-02-22 20:13:10.380000 maptasker-4.0.2/maptasker/src/actiond.py
--rw-r--r--   0        0        0    15298 2024-05-06 23:54:46.924101 maptasker-4.0.2/maptasker/src/actione.py
--rw-r--r--   0        0        0     9824 2024-04-22 17:26:35.332913 maptasker-4.0.2/maptasker/src/actionr.py
--rw-r--r--   0        0        0    17204 2024-04-25 15:06:44.559901 maptasker-4.0.2/maptasker/src/actiont.py
--rw-r--r--   0        0        0     3376 2024-02-22 20:13:12.356000 maptasker-4.0.2/maptasker/src/addcss.py
--rw-r--r--   0        0        0     3783 2024-04-03 14:57:05.818846 maptasker-4.0.2/maptasker/src/caveats.py
--rw-r--r--   0        0        0    11837 2024-04-08 18:48:52.139846 maptasker-4.0.2/maptasker/src/clip.py
--rw-r--r--   0        0        0     8642 2024-05-06 14:43:13.750448 maptasker-4.0.2/maptasker/src/colors.py
--rw-r--r--   0        0        0     3186 2024-03-08 20:16:24.477154 maptasker-4.0.2/maptasker/src/colrmode.py
--rw-r--r--   0        0        0    11594 2024-04-25 15:06:44.560209 maptasker-4.0.2/maptasker/src/condition.py
--rw-r--r--   0        0        0     3112 2024-05-06 23:54:46.779880 maptasker-4.0.2/maptasker/src/config.py
--rw-r--r--   0        0        0     6541 2024-02-02 20:14:15.316000 maptasker-4.0.2/maptasker/src/debug.py
--rw-r--r--   0        0        0      417 2023-12-04 16:07:45.842000 maptasker-4.0.2/maptasker/src/deprecate.py
--rw-r--r--   0        0        0    30601 2024-03-25 17:21:29.641646 maptasker-4.0.2/maptasker/src/diagram.py
--rw-r--r--   0        0        0    27007 2024-02-16 16:36:21.774000 maptasker-4.0.2/maptasker/src/diagutil.py
--rw-r--r--   0        0        0    19996 2024-02-09 18:52:35.434000 maptasker-4.0.2/maptasker/src/dirout.py
--rw-r--r--   0        0        0     3109 2024-05-06 16:36:10.687404 maptasker-4.0.2/maptasker/src/error.py
--rw-r--r--   0        0        0     2399 2024-02-02 20:14:19.267000 maptasker-4.0.2/maptasker/src/fonts.py
--rw-r--r--   0        0        0     4456 2024-04-22 17:26:35.333800 maptasker-4.0.2/maptasker/src/format.py
--rw-r--r--   0        0        0     5848 2024-05-06 23:54:46.847864 maptasker-4.0.2/maptasker/src/frontmtr.py
--rw-r--r--   0        0        0     5353 2024-04-22 17:26:35.334483 maptasker-4.0.2/maptasker/src/getbakup.py
--rw-r--r--   0        0        0     2311 2024-03-28 13:52:59.398409 maptasker-4.0.2/maptasker/src/getids.py
--rw-r--r--   0        0        0     9793 2024-05-06 14:43:13.752715 maptasker-4.0.2/maptasker/src/getputer.py
--rw-r--r--   0        0        0     9754 2024-02-22 20:13:15.666000 maptasker-4.0.2/maptasker/src/globalvr.py
--rw-r--r--   0        0        0    83582 2024-05-07 14:30:59.654538 maptasker-4.0.2/maptasker/src/guiutils.py
--rw-r--r--   0        0        0     3753 2024-05-06 14:43:13.754152 maptasker-4.0.2/maptasker/src/initparg.py
--rw-r--r--   0        0        0     2660 2024-04-25 15:06:44.561504 maptasker-4.0.2/maptasker/src/kidapp.py
--rw-r--r--   0        0        0    25652 2024-05-06 23:54:46.961056 maptasker-4.0.2/maptasker/src/lineout.py
--rw-r--r--   0        0        0    11484 2024-05-06 23:54:46.913549 maptasker-4.0.2/maptasker/src/mapai.py
--rw-r--r--   0        0        0    30992 2024-05-06 16:27:01.282662 maptasker-4.0.2/maptasker/src/mapit.py
--rw-r--r--   0        0        0    11468 2024-05-06 14:43:13.756075 maptasker-4.0.2/maptasker/src/maputils.py
--rw-r--r--   0        0        0     2788 2023-12-28 18:49:26.174000 maptasker-4.0.2/maptasker/src/nameattr.py
--rw-r--r--   0        0        0    20711 2024-02-16 16:36:22.869000 maptasker-4.0.2/maptasker/src/outline.py
--rw-r--r--   0        0        0    19666 2024-05-06 14:43:13.756791 maptasker-4.0.2/maptasker/src/parsearg.py
--rw-r--r--   0        0        0     8606 2024-02-02 20:14:19.240000 maptasker-4.0.2/maptasker/src/prefers.py
--rw-r--r--   0        0        0     6916 2024-05-06 14:43:13.757332 maptasker-4.0.2/maptasker/src/primitem.py
--rw-r--r--   0        0        0    11458 2024-04-22 17:26:35.337860 maptasker-4.0.2/maptasker/src/proclist.py
--rw-r--r--   0        0        0    14932 2024-05-06 23:54:46.958423 maptasker-4.0.2/maptasker/src/profiles.py
--rw-r--r--   0        0        0     2280 2024-02-02 20:14:19.331000 maptasker-4.0.2/maptasker/src/progargs.py
--rw-r--r--   0        0        0    14916 2024-05-06 14:43:13.758007 maptasker-4.0.2/maptasker/src/proginit.py
--rw-r--r--   0        0        0    30467 2024-05-06 14:43:13.758815 maptasker-4.0.2/maptasker/src/projects.py
--rw-r--r--   0        0        0     6428 2024-05-06 23:54:46.896689 maptasker-4.0.2/maptasker/src/property.py
--rw-r--r--   0        0        0    23015 2024-04-25 15:06:44.563028 maptasker-4.0.2/maptasker/src/runcli.py
--rw-r--r--   0        0        0     7296 2024-05-06 16:32:13.450930 maptasker-4.0.2/maptasker/src/rungui.py
--rw-r--r--   0        0        0    23118 2024-04-25 15:06:44.563378 maptasker-4.0.2/maptasker/src/scenes.py
--rw-r--r--   0        0        0    16315 2024-02-02 20:14:14.236000 maptasker-4.0.2/maptasker/src/servicec.py
--rw-r--r--   0        0        0     6193 2024-02-22 20:13:15.794000 maptasker-4.0.2/maptasker/src/share.py
--rw-r--r--   0        0        0     3658 2024-02-16 16:36:21.861000 maptasker-4.0.2/maptasker/src/shelsort.py
--rw-r--r--   0        0        0     7882 2024-05-06 15:15:41.461773 maptasker-4.0.2/maptasker/src/sysconst.py
--rw-r--r--   0        0        0     6351 2024-04-22 17:26:35.341001 maptasker-4.0.2/maptasker/src/taskactn.py
--rw-r--r--   0        0        0     6835 2024-03-25 17:21:29.645740 maptasker-4.0.2/maptasker/src/taskerd.py
--rw-r--r--   0        0        0     2673 2024-04-22 17:26:35.341286 maptasker-4.0.2/maptasker/src/taskflag.py
--rw-r--r--   0        0        0    23587 2024-05-06 23:54:47.028952 maptasker-4.0.2/maptasker/src/tasks.py
--rw-r--r--   0        0        0    10000 2024-05-06 23:54:46.934833 maptasker-4.0.2/maptasker/src/taskuniq.py
--rw-r--r--   0        0        0     2100 2024-02-20 15:01:50.903000 maptasker-4.0.2/maptasker/src/twisty.py
--rw-r--r--   0        0        0   124737 2024-05-07 14:32:58.867650 maptasker-4.0.2/maptasker/src/userintr.py
--rw-r--r--   0        0        0    10663 2024-04-25 15:06:44.565915 maptasker-4.0.2/maptasker/src/xmldata.py
--rw-r--r--   0        0        0     5077 2024-05-06 15:15:41.437275 maptasker-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 maptasker-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-02-16 16:36:22.405000 maptasker-4.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      536 2024-03-04 15:40:38.700000 maptasker-4.0.5/README_PyPl.md
+-rw-r--r--   0        0        0        0 2024-03-10 15:08:20.218081 maptasker-4.0.5/maptasker/__init__.py
+-rw-r--r--   0        0        0     9216 2024-02-22 20:13:00.839000 maptasker-4.0.5/maptasker/assets/Thumbs.db
+-rw-r--r--   0        0        0      390 2024-03-25 17:21:31.285000 maptasker-4.0.5/maptasker/assets/icons/arrow.png
+-rw-r--r--   0        0        0   104984 2023-11-21 17:46:03.716000 maptasker-4.0.5/maptasker/assets/maptasker_logo_dark.png
+-rw-r--r--   0        0        0   104904 2023-11-21 17:46:03.717000 maptasker-4.0.5/maptasker/assets/maptasker_logo_light.png
+-rw-r--r--   0        0        0     1782 2024-01-08 16:34:50.197000 maptasker-4.0.5/maptasker/main.py
+-rw-r--r--   0        0        0       17 2024-02-02 20:14:04.969000 maptasker-4.0.5/maptasker/src/__init__.py
+-rw-r--r--   0        0        0    13403 2024-04-25 15:06:44.558922 maptasker-4.0.5/maptasker/src/actargs.py
+-rw-r--r--   0        0        0    22348 2024-04-25 15:06:44.559256 maptasker-4.0.5/maptasker/src/action.py
+-rw-r--r--   0        0        0   124901 2024-05-14 13:33:40.514899 maptasker-4.0.5/maptasker/src/actionc.py
+-rw-r--r--   0        0        0     8377 2024-02-22 20:13:10.380000 maptasker-4.0.5/maptasker/src/actiond.py
+-rw-r--r--   0        0        0    15298 2024-05-07 14:51:54.095647 maptasker-4.0.5/maptasker/src/actione.py
+-rw-r--r--   0        0        0     9824 2024-04-22 17:26:35.332913 maptasker-4.0.5/maptasker/src/actionr.py
+-rw-r--r--   0        0        0    17204 2024-04-25 15:06:44.559901 maptasker-4.0.5/maptasker/src/actiont.py
+-rw-r--r--   0        0        0     3376 2024-02-22 20:13:12.356000 maptasker-4.0.5/maptasker/src/addcss.py
+-rw-r--r--   0        0        0     3783 2024-04-03 14:57:05.818846 maptasker-4.0.5/maptasker/src/caveats.py
+-rw-r--r--   0        0        0    11837 2024-04-08 18:48:52.139846 maptasker-4.0.5/maptasker/src/clip.py
+-rw-r--r--   0        0        0     8642 2024-05-06 14:43:13.750448 maptasker-4.0.5/maptasker/src/colors.py
+-rw-r--r--   0        0        0     3186 2024-03-08 20:16:24.477154 maptasker-4.0.5/maptasker/src/colrmode.py
+-rw-r--r--   0        0        0    11594 2024-04-25 15:06:44.560209 maptasker-4.0.5/maptasker/src/condition.py
+-rw-r--r--   0        0        0     3112 2024-05-07 14:51:54.096009 maptasker-4.0.5/maptasker/src/config.py
+-rw-r--r--   0        0        0     6541 2024-02-02 20:14:15.316000 maptasker-4.0.5/maptasker/src/debug.py
+-rw-r--r--   0        0        0      417 2023-12-04 16:07:45.842000 maptasker-4.0.5/maptasker/src/deprecate.py
+-rw-r--r--   0        0        0    30601 2024-03-25 17:21:29.641646 maptasker-4.0.5/maptasker/src/diagram.py
+-rw-r--r--   0        0        0    27007 2024-02-16 16:36:21.774000 maptasker-4.0.5/maptasker/src/diagutil.py
+-rw-r--r--   0        0        0    20049 2024-05-14 17:24:09.321714 maptasker-4.0.5/maptasker/src/dirout.py
+-rw-r--r--   0        0        0     3109 2024-05-07 14:51:54.096334 maptasker-4.0.5/maptasker/src/error.py
+-rw-r--r--   0        0        0     2399 2024-02-02 20:14:19.267000 maptasker-4.0.5/maptasker/src/fonts.py
+-rw-r--r--   0        0        0     4456 2024-04-22 17:26:35.333800 maptasker-4.0.5/maptasker/src/format.py
+-rw-r--r--   0        0        0     5848 2024-05-07 14:51:54.096920 maptasker-4.0.5/maptasker/src/frontmtr.py
+-rw-r--r--   0        0        0     5353 2024-04-22 17:26:35.334483 maptasker-4.0.5/maptasker/src/getbakup.py
+-rw-r--r--   0        0        0     2311 2024-03-28 13:52:59.398409 maptasker-4.0.5/maptasker/src/getids.py
+-rw-r--r--   0        0        0    10004 2024-05-14 19:02:03.275498 maptasker-4.0.5/maptasker/src/getputer.py
+-rw-r--r--   0        0        0     9754 2024-02-22 20:13:15.666000 maptasker-4.0.5/maptasker/src/globalvr.py
+-rw-r--r--   0        0        0    90868 2024-05-14 19:03:13.210451 maptasker-4.0.5/maptasker/src/guiutils.py
+-rw-r--r--   0        0        0     3929 2024-05-13 18:12:35.813478 maptasker-4.0.5/maptasker/src/initparg.py
+-rw-r--r--   0        0        0     2660 2024-04-25 15:06:44.561504 maptasker-4.0.5/maptasker/src/kidapp.py
+-rw-r--r--   0        0        0    25652 2024-05-07 14:51:54.098265 maptasker-4.0.5/maptasker/src/lineout.py
+-rw-r--r--   0        0        0    12042 2024-05-14 15:25:44.652366 maptasker-4.0.5/maptasker/src/mapai.py
+-rw-r--r--   0        0        0    30992 2024-05-07 14:51:54.099082 maptasker-4.0.5/maptasker/src/mapit.py
+-rw-r--r--   0        0        0    11488 2024-05-13 16:05:33.251538 maptasker-4.0.5/maptasker/src/maputils.py
+-rw-r--r--   0        0        0     2788 2023-12-28 18:49:26.174000 maptasker-4.0.5/maptasker/src/nameattr.py
+-rw-r--r--   0        0        0    20711 2024-02-16 16:36:22.869000 maptasker-4.0.5/maptasker/src/outline.py
+-rw-r--r--   0        0        0    19666 2024-05-06 14:43:13.756791 maptasker-4.0.5/maptasker/src/parsearg.py
+-rw-r--r--   0        0        0     8606 2024-02-02 20:14:19.240000 maptasker-4.0.5/maptasker/src/prefers.py
+-rw-r--r--   0        0        0     6916 2024-05-06 14:43:13.757332 maptasker-4.0.5/maptasker/src/primitem.py
+-rw-r--r--   0        0        0    11458 2024-04-22 17:26:35.337860 maptasker-4.0.5/maptasker/src/proclist.py
+-rw-r--r--   0        0        0    14932 2024-05-07 14:51:54.099465 maptasker-4.0.5/maptasker/src/profiles.py
+-rw-r--r--   0        0        0     2280 2024-02-02 20:14:19.331000 maptasker-4.0.5/maptasker/src/progargs.py
+-rw-r--r--   0        0        0    14916 2024-05-06 14:43:13.758007 maptasker-4.0.5/maptasker/src/proginit.py
+-rw-r--r--   0        0        0    30467 2024-05-06 14:43:13.758815 maptasker-4.0.5/maptasker/src/projects.py
+-rw-r--r--   0        0        0     6428 2024-05-07 14:51:54.099813 maptasker-4.0.5/maptasker/src/property.py
+-rw-r--r--   0        0        0    23015 2024-04-25 15:06:44.563028 maptasker-4.0.5/maptasker/src/runcli.py
+-rw-r--r--   0        0        0     7289 2024-05-14 14:48:39.484175 maptasker-4.0.5/maptasker/src/rungui.py
+-rw-r--r--   0        0        0    23107 2024-05-12 16:47:13.192977 maptasker-4.0.5/maptasker/src/scenes.py
+-rw-r--r--   0        0        0    16315 2024-02-02 20:14:14.236000 maptasker-4.0.5/maptasker/src/servicec.py
+-rw-r--r--   0        0        0     6193 2024-02-22 20:13:15.794000 maptasker-4.0.5/maptasker/src/share.py
+-rw-r--r--   0        0        0     3658 2024-02-16 16:36:21.861000 maptasker-4.0.5/maptasker/src/shelsort.py
+-rw-r--r--   0        0        0     8187 2024-05-14 19:04:41.783368 maptasker-4.0.5/maptasker/src/sysconst.py
+-rw-r--r--   0        0        0     6351 2024-04-22 17:26:35.341001 maptasker-4.0.5/maptasker/src/taskactn.py
+-rw-r--r--   0        0        0     6835 2024-03-25 17:21:29.645740 maptasker-4.0.5/maptasker/src/taskerd.py
+-rw-r--r--   0        0        0     2673 2024-04-22 17:26:35.341286 maptasker-4.0.5/maptasker/src/taskflag.py
+-rw-r--r--   0        0        0    23587 2024-05-07 14:51:54.100865 maptasker-4.0.5/maptasker/src/tasks.py
+-rw-r--r--   0        0        0    10000 2024-05-07 14:51:54.101209 maptasker-4.0.5/maptasker/src/taskuniq.py
+-rw-r--r--   0        0        0     2100 2024-02-20 15:01:50.903000 maptasker-4.0.5/maptasker/src/twisty.py
+-rw-r--r--   0        0        0   110257 2024-05-14 15:27:33.349930 maptasker-4.0.5/maptasker/src/userintr.py
+-rw-r--r--   0        0        0    10580 2024-05-13 18:56:54.744700 maptasker-4.0.5/maptasker/src/xmldata.py
+-rw-r--r--   0        0        0     5077 2024-05-14 19:04:41.755783 maptasker-4.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 maptasker-4.0.5/PKG-INFO
```

### Comparing `maptasker-4.0.2/LICENSE.txt` & `maptasker-4.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/README_PyPl.md` & `maptasker-4.0.5/README_PyPl.md`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/assets/Thumbs.db` & `maptasker-4.0.5/maptasker/assets/Thumbs.db`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/assets/maptasker_logo_dark.png` & `maptasker-4.0.5/maptasker/assets/maptasker_logo_dark.png`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/assets/maptasker_logo_light.png` & `maptasker-4.0.5/maptasker/assets/maptasker_logo_light.png`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/main.py` & `maptasker-4.0.5/maptasker/main.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/actargs.py` & `maptasker-4.0.5/maptasker/src/actargs.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/action.py` & `maptasker-4.0.5/maptasker/src/action.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/actionc.py` & `maptasker-4.0.5/maptasker/src/actionc.py`

 * *Files 0% similar despite different names*

```diff
@@ -2577,37 +2577,48 @@
         "New Package",
         ["0", "1"],
         [",Name=", ", Package="],
     ),
     "450t": ActionCode(0, "", [], [], "APN Droid", [], []),
     "451e": ActionCode(1, "", ["0"], ["Str"], "Package Removed", ["0"], ["Package="]),
     "451t": ActionCode(1, "", ["0"], ["Int"], "Music Skip", ["0"], ["Jump="]),
+    "452t": ActionCode(0, "", [], [], "Show Running Tasks", [], []),
     "453e": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Package Updated",
         ["0", "1"],
         ["Name=", ", Package="],
     ),
     "453t": ActionCode(1, "", ["0"], ["Int"], "Music Back", ["0"], ["Jump="]),
+    "454t": ActionCode(0, "", [], [], "Show Active Profiles", [], []),
     "455t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Int", "Int", "Int", "Int"],
         "Record Audio",
         ["0", "1", "2", "3"],
         ["File=", [", Source=", "l", "455"], ", MaxSize=", [", Format=", "l", "455a"]],
     ),
-    "456t": ActionCode(0, "", [], [], "JD APN", [], []),
+    "456t": ActionCode(0, "", ["0", "1", "2", "3", "4"], [], "JD APN", [], []),
     "457t": ActionCode(0, "", [], [], "Default Ringtone", [], []),
     "458t": ActionCode(0, "", [], [], "WidgetLocker", [], []),
     "459t": ActionCode(1, "", ["0"], ["Str"], "Scan Media", ["0"], ["File="]),
+    "460t": ActionCode(
+        4,
+        "",
+        ["0", "1", "2", "3"],
+        ["Bundle", "Int", "Int", "Int"],
+        "Set Device Effects",
+        ["1", "2", "3"],
+        [["", "e", ", 'Grayscale' On"], ["", "e", ", 'Wallpaper' On"], ["", "e", ", 'Disable Always On Display' On"]],
+    ),
     "460e": ActionCode(0, "", [], [], "Wallpaper Changed", [], []),
     "461e": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["App", "Str", "Str", "Str", "Str", "Str", "Str", "Int"],
         "Notification",
```

### Comparing `maptasker-4.0.2/maptasker/src/actiond.py` & `maptasker-4.0.5/maptasker/src/actiond.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/actione.py` & `maptasker-4.0.5/maptasker/src/actione.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/actionr.py` & `maptasker-4.0.5/maptasker/src/actionr.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/actiont.py` & `maptasker-4.0.5/maptasker/src/actiont.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/addcss.py` & `maptasker-4.0.5/maptasker/src/addcss.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/caveats.py` & `maptasker-4.0.5/maptasker/src/caveats.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/clip.py` & `maptasker-4.0.5/maptasker/src/clip.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/colors.py` & `maptasker-4.0.5/maptasker/src/colors.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/colrmode.py` & `maptasker-4.0.5/maptasker/src/colrmode.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/condition.py` & `maptasker-4.0.5/maptasker/src/condition.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/config.py` & `maptasker-4.0.5/maptasker/src/config.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/debug.py` & `maptasker-4.0.5/maptasker/src/debug.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/diagram.py` & `maptasker-4.0.5/maptasker/src/diagram.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/diagutil.py` & `maptasker-4.0.5/maptasker/src/diagutil.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/dirout.py` & `maptasker-4.0.5/maptasker/src/dirout.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,28 +261,28 @@
         # Find out if this Scene is in the single Project's Profile' we are looking for.
         # Get the Profile ID for the single Profile we are looking for
         for profile_id in PrimeItems.tasker_root_elements["all_profiles"]:
             if PrimeItems.tasker_root_elements["all_profiles"][profile_id]["name"] == profile_name:
                 found, project = find_task_in_project("", profile_id, "pids")
                 if found:
                     scenes = project.find("scenes")
-                    if scenes is not None and item["name"] in scenes.text.split(","):
+                    if scenes is not None and item[1] in scenes.text.split(","):
                         return True
 
         return False
     # Single Task?
     if (profile_name := PrimeItems.program_arguments["single_task_name"]) and (
         this_task_id := find_task_by_name(PrimeItems.program_arguments["single_task_name"])
     ):
         # Find the Project this single Task belongs to.
         found, project = find_task_in_project("", this_task_id, "tids")
         if found:
             # Found Project with Profile, now check If Scenes in Project
             scenes = project.find("scenes")
-            if scenes is not None and item["name"] in scenes.text.split(","):
+            if scenes is not None and item[1] in scenes.text.split(","):
                 return True
         return False
 
     # Not doing single name...Scene hyperlink is okay to include.
     return True
 
 
@@ -416,14 +416,16 @@
         None
     """
     # Output the table header
     if PrimeItems.directory_items[name]:
         # Go through each item and accumulate the names to be used for
         # the directory hyperlinks
         directory_hyperlinks = []
+        if name == "scenes":
+            print("dirout bingo")
         for item in PrimeItems.directory_items[name]:
             if check_item(name, item):
                 # Directory item is valid for this name.
                 # Get the name and display name for this item
                 hyperlink_name = item[0]
                 display_name = item[1]
                 # Append our hyperlink to this Project to the list
```

### Comparing `maptasker-4.0.2/maptasker/src/error.py` & `maptasker-4.0.5/maptasker/src/error.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/fonts.py` & `maptasker-4.0.5/maptasker/src/fonts.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/format.py` & `maptasker-4.0.5/maptasker/src/format.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/frontmtr.py` & `maptasker-4.0.5/maptasker/src/frontmtr.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/getbakup.py` & `maptasker-4.0.5/maptasker/src/getbakup.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/getids.py` & `maptasker-4.0.5/maptasker/src/getids.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/getputer.py` & `maptasker-4.0.5/maptasker/src/getputer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import tomli_w
 import tomllib
 
 from maptasker.src.colrmode import set_color_mode
 from maptasker.src.error import error_handler
 from maptasker.src.initparg import initialize_runtime_arguments
 from maptasker.src.primitem import PrimeItems
-from maptasker.src.sysconst import ARGUMENTS_FILE, NOW_TIME, OLD_ARGUMENTS_FILE
+from maptasker.src.sysconst import ARGUMENTS_FILE, NOW_TIME, OLD_ARGUMENTS_FILE, logger
 
 twenty_four_hours_ago = NOW_TIME - timedelta(hours=25)
 
 
 # ##################################################################################
 # Settings file is corrupt.  Let user know and reset colors to use and program arguments
 # ##################################################################################
@@ -106,15 +106,19 @@
     with open(new_file, "wb") as settings_file:
         tomli_w.dump(guidance, settings_file)
         settings_file.close()
 
     # Write out the program arguments in TOML format.  Open in binary append format (ab).
     with open(new_file, "ab") as settings_file:
         settings["program_arguments"] = dict(sorted(program_arguments.items()))  # Sort the program args first.
-        tomli_w.dump(settings, settings_file)
+        settings["colors_to_use"] = dict(sorted(colors_to_use.items()))  # Sort the colors first.
+        try:
+            tomli_w.dump(settings, settings_file)
+        except TypeError as e:
+            logger.debug(f"getputer tomli failure: {e}")
         settings_file.close()
 
 
 # ##################################################################################
 # Read in the TOML runtime settings
 # ##################################################################################
 def read_arguments(program_arguments: dict, colors_to_use: dict, old_file: str, new_file: str) -> None:
```

### Comparing `maptasker-4.0.2/maptasker/src/globalvr.py` & `maptasker-4.0.5/maptasker/src/globalvr.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/guiutils.py` & `maptasker-4.0.5/maptasker/src/guiutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,5224 +1,5680 @@
 00000000: 2222 2255 7469 6c69 7469 6573 2075 7365  """Utilities use
 00000010: 6420 6279 2047 5549 2222 220a 0a23 2120  d by GUI"""..#! 
 00000020: 2f75 7372 2f62 696e 2f65 6e76 2070 7974  /usr/bin/env pyt
-00000030: 686f 6e33 0a0a 2320 2323 2323 2323 2323  hon3..# ########
-00000040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000060: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000080: 2323 2323 2323 2323 2323 2323 2023 0a23  ############ #.#
-00000090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000000a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000030: 686f 6e33 0a0a 2320 2020 2020 2020 2020  hon3..#         
+00000040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000080: 2020 2020 2020 2020 2020 2020 2023 0a23               #.#
+00000090: 2067 7569 7574 696c 3a20 5574 696c 6974   guiutil: Utilit
+000000a0: 6965 7320 7573 6564 2062 7920 4755 4920  ies used by GUI 
 000000b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000000c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000000d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000000e0: 2020 2020 2020 230a 2320 6775 6975 7469        #.# guiuti
-000000f0: 6c3a 2055 7469 6c69 7469 6573 2075 7365  l: Utilities use
-00000100: 6420 6279 2047 5549 2020 2020 2020 2020  d by GUI        
+000000e0: 2020 2020 2020 230a 2320 2020 2020 2020        #.#       
+000000f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000110: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000120: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000130: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00000140: 0a23 2020 2020 2020 2020 2020 2020 2020  .#              
-00000150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000140: 0a23 2047 4e55 2047 656e 6572 616c 2050  .# GNU General P
+00000150: 7562 6c69 6320 4c69 6365 6e73 6520 7633  ublic License v3
+00000160: 2e30 2020 2020 2020 2020 2020 2020 2020  .0              
 00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000190: 2020 2020 2020 2020 230a 2320 474e 5520          #.# GNU 
-000001a0: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-000001b0: 6963 656e 7365 2076 332e 3020 2020 2020  icense v3.0     
-000001c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001f0: 2023 0a23 2050 6572 6d69 7373 696f 6e73   #.# Permissions
-00000200: 206f 6620 7468 6973 2073 7472 6f6e 6720   of this strong 
-00000210: 636f 7079 6c65 6674 206c 6963 656e 7365  copyleft license
-00000220: 2061 7265 2063 6f6e 6469 7469 6f6e 6564   are conditioned
-00000230: 206f 6e20 6d61 6b69 6e67 2061 7661 696c   on making avail
-00000240: 6162 6c65 2020 2020 2020 230a 2320 636f  able      #.# co
-00000250: 6d70 6c65 7465 2073 6f75 7263 6520 636f  mplete source co
-00000260: 6465 206f 6620 6c69 6365 6e73 6564 2077  de of licensed w
-00000270: 6f72 6b73 2061 6e64 206d 6f64 6966 6963  orks and modific
-00000280: 6174 696f 6e73 2c20 7768 6963 6820 696e  ations, which in
-00000290: 636c 7564 6520 6c61 7267 6572 2077 6f72  clude larger wor
-000002a0: 6b73 2023 0a23 2075 7369 6e67 2061 206c  ks #.# using a l
-000002b0: 6963 656e 7365 6420 776f 726b 2c20 756e  icensed work, un
-000002c0: 6465 7220 7468 6520 7361 6d65 206c 6963  der the same lic
-000002d0: 656e 7365 2e20 436f 7079 7269 6768 7420  ense. Copyright 
-000002e0: 616e 6420 6c69 6365 6e73 6520 6e6f 7469  and license noti
-000002f0: 6365 7320 6d75 7374 2062 6520 230a 2320  ces must be #.# 
-00000300: 7072 6573 6572 7665 642e 2043 6f6e 7472  preserved. Contr
-00000310: 6962 7574 6f72 7320 7072 6f76 6964 6520  ibutors provide 
-00000320: 616e 2065 7870 7265 7373 2067 7261 6e74  an express grant
-00000330: 206f 6620 7061 7465 6e74 2072 6967 6874   of patent right
-00000340: 732e 2020 2020 2020 2020 2020 2020 2020  s.              
-00000350: 2020 2020 2023 0a23 2023 2323 2323 2323       #.# #######
-00000360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000003a0: 2323 2323 2323 2323 2323 2323 2320 230a  ############# #.
-000003b0: 6672 6f6d 205f 5f66 7574 7572 655f 5f20  from __future__ 
-000003c0: 696d 706f 7274 2061 6e6e 6f74 6174 696f  import annotatio
-000003d0: 6e73 0a0a 696d 706f 7274 2063 6f6e 7465  ns..import conte
-000003e0: 7874 6c69 620a 696d 706f 7274 206f 730a  xtlib.import os.
-000003f0: 6672 6f6d 2074 6b69 6e74 6572 2069 6d70  from tkinter imp
-00000400: 6f72 7420 5463 6c45 7272 6f72 2c20 666f  ort TclError, fo
-00000410: 6e74 2c20 7474 6b0a 6672 6f6d 2074 7970  nt, ttk.from typ
-00000420: 696e 6720 696d 706f 7274 2054 5950 455f  ing import TYPE_
-00000430: 4348 4543 4b49 4e47 0a0a 696d 706f 7274  CHECKING..import
-00000440: 2063 7573 746f 6d74 6b69 6e74 6572 2061   customtkinter a
-00000450: 7320 6374 6b0a 6672 6f6d 2050 494c 2069  s ctk.from PIL i
-00000460: 6d70 6f72 7420 496d 6167 652c 2049 6d61  mport Image, Ima
-00000470: 6765 546b 0a0a 6672 6f6d 206d 6170 7461  geTk..from mapta
-00000480: 736b 6572 2e73 7263 2e63 6f6c 726d 6f64  sker.src.colrmod
-00000490: 6520 696d 706f 7274 2073 6574 5f63 6f6c  e import set_col
-000004a0: 6f72 5f6d 6f64 650a 6672 6f6d 206d 6170  or_mode.from map
-000004b0: 7461 736b 6572 2e73 7263 2e6c 696e 656f  tasker.src.lineo
-000004c0: 7574 2069 6d70 6f72 7420 4c69 6e65 4f75  ut import LineOu
-000004d0: 740a 6672 6f6d 206d 6170 7461 736b 6572  t.from maptasker
-000004e0: 2e73 7263 2e6d 6170 7574 696c 7320 696d  .src.maputils im
-000004f0: 706f 7274 2028 0a20 2020 2067 6574 5f70  port (.    get_p
-00000500: 7970 695f 7665 7273 696f 6e2c 0a20 2020  ypi_version,.   
-00000510: 2068 7474 705f 7265 7175 6573 742c 0a20   http_request,. 
-00000520: 2020 2076 616c 6964 6174 655f 6970 5f61     validate_ip_a
-00000530: 6464 7265 7373 2c0a 2020 2020 7661 6c69  ddress,.    vali
-00000540: 6461 7465 5f70 6f72 742c 0a20 2020 2076  date_port,.    v
-00000550: 616c 6964 6174 655f 786d 6c5f 6669 6c65  alidate_xml_file
-00000560: 2c0a 290a 6672 6f6d 206d 6170 7461 736b  ,.).from maptask
-00000570: 6572 2e73 7263 2e6e 616d 6561 7474 7220  er.src.nameattr 
-00000580: 696d 706f 7274 2067 6574 5f74 6b0a 6672  import get_tk.fr
-00000590: 6f6d 206d 6170 7461 736b 6572 2e73 7263  om maptasker.src
-000005a0: 2e70 7269 6d69 7465 6d20 696d 706f 7274  .primitem import
-000005b0: 2050 7269 6d65 4974 656d 730a 6672 6f6d   PrimeItems.from
-000005c0: 206d 6170 7461 736b 6572 2e73 7263 2e70   maptasker.src.p
-000005d0: 726f 6669 6c65 7320 696d 706f 7274 2067  rofiles import g
-000005e0: 6574 5f70 726f 6669 6c65 5f74 6173 6b73  et_profile_tasks
-000005f0: 0a66 726f 6d20 6d61 7074 6173 6b65 722e  .from maptasker.
-00000600: 7372 632e 7072 6f67 696e 6974 2069 6d70  src.proginit imp
-00000610: 6f72 7420 6765 745f 6461 7461 5f61 6e64  ort get_data_and
-00000620: 5f6f 7574 7075 745f 696e 7472 6f0a 6672  _output_intro.fr
-00000630: 6f6d 206d 6170 7461 736b 6572 2e73 7263  om maptasker.src
-00000640: 2e73 7973 636f 6e73 7420 696d 706f 7274  .sysconst import
-00000650: 2028 0a20 2020 2041 4e41 4c59 5349 535f   (.    ANALYSIS_
-00000660: 4649 4c45 2c0a 2020 2020 4348 414e 4745  FILE,.    CHANGE
-00000670: 4c4f 475f 4649 4c45 2c0a 2020 2020 4552  LOG_FILE,.    ER
-00000680: 524f 525f 4649 4c45 2c0a 2020 2020 4b45  ROR_FILE,.    KE
-00000690: 5946 494c 452c 0a20 2020 204c 4c41 4d41  YFILE,.    LLAMA
-000006a0: 5f4d 4f44 454c 532c 0a20 2020 204e 4f57  _MODELS,.    NOW
-000006b0: 5f54 494d 452c 0a20 2020 204f 5045 4e41  _TIME,.    OPENA
-000006c0: 495f 4d4f 4445 4c53 2c0a 2020 2020 5645  I_MODELS,.    VE
-000006d0: 5253 494f 4e2c 0a29 0a0a 6966 2054 5950  RSION,.)..if TYP
-000006e0: 455f 4348 4543 4b49 4e47 3a0a 2020 2020  E_CHECKING:.    
-000006f0: 6672 6f6d 2064 6174 6574 696d 6520 696d  from datetime im
-00000700: 706f 7274 2064 6174 6574 696d 650a 0a23  port datetime..#
-00000710: 2054 4f44 4f20 4368 616e 6765 2074 6869   TODO Change thi
-00000720: 7320 2763 6861 6e67 656c 6f67 2720 7769  s 'changelog' wi
-00000730: 7468 2065 6163 6820 7265 6c65 6173 6521  th each release!
-00000740: 2020 4e65 7720 6c69 6e65 7320 285c 6e29    New lines (\n)
-00000750: 206d 7573 7420 6265 2061 6464 6564 2e0a   must be added..
-00000760: 4348 414e 4745 4c4f 4720 3d20 2222 220a  CHANGELOG = """.
-00000770: 5665 7273 696f 6e20 342e 302f 342e 302e  Version 4.0/4.0.
-00000780: 312f 342e 302e 3220 2d20 284d 616a 6f72  1/4.0.2 - (Major
-00000790: 2920 4368 616e 6765 204c 6f67 5c6e 0a54  ) Change Log\n.T
-000007a0: 6869 7320 7665 7273 696f 6e20 696e 7472  his version intr
-000007b0: 6f64 7563 6573 2041 6920 416e 616c 7973  oduces Ai Analys
-000007c0: 6973 2e5c 6e0a 2323 2041 6464 6564 5c6e  is.\n.## Added\n
-000007d0: 0a2d 2041 6464 6564 3a20 4169 2061 6e61  .- Added: Ai ana
-000007e0: 6c79 7369 7320 7375 7070 6f72 7420 666f  lysis support fo
-000007f0: 7220 5072 6f66 696c 6573 2061 6e64 2054  r Profiles and T
-00000800: 6173 6b73 3a20 626f 7468 2043 6861 7447  asks: both ChatG
-00000810: 5054 2028 7365 7276 6572 2d62 6173 6564  PT (server-based
-00000820: 2920 616e 6420 284f 296c 6c61 6d61 2028  ) and (O)llama (
-00000830: 6c6f 6361 6c2d 6261 7365 6429 2e20 2053  local-based).  S
-00000840: 6565 2027 416e 616c 797a 6527 2074 6162  ee 'Analyze' tab
-00000850: 2e5c 6e0a 2d20 4164 6465 643a 2044 6973  .\n.- Added: Dis
-00000860: 706c 6179 2074 6865 2063 7572 7265 6e74  play the current
-00000870: 2066 696c 6520 696e 2047 5549 2e5c 6e0a   file in GUI.\n.
-00000880: 2d20 4164 6465 643a 2041 206e 6577 2027  - Added: A new '
-00000890: 4765 7420 4c6f 6361 6c20 584d 4c27 2062  Get Local XML' b
-000008a0: 7574 746f 6e20 6861 7320 6265 656e 2061  utton has been a
-000008b0: 6464 6564 2074 6f20 656e 6162 6c65 2074  dded to enable t
-000008c0: 6865 2047 5549 2074 6f20 6765 7420 7468  he GUI to get th
-000008d0: 6520 6c6f 6361 6c20 584d 4c20 6669 6c65  e local XML file
-000008e0: 2061 6e64 2076 616c 6964 6174 6520 6974   and validate it
-000008f0: 2066 6f72 2061 6e61 6c79 7369 732e 5c6e   for analysis.\n
-00000900: 0a2d 2041 6464 6564 3a20 4365 6e74 6572  .- Added: Center
-00000910: 2074 6865 2047 5549 2077 696e 646f 7720   the GUI window 
-00000920: 6f6e 2074 6865 2073 6372 6565 6e2e 5c6e  on the screen.\n
-00000930: 0a2d 2041 6464 6564 3a20 4120 706f 7075  .- Added: A popu
-00000940: 7020 7769 6e64 6f77 2077 696c 6c20 6469  p window will di
-00000950: 7370 6c61 7920 7768 656e 2061 6e61 6c79  splay when analy
-00000960: 7369 7320 6973 2072 756e 6e69 6e67 2069  sis is running i
-00000970: 6e20 7468 6520 6261 636b 6772 6f75 6e64  n the background
-00000980: 2e5c 6e0a 2323 2043 6861 6e67 6564 5c6e  .\n.## Changed\n
-00000990: 0a2d 2043 6861 6e67 6564 3a20 4755 4920  .- Changed: GUI 
-000009a0: 636f 6c6f 7220 7365 7474 696e 6773 2061  color settings a
-000009b0: 7265 206e 6f77 2064 6973 706c 6179 6564  re now displayed
-000009c0: 2069 6e20 7468 6569 7220 636f 6c6f 7273   in their colors
-000009d0: 206f 6e20 7468 6520 7374 6172 7475 7020   on the startup 
-000009e0: 6f66 2074 6865 2047 5549 2e5c 6e0a 2d20  of the GUI.\n.- 
-000009f0: 4368 616e 6765 643a 2047 5549 2077 6172  Changed: GUI war
-00000a00: 6e69 6e67 206d 6573 7361 6765 7320 6172  ning messages ar
-00000a10: 6520 6e6f 7720 6469 7370 6c61 7965 6420  e now displayed 
-00000a20: 696e 206f 7261 6e67 6520 7261 7468 6572  in orange rather
-00000a30: 2074 6861 6e20 7265 642e 5c6e 0a23 2320   than red.\n.## 
-00000a40: 4669 7865 645c 6e0a 2d20 4669 7865 643a  Fixed\n.- Fixed:
-00000a50: 2054 6865 2070 726f 6772 616d 2067 6574   The program get
-00000a60: 7320 7275 6e74 696d 6520 6572 726f 7273  s runtime errors
-00000a70: 2069 6620 7468 6520 7365 7474 696e 6773   if the settings
-00000a80: 2073 6176 6564 2066 696c 6520 6973 2063   saved file is c
-00000a90: 6f72 7275 7074 6564 2e5c 6e0a 2d20 4669  orrupted.\n.- Fi
-00000aa0: 7865 643a 2054 6865 2073 6574 7469 6e67  xed: The setting
-00000ab0: 7320 6172 6520 6e6f 7420 7072 6f70 6572  s are not proper
-00000ac0: 6c79 2073 6176 6564 2075 706f 6e20 6578  ly saved upon ex
-00000ad0: 6974 2066 726f 6d20 7468 6520 4755 492e  it from the GUI.
-00000ae0: 5c6e 0a2d 2046 6978 6564 3a20 5265 6d6f  \n.- Fixed: Remo
-00000af0: 7665 6420 6572 726f 7220 6d65 7373 6167  ved error messag
-00000b00: 6520 2750 726f 6772 616d 2063 616e 6365  e 'Program cance
-00000b10: 6c65 6420 6279 2075 7365 7220 286b 696c  led by user (kil
-00000b20: 6c65 6420 4755 4929 2720 6966 2074 6865  led GUI)' if the
-00000b30: 2027 4578 6974 2720 6275 7474 6f6e 2069   'Exit' button i
-00000b40: 7320 7365 6c65 6374 6564 2e5c 6e0a 2d20  s selected.\n.- 
-00000b50: 4669 7865 643a 2049 6620 7468 6520 416e  Fixed: If the An
-00000b60: 6472 6f69 6420 6669 6c65 206c 6f63 6174  droid file locat
-00000b70: 696f 6e20 6973 2073 7065 6369 6669 6564  ion is specified
-00000b80: 206f 6e20 7374 6172 7475 7020 616e 6420   on startup and 
-00000b90: 7468 6520 6669 6c65 2069 7320 666f 756e  the file is foun
-00000ba0: 6420 6f6e 2074 6865 206c 6f63 616c 2064  d on the local d
-00000bb0: 7269 7665 2066 726f 6d20 7468 6520 7072  rive from the pr
-00000bc0: 6576 696f 7573 2072 756e 2c20 7468 656e  evious run, then
-00000bd0: 2075 7365 2069 7420 616e 6420 646f 6e27   use it and don'
-00000be0: 7420 7072 6f6d 7074 2061 6761 696e 2066  t prompt again f
-00000bf0: 6f72 2069 742e 5c6e 0a2d 2046 6978 6564  or it.\n.- Fixed
-00000c00: 3a20 5468 6520 584d 4c20 6f62 7461 696e  : The XML obtain
-00000c10: 6564 2076 6961 2074 6865 2027 4765 7420  ed via the 'Get 
-00000c20: 4c6f 6361 6c20 584d 4c27 2062 7574 746f  Local XML' butto
-00000c30: 6e20 6973 206e 6f74 2073 6176 6564 2069  n is not saved i
-00000c40: 6e20 7468 6520 7365 7474 696e 6773 2e5c  n the settings.\
-00000c50: 6e0a 2d20 4669 7865 643a 2041 2072 6573  n.- Fixed: A res
-00000c60: 746f 7265 6420 584d 4c20 6669 6c65 206e  tored XML file n
-00000c70: 616d 6520 6261 7365 6420 6f6e 2073 6176  ame based on sav
-00000c80: 6564 2073 6574 7469 6e67 7320 6973 206e  ed settings is n
-00000c90: 6f74 2062 6569 6e67 2064 6973 706c 6179  ot being display
-00000ca0: 6564 2069 6e20 7468 6520 4755 492e 5c6e  ed in the GUI.\n
-00000cb0: 0a2d 2046 6978 6564 3a20 5072 6f70 6572  .- Fixed: Proper
-00000cc0: 6c79 2074 6572 6d69 6e61 7465 2074 6865  ly terminate the
-00000cd0: 2070 726f 6772 616d 2069 6620 7468 6520   program if the 
-00000ce0: 4755 4920 7769 6e64 6f77 2069 7320 636c  GUI window is cl
-00000cf0: 6f73 6564 2e5c 6e0a 2d20 4669 7865 643a  osed.\n.- Fixed:
-00000d00: 2054 6865 2047 5549 2773 2027 4170 7065   The GUI's 'Appe
-00000d10: 6172 616e 6365 204d 6f64 6527 2c20 2754  arance Mode', 'T
-00000d20: 7265 6520 5669 6577 2720 616e 6420 2752  ree View' and 'R
-00000d30: 6573 6574 2720 6275 7474 6f6e 7320 6469  eset' buttons di
-00000d40: 7361 7070 6561 7265 642e 5c6e 0a22 2222  sappeared.\n."""
-00000d50: 0a64 6566 6175 6c74 5f66 6f6e 745f 7369  .default_font_si
-00000d60: 7a65 203d 2031 340a 0a23 2053 6574 2075  ze = 14..# Set u
-00000d70: 7020 666f 7220 6163 6365 7373 2074 6f20  p for access to 
-00000d80: 6963 6f6e 730a 4355 5252 454e 545f 5041  icons.CURRENT_PA
-00000d90: 5448 203d 206f 732e 7061 7468 2e64 6972  TH = os.path.dir
-00000da0: 6e61 6d65 286f 732e 7061 7468 2e72 6561  name(os.path.rea
-00000db0: 6c70 6174 6828 5f5f 6669 6c65 5f5f 2929  lpath(__file__))
-00000dc0: 0a49 434f 4e5f 4449 5220 3d20 6f73 2e70  .ICON_DIR = os.p
-00000dd0: 6174 682e 6a6f 696e 2843 5552 5245 4e54  ath.join(CURRENT
-00000de0: 5f50 4154 482c 2022 2e2e 2f61 7373 6574  _PATH, "../asset
-00000df0: 7322 2c20 2269 636f 6e73 2229 0a49 434f  s", "icons").ICO
-00000e00: 4e5f 5041 5448 203d 207b 0a20 2020 2022  N_PATH = {.    "
-00000e10: 636c 6f73 6522 3a20 286f 732e 7061 7468  close": (os.path
-00000e20: 2e6a 6f69 6e28 4943 4f4e 5f44 4952 2c20  .join(ICON_DIR, 
-00000e30: 2263 6c6f 7365 5f62 6c61 636b 2e70 6e67  "close_black.png
-00000e40: 2229 2c20 6f73 2e70 6174 682e 6a6f 696e  "), os.path.join
-00000e50: 2849 434f 4e5f 4449 522c 2022 636c 6f73  (ICON_DIR, "clos
-00000e60: 655f 7768 6974 652e 706e 6722 2929 2c0a  e_white.png")),.
-00000e70: 2020 2020 2320 2269 6d61 6765 7322 3a20      # "images": 
-00000e80: 6c69 7374 286f 732e 7061 7468 2e6a 6f69  list(os.path.joi
-00000e90: 6e28 4943 4f4e 5f44 4952 2c20 6622 696d  n(ICON_DIR, f"im
-00000ea0: 6167 657b 697d 2e6a 7067 2229 2066 6f72  age{i}.jpg") for
-00000eb0: 2069 2069 6e20 7261 6e67 6528 312c 2034   i in range(1, 4
-00000ec0: 2929 2c0a 2020 2020 2265 7965 3122 3a20  )),.    "eye1": 
-00000ed0: 286f 732e 7061 7468 2e6a 6f69 6e28 4943  (os.path.join(IC
-00000ee0: 4f4e 5f44 4952 2c20 2265 7965 315f 626c  ON_DIR, "eye1_bl
-00000ef0: 6163 6b2e 706e 6722 292c 206f 732e 7061  ack.png"), os.pa
-00000f00: 7468 2e6a 6f69 6e28 4943 4f4e 5f44 4952  th.join(ICON_DIR
-00000f10: 2c20 2265 7965 315f 7768 6974 652e 706e  , "eye1_white.pn
-00000f20: 6722 2929 2c0a 2020 2020 2265 7965 3222  g")),.    "eye2"
-00000f30: 3a20 286f 732e 7061 7468 2e6a 6f69 6e28  : (os.path.join(
-00000f40: 4943 4f4e 5f44 4952 2c20 2265 7965 325f  ICON_DIR, "eye2_
-00000f50: 626c 6163 6b2e 706e 6722 292c 206f 732e  black.png"), os.
-00000f60: 7061 7468 2e6a 6f69 6e28 4943 4f4e 5f44  path.join(ICON_D
-00000f70: 4952 2c20 2265 7965 325f 7768 6974 652e  IR, "eye2_white.
-00000f80: 706e 6722 2929 2c0a 2020 2020 2269 6e66  png")),.    "inf
-00000f90: 6f22 3a20 6f73 2e70 6174 682e 6a6f 696e  o": os.path.join
-00000fa0: 2849 434f 4e5f 4449 522c 2022 696e 666f  (ICON_DIR, "info
-00000fb0: 2e70 6e67 2229 2c0a 2020 2020 2277 6172  .png"),.    "war
-00000fc0: 6e69 6e67 223a 206f 732e 7061 7468 2e6a  ning": os.path.j
-00000fd0: 6f69 6e28 4943 4f4e 5f44 4952 2c20 2277  oin(ICON_DIR, "w
-00000fe0: 6172 6e69 6e67 2e70 6e67 2229 2c0a 2020  arning.png"),.  
-00000ff0: 2020 2265 7272 6f72 223a 206f 732e 7061    "error": os.pa
-00001000: 7468 2e6a 6f69 6e28 4943 4f4e 5f44 4952  th.join(ICON_DIR
-00001010: 2c20 2265 7272 6f72 2e70 6e67 2229 2c0a  , "error.png"),.
-00001020: 2020 2020 226c 6566 7422 3a20 6f73 2e70      "left": os.p
-00001030: 6174 682e 6a6f 696e 2849 434f 4e5f 4449  ath.join(ICON_DI
-00001040: 522c 2022 6c65 6674 2e70 6e67 2229 2c0a  R, "left.png"),.
-00001050: 2020 2020 2272 6967 6874 223a 206f 732e      "right": os.
-00001060: 7061 7468 2e6a 6f69 6e28 4943 4f4e 5f44  path.join(ICON_D
-00001070: 4952 2c20 2272 6967 6874 2e70 6e67 2229  IR, "right.png")
-00001080: 2c0a 2020 2020 2277 6172 6e69 6e67 3222  ,.    "warning2"
-00001090: 3a20 6f73 2e70 6174 682e 6a6f 696e 2849  : os.path.join(I
-000010a0: 434f 4e5f 4449 522c 2022 7761 726e 696e  CON_DIR, "warnin
-000010b0: 6732 2e70 6e67 2229 2c0a 2020 2020 226c  g2.png"),.    "l
-000010c0: 6f61 6465 7222 3a20 6f73 2e70 6174 682e  oader": os.path.
-000010d0: 6a6f 696e 2849 434f 4e5f 4449 522c 2022  join(ICON_DIR, "
-000010e0: 6c6f 6164 6572 2e67 6966 2229 2c0a 2020  loader.gif"),.  
-000010f0: 2020 2269 636f 6e22 3a20 6f73 2e70 6174    "icon": os.pat
-00001100: 682e 6a6f 696e 2849 434f 4e5f 4449 522c  h.join(ICON_DIR,
-00001110: 2022 6963 6f6e 2e70 6e67 2229 2c0a 2020   "icon.png"),.  
-00001120: 2020 2261 7272 6f77 223a 206f 732e 7061    "arrow": os.pa
-00001130: 7468 2e6a 6f69 6e28 4943 4f4e 5f44 4952  th.join(ICON_DIR
-00001140: 2c20 2261 7272 6f77 2e70 6e67 2229 2c0a  , "arrow.png"),.
-00001150: 2020 2020 2269 6d61 6765 223a 206f 732e      "image": os.
-00001160: 7061 7468 2e6a 6f69 6e28 4943 4f4e 5f44  path.join(ICON_D
-00001170: 4952 2c20 2269 6d61 6765 2e70 6e67 2229  IR, "image.png")
-00001180: 2c0a 7d0a 0a0a 2320 2323 2323 2323 2323  ,.}...# ########
-00001190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000011a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000011b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000011c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000011d0: 2323 2323 2323 2323 2323 0a23 204d 616b  ##########.# Mak
-000011e0: 6520 7375 7265 2074 6865 2073 696e 676c  e sure the singl
-000011f0: 6520 6e61 6d65 6420 6974 656d 2065 7869  e named item exi
-00001200: 7374 732e 2e2e 7468 6174 2069 7420 6973  sts...that it is
-00001210: 2061 2076 616c 6964 206e 616d 650a 2320   a valid name.# 
-00001220: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001260: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001270: 2323 0a64 6566 2076 616c 6964 5f69 7465  ##.def valid_ite
-00001280: 6d28 7365 6c66 2c20 7468 655f 6e61 6d65  m(self, the_name
-00001290: 3a20 7374 722c 2065 6c65 6d65 6e74 5f6e  : str, element_n
-000012a0: 616d 653a 2073 7472 2c20 6465 6275 673a  ame: str, debug:
-000012b0: 2062 6f6f 6c2c 2061 7070 6561 7261 6e63   bool, appearanc
-000012c0: 655f 6d6f 6465 3a20 7374 7229 202d 3e20  e_mode: str) -> 
-000012d0: 626f 6f6c 3a20 2023 206e 6f71 613a 2041  bool:  # noqa: A
-000012e0: 4e4e 3030 310a 2020 2020 2222 220a 2020  NN001.    """.  
-000012f0: 2020 4368 6563 6b73 2069 6620 616e 2069    Checks if an i
-00001300: 7465 6d20 6e61 6d65 2069 7320 7661 6c69  tem name is vali
-00001310: 640a 2020 2020 4172 6773 3a0a 2020 2020  d.    Args:.    
-00001320: 2020 2020 7468 655f 6e61 6d65 3a20 5374      the_name: St
-00001330: 7269 6e67 202d 204e 616d 6520 746f 2063  ring - Name to c
-00001340: 6865 636b 0a20 2020 2020 2020 2065 6c65  heck.        ele
-00001350: 6d65 6e74 5f6e 616d 653a 2053 7472 696e  ment_name: Strin
-00001360: 6720 2d20 456c 656d 656e 7420 7479 7065  g - Element type
-00001370: 2062 6569 6e67 2063 6865 636b 6564 0a20   being checked. 
-00001380: 2020 2020 2020 2064 6562 7567 3a20 626f         debug: bo
-00001390: 6f6c 6561 6e20 2d20 4755 4920 6465 6275  olean - GUI debu
-000013a0: 6720 6d6f 6465 2054 7275 6520 6f72 2046  g mode True or F
-000013b0: 616c 7365 0a20 2020 2020 2020 2061 7070  alse.        app
-000013c0: 6561 7261 6e63 655f 6d6f 6465 3a20 5374  earance_mode: St
-000013d0: 7269 6e67 202d 204c 6967 6874 2f44 6172  ring - Light/Dar
-000013e0: 6b2f 5379 7374 656d 0a20 2020 2052 6574  k/System.    Ret
-000013f0: 7572 6e73 3a0a 2020 2020 2020 2020 426f  urns:.        Bo
-00001400: 6f6c 6561 6e20 2d20 5768 6574 6865 7220  olean - Whether 
-00001410: 7468 6520 6e61 6d65 2069 7320 7661 6c69  the name is vali
-00001420: 640a 2020 2020 5072 6f63 6573 7369 6e67  d.    Processing
-00001430: 204c 6f67 6963 3a0a 2020 2020 2d20 496e   Logic:.    - In
-00001440: 6974 6961 6c69 7a65 2074 656d 706f 7261  itialize tempora
-00001450: 7279 2070 7269 6d61 7279 2069 7465 6d73  ry primary items
-00001460: 206f 626a 6563 740a 2020 2020 2d20 4765   object.    - Ge
-00001470: 7420 6261 636b 7570 2078 6d6c 2064 6174  t backup xml dat
-00001480: 6120 616e 6420 726f 6f74 2065 6c65 6d65  a and root eleme
-00001490: 6e74 730a 2020 2020 2d20 4d61 7463 6820  nts.    - Match 
-000014a0: 656c 656d 656e 7420 7479 7065 2061 6e64  element type and
-000014b0: 2067 6574 2063 6f72 7265 7370 6f6e 6469   get correspondi
-000014c0: 6e67 2072 6f6f 7420 656c 656d 656e 740a  ng root element.
-000014d0: 2020 2020 2d20 4368 6563 6b20 6966 2069      - Check if i
-000014e0: 7465 6d20 6e61 6d65 2065 7869 7374 7320  tem name exists 
-000014f0: 6279 2067 6f69 6e67 2074 6872 6f75 6768  by going through
-00001500: 2061 6c6c 206e 616d 6573 2069 6e20 726f   all names in ro
-00001510: 6f74 2065 6c65 6d65 6e74 0a20 2020 2022  ot element.    "
-00001520: 2222 0a20 2020 2023 2053 6574 206f 7572  "".    # Set our
-00001530: 2066 696c 6520 746f 2067 6574 2074 6865   file to get the
-00001540: 2066 696c 6520 6672 6f6d 2074 6865 206c   file from the l
-00001550: 6f63 616c 2064 7269 7665 2073 696e 6365  ocal drive since
-00001560: 2069 7420 6861 6420 7072 6576 696f 7573   it had previous
-00001570: 6c79 2062 6565 6e20 7075 6c6c 6564 2066  ly been pulled f
-00001580: 726f 6d20 7468 6520 416e 6472 6f69 6420  rom the Android 
-00001590: 6465 7669 6365 2e0a 2020 2020 2320 5365  device..    # Se
-000015a0: 7474 696e 6720 5072 696d 6549 7465 6d73  tting PrimeItems
-000015b0: 2e70 726f 6772 616d 5f61 7267 756d 656e  .program_argumen
-000015c0: 7473 5b22 6669 6c65 225d 2077 696c 6c20  ts["file"] will 
-000015d0: 6265 2075 7365 6420 696e 2067 6574 5f78  be used in get_x
-000015e0: 6d6c 2829 2061 6e64 2077 6f6e 2774 2070  ml() and won't p
-000015f0: 726f 6d70 7420 666f 7220 6669 6c65 2069  rompt for file i
-00001600: 6620 6974 2065 7869 7374 732e 0a20 2020  f it exists..   
-00001610: 2066 696c 656e 616d 655f 6c6f 6361 7469   filename_locati
-00001620: 6f6e 203d 2073 656c 662e 616e 6472 6f69  on = self.androi
-00001630: 645f 6669 6c65 2e72 6669 6e64 2850 7269  d_file.rfind(Pri
-00001640: 6d65 4974 656d 732e 736c 6173 6829 202b  meItems.slash) +
-00001650: 2031 0a20 2020 2069 6620 6669 6c65 6e61   1.    if filena
-00001660: 6d65 5f6c 6f63 6174 696f 6e20 213d 2030  me_location != 0
-00001670: 3a0a 2020 2020 2020 2020 5072 696d 6549  :.        PrimeI
-00001680: 7465 6d73 2e70 726f 6772 616d 5f61 7267  tems.program_arg
-00001690: 756d 656e 7473 5b22 6669 6c65 225d 203d  uments["file"] =
-000016a0: 2073 656c 662e 616e 6472 6f69 645f 6669   self.android_fi
-000016b0: 6c65 5b66 696c 656e 616d 655f 6c6f 6361  le[filename_loca
-000016c0: 7469 6f6e 3a5d 0a20 2020 2065 6c69 6620  tion:].    elif 
-000016d0: 7365 6c66 2e66 696c 653a 0a20 2020 2020  self.file:.     
-000016e0: 2020 2050 7269 6d65 4974 656d 732e 7072     PrimeItems.pr
-000016f0: 6f67 7261 6d5f 6172 6775 6d65 6e74 735b  ogram_arguments[
-00001700: 2266 696c 6522 5d20 3d20 7365 6c66 2e66  "file"] = self.f
-00001710: 696c 650a 2020 2020 656c 7365 3a0a 2020  ile.    else:.  
-00001720: 2020 2020 2020 5f20 3d20 7365 6c66 2e70        _ = self.p
-00001730: 726f 6d70 745f 616e 645f 6765 745f 6669  rompt_and_get_fi
-00001740: 6c65 2873 656c 662e 6465 6275 672c 2073  le(self.debug, s
-00001750: 656c 662e 6170 7065 6172 616e 6365 5f6d  elf.appearance_m
-00001760: 6f64 6529 0a0a 2020 2020 2320 4765 7420  ode)..    # Get 
-00001770: 7468 6520 584d 4c20 6461 7461 0a20 2020  the XML data.   
-00001780: 2072 6574 7572 6e5f 636f 6465 203d 2067   return_code = g
-00001790: 6574 5f78 6d6c 2864 6562 7567 2c20 6170  et_xml(debug, ap
-000017a0: 7065 6172 616e 6365 5f6d 6f64 6529 0a0a  pearance_mode)..
-000017b0: 2020 2020 2320 4469 6420 7765 2067 6574      # Did we get
-000017c0: 2061 6e20 6572 726f 7220 7265 6164 696e   an error readin
-000017d0: 6720 7468 6520 6261 636b 7570 2066 696c  g the backup fil
-000017e0: 653f 0a20 2020 2069 6620 7265 7475 726e  e?.    if return
-000017f0: 5f63 6f64 6520 3e20 303a 0a20 2020 2020  _code > 0:.     
-00001800: 2020 2069 6620 7265 7475 726e 5f63 6f64     if return_cod
-00001810: 6520 3d3d 2036 3a0a 2020 2020 2020 2020  e == 6:.        
-00001820: 2020 2020 5072 696d 6549 7465 6d73 2e65      PrimeItems.e
-00001830: 7272 6f72 5f6d 7367 203d 2022 4361 6e63  rror_msg = "Canc
-00001840: 656c 2062 7574 746f 6e20 7072 6573 7365  el button presse
-00001850: 642e 220a 2020 2020 2020 2020 5072 696d  d.".        Prim
-00001860: 6549 7465 6d73 2e65 7272 6f72 5f63 6f64  eItems.error_cod
-00001870: 6520 3d20 300a 2020 2020 2020 2020 7265  e = 0.        re
-00001880: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
-00001890: 2320 5365 7420 7570 2066 6f72 206e 616d  # Set up for nam
-000018a0: 6520 6368 6563 6b69 6e67 0a20 2020 2023  e checking.    #
-000018b0: 2046 696e 6420 7468 6520 7370 6563 6966   Find the specif
-000018c0: 6963 2069 7465 6d20 616e 6420 6765 7420  ic item and get 
-000018d0: 6974 2773 2072 6f6f 7420 656c 656d 656e  it's root elemen
-000018e0: 740a 2020 2020 726f 6f74 5f65 6c65 6d65  t.    root_eleme
-000018f0: 6e74 5f63 686f 6963 6573 203d 207b 0a20  nt_choices = {. 
-00001900: 2020 2020 2020 2022 5072 6f6a 6563 7422         "Project"
-00001910: 3a20 5072 696d 6549 7465 6d73 2e74 6173  : PrimeItems.tas
-00001920: 6b65 725f 726f 6f74 5f65 6c65 6d65 6e74  ker_root_element
-00001930: 735b 2261 6c6c 5f70 726f 6a65 6374 7322  s["all_projects"
-00001940: 5d2c 0a20 2020 2020 2020 2022 5072 6f66  ],.        "Prof
-00001950: 696c 6522 3a20 5072 696d 6549 7465 6d73  ile": PrimeItems
-00001960: 2e74 6173 6b65 725f 726f 6f74 5f65 6c65  .tasker_root_ele
-00001970: 6d65 6e74 735b 2261 6c6c 5f70 726f 6669  ments["all_profi
-00001980: 6c65 7322 5d2c 0a20 2020 2020 2020 2022  les"],.        "
-00001990: 5461 736b 223a 2050 7269 6d65 4974 656d  Task": PrimeItem
-000019a0: 732e 7461 736b 6572 5f72 6f6f 745f 656c  s.tasker_root_el
-000019b0: 656d 656e 7473 5b22 616c 6c5f 7461 736b  ements["all_task
-000019c0: 7322 5d2c 0a20 2020 207d 0a20 2020 2072  s"],.    }.    r
-000019d0: 6f6f 745f 656c 656d 656e 7420 3d20 726f  oot_element = ro
-000019e0: 6f74 5f65 6c65 6d65 6e74 5f63 686f 6963  ot_element_choic
-000019f0: 6573 5b65 6c65 6d65 6e74 5f6e 616d 655d  es[element_name]
-00001a00: 0a0a 2020 2020 2320 5365 6520 6966 2074  ..    # See if t
-00001a10: 6865 2069 7465 6d20 6578 6973 7473 2062  he item exists b
-00001a20: 7920 676f 696e 6720 7468 726f 7567 6820  y going through 
-00001a30: 616c 6c20 6e61 6d65 730a 2020 2020 7265  all names.    re
-00001a40: 7475 726e 2061 6e79 2872 6f6f 745f 656c  turn any(root_el
-00001a50: 656d 656e 745b 6974 656d 5d5b 226e 616d  ement[item]["nam
-00001a60: 6522 5d20 3d3d 2074 6865 5f6e 616d 6520  e"] == the_name 
-00001a70: 666f 7220 6974 656d 2069 6e20 726f 6f74  for item in root
-00001a80: 5f65 6c65 6d65 6e74 290a 0a0a 2320 2323  _element)...# ##
-00001a90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001ab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001ac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001ad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001ae0: 0a23 2047 6574 2074 6865 2058 4d4c 2064  .# Get the XML d
-00001af0: 6174 6120 616e 6420 7365 7475 7020 5072  ata and setup Pr
-00001b00: 696d 6569 7465 6d73 0a23 2023 2323 2323  imeitems.# #####
-00001b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b50: 2323 2323 2323 2323 2323 2323 230a 6465  #############.de
-00001b60: 6620 6765 745f 786d 6c28 6465 6275 673a  f get_xml(debug:
-00001b70: 2062 6f6f 6c2c 2061 7070 6561 7261 6e63   bool, appearanc
-00001b80: 655f 6d6f 6465 3a20 7374 7229 202d 3e20  e_mode: str) -> 
-00001b90: 696e 743a 0a20 2020 2022 2222 2022 5265  int:.    """ "Re
-00001ba0: 7475 726e 7320 7468 6520 7461 736b 6572  turns the tasker
-00001bb0: 2072 6f6f 7420 786d 6c20 6974 656d 7320   root xml items 
-00001bc0: 6672 6f6d 2074 6865 2062 6163 6b75 7020  from the backup 
-00001bd0: 786d 6c20 6669 6c65 2062 6173 6564 206f  xml file based o
-00001be0: 6e20 7468 6520 6769 7665 6e20 6465 6275  n the given debu
-00001bf0: 6720 616e 6420 6170 7065 6172 616e 6365  g and appearance
-00001c00: 206d 6f64 6520 7061 7261 6d65 7465 7273   mode parameters
-00001c10: 2e22 0a20 2020 2050 6172 616d 6574 6572  .".    Parameter
-00001c20: 733a 0a20 2020 2020 2020 2064 6562 7567  s:.        debug
-00001c30: 2028 626f 6f6c 293a 2049 6e64 6963 6174   (bool): Indicat
-00001c40: 6573 2077 6865 7468 6572 2074 6865 2070  es whether the p
-00001c50: 726f 6772 616d 2069 7320 696e 2064 6562  rogram is in deb
-00001c60: 7567 206d 6f64 6520 6f72 206e 6f74 2e0a  ug mode or not..
-00001c70: 2020 2020 2020 2020 6170 7065 6172 616e          appearan
-00001c80: 6365 5f6d 6f64 6520 2873 7472 293a 2053  ce_mode (str): S
-00001c90: 7065 6369 6669 6573 2074 6865 2063 6f6c  pecifies the col
-00001ca0: 6f72 206d 6f64 6520 746f 2062 6520 7573  or mode to be us
-00001cb0: 6564 2e0a 2020 2020 5265 7475 726e 733a  ed..    Returns:
-00001cc0: 0a20 2020 2020 2020 2069 6e74 3a20 5468  .        int: Th
-00001cd0: 6520 7265 7475 726e 2063 6f64 6520 6672  e return code fr
-00001ce0: 6f6d 2067 6574 7469 6e67 2074 6865 2078  om getting the x
-00001cf0: 6d6c 2066 696c 652e 0a20 2020 2050 726f  ml file..    Pro
-00001d00: 6365 7373 696e 6720 4c6f 6769 633a 0a20  cessing Logic:. 
-00001d10: 2020 2020 2020 202d 2049 6e69 7469 616c         - Initial
-00001d20: 697a 6520 7465 6d70 6f72 6172 7920 5072  ize temporary Pr
-00001d30: 696d 6172 7949 7465 6d73 206f 626a 6563  imaryItems objec
-00001d40: 742e 0a20 2020 2020 2020 202d 2053 6574  t..        - Set
-00001d50: 2066 696c 655f 746f 5f67 6574 2076 6172   file_to_get var
-00001d60: 6961 626c 6520 6261 7365 6420 6f6e 2064  iable based on d
-00001d70: 6562 7567 206d 6f64 652e 0a20 2020 2020  ebug mode..     
-00001d80: 2020 202d 2053 6574 2070 726f 6772 616d     - Set program
-00001d90: 5f61 7267 756d 656e 7473 2076 6172 6961  _arguments varia
-00001da0: 626c 6520 666f 7220 6465 6275 6720 6d6f  ble for debug mo
-00001db0: 6465 2e0a 2020 2020 2020 2020 2d20 5365  de..        - Se
-00001dc0: 7420 636f 6c6f 7273 5f74 6f5f 7573 6520  t colors_to_use 
-00001dd0: 7661 7269 6162 6c65 2062 6173 6564 206f  variable based o
-00001de0: 6e20 6170 7065 6172 616e 6365 206d 6f64  n appearance mod
-00001df0: 652e 0a20 2020 2020 2020 202d 2049 6e69  e..        - Ini
-00001e00: 7469 616c 697a 6520 6f75 7470 7574 5f6c  tialize output_l
-00001e10: 696e 6573 2076 6172 6961 626c 652e 0a20  ines variable.. 
-00001e20: 2020 2020 2020 202d 2052 6574 7572 6e20         - Return 
-00001e30: 6461 7461 2061 6e64 206f 7574 7075 7420  data and output 
-00001e40: 696e 7472 6f2e 2222 220a 2020 2020 6966  intro.""".    if
-00001e50: 206e 6f74 2050 7269 6d65 4974 656d 732e   not PrimeItems.
-00001e60: 6669 6c65 5f74 6f5f 6765 743a 0a20 2020  file_to_get:.   
-00001e70: 2020 2020 2050 7269 6d65 4974 656d 732e       PrimeItems.
-00001e80: 6669 6c65 5f74 6f5f 6765 7420 3d20 2262  file_to_get = "b
-00001e90: 6163 6b75 702e 786d 6c22 2069 6620 6465  ackup.xml" if de
-00001ea0: 6275 6720 656c 7365 2022 220a 2020 2020  bug else "".    
-00001eb0: 5072 696d 6549 7465 6d73 2e70 726f 6772  PrimeItems.progr
-00001ec0: 616d 5f61 7267 756d 656e 7473 5b22 6465  am_arguments["de
-00001ed0: 6275 6722 5d20 3d20 6465 6275 670a 2020  bug"] = debug.  
-00001ee0: 2020 5072 696d 6549 7465 6d73 2e70 726f    PrimeItems.pro
-00001ef0: 6772 616d 5f61 7267 756d 656e 7473 5b22  gram_arguments["
-00001f00: 6775 6922 5d20 3d20 5472 7565 0a20 2020  gui"] = True.   
-00001f10: 2050 7269 6d65 4974 656d 732e 636f 6c6f   PrimeItems.colo
-00001f20: 7273 5f74 6f5f 7573 6520 3d20 7365 745f  rs_to_use = set_
-00001f30: 636f 6c6f 725f 6d6f 6465 2861 7070 6561  color_mode(appea
-00001f40: 7261 6e63 655f 6d6f 6465 290a 2020 2020  rance_mode).    
-00001f50: 5072 696d 6549 7465 6d73 2e6f 7574 7075  PrimeItems.outpu
-00001f60: 745f 6c69 6e65 7320 3d20 4c69 6e65 4f75  t_lines = LineOu
-00001f70: 7428 290a 0a20 2020 2072 6574 7572 6e20  t()..    return 
-00001f80: 6765 745f 6461 7461 5f61 6e64 5f6f 7574  get_data_and_out
-00001f90: 7075 745f 696e 7472 6f28 4661 6c73 6529  put_intro(False)
-00001fa0: 0a0a 0a23 2023 2323 2323 2323 2323 2323  ...# ###########
-00001fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001fc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001fd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001fe0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001ff0: 2323 2323 2323 230a 2320 4765 7420 616c  #######.# Get al
-00002000: 6c20 6d6f 6e6f 7370 6163 6520 666f 6e74  l monospace font
-00002010: 7320 6672 6f6d 2054 4b49 6e74 6572 0a23  s from TKInter.#
-00002020: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00002030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002060: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002070: 2323 230a 6465 6620 6765 745f 6d6f 6e6f  ###.def get_mono
-00002080: 5f66 6f6e 7473 2829 202d 3e20 4e6f 6e65  _fonts() -> None
-00002090: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-000020a0: 7475 726e 7320 6120 6469 6374 696f 6e61  turns a dictiona
-000020b0: 7279 206f 6620 6669 7865 642d 7769 6474  ry of fixed-widt
-000020c0: 6820 666f 6e74 730a 2020 2020 4172 6773  h fonts.    Args
-000020d0: 3a0a 2020 2020 2020 2020 7365 6c66 3a20  :.        self: 
-000020e0: 5468 6520 636c 6173 7320 696e 7374 616e  The class instan
-000020f0: 6365 0a20 2020 2052 6574 7572 6e73 3a0a  ce.    Returns:.
-00002100: 2020 2020 2020 2020 6469 6374 3a20 4120          dict: A 
-00002110: 6469 6374 696f 6e61 7279 206f 6620 6669  dictionary of fi
-00002120: 7865 642d 7769 6474 6820 666f 6e74 7320  xed-width fonts 
-00002130: 616e 6420 7468 6569 7220 6661 6d69 6c79  and their family
-00002140: 206e 616d 6573 0a20 2020 202d 2047 6574   names.    - Get
-00002150: 2061 6c6c 2061 7661 696c 6162 6c65 2066   all available f
-00002160: 6f6e 7473 2066 726f 6d20 7468 6520 666f  onts from the fo
-00002170: 6e74 206d 6f64 756c 650a 2020 2020 2d20  nt module.    - 
-00002180: 4669 6c74 6572 2066 6f6e 7473 2074 6f20  Filter fonts to 
-00002190: 6f6e 6c79 2074 686f 7365 2077 6974 6820  only those with 
-000021a0: 6120 6669 7865 6420 7769 6474 680a 2020  a fixed width.  
-000021b0: 2020 2d20 4275 696c 6420 6120 6469 6374    - Build a dict
-000021c0: 696f 6e61 7279 2077 6974 6820 666f 6e74  ionary with font
-000021d0: 206e 616d 6520 6173 206b 6579 2061 6e64   name as key and
-000021e0: 2066 616d 696c 7920 6173 2076 616c 7565   family as value
-000021f0: 0a20 2020 2022 2222 0a20 2020 2023 204d  .    """.    # M
-00002200: 616b 6520 7375 7265 2077 6520 6861 7665  ake sure we have
-00002210: 2074 6865 2054 6b69 6e74 6572 2077 696e   the Tkinter win
-00002220: 646f 772f 726f 6f74 0a20 2020 2067 6574  dow/root.    get
-00002230: 5f74 6b28 290a 2020 2020 666f 6e74 7320  _tk().    fonts 
-00002240: 3d20 5b66 6f6e 742e 466f 6e74 2866 616d  = [font.Font(fam
-00002250: 696c 793d 6629 2066 6f72 2066 2069 6e20  ily=f) for f in 
-00002260: 666f 6e74 2e66 616d 696c 6965 7328 295d  font.families()]
-00002270: 0a20 2020 2072 6574 7572 6e20 7b66 2e6e  .    return {f.n
-00002280: 616d 653a 2066 2e61 6374 7561 6c28 2266  ame: f.actual("f
-00002290: 616d 696c 7922 2920 666f 7220 6620 696e  amily") for f in
-000022a0: 2066 6f6e 7473 2069 6620 662e 6d65 7472   fonts if f.metr
-000022b0: 6963 7328 2266 6978 6564 2229 7d0a 0a0a  ics("fixed")}...
-000022c0: 2320 2323 2323 2323 2323 2323 2323 2323  # ##############
-000022d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000022e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000022f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002310: 2323 2323 0a23 2042 7569 6c64 206c 6973  ####.# Build lis
-00002320: 7420 6f66 2061 6c6c 2061 7661 696c 6162  t of all availab
-00002330: 6c65 206d 6f6e 6f73 7061 6365 2066 6f6e  le monospace fon
-00002340: 7473 0a23 2023 2323 2323 2323 2323 2323  ts.# ###########
-00002350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002390: 2323 2323 2323 230a 6465 6620 6765 745f  #######.def get_
-000023a0: 6d6f 6e6f 7370 6163 655f 666f 6e74 7328  monospace_fonts(
-000023b0: 2920 2d3e 2064 6963 743a 0a20 2020 2022  ) -> dict:.    "
-000023c0: 2222 0a20 2020 2052 6574 7572 6e73 206d  "".    Returns m
-000023d0: 6f6e 6f73 7061 6365 2066 6f6e 7473 2066  onospace fonts f
-000023e0: 726f 6d20 7379 7374 656d 2066 6f6e 7473  rom system fonts
-000023f0: 2e0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00002400: 2020 2020 666f 6e74 733a 2041 6c6c 2073      fonts: All s
-00002410: 7973 7465 6d20 666f 6e74 730a 2020 2020  ystem fonts.    
-00002420: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00002430: 2066 6f6e 745f 6974 656d 733a 204c 6973   font_items: Lis
-00002440: 7420 6f66 206d 6f6e 6f73 7061 6365 2066  t of monospace f
-00002450: 6f6e 7473 0a20 2020 2020 2020 2072 6573  onts.        res
-00002460: 3a20 4c69 7374 2063 6f6e 7461 696e 696e  : List containin
-00002470: 6720 436f 7572 6965 7220 6f72 2064 6566  g Courier or def
-00002480: 6175 6c74 204d 6f6e 6163 6f20 666f 6e74  ault Monaco font
-00002490: 0a20 2020 202d 2047 6574 2061 6c6c 2073  .    - Get all s
-000024a0: 7973 7465 6d20 666f 6e74 730a 2020 2020  ystem fonts.    
-000024b0: 2d20 4669 6c74 6572 2066 6f6e 7473 2074  - Filter fonts t
-000024c0: 6f20 6f6e 6c79 2069 6e63 6c75 6465 206d  o only include m
-000024d0: 6f6e 6f73 7061 6365 2066 6f6e 7473 2065  onospace fonts e
-000024e0: 7863 6c75 6469 6e67 2057 696e 6764 696e  xcluding Wingdin
-000024f0: 6773 0a20 2020 202d 2046 696e 6420 436f  gs.    - Find Co
-00002500: 7572 6965 7220 666f 6e74 2069 6e20 6c69  urier font in li
-00002510: 7374 2061 6e64 2073 6574 2061 7320 7265  st and set as re
-00002520: 730a 2020 2020 2d20 4966 2043 6f75 7269  s.    - If Couri
-00002530: 6572 206e 6f74 2066 6f75 6e64 2c20 7365  er not found, se
-00002540: 7420 4d6f 6e61 636f 2061 7320 6465 6661  t Monaco as defa
-00002550: 756c 7420 7265 730a 2020 2020 2d20 5265  ult res.    - Re
-00002560: 7475 726e 206c 6973 7473 206f 6620 6d6f  turn lists of mo
-00002570: 6e6f 7370 6163 6520 666f 6e74 7320 616e  nospace fonts an
-00002580: 6420 436f 7572 6965 722f 4d6f 6e61 636f  d Courier/Monaco
-00002590: 2066 6f6e 740a 2020 2020 2222 220a 2020   font.    """.  
-000025a0: 2020 666f 6e74 7320 3d20 6765 745f 6d6f    fonts = get_mo
-000025b0: 6e6f 5f66 6f6e 7473 2829 0a20 2020 2066  no_fonts().    f
-000025c0: 6f6e 745f 6974 656d 7320 3d20 5b22 436f  ont_items = ["Co
-000025d0: 7572 6965 7222 5d0a 2020 2020 666f 6e74  urier"].    font
-000025e0: 5f69 7465 6d73 203d 205b 7661 6c75 6520  _items = [value 
-000025f0: 666f 7220 7661 6c75 6520 696e 2066 6f6e  for value in fon
-00002600: 7473 2e76 616c 7565 7328 2920 6966 2022  ts.values() if "
-00002610: 5769 6e67 6469 6e67 7322 206e 6f74 2069  Wingdings" not i
-00002620: 6e20 7661 6c75 655d 0a20 2020 2023 2046  n value].    # F
-00002630: 696e 6420 7768 6963 6820 436f 7572 6965  ind which Courie
-00002640: 7220 666f 6e74 2069 7320 696e 206f 7572  r font is in our
-00002650: 206c 6973 7420 616e 6420 7365 742e 0a20   list and set.. 
-00002660: 2020 2072 6573 203d 205b 6920 666f 7220     res = [i for 
-00002670: 6920 696e 2066 6f6e 745f 6974 656d 7320  i in font_items 
-00002680: 6966 2022 436f 7572 6965 7222 2069 6e20  if "Courier" in 
-00002690: 695d 0a20 2020 2023 2049 6620 436f 7572  i].    # If Cour
-000026a0: 6965 7220 6973 206e 6f74 2066 6f75 6e64  ier is not found
-000026b0: 2066 6f72 2073 6f6d 6520 7265 6173 6f6e   for some reason
-000026c0: 2c20 6465 6661 756c 7420 746f 204d 6f6e  , default to Mon
-000026d0: 6163 6f0a 2020 2020 6966 206e 6f74 2072  aco.    if not r
-000026e0: 6573 3a0a 2020 2020 2020 2020 7265 7320  es:.        res 
-000026f0: 3d20 5b69 2066 6f72 2069 2069 6e20 666f  = [i for i in fo
-00002700: 6e74 5f69 7465 6d73 2069 6620 224d 6f6e  nt_items if "Mon
-00002710: 6163 6f22 2069 6e20 695d 0a20 2020 2072  aco" in i].    r
-00002720: 6574 7572 6e20 666f 6e74 5f69 7465 6d73  eturn font_items
-00002730: 2c20 7265 730a 0a0a 2320 2323 2323 2323  , res...# ######
-00002740: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002750: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002760: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002770: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002780: 2323 2323 2323 2323 2323 2323 0a23 2050  ############.# P
-00002790: 696e 6720 7468 6520 416e 6472 6f69 6420  ing the Android 
-000027a0: 6576 6963 6520 746f 206d 616b 6520 7375  evice to make su
-000027b0: 7265 2069 7420 6973 2072 6561 6368 6162  re it is reachab
-000027c0: 6c65 2e0a 2320 2323 2323 2323 2323 2323  le..# ##########
-000027d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000027e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000027f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002810: 2323 2323 2323 2323 0a64 6566 2070 696e  ########.def pin
-00002820: 675f 616e 6472 6f69 645f 6465 7669 6365  g_android_device
-00002830: 2873 656c 662c 2069 705f 6164 6472 6573  (self, ip_addres
-00002840: 733a 2073 7472 2c20 706f 7274 5f6e 756d  s: str, port_num
-00002850: 6265 723a 2073 7472 2920 2d3e 2062 6f6f  ber: str) -> boo
-00002860: 6c3a 2020 2320 6e6f 7161 3a20 414e 4e30  l:  # noqa: ANN0
-00002870: 3031 0a20 2020 2023 2054 6865 2066 6f6c  01.    # The fol
-00002880: 6c6f 7769 6e67 2073 686f 756c 6420 7265  lowing should re
-00002890: 7475 726e 2061 206c 6973 743a 205b 6970  turn a list: [ip
-000028a0: 5f61 6464 7265 7373 3a70 6f72 745f 6e75  _address:port_nu
-000028b0: 6d62 6572 2c20 6669 6c65 5f6c 6f63 6174  mber, file_locat
-000028c0: 696f 6e5d 0a20 2020 2022 2222 0a20 2020  ion].    """.   
-000028d0: 2050 696e 6773 2061 6e20 416e 6472 6f69   Pings an Androi
-000028e0: 6420 6465 7669 6365 0a20 2020 2041 7267  d device.    Arg
-000028f0: 733a 0a20 2020 2020 2020 2069 705f 6164  s:.        ip_ad
-00002900: 6472 6573 733a 2073 7472 202d 2054 4350  dress: str - TCP
-00002910: 2049 5020 6164 6472 6573 7320 6f66 2074   IP address of t
-00002920: 6865 2041 6e64 726f 6964 2064 6576 6963  he Android devic
-00002930: 650a 2020 2020 2020 2020 706f 7274 5f6e  e.        port_n
-00002940: 756d 6265 723a 2073 7472 202d 2054 4350  umber: str - TCP
-00002950: 2070 6f72 7420 6e75 6d62 6572 206f 6620   port number of 
-00002960: 7468 6520 416e 6472 6f69 6420 6465 7669  the Android devi
-00002970: 6365 0a20 2020 2052 6574 7572 6e3a 0a20  ce.    Return:. 
-00002980: 2020 2020 2020 2045 7272 6f72 3a20 5472         Error: Tr
-00002990: 7565 2069 6620 6572 726f 722c 2066 616c  ue if error, fal
-000029a0: 7365 2069 6620 616c 6c20 6973 2067 6f6f  se if all is goo
-000029b0: 642e 0a20 2020 2050 726f 6365 7373 696e  d..    Processin
-000029c0: 6720 4c6f 6769 633a 0a20 2020 202d 2053  g Logic:.    - S
-000029d0: 706c 6974 7320 7468 6520 6261 636b 7570  plits the backup
-000029e0: 5f69 6e66 6f20 7374 7269 6e67 2069 6e74  _info string int
-000029f0: 6f20 6970 5f61 6464 7265 7373 2c20 706f  o ip_address, po
-00002a00: 7274 5f6e 756d 6265 722c 2061 6e64 2066  rt_number, and f
-00002a10: 696c 655f 6c6f 6361 7469 6f6e 0a20 2020  ile_location.   
-00002a20: 202d 2056 616c 6964 6174 6573 2074 6865   - Validates the
-00002a30: 2049 5020 6164 6472 6573 732c 2070 6f72   IP address, por
-00002a40: 7420 6e75 6d62 6572 2c20 616e 6420 6669  t number, and fi
-00002a50: 6c65 206c 6f63 6174 696f 6e0a 2020 2020  le location.    
-00002a60: 2d20 5069 6e67 7320 7468 6520 4950 2061  - Pings the IP a
-00002a70: 6464 7265 7373 2074 6f20 6368 6563 6b20  ddress to check 
-00002a80: 636f 6e6e 6563 7469 7669 7479 0a20 2020  connectivity.   
-00002a90: 202d 2052 6574 7572 6e73 2061 2074 7570   - Returns a tup
-00002aa0: 6c65 2069 6e64 6963 6174 696e 6720 7375  le indicating su
-00002ab0: 6363 6573 732f 6661 696c 7572 6520 616e  ccess/failure an
-00002ac0: 6420 616e 7920 6572 726f 7220 6d65 7373  d any error mess
-00002ad0: 6167 650a 2020 2020 2222 220a 2020 2020  age.    """.    
-00002ae0: 2320 5661 6c69 6461 7465 2049 5020 4164  # Validate IP Ad
-00002af0: 6472 6573 730a 2020 2020 6966 2076 616c  dress.    if val
-00002b00: 6964 6174 655f 6970 5f61 6464 7265 7373  idate_ip_address
-00002b10: 2869 705f 6164 6472 6573 7329 3a0a 2020  (ip_address):.  
-00002b20: 2020 2020 2020 2320 5665 7269 6679 2074        # Verify t
-00002b30: 6861 7420 7468 6520 686f 7374 2049 5020  hat the host IP 
-00002b40: 6973 2072 6561 6368 6162 6c65 3a0a 2020  is reachable:.  
-00002b50: 2020 2020 2020 7365 6c66 2e64 6973 706c        self.displ
-00002b60: 6179 5f6d 6573 7361 6765 5f62 6f78 2866  ay_message_box(f
-00002b70: 2250 696e 6769 6e67 2061 6464 7265 7373  "Pinging address
-00002b80: 207b 6970 5f61 6464 7265 7373 7d2e 2020   {ip_address}.  
-00002b90: 506c 6561 7365 2077 6169 742e 2e2e 222c  Please wait...",
-00002ba0: 2022 4772 6565 6e22 290a 2020 2020 2020   "Green").      
-00002bb0: 2020 7365 6c66 2e75 7064 6174 6528 2920    self.update() 
-00002bc0: 2023 2046 6f72 6365 2061 2077 696e 646f   # Force a windo
-00002bd0: 7720 7265 6672 6573 682e 0a0a 2020 2020  w refresh...    
-00002be0: 2020 2020 2320 5069 6e67 2049 5020 6164      # Ping IP ad
-00002bf0: 6472 6573 732e 0a20 2020 2020 2020 2072  dress..        r
-00002c00: 6573 706f 6e73 6520 3d20 6f73 2e73 7973  esponse = os.sys
-00002c10: 7465 6d28 6622 7069 6e67 202d 6320 3120  tem(f"ping -c 1 
-00002c20: 2d74 3530 203e 202f 6465 762f 6e75 6c6c  -t50 > /dev/null
-00002c30: 207b 6970 5f61 6464 7265 7373 7d22 2920   {ip_address}") 
-00002c40: 2023 206e 6f71 613a 2053 3630 350a 2020   # noqa: S605.  
-00002c50: 2020 2020 2020 6966 2072 6573 706f 6e73        if respons
-00002c60: 6520 213d 2030 3a0a 2020 2020 2020 2020  e != 0:.        
-00002c70: 2020 2020 7365 6c66 2e62 6163 6b75 705f      self.backup_
-00002c80: 6572 726f 7228 0a20 2020 2020 2020 2020  error(.         
-00002c90: 2020 2020 2020 2066 227b 6970 5f61 6464         f"{ip_add
-00002ca0: 7265 7373 7d20 6973 206e 6f74 2072 6561  ress} is not rea
-00002cb0: 6368 6162 6c65 2028 6572 726f 7220 7b72  chable (error {r
-00002cc0: 6573 706f 6e73 657d 292e 2020 5472 7920  esponse}).  Try 
-00002cd0: 6167 6169 6e2e 222c 0a20 2020 2020 2020  again.",.       
-00002ce0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00002cf0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00002d00: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
-00002d10: 706c 6179 5f6d 6573 7361 6765 5f62 6f78  play_message_box
-00002d20: 2822 5069 6e67 2073 7563 6365 7373 6675  ("Ping successfu
-00002d30: 6c2e 222c 2022 4772 6565 6e22 290a 2020  l.", "Green").  
-00002d40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00002d50: 7365 6c66 2e62 6163 6b75 705f 6572 726f  self.backup_erro
-00002d60: 7228 0a20 2020 2020 2020 2020 2020 2066  r(.            f
-00002d70: 2249 6e76 616c 6964 2049 5020 6164 6472  "Invalid IP addr
-00002d80: 6573 733a 207b 6970 5f61 6464 7265 7373  ess: {ip_address
-00002d90: 7d2e 2020 5472 7920 6167 6169 6e2e 222c  }.  Try again.",
-00002da0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00002db0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00002dc0: 0a20 2020 2023 2056 616c 6964 6174 6520  .    # Validate 
-00002dd0: 706f 7274 206e 756d 6265 720a 2020 2020  port number.    
-00002de0: 6966 2076 616c 6964 6174 655f 706f 7274  if validate_port
-00002df0: 2869 705f 6164 6472 6573 732c 2070 6f72  (ip_address, por
-00002e00: 745f 6e75 6d62 6572 2920 213d 2030 3a0a  t_number) != 0:.
-00002e10: 2020 2020 2020 2020 7365 6c66 2e62 6163          self.bac
-00002e20: 6b75 705f 6572 726f 7228 0a20 2020 2020  kup_error(.     
-00002e30: 2020 2020 2020 2066 2249 6e76 616c 6964         f"Invalid
-00002e40: 2050 6f72 7420 6e75 6d62 6572 3a20 7b70   Port number: {p
-00002e50: 6f72 745f 6e75 6d62 6572 7d20 6f72 2074  ort_number} or t
-00002e60: 6865 2067 6976 656e 2049 5020 6164 6472  he given IP addr
-00002e70: 6573 7320 646f 6573 206e 6f74 2070 6572  ess does not per
-00002e80: 6d69 7420 6163 6365 7373 2074 6f20 7468  mit access to th
-00002e90: 6973 2070 6f72 742e 2020 5472 7920 6167  is port.  Try ag
-00002ea0: 6169 6e2e 222c 0a20 2020 2020 2020 2029  ain.",.        )
-00002eb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002ec0: 4661 6c73 650a 0a20 2020 2023 2056 616c  False..    # Val
-00002ed0: 6964 2049 5020 4164 6472 6573 732e 2e2e  id IP Address...
-00002ee0: 676f 6f64 2070 696e 672e 0a20 2020 2072  good ping..    r
-00002ef0: 6574 7572 6e20 5472 7565 0a0a 0a23 2023  eturn True...# #
-00002f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002f10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002f20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002f30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002f50: 230a 2320 436c 6561 7220 616c 6c20 6275  #.# Clear all bu
-00002f60: 7474 6f6e 7320 6173 736f 6369 6174 6564  ttons associated
-00002f70: 2077 6974 6820 6665 7463 6869 6e67 2074   with fetching t
-00002f80: 6865 2062 6163 6b75 7020 6669 6c65 2066  he backup file f
-00002f90: 726f 6d20 416e 6472 6f69 6420 6465 7669  rom Android devi
-00002fa0: 6365 0a23 2023 2323 2323 2323 2323 2323  ce.# ###########
-00002fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002fc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002fd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002fe0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002ff0: 2323 2323 2323 230a 6465 6620 636c 6561  #######.def clea
-00003000: 725f 616e 6472 6f69 645f 6275 7474 6f6e  r_android_button
-00003010: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
-00003020: 2020 2320 6e6f 7161 3a20 414e 4e30 3031    # noqa: ANN001
-00003030: 0a20 2020 2022 2222 0a20 2020 2043 6c65  .    """.    Cle
-00003040: 6172 7320 616e 6472 6f69 6420 6465 7669  ars android devi
-00003050: 6365 2063 6f6e 6669 6775 7261 7469 6f6e  ce configuration
-00003060: 2062 7574 746f 6e73 2061 6e64 2064 6973   buttons and dis
-00003070: 706c 6179 7320 6261 636b 7570 2062 7574  plays backup but
-00003080: 746f 6e0a 2020 2020 4172 6773 3a0a 2020  ton.    Args:.  
-00003090: 2020 2020 2020 7365 6c66 3a20 5468 6520        self: The 
-000030a0: 636c 6173 7320 696e 7374 616e 6365 0a20  class instance. 
-000030b0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-000030c0: 2020 2020 4e6f 6e65 0a20 2020 202d 2044      None.    - D
-000030d0: 6573 7472 6f79 7320 4950 2c20 706f 7274  estroys IP, port
-000030e0: 2c20 6669 6c65 2065 6e74 7279 2061 6e64  , file entry and
-000030f0: 206c 6162 656c 2077 6964 6765 7473 0a20   label widgets. 
-00003100: 2020 202d 2044 6573 7472 6f79 7320 6765     - Destroys ge
-00003110: 7420 6261 636b 7570 2062 7574 746f 6e0a  t backup button.
-00003120: 2020 2020 2d20 4469 7370 6c61 7973 206e      - Displays n
-00003130: 6577 2062 6163 6b75 7020 6275 7474 6f6e  ew backup button
-00003140: 2077 6974 6820 6361 6c6c 6261 636b 2074   with callback t
-00003150: 6f20 6765 745f 6261 636b 7570 5f65 7665  o get_backup_eve
-00003160: 6e74 206d 6574 686f 6422 2222 0a0a 2020  nt method"""..  
-00003170: 2020 2320 4561 6368 2065 6c65 6d65 6e74    # Each element
-00003180: 2074 6f20 6265 2064 6573 746f 7279 6564   to be destoryed
-00003190: 206e 6565 6473 2061 2073 7570 7072 6573   needs a suppres
-000031a0: 7369 6f6e 2073 696e 6365 2061 6e79 206f  sion since any o
-000031b0: 6e65 2073 7570 7072 6573 7369 6f6e 2077  ne suppression w
-000031c0: 696c 6c20 6265 2074 7269 6767 6572 6564  ill be triggered
-000031d0: 2069 6620 616e 7920 6f6e 6520 6f66 0a20   if any one of. 
-000031e0: 2020 2023 2074 6865 2065 6c65 6d65 6e74     # the element
-000031f0: 7320 6973 206e 6f74 2064 6566 696e 6564  s is not defined
-00003200: 2e0a 2020 2020 7769 7468 2063 6f6e 7465  ..    with conte
-00003210: 7874 6c69 622e 7375 7070 7265 7373 2841  xtlib.suppress(A
-00003220: 7474 7269 6275 7465 4572 726f 7229 3a0a  ttributeError):.
-00003230: 2020 2020 2020 2020 7365 6c66 2e69 705f          self.ip_
-00003240: 656e 7472 792e 6465 7374 726f 7928 290a  entry.destroy().
-00003250: 2020 2020 7769 7468 2063 6f6e 7465 7874      with context
-00003260: 6c69 622e 7375 7070 7265 7373 2841 7474  lib.suppress(Att
-00003270: 7269 6275 7465 4572 726f 7229 3a0a 2020  ributeError):.  
-00003280: 2020 2020 2020 7365 6c66 2e70 6f72 745f        self.port_
-00003290: 656e 7472 792e 6465 7374 726f 7928 290a  entry.destroy().
-000032a0: 2020 2020 7769 7468 2063 6f6e 7465 7874      with context
-000032b0: 6c69 622e 7375 7070 7265 7373 2841 7474  lib.suppress(Att
-000032c0: 7269 6275 7465 4572 726f 7229 3a0a 2020  ributeError):.  
-000032d0: 2020 2020 2020 7365 6c66 2e66 696c 655f        self.file_
-000032e0: 656e 7472 792e 6465 7374 726f 7928 290a  entry.destroy().
-000032f0: 2020 2020 7769 7468 2063 6f6e 7465 7874      with context
-00003300: 6c69 622e 7375 7070 7265 7373 2841 7474  lib.suppress(Att
-00003310: 7269 6275 7465 4572 726f 7229 3a0a 2020  ributeError):.  
-00003320: 2020 2020 2020 7365 6c66 2e69 705f 6c61        self.ip_la
-00003330: 6265 6c2e 6465 7374 726f 7928 290a 2020  bel.destroy().  
-00003340: 2020 7769 7468 2063 6f6e 7465 7874 6c69    with contextli
-00003350: 622e 7375 7070 7265 7373 2841 7474 7269  b.suppress(Attri
-00003360: 6275 7465 4572 726f 7229 3a0a 2020 2020  buteError):.    
-00003370: 2020 2020 7365 6c66 2e70 6f72 745f 6c61      self.port_la
-00003380: 6265 6c2e 6465 7374 726f 7928 290a 2020  bel.destroy().  
-00003390: 2020 7769 7468 2063 6f6e 7465 7874 6c69    with contextli
-000033a0: 622e 7375 7070 7265 7373 2841 7474 7269  b.suppress(Attri
-000033b0: 6275 7465 4572 726f 7229 3a0a 2020 2020  buteError):.    
-000033c0: 2020 2020 7365 6c66 2e66 696c 655f 6c61      self.file_la
-000033d0: 6265 6c2e 6465 7374 726f 7928 290a 2020  bel.destroy().  
-000033e0: 2020 7769 7468 2063 6f6e 7465 7874 6c69    with contextli
-000033f0: 622e 7375 7070 7265 7373 2841 7474 7269  b.suppress(Attri
-00003400: 6275 7465 4572 726f 7229 3a0a 2020 2020  buteError):.    
-00003410: 2020 2020 7365 6c66 2e67 6574 5f62 6163      self.get_bac
-00003420: 6b75 705f 6275 7474 6f6e 2e64 6573 7472  kup_button.destr
-00003430: 6f79 2829 0a20 2020 2077 6974 6820 636f  oy().    with co
-00003440: 6e74 6578 746c 6962 2e73 7570 7072 6573  ntextlib.suppres
-00003450: 7328 4174 7472 6962 7574 6545 7272 6f72  s(AttributeError
-00003460: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00003470: 6361 6e63 656c 5f65 6e74 7279 5f62 7574  cancel_entry_but
-00003480: 746f 6e2e 6465 7374 726f 7928 290a 2020  ton.destroy().  
-00003490: 2020 7769 7468 2063 6f6e 7465 7874 6c69    with contextli
-000034a0: 622e 7375 7070 7265 7373 2841 7474 7269  b.suppress(Attri
-000034b0: 6275 7465 4572 726f 7229 3a0a 2020 2020  buteError):.    
-000034c0: 2020 2020 7365 6c66 2e6c 6973 745f 6669      self.list_fi
-000034d0: 6c65 735f 6275 7474 6f6e 2e64 6573 7472  les_button.destr
-000034e0: 6f79 2829 0a20 2020 2077 6974 6820 636f  oy().    with co
-000034f0: 6e74 6578 746c 6962 2e73 7570 7072 6573  ntextlib.suppres
-00003500: 7328 4174 7472 6962 7574 6545 7272 6f72  s(AttributeError
-00003510: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00003520: 6c61 6265 6c5f 6f72 2e64 6573 7472 6f79  label_or.destroy
-00003530: 2829 0a20 2020 2077 6974 6820 636f 6e74  ().    with cont
-00003540: 6578 746c 6962 2e73 7570 7072 6573 7328  extlib.suppress(
-00003550: 4174 7472 6962 7574 6545 7272 6f72 293a  AttributeError):
-00003560: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
-00003570: 6c65 6c69 7374 5f6c 6162 656c 2e64 6573  lelist_label.des
-00003580: 7472 6f79 2829 0a20 2020 2077 6974 6820  troy().    with 
-00003590: 636f 6e74 6578 746c 6962 2e73 7570 7072  contextlib.suppr
-000035a0: 6573 7328 4174 7472 6962 7574 6545 7272  ess(AttributeErr
-000035b0: 6f72 293a 0a20 2020 2020 2020 2073 656c  or):.        sel
-000035c0: 662e 6669 6c65 6c69 7374 5f6f 7074 696f  f.filelist_optio
-000035d0: 6e2e 6465 7374 726f 7928 290a 2020 2020  n.destroy().    
-000035e0: 7769 7468 2063 6f6e 7465 7874 6c69 622e  with contextlib.
-000035f0: 7375 7070 7265 7373 2841 7474 7269 6275  suppress(Attribu
-00003600: 7465 4572 726f 7229 3a0a 2020 2020 2020  teError):.      
-00003610: 2020 7365 6c66 2e6c 6973 745f 6669 6c65    self.list_file
-00003620: 735f 7175 6572 795f 6275 7474 6f6e 2e64  s_query_button.d
-00003630: 6573 7472 6f79 2829 0a20 2020 2077 6974  estroy().    wit
-00003640: 6820 636f 6e74 6578 746c 6962 2e73 7570  h contextlib.sup
-00003650: 7072 6573 7328 4174 7472 6962 7574 6545  press(AttributeE
-00003660: 7272 6f72 293a 2020 2320 4465 7374 726f  rror):  # Destro
-00003670: 7920 7570 6772 6164 6520 6275 7474 6f6e  y upgrade button
-00003680: 2073 696e 6365 2066 696c 6520 6c6f 6361   since file loca
-00003690: 7469 6f6e 2077 6f75 6c64 2073 6974 206f  tion would sit o
-000036a0: 6e20 746f 7020 6f66 2069 742e 0a20 2020  n top of it..   
-000036b0: 2020 2020 2073 656c 662e 7570 6772 6164       self.upgrad
-000036c0: 655f 6275 7474 6f6e 2e64 6573 7472 6f79  e_button.destroy
-000036d0: 2829 0a0a 2020 2020 7365 6c66 2e67 6574  ()..    self.get
-000036e0: 5f62 6163 6b75 705f 6275 7474 6f6e 203d  _backup_button =
-000036f0: 2073 656c 662e 6469 7370 6c61 795f 6261   self.display_ba
-00003700: 636b 7570 5f62 7574 746f 6e28 0a20 2020  ckup_button(.   
-00003710: 2020 2020 2022 4765 7420 584d 4c20 6672       "Get XML fr
-00003720: 6f6d 2041 6e64 726f 6964 2044 6576 6963  om Android Devic
-00003730: 6522 2c0a 2020 2020 2020 2020 2223 3234  e",.        "#24
-00003740: 3646 4236 222c 0a20 2020 2020 2020 2022  6FB6",.        "
-00003750: 2336 3536 3366 6622 2c0a 2020 2020 2020  #6563ff",.      
-00003760: 2020 7365 6c66 2e67 6574 5f62 6163 6b75    self.get_backu
-00003770: 705f 6576 656e 742c 0a20 2020 2029 0a0a  p_event,.    )..
-00003780: 0a23 2023 2323 2323 2323 2323 2323 2323  .# #############
-00003790: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000037a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000037b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000037c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000037d0: 2323 2323 230a 2320 436f 6d70 6172 6520  #####.# Compare 
-000037e0: 7477 6f20 7665 7273 696f 6e73 2061 6e64  two versions and
-000037f0: 2072 6574 7572 6e20 5472 7565 2069 6620   return True if 
-00003800: 7665 7273 696f 6e32 2069 7320 6772 6561  version2 is grea
-00003810: 7465 7220 7468 616e 2076 6572 7369 6f6e  ter than version
-00003820: 312e 0a23 2023 2323 2323 2323 2323 2323  1..# ###########
-00003830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003870: 2323 2323 2323 230a 6465 6620 6973 5f76  #######.def is_v
-00003880: 6572 7369 6f6e 5f67 7265 6174 6572 2876  ersion_greater(v
-00003890: 6572 7369 6f6e 313a 2073 7472 2c20 7665  ersion1: str, ve
-000038a0: 7273 696f 6e32 3a20 7374 7229 202d 3e20  rsion2: str) -> 
-000038b0: 626f 6f6c 3a0a 2020 2020 2222 220a 2020  bool:.    """.  
-000038c0: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-000038d0: 6368 6563 6b73 2069 6620 7665 7273 696f  checks if versio
-000038e0: 6e32 2069 7320 6772 6561 7465 7220 7468  n2 is greater th
-000038f0: 616e 2076 6572 7369 6f6e 312e 0a0a 2020  an version1...  
-00003900: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00003910: 7665 7273 696f 6e31 3a20 4120 7374 7269  version1: A stri
-00003920: 6e67 2072 6570 7265 7365 6e74 696e 6720  ng representing 
-00003930: 7468 6520 6669 7273 7420 7665 7273 696f  the first versio
-00003940: 6e20 696e 2074 6865 2066 6f72 6d61 7420  n in the format 
-00003950: 226d 616a 6f72 2e6d 696e 6f72 2e70 6174  "major.minor.pat
-00003960: 6368 222e 0a20 2020 2020 2020 2076 6572  ch"..        ver
-00003970: 7369 6f6e 323a 2041 2073 7472 696e 6720  sion2: A string 
-00003980: 7265 7072 6573 656e 7469 6e67 2074 6865  representing the
-00003990: 2073 6563 6f6e 6420 7665 7273 696f 6e20   second version 
-000039a0: 696e 2074 6865 2066 6f72 6d61 7420 226d  in the format "m
-000039b0: 616a 6f72 2e6d 696e 6f72 2e70 6174 6368  ajor.minor.patch
-000039c0: 222e 0a0a 2020 2020 5265 7475 726e 733a  "...    Returns:
-000039d0: 0a20 2020 2020 2020 2054 7275 6520 6966  .        True if
-000039e0: 2076 6572 7369 6f6e 3220 6973 2067 7265   version2 is gre
-000039f0: 6174 6572 2074 6861 6e20 7665 7273 696f  ater than versio
-00003a00: 6e31 2c20 4661 6c73 6520 6f74 6865 7277  n1, False otherw
-00003a10: 6973 652e 0a20 2020 2022 2222 0a0a 2020  ise..    """..  
-00003a20: 2020 2320 5370 6c69 7420 7468 6520 7665    # Split the ve
-00003a30: 7273 696f 6e73 2062 7920 222e 220a 2020  rsions by ".".  
-00003a40: 2020 7631 5f70 6172 7473 203d 205b 696e    v1_parts = [in
-00003a50: 7428 7829 2066 6f72 2078 2069 6e20 7665  t(x) for x in ve
-00003a60: 7273 696f 6e31 2e73 706c 6974 2822 2e22  rsion1.split("."
-00003a70: 295d 0a20 2020 2076 325f 7061 7274 7320  )].    v2_parts 
-00003a80: 3d20 5b69 6e74 2878 2920 666f 7220 7820  = [int(x) for x 
-00003a90: 696e 2076 6572 7369 6f6e 322e 7370 6c69  in version2.spli
-00003aa0: 7428 222e 2229 5d0a 0a20 2020 2023 2049  t(".")]..    # I
-00003ab0: 7465 7261 7465 2074 6872 6f75 6768 2065  terate through e
-00003ac0: 6163 6820 7061 7274 206f 6620 7468 6520  ach part of the 
-00003ad0: 7665 7273 696f 6e0a 2020 2020 666f 7220  version.    for 
-00003ae0: 6920 696e 2072 616e 6765 286d 696e 286c  i in range(min(l
-00003af0: 656e 2876 315f 7061 7274 7329 2c20 6c65  en(v1_parts), le
-00003b00: 6e28 7632 5f70 6172 7473 2929 293a 0a20  n(v2_parts))):. 
-00003b10: 2020 2020 2020 2069 6620 7631 5f70 6172         if v1_par
-00003b20: 7473 5b69 5d20 3c20 7632 5f70 6172 7473  ts[i] < v2_parts
-00003b30: 5b69 5d3a 0a20 2020 2020 2020 2020 2020  [i]:.           
-00003b40: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-00003b50: 2020 2020 2069 6620 7631 5f70 6172 7473       if v1_parts
-00003b60: 5b69 5d20 3e20 7632 5f70 6172 7473 5b69  [i] > v2_parts[i
-00003b70: 5d3a 0a20 2020 2020 2020 2020 2020 2072  ]:.            r
-00003b80: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-00003b90: 2023 2049 6620 616c 6c20 7061 7274 7320   # If all parts 
-00003ba0: 6172 6520 6571 7561 6c2c 2063 6865 636b  are equal, check
-00003bb0: 206c 656e 6774 680a 2020 2020 7265 7475   length.    retu
-00003bc0: 726e 206c 656e 2876 325f 7061 7274 7329  rn len(v2_parts)
-00003bd0: 203e 206c 656e 2876 315f 7061 7274 7329   > len(v1_parts)
-00003be0: 0a0a 0a23 2023 2323 2323 2323 2323 2323  ...# ###########
-00003bf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003c00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003c10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003c20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003c30: 2323 2323 2323 230a 2320 4368 6563 6b73  #######.# Checks
-00003c40: 2069 6620 3234 2068 6f75 7273 2068 6176   if 24 hours hav
-00003c50: 6520 7061 7373 6564 2073 696e 6365 2074  e passed since t
-00003c60: 6865 2067 6976 656e 2070 7265 7669 6f75  he given previou
-00003c70: 7320 6461 7465 2e0a 2320 2323 2323 2323  s date..# ######
-00003c80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003c90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003ca0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003cb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003cc0: 2323 2323 2323 2323 2323 2323 0a64 6566  ############.def
-00003cd0: 2069 735f 6d6f 7265 5f74 6861 6e5f 3234   is_more_than_24
-00003ce0: 6872 7328 696e 7075 745f 6461 7465 7469  hrs(input_dateti
-00003cf0: 6d65 3a20 6461 7465 7469 6d65 2920 2d3e  me: datetime) ->
-00003d00: 2062 6f6f 6c3a 0a20 2020 2022 2222 4368   bool:.    """Ch
-00003d10: 6563 6b73 2069 6620 7468 6520 696e 7075  ecks if the inpu
-00003d20: 7420 6461 7465 7469 6d65 2069 7320 6d6f  t datetime is mo
-00003d30: 7265 2074 6861 6e20 3234 2068 6f75 7273  re than 24 hours
-00003d40: 2061 676f 2e0a 2020 2020 4172 6775 6d65   ago..    Argume
-00003d50: 6e74 733a 0a20 2020 2020 2020 2069 6e70  nts:.        inp
-00003d60: 7574 5f64 6174 6574 696d 6520 2864 6174  ut_datetime (dat
-00003d70: 6574 696d 6529 3a20 5468 6520 6461 7465  etime): The date
-00003d80: 7469 6d65 2074 6f20 6265 2063 6865 636b  time to be check
-00003d90: 6564 2e0a 2020 2020 5265 7475 726e 733a  ed..    Returns:
-00003da0: 0a20 2020 2020 2020 2062 6f6f 6c3a 2054  .        bool: T
-00003db0: 7275 6520 6966 2069 6e70 7574 2064 6174  rue if input dat
-00003dc0: 6574 696d 6520 6973 206d 6f72 6520 7468  etime is more th
-00003dd0: 616e 2032 3420 686f 7572 7320 6167 6f2c  an 24 hours ago,
-00003de0: 2046 616c 7365 206f 7468 6572 7769 7365   False otherwise
-00003df0: 2e0a 2020 2020 5072 6f63 6573 7369 6e67  ..    Processing
-00003e00: 204c 6f67 6963 3a0a 2020 2020 2020 2020   Logic:.        
-00003e10: 2d20 4361 6c63 756c 6174 6520 7365 636f  - Calculate seco
-00003e20: 6e64 7320 696e 2032 3420 686f 7572 732e  nds in 24 hours.
-00003e30: 0a20 2020 2020 2020 202d 2047 6574 2063  .        - Get c
-00003e40: 7572 7265 6e74 2064 6174 6574 696d 652e  urrent datetime.
-00003e50: 0a20 2020 2020 2020 202d 2043 6865 636b  .        - Check
-00003e60: 2069 6620 6469 6666 6572 656e 6365 2062   if difference b
-00003e70: 6574 7765 656e 2063 7572 7265 6e74 2064  etween current d
-00003e80: 6174 6574 696d 6520 616e 6420 696e 7075  atetime and inpu
-00003e90: 7420 6461 7465 7469 6d65 2069 7320 6772  t datetime is gr
-00003ea0: 6561 7465 7220 7468 616e 2032 3420 686f  eater than 24 ho
-00003eb0: 7572 732e 0a20 2020 2020 2020 202d 2052  urs..        - R
-00003ec0: 6574 7572 6e20 7265 7375 6c74 2061 7320  eturn result as 
-00003ed0: 626f 6f6c 6561 6e2e 2222 220a 2020 2020  boolean.""".    
-00003ee0: 7477 656e 7479 5f66 6f75 725f 686f 7572  twenty_four_hour
-00003ef0: 7320 3d20 3836 3430 3020 2023 2073 6563  s = 86400  # sec
-00003f00: 6f6e 6473 2069 6e20 3234 2068 6f75 7273  onds in 24 hours
-00003f10: 0a20 2020 2072 6574 7572 6e20 284e 4f57  .    return (NOW
-00003f20: 5f54 494d 4520 2d20 696e 7075 745f 6461  _TIME - input_da
-00003f30: 7465 7469 6d65 292e 746f 7461 6c5f 7365  tetime).total_se
-00003f40: 636f 6e64 7328 2920 3e20 7477 656e 7479  conds() > twenty
-00003f50: 5f66 6f75 725f 686f 7572 730a 0a0a 2320  _four_hours...# 
-00003f60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003f70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003f80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003f90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003fa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003fb0: 2323 0a23 2047 6574 2050 7970 6920 7665  ##.# Get Pypi ve
-00003fc0: 7273 696f 6e20 616e 6420 7265 7475 726e  rsion and return
-00003fd0: 2054 7275 6520 6966 2069 7420 6973 206e   True if it is n
-00003fe0: 6577 6572 2074 6861 6e20 6f75 7220 6375  ewer than our cu
-00003ff0: 7272 656e 7420 7665 7273 696f 6e2e 0a23  rrent version..#
-00004000: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00004010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004050: 2323 230a 6465 6620 6973 5f6e 6577 5f76  ###.def is_new_v
-00004060: 6572 7369 6f6e 2829 202d 3e20 626f 6f6c  ersion() -> bool
-00004070: 3a0a 2020 2020 2222 220a 2020 2020 4368  :.    """.    Ch
-00004080: 6563 6b20 6966 2074 6865 206e 6577 2076  eck if the new v
-00004090: 6572 7369 6f6e 2069 7320 6176 6169 6c61  ersion is availa
-000040a0: 626c 650a 2020 2020 4172 6773 3a0a 2020  ble.    Args:.  
-000040b0: 2020 2020 2020 7365 6c66 3a20 5468 6520        self: The 
-000040c0: 636c 6173 7320 696e 7374 616e 6365 0a20  class instance. 
-000040d0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-000040e0: 2020 2020 626f 6f6c 3a20 5472 7565 2069      bool: True i
-000040f0: 6620 6e65 7720 7665 7273 696f 6e20 6973  f new version is
-00004100: 2061 7661 696c 6162 6c65 2c20 4661 6c73   available, Fals
-00004110: 6520 6966 206e 6f74 2222 220a 2020 2020  e if not""".    
-00004120: 2320 4368 6563 6b20 6966 206e 6577 6572  # Check if newer
-00004130: 2076 6572 7369 6f6e 206f 6620 6f75 7220   version of our 
-00004140: 636f 6465 2069 7320 6176 6169 6c61 626c  code is availabl
-00004150: 6520 6f6e 2050 7970 692e 0a20 2020 2023  e on Pypi..    #
-00004160: 2069 6620 6973 5f6d 6f72 655f 7468 616e   if is_more_than
-00004170: 5f32 3468 7273 2850 7269 6d65 4974 656d  _24hrs(PrimeItem
-00004180: 732e 6c61 7374 5f72 756e 293a 2020 2320  s.last_run):  # 
-00004190: 4f6e 6c79 2063 6865 636b 2065 7665 7279  Only check every
-000041a0: 2032 3420 686f 7572 732e 0a20 2020 2070   24 hours..    p
-000041b0: 7970 695f 7665 7273 696f 6e5f 636f 6465  ypi_version_code
-000041c0: 203d 2067 6574 5f70 7970 695f 7665 7273   = get_pypi_vers
-000041d0: 696f 6e28 290a 2020 2020 6966 2070 7970  ion().    if pyp
-000041e0: 695f 7665 7273 696f 6e5f 636f 6465 3a0a  i_version_code:.
-000041f0: 2020 2020 2020 2020 7079 7069 5f76 6572          pypi_ver
-00004200: 7369 6f6e 203d 2070 7970 695f 7665 7273  sion = pypi_vers
-00004210: 696f 6e5f 636f 6465 2e73 706c 6974 2822  ion_code.split("
-00004220: 3d3d 2229 5b31 5d0a 2020 2020 2020 2020  ==")[1].        
-00004230: 5072 696d 6549 7465 6d73 2e6c 6173 745f  PrimeItems.last_
-00004240: 7275 6e20 3d20 4e4f 575f 5449 4d45 2020  run = NOW_TIME  
-00004250: 2320 5570 6461 7465 206c 6173 7420 7275  # Update last ru
-00004260: 6e20 746f 206e 6f77 2073 696e 6365 2077  n to now since w
-00004270: 6520 6172 6520 646f 696e 6720 7468 6520  e are doing the 
-00004280: 6368 6563 6b2e 0a20 2020 2020 2020 2072  check..        r
-00004290: 6574 7572 6e20 6973 5f76 6572 7369 6f6e  eturn is_version
-000042a0: 5f67 7265 6174 6572 2856 4552 5349 4f4e  _greater(VERSION
-000042b0: 2c20 7079 7069 5f76 6572 7369 6f6e 290a  , pypi_version).
-000042c0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000042d0: 0a0a 0a23 2023 2323 2323 2323 2323 2323  ...# ###########
-000042e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000042f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004320: 2323 2323 2323 230a 2320 4c69 7374 2074  #######.# List t
-00004330: 6865 2058 4d4c 2066 696c 6573 206f 6e20  he XML files on 
-00004340: 7468 6520 416e 6472 6f69 6420 6465 7669  the Android devi
-00004350: 6365 0a23 2023 2323 2323 2323 2323 2323  ce.# ###########
-00004360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000043a0: 2323 2323 2323 230a 6465 6620 6765 745f  #######.def get_
-000043b0: 6c69 7374 5f6f 665f 6669 6c65 7328 6970  list_of_files(ip
-000043c0: 5f61 6464 7265 7373 3a20 7374 722c 2069  _address: str, i
-000043d0: 705f 706f 7274 3a20 7374 722c 2066 696c  p_port: str, fil
-000043e0: 655f 6c6f 6361 7469 6f6e 3a20 7374 7229  e_location: str)
-000043f0: 202d 3e20 7475 706c 653a 0a20 2020 2022   -> tuple:.    "
-00004400: 2222 4765 7420 6c69 7374 206f 6620 6669  ""Get list of fi
-00004410: 6c65 7320 6672 6f6d 2067 6976 656e 2049  les from given I
-00004420: 5020 6164 6472 6573 732e 0a20 2020 2050  P address..    P
-00004430: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
-00004440: 2020 202d 2069 705f 6164 6472 6573 7320     - ip_address 
-00004450: 2873 7472 293a 2049 5020 6164 6472 6573  (str): IP addres
-00004460: 7320 746f 2063 6f6e 6e65 6374 2074 6f2e  s to connect to.
-00004470: 0a20 2020 2020 2020 202d 2069 705f 706f  .        - ip_po
-00004480: 7274 2028 7374 7229 3a20 506f 7274 206e  rt (str): Port n
-00004490: 756d 6265 7220 746f 2063 6f6e 6e65 6374  umber to connect
-000044a0: 2074 6f2e 0a20 2020 2020 2020 202d 2066   to..        - f
-000044b0: 696c 655f 6c6f 6361 7469 6f6e 2028 7374  ile_location (st
-000044c0: 7229 3a20 4c6f 6361 7469 6f6e 206f 6620  r): Location of 
-000044d0: 7468 6520 6669 6c65 2074 6f20 7265 7472  the file to retr
-000044e0: 6965 7665 2e0a 2020 2020 5265 7475 726e  ieve..    Return
-000044f0: 733a 0a20 2020 2020 2020 202d 2074 7570  s:.        - tup
-00004500: 6c65 3a20 5265 7475 726e 2063 6f64 6520  le: Return code 
-00004510: 616e 6420 6c69 7374 206f 6620 6669 6c65  and list of file
-00004520: 206c 6f63 6174 696f 6e73 2e0a 2020 2020   locations..    
-00004530: 5072 6f63 6573 7369 6e67 204c 6f67 6963  Processing Logic
-00004540: 3a0a 2020 2020 2020 2020 2d20 5265 7472  :.        - Retr
-00004550: 6965 7665 2066 696c 6520 636f 6e74 656e  ieve file conten
-00004560: 7473 2075 7369 6e67 2068 7474 705f 7265  ts using http_re
-00004570: 7175 6573 742e 0a20 2020 2020 2020 202d  quest..        -
-00004580: 2049 6620 7265 7475 726e 2063 6f64 6520   If return code 
-00004590: 6973 2030 2c20 7370 6c69 7420 7468 6520  is 0, split the 
-000045a0: 6465 636f 6465 6420 7374 7269 6e67 2069  decoded string i
-000045b0: 6e74 6f20 6120 6c69 7374 2061 6e64 2072  nto a list and r
-000045c0: 6574 7572 6e2e 0a20 2020 2020 2020 202d  eturn..        -
-000045d0: 204f 7468 6572 7769 7365 2c20 7265 7475   Otherwise, retu
-000045e0: 726e 2065 7272 6f72 2077 6974 6820 656d  rn error with em
-000045f0: 7074 7920 7374 7269 6e67 2e22 2222 0a0a  pty string."""..
-00004600: 2020 2020 2320 4765 7420 7468 6520 636f      # Get the co
-00004610: 6e74 656e 7473 206f 6620 7468 6520 6669  ntents of the fi
-00004620: 6c65 2e0a 2020 2020 7265 7475 726e 5f63  le..    return_c
-00004630: 6f64 652c 2066 696c 655f 636f 6e74 656e  ode, file_conten
-00004640: 7473 203d 2068 7474 705f 7265 7175 6573  ts = http_reques
-00004650: 7428 6970 5f61 6464 7265 7373 2c20 6970  t(ip_address, ip
-00004660: 5f70 6f72 742c 2066 696c 655f 6c6f 6361  _port, file_loca
-00004670: 7469 6f6e 2c20 226d 6170 6c69 7374 222c  tion, "maplist",
-00004680: 2022 3f78 6d6c 2229 0a0a 2020 2020 2320   "?xml")..    # 
-00004690: 4966 2067 6f6f 6420 7265 7475 726e 2063  If good return c
-000046a0: 6f64 652c 2067 6574 2074 6865 206c 6973  ode, get the lis
-000046b0: 7420 6f66 2058 4d4c 2066 696c 6520 6c6f  t of XML file lo
-000046c0: 6361 7469 6f6e 7320 696e 746f 2061 206c  cations into a l
-000046d0: 6973 7420 616e 6420 7265 7475 726e 2e0a  ist and return..
-000046e0: 2020 2020 6966 2072 6574 7572 6e5f 636f      if return_co
-000046f0: 6465 203d 3d20 303a 0a20 2020 2020 2020  de == 0:.       
-00004700: 2064 6563 6f64 6564 5f73 7472 696e 6720   decoded_string 
-00004710: 3d20 2866 696c 655f 636f 6e74 656e 7473  = (file_contents
-00004720: 2e64 6563 6f64 6528 2275 7466 2d38 2229  .decode("utf-8")
-00004730: 292e 7370 6c69 7428 222c 2229 0a20 2020  ).split(",").   
-00004740: 2020 2020 2023 2053 7472 6970 206f 6666       # Strip off
-00004750: 2074 6865 2063 6f75 6e74 2066 6965 6c64   the count field
-00004760: 0a20 2020 2020 2020 2066 6f72 206e 756d  .        for num
-00004770: 2c20 6974 656d 2069 6e20 656e 756d 6572  , item in enumer
-00004780: 6174 6528 6465 636f 6465 645f 7374 7269  ate(decoded_stri
-00004790: 6e67 293a 0a20 2020 2020 2020 2020 2020  ng):.           
-000047a0: 2074 656d 705f 6974 656d 203d 2069 7465   temp_item = ite
-000047b0: 6d5b 3a2d 335d 2020 2320 4472 6f70 206c  m[:-3]  # Drop l
-000047c0: 6173 7420 3320 6368 6172 6163 7465 7273  ast 3 characters
-000047d0: 0a20 2020 2020 2020 2020 2020 2064 6563  .            dec
-000047e0: 6f64 6564 5f73 7472 696e 675b 6e75 6d5d  oded_string[num]
-000047f0: 203d 2074 656d 705f 6974 656d 2e72 6570   = temp_item.rep
-00004800: 6c61 6365 2822 2f73 746f 7261 6765 2f65  lace("/storage/e
-00004810: 6d75 6c61 7465 642f 3022 2c20 2222 290a  mulated/0", "").
-00004820: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
-00004830: 2069 7465 6d73 2074 6861 7420 6172 6520   items that are 
-00004840: 696e 2074 6865 2074 7261 7368 0a20 2020  in the trash.   
-00004850: 2020 2020 2066 696e 616c 5f6c 6973 7420       final_list 
-00004860: 3d20 5b69 7465 6d20 666f 7220 6974 656d  = [item for item
-00004870: 2069 6e20 6465 636f 6465 645f 7374 7269   in decoded_stri
-00004880: 6e67 2069 6620 222e 5472 6173 6822 206e  ng if ".Trash" n
-00004890: 6f74 2069 6e20 6974 656d 5d0a 2020 2020  ot in item].    
-000048a0: 2020 2020 7265 7475 726e 2030 2c20 6669      return 0, fi
-000048b0: 6e61 6c5f 6c69 7374 0a0a 2020 2020 2320  nal_list..    # 
-000048c0: 4f74 6865 7277 6973 652c 2072 6574 7572  Otherwise, retur
-000048d0: 6e20 6572 726f 720a 2020 2020 7265 7475  n error.    retu
-000048e0: 726e 2072 6574 7572 6e5f 636f 6465 2c20  rn return_code, 
-000048f0: 6669 6c65 5f63 6f6e 7465 6e74 730a 0a0a  file_contents...
-00004900: 2320 2323 2323 2323 2323 2323 2323 2323  # ##############
-00004910: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004930: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004950: 2323 2323 0a23 2057 7269 7465 206f 7574  ####.# Write out
-00004960: 2074 6865 2063 6861 6e67 656c 6f67 0a23   the changelog.#
-00004970: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00004980: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004990: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000049a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000049b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000049c0: 2323 230a 6465 6620 6372 6561 7465 5f63  ###.def create_c
-000049d0: 6861 6e67 656c 6f67 2829 202d 3e20 4e6f  hangelog() -> No
-000049e0: 6e65 3a0a 2020 2020 2222 2243 7265 6174  ne:.    """Creat
-000049f0: 6520 6368 616e 6765 6c6f 6720 6669 6c65  e changelog file
-00004a00: 2e22 2222 0a20 2020 2077 6974 6820 6f70  .""".    with op
-00004a10: 656e 2843 4841 4e47 454c 4f47 5f46 494c  en(CHANGELOG_FIL
-00004a20: 452c 2022 7722 2920 6173 2063 6861 6e67  E, "w") as chang
-00004a30: 656c 6f67 5f66 696c 653a 0a20 2020 2020  elog_file:.     
-00004a40: 2020 2063 6861 6e67 656c 6f67 5f66 696c     changelog_fil
-00004a50: 652e 7772 6974 6528 4348 414e 4745 4c4f  e.write(CHANGELO
-00004a60: 4729 0a0a 0a23 2023 2323 2323 2323 2323  G)...# #########
-00004a70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004a80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004a90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004ab0: 2323 2323 2323 2323 230a 2320 5265 6164  #########.# Read
-00004ac0: 2074 6865 2063 6861 6e67 6520 6c6f 6720   the change log 
-00004ad0: 6669 6c65 2c20 6164 6420 6974 2074 6f20  file, add it to 
-00004ae0: 7468 6520 6d65 7373 6167 6573 2074 6f20  the messages to 
-00004af0: 6265 2064 6973 706c 6179 6564 2061 6e64  be displayed and
-00004b00: 2074 6865 6e20 7265 6d6f 7665 2069 742e   then remove it.
-00004b10: 0a23 2023 2323 2323 2323 2323 2323 2323  .# #############
-00004b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004b30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004b40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004b50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004b60: 2323 2323 230a 6465 6620 6368 6563 6b5f  #####.def check_
-00004b70: 666f 725f 6368 616e 6765 6c6f 6728 7365  for_changelog(se
-00004b80: 6c66 2920 2d3e 204e 6f6e 653a 2020 2320  lf) -> None:  # 
-00004b90: 6e6f 7161 3a20 414e 4e30 3031 0a20 2020  noqa: ANN001.   
-00004ba0: 2022 2222 4675 6e63 7469 6f6e 2074 6f20   """Function to 
-00004bb0: 6368 6563 6b20 666f 7220 6120 6368 616e  check for a chan
-00004bc0: 6765 6c6f 6720 6669 6c65 2061 6e64 2061  gelog file and a
-00004bd0: 6464 2069 7473 2063 6f6e 7465 6e74 7320  dd its contents 
-00004be0: 746f 2061 206d 6573 7361 6765 2069 6620  to a message if 
-00004bf0: 7468 6520 6375 7272 656e 7420 7665 7273  the current vers
-00004c00: 696f 6e20 6973 2063 6f72 7265 6374 2e0a  ion is correct..
-00004c10: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
-00004c20: 2020 2020 2020 2020 2d20 7365 6c66 2028          - self (
-00004c30: 6f62 6a65 6374 293a 2054 6865 206f 626a  object): The obj
-00004c40: 6563 7420 7468 6174 2074 6865 2066 756e  ect that the fun
-00004c50: 6374 696f 6e20 6973 2062 6569 6e67 2063  ction is being c
-00004c60: 616c 6c65 6420 6f6e 2e0a 2020 2020 5265  alled on..    Re
-00004c70: 7475 726e 733a 0a20 2020 2020 2020 202d  turns:.        -
-00004c80: 204e 6f6e 653a 2054 6865 2066 756e 6374   None: The funct
-00004c90: 696f 6e20 646f 6573 206e 6f74 2072 6574  ion does not ret
-00004ca0: 7572 6e20 616e 7974 6869 6e67 2c20 6275  urn anything, bu
-00004cb0: 7420 7570 6461 7465 7320 7468 6520 6d65  t updates the me
-00004cc0: 7373 6167 6520 6174 7472 6962 7574 6520  ssage attribute 
-00004cd0: 6f66 2074 6865 206f 626a 6563 742e 0a20  of the object.. 
-00004ce0: 2020 2050 726f 6365 7373 696e 6720 4c6f     Processing Lo
-00004cf0: 6769 633a 0a20 2020 2020 2020 202d 2043  gic:.        - C
-00004d00: 6865 636b 2069 6620 7468 6520 6368 616e  heck if the chan
-00004d10: 6765 6c6f 6720 6669 6c65 2065 7869 7374  gelog file exist
-00004d20: 732e 0a20 2020 2020 2020 202d 2049 6620  s..        - If 
-00004d30: 6974 2065 7869 7374 732c 2070 7265 7061  it exists, prepa
-00004d40: 7265 2074 6f20 6469 7370 6c61 7920 6368  re to display ch
-00004d50: 616e 6765 7320 616e 6420 7265 6d6f 7665  anges and remove
-00004d60: 2074 6865 2066 696c 6520 736f 2077 6520   the file so we 
-00004d70: 6f6e 6c79 2064 6973 706c 6179 2074 6865  only display the
-00004d80: 2063 6861 6e67 6573 206f 6e63 652e 2222   changes once.""
-00004d90: 220a 2020 2020 2320 544f 444f 2054 6573  ".    # TODO Tes
-00004da0: 7420 6368 616e 6765 6c6f 6720 6265 666f  t changelog befo
-00004db0: 7265 2070 6f73 7469 6e67 2074 6f20 5079  re posting to Py
-00004dc0: 5069 2e20 2043 6f6d 6d65 6e74 2069 7420  Pi.  Comment it 
-00004dd0: 6f75 7420 6166 7465 7220 7465 7374 696e  out after testin
-00004de0: 672e 0a20 2020 2023 7365 6c66 2e6d 6573  g..    #self.mes
-00004df0: 7361 6765 203d 2043 4841 4e47 454c 4f47  sage = CHANGELOG
-00004e00: 0a0a 2020 2020 6966 206f 732e 7061 7468  ..    if os.path
-00004e10: 2e69 7366 696c 6528 4348 414e 4745 4c4f  .isfile(CHANGELO
-00004e20: 475f 4649 4c45 293a 0a20 2020 2020 2020  G_FILE):.       
-00004e30: 2073 656c 662e 6d65 7373 6167 6520 3d20   self.message = 
-00004e40: 4348 414e 4745 4c4f 470a 2020 2020 2020  CHANGELOG.      
-00004e50: 2020 6f73 2e72 656d 6f76 6528 4348 414e    os.remove(CHAN
-00004e60: 4745 4c4f 475f 4649 4c45 290a 0a0a 2320  GELOG_FILE)...# 
-00004e70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004e80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004e90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004ea0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004eb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004ec0: 2323 0a23 2049 6e69 7469 616c 697a 6520  ##.# Initialize 
-00004ed0: 7468 6520 4755 4920 285f 696e 6974 5f20  the GUI (_init_ 
-00004ee0: 6d65 7468 6f64 290a 2320 2323 2323 2323  method).# ######
-00004ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004f10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004f20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004f30: 2323 2323 2323 2323 2323 2323 0a64 6566  ############.def
-00004f40: 2069 6e69 7469 616c 697a 655f 6775 6928   initialize_gui(
-00004f50: 7365 6c66 2920 2d3e 204e 6f6e 653a 2020  self) -> None:  
-00004f60: 2320 6e6f 7161 3a20 414e 4e30 3031 0a20  # noqa: ANN001. 
-00004f70: 2020 2022 2222 496e 6974 6961 6c69 7a65     """Initialize
-00004f80: 7320 7468 6520 4755 4920 6279 2069 6e69  s the GUI by ini
-00004f90: 7469 616c 697a 696e 6720 7661 7269 6162  tializing variab
-00004fa0: 6c65 7320 616e 6420 6164 6469 6e67 2061  les and adding a
-00004fb0: 206c 6f67 6f2e 0a20 2020 2050 6172 616d   logo..    Param
-00004fc0: 6574 6572 733a 0a20 2020 2020 2020 202d  eters:.        -
-00004fd0: 2073 656c 6620 2863 6c61 7373 293a 2054   self (class): T
-00004fe0: 6865 2063 6c61 7373 206f 626a 6563 742e  he class object.
-00004ff0: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-00005000: 2020 2020 2020 2d20 4e6f 6e65 3a20 446f        - None: Do
-00005010: 6573 206e 6f74 2072 6574 7572 6e20 616e  es not return an
-00005020: 7974 6869 6e67 2e0a 2020 2020 5072 6f63  ything..    Proc
-00005030: 6573 7369 6e67 204c 6f67 6963 3a0a 2020  essing Logic:.  
-00005040: 2020 2020 2020 2d20 4361 6c6c 7320 696e        - Calls in
-00005050: 6974 6961 6c69 7a65 5f76 6172 6961 626c  itialize_variabl
-00005060: 6573 2066 756e 6374 696f 6e2e 0a20 2020  es function..   
-00005070: 2020 2020 202d 2043 616c 6c73 2061 6464       - Calls add
-00005080: 5f6c 6f67 6f20 6675 6e63 7469 6f6e 2e22  _logo function."
-00005090: 2222 0a20 2020 2069 6e69 7469 616c 697a  "".    initializ
-000050a0: 655f 7661 7269 6162 6c65 7328 7365 6c66  e_variables(self
-000050b0: 290a 2020 2020 6164 645f 6c6f 676f 2873  ).    add_logo(s
-000050c0: 656c 6629 0a0a 0a23 2023 2323 2323 2323  elf)...# #######
-000050d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000050e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000050f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005100: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005110: 2323 2323 2323 2323 2323 230a 2320 496e  ###########.# In
-00005120: 6974 6961 6c69 7a65 2074 6865 2047 5549  itialize the GUI
-00005130: 2076 6172 6c69 6162 6c65 7320 2865 2e2e   varliables (e..
-00005140: 6720 5f69 6e69 745f 206d 6574 686f 6429  g _init_ method)
-00005150: 0a23 2023 2323 2323 2323 2323 2323 2323  .# #############
-00005160: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005180: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000051a0: 2323 2323 230a 6465 6620 696e 6974 6961  #####.def initia
-000051b0: 6c69 7a65 5f76 6172 6961 626c 6573 2873  lize_variables(s
-000051c0: 656c 6629 202d 3e20 4e6f 6e65 3a20 2023  elf) -> None:  #
-000051d0: 206e 6f71 613a 2041 4e4e 3030 310a 2020   noqa: ANN001.  
-000051e0: 2020 2222 220a 2020 2020 496e 6974 6961    """.    Initia
-000051f0: 6c69 7a65 2076 6172 6961 626c 6573 2066  lize variables f
-00005200: 6f72 2074 6865 204d 6170 5461 736b 6572  or the MapTasker
-00005210: 2052 756e 7469 6d65 204f 7074 696f 6e73   Runtime Options
-00005220: 2077 696e 646f 772e 0a20 2020 2022 2222   window..    """
-00005230: 0a20 2020 2073 656c 662e 616e 6472 6f69  .    self.androi
-00005240: 645f 6970 6164 6472 203d 2022 220a 2020  d_ipaddr = "".  
-00005250: 2020 7365 6c66 2e61 6e64 726f 6964 5f70    self.android_p
-00005260: 6f72 7420 3d20 2222 0a20 2020 2073 656c  ort = "".    sel
-00005270: 662e 616e 6472 6f69 645f 6669 6c65 203d  f.android_file =
-00005280: 2022 220a 2020 2020 7365 6c66 2e61 7070   "".    self.app
-00005290: 6561 7261 6e63 655f 6d6f 6465 203d 204e  earance_mode = N
-000052a0: 6f6e 650a 2020 2020 7365 6c66 2e62 6f6c  one.    self.bol
-000052b0: 6420 3d20 4e6f 6e65 0a20 2020 2073 656c  d = None.    sel
-000052c0: 662e 636f 6c6f 725f 6c61 6265 6c73 203d  f.color_labels =
-000052d0: 204e 6f6e 650a 2020 2020 7365 6c66 2e63   None.    self.c
-000052e0: 6f6c 6f72 5f6c 6f6f 6b75 7020 3d20 4e6f  olor_lookup = No
-000052f0: 6e65 0a20 2020 2073 656c 662e 636f 6c6f  ne.    self.colo
-00005300: 725f 7465 7874 5f72 6f77 203d 204e 6f6e  r_text_row = Non
-00005310: 650a 2020 2020 7365 6c66 2e64 6562 7567  e.    self.debug
-00005320: 203d 204e 6f6e 650a 2020 2020 7365 6c66   = None.    self
-00005330: 2e64 6973 706c 6179 5f64 6574 6169 6c5f  .display_detail_
-00005340: 6c65 7665 6c20 3d20 4e6f 6e65 0a20 2020  level = None.   
-00005350: 2073 656c 662e 7072 6566 6572 656e 6365   self.preference
-00005360: 7320 3d20 4e6f 6e65 0a20 2020 2073 656c  s = None.    sel
-00005370: 662e 636f 6e64 6974 696f 6e73 203d 204e  f.conditions = N
-00005380: 6f6e 650a 2020 2020 7365 6c66 2e65 7665  one.    self.eve
-00005390: 7279 7468 696e 6720 3d20 4e6f 6e65 0a20  rything = None. 
-000053a0: 2020 2073 656c 662e 7461 736b 6572 6e65     self.taskerne
-000053b0: 7420 3d20 4e6f 6e65 0a20 2020 2073 656c  t = None.    sel
-000053c0: 662e 6578 6974 203d 204e 6f6e 650a 2020  f.exit = None.  
-000053d0: 2020 7365 6c66 2e66 6574 6368 6564 5f62    self.fetched_b
-000053e0: 6163 6b75 705f 6672 6f6d 5f61 6e64 726f  ackup_from_andro
-000053f0: 6964 203d 2046 616c 7365 0a20 2020 2073  id = False.    s
-00005400: 656c 662e 6669 6c65 203d 204e 6f6e 650a  elf.file = None.
-00005410: 2020 2020 7365 6c66 2e66 6f6e 7420 3d20      self.font = 
-00005420: 4e6f 6e65 0a20 2020 2073 656c 662e 676f  None.    self.go
-00005430: 5f70 726f 6772 616d 203d 204e 6f6e 650a  _program = None.
-00005440: 2020 2020 7365 6c66 2e67 7569 203d 2054      self.gui = T
-00005450: 7275 650a 2020 2020 7365 6c66 2e68 6967  rue.    self.hig
-00005460: 686c 6967 6874 203d 204e 6f6e 650a 2020  hlight = None.  
-00005470: 2020 7365 6c66 2e69 6e64 656e 7420 3d20    self.indent = 
-00005480: 4e6f 6e65 0a20 2020 2073 656c 662e 6974  None.    self.it
-00005490: 616c 6963 697a 6520 3d20 4e6f 6e65 0a20  alicize = None. 
-000054a0: 2020 2073 656c 662e 6e61 6d65 645f 6974     self.named_it
-000054b0: 656d 203d 204e 6f6e 650a 2020 2020 7365  em = None.    se
-000054c0: 6c66 2e72 6572 756e 203d 204e 6f6e 650a  lf.rerun = None.
-000054d0: 2020 2020 7365 6c66 2e72 6573 6574 203d      self.reset =
-000054e0: 204e 6f6e 650a 2020 2020 7365 6c66 2e72   None.    self.r
-000054f0: 6573 746f 7265 203d 2046 616c 7365 0a20  estore = False. 
-00005500: 2020 2073 656c 662e 7275 6e74 696d 6520     self.runtime 
-00005510: 3d20 4661 6c73 650a 2020 2020 7365 6c66  = False.    self
-00005520: 2e73 6176 6520 3d20 4661 6c73 650a 2020  .save = False.  
-00005530: 2020 7365 6c66 2e73 696e 676c 655f 7072    self.single_pr
-00005540: 6f66 696c 655f 6e61 6d65 203d 204e 6f6e  ofile_name = Non
-00005550: 650a 2020 2020 7365 6c66 2e73 696e 676c  e.    self.singl
-00005560: 655f 7072 6f6a 6563 745f 6e61 6d65 203d  e_project_name =
-00005570: 204e 6f6e 650a 2020 2020 7365 6c66 2e73   None.    self.s
-00005580: 696e 676c 655f 7461 736b 5f6e 616d 6520  ingle_task_name 
-00005590: 3d20 4e6f 6e65 0a20 2020 2073 656c 662e  = None.    self.
-000055a0: 7477 6973 7479 203d 204e 6f6e 650a 2020  twisty = None.  
-000055b0: 2020 7365 6c66 2e75 6e64 6572 6c69 6e65    self.underline
-000055c0: 203d 204e 6f6e 650a 2020 2020 7365 6c66   = None.    self
-000055d0: 2e6f 7574 6c69 6e65 203d 2046 616c 7365  .outline = False
-000055e0: 0a20 2020 2073 656c 662e 7072 6574 7479  .    self.pretty
-000055f0: 203d 2046 616c 7365 0a20 2020 2073 656c   = False.    sel
-00005600: 662e 746f 706c 6576 656c 5f77 696e 646f  f.toplevel_windo
-00005610: 7720 3d20 4e6f 6e65 0a20 2020 2050 7269  w = None.    Pri
-00005620: 6d65 4974 656d 732e 7072 6f67 7261 6d5f  meItems.program_
-00005630: 6172 6775 6d65 6e74 735b 2267 7569 225d  arguments["gui"]
-00005640: 203d 2054 7275 650a 2020 2020 7365 6c66   = True.    self
-00005650: 2e6c 6973 745f 6669 6c65 7320 3d20 4661  .list_files = Fa
-00005660: 6c73 650a 2020 2020 7365 6c66 2e61 695f  lse.    self.ai_
-00005670: 6170 696b 6579 203d 204e 6f6e 650a 2020  apikey = None.  
-00005680: 2020 7365 6c66 2e61 695f 6d6f 6465 6c20    self.ai_model 
-00005690: 3d20 4e6f 6e65 0a20 2020 2073 656c 662e  = None.    self.
-000056a0: 6169 5f61 6e61 6c79 7369 7320 3d20 4e6f  ai_analysis = No
-000056b0: 6e65 0a20 2020 2073 656c 662e 6169 5f6d  ne.    self.ai_m
-000056c0: 6973 7369 6e67 5f6d 6f64 756c 6520 3d20  issing_module = 
-000056d0: 4e6f 6e65 0a0a 2020 2020 7365 6c66 2e74  None..    self.t
-000056e0: 6974 6c65 2822 4d61 7054 6173 6b65 7220  itle("MapTasker 
-000056f0: 5275 6e74 696d 6520 4f70 7469 6f6e 7322  Runtime Options"
-00005700: 290a 0a20 2020 2023 2047 6574 2074 6865  )..    # Get the
-00005710: 2073 6372 6565 6e20 7369 7a65 0a20 2020   screen size.   
-00005720: 2073 6372 6565 6e5f 7769 6474 6820 3d20   screen_width = 
-00005730: 7365 6c66 2e77 696e 666f 5f73 6372 6565  self.winfo_scree
-00005740: 6e77 6964 7468 2829 0a20 2020 2073 6372  nwidth().    scr
-00005750: 6565 6e5f 6865 6967 6874 203d 2073 656c  een_height = sel
-00005760: 662e 7769 6e66 6f5f 7363 7265 656e 6865  f.winfo_screenhe
-00005770: 6967 6874 2829 0a0a 2020 2020 2320 4f76  ight()..    # Ov
-00005780: 6572 616c 6c20 7769 6e64 6f77 2064 696d  erall window dim
-00005790: 656e 7369 6f6e 730a 2020 2020 7365 6c66  ensions.    self
-000057a0: 2e67 656f 6d65 7472 7928 6622 3131 3030  .geometry(f"1100
-000057b0: 7839 3030 2b7b 7363 7265 656e 5f77 6964  x900+{screen_wid
-000057c0: 7468 2f2f 347d 2b7b 7363 7265 656e 5f68  th//4}+{screen_h
-000057d0: 6569 6768 742f 2f36 7d22 290a 0a20 2020  eight//6}")..   
-000057e0: 2023 2063 6f6e 6669 6775 7265 2067 7269   # configure gri
-000057f0: 6420 6c61 796f 7574 2028 3478 3429 0a20  d layout (4x4). 
-00005800: 2020 2073 656c 662e 6772 6964 5f63 6f6c     self.grid_col
-00005810: 756d 6e63 6f6e 6669 6775 7265 2831 2c20  umnconfigure(1, 
-00005820: 7765 6967 6874 3d31 290a 2020 2020 7365  weight=1).    se
-00005830: 6c66 2e67 7269 645f 636f 6c75 6d6e 636f  lf.grid_columnco
-00005840: 6e66 6967 7572 6528 2832 2c20 3329 2c20  nfigure((2, 3), 
-00005850: 7765 6967 6874 3d30 290a 2020 2020 7365  weight=0).    se
-00005860: 6c66 2e67 7269 645f 726f 7763 6f6e 6669  lf.grid_rowconfi
-00005870: 6775 7265 2828 302c 2033 292c 2077 6569  gure((0, 3), wei
-00005880: 6768 743d 3129 0a0a 2020 2020 2320 6c6f  ght=1)..    # lo
-00005890: 6164 2061 6e64 2063 7265 6174 6520 6261  ad and create ba
-000058a0: 636b 6772 6f75 6e64 2069 6d61 6765 0a0a  ckground image..
-000058b0: 2020 2020 2320 6372 6561 7465 2073 6964      # create sid
-000058c0: 6562 6172 2066 7261 6d65 2077 6974 6820  ebar frame with 
-000058d0: 7769 6467 6574 7320 6f6e 2074 6865 206c  widgets on the l
-000058e0: 6566 7420 7369 6465 206f 6620 7468 6520  eft side of the 
-000058f0: 7769 6e64 6f77 2e0a 2020 2020 7365 6c66  window..    self
-00005900: 2e73 6964 6562 6172 5f66 7261 6d65 203d  .sidebar_frame =
-00005910: 2063 746b 2e43 546b 4672 616d 6528 7365   ctk.CTkFrame(se
-00005920: 6c66 2c20 7769 6474 683d 3134 302c 2063  lf, width=140, c
-00005930: 6f72 6e65 725f 7261 6469 7573 3d30 290a  orner_radius=0).
-00005940: 2020 2020 7365 6c66 2e73 6964 6562 6172      self.sidebar
-00005950: 5f66 7261 6d65 2e63 6f6e 6669 6775 7265  _frame.configure
-00005960: 2862 675f 636f 6c6f 723d 2262 6c61 636b  (bg_color="black
-00005970: 2229 0a20 2020 2073 656c 662e 7369 6465  ").    self.side
-00005980: 6261 725f 6672 616d 652e 6772 6964 2872  bar_frame.grid(r
-00005990: 6f77 3d30 2c20 636f 6c75 6d6e 3d30 2c20  ow=0, column=0, 
-000059a0: 726f 7773 7061 6e3d 3137 2c20 7374 6963  rowspan=17, stic
-000059b0: 6b79 3d22 6e73 6577 2229 0a20 2020 2023  ky="nsew").    #
-000059c0: 2044 6566 696e 6520 7369 6465 6261 7220   Define sidebar 
-000059d0: 6261 636b 6772 6f75 6e64 2066 7261 6d65  background frame
-000059e0: 2077 6974 6820 3137 2072 6f77 730a 2020   with 17 rows.  
-000059f0: 2020 7365 6c66 2e73 6964 6562 6172 5f66    self.sidebar_f
-00005a00: 7261 6d65 2e67 7269 645f 726f 7763 6f6e  rame.grid_rowcon
-00005a10: 6669 6775 7265 2831 372c 2077 6569 6768  figure(17, weigh
-00005a20: 743d 3129 0a0a 0a23 2023 2323 2323 2323  t=1)...# #######
-00005a30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005a60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005a70: 2323 2323 2323 2323 2323 230a 2320 4164  ###########.# Ad
-00005a80: 6420 7468 6520 4d61 7054 6173 6b65 7220  d the MapTasker 
-00005a90: 6963 6f6e 2074 6f20 7468 6520 7363 7265  icon to the scre
-00005aa0: 656e 0a23 2023 2323 2323 2323 2323 2323  en.# ###########
-00005ab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005ac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005ad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005ae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005af0: 2323 2323 2323 230a 6465 6620 6164 645f  #######.def add_
-00005b00: 6c6f 676f 2873 656c 6629 202d 3e20 4e6f  logo(self) -> No
-00005b10: 6e65 3a20 2023 206e 6f71 613a 2041 4e4e  ne:  # noqa: ANN
-00005b20: 3030 310a 2020 2020 2222 2246 756e 6374  001.    """Funct
-00005b30: 696f 6e3a 0a20 2020 2020 2020 2061 6464  ion:.        add
-00005b40: 5f6c 6f67 6f0a 2020 2020 5061 7261 6d65  _logo.    Parame
-00005b50: 7465 7273 3a0a 2020 2020 2020 2020 2d20  ters:.        - 
-00005b60: 7365 6c66 2028 6f62 6a65 6374 293a 2054  self (object): T
-00005b70: 6865 206f 626a 6563 7420 7468 6174 2074  he object that t
-00005b80: 6865 2066 756e 6374 696f 6e20 6973 2062  he function is b
-00005b90: 6569 6e67 2063 616c 6c65 6420 6f6e 2e0a  eing called on..
-00005ba0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00005bb0: 2020 2020 202d 204e 6f6e 653a 2054 6865       - None: The
-00005bc0: 2066 756e 6374 696f 6e20 646f 6573 206e   function does n
-00005bd0: 6f74 2072 6574 7572 6e20 616e 7974 6869  ot return anythi
-00005be0: 6e67 2e0a 2020 2020 5072 6f63 6573 7369  ng..    Processi
-00005bf0: 6e67 204c 6f67 6963 3a0a 2020 2020 2020  ng Logic:.      
-00005c00: 2020 2d20 4765 7420 7468 6520 7061 7468    - Get the path
-00005c10: 2074 6f20 6f75 7220 6c6f 676f 732e 0a20   to our logos.. 
-00005c20: 2020 2020 2020 202d 2053 7769 7463 6820         - Switch 
-00005c30: 746f 206f 7572 2074 656d 7020 6469 7265  to our temp dire
-00005c40: 6374 6f72 7920 2861 7373 6574 7329 2e0a  ctory (assets)..
-00005c50: 2020 2020 2020 2020 2d20 4372 6561 7465          - Create
-00005c60: 2061 2043 546b 496d 6167 6520 6f62 6a65   a CTkImage obje
-00005c70: 6374 2074 6f20 6469 7370 6c61 7920 7468  ct to display th
-00005c80: 6520 6c6f 676f 2e0a 2020 2020 2020 2020  e logo..        
-00005c90: 2d20 5472 7920 746f 2064 6973 706c 6179  - Try to display
-00005ca0: 2074 6865 206c 6f67 6f20 7769 7468 2061   the logo with a
-00005cb0: 2043 546b 4c61 6265 6c2e 0a20 2020 2020   CTkLabel..     
-00005cc0: 2020 202d 2053 7769 7463 6820 6261 636b     - Switch back
-00005cd0: 2074 6f20 7072 6f70 6572 2064 6972 6563   to proper direc
-00005ce0: 746f 7279 2e22 2222 0a20 2020 2023 2041  tory.""".    # A
-00005cf0: 6464 206f 7572 206c 6f67 6f0a 2020 2020  dd our logo.    
-00005d00: 2320 4765 7420 7468 6520 7061 7468 2074  # Get the path t
-00005d10: 6f20 6f75 7220 6c6f 676f 733a 0a20 2020  o our logos:.   
-00005d20: 2023 2063 7572 7265 6e74 5f64 6972 203d   # current_dir =
-00005d30: 2064 6972 6563 746f 7279 2066 726f 6d20   directory from 
-00005d40: 7768 6963 6820 7765 2061 7265 2072 756e  which we are run
-00005d50: 6e69 6e67 2e0a 2020 2020 2320 6162 7370  ning..    # absp
-00005d60: 6174 6820 3d20 7061 7468 206f 6620 7468  ath = path of th
-00005d70: 6973 2073 6f75 7263 6520 636f 6465 2028  is source code (
-00005d80: 7573 6572 696e 7472 2e70 7929 2e0a 2020  userintr.py)..  
-00005d90: 2020 2320 6377 6420 3d20 6469 7265 6374    # cwd = direct
-00005da0: 6f72 7920 6672 6f6d 2077 6869 6368 2074  ory from which t
-00005db0: 6865 206d 6169 6e20 7072 6f67 7261 6d20  he main program 
-00005dc0: 6973 2028 6d61 696e 2e70 7929 0a20 2020  is (main.py).   
-00005dd0: 2023 2064 6e61 6d65 203d 2064 6972 6563   # dname = direc
-00005de0: 746f 7279 206f 6620 7372 630a 2020 2020  tory of src.    
-00005df0: 6375 7272 656e 745f 6469 7220 3d20 6f73  current_dir = os
-00005e00: 2e67 6574 6377 6428 290a 2020 2020 6162  .getcwd().    ab
-00005e10: 7370 6174 6820 3d20 6f73 2e70 6174 682e  spath = os.path.
-00005e20: 6162 7370 6174 6828 5f5f 6669 6c65 5f5f  abspath(__file__
-00005e30: 290a 2020 2020 2320 6377 6420 3d20 6f73  ).    # cwd = os
-00005e40: 2e70 6174 682e 6162 7370 6174 6828 6f73  .path.abspath(os
-00005e50: 2e70 6174 682e 6469 726e 616d 6528 7379  .path.dirname(sy
-00005e60: 732e 6172 6776 5b30 5d29 290a 2020 2020  s.argv[0])).    
-00005e70: 646e 616d 6520 3d20 6f73 2e70 6174 682e  dname = os.path.
-00005e80: 6469 726e 616d 6528 6162 7370 6174 6829  dirname(abspath)
-00005e90: 0a20 2020 2074 656d 705f 6469 7220 3d20  .    temp_dir = 
-00005ea0: 646e 616d 652e 7265 706c 6163 6528 2273  dname.replace("s
-00005eb0: 7263 222c 2022 6173 7365 7473 2229 0a20  rc", "assets"). 
-00005ec0: 2020 2023 2053 7769 7463 6820 746f 206f     # Switch to o
-00005ed0: 7572 2074 656d 7020 6469 7265 6374 6f72  ur temp director
-00005ee0: 7920 2861 7373 6574 7329 0a20 2020 206f  y (assets).    o
-00005ef0: 732e 6368 6469 7228 7465 6d70 5f64 6972  s.chdir(temp_dir
-00005f00: 290a 0a20 2020 2023 2043 7265 6174 6520  )..    # Create 
-00005f10: 6120 4354 6b49 6d61 6765 206f 626a 6563  a CTkImage objec
-00005f20: 7420 746f 2064 6973 706c 6179 2074 6865  t to display the
-00005f30: 206c 6f67 6f0a 2020 2020 6d79 5f69 6d61   logo.    my_ima
-00005f40: 6765 203d 2063 746b 2e43 546b 496d 6167  ge = ctk.CTkImag
-00005f50: 6528 0a20 2020 2020 2020 206c 6967 6874  e(.        light
-00005f60: 5f69 6d61 6765 3d49 6d61 6765 2e6f 7065  _image=Image.ope
-00005f70: 6e28 226d 6170 7461 736b 6572 5f6c 6f67  n("maptasker_log
-00005f80: 6f5f 6c69 6768 742e 706e 6722 292c 0a20  o_light.png"),. 
-00005f90: 2020 2020 2020 2064 6172 6b5f 696d 6167         dark_imag
-00005fa0: 653d 496d 6167 652e 6f70 656e 2822 6d61  e=Image.open("ma
-00005fb0: 7074 6173 6b65 725f 6c6f 676f 5f64 6172  ptasker_logo_dar
-00005fc0: 6b2e 706e 6722 292c 0a20 2020 2020 2020  k.png"),.       
-00005fd0: 2073 697a 653d 2831 3930 2c20 3530 292c   size=(190, 50),
-00005fe0: 0a20 2020 2029 0a20 2020 2074 7279 3a0a  .    ).    try:.
-00005ff0: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
-00006000: 6f5f 6c61 6265 6c20 3d20 6374 6b2e 4354  o_label = ctk.CT
-00006010: 6b4c 6162 656c 280a 2020 2020 2020 2020  kLabel(.        
-00006020: 2020 2020 7365 6c66 2e73 6964 6562 6172      self.sidebar
-00006030: 5f66 7261 6d65 2c0a 2020 2020 2020 2020  _frame,.        
-00006040: 2020 2020 696d 6167 653d 6d79 5f69 6d61      image=my_ima
-00006050: 6765 2c0a 2020 2020 2020 2020 2020 2020  ge,.            
-00006060: 7465 7874 3d22 222c 0a20 2020 2020 2020  text="",.       
-00006070: 2020 2020 2063 6f6d 706f 756e 643d 226c       compound="l
-00006080: 6566 7422 2c0a 2020 2020 2020 2020 2020  eft",.          
-00006090: 2020 666f 6e74 3d63 746b 2e43 546b 466f    font=ctk.CTkFo
-000060a0: 6e74 2873 697a 653d 312c 2077 6569 6768  nt(size=1, weigh
-000060b0: 743d 2262 6f6c 6422 292c 0a20 2020 2020  t="bold"),.     
-000060c0: 2020 2029 2020 2320 6469 7370 6c61 7920     )  # display 
-000060d0: 696d 6167 6520 7769 7468 2061 2043 546b  image with a CTk
-000060e0: 4c61 6265 6c0a 2020 2020 2020 2020 7365  Label.        se
-000060f0: 6c66 2e6c 6f67 6f5f 6c61 6265 6c2e 6772  lf.logo_label.gr
-00006100: 6964 2872 6f77 3d30 2c20 636f 6c75 6d6e  id(row=0, column
-00006110: 3d30 2c20 7061 6478 3d30 2c20 7061 6479  =0, padx=0, pady
-00006120: 3d30 2c20 7374 6963 6b79 3d22 6e22 290a  =0, sticky="n").
-00006130: 2020 2020 6578 6365 7074 3a20 2023 206e      except:  # n
-00006140: 6f71 613a 2053 3131 300a 2020 2020 2020  oqa: S110.      
-00006150: 2020 7061 7373 0a20 2020 2023 2064 656c    pass.    # del
-00006160: 206d 795f 696d 6167 6520 2023 2044 6f6e   my_image  # Don
-00006170: 6520 7769 7468 2069 6d61 6765 2e2e 2e67  e with image...g
-00006180: 6574 2072 6964 206f 6620 6974 2e0a 0a20  et rid of it... 
-00006190: 2020 2023 2053 7769 7463 6820 6261 636b     # Switch back
-000061a0: 2074 6f20 7072 6f70 6572 2064 6972 6563   to proper direc
-000061b0: 746f 7279 0a20 2020 206f 732e 6368 6469  tory.    os.chdi
-000061c0: 7228 6375 7272 656e 745f 6469 7229 0a0a  r(current_dir)..
-000061d0: 0a23 2023 2323 2323 2323 2323 2323 2323  .# #############
-000061e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000061f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006220: 2323 2323 230a 2320 4372 6561 7465 2061  #####.# Create a
-00006230: 206c 6162 656c 2067 656e 6572 616c 2072   label general r
-00006240: 6f75 7469 6e65 0a23 2023 2323 2323 2323  outine.# #######
-00006250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006260: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006270: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006280: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006290: 2323 2323 2323 2323 2323 230a 6465 6620  ###########.def 
-000062a0: 6164 645f 6c61 6265 6c28 0a20 2020 2073  add_label(.    s
-000062b0: 656c 662c 2020 2320 6e6f 7161 3a20 414e  elf,  # noqa: AN
-000062c0: 4e30 3031 2c20 4152 4730 3031 0a20 2020  N001, ARG001.   
-000062d0: 2066 7261 6d65 3a20 6374 6b2e 4354 6b46   frame: ctk.CTkF
-000062e0: 7261 6d65 2c0a 2020 2020 7465 7874 3a20  rame,.    text: 
-000062f0: 7374 722c 0a20 2020 2074 6578 745f 636f  str,.    text_co
-00006300: 6c6f 723a 2073 7472 2c0a 2020 2020 666f  lor: str,.    fo
-00006310: 6e74 5f73 697a 653a 2069 6e74 2c0a 2020  nt_size: int,.  
-00006320: 2020 666f 6e74 5f77 6569 6768 743a 2073    font_weight: s
-00006330: 7472 2c0a 2020 2020 726f 773a 2069 6e74  tr,.    row: int
-00006340: 2c0a 2020 2020 636f 6c75 6d6e 3a20 696e  ,.    column: in
-00006350: 742c 0a20 2020 2070 6164 783a 2074 7570  t,.    padx: tup
-00006360: 6c65 2c0a 2020 2020 7061 6479 3a20 7475  le,.    pady: tu
-00006370: 706c 652c 0a20 2020 2073 7469 636b 793a  ple,.    sticky:
-00006380: 2073 7472 2c0a 2920 2d3e 204e 6f6e 653a   str,.) -> None:
-00006390: 0a20 2020 2022 2222 4164 6473 2061 2063  .    """Adds a c
-000063a0: 7573 746f 6d20 6c61 6265 6c20 746f 2061  ustom label to a
-000063b0: 2063 7573 746f 6d20 746b 696e 7465 7220   custom tkinter 
-000063c0: 6672 616d 652e 0a20 2020 2050 6172 616d  frame..    Param
-000063d0: 6574 6572 733a 0a20 2020 2020 2020 202d  eters:.        -
-000063e0: 2066 7261 6d65 2028 6374 6b2e 4354 6b46   frame (ctk.CTkF
-000063f0: 7261 6d65 293a 2054 6865 2066 7261 6d65  rame): The frame
-00006400: 2074 6f20 6164 6420 7468 6520 6c61 6265   to add the labe
-00006410: 6c20 746f 2e0a 2020 2020 2020 2020 2d20  l to..        - 
-00006420: 6e61 6d65 2028 6374 6b2e 4354 6b4c 6162  name (ctk.CTkLab
-00006430: 656c 293a 2054 6865 206c 6162 656c 2074  el): The label t
-00006440: 6f20 6265 2061 6464 6564 2e0a 2020 2020  o be added..    
-00006450: 2020 2020 2d20 7465 7874 2028 7374 7229      - text (str)
-00006460: 3a20 5468 6520 7465 7874 2074 6f20 6265  : The text to be
-00006470: 2064 6973 706c 6179 6564 206f 6e20 7468   displayed on th
-00006480: 6520 6c61 6265 6c2e 0a20 2020 2020 2020  e label..       
-00006490: 202d 2074 6578 745f 636f 6c6f 7220 2873   - text_color (s
-000064a0: 7472 293a 2063 6f6c 6f72 2066 6f72 2074  tr): color for t
-000064b0: 6865 2074 6578 740a 2020 2020 2020 2020  he text.        
-000064c0: 2d20 666f 6e74 5f73 697a 6520 2869 6e74  - font_size (int
-000064d0: 293a 2054 6865 2066 6f6e 7420 7369 7a65  ): The font size
-000064e0: 206f 6620 7468 6520 6c61 6265 6c2e 0a20   of the label.. 
-000064f0: 2020 2020 2020 202d 2066 6f6e 745f 7765         - font_we
-00006500: 6967 6874 2028 7374 7229 3a20 5468 6520  ight (str): The 
-00006510: 666f 6e74 2077 6569 6768 7420 6f66 2074  font weight of t
-00006520: 6865 206c 6162 656c 2e0a 2020 2020 2020  he label..      
-00006530: 2020 2d20 726f 7720 2869 6e74 293a 2054    - row (int): T
-00006540: 6865 2072 6f77 206e 756d 6265 7220 746f  he row number to
-00006550: 2070 6c61 6365 2074 6865 206c 6162 656c   place the label
-00006560: 2069 6e2e 0a20 2020 2020 2020 202d 2063   in..        - c
-00006570: 6f6c 756d 6e20 2869 6e74 293a 2054 6865  olumn (int): The
-00006580: 2063 6f6c 756d 6e20 6e75 6d62 6572 2074   column number t
-00006590: 6f20 706c 6163 6520 7468 6520 6c61 6265  o place the labe
-000065a0: 6c20 696e 2e0a 2020 2020 2020 2020 2d20  l in..        - 
-000065b0: 7061 6478 2028 7475 706c 6529 3a20 5468  padx (tuple): Th
-000065c0: 6520 686f 7269 7a6f 6e74 616c 2070 6164  e horizontal pad
-000065d0: 6469 6e67 206f 6620 7468 6520 6c61 6265  ding of the labe
-000065e0: 6c2e 0a20 2020 2020 2020 202d 2070 6164  l..        - pad
-000065f0: 7920 2874 7570 6c65 293a 2054 6865 2076  y (tuple): The v
-00006600: 6572 7469 6361 6c20 7061 6464 696e 6720  ertical padding 
-00006610: 6f66 2074 6865 206c 6162 656c 2e0a 2020  of the label..  
-00006620: 2020 2020 2020 2d20 7374 6963 6b79 2028        - sticky (
-00006630: 7374 7229 3a20 5468 6520 616c 6967 6e6d  str): The alignm
-00006640: 656e 7420 6f66 2074 6865 206c 6162 656c  ent of the label
-00006650: 2077 6974 6869 6e20 6974 7320 6772 6964   within its grid
-00006660: 2063 656c 6c2e 0a20 2020 2052 6574 7572   cell..    Retur
-00006670: 6e73 3a0a 2020 2020 2020 2020 2d20 6c61  ns:.        - la
-00006680: 6265 6c5f 6e61 6d65 2028 7374 7229 3a20  bel_name (str): 
-00006690: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-000066a0: 6c61 6265 6c2e 0a20 2020 2050 726f 6365  label..    Proce
-000066b0: 7373 696e 6720 4c6f 6769 633a 0a20 2020  ssing Logic:.   
-000066c0: 2020 2020 202d 2043 7265 6174 6573 2061       - Creates a
-000066d0: 2063 7573 746f 6d20 6c61 6265 6c20 7769   custom label wi
-000066e0: 7468 2074 6865 2067 6976 656e 2070 6172  th the given par
-000066f0: 616d 6574 6572 732e 0a20 2020 2020 2020  ameters..       
-00006700: 202d 2050 6c61 6365 7320 7468 6520 6c61   - Places the la
-00006710: 6265 6c20 696e 2074 6865 2073 7065 6369  bel in the speci
-00006720: 6669 6564 2072 6f77 2061 6e64 2063 6f6c  fied row and col
-00006730: 756d 6e20 6f66 2074 6865 2066 7261 6d65  umn of the frame
-00006740: 2e0a 2020 2020 2020 2020 2d20 4164 6473  ..        - Adds
-00006750: 2068 6f72 697a 6f6e 7461 6c20 616e 6420   horizontal and 
-00006760: 7665 7274 6963 616c 2070 6164 6469 6e67  vertical padding
-00006770: 2074 6f20 7468 6520 6c61 6265 6c2e 0a20   to the label.. 
-00006780: 2020 2020 2020 202d 2041 6c69 676e 7320         - Aligns 
-00006790: 7468 6520 6c61 6265 6c20 7769 7468 696e  the label within
-000067a0: 2069 7473 2067 7269 6420 6365 6c6c 2e22   its grid cell."
-000067b0: 2222 0a20 2020 2069 6620 6e6f 7420 666f  "".    if not fo
-000067c0: 6e74 5f73 697a 6520 6f72 2066 6f6e 745f  nt_size or font_
-000067d0: 7369 7a65 203d 3d20 303a 0a20 2020 2020  size == 0:.     
-000067e0: 2020 2066 6f6e 745f 7369 7a65 203d 2064     font_size = d
-000067f0: 6566 6175 6c74 5f66 6f6e 745f 7369 7a65  efault_font_size
-00006800: 0a20 2020 2069 6620 6e6f 7420 7465 7874  .    if not text
-00006810: 5f63 6f6c 6f72 3a0a 2020 2020 2020 2020  _color:.        
-00006820: 7465 7874 5f63 6f6c 6f72 203d 2022 2346  text_color = "#F
-00006830: 4646 4646 4622 0a20 2020 206c 6162 656c  FFFFF".    label
-00006840: 5f6e 616d 6520 3d20 6374 6b2e 4354 6b4c  _name = ctk.CTkL
-00006850: 6162 656c 280a 2020 2020 2020 2020 6672  abel(.        fr
-00006860: 616d 652c 0a20 2020 2020 2020 2074 6578  ame,.        tex
-00006870: 743d 7465 7874 2c0a 2020 2020 2020 2020  t=text,.        
-00006880: 7465 7874 5f63 6f6c 6f72 3d74 6578 745f  text_color=text_
-00006890: 636f 6c6f 722c 0a20 2020 2020 2020 2066  color,.        f
-000068a0: 6f6e 743d 6374 6b2e 4354 6b46 6f6e 7428  ont=ctk.CTkFont(
-000068b0: 7369 7a65 3d66 6f6e 745f 7369 7a65 2c20  size=font_size, 
-000068c0: 7765 6967 6874 3d66 6f6e 745f 7765 6967  weight=font_weig
-000068d0: 6874 292c 0a20 2020 2029 0a20 2020 206c  ht),.    ).    l
-000068e0: 6162 656c 5f6e 616d 652e 6772 6964 2872  abel_name.grid(r
-000068f0: 6f77 3d72 6f77 2c20 636f 6c75 6d6e 3d63  ow=row, column=c
-00006900: 6f6c 756d 6e2c 2070 6164 783d 7061 6478  olumn, padx=padx
-00006910: 2c20 7061 6479 3d70 6164 792c 2073 7469  , pady=pady, sti
-00006920: 636b 793d 7374 6963 6b79 290a 2020 2020  cky=sticky).    
-00006930: 7265 7475 726e 206c 6162 656c 5f6e 616d  return label_nam
-00006940: 650a 0a0a 2320 2323 2323 2323 2323 2323  e...# ##########
-00006950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006960: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006970: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006980: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006990: 2323 2323 2323 2323 0a23 2043 7265 6174  ########.# Creat
-000069a0: 6520 6120 6368 6563 6b62 6f78 2067 656e  e a checkbox gen
-000069b0: 6572 616c 2072 6f75 7469 6e65 0a23 2023  eral routine.# #
-000069c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000069d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000069e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000069f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006a00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006a10: 230a 6465 6620 6164 645f 6368 6563 6b62  #.def add_checkb
-00006a20: 6f78 280a 2020 2020 7365 6c66 2c20 2023  ox(.    self,  #
-00006a30: 206e 6f71 613a 2041 4e4e 3030 312c 2041   noqa: ANN001, A
-00006a40: 5247 3030 310a 2020 2020 6672 616d 653a  RG001.    frame:
-00006a50: 2063 746b 2e43 546b 4672 616d 652c 0a20   ctk.CTkFrame,. 
-00006a60: 2020 2063 6f6d 6d61 6e64 3a20 6f62 6a65     command: obje
-00006a70: 6374 2c0a 2020 2020 7465 7874 3a20 7374  ct,.    text: st
-00006a80: 722c 0a20 2020 2072 6f77 3a20 696e 742c  r,.    row: int,
-00006a90: 0a20 2020 2063 6f6c 756d 6e3a 2069 6e74  .    column: int
-00006aa0: 2c0a 2020 2020 7061 6478 3a20 7475 706c  ,.    padx: tupl
-00006ab0: 652c 0a20 2020 2070 6164 793a 2074 7570  e,.    pady: tup
-00006ac0: 6c65 2c0a 2020 2020 7374 6963 6b79 3a20  le,.    sticky: 
-00006ad0: 7374 722c 0a20 2020 2062 6f72 6465 725f  str,.    border_
-00006ae0: 636f 6c6f 723a 2073 7472 2c0a 2920 2d3e  color: str,.) ->
-00006af0: 204e 6f6e 653a 0a20 2020 2022 2222 4164   None:.    """Ad
-00006b00: 6420 6120 6368 6563 6b62 6f78 2074 6f20  d a checkbox to 
-00006b10: 6120 6375 7374 6f6d 2074 6b69 6e74 6572  a custom tkinter
-00006b20: 2066 7261 6d65 2e0a 2020 2020 5061 7261   frame..    Para
-00006b30: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
-00006b40: 2d20 6672 616d 6520 2863 746b 2e43 546b  - frame (ctk.CTk
-00006b50: 4672 616d 6529 3a20 5468 6520 6375 7374  Frame): The cust
-00006b60: 6f6d 2074 6b69 6e74 6572 2066 7261 6d65  om tkinter frame
-00006b70: 2074 6f20 6164 6420 7468 6520 6368 6563   to add the chec
-00006b80: 6b62 6f78 2074 6f2e 0a20 2020 2020 2020  kbox to..       
-00006b90: 202d 2063 6f6d 6d61 6e64 2028 6f62 6a65   - command (obje
-00006ba0: 6374 293a 2054 6865 2063 6f6d 6d61 6e64  ct): The command
-00006bb0: 2074 6f20 6265 2065 7865 6375 7465 6420   to be executed 
-00006bc0: 7768 656e 2074 6865 2063 6865 636b 626f  when the checkbo
-00006bd0: 7820 6973 2063 6c69 636b 6564 2e0a 2020  x is clicked..  
-00006be0: 2020 2020 2020 2d20 7465 7874 2028 7374        - text (st
-00006bf0: 7229 3a20 5468 6520 7465 7874 2074 6f20  r): The text to 
-00006c00: 6265 2064 6973 706c 6179 6564 206e 6578  be displayed nex
-00006c10: 7420 746f 2074 6865 2063 6865 636b 626f  t to the checkbo
-00006c20: 782e 0a20 2020 2020 2020 202d 2072 6f77  x..        - row
-00006c30: 2028 696e 7429 3a20 5468 6520 726f 7720   (int): The row 
-00006c40: 746f 2070 6c61 6365 2074 6865 2063 6865  to place the che
-00006c50: 636b 626f 7820 696e 2e0a 2020 2020 2020  ckbox in..      
-00006c60: 2020 2d20 636f 6c75 6d6e 2028 696e 7429    - column (int)
-00006c70: 3a20 5468 6520 636f 6c75 6d6e 2074 6f20  : The column to 
-00006c80: 706c 6163 6520 7468 6520 6368 6563 6b62  place the checkb
-00006c90: 6f78 2069 6e2e 0a20 2020 2020 2020 202d  ox in..        -
-00006ca0: 2070 6164 7820 2874 7570 6c65 293a 2054   padx (tuple): T
-00006cb0: 6865 2068 6f72 697a 6f6e 7461 6c20 7061  he horizontal pa
-00006cc0: 6464 696e 6720 666f 7220 7468 6520 6368  dding for the ch
-00006cd0: 6563 6b62 6f78 2e0a 2020 2020 2020 2020  eckbox..        
-00006ce0: 2d20 7061 6479 2028 7475 706c 6529 3a20  - pady (tuple): 
-00006cf0: 5468 6520 7665 7274 6963 616c 2070 6164  The vertical pad
-00006d00: 6469 6e67 2066 6f72 2074 6865 2063 6865  ding for the che
-00006d10: 636b 626f 782e 0a20 2020 2020 2020 202d  ckbox..        -
-00006d20: 2073 7469 636b 7920 2873 7472 293a 2054   sticky (str): T
-00006d30: 6865 2061 6c69 676e 6d65 6e74 206f 6620  he alignment of 
-00006d40: 7468 6520 6368 6563 6b62 6f78 2077 6974  the checkbox wit
-00006d50: 6869 6e20 6974 7320 6772 6964 2063 656c  hin its grid cel
-00006d60: 6c2e 0a20 2020 2020 2020 202d 2062 6f72  l..        - bor
-00006d70: 6465 725f 636f 6c6f 7220 2873 7472 293a  der_color (str):
-00006d80: 2054 6865 2063 6f6c 6f72 2074 6f20 6869   The color to hi
-00006d90: 6768 6c69 6768 746e 2074 6865 2062 7574  ghlightn the but
-00006da0: 746f 6e20 7769 7468 2e0a 2020 2020 5265  ton with..    Re
-00006db0: 7475 726e 733a 0a20 2020 2020 2020 202d  turns:.        -
-00006dc0: 2063 6865 636b 626f 785f 6e61 6d65 3a20   checkbox_name: 
-00006dd0: 7468 6520 6e61 6d65 6420 6368 6563 6b62  the named checkb
-00006de0: 6f78 2e0a 2020 2020 5072 6f63 6573 7369  ox..    Processi
-00006df0: 6e67 204c 6f67 6963 3a0a 2020 2020 2020  ng Logic:.      
-00006e00: 2020 2d20 4372 6561 7465 2061 2063 7573    - Create a cus
-00006e10: 746f 6d20 746b 696e 7465 7220 6368 6563  tom tkinter chec
-00006e20: 6b62 6f78 2e0a 2020 2020 2020 2020 2d20  kbox..        - 
-00006e30: 4164 6420 7468 6520 6368 6563 6b62 6f78  Add the checkbox
-00006e40: 2074 6f20 7468 6520 7370 6563 6966 6965   to the specifie
-00006e50: 6420 6672 616d 652e 0a20 2020 2020 2020  d frame..       
-00006e60: 202d 2050 6c61 6365 2074 6865 2063 6865   - Place the che
-00006e70: 636b 626f 7820 696e 2074 6865 2073 7065  ckbox in the spe
-00006e80: 6369 6669 6564 2072 6f77 2061 6e64 2063  cified row and c
-00006e90: 6f6c 756d 6e2e 0a20 2020 2020 2020 202d  olumn..        -
-00006ea0: 2041 7070 6c79 2074 6865 2073 7065 6369   Apply the speci
-00006eb0: 6669 6564 2070 6164 6469 6e67 2074 6f20  fied padding to 
-00006ec0: 7468 6520 6368 6563 6b62 6f78 2e0a 2020  the checkbox..  
-00006ed0: 2020 2020 2020 2d20 416c 6967 6e20 7468        - Align th
-00006ee0: 6520 6368 6563 6b62 6f78 2077 6974 6869  e checkbox withi
-00006ef0: 6e20 6974 7320 6772 6964 2063 656c 6c2e  n its grid cell.
-00006f00: 2222 220a 2020 2020 6368 6563 6b62 6f78  """.    checkbox
-00006f10: 5f6e 616d 6520 3d20 6374 6b2e 4354 6b43  _name = ctk.CTkC
-00006f20: 6865 636b 426f 7828 0a20 2020 2020 2020  heckBox(.       
-00006f30: 2066 7261 6d65 2c0a 2020 2020 2020 2020   frame,.        
-00006f40: 636f 6d6d 616e 643d 636f 6d6d 616e 642c  command=command,
-00006f50: 0a20 2020 2020 2020 2074 6578 743d 7465  .        text=te
-00006f60: 7874 2c0a 2020 2020 2020 2020 666f 6e74  xt,.        font
-00006f70: 3d63 746b 2e43 546b 466f 6e74 2873 697a  =ctk.CTkFont(siz
-00006f80: 653d 6465 6661 756c 745f 666f 6e74 5f73  e=default_font_s
-00006f90: 697a 652c 2077 6569 6768 743d 226e 6f72  ize, weight="nor
-00006fa0: 6d61 6c22 292c 0a20 2020 2020 2020 206f  mal"),.        o
-00006fb0: 6e76 616c 7565 3d54 7275 652c 0a20 2020  nvalue=True,.   
-00006fc0: 2020 2020 206f 6666 7661 6c75 653d 4661       offvalue=Fa
-00006fd0: 6c73 652c 0a20 2020 2029 0a20 2020 2069  lse,.    ).    i
-00006fe0: 6620 626f 7264 6572 5f63 6f6c 6f72 3a0a  f border_color:.
-00006ff0: 2020 2020 2020 2020 6368 6563 6b62 6f78          checkbox
-00007000: 5f6e 616d 652e 636f 6e66 6967 7572 6528  _name.configure(
-00007010: 626f 7264 6572 5f63 6f6c 6f72 3d62 6f72  border_color=bor
-00007020: 6465 725f 636f 6c6f 7229 0a20 2020 2063  der_color).    c
-00007030: 6865 636b 626f 785f 6e61 6d65 2e67 7269  heckbox_name.gri
-00007040: 6428 726f 773d 726f 772c 2063 6f6c 756d  d(row=row, colum
-00007050: 6e3d 636f 6c75 6d6e 2c20 7061 6478 3d70  n=column, padx=p
-00007060: 6164 782c 2070 6164 793d 7061 6479 2c20  adx, pady=pady, 
-00007070: 7374 6963 6b79 3d73 7469 636b 7929 0a20  sticky=sticky). 
-00007080: 2020 2072 6574 7572 6e20 6368 6563 6b62     return checkb
-00007090: 6f78 5f6e 616d 650a 0a0a 2320 2323 2323  ox_name...# ####
-000070a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000070b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000070c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000070d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000070e0: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
-000070f0: 2043 7265 6174 6520 6120 6275 7474 6f6e   Create a button
-00007100: 2067 656e 6572 616c 2072 6f75 7469 6e65   general routine
-00007110: 0a23 2023 2323 2323 2323 2323 2323 2323  .# #############
-00007120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007130: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007140: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007150: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007160: 2323 2323 230a 6465 6620 6164 645f 6275  #####.def add_bu
-00007170: 7474 6f6e 280a 2020 2020 7365 6c66 2c20  tton(.    self, 
-00007180: 2023 206e 6f71 613a 2041 4e4e 3030 312c   # noqa: ANN001,
-00007190: 2041 5247 3030 310a 2020 2020 6672 616d   ARG001.    fram
-000071a0: 653a 2063 746b 2e43 546b 4672 616d 652c  e: ctk.CTkFrame,
-000071b0: 0a20 2020 2066 675f 636f 6c6f 723a 2073  .    fg_color: s
-000071c0: 7472 2c0a 2020 2020 7465 7874 5f63 6f6c  tr,.    text_col
-000071d0: 6f72 3a20 7374 722c 0a20 2020 2062 6f72  or: str,.    bor
-000071e0: 6465 725f 636f 6c6f 723a 2073 7472 2c0a  der_color: str,.
-000071f0: 2020 2020 636f 6d6d 616e 643a 206f 626a      command: obj
-00007200: 6563 742c 0a20 2020 2062 6f72 6465 725f  ect,.    border_
-00007210: 7769 6474 683a 2069 6e74 2c0a 2020 2020  width: int,.    
-00007220: 7465 7874 3a20 7374 722c 0a20 2020 2063  text: str,.    c
-00007230: 6f6c 756d 6e73 7061 6e3a 2069 6e74 2c0a  olumnspan: int,.
-00007240: 2020 2020 726f 773a 2069 6e74 2c0a 2020      row: int,.  
-00007250: 2020 636f 6c75 6d6e 3a20 696e 742c 0a20    column: int,. 
-00007260: 2020 2070 6164 783a 2074 7570 6c65 2c0a     padx: tuple,.
-00007270: 2020 2020 7061 6479 3a20 7475 706c 652c      pady: tuple,
-00007280: 0a20 2020 2073 7469 636b 793a 2073 7472  .    sticky: str
-00007290: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
-000072a0: 2022 2222 4164 6420 6120 6275 7474 6f6e   """Add a button
-000072b0: 2074 6f20 6120 6375 7374 6f6d 2074 6b69   to a custom tki
-000072c0: 6e74 6572 2066 7261 6d65 2e0a 2020 2020  nter frame..    
-000072d0: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
-000072e0: 2020 2020 2d20 6672 616d 6520 2863 746b      - frame (ctk
-000072f0: 2e43 546b 4672 616d 6529 3a20 5468 6520  .CTkFrame): The 
-00007300: 6672 616d 6520 746f 2061 6464 2074 6865  frame to add the
-00007310: 2062 7574 746f 6e20 746f 2e0a 2020 2020   button to..    
-00007320: 2020 2020 2d20 6667 5f63 6f6c 6f72 2028      - fg_color (
-00007330: 7374 7229 3a20 5468 6520 636f 6c6f 7220  str): The color 
-00007340: 6f66 2074 6865 2062 7574 746f 6e27 7320  of the button's 
-00007350: 7465 7874 2e0a 2020 2020 2020 2020 2d20  text..        - 
-00007360: 7465 7874 5f63 6f6c 6f72 2028 7374 7229  text_color (str)
-00007370: 2054 6865 2063 6f6c 6f72 206f 6620 7468   The color of th
-00007380: 6520 6275 7474 6f6e 2773 2074 6578 742e  e button's text.
-00007390: 0a20 2020 2020 2020 202d 2063 6f6d 6d61  .        - comma
-000073a0: 6e64 2028 6f62 6a65 6374 293a 2054 6865  nd (object): The
-000073b0: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-000073c0: 6578 6563 7574 6564 2077 6865 6e20 7468  executed when th
-000073d0: 6520 6275 7474 6f6e 2069 7320 636c 6963  e button is clic
-000073e0: 6b65 642e 0a20 2020 2020 2020 202d 2062  ked..        - b
-000073f0: 6f72 6465 725f 7769 6474 6820 2869 6e74  order_width (int
-00007400: 293a 2054 6865 2077 6964 7468 206f 6620  ): The width of 
-00007410: 7468 6520 6275 7474 6f6e 2773 2062 6f72  the button's bor
-00007420: 6465 722e 0a20 2020 2020 2020 202d 2074  der..        - t
-00007430: 6578 7420 2873 7472 293a 2054 6865 2074  ext (str): The t
-00007440: 6578 7420 746f 2062 6520 6469 7370 6c61  ext to be displa
-00007450: 7965 6420 6f6e 2074 6865 2062 7574 746f  yed on the butto
-00007460: 6e2e 0a20 2020 2020 2020 202d 2063 6f6c  n..        - col
-00007470: 756d 6e73 7061 6e20 2869 6e74 293a 2054  umnspan (int): T
-00007480: 6865 206e 756d 6265 7220 6f66 2063 6f6c  he number of col
-00007490: 756d 6e73 2074 6f20 7370 616e 2074 6865  umns to span the
-000074a0: 2062 7574 746f 6e20 6163 726f 7373 2e0a   button across..
-000074b0: 2020 2020 2020 2020 2d20 726f 7720 2869          - row (i
-000074c0: 6e74 293a 2054 6865 2072 6f77 2074 6f20  nt): The row to 
-000074d0: 706c 6163 6520 7468 6520 6275 7474 6f6e  place the button
-000074e0: 2069 6e2e 0a20 2020 2020 2020 202d 2063   in..        - c
-000074f0: 6f6c 756d 6e20 2869 6e74 293a 2054 6865  olumn (int): The
-00007500: 2063 6f6c 756d 6e20 746f 2070 6c61 6365   column to place
-00007510: 2074 6865 2062 7574 746f 6e20 696e 2e0a   the button in..
-00007520: 2020 2020 2020 2020 2d20 7061 6478 2028          - padx (
-00007530: 7475 706c 6529 3a20 5468 6520 616d 6f75  tuple): The amou
-00007540: 6e74 206f 6620 7061 6464 696e 6720 6f6e  nt of padding on
-00007550: 2074 6865 2078 2d61 7869 732e 0a20 2020   the x-axis..   
-00007560: 2020 2020 202d 2070 6164 7920 2874 7570       - pady (tup
-00007570: 6c65 293a 2054 6865 2061 6d6f 756e 7420  le): The amount 
-00007580: 6f66 2070 6164 6469 6e67 206f 6e20 7468  of padding on th
-00007590: 6520 792d 6178 6973 2e0a 2020 2020 2020  e y-axis..      
-000075a0: 2020 2d20 7374 6963 6b79 2028 7374 7229    - sticky (str)
-000075b0: 3a20 5468 6520 616c 6967 6e6d 656e 7420  : The alignment 
-000075c0: 6f66 2074 6865 2062 7574 746f 6e20 7769  of the button wi
-000075d0: 7468 696e 2069 7473 2063 656c 6c2e 0a20  thin its cell.. 
-000075e0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-000075f0: 2020 2020 2d20 6275 7474 6f6e 5f6e 616d      - button_nam
-00007600: 653a 2074 6865 206e 616d 6564 2062 7574  e: the named but
-00007610: 746f 6e2e 0a20 2020 2050 726f 6365 7373  ton..    Process
-00007620: 696e 6720 4c6f 6769 633a 0a20 2020 2020  ing Logic:.     
-00007630: 2020 202d 2043 7265 6174 6520 6120 6375     - Create a cu
-00007640: 7374 6f6d 2074 6b69 6e74 6572 2062 7574  stom tkinter but
-00007650: 746f 6e20 7769 7468 2074 6865 2067 6976  ton with the giv
-00007660: 656e 2070 6172 616d 6574 6572 732e 0a20  en parameters.. 
-00007670: 2020 2020 2020 202d 2050 6c61 6365 2074         - Place t
-00007680: 6865 2062 7574 746f 6e20 696e 2074 6865  he button in the
-00007690: 2073 7065 6369 6669 6564 2072 6f77 2061   specified row a
-000076a0: 6e64 2063 6f6c 756d 6e2e 0a20 2020 2020  nd column..     
-000076b0: 2020 202d 2041 6464 2070 6164 6469 6e67     - Add padding
-000076c0: 2061 6e64 2061 6c69 676e 6d65 6e74 2074   and alignment t
-000076d0: 6f20 7468 6520 6275 7474 6f6e 2e22 2222  o the button."""
-000076e0: 0a20 2020 2069 6620 6e6f 7420 6667 5f63  .    if not fg_c
-000076f0: 6f6c 6f72 3a0a 2020 2020 2020 2020 6667  olor:.        fg
-00007700: 5f63 6f6c 6f72 203d 2022 2332 3436 4642  _color = "#246FB
-00007710: 3622 0a20 2020 2069 6620 6e6f 7420 7465  6".    if not te
-00007720: 7874 5f63 6f6c 6f72 3a0a 2020 2020 2020  xt_color:.      
-00007730: 2020 7465 7874 5f63 6f6c 6f72 203d 2022    text_color = "
-00007740: 2346 4646 4646 4622 0a20 2020 2069 6620  #FFFFFF".    if 
-00007750: 6e6f 7420 626f 7264 6572 5f63 6f6c 6f72  not border_color
-00007760: 3a0a 2020 2020 2020 2020 626f 7264 6572  :.        border
-00007770: 5f63 6f6c 6f72 203d 2022 4772 6179 220a  _color = "Gray".
-00007780: 2020 2020 6966 206e 6f74 2063 6f6c 756d      if not colum
-00007790: 6e73 7061 6e3a 0a20 2020 2020 2020 2063  nspan:.        c
-000077a0: 6f6c 756d 6e73 7061 6e20 3d20 310a 2020  olumnspan = 1.  
-000077b0: 2020 6275 7474 6f6e 5f6e 616d 6520 3d20    button_name = 
-000077c0: 6374 6b2e 4354 6b42 7574 746f 6e28 0a20  ctk.CTkButton(. 
-000077d0: 2020 2020 2020 2066 7261 6d65 2c0a 2020         frame,.  
-000077e0: 2020 2020 2020 6667 5f63 6f6c 6f72 3d66        fg_color=f
-000077f0: 675f 636f 6c6f 722c 0a20 2020 2020 2020  g_color,.       
-00007800: 2074 6578 745f 636f 6c6f 723d 7465 7874   text_color=text
-00007810: 5f63 6f6c 6f72 2c0a 2020 2020 2020 2020  _color,.        
-00007820: 666f 6e74 3d63 746b 2e43 546b 466f 6e74  font=ctk.CTkFont
-00007830: 2873 697a 653d 6465 6661 756c 745f 666f  (size=default_fo
-00007840: 6e74 5f73 697a 652c 2077 6569 6768 743d  nt_size, weight=
-00007850: 226e 6f72 6d61 6c22 292c 0a20 2020 2020  "normal"),.     
-00007860: 2020 2062 6f72 6465 725f 636f 6c6f 723d     border_color=
-00007870: 626f 7264 6572 5f63 6f6c 6f72 2c0a 2020  border_color,.  
-00007880: 2020 2020 2020 636f 6d6d 616e 643d 636f        command=co
-00007890: 6d6d 616e 642c 0a20 2020 2020 2020 2062  mmand,.        b
-000078a0: 6f72 6465 725f 7769 6474 683d 626f 7264  order_width=bord
-000078b0: 6572 5f77 6964 7468 2c0a 2020 2020 2020  er_width,.      
-000078c0: 2020 7465 7874 3d74 6578 742c 0a20 2020    text=text,.   
-000078d0: 2029 0a20 2020 2062 7574 746f 6e5f 6e61   ).    button_na
-000078e0: 6d65 2e67 7269 6428 726f 773d 726f 772c  me.grid(row=row,
-000078f0: 2063 6f6c 756d 6e3d 636f 6c75 6d6e 2c20   column=column, 
-00007900: 636f 6c75 6d6e 7370 616e 3d63 6f6c 756d  columnspan=colum
-00007910: 6e73 7061 6e2c 2070 6164 783d 7061 6478  nspan, padx=padx
-00007920: 2c20 7061 6479 3d70 6164 792c 2073 7469  , pady=pady, sti
-00007930: 636b 793d 7374 6963 6b79 290a 2020 2020  cky=sticky).    
-00007940: 7265 7475 726e 2062 7574 746f 6e5f 6e61  return button_na
-00007950: 6d65 0a0a 0a23 2023 2323 2323 2323 2323  me...# #########
-00007960: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007970: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007980: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007990: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000079a0: 2323 2323 2323 2323 230a 2320 4372 6561  #########.# Crea
-000079b0: 7465 2061 2062 7574 746f 6e20 6765 6e65  te a button gene
-000079c0: 7261 6c20 726f 7574 696e 650a 2320 2323  ral routine.# ##
-000079d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000079e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000079f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007a00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007a10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007a20: 0a64 6566 2061 6464 5f6f 7074 696f 6e5f  .def add_option_
-00007a30: 6d65 6e75 280a 2020 2020 7365 6c66 2c20  menu(.    self, 
-00007a40: 2023 206e 6f71 613a 2041 4e4e 3030 312c   # noqa: ANN001,
-00007a50: 2041 5247 3030 310a 2020 2020 6672 616d   ARG001.    fram
-00007a60: 653a 2063 746b 2e43 546b 4672 616d 652c  e: ctk.CTkFrame,
-00007a70: 0a20 2020 2063 6f6d 6d61 6e64 3a20 6f62  .    command: ob
-00007a80: 6a65 6374 2c0a 2020 2020 7661 6c75 6573  ject,.    values
-00007a90: 3a20 7374 7220 7c20 6c69 7374 2c0a 2020  : str | list,.  
-00007aa0: 2020 726f 773a 2069 6e74 2c0a 2020 2020    row: int,.    
-00007ab0: 636f 6c75 6d6e 3a20 696e 742c 0a20 2020  column: int,.   
-00007ac0: 2070 6164 783a 2074 7570 6c65 2c0a 2020   padx: tuple,.  
-00007ad0: 2020 7061 6479 3a20 7475 706c 652c 0a20    pady: tuple,. 
-00007ae0: 2020 2073 7469 636b 793a 2073 7472 2c0a     sticky: str,.
-00007af0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
-00007b00: 2222 4164 6473 2061 6e20 6f70 7469 6f6e  ""Adds an option
-00007b10: 206d 656e 7520 746f 2061 2067 6976 656e   menu to a given
-00007b20: 2066 7261 6d65 2077 6974 6820 7370 6563   frame with spec
-00007b30: 6966 6965 6420 7061 7261 6d65 7465 7273  ified parameters
-00007b40: 2e0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00007b50: 3a0a 2020 2020 2020 2020 2d20 6672 616d  :.        - fram
-00007b60: 6520 2863 746b 2e43 546b 4672 616d 6529  e (ctk.CTkFrame)
-00007b70: 3a20 5468 6520 6672 616d 6520 746f 2061  : The frame to a
-00007b80: 6464 2074 6865 206f 7074 696f 6e20 6d65  dd the option me
-00007b90: 6e75 2074 6f2e 0a20 2020 2020 2020 202d  nu to..        -
-00007ba0: 2063 6f6d 6d61 6e64 2028 6f62 6a65 6374   command (object
-00007bb0: 293a 2054 6865 2066 756e 6374 696f 6e20  ): The function 
-00007bc0: 746f 2062 6520 6361 6c6c 6564 2077 6865  to be called whe
-00007bd0: 6e20 616e 206f 7074 696f 6e20 6973 2073  n an option is s
-00007be0: 656c 6563 7465 642e 0a20 2020 2020 2020  elected..       
-00007bf0: 202d 2076 616c 7565 7320 2873 7472 207c   - values (str |
-00007c00: 206c 6973 7429 3a20 5468 6520 6f70 7469   list): The opti
-00007c10: 6f6e 7320 746f 2062 6520 6469 7370 6c61  ons to be displa
-00007c20: 7965 6420 696e 2074 6865 206d 656e 752e  yed in the menu.
-00007c30: 0a20 2020 2020 2020 202d 2072 6f77 2028  .        - row (
-00007c40: 696e 7429 3a20 5468 6520 726f 7720 696e  int): The row in
-00007c50: 2077 6869 6368 2074 6865 206f 7074 696f   which the optio
-00007c60: 6e20 6d65 6e75 2073 686f 756c 6420 6265  n menu should be
-00007c70: 2070 6c61 6365 642e 0a20 2020 2020 2020   placed..       
-00007c80: 202d 2063 6f6c 756d 6e20 2869 6e74 293a   - column (int):
-00007c90: 2054 6865 2063 6f6c 756d 6e20 696e 2077   The column in w
-00007ca0: 6869 6368 2074 6865 206f 7074 696f 6e20  hich the option 
-00007cb0: 6d65 6e75 2073 686f 756c 6420 6265 2070  menu should be p
-00007cc0: 6c61 6365 642e 0a20 2020 2020 2020 202d  laced..        -
-00007cd0: 2070 6164 7820 2874 7570 6c65 293a 2054   padx (tuple): T
-00007ce0: 6865 2061 6d6f 756e 7420 6f66 2070 6164  he amount of pad
-00007cf0: 6469 6e67 2069 6e20 7468 6520 782d 6469  ding in the x-di
-00007d00: 7265 6374 696f 6e2e 0a20 2020 2020 2020  rection..       
-00007d10: 202d 2070 6164 7920 2874 7570 6c65 293a   - pady (tuple):
-00007d20: 2054 6865 2061 6d6f 756e 7420 6f66 2070   The amount of p
-00007d30: 6164 6469 6e67 2069 6e20 7468 6520 792d  adding in the y-
-00007d40: 6469 7265 6374 696f 6e2e 0a20 2020 2020  direction..     
-00007d50: 2020 202d 2073 7469 636b 7920 2873 7472     - sticky (str
-00007d60: 293a 2054 6865 2064 6972 6563 7469 6f6e  ): The direction
-00007d70: 2069 6e20 7768 6963 6820 7468 6520 6f70   in which the op
-00007d80: 7469 6f6e 206d 656e 7520 7368 6f75 6c64  tion menu should
-00007d90: 2073 7469 636b 2074 6f20 7468 6520 6672   stick to the fr
-00007da0: 616d 652e 0a20 2020 2052 6574 7572 6e73  ame..    Returns
-00007db0: 3a0a 2020 2020 2020 2020 2d20 4e6f 6e65  :.        - None
-00007dc0: 3a20 5468 6973 2066 756e 6374 696f 6e20  : This function 
-00007dd0: 646f 6573 206e 6f74 2072 6574 7572 6e20  does not return 
-00007de0: 616e 7920 7661 6c75 652e 0a20 2020 2050  any value..    P
-00007df0: 726f 6365 7373 696e 6720 4c6f 6769 633a  rocessing Logic:
-00007e00: 0a20 2020 2020 2020 202d 2041 6464 7320  .        - Adds 
-00007e10: 616e 206f 7074 696f 6e20 6d65 6e75 2074  an option menu t
-00007e20: 6f20 6120 6672 616d 652e 0a20 2020 2020  o a frame..     
-00007e30: 2020 202d 2053 6574 7320 7468 6520 636f     - Sets the co
-00007e40: 6d6d 616e 6420 746f 2062 6520 6361 6c6c  mmand to be call
-00007e50: 6564 2077 6865 6e20 616e 206f 7074 696f  ed when an optio
-00007e60: 6e20 6973 2073 656c 6563 7465 642e 0a20  n is selected.. 
-00007e70: 2020 2020 2020 202d 2044 6973 706c 6179         - Display
-00007e80: 7320 7468 6520 7370 6563 6966 6965 6420  s the specified 
-00007e90: 6f70 7469 6f6e 7320 696e 2074 6865 206d  options in the m
-00007ea0: 656e 752e 0a20 2020 2020 2020 202d 2050  enu..        - P
-00007eb0: 6c61 6365 7320 7468 6520 6f70 7469 6f6e  laces the option
-00007ec0: 206d 656e 7520 696e 2074 6865 2073 7065   menu in the spe
-00007ed0: 6369 6669 6564 2072 6f77 2061 6e64 2063  cified row and c
-00007ee0: 6f6c 756d 6e2e 0a20 2020 2020 2020 202d  olumn..        -
-00007ef0: 2041 6464 7320 7061 6464 696e 6720 746f   Adds padding to
-00007f00: 2074 6865 206f 7074 696f 6e20 6d65 6e75   the option menu
-00007f10: 2e0a 2020 2020 2020 2020 2d20 5365 7473  ..        - Sets
-00007f20: 2074 6865 2064 6972 6563 7469 6f6e 2069   the direction i
-00007f30: 6e20 7768 6963 6820 7468 6520 6f70 7469  n which the opti
-00007f40: 6f6e 206d 656e 7520 7368 6f75 6c64 2073  on menu should s
-00007f50: 7469 636b 2074 6f20 7468 6520 6672 616d  tick to the fram
-00007f60: 652e 2222 220a 2020 2020 6f70 7469 6f6e  e.""".    option
-00007f70: 5f6d 656e 755f 6e61 6d65 203d 2063 746b  _menu_name = ctk
-00007f80: 2e43 546b 4f70 7469 6f6e 4d65 6e75 280a  .CTkOptionMenu(.
-00007f90: 2020 2020 2020 2020 6672 616d 652c 0a20          frame,. 
-00007fa0: 2020 2020 2020 2076 616c 7565 733d 7661         values=va
-00007fb0: 6c75 6573 2c0a 2020 2020 2020 2020 636f  lues,.        co
-00007fc0: 6d6d 616e 643d 636f 6d6d 616e 642c 0a20  mmand=command,. 
-00007fd0: 2020 2029 0a20 2020 206f 7074 696f 6e5f     ).    option_
-00007fe0: 6d65 6e75 5f6e 616d 652e 6772 6964 2872  menu_name.grid(r
-00007ff0: 6f77 3d72 6f77 2c20 636f 6c75 6d6e 3d63  ow=row, column=c
-00008000: 6f6c 756d 6e2c 2070 6164 783d 7061 6478  olumn, padx=padx
-00008010: 2c20 7061 6479 3d70 6164 792c 2073 7469  , pady=pady, sti
-00008020: 636b 793d 7374 6963 6b79 290a 2020 2020  cky=sticky).    
-00008030: 7265 7475 726e 206f 7074 696f 6e5f 6d65  return option_me
-00008040: 6e75 5f6e 616d 650a 0a0a 2320 2323 2323  nu_name...# ####
-00008050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008060: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008090: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
-000080a0: 2044 6566 696e 6520 616c 6c20 6f66 2074   Define all of t
-000080b0: 6865 206d 656e 7520 656c 656d 656e 7473  he menu elements
-000080c0: 0a23 2023 2323 2323 2323 2323 2323 2323  .# #############
-000080d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000080e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000080f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008100: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008110: 2323 2323 2323 0a64 6566 2069 6e69 7469  ######.def initi
-00008120: 616c 697a 655f 7363 7265 656e 2873 656c  alize_screen(sel
-00008130: 6629 202d 3e20 4e6f 6e65 3a20 2023 206e  f) -> None:  # n
-00008140: 6f71 613a 2041 4e4e 3030 310a 2020 2020  oqa: ANN001.    
-00008150: 2320 4164 6420 6772 6964 2074 6974 6c65  # Add grid title
-00008160: 0a20 2020 2022 2222 496e 6974 6961 6c69  .    """Initiali
-00008170: 7a65 7320 7468 6520 7363 7265 656e 2077  zes the screen w
-00008180: 6974 6820 7661 7269 6f75 7320 6469 7370  ith various disp
-00008190: 6c61 7920 6f70 7469 6f6e 7320 616e 6420  lay options and 
-000081a0: 7365 7474 696e 6773 2e0a 2020 2020 5061  settings..    Pa
-000081b0: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-000081c0: 2020 2d20 7365 6c66 2028 6f62 6a65 6374    - self (object
-000081d0: 293a 2054 6865 206f 626a 6563 7420 746f  ): The object to
-000081e0: 2077 6869 6368 2074 6865 2066 756e 6374   which the funct
-000081f0: 696f 6e20 6265 6c6f 6e67 732e 0a20 2020  ion belongs..   
-00008200: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00008210: 2020 2d20 4e6f 6e65 3a20 5468 6973 2066    - None: This f
-00008220: 756e 6374 696f 6e20 646f 6573 206e 6f74  unction does not
-00008230: 2072 6574 7572 6e20 616e 7920 7661 6c75   return any valu
-00008240: 652e 0a20 2020 2050 726f 6365 7373 696e  e..    Processin
-00008250: 6720 4c6f 6769 633a 0a20 2020 2020 2020  g Logic:.       
-00008260: 202d 2043 7265 6174 6573 2061 2067 7269   - Creates a gri
-00008270: 6420 7469 746c 6520 616e 6420 6164 6473  d title and adds
-00008280: 2069 7420 746f 2074 6865 2073 6964 6562   it to the sideb
-00008290: 6172 2066 7261 6d65 2e0a 2020 2020 2020  ar frame..      
-000082a0: 2020 2d20 4465 6669 6e65 7320 7468 6520    - Defines the 
-000082b0: 6669 7273 7420 6772 6964 202f 2063 6f6c  first grid / col
-000082c0: 756d 6e20 666f 7220 6469 7370 6c61 7920  umn for display 
-000082d0: 6465 7461 696c 206c 6576 656c 2e0a 2020  detail level..  
-000082e0: 2020 2020 2020 2d20 4465 6669 6e65 7320        - Defines 
-000082f0: 7468 6520 7365 636f 6e64 2067 7269 6420  the second grid 
-00008300: 2f20 636f 6c75 6d6e 2066 6f72 2063 6865  / column for che
-00008310: 636b 626f 7865 7320 7265 6c61 7465 6420  ckboxes related 
-00008320: 746f 2064 6973 706c 6179 206f 7074 696f  to display optio
-00008330: 6e73 2e0a 2020 2020 2020 2020 2d20 4465  ns..        - De
-00008340: 6669 6e65 7320 7468 6520 7468 6972 6420  fines the third 
-00008350: 6772 6964 202f 2063 6f6c 756d 6e20 666f  grid / column fo
-00008360: 7220 6275 7474 6f6e 7320 7265 6c61 7465  r buttons relate
-00008370: 6420 746f 2070 726f 6772 616d 2073 6574  d to program set
-00008380: 7469 6e67 732e 0a20 2020 2020 2020 202d  tings..        -
-00008390: 2043 7265 6174 6573 2061 2074 6578 7462   Creates a textb
-000083a0: 6f78 2066 6f72 2064 6973 706c 6179 696e  ox for displayin
-000083b0: 6720 6865 6c70 2069 6e66 6f72 6d61 7469  g help informati
-000083c0: 6f6e 2e0a 2020 2020 2020 2020 2d20 4372  on..        - Cr
-000083d0: 6561 7465 7320 6120 7461 6276 6965 7720  eates a tabview 
-000083e0: 666f 7220 7365 7474 696e 6720 7370 6563  for setting spec
-000083f0: 6966 6963 206e 616d 6573 2c20 636f 6c6f  ific names, colo
-00008400: 7273 2c20 616e 6420 6465 6275 6720 6f70  rs, and debug op
-00008410: 7469 6f6e 732e 0a20 2020 2020 2020 202d  tions..        -
-00008420: 2044 6566 696e 6573 2074 6865 2066 6f75   Defines the fou
-00008430: 7274 6820 6772 6964 202f 2063 6f6c 756d  rth grid / colum
-00008440: 6e20 666f 7220 6368 6563 6b62 6f78 6573  n for checkboxes
-00008450: 2072 656c 6174 6564 2074 6f20 6465 6275   related to debu
-00008460: 6720 6f70 7469 6f6e 732e 0a20 2020 2020  g options..     
-00008470: 2020 202d 2044 6566 696e 6573 2074 6865     - Defines the
-00008480: 2073 6978 7468 2067 7269 6420 2f20 636f   sixth grid / co
-00008490: 6c75 6d6e 2066 6f72 2063 6865 636b 626f  lumn for checkbo
-000084a0: 7865 7320 7265 6c61 7465 6420 746f 2072  xes related to r
-000084b0: 756e 7469 6d65 2073 6574 7469 6e67 732e  untime settings.
-000084c0: 2222 220a 0a20 2020 2023 2044 6973 706c  """..    # Displ
-000084d0: 6179 2074 6865 2066 7261 6d65 2074 6974  ay the frame tit
-000084e0: 6c65 0a20 2020 2073 656c 662e 6c6f 676f  le.    self.logo
-000084f0: 5f6c 6162 656c 203d 2061 6464 5f6c 6162  _label = add_lab
-00008500: 656c 2873 656c 662c 2073 656c 662e 7369  el(self, self.si
-00008510: 6465 6261 725f 6672 616d 652c 2022 4469  debar_frame, "Di
-00008520: 7370 6c61 7920 4f70 7469 6f6e 7322 2c20  splay Options", 
-00008530: 2222 2c20 3230 2c20 2262 6f6c 6422 2c20  "", 20, "bold", 
-00008540: 302c 2030 2c20 3230 2c20 2836 302c 2031  0, 0, 20, (60, 1
-00008550: 3029 2c20 2273 2229 0a0a 2020 2020 2320  0), "s")..    # 
-00008560: 5374 6172 7420 6669 7273 7420 6772 6964  Start first grid
-00008570: 202f 2063 6f6c 756d 6e20 6465 6669 6e69   / column defini
-00008580: 7469 6f6e 730a 0a20 2020 2023 2044 6973  tions..    # Dis
-00008590: 706c 6179 2044 6574 6169 6c20 4c65 7665  play Detail Leve
-000085a0: 6c0a 2020 2020 7365 6c66 2e64 6574 6169  l.    self.detai
-000085b0: 6c5f 6c61 6265 6c20 3d20 6164 645f 6c61  l_label = add_la
-000085c0: 6265 6c28 0a20 2020 2020 2020 2073 656c  bel(.        sel
-000085d0: 662c 0a20 2020 2020 2020 2073 656c 662e  f,.        self.
-000085e0: 7369 6465 6261 725f 6672 616d 652c 0a20  sidebar_frame,. 
+00000190: 2020 2020 2020 2020 230a 2320 5065 726d          #.# Perm
+000001a0: 6973 7369 6f6e 7320 6f66 2074 6869 7320  issions of this 
+000001b0: 7374 726f 6e67 2063 6f70 796c 6566 7420  strong copyleft 
+000001c0: 6c69 6365 6e73 6520 6172 6520 636f 6e64  license are cond
+000001d0: 6974 696f 6e65 6420 6f6e 206d 616b 696e  itioned on makin
+000001e0: 6720 6176 6169 6c61 626c 6520 2020 2020  g available     
+000001f0: 2023 0a23 2063 6f6d 706c 6574 6520 736f   #.# complete so
+00000200: 7572 6365 2063 6f64 6520 6f66 206c 6963  urce code of lic
+00000210: 656e 7365 6420 776f 726b 7320 616e 6420  ensed works and 
+00000220: 6d6f 6469 6669 6361 7469 6f6e 732c 2077  modifications, w
+00000230: 6869 6368 2069 6e63 6c75 6465 206c 6172  hich include lar
+00000240: 6765 7220 776f 726b 7320 230a 2320 7573  ger works #.# us
+00000250: 696e 6720 6120 6c69 6365 6e73 6564 2077  ing a licensed w
+00000260: 6f72 6b2c 2075 6e64 6572 2074 6865 2073  ork, under the s
+00000270: 616d 6520 6c69 6365 6e73 652e 2043 6f70  ame license. Cop
+00000280: 7972 6967 6874 2061 6e64 206c 6963 656e  yright and licen
+00000290: 7365 206e 6f74 6963 6573 206d 7573 7420  se notices must 
+000002a0: 6265 2023 0a23 2070 7265 7365 7276 6564  be #.# preserved
+000002b0: 2e20 436f 6e74 7269 6275 746f 7273 2070  . Contributors p
+000002c0: 726f 7669 6465 2061 6e20 6578 7072 6573  rovide an expres
+000002d0: 7320 6772 616e 7420 6f66 2070 6174 656e  s grant of paten
+000002e0: 7420 7269 6768 7473 2e20 2020 2020 2020  t rights.       
+000002f0: 2020 2020 2020 2020 2020 2020 230a 6672              #.fr
+00000300: 6f6d 205f 5f66 7574 7572 655f 5f20 696d  om __future__ im
+00000310: 706f 7274 2061 6e6e 6f74 6174 696f 6e73  port annotations
+00000320: 0a0a 696d 706f 7274 2063 6f6e 7465 7874  ..import context
+00000330: 6c69 620a 696d 706f 7274 206a 736f 6e0a  lib.import json.
+00000340: 696d 706f 7274 206f 730a 6672 6f6d 2074  import os.from t
+00000350: 6b69 6e74 6572 2069 6d70 6f72 7420 5463  kinter import Tc
+00000360: 6c45 7272 6f72 2c20 666f 6e74 2c20 7474  lError, font, tt
+00000370: 6b0a 6672 6f6d 2074 7970 696e 6720 696d  k.from typing im
+00000380: 706f 7274 2054 5950 455f 4348 4543 4b49  port TYPE_CHECKI
+00000390: 4e47 2c20 4361 6c6c 6162 6c65 0a0a 696d  NG, Callable..im
+000003a0: 706f 7274 2063 7573 746f 6d74 6b69 6e74  port customtkint
+000003b0: 6572 2061 7320 6374 6b0a 6672 6f6d 2050  er as ctk.from P
+000003c0: 494c 2069 6d70 6f72 7420 496d 6167 652c  IL import Image,
+000003d0: 2049 6d61 6765 546b 0a0a 6672 6f6d 206d   ImageTk..from m
+000003e0: 6170 7461 736b 6572 2e73 7263 2e63 6f6c  aptasker.src.col
+000003f0: 726d 6f64 6520 696d 706f 7274 2073 6574  rmode import set
+00000400: 5f63 6f6c 6f72 5f6d 6f64 650a 6672 6f6d  _color_mode.from
+00000410: 206d 6170 7461 736b 6572 2e73 7263 2e6c   maptasker.src.l
+00000420: 696e 656f 7574 2069 6d70 6f72 7420 4c69  ineout import Li
+00000430: 6e65 4f75 740a 6672 6f6d 206d 6170 7461  neOut.from mapta
+00000440: 736b 6572 2e73 7263 2e6d 6170 7574 696c  sker.src.maputil
+00000450: 7320 696d 706f 7274 2028 0a20 2020 2067  s import (.    g
+00000460: 6574 5f70 7970 695f 7665 7273 696f 6e2c  et_pypi_version,
+00000470: 0a20 2020 2068 7474 705f 7265 7175 6573  .    http_reques
+00000480: 742c 0a20 2020 2076 616c 6964 6174 655f  t,.    validate_
+00000490: 6970 5f61 6464 7265 7373 2c0a 2020 2020  ip_address,.    
+000004a0: 7661 6c69 6461 7465 5f70 6f72 742c 0a20  validate_port,. 
+000004b0: 2020 2076 616c 6964 6174 655f 786d 6c5f     validate_xml_
+000004c0: 6669 6c65 2c0a 290a 6672 6f6d 206d 6170  file,.).from map
+000004d0: 7461 736b 6572 2e73 7263 2e6e 616d 6561  tasker.src.namea
+000004e0: 7474 7220 696d 706f 7274 2067 6574 5f74  ttr import get_t
+000004f0: 6b0a 6672 6f6d 206d 6170 7461 736b 6572  k.from maptasker
+00000500: 2e73 7263 2e70 7269 6d69 7465 6d20 696d  .src.primitem im
+00000510: 706f 7274 2050 7269 6d65 4974 656d 730a  port PrimeItems.
+00000520: 6672 6f6d 206d 6170 7461 736b 6572 2e73  from maptasker.s
+00000530: 7263 2e70 726f 6669 6c65 7320 696d 706f  rc.profiles impo
+00000540: 7274 2067 6574 5f70 726f 6669 6c65 5f74  rt get_profile_t
+00000550: 6173 6b73 0a66 726f 6d20 6d61 7074 6173  asks.from maptas
+00000560: 6b65 722e 7372 632e 7072 6f67 696e 6974  ker.src.proginit
+00000570: 2069 6d70 6f72 7420 6765 745f 6461 7461   import get_data
+00000580: 5f61 6e64 5f6f 7574 7075 745f 696e 7472  _and_output_intr
+00000590: 6f0a 6672 6f6d 206d 6170 7461 736b 6572  o.from maptasker
+000005a0: 2e73 7263 2e73 7973 636f 6e73 7420 696d  .src.sysconst im
+000005b0: 706f 7274 2028 0a20 2020 2041 4e41 4c59  port (.    ANALY
+000005c0: 5349 535f 4649 4c45 2c0a 2020 2020 4348  SIS_FILE,.    CH
+000005d0: 414e 4745 4c4f 475f 4649 4c45 2c0a 2020  ANGELOG_FILE,.  
+000005e0: 2020 4348 414e 4745 4c4f 475f 4a53 4f4e    CHANGELOG_JSON
+000005f0: 5f46 494c 452c 0a20 2020 2045 5252 4f52  _FILE,.    ERROR
+00000600: 5f46 494c 452c 0a20 2020 204b 4559 4649  _FILE,.    KEYFI
+00000610: 4c45 2c0a 2020 2020 4c4c 414d 415f 4d4f  LE,.    LLAMA_MO
+00000620: 4445 4c53 2c0a 2020 2020 4e4f 575f 5449  DELS,.    NOW_TI
+00000630: 4d45 2c0a 2020 2020 4f50 454e 4149 5f4d  ME,.    OPENAI_M
+00000640: 4f44 454c 532c 0a20 2020 2056 4552 5349  ODELS,.    VERSI
+00000650: 4f4e 2c0a 290a 0a69 6620 5459 5045 5f43  ON,.)..if TYPE_C
+00000660: 4845 434b 494e 473a 0a20 2020 2066 726f  HECKING:.    fro
+00000670: 6d20 6461 7465 7469 6d65 2069 6d70 6f72  m datetime impor
+00000680: 7420 6461 7465 7469 6d65 0a0a 616c 6c5f  t datetime..all_
+00000690: 6f62 6a65 6374 7320 3d20 2244 6973 706c  objects = "Displ
+000006a0: 6179 2061 6c6c 2050 726f 6a65 6374 732c  ay all Projects,
+000006b0: 2050 726f 6669 6c65 732c 2061 6e64 2054   Profiles, and T
+000006c0: 6173 6b73 2e22 0a0a 2320 544f 444f 2043  asks."..# TODO C
+000006d0: 6861 6e67 6520 7468 6973 2027 6368 616e  hange this 'chan
+000006e0: 6765 6c6f 6727 2077 6974 6820 6561 6368  gelog' with each
+000006f0: 2072 656c 6561 7365 2120 204e 6577 206c   release!  New l
+00000700: 696e 6573 2028 5c6e 2920 6d75 7374 2062  ines (\n) must b
+00000710: 6520 6164 6465 642e 0a43 4841 4e47 454c  e added..CHANGEL
+00000720: 4f47 203d 2022 2222 0a56 6572 7369 6f6e  OG = """.Version
+00000730: 2034 2e30 2e33 2f34 2e30 2e34 2f34 2e30   4.0.3/4.0.4/4.0
+00000740: 2e35 202d 2043 6861 6e67 6520 4c6f 675c  .5 - Change Log\
+00000750: 6e0a 2323 2320 4164 6465 645c 6e0a 2d20  n.### Added\n.- 
+00000760: 4164 6465 643a 2052 6573 746f 7265 2074  Added: Restore t
+00000770: 6865 2047 5549 2077 696e 646f 7720 746f  he GUI window to
+00000780: 2074 6865 206c 6173 742d 7573 6564 2070   the last-used p
+00000790: 6f73 6974 696f 6e20 616e 6420 7369 7a65  osition and size
+000007a0: 2e5c 6e0a 2d20 4164 6465 643a 2054 6865  .\n.- Added: The
+000007b0: 2061 6269 6c69 7479 2074 6f20 6368 616e   ability to chan
+000007c0: 6765 2074 6865 2070 726f 6d70 7420 7573  ge the prompt us
+000007d0: 6564 2066 6f72 2074 6865 2050 726f 6669  ed for the Profi
+000007e0: 6c65 2f54 6173 6b20 616e 616c 7973 6973  le/Task analysis
+000007f0: 2068 6173 2062 6565 6e20 6164 6465 642e   has been added.
+00000800: 5c6e 0a2d 2041 6464 6564 3a20 476f 696e  \n.- Added: Goin
+00000810: 6720 666f 7277 6172 642c 2069 6620 6120  g forward, if a 
+00000820: 6e65 7720 7265 6c65 6173 6520 6973 2061  new release is a
+00000830: 7661 696c 6162 6c65 2c20 7468 6520 4755  vailable, the GU
+00000840: 4920 7769 6c6c 2070 726f 7669 6465 2061  I will provide a
+00000850: 2022 5768 6174 2773 204e 6577 2220 6275   "What's New" bu
+00000860: 7474 6f6e 2e20 2059 6f75 2077 696c 6c20  tton.  You will 
+00000870: 6265 2061 626c 6520 746f 2073 6565 2077  be able to see w
+00000880: 6861 7420 6973 2063 6861 6e67 696e 6720  hat is changing 
+00000890: 6265 666f 7265 2061 7070 6c79 696e 6720  before applying 
+000008a0: 7468 6520 6368 616e 6765 732e 5c6e 0a2d  the changes.\n.-
+000008b0: 2041 6464 6564 3a20 4169 2041 6e61 6c79   Added: Ai Analy
+000008c0: 7369 7320 6e6f 7720 7375 7070 6f72 7473  sis now supports
+000008d0: 2074 6865 206e 6577 204f 7065 6e41 4920   the new OpenAI 
+000008e0: 2767 7074 2d34 6f27 206d 6f64 656c 2e5c  'gpt-4o' model.\
+000008f0: 6e0a 2d20 4164 6465 643a 2053 7570 706f  n.- Added: Suppo
+00000900: 7274 2066 6f72 2054 6173 6b65 7220 362e  rt for Tasker 6.
+00000910: 332e 3820 4265 7461 2063 6f64 652e 5c6e  3.8 Beta code.\n
+00000920: 0a23 2323 2043 6861 6e67 6564 5c6e 0a2d  .### Changed\n.-
+00000930: 2043 6861 6e67 6564 3a20 5769 6465 6e65   Changed: Widene
+00000940: 6420 7468 6520 4755 4920 7769 6e64 6f77  d the GUI window
+00000950: 2073 6c69 6768 746c 7920 666f 7220 6265   slightly for be
+00000960: 7474 6572 2072 6561 6461 6269 6c69 7479  tter readability
+00000970: 2e5c 6e0a 2d20 4368 616e 6765 643a 2027  .\n.- Changed: '
+00000980: 5370 6563 6966 6963 204e 616d 6527 2069  Specific Name' i
+00000990: 7465 6d73 2061 7265 206e 6f77 2061 7661  tems are now ava
+000009a0: 696c 6162 6c65 2076 6961 2061 2070 756c  ilable via a pul
+000009b0: 6c64 6f77 6e20 6d65 6e75 2e20 2049 7420  ldown menu.  It 
+000009c0: 6973 206e 6f20 6c6f 6e67 6572 206e 6563  is no longer nec
+000009d0: 6573 7361 7279 2074 6f20 656e 7465 7220  essary to enter 
+000009e0: 7468 6520 6e61 6d65 7320 7468 726f 7567  the names throug
+000009f0: 6820 6120 7465 7874 2069 6e70 7574 2062  h a text input b
+00000a00: 6f78 2e5c 6e0a 2d20 4368 616e 6765 643a  ox.\n.- Changed:
+00000a10: 2054 6865 2073 6574 7469 6e67 7320 6669   The settings fi
+00000a20: 6c65 206e 6f77 2073 6f72 7473 2074 6865  le now sorts the
+00000a30: 2063 6f6c 6f72 7320 746f 2075 7365 2062   colors to use b
+00000a40: 7920 6e61 6d65 2e5c 6e0a 2323 2320 4669  y name.\n.### Fi
+00000a50: 7865 645c 6e0a 2d20 4669 7865 643a 2054  xed\n.- Fixed: T
+00000a60: 6865 2027 5265 7365 7427 2062 7574 746f  he 'Reset' butto
+00000a70: 6e20 696e 2074 6865 2047 5549 2069 7320  n in the GUI is 
+00000a80: 6e6f 7420 7265 7365 7474 696e 6720 7468  not resetting th
+00000a90: 6520 616e 616c 7973 6973 206d 6f64 656c  e analysis model
+00000aa0: 2e5c 6e0a 2d20 4669 7865 643a 2049 6620  .\n.- Fixed: If 
+00000ab0: 2747 6574 204c 6f63 616c 2058 4d4c 2720  'Get Local XML' 
+00000ac0: 6973 2073 656c 6563 7465 6420 696e 2074  is selected in t
+00000ad0: 6865 2047 5549 2c20 7468 6520 616e 616c  he GUI, the anal
+00000ae0: 797a 6520 5072 6f66 696c 6520 616e 6420  yze Profile and 
+00000af0: 5461 736b 206c 6973 7420 6973 206e 6f74  Task list is not
+00000b00: 2075 7064 6174 6564 2e5c 6e0a 2d20 4669   updated.\n.- Fi
+00000b10: 7865 643a 2054 6865 2027 5370 6563 6966  xed: The 'Specif
+00000b20: 6963 204e 616d 6527 2074 6162 2068 6173  ic Name' tab has
+00000b30: 2074 6865 206c 6162 656c 2066 6f72 2074   the label for t
+00000b40: 6865 2027 436f 6c6f 7273 2720 7461 6220  he 'Colors' tab 
+00000b50: 696e 2074 6865 2047 5549 2e5c 6e0a 2d20  in the GUI.\n.- 
+00000b60: 4669 7865 643a 2055 6e64 6572 2063 6572  Fixed: Under cer
+00000b70: 7461 696e 2073 6974 7561 7469 6f6e 732c  tain situations,
+00000b80: 2074 6865 2047 5549 2077 696c 6c20 7573   the GUI will us
+00000b90: 6520 7468 6520 6f6c 6420 6461 7461 2065  e the old data e
+00000ba0: 7665 6e20 6166 7465 7220 6765 7474 696e  ven after gettin
+00000bb0: 6720 6120 6e65 7720 584d 4c20 6669 6c65  g a new XML file
+00000bc0: 2e5c 6e0a 2d20 4669 7865 643a 204f 6363  .\n.- Fixed: Occ
+00000bd0: 6173 696f 6e20 7072 6f67 7261 6d20 6162  asion program ab
+00000be0: 6e6f 726d 616c 2074 6572 6d69 6e61 7469  normal terminati
+00000bf0: 6f6e 2077 6865 6e20 7365 6c65 6374 696e  on when selectin
+00000c00: 6720 6120 7370 6563 6966 6963 2050 726f  g a specific Pro
+00000c10: 6a65 6374 206f 7220 5072 6f66 696c 6520  ject or Profile 
+00000c20: 7468 6174 2068 6173 2061 2053 6365 6e65  that has a Scene
+00000c30: 2e5c 6e0a 7468 6174 2068 6173 2061 2053  .\n.that has a S
+00000c40: 6365 6e65 2e0a 2d20 4669 7865 643a 2054  cene..- Fixed: T
+00000c50: 6865 2070 726f 6772 616d 206f 6363 6173  he program occas
+00000c60: 696f 6e61 6c6c 7920 7465 726d 696e 6174  ionally terminat
+00000c70: 6573 2061 626e 6f72 6d61 6c6c 7920 7768  es abnormally wh
+00000c80: 656e 2074 7279 696e 6720 746f 2073 6176  en trying to sav
+00000c90: 6520 7468 6520 7365 7474 696e 6773 2066  e the settings f
+00000ca0: 696c 652e 5c6e 0a22 2222 0a43 4841 4e47  ile.\n.""".CHANG
+00000cb0: 454c 4f47 5f4a 534f 4e20 3d20 7b0a 2020  ELOG_JSON = {.  
+00000cc0: 2020 2276 6572 7369 6f6e 223a 2022 342e    "version": "4.
+00000cd0: 302e 3322 2c0a 2020 2020 2263 6861 6e67  0.3",.    "chang
+00000ce0: 6573 223a 205b 0a20 2020 2020 2020 207b  es": [.        {
+00000cf0: 0a20 2020 2020 2020 2020 2020 2022 6368  .            "ch
+00000d00: 616e 6765 223a 2022 4669 7865 6420 616e  ange": "Fixed an
+00000d10: 2069 7373 7565 2077 6865 7265 2061 6e61   issue where ana
+00000d20: 6c79 7369 7320 7265 7375 6c74 7320 7765  lysis results we
+00000d30: 7265 206e 6f74 2062 6569 6e67 2070 726f  re not being pro
+00000d40: 7065 726c 7920 636c 6561 7265 6420 6265  perly cleared be
+00000d50: 7477 6565 6e20 616e 616c 7973 6573 2e22  tween analyses."
+00000d60: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+00000d70: 7970 6522 3a20 2266 6978 6564 222c 0a20  ype": "fixed",. 
+00000d80: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00000d90: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00000da0: 2263 6861 6e67 6522 3a20 2249 6d70 726f  "change": "Impro
+00000db0: 7665 6420 6572 726f 7220 6861 6e64 6c69  ved error handli
+00000dc0: 6e67 2066 6f72 2061 6e61 6c79 7369 7320  ng for analysis 
+00000dd0: 6661 696c 7572 6573 2e22 2c0a 2020 2020  failures.",.    
+00000de0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00000df0: 2263 6861 6e67 6564 222c 0a20 2020 2020  "changed",.     
+00000e00: 2020 207d 2c0a 2020 2020 5d2c 0a7d 0a64     },.    ],.}.d
+00000e10: 6566 6175 6c74 5f66 6f6e 745f 7369 7a65  efault_font_size
+00000e20: 203d 2031 340a 0a23 2053 6574 2075 7020   = 14..# Set up 
+00000e30: 666f 7220 6163 6365 7373 2074 6f20 6963  for access to ic
+00000e40: 6f6e 730a 4355 5252 454e 545f 5041 5448  ons.CURRENT_PATH
+00000e50: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
+00000e60: 6d65 286f 732e 7061 7468 2e72 6561 6c70  me(os.path.realp
+00000e70: 6174 6828 5f5f 6669 6c65 5f5f 2929 0a49  ath(__file__)).I
+00000e80: 434f 4e5f 4449 5220 3d20 6f73 2e70 6174  CON_DIR = os.pat
+00000e90: 682e 6a6f 696e 2843 5552 5245 4e54 5f50  h.join(CURRENT_P
+00000ea0: 4154 482c 2022 2e2e 2f61 7373 6574 7322  ATH, "../assets"
+00000eb0: 2c20 2269 636f 6e73 2229 0a49 434f 4e5f  , "icons").ICON_
+00000ec0: 5041 5448 203d 207b 0a20 2020 2022 636c  PATH = {.    "cl
+00000ed0: 6f73 6522 3a20 286f 732e 7061 7468 2e6a  ose": (os.path.j
+00000ee0: 6f69 6e28 4943 4f4e 5f44 4952 2c20 2263  oin(ICON_DIR, "c
+00000ef0: 6c6f 7365 5f62 6c61 636b 2e70 6e67 2229  lose_black.png")
+00000f00: 2c20 6f73 2e70 6174 682e 6a6f 696e 2849  , os.path.join(I
+00000f10: 434f 4e5f 4449 522c 2022 636c 6f73 655f  CON_DIR, "close_
+00000f20: 7768 6974 652e 706e 6722 2929 2c0a 2020  white.png")),.  
+00000f30: 2020 2320 2269 6d61 6765 7322 3a20 6c69    # "images": li
+00000f40: 7374 286f 732e 7061 7468 2e6a 6f69 6e28  st(os.path.join(
+00000f50: 4943 4f4e 5f44 4952 2c20 6622 696d 6167  ICON_DIR, f"imag
+00000f60: 657b 697d 2e6a 7067 2229 2066 6f72 2069  e{i}.jpg") for i
+00000f70: 2069 6e20 7261 6e67 6528 312c 2034 2929   in range(1, 4))
+00000f80: 2c0a 2020 2020 2265 7965 3122 3a20 286f  ,.    "eye1": (o
+00000f90: 732e 7061 7468 2e6a 6f69 6e28 4943 4f4e  s.path.join(ICON
+00000fa0: 5f44 4952 2c20 2265 7965 315f 626c 6163  _DIR, "eye1_blac
+00000fb0: 6b2e 706e 6722 292c 206f 732e 7061 7468  k.png"), os.path
+00000fc0: 2e6a 6f69 6e28 4943 4f4e 5f44 4952 2c20  .join(ICON_DIR, 
+00000fd0: 2265 7965 315f 7768 6974 652e 706e 6722  "eye1_white.png"
+00000fe0: 2929 2c0a 2020 2020 2265 7965 3222 3a20  )),.    "eye2": 
+00000ff0: 286f 732e 7061 7468 2e6a 6f69 6e28 4943  (os.path.join(IC
+00001000: 4f4e 5f44 4952 2c20 2265 7965 325f 626c  ON_DIR, "eye2_bl
+00001010: 6163 6b2e 706e 6722 292c 206f 732e 7061  ack.png"), os.pa
+00001020: 7468 2e6a 6f69 6e28 4943 4f4e 5f44 4952  th.join(ICON_DIR
+00001030: 2c20 2265 7965 325f 7768 6974 652e 706e  , "eye2_white.pn
+00001040: 6722 2929 2c0a 2020 2020 2269 6e66 6f22  g")),.    "info"
+00001050: 3a20 6f73 2e70 6174 682e 6a6f 696e 2849  : os.path.join(I
+00001060: 434f 4e5f 4449 522c 2022 696e 666f 2e70  CON_DIR, "info.p
+00001070: 6e67 2229 2c0a 2020 2020 2277 6172 6e69  ng"),.    "warni
+00001080: 6e67 223a 206f 732e 7061 7468 2e6a 6f69  ng": os.path.joi
+00001090: 6e28 4943 4f4e 5f44 4952 2c20 2277 6172  n(ICON_DIR, "war
+000010a0: 6e69 6e67 2e70 6e67 2229 2c0a 2020 2020  ning.png"),.    
+000010b0: 2265 7272 6f72 223a 206f 732e 7061 7468  "error": os.path
+000010c0: 2e6a 6f69 6e28 4943 4f4e 5f44 4952 2c20  .join(ICON_DIR, 
+000010d0: 2265 7272 6f72 2e70 6e67 2229 2c0a 2020  "error.png"),.  
+000010e0: 2020 226c 6566 7422 3a20 6f73 2e70 6174    "left": os.pat
+000010f0: 682e 6a6f 696e 2849 434f 4e5f 4449 522c  h.join(ICON_DIR,
+00001100: 2022 6c65 6674 2e70 6e67 2229 2c0a 2020   "left.png"),.  
+00001110: 2020 2272 6967 6874 223a 206f 732e 7061    "right": os.pa
+00001120: 7468 2e6a 6f69 6e28 4943 4f4e 5f44 4952  th.join(ICON_DIR
+00001130: 2c20 2272 6967 6874 2e70 6e67 2229 2c0a  , "right.png"),.
+00001140: 2020 2020 2277 6172 6e69 6e67 3222 3a20      "warning2": 
+00001150: 6f73 2e70 6174 682e 6a6f 696e 2849 434f  os.path.join(ICO
+00001160: 4e5f 4449 522c 2022 7761 726e 696e 6732  N_DIR, "warning2
+00001170: 2e70 6e67 2229 2c0a 2020 2020 226c 6f61  .png"),.    "loa
+00001180: 6465 7222 3a20 6f73 2e70 6174 682e 6a6f  der": os.path.jo
+00001190: 696e 2849 434f 4e5f 4449 522c 2022 6c6f  in(ICON_DIR, "lo
+000011a0: 6164 6572 2e67 6966 2229 2c0a 2020 2020  ader.gif"),.    
+000011b0: 2269 636f 6e22 3a20 6f73 2e70 6174 682e  "icon": os.path.
+000011c0: 6a6f 696e 2849 434f 4e5f 4449 522c 2022  join(ICON_DIR, "
+000011d0: 6963 6f6e 2e70 6e67 2229 2c0a 2020 2020  icon.png"),.    
+000011e0: 2261 7272 6f77 223a 206f 732e 7061 7468  "arrow": os.path
+000011f0: 2e6a 6f69 6e28 4943 4f4e 5f44 4952 2c20  .join(ICON_DIR, 
+00001200: 2261 7272 6f77 2e70 6e67 2229 2c0a 2020  "arrow.png"),.  
+00001210: 2020 2269 6d61 6765 223a 206f 732e 7061    "image": os.pa
+00001220: 7468 2e6a 6f69 6e28 4943 4f4e 5f44 4952  th.join(ICON_DIR
+00001230: 2c20 2269 6d61 6765 2e70 6e67 2229 2c0a  , "image.png"),.
+00001240: 7d0a 0a0a 2320 4d61 6b65 2073 7572 6520  }...# Make sure 
+00001250: 7468 6520 7369 6e67 6c65 206e 616d 6564  the single named
+00001260: 2069 7465 6d20 6578 6973 7473 2e2e 2e74   item exists...t
+00001270: 6861 7420 6974 2069 7320 6120 7661 6c69  hat it is a vali
+00001280: 6420 6e61 6d65 0a64 6566 2076 616c 6964  d name.def valid
+00001290: 5f69 7465 6d28 7365 6c66 2c20 7468 655f  _item(self, the_
+000012a0: 6e61 6d65 3a20 7374 722c 2065 6c65 6d65  name: str, eleme
+000012b0: 6e74 5f6e 616d 653a 2073 7472 2c20 6465  nt_name: str, de
+000012c0: 6275 673a 2062 6f6f 6c2c 2061 7070 6561  bug: bool, appea
+000012d0: 7261 6e63 655f 6d6f 6465 3a20 7374 7229  rance_mode: str)
+000012e0: 202d 3e20 626f 6f6c 3a20 2023 206e 6f71   -> bool:  # noq
+000012f0: 613a 2041 4e4e 3030 310a 2020 2020 2222  a: ANN001.    ""
+00001300: 220a 2020 2020 4368 6563 6b73 2069 6620  ".    Checks if 
+00001310: 616e 2069 7465 6d20 6e61 6d65 2069 7320  an item name is 
+00001320: 7661 6c69 640a 2020 2020 4172 6773 3a0a  valid.    Args:.
+00001330: 2020 2020 2020 2020 7468 655f 6e61 6d65          the_name
+00001340: 3a20 5374 7269 6e67 202d 204e 616d 6520  : String - Name 
+00001350: 746f 2063 6865 636b 0a20 2020 2020 2020  to check.       
+00001360: 2065 6c65 6d65 6e74 5f6e 616d 653a 2053   element_name: S
+00001370: 7472 696e 6720 2d20 456c 656d 656e 7420  tring - Element 
+00001380: 7479 7065 2062 6569 6e67 2063 6865 636b  type being check
+00001390: 6564 0a20 2020 2020 2020 2064 6562 7567  ed.        debug
+000013a0: 3a20 626f 6f6c 6561 6e20 2d20 4755 4920  : boolean - GUI 
+000013b0: 6465 6275 6720 6d6f 6465 2054 7275 6520  debug mode True 
+000013c0: 6f72 2046 616c 7365 0a20 2020 2020 2020  or False.       
+000013d0: 2061 7070 6561 7261 6e63 655f 6d6f 6465   appearance_mode
+000013e0: 3a20 5374 7269 6e67 202d 204c 6967 6874  : String - Light
+000013f0: 2f44 6172 6b2f 5379 7374 656d 0a20 2020  /Dark/System.   
+00001400: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00001410: 2020 426f 6f6c 6561 6e20 2d20 5768 6574    Boolean - Whet
+00001420: 6865 7220 7468 6520 6e61 6d65 2069 7320  her the name is 
+00001430: 7661 6c69 640a 2020 2020 5072 6f63 6573  valid.    Proces
+00001440: 7369 6e67 204c 6f67 6963 3a0a 2020 2020  sing Logic:.    
+00001450: 2d20 496e 6974 6961 6c69 7a65 2074 656d  - Initialize tem
+00001460: 706f 7261 7279 2070 7269 6d61 7279 2069  porary primary i
+00001470: 7465 6d73 206f 626a 6563 740a 2020 2020  tems object.    
+00001480: 2d20 4765 7420 6261 636b 7570 2078 6d6c  - Get backup xml
+00001490: 2064 6174 6120 616e 6420 726f 6f74 2065   data and root e
+000014a0: 6c65 6d65 6e74 730a 2020 2020 2d20 4d61  lements.    - Ma
+000014b0: 7463 6820 656c 656d 656e 7420 7479 7065  tch element type
+000014c0: 2061 6e64 2067 6574 2063 6f72 7265 7370   and get corresp
+000014d0: 6f6e 6469 6e67 2072 6f6f 7420 656c 656d  onding root elem
+000014e0: 656e 740a 2020 2020 2d20 4368 6563 6b20  ent.    - Check 
+000014f0: 6966 2069 7465 6d20 6e61 6d65 2065 7869  if item name exi
+00001500: 7374 7320 6279 2067 6f69 6e67 2074 6872  sts by going thr
+00001510: 6f75 6768 2061 6c6c 206e 616d 6573 2069  ough all names i
+00001520: 6e20 726f 6f74 2065 6c65 6d65 6e74 0a20  n root element. 
+00001530: 2020 2022 2222 0a20 2020 2023 2053 6574     """.    # Set
+00001540: 206f 7572 2066 696c 6520 746f 2067 6574   our file to get
+00001550: 2074 6865 2066 696c 6520 6672 6f6d 2074   the file from t
+00001560: 6865 206c 6f63 616c 2064 7269 7665 2073  he local drive s
+00001570: 696e 6365 2069 7420 6861 6420 7072 6576  ince it had prev
+00001580: 696f 7573 6c79 2062 6565 6e20 7075 6c6c  iously been pull
+00001590: 6564 2066 726f 6d20 7468 6520 416e 6472  ed from the Andr
+000015a0: 6f69 6420 6465 7669 6365 2e0a 2020 2020  oid device..    
+000015b0: 2320 5365 7474 696e 6720 5072 696d 6549  # Setting PrimeI
+000015c0: 7465 6d73 2e70 726f 6772 616d 5f61 7267  tems.program_arg
+000015d0: 756d 656e 7473 5b22 6669 6c65 225d 2077  uments["file"] w
+000015e0: 696c 6c20 6265 2075 7365 6420 696e 2067  ill be used in g
+000015f0: 6574 5f78 6d6c 2829 2061 6e64 2077 6f6e  et_xml() and won
+00001600: 2774 2070 726f 6d70 7420 666f 7220 6669  't prompt for fi
+00001610: 6c65 2069 6620 6974 2065 7869 7374 732e  le if it exists.
+00001620: 0a20 2020 2066 696c 656e 616d 655f 6c6f  .    filename_lo
+00001630: 6361 7469 6f6e 203d 2073 656c 662e 616e  cation = self.an
+00001640: 6472 6f69 645f 6669 6c65 2e72 6669 6e64  droid_file.rfind
+00001650: 2850 7269 6d65 4974 656d 732e 736c 6173  (PrimeItems.slas
+00001660: 6829 202b 2031 0a20 2020 2069 6620 6669  h) + 1.    if fi
+00001670: 6c65 6e61 6d65 5f6c 6f63 6174 696f 6e20  lename_location 
+00001680: 213d 2030 3a0a 2020 2020 2020 2020 5072  != 0:.        Pr
+00001690: 696d 6549 7465 6d73 2e70 726f 6772 616d  imeItems.program
+000016a0: 5f61 7267 756d 656e 7473 5b22 6669 6c65  _arguments["file
+000016b0: 225d 203d 2073 656c 662e 616e 6472 6f69  "] = self.androi
+000016c0: 645f 6669 6c65 5b66 696c 656e 616d 655f  d_file[filename_
+000016d0: 6c6f 6361 7469 6f6e 3a5d 0a20 2020 2065  location:].    e
+000016e0: 6c69 6620 7365 6c66 2e66 696c 653a 0a20  lif self.file:. 
+000016f0: 2020 2020 2020 2050 7269 6d65 4974 656d         PrimeItem
+00001700: 732e 7072 6f67 7261 6d5f 6172 6775 6d65  s.program_argume
+00001710: 6e74 735b 2266 696c 6522 5d20 3d20 7365  nts["file"] = se
+00001720: 6c66 2e66 696c 650a 2020 2020 656c 7365  lf.file.    else
+00001730: 3a0a 2020 2020 2020 2020 5f20 3d20 7365  :.        _ = se
+00001740: 6c66 2e70 726f 6d70 745f 616e 645f 6765  lf.prompt_and_ge
+00001750: 745f 6669 6c65 2873 656c 662e 6465 6275  t_file(self.debu
+00001760: 672c 2073 656c 662e 6170 7065 6172 616e  g, self.appearan
+00001770: 6365 5f6d 6f64 6529 0a0a 2020 2020 2320  ce_mode)..    # 
+00001780: 4765 7420 7468 6520 584d 4c20 6461 7461  Get the XML data
+00001790: 0a20 2020 2072 6574 7572 6e5f 636f 6465  .    return_code
+000017a0: 203d 2067 6574 5f78 6d6c 2864 6562 7567   = get_xml(debug
+000017b0: 2c20 6170 7065 6172 616e 6365 5f6d 6f64  , appearance_mod
+000017c0: 6529 0a0a 2020 2020 2320 4469 6420 7765  e)..    # Did we
+000017d0: 2067 6574 2061 6e20 6572 726f 7220 7265   get an error re
+000017e0: 6164 696e 6720 7468 6520 6261 636b 7570  ading the backup
+000017f0: 2066 696c 653f 0a20 2020 2069 6620 7265   file?.    if re
+00001800: 7475 726e 5f63 6f64 6520 3e20 303a 0a20  turn_code > 0:. 
+00001810: 2020 2020 2020 2069 6620 7265 7475 726e         if return
+00001820: 5f63 6f64 6520 3d3d 2036 3a0a 2020 2020  _code == 6:.    
+00001830: 2020 2020 2020 2020 5072 696d 6549 7465          PrimeIte
+00001840: 6d73 2e65 7272 6f72 5f6d 7367 203d 2022  ms.error_msg = "
+00001850: 4361 6e63 656c 2062 7574 746f 6e20 7072  Cancel button pr
+00001860: 6573 7365 642e 220a 2020 2020 2020 2020  essed.".        
+00001870: 5072 696d 6549 7465 6d73 2e65 7272 6f72  PrimeItems.error
+00001880: 5f63 6f64 6520 3d20 300a 2020 2020 2020  _code = 0.      
+00001890: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+000018a0: 2020 2020 2320 5365 7420 7570 2066 6f72      # Set up for
+000018b0: 206e 616d 6520 6368 6563 6b69 6e67 0a20   name checking. 
+000018c0: 2020 2023 2046 696e 6420 7468 6520 7370     # Find the sp
+000018d0: 6563 6966 6963 2069 7465 6d20 616e 6420  ecific item and 
+000018e0: 6765 7420 6974 2773 2072 6f6f 7420 656c  get it's root el
+000018f0: 656d 656e 740a 2020 2020 726f 6f74 5f65  ement.    root_e
+00001900: 6c65 6d65 6e74 5f63 686f 6963 6573 203d  lement_choices =
+00001910: 207b 0a20 2020 2020 2020 2022 5072 6f6a   {.        "Proj
+00001920: 6563 7422 3a20 5072 696d 6549 7465 6d73  ect": PrimeItems
+00001930: 2e74 6173 6b65 725f 726f 6f74 5f65 6c65  .tasker_root_ele
+00001940: 6d65 6e74 735b 2261 6c6c 5f70 726f 6a65  ments["all_proje
+00001950: 6374 7322 5d2c 0a20 2020 2020 2020 2022  cts"],.        "
+00001960: 5072 6f66 696c 6522 3a20 5072 696d 6549  Profile": PrimeI
+00001970: 7465 6d73 2e74 6173 6b65 725f 726f 6f74  tems.tasker_root
+00001980: 5f65 6c65 6d65 6e74 735b 2261 6c6c 5f70  _elements["all_p
+00001990: 726f 6669 6c65 7322 5d2c 0a20 2020 2020  rofiles"],.     
+000019a0: 2020 2022 5461 736b 223a 2050 7269 6d65     "Task": Prime
+000019b0: 4974 656d 732e 7461 736b 6572 5f72 6f6f  Items.tasker_roo
+000019c0: 745f 656c 656d 656e 7473 5b22 616c 6c5f  t_elements["all_
+000019d0: 7461 736b 7322 5d2c 0a20 2020 207d 0a20  tasks"],.    }. 
+000019e0: 2020 2072 6f6f 745f 656c 656d 656e 7420     root_element 
+000019f0: 3d20 726f 6f74 5f65 6c65 6d65 6e74 5f63  = root_element_c
+00001a00: 686f 6963 6573 5b65 6c65 6d65 6e74 5f6e  hoices[element_n
+00001a10: 616d 655d 0a0a 2020 2020 2320 5365 6520  ame]..    # See 
+00001a20: 6966 2074 6865 2069 7465 6d20 6578 6973  if the item exis
+00001a30: 7473 2062 7920 676f 696e 6720 7468 726f  ts by going thro
+00001a40: 7567 6820 616c 6c20 6e61 6d65 730a 2020  ugh all names.  
+00001a50: 2020 7265 7475 726e 2061 6e79 2872 6f6f    return any(roo
+00001a60: 745f 656c 656d 656e 745b 6974 656d 5d5b  t_element[item][
+00001a70: 226e 616d 6522 5d20 3d3d 2074 6865 5f6e  "name"] == the_n
+00001a80: 616d 6520 666f 7220 6974 656d 2069 6e20  ame for item in 
+00001a90: 726f 6f74 5f65 6c65 6d65 6e74 290a 0a0a  root_element)...
+00001aa0: 2320 4765 7420 7468 6520 584d 4c20 6461  # Get the XML da
+00001ab0: 7461 2061 6e64 2073 6574 7570 2050 7269  ta and setup Pri
+00001ac0: 6d65 6974 656d 730a 6465 6620 6765 745f  meitems.def get_
+00001ad0: 786d 6c28 6465 6275 673a 2062 6f6f 6c2c  xml(debug: bool,
+00001ae0: 2061 7070 6561 7261 6e63 655f 6d6f 6465   appearance_mode
+00001af0: 3a20 7374 7229 202d 3e20 696e 743a 0a20  : str) -> int:. 
+00001b00: 2020 2022 2222 2022 5265 7475 726e 7320     """ "Returns 
+00001b10: 7468 6520 7461 736b 6572 2072 6f6f 7420  the tasker root 
+00001b20: 786d 6c20 6974 656d 7320 6672 6f6d 2074  xml items from t
+00001b30: 6865 2062 6163 6b75 7020 786d 6c20 6669  he backup xml fi
+00001b40: 6c65 2062 6173 6564 206f 6e20 7468 6520  le based on the 
+00001b50: 6769 7665 6e20 6465 6275 6720 616e 6420  given debug and 
+00001b60: 6170 7065 6172 616e 6365 206d 6f64 6520  appearance mode 
+00001b70: 7061 7261 6d65 7465 7273 2e22 0a20 2020  parameters.".   
+00001b80: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
+00001b90: 2020 2020 2064 6562 7567 2028 626f 6f6c       debug (bool
+00001ba0: 293a 2049 6e64 6963 6174 6573 2077 6865  ): Indicates whe
+00001bb0: 7468 6572 2074 6865 2070 726f 6772 616d  ther the program
+00001bc0: 2069 7320 696e 2064 6562 7567 206d 6f64   is in debug mod
+00001bd0: 6520 6f72 206e 6f74 2e0a 2020 2020 2020  e or not..      
+00001be0: 2020 6170 7065 6172 616e 6365 5f6d 6f64    appearance_mod
+00001bf0: 6520 2873 7472 293a 2053 7065 6369 6669  e (str): Specifi
+00001c00: 6573 2074 6865 2063 6f6c 6f72 206d 6f64  es the color mod
+00001c10: 6520 746f 2062 6520 7573 6564 2e0a 2020  e to be used..  
+00001c20: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00001c30: 2020 2069 6e74 3a20 5468 6520 7265 7475     int: The retu
+00001c40: 726e 2063 6f64 6520 6672 6f6d 2067 6574  rn code from get
+00001c50: 7469 6e67 2074 6865 2078 6d6c 2066 696c  ting the xml fil
+00001c60: 652e 0a20 2020 2050 726f 6365 7373 696e  e..    Processin
+00001c70: 6720 4c6f 6769 633a 0a20 2020 2020 2020  g Logic:.       
+00001c80: 202d 2049 6e69 7469 616c 697a 6520 7465   - Initialize te
+00001c90: 6d70 6f72 6172 7920 5072 696d 6172 7949  mporary PrimaryI
+00001ca0: 7465 6d73 206f 626a 6563 742e 0a20 2020  tems object..   
+00001cb0: 2020 2020 202d 2053 6574 2066 696c 655f       - Set file_
+00001cc0: 746f 5f67 6574 2076 6172 6961 626c 6520  to_get variable 
+00001cd0: 6261 7365 6420 6f6e 2064 6562 7567 206d  based on debug m
+00001ce0: 6f64 652e 0a20 2020 2020 2020 202d 2053  ode..        - S
+00001cf0: 6574 2070 726f 6772 616d 5f61 7267 756d  et program_argum
+00001d00: 656e 7473 2076 6172 6961 626c 6520 666f  ents variable fo
+00001d10: 7220 6465 6275 6720 6d6f 6465 2e0a 2020  r debug mode..  
+00001d20: 2020 2020 2020 2d20 5365 7420 636f 6c6f        - Set colo
+00001d30: 7273 5f74 6f5f 7573 6520 7661 7269 6162  rs_to_use variab
+00001d40: 6c65 2062 6173 6564 206f 6e20 6170 7065  le based on appe
+00001d50: 6172 616e 6365 206d 6f64 652e 0a20 2020  arance mode..   
+00001d60: 2020 2020 202d 2049 6e69 7469 616c 697a       - Initializ
+00001d70: 6520 6f75 7470 7574 5f6c 696e 6573 2076  e output_lines v
+00001d80: 6172 6961 626c 652e 0a20 2020 2020 2020  ariable..       
+00001d90: 202d 2052 6574 7572 6e20 6461 7461 2061   - Return data a
+00001da0: 6e64 206f 7574 7075 7420 696e 7472 6f2e  nd output intro.
+00001db0: 2222 220a 2020 2020 6966 206e 6f74 2050  """.    if not P
+00001dc0: 7269 6d65 4974 656d 732e 6669 6c65 5f74  rimeItems.file_t
+00001dd0: 6f5f 6765 743a 0a20 2020 2020 2020 2050  o_get:.        P
+00001de0: 7269 6d65 4974 656d 732e 6669 6c65 5f74  rimeItems.file_t
+00001df0: 6f5f 6765 7420 3d20 2262 6163 6b75 702e  o_get = "backup.
+00001e00: 786d 6c22 2069 6620 6465 6275 6720 656c  xml" if debug el
+00001e10: 7365 2022 220a 2020 2020 5072 696d 6549  se "".    PrimeI
+00001e20: 7465 6d73 2e70 726f 6772 616d 5f61 7267  tems.program_arg
+00001e30: 756d 656e 7473 5b22 6465 6275 6722 5d20  uments["debug"] 
+00001e40: 3d20 6465 6275 670a 2020 2020 5072 696d  = debug.    Prim
+00001e50: 6549 7465 6d73 2e70 726f 6772 616d 5f61  eItems.program_a
+00001e60: 7267 756d 656e 7473 5b22 6775 6922 5d20  rguments["gui"] 
+00001e70: 3d20 5472 7565 0a20 2020 2050 7269 6d65  = True.    Prime
+00001e80: 4974 656d 732e 636f 6c6f 7273 5f74 6f5f  Items.colors_to_
+00001e90: 7573 6520 3d20 7365 745f 636f 6c6f 725f  use = set_color_
+00001ea0: 6d6f 6465 2861 7070 6561 7261 6e63 655f  mode(appearance_
+00001eb0: 6d6f 6465 290a 2020 2020 5072 696d 6549  mode).    PrimeI
+00001ec0: 7465 6d73 2e6f 7574 7075 745f 6c69 6e65  tems.output_line
+00001ed0: 7320 3d20 4c69 6e65 4f75 7428 290a 0a20  s = LineOut().. 
+00001ee0: 2020 2072 6574 7572 6e20 6765 745f 6461     return get_da
+00001ef0: 7461 5f61 6e64 5f6f 7574 7075 745f 696e  ta_and_output_in
+00001f00: 7472 6f28 4661 6c73 6529 0a0a 0a23 2047  tro(False)...# G
+00001f10: 6574 2061 6c6c 206d 6f6e 6f73 7061 6365  et all monospace
+00001f20: 2066 6f6e 7473 2066 726f 6d20 544b 496e   fonts from TKIn
+00001f30: 7465 720a 6465 6620 6765 745f 6d6f 6e6f  ter.def get_mono
+00001f40: 5f66 6f6e 7473 2829 202d 3e20 4e6f 6e65  _fonts() -> None
+00001f50: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+00001f60: 7475 726e 7320 6120 6469 6374 696f 6e61  turns a dictiona
+00001f70: 7279 206f 6620 6669 7865 642d 7769 6474  ry of fixed-widt
+00001f80: 6820 666f 6e74 730a 2020 2020 4172 6773  h fonts.    Args
+00001f90: 3a0a 2020 2020 2020 2020 7365 6c66 3a20  :.        self: 
+00001fa0: 5468 6520 636c 6173 7320 696e 7374 616e  The class instan
+00001fb0: 6365 0a20 2020 2052 6574 7572 6e73 3a0a  ce.    Returns:.
+00001fc0: 2020 2020 2020 2020 6469 6374 3a20 4120          dict: A 
+00001fd0: 6469 6374 696f 6e61 7279 206f 6620 6669  dictionary of fi
+00001fe0: 7865 642d 7769 6474 6820 666f 6e74 7320  xed-width fonts 
+00001ff0: 616e 6420 7468 6569 7220 6661 6d69 6c79  and their family
+00002000: 206e 616d 6573 0a20 2020 202d 2047 6574   names.    - Get
+00002010: 2061 6c6c 2061 7661 696c 6162 6c65 2066   all available f
+00002020: 6f6e 7473 2066 726f 6d20 7468 6520 666f  onts from the fo
+00002030: 6e74 206d 6f64 756c 650a 2020 2020 2d20  nt module.    - 
+00002040: 4669 6c74 6572 2066 6f6e 7473 2074 6f20  Filter fonts to 
+00002050: 6f6e 6c79 2074 686f 7365 2077 6974 6820  only those with 
+00002060: 6120 6669 7865 6420 7769 6474 680a 2020  a fixed width.  
+00002070: 2020 2d20 4275 696c 6420 6120 6469 6374    - Build a dict
+00002080: 696f 6e61 7279 2077 6974 6820 666f 6e74  ionary with font
+00002090: 206e 616d 6520 6173 206b 6579 2061 6e64   name as key and
+000020a0: 2066 616d 696c 7920 6173 2076 616c 7565   family as value
+000020b0: 0a20 2020 2022 2222 0a20 2020 2023 204d  .    """.    # M
+000020c0: 616b 6520 7375 7265 2077 6520 6861 7665  ake sure we have
+000020d0: 2074 6865 2054 6b69 6e74 6572 2077 696e   the Tkinter win
+000020e0: 646f 772f 726f 6f74 0a20 2020 2067 6574  dow/root.    get
+000020f0: 5f74 6b28 290a 2020 2020 666f 6e74 7320  _tk().    fonts 
+00002100: 3d20 5b66 6f6e 742e 466f 6e74 2866 616d  = [font.Font(fam
+00002110: 696c 793d 6629 2066 6f72 2066 2069 6e20  ily=f) for f in 
+00002120: 666f 6e74 2e66 616d 696c 6965 7328 295d  font.families()]
+00002130: 0a20 2020 2072 6574 7572 6e20 7b66 2e6e  .    return {f.n
+00002140: 616d 653a 2066 2e61 6374 7561 6c28 2266  ame: f.actual("f
+00002150: 616d 696c 7922 2920 666f 7220 6620 696e  amily") for f in
+00002160: 2066 6f6e 7473 2069 6620 662e 6d65 7472   fonts if f.metr
+00002170: 6963 7328 2266 6978 6564 2229 7d0a 0a0a  ics("fixed")}...
+00002180: 2320 4275 696c 6420 6c69 7374 206f 6620  # Build list of 
+00002190: 616c 6c20 6176 6169 6c61 626c 6520 6d6f  all available mo
+000021a0: 6e6f 7370 6163 6520 666f 6e74 730a 6465  nospace fonts.de
+000021b0: 6620 6765 745f 6d6f 6e6f 7370 6163 655f  f get_monospace_
+000021c0: 666f 6e74 7328 2920 2d3e 2064 6963 743a  fonts() -> dict:
+000021d0: 0a20 2020 2022 2222 0a20 2020 2052 6574  .    """.    Ret
+000021e0: 7572 6e73 206d 6f6e 6f73 7061 6365 2066  urns monospace f
+000021f0: 6f6e 7473 2066 726f 6d20 7379 7374 656d  onts from system
+00002200: 2066 6f6e 7473 2e0a 2020 2020 4172 6773   fonts..    Args
+00002210: 3a0a 2020 2020 2020 2020 666f 6e74 733a  :.        fonts:
+00002220: 2041 6c6c 2073 7973 7465 6d20 666f 6e74   All system font
+00002230: 730a 2020 2020 5265 7475 726e 733a 0a20  s.    Returns:. 
+00002240: 2020 2020 2020 2066 6f6e 745f 6974 656d         font_item
+00002250: 733a 204c 6973 7420 6f66 206d 6f6e 6f73  s: List of monos
+00002260: 7061 6365 2066 6f6e 7473 0a20 2020 2020  pace fonts.     
+00002270: 2020 2072 6573 3a20 4c69 7374 2063 6f6e     res: List con
+00002280: 7461 696e 696e 6720 436f 7572 6965 7220  taining Courier 
+00002290: 6f72 2064 6566 6175 6c74 204d 6f6e 6163  or default Monac
+000022a0: 6f20 666f 6e74 0a20 2020 202d 2047 6574  o font.    - Get
+000022b0: 2061 6c6c 2073 7973 7465 6d20 666f 6e74   all system font
+000022c0: 730a 2020 2020 2d20 4669 6c74 6572 2066  s.    - Filter f
+000022d0: 6f6e 7473 2074 6f20 6f6e 6c79 2069 6e63  onts to only inc
+000022e0: 6c75 6465 206d 6f6e 6f73 7061 6365 2066  lude monospace f
+000022f0: 6f6e 7473 2065 7863 6c75 6469 6e67 2057  onts excluding W
+00002300: 696e 6764 696e 6773 0a20 2020 202d 2046  ingdings.    - F
+00002310: 696e 6420 436f 7572 6965 7220 666f 6e74  ind Courier font
+00002320: 2069 6e20 6c69 7374 2061 6e64 2073 6574   in list and set
+00002330: 2061 7320 7265 730a 2020 2020 2d20 4966   as res.    - If
+00002340: 2043 6f75 7269 6572 206e 6f74 2066 6f75   Courier not fou
+00002350: 6e64 2c20 7365 7420 4d6f 6e61 636f 2061  nd, set Monaco a
+00002360: 7320 6465 6661 756c 7420 7265 730a 2020  s default res.  
+00002370: 2020 2d20 5265 7475 726e 206c 6973 7473    - Return lists
+00002380: 206f 6620 6d6f 6e6f 7370 6163 6520 666f   of monospace fo
+00002390: 6e74 7320 616e 6420 436f 7572 6965 722f  nts and Courier/
+000023a0: 4d6f 6e61 636f 2066 6f6e 740a 2020 2020  Monaco font.    
+000023b0: 2222 220a 2020 2020 666f 6e74 7320 3d20  """.    fonts = 
+000023c0: 6765 745f 6d6f 6e6f 5f66 6f6e 7473 2829  get_mono_fonts()
+000023d0: 0a20 2020 2066 6f6e 745f 6974 656d 7320  .    font_items 
+000023e0: 3d20 5b22 436f 7572 6965 7222 5d0a 2020  = ["Courier"].  
+000023f0: 2020 666f 6e74 5f69 7465 6d73 203d 205b    font_items = [
+00002400: 7661 6c75 6520 666f 7220 7661 6c75 6520  value for value 
+00002410: 696e 2066 6f6e 7473 2e76 616c 7565 7328  in fonts.values(
+00002420: 2920 6966 2022 5769 6e67 6469 6e67 7322  ) if "Wingdings"
+00002430: 206e 6f74 2069 6e20 7661 6c75 655d 0a20   not in value]. 
+00002440: 2020 2023 2046 696e 6420 7768 6963 6820     # Find which 
+00002450: 436f 7572 6965 7220 666f 6e74 2069 7320  Courier font is 
+00002460: 696e 206f 7572 206c 6973 7420 616e 6420  in our list and 
+00002470: 7365 742e 0a20 2020 2072 6573 203d 205b  set..    res = [
+00002480: 6920 666f 7220 6920 696e 2066 6f6e 745f  i for i in font_
+00002490: 6974 656d 7320 6966 2022 436f 7572 6965  items if "Courie
+000024a0: 7222 2069 6e20 695d 0a20 2020 2023 2049  r" in i].    # I
+000024b0: 6620 436f 7572 6965 7220 6973 206e 6f74  f Courier is not
+000024c0: 2066 6f75 6e64 2066 6f72 2073 6f6d 6520   found for some 
+000024d0: 7265 6173 6f6e 2c20 6465 6661 756c 7420  reason, default 
+000024e0: 746f 204d 6f6e 6163 6f0a 2020 2020 6966  to Monaco.    if
+000024f0: 206e 6f74 2072 6573 3a0a 2020 2020 2020   not res:.      
+00002500: 2020 7265 7320 3d20 5b69 2066 6f72 2069    res = [i for i
+00002510: 2069 6e20 666f 6e74 5f69 7465 6d73 2069   in font_items i
+00002520: 6620 224d 6f6e 6163 6f22 2069 6e20 695d  f "Monaco" in i]
+00002530: 0a20 2020 2072 6574 7572 6e20 666f 6e74  .    return font
+00002540: 5f69 7465 6d73 2c20 7265 730a 0a0a 2320  _items, res...# 
+00002550: 5069 6e67 2074 6865 2041 6e64 726f 6964  Ping the Android
+00002560: 2065 7669 6365 2074 6f20 6d61 6b65 2073   evice to make s
+00002570: 7572 6520 6974 2069 7320 7265 6163 6861  ure it is reacha
+00002580: 626c 652e 0a64 6566 2070 696e 675f 616e  ble..def ping_an
+00002590: 6472 6f69 645f 6465 7669 6365 2873 656c  droid_device(sel
+000025a0: 662c 2069 705f 6164 6472 6573 733a 2073  f, ip_address: s
+000025b0: 7472 2c20 706f 7274 5f6e 756d 6265 723a  tr, port_number:
+000025c0: 2073 7472 2920 2d3e 2062 6f6f 6c3a 2020   str) -> bool:  
+000025d0: 2320 6e6f 7161 3a20 414e 4e30 3031 0a20  # noqa: ANN001. 
+000025e0: 2020 2023 2054 6865 2066 6f6c 6c6f 7769     # The followi
+000025f0: 6e67 2073 686f 756c 6420 7265 7475 726e  ng should return
+00002600: 2061 206c 6973 743a 205b 6970 5f61 6464   a list: [ip_add
+00002610: 7265 7373 3a70 6f72 745f 6e75 6d62 6572  ress:port_number
+00002620: 2c20 6669 6c65 5f6c 6f63 6174 696f 6e5d  , file_location]
+00002630: 0a20 2020 2022 2222 0a20 2020 2050 696e  .    """.    Pin
+00002640: 6773 2061 6e20 416e 6472 6f69 6420 6465  gs an Android de
+00002650: 7669 6365 0a20 2020 2041 7267 733a 0a20  vice.    Args:. 
+00002660: 2020 2020 2020 2069 705f 6164 6472 6573         ip_addres
+00002670: 733a 2073 7472 202d 2054 4350 2049 5020  s: str - TCP IP 
+00002680: 6164 6472 6573 7320 6f66 2074 6865 2041  address of the A
+00002690: 6e64 726f 6964 2064 6576 6963 650a 2020  ndroid device.  
+000026a0: 2020 2020 2020 706f 7274 5f6e 756d 6265        port_numbe
+000026b0: 723a 2073 7472 202d 2054 4350 2070 6f72  r: str - TCP por
+000026c0: 7420 6e75 6d62 6572 206f 6620 7468 6520  t number of the 
+000026d0: 416e 6472 6f69 6420 6465 7669 6365 0a20  Android device. 
+000026e0: 2020 2052 6574 7572 6e3a 0a20 2020 2020     Return:.     
+000026f0: 2020 2045 7272 6f72 3a20 5472 7565 2069     Error: True i
+00002700: 6620 6572 726f 722c 2066 616c 7365 2069  f error, false i
+00002710: 6620 616c 6c20 6973 2067 6f6f 642e 0a20  f all is good.. 
+00002720: 2020 2050 726f 6365 7373 696e 6720 4c6f     Processing Lo
+00002730: 6769 633a 0a20 2020 202d 2053 706c 6974  gic:.    - Split
+00002740: 7320 7468 6520 6261 636b 7570 5f69 6e66  s the backup_inf
+00002750: 6f20 7374 7269 6e67 2069 6e74 6f20 6970  o string into ip
+00002760: 5f61 6464 7265 7373 2c20 706f 7274 5f6e  _address, port_n
+00002770: 756d 6265 722c 2061 6e64 2066 696c 655f  umber, and file_
+00002780: 6c6f 6361 7469 6f6e 0a20 2020 202d 2056  location.    - V
+00002790: 616c 6964 6174 6573 2074 6865 2049 5020  alidates the IP 
+000027a0: 6164 6472 6573 732c 2070 6f72 7420 6e75  address, port nu
+000027b0: 6d62 6572 2c20 616e 6420 6669 6c65 206c  mber, and file l
+000027c0: 6f63 6174 696f 6e0a 2020 2020 2d20 5069  ocation.    - Pi
+000027d0: 6e67 7320 7468 6520 4950 2061 6464 7265  ngs the IP addre
+000027e0: 7373 2074 6f20 6368 6563 6b20 636f 6e6e  ss to check conn
+000027f0: 6563 7469 7669 7479 0a20 2020 202d 2052  ectivity.    - R
+00002800: 6574 7572 6e73 2061 2074 7570 6c65 2069  eturns a tuple i
+00002810: 6e64 6963 6174 696e 6720 7375 6363 6573  ndicating succes
+00002820: 732f 6661 696c 7572 6520 616e 6420 616e  s/failure and an
+00002830: 7920 6572 726f 7220 6d65 7373 6167 650a  y error message.
+00002840: 2020 2020 2222 220a 2020 2020 2320 5661      """.    # Va
+00002850: 6c69 6461 7465 2049 5020 4164 6472 6573  lidate IP Addres
+00002860: 730a 2020 2020 6966 2076 616c 6964 6174  s.    if validat
+00002870: 655f 6970 5f61 6464 7265 7373 2869 705f  e_ip_address(ip_
+00002880: 6164 6472 6573 7329 3a0a 2020 2020 2020  address):.      
+00002890: 2020 2320 5665 7269 6679 2074 6861 7420    # Verify that 
+000028a0: 7468 6520 686f 7374 2049 5020 6973 2072  the host IP is r
+000028b0: 6561 6368 6162 6c65 3a0a 2020 2020 2020  eachable:.      
+000028c0: 2020 7365 6c66 2e64 6973 706c 6179 5f6d    self.display_m
+000028d0: 6573 7361 6765 5f62 6f78 2866 2250 696e  essage_box(f"Pin
+000028e0: 6769 6e67 2061 6464 7265 7373 207b 6970  ging address {ip
+000028f0: 5f61 6464 7265 7373 7d2e 2020 506c 6561  _address}.  Plea
+00002900: 7365 2077 6169 742e 2e2e 222c 2022 4772  se wait...", "Gr
+00002910: 6565 6e22 290a 2020 2020 2020 2020 7365  een").        se
+00002920: 6c66 2e75 7064 6174 6528 2920 2023 2046  lf.update()  # F
+00002930: 6f72 6365 2061 2077 696e 646f 7720 7265  orce a window re
+00002940: 6672 6573 682e 0a0a 2020 2020 2020 2020  fresh...        
+00002950: 2320 5069 6e67 2049 5020 6164 6472 6573  # Ping IP addres
+00002960: 732e 0a20 2020 2020 2020 2072 6573 706f  s..        respo
+00002970: 6e73 6520 3d20 6f73 2e73 7973 7465 6d28  nse = os.system(
+00002980: 6622 7069 6e67 202d 6320 3120 2d74 3530  f"ping -c 1 -t50
+00002990: 203e 202f 6465 762f 6e75 6c6c 207b 6970   > /dev/null {ip
+000029a0: 5f61 6464 7265 7373 7d22 2920 2023 206e  _address}")  # n
+000029b0: 6f71 613a 2053 3630 350a 2020 2020 2020  oqa: S605.      
+000029c0: 2020 6966 2072 6573 706f 6e73 6520 213d    if response !=
+000029d0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+000029e0: 7365 6c66 2e62 6163 6b75 705f 6572 726f  self.backup_erro
+000029f0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00002a00: 2020 2066 227b 6970 5f61 6464 7265 7373     f"{ip_address
+00002a10: 7d20 6973 206e 6f74 2072 6561 6368 6162  } is not reachab
+00002a20: 6c65 2028 6572 726f 7220 7b72 6573 706f  le (error {respo
+00002a30: 6e73 657d 292e 2020 5472 7920 6167 6169  nse}).  Try agai
+00002a40: 6e2e 222c 0a20 2020 2020 2020 2020 2020  n.",.           
+00002a50: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
+00002a60: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+00002a70: 2020 2020 7365 6c66 2e64 6973 706c 6179      self.display
+00002a80: 5f6d 6573 7361 6765 5f62 6f78 2822 5069  _message_box("Pi
+00002a90: 6e67 2073 7563 6365 7373 6675 6c2e 222c  ng successful.",
+00002aa0: 2022 4772 6565 6e22 290a 2020 2020 656c   "Green").    el
+00002ab0: 7365 3a0a 2020 2020 2020 2020 7365 6c66  se:.        self
+00002ac0: 2e62 6163 6b75 705f 6572 726f 7228 0a20  .backup_error(. 
+00002ad0: 2020 2020 2020 2020 2020 2066 2249 6e76             f"Inv
+00002ae0: 616c 6964 2049 5020 6164 6472 6573 733a  alid IP address:
+00002af0: 207b 6970 5f61 6464 7265 7373 7d2e 2020   {ip_address}.  
+00002b00: 5472 7920 6167 6169 6e2e 222c 0a20 2020  Try again.",.   
+00002b10: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+00002b20: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00002b30: 2023 2056 616c 6964 6174 6520 706f 7274   # Validate port
+00002b40: 206e 756d 6265 720a 2020 2020 6966 2076   number.    if v
+00002b50: 616c 6964 6174 655f 706f 7274 2869 705f  alidate_port(ip_
+00002b60: 6164 6472 6573 732c 2070 6f72 745f 6e75  address, port_nu
+00002b70: 6d62 6572 2920 213d 2030 3a0a 2020 2020  mber) != 0:.    
+00002b80: 2020 2020 7365 6c66 2e62 6163 6b75 705f      self.backup_
+00002b90: 6572 726f 7228 0a20 2020 2020 2020 2020  error(.         
+00002ba0: 2020 2066 2249 6e76 616c 6964 2050 6f72     f"Invalid Por
+00002bb0: 7420 6e75 6d62 6572 3a20 7b70 6f72 745f  t number: {port_
+00002bc0: 6e75 6d62 6572 7d20 6f72 2074 6865 2067  number} or the g
+00002bd0: 6976 656e 2049 5020 6164 6472 6573 7320  iven IP address 
+00002be0: 646f 6573 206e 6f74 2070 6572 6d69 7420  does not permit 
+00002bf0: 6163 6365 7373 2074 6f20 7468 6973 2070  access to this p
+00002c00: 6f72 742e 2020 5472 7920 6167 6169 6e2e  ort.  Try again.
+00002c10: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
+00002c20: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00002c30: 650a 0a20 2020 2023 2056 616c 6964 2049  e..    # Valid I
+00002c40: 5020 4164 6472 6573 732e 2e2e 676f 6f64  P Address...good
+00002c50: 2070 696e 672e 0a20 2020 2072 6574 7572   ping..    retur
+00002c60: 6e20 5472 7565 0a0a 0a23 2043 6c65 6172  n True...# Clear
+00002c70: 2061 6c6c 2062 7574 746f 6e73 2061 7373   all buttons ass
+00002c80: 6f63 6961 7465 6420 7769 7468 2066 6574  ociated with fet
+00002c90: 6368 696e 6720 7468 6520 6261 636b 7570  ching the backup
+00002ca0: 2066 696c 6520 6672 6f6d 2041 6e64 726f   file from Andro
+00002cb0: 6964 2064 6576 6963 650a 6465 6620 636c  id device.def cl
+00002cc0: 6561 725f 616e 6472 6f69 645f 6275 7474  ear_android_butt
+00002cd0: 6f6e 7328 7365 6c66 2920 2d3e 204e 6f6e  ons(self) -> Non
+00002ce0: 653a 2020 2320 6e6f 7161 3a20 414e 4e30  e:  # noqa: ANN0
+00002cf0: 3031 0a20 2020 2022 2222 0a20 2020 2043  01.    """.    C
+00002d00: 6c65 6172 7320 616e 6472 6f69 6420 6465  lears android de
+00002d10: 7669 6365 2063 6f6e 6669 6775 7261 7469  vice configurati
+00002d20: 6f6e 2062 7574 746f 6e73 2061 6e64 2064  on buttons and d
+00002d30: 6973 706c 6179 7320 6261 636b 7570 2062  isplays backup b
+00002d40: 7574 746f 6e0a 2020 2020 4172 6773 3a0a  utton.    Args:.
+00002d50: 2020 2020 2020 2020 7365 6c66 3a20 5468          self: Th
+00002d60: 6520 636c 6173 7320 696e 7374 616e 6365  e class instance
+00002d70: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+00002d80: 2020 2020 2020 4e6f 6e65 0a20 2020 202d        None.    -
+00002d90: 2044 6573 7472 6f79 7320 4950 2c20 706f   Destroys IP, po
+00002da0: 7274 2c20 6669 6c65 2065 6e74 7279 2061  rt, file entry a
+00002db0: 6e64 206c 6162 656c 2077 6964 6765 7473  nd label widgets
+00002dc0: 0a20 2020 202d 2044 6573 7472 6f79 7320  .    - Destroys 
+00002dd0: 6765 7420 6261 636b 7570 2062 7574 746f  get backup butto
+00002de0: 6e0a 2020 2020 2d20 4469 7370 6c61 7973  n.    - Displays
+00002df0: 206e 6577 2062 6163 6b75 7020 6275 7474   new backup butt
+00002e00: 6f6e 2077 6974 6820 6361 6c6c 6261 636b  on with callback
+00002e10: 2074 6f20 6765 745f 6261 636b 7570 5f65   to get_backup_e
+00002e20: 7665 6e74 206d 6574 686f 6422 2222 0a0a  vent method"""..
+00002e30: 2020 2020 2320 4561 6368 2065 6c65 6d65      # Each eleme
+00002e40: 6e74 2074 6f20 6265 2064 6573 746f 7279  nt to be destory
+00002e50: 6564 206e 6565 6473 2061 2073 7570 7072  ed needs a suppr
+00002e60: 6573 7369 6f6e 2073 696e 6365 2061 6e79  ession since any
+00002e70: 206f 6e65 2073 7570 7072 6573 7369 6f6e   one suppression
+00002e80: 2077 696c 6c20 6265 2074 7269 6767 6572   will be trigger
+00002e90: 6564 2069 6620 616e 7920 6f6e 6520 6f66  ed if any one of
+00002ea0: 0a20 2020 2023 2074 6865 2065 6c65 6d65  .    # the eleme
+00002eb0: 6e74 7320 6973 206e 6f74 2064 6566 696e  nts is not defin
+00002ec0: 6564 2e0a 2020 2020 7769 7468 2063 6f6e  ed..    with con
+00002ed0: 7465 7874 6c69 622e 7375 7070 7265 7373  textlib.suppress
+00002ee0: 2841 7474 7269 6275 7465 4572 726f 7229  (AttributeError)
+00002ef0: 3a0a 2020 2020 2020 2020 7365 6c66 2e69  :.        self.i
+00002f00: 705f 656e 7472 792e 6465 7374 726f 7928  p_entry.destroy(
+00002f10: 290a 2020 2020 7769 7468 2063 6f6e 7465  ).    with conte
+00002f20: 7874 6c69 622e 7375 7070 7265 7373 2841  xtlib.suppress(A
+00002f30: 7474 7269 6275 7465 4572 726f 7229 3a0a  ttributeError):.
+00002f40: 2020 2020 2020 2020 7365 6c66 2e70 6f72          self.por
+00002f50: 745f 656e 7472 792e 6465 7374 726f 7928  t_entry.destroy(
+00002f60: 290a 2020 2020 7769 7468 2063 6f6e 7465  ).    with conte
+00002f70: 7874 6c69 622e 7375 7070 7265 7373 2841  xtlib.suppress(A
+00002f80: 7474 7269 6275 7465 4572 726f 7229 3a0a  ttributeError):.
+00002f90: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
+00002fa0: 655f 656e 7472 792e 6465 7374 726f 7928  e_entry.destroy(
+00002fb0: 290a 2020 2020 7769 7468 2063 6f6e 7465  ).    with conte
+00002fc0: 7874 6c69 622e 7375 7070 7265 7373 2841  xtlib.suppress(A
+00002fd0: 7474 7269 6275 7465 4572 726f 7229 3a0a  ttributeError):.
+00002fe0: 2020 2020 2020 2020 7365 6c66 2e69 705f          self.ip_
+00002ff0: 6c61 6265 6c2e 6465 7374 726f 7928 290a  label.destroy().
+00003000: 2020 2020 7769 7468 2063 6f6e 7465 7874      with context
+00003010: 6c69 622e 7375 7070 7265 7373 2841 7474  lib.suppress(Att
+00003020: 7269 6275 7465 4572 726f 7229 3a0a 2020  ributeError):.  
+00003030: 2020 2020 2020 7365 6c66 2e70 6f72 745f        self.port_
+00003040: 6c61 6265 6c2e 6465 7374 726f 7928 290a  label.destroy().
+00003050: 2020 2020 7769 7468 2063 6f6e 7465 7874      with context
+00003060: 6c69 622e 7375 7070 7265 7373 2841 7474  lib.suppress(Att
+00003070: 7269 6275 7465 4572 726f 7229 3a0a 2020  ributeError):.  
+00003080: 2020 2020 2020 7365 6c66 2e66 696c 655f        self.file_
+00003090: 6c61 6265 6c2e 6465 7374 726f 7928 290a  label.destroy().
+000030a0: 2020 2020 7769 7468 2063 6f6e 7465 7874      with context
+000030b0: 6c69 622e 7375 7070 7265 7373 2841 7474  lib.suppress(Att
+000030c0: 7269 6275 7465 4572 726f 7229 3a0a 2020  ributeError):.  
+000030d0: 2020 2020 2020 7365 6c66 2e67 6574 5f62        self.get_b
+000030e0: 6163 6b75 705f 6275 7474 6f6e 2e64 6573  ackup_button.des
+000030f0: 7472 6f79 2829 0a20 2020 2077 6974 6820  troy().    with 
+00003100: 636f 6e74 6578 746c 6962 2e73 7570 7072  contextlib.suppr
+00003110: 6573 7328 4174 7472 6962 7574 6545 7272  ess(AttributeErr
+00003120: 6f72 293a 0a20 2020 2020 2020 2073 656c  or):.        sel
+00003130: 662e 6361 6e63 656c 5f65 6e74 7279 5f62  f.cancel_entry_b
+00003140: 7574 746f 6e2e 6465 7374 726f 7928 290a  utton.destroy().
+00003150: 2020 2020 7769 7468 2063 6f6e 7465 7874      with context
+00003160: 6c69 622e 7375 7070 7265 7373 2841 7474  lib.suppress(Att
+00003170: 7269 6275 7465 4572 726f 7229 3a0a 2020  ributeError):.  
+00003180: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003190: 6669 6c65 735f 6275 7474 6f6e 2e64 6573  files_button.des
+000031a0: 7472 6f79 2829 0a20 2020 2077 6974 6820  troy().    with 
+000031b0: 636f 6e74 6578 746c 6962 2e73 7570 7072  contextlib.suppr
+000031c0: 6573 7328 4174 7472 6962 7574 6545 7272  ess(AttributeErr
+000031d0: 6f72 293a 0a20 2020 2020 2020 2073 656c  or):.        sel
+000031e0: 662e 6c61 6265 6c5f 6f72 2e64 6573 7472  f.label_or.destr
+000031f0: 6f79 2829 0a20 2020 2077 6974 6820 636f  oy().    with co
+00003200: 6e74 6578 746c 6962 2e73 7570 7072 6573  ntextlib.suppres
+00003210: 7328 4174 7472 6962 7574 6545 7272 6f72  s(AttributeError
+00003220: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00003230: 6669 6c65 6c69 7374 5f6c 6162 656c 2e64  filelist_label.d
+00003240: 6573 7472 6f79 2829 0a20 2020 2077 6974  estroy().    wit
+00003250: 6820 636f 6e74 6578 746c 6962 2e73 7570  h contextlib.sup
+00003260: 7072 6573 7328 4174 7472 6962 7574 6545  press(AttributeE
+00003270: 7272 6f72 293a 0a20 2020 2020 2020 2073  rror):.        s
+00003280: 656c 662e 6669 6c65 6c69 7374 5f6f 7074  elf.filelist_opt
+00003290: 696f 6e2e 6465 7374 726f 7928 290a 2020  ion.destroy().  
+000032a0: 2020 7769 7468 2063 6f6e 7465 7874 6c69    with contextli
+000032b0: 622e 7375 7070 7265 7373 2841 7474 7269  b.suppress(Attri
+000032c0: 6275 7465 4572 726f 7229 3a0a 2020 2020  buteError):.    
+000032d0: 2020 2020 7365 6c66 2e6c 6973 745f 6669      self.list_fi
+000032e0: 6c65 735f 7175 6572 795f 6275 7474 6f6e  les_query_button
+000032f0: 2e64 6573 7472 6f79 2829 0a20 2020 2077  .destroy().    w
+00003300: 6974 6820 636f 6e74 6578 746c 6962 2e73  ith contextlib.s
+00003310: 7570 7072 6573 7328 4174 7472 6962 7574  uppress(Attribut
+00003320: 6545 7272 6f72 293a 2020 2320 4465 7374  eError):  # Dest
+00003330: 726f 7920 7570 6772 6164 6520 6275 7474  roy upgrade butt
+00003340: 6f6e 2073 696e 6365 2066 696c 6520 6c6f  on since file lo
+00003350: 6361 7469 6f6e 2077 6f75 6c64 2073 6974  cation would sit
+00003360: 206f 6e20 746f 7020 6f66 2069 742e 0a20   on top of it.. 
+00003370: 2020 2020 2020 2073 656c 662e 7570 6772         self.upgr
+00003380: 6164 655f 6275 7474 6f6e 2e64 6573 7472  ade_button.destr
+00003390: 6f79 2829 0a0a 2020 2020 7365 6c66 2e67  oy()..    self.g
+000033a0: 6574 5f62 6163 6b75 705f 6275 7474 6f6e  et_backup_button
+000033b0: 203d 2073 656c 662e 6469 7370 6c61 795f   = self.display_
+000033c0: 6261 636b 7570 5f62 7574 746f 6e28 0a20  backup_button(. 
+000033d0: 2020 2020 2020 2022 4765 7420 584d 4c20         "Get XML 
+000033e0: 6672 6f6d 2041 6e64 726f 6964 2044 6576  from Android Dev
+000033f0: 6963 6522 2c0a 2020 2020 2020 2020 2223  ice",.        "#
+00003400: 3234 3646 4236 222c 0a20 2020 2020 2020  246FB6",.       
+00003410: 2022 2336 3536 3366 6622 2c0a 2020 2020   "#6563ff",.    
+00003420: 2020 2020 7365 6c66 2e67 6574 5f62 6163      self.get_bac
+00003430: 6b75 705f 6576 656e 742c 0a20 2020 2029  kup_event,.    )
+00003440: 0a0a 0a23 2043 6f6d 7061 7265 2074 776f  ...# Compare two
+00003450: 2076 6572 7369 6f6e 7320 616e 6420 7265   versions and re
+00003460: 7475 726e 2054 7275 6520 6966 2076 6572  turn True if ver
+00003470: 7369 6f6e 3220 6973 2067 7265 6174 6572  sion2 is greater
+00003480: 2074 6861 6e20 7665 7273 696f 6e31 2e0a   than version1..
+00003490: 6465 6620 6973 5f76 6572 7369 6f6e 5f67  def is_version_g
+000034a0: 7265 6174 6572 2876 6572 7369 6f6e 313a  reater(version1:
+000034b0: 2073 7472 2c20 7665 7273 696f 6e32 3a20   str, version2: 
+000034c0: 7374 7229 202d 3e20 626f 6f6c 3a0a 2020  str) -> bool:.  
+000034d0: 2020 2222 220a 2020 2020 5468 6973 2066    """.    This f
+000034e0: 756e 6374 696f 6e20 6368 6563 6b73 2069  unction checks i
+000034f0: 6620 7665 7273 696f 6e32 2069 7320 6772  f version2 is gr
+00003500: 6561 7465 7220 7468 616e 2076 6572 7369  eater than versi
+00003510: 6f6e 312e 0a0a 2020 2020 4172 6773 3a0a  on1...    Args:.
+00003520: 2020 2020 2020 2020 7665 7273 696f 6e31          version1
+00003530: 3a20 4120 7374 7269 6e67 2072 6570 7265  : A string repre
+00003540: 7365 6e74 696e 6720 7468 6520 6669 7273  senting the firs
+00003550: 7420 7665 7273 696f 6e20 696e 2074 6865  t version in the
+00003560: 2066 6f72 6d61 7420 226d 616a 6f72 2e6d   format "major.m
+00003570: 696e 6f72 2e70 6174 6368 222e 0a20 2020  inor.patch"..   
+00003580: 2020 2020 2076 6572 7369 6f6e 323a 2041       version2: A
+00003590: 2073 7472 696e 6720 7265 7072 6573 656e   string represen
+000035a0: 7469 6e67 2074 6865 2073 6563 6f6e 6420  ting the second 
+000035b0: 7665 7273 696f 6e20 696e 2074 6865 2066  version in the f
+000035c0: 6f72 6d61 7420 226d 616a 6f72 2e6d 696e  ormat "major.min
+000035d0: 6f72 2e70 6174 6368 222e 0a0a 2020 2020  or.patch"...    
+000035e0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+000035f0: 2054 7275 6520 6966 2076 6572 7369 6f6e   True if version
+00003600: 3220 6973 2067 7265 6174 6572 2074 6861  2 is greater tha
+00003610: 6e20 7665 7273 696f 6e31 2c20 4661 6c73  n version1, Fals
+00003620: 6520 6f74 6865 7277 6973 652e 0a20 2020  e otherwise..   
+00003630: 2022 2222 0a0a 2020 2020 2320 5370 6c69   """..    # Spli
+00003640: 7420 7468 6520 7665 7273 696f 6e73 2062  t the versions b
+00003650: 7920 222e 220a 2020 2020 7631 5f70 6172  y ".".    v1_par
+00003660: 7473 203d 205b 696e 7428 7829 2066 6f72  ts = [int(x) for
+00003670: 2078 2069 6e20 7665 7273 696f 6e31 2e73   x in version1.s
+00003680: 706c 6974 2822 2e22 295d 0a20 2020 2076  plit(".")].    v
+00003690: 325f 7061 7274 7320 3d20 5b69 6e74 2878  2_parts = [int(x
+000036a0: 2920 666f 7220 7820 696e 2076 6572 7369  ) for x in versi
+000036b0: 6f6e 322e 7370 6c69 7428 222e 2229 5d0a  on2.split(".")].
+000036c0: 0a20 2020 2023 2049 7465 7261 7465 2074  .    # Iterate t
+000036d0: 6872 6f75 6768 2065 6163 6820 7061 7274  hrough each part
+000036e0: 206f 6620 7468 6520 7665 7273 696f 6e0a   of the version.
+000036f0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00003700: 6765 286d 696e 286c 656e 2876 315f 7061  ge(min(len(v1_pa
+00003710: 7274 7329 2c20 6c65 6e28 7632 5f70 6172  rts), len(v2_par
+00003720: 7473 2929 293a 0a20 2020 2020 2020 2069  ts))):.        i
+00003730: 6620 7631 5f70 6172 7473 5b69 5d20 3c20  f v1_parts[i] < 
+00003740: 7632 5f70 6172 7473 5b69 5d3a 0a20 2020  v2_parts[i]:.   
+00003750: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00003760: 5472 7565 0a20 2020 2020 2020 2069 6620  True.        if 
+00003770: 7631 5f70 6172 7473 5b69 5d20 3e20 7632  v1_parts[i] > v2
+00003780: 5f70 6172 7473 5b69 5d3a 0a20 2020 2020  _parts[i]:.     
+00003790: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000037a0: 6c73 650a 0a20 2020 2023 2049 6620 616c  lse..    # If al
+000037b0: 6c20 7061 7274 7320 6172 6520 6571 7561  l parts are equa
+000037c0: 6c2c 2063 6865 636b 206c 656e 6774 680a  l, check length.
+000037d0: 2020 2020 7265 7475 726e 206c 656e 2876      return len(v
+000037e0: 325f 7061 7274 7329 203e 206c 656e 2876  2_parts) > len(v
+000037f0: 315f 7061 7274 7329 0a0a 0a23 2043 6865  1_parts)...# Che
+00003800: 636b 7320 6966 2032 3420 686f 7572 7320  cks if 24 hours 
+00003810: 6861 7665 2070 6173 7365 6420 7369 6e63  have passed sinc
+00003820: 6520 7468 6520 6769 7665 6e20 7072 6576  e the given prev
+00003830: 696f 7573 2064 6174 652e 0a64 6566 2069  ious date..def i
+00003840: 735f 6d6f 7265 5f74 6861 6e5f 3234 6872  s_more_than_24hr
+00003850: 7328 696e 7075 745f 6461 7465 7469 6d65  s(input_datetime
+00003860: 3a20 6461 7465 7469 6d65 2920 2d3e 2062  : datetime) -> b
+00003870: 6f6f 6c3a 0a20 2020 2022 2222 4368 6563  ool:.    """Chec
+00003880: 6b73 2069 6620 7468 6520 696e 7075 7420  ks if the input 
+00003890: 6461 7465 7469 6d65 2069 7320 6d6f 7265  datetime is more
+000038a0: 2074 6861 6e20 3234 2068 6f75 7273 2061   than 24 hours a
+000038b0: 676f 2e0a 2020 2020 4172 6775 6d65 6e74  go..    Argument
+000038c0: 733a 0a20 2020 2020 2020 2069 6e70 7574  s:.        input
+000038d0: 5f64 6174 6574 696d 6520 2864 6174 6574  _datetime (datet
+000038e0: 696d 6529 3a20 5468 6520 6461 7465 7469  ime): The dateti
+000038f0: 6d65 2074 6f20 6265 2063 6865 636b 6564  me to be checked
+00003900: 2e0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+00003910: 2020 2020 2020 2062 6f6f 6c3a 2054 7275         bool: Tru
+00003920: 6520 6966 2069 6e70 7574 2064 6174 6574  e if input datet
+00003930: 696d 6520 6973 206d 6f72 6520 7468 616e  ime is more than
+00003940: 2032 3420 686f 7572 7320 6167 6f2c 2046   24 hours ago, F
+00003950: 616c 7365 206f 7468 6572 7769 7365 2e0a  alse otherwise..
+00003960: 2020 2020 5072 6f63 6573 7369 6e67 204c      Processing L
+00003970: 6f67 6963 3a0a 2020 2020 2020 2020 2d20  ogic:.        - 
+00003980: 4361 6c63 756c 6174 6520 7365 636f 6e64  Calculate second
+00003990: 7320 696e 2032 3420 686f 7572 732e 0a20  s in 24 hours.. 
+000039a0: 2020 2020 2020 202d 2047 6574 2063 7572         - Get cur
+000039b0: 7265 6e74 2064 6174 6574 696d 652e 0a20  rent datetime.. 
+000039c0: 2020 2020 2020 202d 2043 6865 636b 2069         - Check i
+000039d0: 6620 6469 6666 6572 656e 6365 2062 6574  f difference bet
+000039e0: 7765 656e 2063 7572 7265 6e74 2064 6174  ween current dat
+000039f0: 6574 696d 6520 616e 6420 696e 7075 7420  etime and input 
+00003a00: 6461 7465 7469 6d65 2069 7320 6772 6561  datetime is grea
+00003a10: 7465 7220 7468 616e 2032 3420 686f 7572  ter than 24 hour
+00003a20: 732e 0a20 2020 2020 2020 202d 2052 6574  s..        - Ret
+00003a30: 7572 6e20 7265 7375 6c74 2061 7320 626f  urn result as bo
+00003a40: 6f6c 6561 6e2e 2222 220a 2020 2020 7477  olean.""".    tw
+00003a50: 656e 7479 5f66 6f75 725f 686f 7572 7320  enty_four_hours 
+00003a60: 3d20 3836 3430 3020 2023 2073 6563 6f6e  = 86400  # secon
+00003a70: 6473 2069 6e20 3234 2068 6f75 7273 0a20  ds in 24 hours. 
+00003a80: 2020 2072 6574 7572 6e20 284e 4f57 5f54     return (NOW_T
+00003a90: 494d 4520 2d20 696e 7075 745f 6461 7465  IME - input_date
+00003aa0: 7469 6d65 292e 746f 7461 6c5f 7365 636f  time).total_seco
+00003ab0: 6e64 7328 2920 3e20 7477 656e 7479 5f66  nds() > twenty_f
+00003ac0: 6f75 725f 686f 7572 730a 0a0a 2320 4765  our_hours...# Ge
+00003ad0: 7420 5079 7069 2076 6572 7369 6f6e 2061  t Pypi version a
+00003ae0: 6e64 2072 6574 7572 6e20 5472 7565 2069  nd return True i
+00003af0: 6620 6974 2069 7320 6e65 7765 7220 7468  f it is newer th
+00003b00: 616e 206f 7572 2063 7572 7265 6e74 2076  an our current v
+00003b10: 6572 7369 6f6e 2e0a 6465 6620 6973 5f6e  ersion..def is_n
+00003b20: 6577 5f76 6572 7369 6f6e 2829 202d 3e20  ew_version() -> 
+00003b30: 626f 6f6c 3a0a 2020 2020 2222 220a 2020  bool:.    """.  
+00003b40: 2020 4368 6563 6b20 6966 2074 6865 206e    Check if the n
+00003b50: 6577 2076 6572 7369 6f6e 2069 7320 6176  ew version is av
+00003b60: 6169 6c61 626c 650a 2020 2020 4172 6773  ailable.    Args
+00003b70: 3a0a 2020 2020 2020 2020 7365 6c66 3a20  :.        self: 
+00003b80: 5468 6520 636c 6173 7320 696e 7374 616e  The class instan
+00003b90: 6365 0a20 2020 2052 6574 7572 6e73 3a0a  ce.    Returns:.
+00003ba0: 2020 2020 2020 2020 626f 6f6c 3a20 5472          bool: Tr
+00003bb0: 7565 2069 6620 6e65 7720 7665 7273 696f  ue if new versio
+00003bc0: 6e20 6973 2061 7661 696c 6162 6c65 2c20  n is available, 
+00003bd0: 4661 6c73 6520 6966 206e 6f74 2222 220a  False if not""".
+00003be0: 2020 2020 2320 4368 6563 6b20 6966 206e      # Check if n
+00003bf0: 6577 6572 2076 6572 7369 6f6e 206f 6620  ewer version of 
+00003c00: 6f75 7220 636f 6465 2069 7320 6176 6169  our code is avai
+00003c10: 6c61 626c 6520 6f6e 2050 7970 692e 0a20  lable on Pypi.. 
+00003c20: 2020 2023 2069 6620 6973 5f6d 6f72 655f     # if is_more_
+00003c30: 7468 616e 5f32 3468 7273 2850 7269 6d65  than_24hrs(Prime
+00003c40: 4974 656d 732e 6c61 7374 5f72 756e 293a  Items.last_run):
+00003c50: 2020 2320 4f6e 6c79 2063 6865 636b 2065    # Only check e
+00003c60: 7665 7279 2032 3420 686f 7572 732e 0a20  very 24 hours.. 
+00003c70: 2020 2070 7970 695f 7665 7273 696f 6e5f     pypi_version_
+00003c80: 636f 6465 203d 2067 6574 5f70 7970 695f  code = get_pypi_
+00003c90: 7665 7273 696f 6e28 290a 2020 2020 6966  version().    if
+00003ca0: 2070 7970 695f 7665 7273 696f 6e5f 636f   pypi_version_co
+00003cb0: 6465 3a0a 2020 2020 2020 2020 7079 7069  de:.        pypi
+00003cc0: 5f76 6572 7369 6f6e 203d 2070 7970 695f  _version = pypi_
+00003cd0: 7665 7273 696f 6e5f 636f 6465 2e73 706c  version_code.spl
+00003ce0: 6974 2822 3d3d 2229 5b31 5d0a 2020 2020  it("==")[1].    
+00003cf0: 2020 2020 5072 696d 6549 7465 6d73 2e6c      PrimeItems.l
+00003d00: 6173 745f 7275 6e20 3d20 4e4f 575f 5449  ast_run = NOW_TI
+00003d10: 4d45 2020 2320 5570 6461 7465 206c 6173  ME  # Update las
+00003d20: 7420 7275 6e20 746f 206e 6f77 2073 696e  t run to now sin
+00003d30: 6365 2077 6520 6172 6520 646f 696e 6720  ce we are doing 
+00003d40: 7468 6520 6368 6563 6b2e 0a20 2020 2020  the check..     
+00003d50: 2020 2072 6574 7572 6e20 6973 5f76 6572     return is_ver
+00003d60: 7369 6f6e 5f67 7265 6174 6572 2856 4552  sion_greater(VER
+00003d70: 5349 4f4e 2c20 7079 7069 5f76 6572 7369  SION, pypi_versi
+00003d80: 6f6e 290a 2020 2020 7265 7475 726e 2046  on).    return F
+00003d90: 616c 7365 0a0a 0a23 204c 6973 7420 7468  alse...# List th
+00003da0: 6520 584d 4c20 6669 6c65 7320 6f6e 2074  e XML files on t
+00003db0: 6865 2041 6e64 726f 6964 2064 6576 6963  he Android devic
+00003dc0: 650a 6465 6620 6765 745f 6c69 7374 5f6f  e.def get_list_o
+00003dd0: 665f 6669 6c65 7328 6970 5f61 6464 7265  f_files(ip_addre
+00003de0: 7373 3a20 7374 722c 2069 705f 706f 7274  ss: str, ip_port
+00003df0: 3a20 7374 722c 2066 696c 655f 6c6f 6361  : str, file_loca
+00003e00: 7469 6f6e 3a20 7374 7229 202d 3e20 7475  tion: str) -> tu
+00003e10: 706c 653a 0a20 2020 2022 2222 4765 7420  ple:.    """Get 
+00003e20: 6c69 7374 206f 6620 6669 6c65 7320 6672  list of files fr
+00003e30: 6f6d 2067 6976 656e 2049 5020 6164 6472  om given IP addr
+00003e40: 6573 732e 0a20 2020 2050 6172 616d 6574  ess..    Paramet
+00003e50: 6572 733a 0a20 2020 2020 2020 202d 2069  ers:.        - i
+00003e60: 705f 6164 6472 6573 7320 2873 7472 293a  p_address (str):
+00003e70: 2049 5020 6164 6472 6573 7320 746f 2063   IP address to c
+00003e80: 6f6e 6e65 6374 2074 6f2e 0a20 2020 2020  onnect to..     
+00003e90: 2020 202d 2069 705f 706f 7274 2028 7374     - ip_port (st
+00003ea0: 7229 3a20 506f 7274 206e 756d 6265 7220  r): Port number 
+00003eb0: 746f 2063 6f6e 6e65 6374 2074 6f2e 0a20  to connect to.. 
+00003ec0: 2020 2020 2020 202d 2066 696c 655f 6c6f         - file_lo
+00003ed0: 6361 7469 6f6e 2028 7374 7229 3a20 4c6f  cation (str): Lo
+00003ee0: 6361 7469 6f6e 206f 6620 7468 6520 6669  cation of the fi
+00003ef0: 6c65 2074 6f20 7265 7472 6965 7665 2e0a  le to retrieve..
+00003f00: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00003f10: 2020 2020 202d 2074 7570 6c65 3a20 5265       - tuple: Re
+00003f20: 7475 726e 2063 6f64 6520 616e 6420 6c69  turn code and li
+00003f30: 7374 206f 6620 6669 6c65 206c 6f63 6174  st of file locat
+00003f40: 696f 6e73 2e0a 2020 2020 5072 6f63 6573  ions..    Proces
+00003f50: 7369 6e67 204c 6f67 6963 3a0a 2020 2020  sing Logic:.    
+00003f60: 2020 2020 2d20 5265 7472 6965 7665 2066      - Retrieve f
+00003f70: 696c 6520 636f 6e74 656e 7473 2075 7369  ile contents usi
+00003f80: 6e67 2068 7474 705f 7265 7175 6573 742e  ng http_request.
+00003f90: 0a20 2020 2020 2020 202d 2049 6620 7265  .        - If re
+00003fa0: 7475 726e 2063 6f64 6520 6973 2030 2c20  turn code is 0, 
+00003fb0: 7370 6c69 7420 7468 6520 6465 636f 6465  split the decode
+00003fc0: 6420 7374 7269 6e67 2069 6e74 6f20 6120  d string into a 
+00003fd0: 6c69 7374 2061 6e64 2072 6574 7572 6e2e  list and return.
+00003fe0: 0a20 2020 2020 2020 202d 204f 7468 6572  .        - Other
+00003ff0: 7769 7365 2c20 7265 7475 726e 2065 7272  wise, return err
+00004000: 6f72 2077 6974 6820 656d 7074 7920 7374  or with empty st
+00004010: 7269 6e67 2e22 2222 0a0a 2020 2020 2320  ring."""..    # 
+00004020: 4765 7420 7468 6520 636f 6e74 656e 7473  Get the contents
+00004030: 206f 6620 7468 6520 6669 6c65 2e0a 2020   of the file..  
+00004040: 2020 7265 7475 726e 5f63 6f64 652c 2066    return_code, f
+00004050: 696c 655f 636f 6e74 656e 7473 203d 2068  ile_contents = h
+00004060: 7474 705f 7265 7175 6573 7428 6970 5f61  ttp_request(ip_a
+00004070: 6464 7265 7373 2c20 6970 5f70 6f72 742c  ddress, ip_port,
+00004080: 2066 696c 655f 6c6f 6361 7469 6f6e 2c20   file_location, 
+00004090: 226d 6170 6c69 7374 222c 2022 3f78 6d6c  "maplist", "?xml
+000040a0: 2229 0a0a 2020 2020 2320 4966 2067 6f6f  ")..    # If goo
+000040b0: 6420 7265 7475 726e 2063 6f64 652c 2067  d return code, g
+000040c0: 6574 2074 6865 206c 6973 7420 6f66 2058  et the list of X
+000040d0: 4d4c 2066 696c 6520 6c6f 6361 7469 6f6e  ML file location
+000040e0: 7320 696e 746f 2061 206c 6973 7420 616e  s into a list an
+000040f0: 6420 7265 7475 726e 2e0a 2020 2020 6966  d return..    if
+00004100: 2072 6574 7572 6e5f 636f 6465 203d 3d20   return_code == 
+00004110: 303a 0a20 2020 2020 2020 2064 6563 6f64  0:.        decod
+00004120: 6564 5f73 7472 696e 6720 3d20 2866 696c  ed_string = (fil
+00004130: 655f 636f 6e74 656e 7473 2e64 6563 6f64  e_contents.decod
+00004140: 6528 2275 7466 2d38 2229 292e 7370 6c69  e("utf-8")).spli
+00004150: 7428 222c 2229 0a20 2020 2020 2020 2023  t(",").        #
+00004160: 2053 7472 6970 206f 6666 2074 6865 2063   Strip off the c
+00004170: 6f75 6e74 2066 6965 6c64 0a20 2020 2020  ount field.     
+00004180: 2020 2066 6f72 206e 756d 2c20 6974 656d     for num, item
+00004190: 2069 6e20 656e 756d 6572 6174 6528 6465   in enumerate(de
+000041a0: 636f 6465 645f 7374 7269 6e67 293a 0a20  coded_string):. 
+000041b0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+000041c0: 6974 656d 203d 2069 7465 6d5b 3a2d 335d  item = item[:-3]
+000041d0: 2020 2320 4472 6f70 206c 6173 7420 3320    # Drop last 3 
+000041e0: 6368 6172 6163 7465 7273 0a20 2020 2020  characters.     
+000041f0: 2020 2020 2020 2064 6563 6f64 6564 5f73         decoded_s
+00004200: 7472 696e 675b 6e75 6d5d 203d 2074 656d  tring[num] = tem
+00004210: 705f 6974 656d 2e72 6570 6c61 6365 2822  p_item.replace("
+00004220: 2f73 746f 7261 6765 2f65 6d75 6c61 7465  /storage/emulate
+00004230: 642f 3022 2c20 2222 290a 2020 2020 2020  d/0", "").      
+00004240: 2020 2320 5265 6d6f 7665 2069 7465 6d73    # Remove items
+00004250: 2074 6861 7420 6172 6520 696e 2074 6865   that are in the
+00004260: 2074 7261 7368 0a20 2020 2020 2020 2066   trash.        f
+00004270: 696e 616c 5f6c 6973 7420 3d20 5b69 7465  inal_list = [ite
+00004280: 6d20 666f 7220 6974 656d 2069 6e20 6465  m for item in de
+00004290: 636f 6465 645f 7374 7269 6e67 2069 6620  coded_string if 
+000042a0: 222e 5472 6173 6822 206e 6f74 2069 6e20  ".Trash" not in 
+000042b0: 6974 656d 5d0a 2020 2020 2020 2020 7265  item].        re
+000042c0: 7475 726e 2030 2c20 6669 6e61 6c5f 6c69  turn 0, final_li
+000042d0: 7374 0a0a 2020 2020 2320 4f74 6865 7277  st..    # Otherw
+000042e0: 6973 652c 2072 6574 7572 6e20 6572 726f  ise, return erro
+000042f0: 720a 2020 2020 7265 7475 726e 2072 6574  r.    return ret
+00004300: 7572 6e5f 636f 6465 2c20 6669 6c65 5f63  urn_code, file_c
+00004310: 6f6e 7465 6e74 730a 0a0a 2320 5772 6974  ontents...# Writ
+00004320: 6520 6f75 7420 7468 6520 6368 616e 6765  e out the change
+00004330: 6c6f 670a 6465 6620 6372 6561 7465 5f63  log.def create_c
+00004340: 6861 6e67 656c 6f67 2829 202d 3e20 4e6f  hangelog() -> No
+00004350: 6e65 3a0a 2020 2020 2222 2243 7265 6174  ne:.    """Creat
+00004360: 6520 6368 616e 6765 6c6f 6720 6669 6c65  e changelog file
+00004370: 2e22 2222 0a20 2020 2077 6974 6820 6f70  .""".    with op
+00004380: 656e 2843 4841 4e47 454c 4f47 5f46 494c  en(CHANGELOG_FIL
+00004390: 452c 2022 7722 2920 6173 2063 6861 6e67  E, "w") as chang
+000043a0: 656c 6f67 5f66 696c 653a 0a20 2020 2020  elog_file:.     
+000043b0: 2020 2063 6861 6e67 656c 6f67 5f66 696c     changelog_fil
+000043c0: 652e 7772 6974 6528 4348 414e 4745 4c4f  e.write(CHANGELO
+000043d0: 4729 0a0a 0a23 2050 6172 7365 2074 6865  G)...# Parse the
+000043e0: 2063 6861 6e67 656c 6f67 2061 6e64 2064   changelog and d
+000043f0: 756d 7020 6974 2061 7320 6120 6a73 6f6e  ump it as a json
+00004400: 2066 696c 652e 0a64 6566 2073 6176 655f   file..def save_
+00004410: 6368 616e 6765 6c6f 675f 6173 5f6a 736f  changelog_as_jso
+00004420: 6e28 7365 6c66 2920 2d3e 204e 6f6e 653a  n(self) -> None:
+00004430: 2020 2320 6e6f 7161 3a20 414e 4e30 3031    # noqa: ANN001
+00004440: 0a20 2020 2022 2222 0a20 2020 2053 6176  .    """.    Sav
+00004450: 6520 7468 6520 6368 616e 6765 6c6f 6720  e the changelog 
+00004460: 6672 6f6d 2061 206d 6172 6b64 6f77 6e20  from a markdown 
+00004470: 6669 6c65 2074 6f20 6120 4a53 4f4e 2066  file to a JSON f
+00004480: 696c 652e 0a0a 2020 2020 5468 6973 2066  ile...    This f
+00004490: 756e 6374 696f 6e20 7265 6164 7320 7468  unction reads th
+000044a0: 6520 636f 6e74 656e 7473 206f 6620 7468  e contents of th
+000044b0: 6520 2263 6861 6e67 656c 6f67 2e6d 6422  e "changelog.md"
+000044c0: 2066 696c 6520 616e 6420 7061 7273 6573   file and parses
+000044d0: 2069 7420 746f 2063 7265 6174 6520 6120   it to create a 
+000044e0: 6469 6374 696f 6e61 7279 2072 6570 7265  dictionary repre
+000044f0: 7365 6e74 696e 6720 7468 6520 6368 616e  senting the chan
+00004500: 6765 6c6f 672e 2054 6865 2064 6963 7469  gelog. The dicti
+00004510: 6f6e 6172 7920 636f 6e74 6169 6e73 2074  onary contains t
+00004520: 6865 2076 6572 7369 6f6e 206e 756d 6265  he version numbe
+00004530: 7220 6173 2074 6865 206b 6579 2061 6e64  r as the key and
+00004540: 2074 6865 2063 6861 6e67 6573 2061 7320   the changes as 
+00004550: 7468 6520 7661 6c75 652e 2054 6865 2066  the value. The f
+00004560: 756e 6374 696f 6e20 7468 656e 2077 7269  unction then wri
+00004570: 7465 7320 7468 6520 6469 6374 696f 6e61  tes the dictiona
+00004580: 7279 2074 6f20 6120 4a53 4f4e 2066 696c  ry to a JSON fil
+00004590: 6520 6e61 6d65 6420 2263 6861 6e67 656c  e named "changel
+000045a0: 6f67 2e6a 736f 6e22 2e0a 0a20 2020 2050  og.json"...    P
+000045b0: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
+000045c0: 2020 204e 6f6e 650a 0a20 2020 2052 6574     None..    Ret
+000045d0: 7572 6e73 3a0a 2020 2020 2020 2020 4e6f  urns:.        No
+000045e0: 6e65 0a20 2020 2022 2222 0a20 2020 2069  ne.    """.    i
+000045f0: 6620 6f73 2e70 6174 682e 6973 6669 6c65  f os.path.isfile
+00004600: 2822 6368 616e 6765 6c6f 672e 6d64 2229  ("changelog.md")
+00004610: 3a0a 2020 2020 2020 2020 6368 616e 6765  :.        change
+00004620: 6c6f 675f 6469 6374 203d 207b 7d0a 2020  log_dict = {}.  
+00004630: 2020 2020 2020 6861 7665 5f66 6972 7374        have_first
+00004640: 5f62 7261 636b 6574 203d 2046 616c 7365  _bracket = False
+00004650: 0a20 2020 2020 2020 2063 6861 6e67 655f  .        change_
+00004660: 636f 756e 7420 3d20 300a 2020 2020 2020  count = 0.      
+00004670: 2020 7769 7468 206f 7065 6e28 2263 6861    with open("cha
+00004680: 6e67 656c 6f67 2e6d 6422 2920 6173 2063  ngelog.md") as c
+00004690: 6861 6e67 656c 6f67 3a0a 2020 2020 2020  hangelog:.      
+000046a0: 2020 2020 2020 6c69 6e65 7320 3d20 6368        lines = ch
+000046b0: 616e 6765 6c6f 672e 7265 6164 6c69 6e65  angelog.readline
+000046c0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000046d0: 666f 7220 6c69 6e65 2069 6e20 6c69 6e65  for line in line
+000046e0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000046f0: 2020 2069 6620 225b 2220 696e 206c 696e     if "[" in lin
+00004700: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00004710: 2020 2020 2020 2069 6620 6861 7665 5f66         if have_f
+00004720: 6972 7374 5f62 7261 636b 6574 3a20 2023  irst_bracket:  #
+00004730: 2049 6620 7765 2061 6c72 6561 6479 2068   If we already h
+00004740: 6176 6520 7468 6520 6272 6163 6b65 7420  ave the bracket 
+00004750: 616e 6420 656e 636f 756e 7465 7220 616e  and encounter an
+00004760: 6f74 6865 722c 2073 746f 7020 7265 6164  other, stop read
+00004770: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00004780: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00004790: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
+000047a0: 2020 2020 2020 6861 7665 5f66 6972 7374        have_first
+000047b0: 5f62 7261 636b 6574 203d 2054 7275 650a  _bracket = True.
+000047c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047d0: 2020 2020 6272 6163 6b65 745f 7374 6172      bracket_star
+000047e0: 745f 706f 7320 3d20 6c69 6e65 2e66 696e  t_pos = line.fin
+000047f0: 6428 225b 2229 0a20 2020 2020 2020 2020  d("[").         
+00004800: 2020 2020 2020 2020 2020 2062 7261 636b             brack
+00004810: 6574 5f65 6e64 5f70 6f73 203d 206c 696e  et_end_pos = lin
+00004820: 652e 6669 6e64 2822 5d22 290a 2020 2020  e.find("]").    
+00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004840: 6368 616e 6765 6c6f 675f 6469 6374 5b22  changelog_dict["
+00004850: 7665 7273 696f 6e22 5d20 3d20 6c69 6e65  version"] = line
+00004860: 5b62 7261 636b 6574 5f73 7461 7274 5f70  [bracket_start_p
+00004870: 6f73 202b 2031 203a 2062 7261 636b 6574  os + 1 : bracket
+00004880: 5f65 6e64 5f70 6f73 5d0a 2020 2020 2020  _end_pos].      
+00004890: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
+000048a0: 696e 6520 213d 2022 5c6e 2220 616e 6420  ine != "\n" and 
+000048b0: 6861 7665 5f66 6972 7374 5f62 7261 636b  have_first_brack
+000048c0: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
+000048d0: 2020 2020 2020 2020 6368 616e 6765 6c6f          changelo
+000048e0: 675f 6469 6374 5b66 2263 6861 6e67 657b  g_dict[f"change{
+000048f0: 6368 616e 6765 5f63 6f75 6e74 2173 7d22  change_count!s}"
+00004900: 5d20 3d20 6c69 6e65 0a20 2020 2020 2020  ] = line.       
+00004910: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00004920: 6e67 655f 636f 756e 7420 2b3d 2031 0a20  nge_count += 1. 
+00004930: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+00004940: 2843 4841 4e47 454c 4f47 5f4a 534f 4e5f  (CHANGELOG_JSON_
+00004950: 4649 4c45 2c20 2277 2229 2061 7320 6368  FILE, "w") as ch
+00004960: 616e 6765 6c6f 675f 6669 6c65 3a0a 2020  angelog_file:.  
+00004970: 2020 2020 2020 2020 2020 6a73 6f6e 2e64            json.d
+00004980: 756d 7028 6368 616e 6765 6c6f 675f 6469  ump(changelog_di
+00004990: 6374 2c20 6368 616e 6765 6c6f 675f 6669  ct, changelog_fi
+000049a0: 6c65 290a 0a20 2020 2020 2020 2073 656c  le)..        sel
+000049b0: 662e 6469 7370 6c61 795f 6d65 7373 6167  f.display_messag
+000049c0: 655f 626f 7828 6622 7b43 4841 4e47 454c  e_box(f"{CHANGEL
+000049d0: 4f47 5f4a 534f 4e5f 4649 4c45 7d20 6669  OG_JSON_FILE} fi
+000049e0: 6c65 2073 6176 6564 2e22 2c20 2254 7572  le saved.", "Tur
+000049f0: 7175 6f69 7365 2229 0a0a 0a23 2052 6561  quoise")...# Rea
+00004a00: 6420 7468 6520 6368 616e 6765 206c 6f67  d the change log
+00004a10: 2066 696c 652c 2061 6464 2069 7420 746f   file, add it to
+00004a20: 2074 6865 206d 6573 7361 6765 7320 746f   the messages to
+00004a30: 2062 6520 6469 7370 6c61 7965 6420 616e   be displayed an
+00004a40: 6420 7468 656e 2072 656d 6f76 6520 6974  d then remove it
+00004a50: 2e0a 6465 6620 6368 6563 6b5f 666f 725f  ..def check_for_
+00004a60: 6368 616e 6765 6c6f 6728 7365 6c66 2920  changelog(self) 
+00004a70: 2d3e 204e 6f6e 653a 2020 2320 6e6f 7161  -> None:  # noqa
+00004a80: 3a20 414e 4e30 3031 0a20 2020 2022 2222  : ANN001.    """
+00004a90: 4675 6e63 7469 6f6e 2074 6f20 6368 6563  Function to chec
+00004aa0: 6b20 666f 7220 6120 6368 616e 6765 6c6f  k for a changelo
+00004ab0: 6720 6669 6c65 2061 6e64 2061 6464 2069  g file and add i
+00004ac0: 7473 2063 6f6e 7465 6e74 7320 746f 2061  ts contents to a
+00004ad0: 206d 6573 7361 6765 2069 6620 7468 6520   message if the 
+00004ae0: 6375 7272 656e 7420 7665 7273 696f 6e20  current version 
+00004af0: 6973 2063 6f72 7265 6374 2e0a 2020 2020  is correct..    
+00004b00: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
+00004b10: 2020 2020 2d20 7365 6c66 2028 6f62 6a65      - self (obje
+00004b20: 6374 293a 2054 6865 206f 626a 6563 7420  ct): The object 
+00004b30: 7468 6174 2074 6865 2066 756e 6374 696f  that the functio
+00004b40: 6e20 6973 2062 6569 6e67 2063 616c 6c65  n is being calle
+00004b50: 6420 6f6e 2e0a 2020 2020 5265 7475 726e  d on..    Return
+00004b60: 733a 0a20 2020 2020 2020 202d 204e 6f6e  s:.        - Non
+00004b70: 653a 2054 6865 2066 756e 6374 696f 6e20  e: The function 
+00004b80: 646f 6573 206e 6f74 2072 6574 7572 6e20  does not return 
+00004b90: 616e 7974 6869 6e67 2c20 6275 7420 7570  anything, but up
+00004ba0: 6461 7465 7320 7468 6520 6d65 7373 6167  dates the messag
+00004bb0: 6520 6174 7472 6962 7574 6520 6f66 2074  e attribute of t
+00004bc0: 6865 206f 626a 6563 742e 0a20 2020 2050  he object..    P
+00004bd0: 726f 6365 7373 696e 6720 4c6f 6769 633a  rocessing Logic:
+00004be0: 0a20 2020 2020 2020 202d 2043 6865 636b  .        - Check
+00004bf0: 2069 6620 7468 6520 6368 616e 6765 6c6f   if the changelo
+00004c00: 6720 6669 6c65 2065 7869 7374 732e 0a20  g file exists.. 
+00004c10: 2020 2020 2020 202d 2049 6620 6974 2065         - If it e
+00004c20: 7869 7374 732c 2070 7265 7061 7265 2074  xists, prepare t
+00004c30: 6f20 6469 7370 6c61 7920 6368 616e 6765  o display change
+00004c40: 7320 616e 6420 7265 6d6f 7665 2074 6865  s and remove the
+00004c50: 2066 696c 6520 736f 2077 6520 6f6e 6c79   file so we only
+00004c60: 2064 6973 706c 6179 2074 6865 2063 6861   display the cha
+00004c70: 6e67 6573 206f 6e63 652e 2222 220a 2020  nges once.""".  
+00004c80: 2020 2320 544f 444f 2054 6573 7420 6368    # TODO Test ch
+00004c90: 616e 6765 6c6f 6720 6265 666f 7265 2070  angelog before p
+00004ca0: 6f73 7469 6e67 2074 6f20 5079 5069 2e20  osting to PyPi. 
+00004cb0: 2043 6f6d 6d65 6e74 2069 7420 6f75 7420   Comment it out 
+00004cc0: 6166 7465 7220 7465 7374 696e 672e 0a20  after testing.. 
+00004cd0: 2020 2023 7365 6c66 2e6d 6573 7361 6765     #self.message
+00004ce0: 203d 2043 4841 4e47 454c 4f47 0a0a 2020   = CHANGELOG..  
+00004cf0: 2020 6966 206f 732e 7061 7468 2e69 7366    if os.path.isf
+00004d00: 696c 6528 4348 414e 4745 4c4f 475f 4649  ile(CHANGELOG_FI
+00004d10: 4c45 293a 0a20 2020 2020 2020 2073 656c  LE):.        sel
+00004d20: 662e 6d65 7373 6167 6520 3d20 4348 414e  f.message = CHAN
+00004d30: 4745 4c4f 470a 2020 2020 2020 2020 6f73  GELOG.        os
+00004d40: 2e72 656d 6f76 6528 4348 414e 4745 4c4f  .remove(CHANGELO
+00004d50: 475f 4649 4c45 290a 0a20 2020 2023 2057  G_FILE)..    # W
+00004d60: 7269 7465 2063 6861 6e67 656c 6f67 206f  rite changelog o
+00004d70: 7574 2061 7320 6a73 6f6e 2066 696c 6520  ut as json file 
+00004d80: 6966 2069 6e20 6465 6275 6720 6d6f 6465  if in debug mode
+00004d90: 2e0a 2020 2020 2320 544f 444f 2053 6574  ..    # TODO Set
+00004da0: 2064 6562 7567 206f 6e20 616e 6420 7265   debug on and re
+00004db0: 7275 6e20 746f 2063 7265 6174 6520 7468  run to create th
+00004dc0: 6520 6368 616e 6765 6c6f 672e 6a73 6f6e  e changelog.json
+00004dd0: 2066 696c 650a 2020 2020 6966 2073 656c   file.    if sel
+00004de0: 662e 6465 6275 673a 0a20 2020 2020 2020  f.debug:.       
+00004df0: 2073 6176 655f 6368 616e 6765 6c6f 675f   save_changelog_
+00004e00: 6173 5f6a 736f 6e28 7365 6c66 290a 0a0a  as_json(self)...
+00004e10: 2320 496e 6974 6961 6c69 7a65 2074 6865  # Initialize the
+00004e20: 2047 5549 2028 5f69 6e69 745f 206d 6574   GUI (_init_ met
+00004e30: 686f 6429 0a64 6566 2069 6e69 7469 616c  hod).def initial
+00004e40: 697a 655f 6775 6928 7365 6c66 2920 2d3e  ize_gui(self) ->
+00004e50: 204e 6f6e 653a 2020 2320 6e6f 7161 3a20   None:  # noqa: 
+00004e60: 414e 4e30 3031 0a20 2020 2022 2222 496e  ANN001.    """In
+00004e70: 6974 6961 6c69 7a65 7320 7468 6520 4755  itializes the GU
+00004e80: 4920 6279 2069 6e69 7469 616c 697a 696e  I by initializin
+00004e90: 6720 7661 7269 6162 6c65 7320 616e 6420  g variables and 
+00004ea0: 6164 6469 6e67 2061 206c 6f67 6f2e 0a20  adding a logo.. 
+00004eb0: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
+00004ec0: 2020 2020 2020 202d 2073 656c 6620 2863         - self (c
+00004ed0: 6c61 7373 293a 2054 6865 2063 6c61 7373  lass): The class
+00004ee0: 206f 626a 6563 742e 0a20 2020 2052 6574   object..    Ret
+00004ef0: 7572 6e73 3a0a 2020 2020 2020 2020 2d20  urns:.        - 
+00004f00: 4e6f 6e65 3a20 446f 6573 206e 6f74 2072  None: Does not r
+00004f10: 6574 7572 6e20 616e 7974 6869 6e67 2e0a  eturn anything..
+00004f20: 2020 2020 5072 6f63 6573 7369 6e67 204c      Processing L
+00004f30: 6f67 6963 3a0a 2020 2020 2020 2020 2d20  ogic:.        - 
+00004f40: 4361 6c6c 7320 696e 6974 6961 6c69 7a65  Calls initialize
+00004f50: 5f76 6172 6961 626c 6573 2066 756e 6374  _variables funct
+00004f60: 696f 6e2e 0a20 2020 2020 2020 202d 2043  ion..        - C
+00004f70: 616c 6c73 2061 6464 5f6c 6f67 6f20 6675  alls add_logo fu
+00004f80: 6e63 7469 6f6e 2e22 2222 0a20 2020 2069  nction.""".    i
+00004f90: 6e69 7469 616c 697a 655f 7661 7269 6162  nitialize_variab
+00004fa0: 6c65 7328 7365 6c66 290a 2020 2020 6164  les(self).    ad
+00004fb0: 645f 6c6f 676f 2873 656c 6629 0a0a 0a23  d_logo(self)...#
+00004fc0: 2049 6e69 7469 616c 697a 6520 7468 6520   Initialize the 
+00004fd0: 4755 4920 7661 726c 6961 626c 6573 2028  GUI varliables (
+00004fe0: 652e 2e67 205f 696e 6974 5f20 6d65 7468  e..g _init_ meth
+00004ff0: 6f64 290a 6465 6620 696e 6974 6961 6c69  od).def initiali
+00005000: 7a65 5f76 6172 6961 626c 6573 2873 656c  ze_variables(sel
+00005010: 6629 202d 3e20 4e6f 6e65 3a20 2023 206e  f) -> None:  # n
+00005020: 6f71 613a 2041 4e4e 3030 310a 2020 2020  oqa: ANN001.    
+00005030: 2222 220a 2020 2020 496e 6974 6961 6c69  """.    Initiali
+00005040: 7a65 2076 6172 6961 626c 6573 2066 6f72  ze variables for
+00005050: 2074 6865 204d 6170 5461 736b 6572 2052   the MapTasker R
+00005060: 756e 7469 6d65 204f 7074 696f 6e73 2077  untime Options w
+00005070: 696e 646f 772e 0a20 2020 2022 2222 0a20  indow..    """. 
+00005080: 2020 2073 656c 662e 616e 6472 6f69 645f     self.android_
+00005090: 6970 6164 6472 203d 2022 220a 2020 2020  ipaddr = "".    
+000050a0: 7365 6c66 2e61 6e64 726f 6964 5f70 6f72  self.android_por
+000050b0: 7420 3d20 2222 0a20 2020 2073 656c 662e  t = "".    self.
+000050c0: 616e 6472 6f69 645f 6669 6c65 203d 2022  android_file = "
+000050d0: 220a 2020 2020 7365 6c66 2e61 7070 6561  ".    self.appea
+000050e0: 7261 6e63 655f 6d6f 6465 203d 204e 6f6e  rance_mode = Non
+000050f0: 650a 2020 2020 7365 6c66 2e62 6f6c 6420  e.    self.bold 
+00005100: 3d20 4e6f 6e65 0a20 2020 2073 656c 662e  = None.    self.
+00005110: 636f 6c6f 725f 6c61 6265 6c73 203d 204e  color_labels = N
+00005120: 6f6e 650a 2020 2020 7365 6c66 2e63 6f6c  one.    self.col
+00005130: 6f72 5f6c 6f6f 6b75 7020 3d20 4e6f 6e65  or_lookup = None
+00005140: 0a20 2020 2073 656c 662e 636f 6c6f 725f  .    self.color_
+00005150: 7465 7874 5f72 6f77 203d 204e 6f6e 650a  text_row = None.
+00005160: 2020 2020 7365 6c66 2e64 6562 7567 203d      self.debug =
+00005170: 204e 6f6e 650a 2020 2020 7365 6c66 2e64   None.    self.d
+00005180: 6973 706c 6179 5f64 6574 6169 6c5f 6c65  isplay_detail_le
+00005190: 7665 6c20 3d20 4e6f 6e65 0a20 2020 2073  vel = None.    s
+000051a0: 656c 662e 7072 6566 6572 656e 6365 7320  elf.preferences 
+000051b0: 3d20 4e6f 6e65 0a20 2020 2073 656c 662e  = None.    self.
+000051c0: 636f 6e64 6974 696f 6e73 203d 204e 6f6e  conditions = Non
+000051d0: 650a 2020 2020 7365 6c66 2e65 7665 7279  e.    self.every
+000051e0: 7468 696e 6720 3d20 4e6f 6e65 0a20 2020  thing = None.   
+000051f0: 2073 656c 662e 7461 736b 6572 6e65 7420   self.taskernet 
+00005200: 3d20 4e6f 6e65 0a20 2020 2073 656c 662e  = None.    self.
+00005210: 6578 6974 203d 204e 6f6e 650a 2020 2020  exit = None.    
+00005220: 7365 6c66 2e66 6574 6368 6564 5f62 6163  self.fetched_bac
+00005230: 6b75 705f 6672 6f6d 5f61 6e64 726f 6964  kup_from_android
+00005240: 203d 2046 616c 7365 0a20 2020 2073 656c   = False.    sel
+00005250: 662e 6669 6c65 203d 204e 6f6e 650a 2020  f.file = None.  
+00005260: 2020 7365 6c66 2e66 6f6e 7420 3d20 4e6f    self.font = No
+00005270: 6e65 0a20 2020 2073 656c 662e 676f 5f70  ne.    self.go_p
+00005280: 726f 6772 616d 203d 204e 6f6e 650a 2020  rogram = None.  
+00005290: 2020 7365 6c66 2e67 7569 203d 2054 7275    self.gui = Tru
+000052a0: 650a 2020 2020 7365 6c66 2e68 6967 686c  e.    self.highl
+000052b0: 6967 6874 203d 204e 6f6e 650a 2020 2020  ight = None.    
+000052c0: 7365 6c66 2e69 6e64 656e 7420 3d20 4e6f  self.indent = No
+000052d0: 6e65 0a20 2020 2073 656c 662e 6974 616c  ne.    self.ital
+000052e0: 6963 697a 6520 3d20 4e6f 6e65 0a20 2020  icize = None.   
+000052f0: 2073 656c 662e 6e61 6d65 645f 6974 656d   self.named_item
+00005300: 203d 204e 6f6e 650a 2020 2020 7365 6c66   = None.    self
+00005310: 2e72 6572 756e 203d 204e 6f6e 650a 2020  .rerun = None.  
+00005320: 2020 7365 6c66 2e72 6573 6574 203d 204e    self.reset = N
+00005330: 6f6e 650a 2020 2020 7365 6c66 2e72 6573  one.    self.res
+00005340: 746f 7265 203d 2046 616c 7365 0a20 2020  tore = False.   
+00005350: 2073 656c 662e 7275 6e74 696d 6520 3d20   self.runtime = 
+00005360: 4661 6c73 650a 2020 2020 7365 6c66 2e73  False.    self.s
+00005370: 6176 6520 3d20 4661 6c73 650a 2020 2020  ave = False.    
+00005380: 7365 6c66 2e73 696e 676c 655f 7072 6f66  self.single_prof
+00005390: 696c 655f 6e61 6d65 203d 204e 6f6e 650a  ile_name = None.
+000053a0: 2020 2020 7365 6c66 2e73 696e 676c 655f      self.single_
+000053b0: 7072 6f6a 6563 745f 6e61 6d65 203d 204e  project_name = N
+000053c0: 6f6e 650a 2020 2020 7365 6c66 2e73 696e  one.    self.sin
+000053d0: 676c 655f 7461 736b 5f6e 616d 6520 3d20  gle_task_name = 
+000053e0: 4e6f 6e65 0a20 2020 2073 656c 662e 7477  None.    self.tw
+000053f0: 6973 7479 203d 204e 6f6e 650a 2020 2020  isty = None.    
+00005400: 7365 6c66 2e75 6e64 6572 6c69 6e65 203d  self.underline =
+00005410: 204e 6f6e 650a 2020 2020 7365 6c66 2e6f   None.    self.o
+00005420: 7574 6c69 6e65 203d 2046 616c 7365 0a20  utline = False. 
+00005430: 2020 2073 656c 662e 7072 6574 7479 203d     self.pretty =
+00005440: 2046 616c 7365 0a20 2020 2073 656c 662e   False.    self.
+00005450: 746f 706c 6576 656c 5f77 696e 646f 7720  toplevel_window 
+00005460: 3d20 4e6f 6e65 0a20 2020 2050 7269 6d65  = None.    Prime
+00005470: 4974 656d 732e 7072 6f67 7261 6d5f 6172  Items.program_ar
+00005480: 6775 6d65 6e74 735b 2267 7569 225d 203d  guments["gui"] =
+00005490: 2054 7275 650a 2020 2020 7365 6c66 2e6c   True.    self.l
+000054a0: 6973 745f 6669 6c65 7320 3d20 4661 6c73  ist_files = Fals
+000054b0: 650a 2020 2020 7365 6c66 2e61 695f 6170  e.    self.ai_ap
+000054c0: 696b 6579 203d 204e 6f6e 650a 2020 2020  ikey = None.    
+000054d0: 7365 6c66 2e61 695f 6d6f 6465 6c20 3d20  self.ai_model = 
+000054e0: 4e6f 6e65 0a20 2020 2073 656c 662e 6169  None.    self.ai
+000054f0: 5f61 6e61 6c79 7369 7320 3d20 4e6f 6e65  _analysis = None
+00005500: 0a20 2020 2073 656c 662e 6169 5f6d 6973  .    self.ai_mis
+00005510: 7369 6e67 5f6d 6f64 756c 6520 3d20 4e6f  sing_module = No
+00005520: 6e65 0a20 2020 2073 656c 662e 6169 5f70  ne.    self.ai_p
+00005530: 726f 6d70 7420 3d20 4e6f 6e65 0a20 2020  rompt = None.   
+00005540: 2073 656c 662e 7769 6e64 6f77 5f70 6f73   self.window_pos
+00005550: 6974 696f 6e20 3d20 4e6f 6e65 0a20 2020  ition = None.   
+00005560: 2073 656c 662e 6169 5f70 6f70 7570 5f77   self.ai_popup_w
+00005570: 696e 646f 775f 706f 7369 7469 6f6e 203d  indow_position =
+00005580: 204e 6f6e 650a 2020 2020 7365 6c66 2e61   None.    self.a
+00005590: 6c6c 5f6d 6573 7361 6765 7320 3d20 7b7d  ll_messages = {}
+000055a0: 0a0a 2020 2020 7365 6c66 2e74 6974 6c65  ..    self.title
+000055b0: 2822 4d61 7054 6173 6b65 7220 5275 6e74  ("MapTasker Runt
+000055c0: 696d 6520 4f70 7469 6f6e 7322 290a 0a20  ime Options").. 
+000055d0: 2020 2023 2047 6574 2074 6865 2073 6372     # Get the scr
+000055e0: 6565 6e20 7369 7a65 0a20 2020 2073 6372  een size.    scr
+000055f0: 6565 6e5f 7769 6474 6820 3d20 7365 6c66  een_width = self
+00005600: 2e77 696e 666f 5f73 6372 6565 6e77 6964  .winfo_screenwid
+00005610: 7468 2829 0a20 2020 2073 6372 6565 6e5f  th().    screen_
+00005620: 6865 6967 6874 203d 2073 656c 662e 7769  height = self.wi
+00005630: 6e66 6f5f 7363 7265 656e 6865 6967 6874  nfo_screenheight
+00005640: 2829 0a0a 2020 2020 2320 4f76 6572 616c  ()..    # Overal
+00005650: 6c20 7769 6e64 6f77 2064 696d 656e 7369  l window dimensi
+00005660: 6f6e 730a 2020 2020 7365 6c66 2e67 656f  ons.    self.geo
+00005670: 6d65 7472 7928 6622 3131 3030 7839 3030  metry(f"1100x900
+00005680: 2b7b 7363 7265 656e 5f77 6964 7468 2f2f  +{screen_width//
+00005690: 347d 2b7b 7363 7265 656e 5f68 6569 6768  4}+{screen_heigh
+000056a0: 742f 2f36 7d22 290a 0a20 2020 2023 2063  t//6}")..    # c
+000056b0: 6f6e 6669 6775 7265 2067 7269 6420 6c61  onfigure grid la
+000056c0: 796f 7574 2028 3478 3429 2e20 2041 206e  yout (4x4).  A n
+000056d0: 6f6e 2d7a 6572 6f20 7765 6967 6874 2063  on-zero weight c
+000056e0: 6175 7365 7320 6120 726f 7720 6f72 2063  auses a row or c
+000056f0: 6f6c 756d 6e20 746f 2067 726f 7720 6966  olumn to grow if
+00005700: 2074 6865 7265 2773 2065 7874 7261 2073   there's extra s
+00005710: 7061 6365 206e 6565 6465 642e 0a20 2020  pace needed..   
+00005720: 2023 2054 6865 2064 6566 6175 6c74 2069   # The default i
+00005730: 7320 6120 7765 6967 6874 206f 6620 7a65  s a weight of ze
+00005740: 726f 2c20 7768 6963 6820 6d65 616e 7320  ro, which means 
+00005750: 7468 6520 636f 6c75 6d6e 2077 696c 6c20  the column will 
+00005760: 6e6f 7420 6772 6f77 2069 6620 7468 6572  not grow if ther
+00005770: 6527 7320 6578 7472 6120 7370 6163 652e  e's extra space.
+00005780: 0a20 2020 2073 656c 662e 6772 6964 5f63  .    self.grid_c
+00005790: 6f6c 756d 6e63 6f6e 6669 6775 7265 2831  olumnconfigure(1
+000057a0: 2c20 7765 6967 6874 3d31 290a 2020 2020  , weight=1).    
+000057b0: 7365 6c66 2e67 7269 645f 636f 6c75 6d6e  self.grid_column
+000057c0: 636f 6e66 6967 7572 6528 2832 2c20 3329  configure((2, 3)
+000057d0: 2c20 7765 6967 6874 3d30 290a 2020 2020  , weight=0).    
+000057e0: 7365 6c66 2e67 7269 645f 726f 7763 6f6e  self.grid_rowcon
+000057f0: 6669 6775 7265 2828 302c 2033 292c 2077  figure((0, 3), w
+00005800: 6569 6768 743d 3429 2020 2320 4469 7676  eight=4)  # Divv
+00005810: 7920 7570 2074 6865 2065 7874 7261 2073  y up the extra s
+00005820: 7061 6365 206e 6565 6465 6420 6571 7561  pace needed equa
+00005830: 6c6c 7920 616d 6f6e 7374 2074 6865 2034  lly amonst the 4
+00005840: 2072 6f77 732e 0a0a 2020 2020 2320 6c6f   rows...    # lo
+00005850: 6164 2061 6e64 2063 7265 6174 6520 6261  ad and create ba
+00005860: 636b 6772 6f75 6e64 2069 6d61 6765 0a0a  ckground image..
+00005870: 2020 2020 2320 6372 6561 7465 2073 6964      # create sid
+00005880: 6562 6172 2066 7261 6d65 2077 6974 6820  ebar frame with 
+00005890: 7769 6467 6574 7320 6f6e 2074 6865 206c  widgets on the l
+000058a0: 6566 7420 7369 6465 206f 6620 7468 6520  eft side of the 
+000058b0: 7769 6e64 6f77 2e0a 2020 2020 7365 6c66  window..    self
+000058c0: 2e73 6964 6562 6172 5f66 7261 6d65 203d  .sidebar_frame =
+000058d0: 2063 746b 2e43 546b 4672 616d 6528 7365   ctk.CTkFrame(se
+000058e0: 6c66 2c20 7769 6474 683d 3134 302c 2063  lf, width=140, c
+000058f0: 6f72 6e65 725f 7261 6469 7573 3d30 290a  orner_radius=0).
+00005900: 2020 2020 7365 6c66 2e73 6964 6562 6172      self.sidebar
+00005910: 5f66 7261 6d65 2e63 6f6e 6669 6775 7265  _frame.configure
+00005920: 2862 675f 636f 6c6f 723d 2262 6c61 636b  (bg_color="black
+00005930: 2229 0a20 2020 2073 656c 662e 7369 6465  ").    self.side
+00005940: 6261 725f 6672 616d 652e 6772 6964 2872  bar_frame.grid(r
+00005950: 6f77 3d30 2c20 636f 6c75 6d6e 3d30 2c20  ow=0, column=0, 
+00005960: 726f 7773 7061 6e3d 3137 2c20 7374 6963  rowspan=17, stic
+00005970: 6b79 3d22 6e73 6577 2229 0a20 2020 2023  ky="nsew").    #
+00005980: 2044 6566 696e 6520 7369 6465 6261 7220   Define sidebar 
+00005990: 6261 636b 6772 6f75 6e64 2066 7261 6d65  background frame
+000059a0: 2077 6974 6820 3137 2072 6f77 730a 2020   with 17 rows.  
+000059b0: 2020 7365 6c66 2e73 6964 6562 6172 5f66    self.sidebar_f
+000059c0: 7261 6d65 2e67 7269 645f 726f 7763 6f6e  rame.grid_rowcon
+000059d0: 6669 6775 7265 2831 372c 2077 6569 6768  figure(17, weigh
+000059e0: 743d 3129 0a0a 0a23 2041 6464 2074 6865  t=1)...# Add the
+000059f0: 204d 6170 5461 736b 6572 2069 636f 6e20   MapTasker icon 
+00005a00: 746f 2074 6865 2073 6372 6565 6e0a 6465  to the screen.de
+00005a10: 6620 6164 645f 6c6f 676f 2873 656c 6629  f add_logo(self)
+00005a20: 202d 3e20 4e6f 6e65 3a20 2023 206e 6f71   -> None:  # noq
+00005a30: 613a 2041 4e4e 3030 310a 2020 2020 2222  a: ANN001.    ""
+00005a40: 2246 756e 6374 696f 6e3a 0a20 2020 2020  "Function:.     
+00005a50: 2020 2061 6464 5f6c 6f67 6f0a 2020 2020     add_logo.    
+00005a60: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
+00005a70: 2020 2020 2d20 7365 6c66 2028 6f62 6a65      - self (obje
+00005a80: 6374 293a 2054 6865 206f 626a 6563 7420  ct): The object 
+00005a90: 7468 6174 2074 6865 2066 756e 6374 696f  that the functio
+00005aa0: 6e20 6973 2062 6569 6e67 2063 616c 6c65  n is being calle
+00005ab0: 6420 6f6e 2e0a 2020 2020 5265 7475 726e  d on..    Return
+00005ac0: 733a 0a20 2020 2020 2020 202d 204e 6f6e  s:.        - Non
+00005ad0: 653a 2054 6865 2066 756e 6374 696f 6e20  e: The function 
+00005ae0: 646f 6573 206e 6f74 2072 6574 7572 6e20  does not return 
+00005af0: 616e 7974 6869 6e67 2e0a 2020 2020 5072  anything..    Pr
+00005b00: 6f63 6573 7369 6e67 204c 6f67 6963 3a0a  ocessing Logic:.
+00005b10: 2020 2020 2020 2020 2d20 4765 7420 7468          - Get th
+00005b20: 6520 7061 7468 2074 6f20 6f75 7220 6c6f  e path to our lo
+00005b30: 676f 732e 0a20 2020 2020 2020 202d 2053  gos..        - S
+00005b40: 7769 7463 6820 746f 206f 7572 2074 656d  witch to our tem
+00005b50: 7020 6469 7265 6374 6f72 7920 2861 7373  p directory (ass
+00005b60: 6574 7329 2e0a 2020 2020 2020 2020 2d20  ets)..        - 
+00005b70: 4372 6561 7465 2061 2043 546b 496d 6167  Create a CTkImag
+00005b80: 6520 6f62 6a65 6374 2074 6f20 6469 7370  e object to disp
+00005b90: 6c61 7920 7468 6520 6c6f 676f 2e0a 2020  lay the logo..  
+00005ba0: 2020 2020 2020 2d20 5472 7920 746f 2064        - Try to d
+00005bb0: 6973 706c 6179 2074 6865 206c 6f67 6f20  isplay the logo 
+00005bc0: 7769 7468 2061 2043 546b 4c61 6265 6c2e  with a CTkLabel.
+00005bd0: 0a20 2020 2020 2020 202d 2053 7769 7463  .        - Switc
+00005be0: 6820 6261 636b 2074 6f20 7072 6f70 6572  h back to proper
+00005bf0: 2064 6972 6563 746f 7279 2e22 2222 0a20   directory.""". 
+00005c00: 2020 2023 2041 6464 206f 7572 206c 6f67     # Add our log
+00005c10: 6f0a 2020 2020 2320 4765 7420 7468 6520  o.    # Get the 
+00005c20: 7061 7468 2074 6f20 6f75 7220 6c6f 676f  path to our logo
+00005c30: 733a 0a20 2020 2023 2063 7572 7265 6e74  s:.    # current
+00005c40: 5f64 6972 203d 2064 6972 6563 746f 7279  _dir = directory
+00005c50: 2066 726f 6d20 7768 6963 6820 7765 2061   from which we a
+00005c60: 7265 2072 756e 6e69 6e67 2e0a 2020 2020  re running..    
+00005c70: 2320 6162 7370 6174 6820 3d20 7061 7468  # abspath = path
+00005c80: 206f 6620 7468 6973 2073 6f75 7263 6520   of this source 
+00005c90: 636f 6465 2028 7573 6572 696e 7472 2e70  code (userintr.p
+00005ca0: 7929 2e0a 2020 2020 2320 6377 6420 3d20  y)..    # cwd = 
+00005cb0: 6469 7265 6374 6f72 7920 6672 6f6d 2077  directory from w
+00005cc0: 6869 6368 2074 6865 206d 6169 6e20 7072  hich the main pr
+00005cd0: 6f67 7261 6d20 6973 2028 6d61 696e 2e70  ogram is (main.p
+00005ce0: 7929 0a20 2020 2023 2064 6e61 6d65 203d  y).    # dname =
+00005cf0: 2064 6972 6563 746f 7279 206f 6620 7372   directory of sr
+00005d00: 630a 2020 2020 6375 7272 656e 745f 6469  c.    current_di
+00005d10: 7220 3d20 6f73 2e67 6574 6377 6428 290a  r = os.getcwd().
+00005d20: 2020 2020 6162 7370 6174 6820 3d20 6f73      abspath = os
+00005d30: 2e70 6174 682e 6162 7370 6174 6828 5f5f  .path.abspath(__
+00005d40: 6669 6c65 5f5f 290a 2020 2020 2320 6377  file__).    # cw
+00005d50: 6420 3d20 6f73 2e70 6174 682e 6162 7370  d = os.path.absp
+00005d60: 6174 6828 6f73 2e70 6174 682e 6469 726e  ath(os.path.dirn
+00005d70: 616d 6528 7379 732e 6172 6776 5b30 5d29  ame(sys.argv[0])
+00005d80: 290a 2020 2020 646e 616d 6520 3d20 6f73  ).    dname = os
+00005d90: 2e70 6174 682e 6469 726e 616d 6528 6162  .path.dirname(ab
+00005da0: 7370 6174 6829 0a20 2020 2074 656d 705f  spath).    temp_
+00005db0: 6469 7220 3d20 646e 616d 652e 7265 706c  dir = dname.repl
+00005dc0: 6163 6528 2273 7263 222c 2022 6173 7365  ace("src", "asse
+00005dd0: 7473 2229 0a20 2020 2023 2053 7769 7463  ts").    # Switc
+00005de0: 6820 746f 206f 7572 2074 656d 7020 6469  h to our temp di
+00005df0: 7265 6374 6f72 7920 2861 7373 6574 7329  rectory (assets)
+00005e00: 0a20 2020 206f 732e 6368 6469 7228 7465  .    os.chdir(te
+00005e10: 6d70 5f64 6972 290a 0a20 2020 2023 2043  mp_dir)..    # C
+00005e20: 7265 6174 6520 6120 4354 6b49 6d61 6765  reate a CTkImage
+00005e30: 206f 626a 6563 7420 746f 2064 6973 706c   object to displ
+00005e40: 6179 2074 6865 206c 6f67 6f0a 2020 2020  ay the logo.    
+00005e50: 6d79 5f69 6d61 6765 203d 2063 746b 2e43  my_image = ctk.C
+00005e60: 546b 496d 6167 6528 0a20 2020 2020 2020  TkImage(.       
+00005e70: 206c 6967 6874 5f69 6d61 6765 3d49 6d61   light_image=Ima
+00005e80: 6765 2e6f 7065 6e28 226d 6170 7461 736b  ge.open("maptask
+00005e90: 6572 5f6c 6f67 6f5f 6c69 6768 742e 706e  er_logo_light.pn
+00005ea0: 6722 292c 0a20 2020 2020 2020 2064 6172  g"),.        dar
+00005eb0: 6b5f 696d 6167 653d 496d 6167 652e 6f70  k_image=Image.op
+00005ec0: 656e 2822 6d61 7074 6173 6b65 725f 6c6f  en("maptasker_lo
+00005ed0: 676f 5f64 6172 6b2e 706e 6722 292c 0a20  go_dark.png"),. 
+00005ee0: 2020 2020 2020 2073 697a 653d 2831 3930         size=(190
+00005ef0: 2c20 3530 292c 0a20 2020 2029 0a20 2020  , 50),.    ).   
+00005f00: 2074 7279 3a0a 2020 2020 2020 2020 7365   try:.        se
+00005f10: 6c66 2e6c 6f67 6f5f 6c61 6265 6c20 3d20  lf.logo_label = 
+00005f20: 6374 6b2e 4354 6b4c 6162 656c 280a 2020  ctk.CTkLabel(.  
+00005f30: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00005f40: 6964 6562 6172 5f66 7261 6d65 2c0a 2020  idebar_frame,.  
+00005f50: 2020 2020 2020 2020 2020 696d 6167 653d            image=
+00005f60: 6d79 5f69 6d61 6765 2c0a 2020 2020 2020  my_image,.      
+00005f70: 2020 2020 2020 7465 7874 3d22 222c 0a20        text="",. 
+00005f80: 2020 2020 2020 2020 2020 2063 6f6d 706f             compo
+00005f90: 756e 643d 226c 6566 7422 2c0a 2020 2020  und="left",.    
+00005fa0: 2020 2020 2020 2020 666f 6e74 3d63 746b          font=ctk
+00005fb0: 2e43 546b 466f 6e74 2873 697a 653d 312c  .CTkFont(size=1,
+00005fc0: 2077 6569 6768 743d 2262 6f6c 6422 292c   weight="bold"),
+00005fd0: 0a20 2020 2020 2020 2029 2020 2320 6469  .        )  # di
+00005fe0: 7370 6c61 7920 696d 6167 6520 7769 7468  splay image with
+00005ff0: 2061 2043 546b 4c61 6265 6c0a 2020 2020   a CTkLabel.    
+00006000: 2020 2020 7365 6c66 2e6c 6f67 6f5f 6c61      self.logo_la
+00006010: 6265 6c2e 6772 6964 2872 6f77 3d30 2c20  bel.grid(row=0, 
+00006020: 636f 6c75 6d6e 3d30 2c20 7061 6478 3d30  column=0, padx=0
+00006030: 2c20 7061 6479 3d30 2c20 7374 6963 6b79  , pady=0, sticky
+00006040: 3d22 6e22 290a 2020 2020 6578 6365 7074  ="n").    except
+00006050: 3a20 2023 206e 6f71 613a 2053 3131 300a  :  # noqa: S110.
+00006060: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+00006070: 2023 2064 656c 206d 795f 696d 6167 6520   # del my_image 
+00006080: 2023 2044 6f6e 6520 7769 7468 2069 6d61   # Done with ima
+00006090: 6765 2e2e 2e67 6574 2072 6964 206f 6620  ge...get rid of 
+000060a0: 6974 2e0a 0a20 2020 2023 2053 7769 7463  it...    # Switc
+000060b0: 6820 6261 636b 2074 6f20 7072 6f70 6572  h back to proper
+000060c0: 2064 6972 6563 746f 7279 0a20 2020 206f   directory.    o
+000060d0: 732e 6368 6469 7228 6375 7272 656e 745f  s.chdir(current_
+000060e0: 6469 7229 0a0a 0a23 2043 7265 6174 6520  dir)...# Create 
+000060f0: 6120 6c61 6265 6c20 6765 6e65 7261 6c20  a label general 
+00006100: 726f 7574 696e 650a 6465 6620 6164 645f  routine.def add_
+00006110: 6c61 6265 6c28 0a20 2020 2073 656c 662c  label(.    self,
+00006120: 2020 2320 6e6f 7161 3a20 414e 4e30 3031    # noqa: ANN001
+00006130: 2c20 4152 4730 3031 0a20 2020 2066 7261  , ARG001.    fra
+00006140: 6d65 3a20 6374 6b2e 4354 6b46 7261 6d65  me: ctk.CTkFrame
+00006150: 2c0a 2020 2020 7465 7874 3a20 7374 722c  ,.    text: str,
+00006160: 0a20 2020 2074 6578 745f 636f 6c6f 723a  .    text_color:
+00006170: 2073 7472 2c0a 2020 2020 666f 6e74 5f73   str,.    font_s
+00006180: 697a 653a 2069 6e74 2c0a 2020 2020 666f  ize: int,.    fo
+00006190: 6e74 5f77 6569 6768 743a 2073 7472 2c0a  nt_weight: str,.
+000061a0: 2020 2020 726f 773a 2069 6e74 2c0a 2020      row: int,.  
+000061b0: 2020 636f 6c75 6d6e 3a20 696e 742c 0a20    column: int,. 
+000061c0: 2020 2070 6164 783a 2074 7570 6c65 2c0a     padx: tuple,.
+000061d0: 2020 2020 7061 6479 3a20 7475 706c 652c      pady: tuple,
+000061e0: 0a20 2020 2073 7469 636b 793a 2073 7472  .    sticky: str
+000061f0: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
+00006200: 2022 2222 4164 6473 2061 2063 7573 746f   """Adds a custo
+00006210: 6d20 6c61 6265 6c20 746f 2061 2063 7573  m label to a cus
+00006220: 746f 6d20 746b 696e 7465 7220 6672 616d  tom tkinter fram
+00006230: 652e 0a20 2020 2050 6172 616d 6574 6572  e..    Parameter
+00006240: 733a 0a20 2020 2020 2020 202d 2066 7261  s:.        - fra
+00006250: 6d65 2028 6374 6b2e 4354 6b46 7261 6d65  me (ctk.CTkFrame
+00006260: 293a 2054 6865 2066 7261 6d65 2074 6f20  ): The frame to 
+00006270: 6164 6420 7468 6520 6c61 6265 6c20 746f  add the label to
+00006280: 2e0a 2020 2020 2020 2020 2d20 6e61 6d65  ..        - name
+00006290: 2028 6374 6b2e 4354 6b4c 6162 656c 293a   (ctk.CTkLabel):
+000062a0: 2054 6865 206c 6162 656c 2074 6f20 6265   The label to be
+000062b0: 2061 6464 6564 2e0a 2020 2020 2020 2020   added..        
+000062c0: 2d20 7465 7874 2028 7374 7229 3a20 5468  - text (str): Th
+000062d0: 6520 7465 7874 2074 6f20 6265 2064 6973  e text to be dis
+000062e0: 706c 6179 6564 206f 6e20 7468 6520 6c61  played on the la
+000062f0: 6265 6c2e 0a20 2020 2020 2020 202d 2074  bel..        - t
+00006300: 6578 745f 636f 6c6f 7220 2873 7472 293a  ext_color (str):
+00006310: 2063 6f6c 6f72 2066 6f72 2074 6865 2074   color for the t
+00006320: 6578 740a 2020 2020 2020 2020 2d20 666f  ext.        - fo
+00006330: 6e74 5f73 697a 6520 2869 6e74 293a 2054  nt_size (int): T
+00006340: 6865 2066 6f6e 7420 7369 7a65 206f 6620  he font size of 
+00006350: 7468 6520 6c61 6265 6c2e 0a20 2020 2020  the label..     
+00006360: 2020 202d 2066 6f6e 745f 7765 6967 6874     - font_weight
+00006370: 2028 7374 7229 3a20 5468 6520 666f 6e74   (str): The font
+00006380: 2077 6569 6768 7420 6f66 2074 6865 206c   weight of the l
+00006390: 6162 656c 2e0a 2020 2020 2020 2020 2d20  abel..        - 
+000063a0: 726f 7720 2869 6e74 293a 2054 6865 2072  row (int): The r
+000063b0: 6f77 206e 756d 6265 7220 746f 2070 6c61  ow number to pla
+000063c0: 6365 2074 6865 206c 6162 656c 2069 6e2e  ce the label in.
+000063d0: 0a20 2020 2020 2020 202d 2063 6f6c 756d  .        - colum
+000063e0: 6e20 2869 6e74 293a 2054 6865 2063 6f6c  n (int): The col
+000063f0: 756d 6e20 6e75 6d62 6572 2074 6f20 706c  umn number to pl
+00006400: 6163 6520 7468 6520 6c61 6265 6c20 696e  ace the label in
+00006410: 2e0a 2020 2020 2020 2020 2d20 7061 6478  ..        - padx
+00006420: 2028 7475 706c 6529 3a20 5468 6520 686f   (tuple): The ho
+00006430: 7269 7a6f 6e74 616c 2070 6164 6469 6e67  rizontal padding
+00006440: 206f 6620 7468 6520 6c61 6265 6c2e 0a20   of the label.. 
+00006450: 2020 2020 2020 202d 2070 6164 7920 2874         - pady (t
+00006460: 7570 6c65 293a 2054 6865 2076 6572 7469  uple): The verti
+00006470: 6361 6c20 7061 6464 696e 6720 6f66 2074  cal padding of t
+00006480: 6865 206c 6162 656c 2e0a 2020 2020 2020  he label..      
+00006490: 2020 2d20 7374 6963 6b79 2028 7374 7229    - sticky (str)
+000064a0: 3a20 5468 6520 616c 6967 6e6d 656e 7420  : The alignment 
+000064b0: 6f66 2074 6865 206c 6162 656c 2077 6974  of the label wit
+000064c0: 6869 6e20 6974 7320 6772 6964 2063 656c  hin its grid cel
+000064d0: 6c2e 0a20 2020 2052 6574 7572 6e73 3a0a  l..    Returns:.
+000064e0: 2020 2020 2020 2020 2d20 6c61 6265 6c5f          - label_
+000064f0: 6e61 6d65 2028 7374 7229 3a20 5468 6520  name (str): The 
+00006500: 6e61 6d65 206f 6620 7468 6520 6c61 6265  name of the labe
+00006510: 6c2e 0a20 2020 2050 726f 6365 7373 696e  l..    Processin
+00006520: 6720 4c6f 6769 633a 0a20 2020 2020 2020  g Logic:.       
+00006530: 202d 2043 7265 6174 6573 2061 2063 7573   - Creates a cus
+00006540: 746f 6d20 6c61 6265 6c20 7769 7468 2074  tom label with t
+00006550: 6865 2067 6976 656e 2070 6172 616d 6574  he given paramet
+00006560: 6572 732e 0a20 2020 2020 2020 202d 2050  ers..        - P
+00006570: 6c61 6365 7320 7468 6520 6c61 6265 6c20  laces the label 
+00006580: 696e 2074 6865 2073 7065 6369 6669 6564  in the specified
+00006590: 2072 6f77 2061 6e64 2063 6f6c 756d 6e20   row and column 
+000065a0: 6f66 2074 6865 2066 7261 6d65 2e0a 2020  of the frame..  
+000065b0: 2020 2020 2020 2d20 4164 6473 2068 6f72        - Adds hor
+000065c0: 697a 6f6e 7461 6c20 616e 6420 7665 7274  izontal and vert
+000065d0: 6963 616c 2070 6164 6469 6e67 2074 6f20  ical padding to 
+000065e0: 7468 6520 6c61 6265 6c2e 0a20 2020 2020  the label..     
+000065f0: 2020 202d 2041 6c69 676e 7320 7468 6520     - Aligns the 
+00006600: 6c61 6265 6c20 7769 7468 696e 2069 7473  label within its
+00006610: 2067 7269 6420 6365 6c6c 2e22 2222 0a20   grid cell.""". 
+00006620: 2020 2069 6620 6e6f 7420 666f 6e74 5f73     if not font_s
+00006630: 697a 6520 6f72 2066 6f6e 745f 7369 7a65  ize or font_size
+00006640: 203d 3d20 303a 0a20 2020 2020 2020 2066   == 0:.        f
+00006650: 6f6e 745f 7369 7a65 203d 2064 6566 6175  ont_size = defau
+00006660: 6c74 5f66 6f6e 745f 7369 7a65 0a20 2020  lt_font_size.   
+00006670: 2069 6620 6e6f 7420 7465 7874 5f63 6f6c   if not text_col
+00006680: 6f72 3a0a 2020 2020 2020 2020 7465 7874  or:.        text
+00006690: 5f63 6f6c 6f72 203d 2022 2346 4646 4646  _color = "#FFFFF
+000066a0: 4622 0a20 2020 206c 6162 656c 5f6e 616d  F".    label_nam
+000066b0: 6520 3d20 6374 6b2e 4354 6b4c 6162 656c  e = ctk.CTkLabel
+000066c0: 280a 2020 2020 2020 2020 6672 616d 652c  (.        frame,
+000066d0: 0a20 2020 2020 2020 2074 6578 743d 7465  .        text=te
+000066e0: 7874 2c0a 2020 2020 2020 2020 7465 7874  xt,.        text
+000066f0: 5f63 6f6c 6f72 3d74 6578 745f 636f 6c6f  _color=text_colo
+00006700: 722c 0a20 2020 2020 2020 2066 6f6e 743d  r,.        font=
+00006710: 6374 6b2e 4354 6b46 6f6e 7428 7369 7a65  ctk.CTkFont(size
+00006720: 3d66 6f6e 745f 7369 7a65 2c20 7765 6967  =font_size, weig
+00006730: 6874 3d66 6f6e 745f 7765 6967 6874 292c  ht=font_weight),
+00006740: 0a20 2020 2029 0a20 2020 206c 6162 656c  .    ).    label
+00006750: 5f6e 616d 652e 6772 6964 2872 6f77 3d72  _name.grid(row=r
+00006760: 6f77 2c20 636f 6c75 6d6e 3d63 6f6c 756d  ow, column=colum
+00006770: 6e2c 2070 6164 783d 7061 6478 2c20 7061  n, padx=padx, pa
+00006780: 6479 3d70 6164 792c 2073 7469 636b 793d  dy=pady, sticky=
+00006790: 7374 6963 6b79 290a 2020 2020 7265 7475  sticky).    retu
+000067a0: 726e 206c 6162 656c 5f6e 616d 650a 0a0a  rn label_name...
+000067b0: 2320 4372 6561 7465 2061 2063 6865 636b  # Create a check
+000067c0: 626f 7820 6765 6e65 7261 6c20 726f 7574  box general rout
+000067d0: 696e 650a 6465 6620 6164 645f 6368 6563  ine.def add_chec
+000067e0: 6b62 6f78 280a 2020 2020 7365 6c66 2c20  kbox(.    self, 
+000067f0: 2023 206e 6f71 613a 2041 4e4e 3030 312c   # noqa: ANN001,
+00006800: 2041 5247 3030 310a 2020 2020 6672 616d   ARG001.    fram
+00006810: 653a 2063 746b 2e43 546b 4672 616d 652c  e: ctk.CTkFrame,
+00006820: 0a20 2020 2063 6f6d 6d61 6e64 3a20 4361  .    command: Ca
+00006830: 6c6c 6162 6c65 2c0a 2020 2020 7465 7874  llable,.    text
+00006840: 3a20 7374 722c 0a20 2020 2072 6f77 3a20  : str,.    row: 
+00006850: 696e 742c 0a20 2020 2063 6f6c 756d 6e3a  int,.    column:
+00006860: 2069 6e74 2c0a 2020 2020 7061 6478 3a20   int,.    padx: 
+00006870: 7475 706c 652c 0a20 2020 2070 6164 793a  tuple,.    pady:
+00006880: 2074 7570 6c65 2c0a 2020 2020 7374 6963   tuple,.    stic
+00006890: 6b79 3a20 7374 722c 0a20 2020 2062 6f72  ky: str,.    bor
+000068a0: 6465 725f 636f 6c6f 723a 2073 7472 2c0a  der_color: str,.
+000068b0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
+000068c0: 2222 4164 6420 6120 6368 6563 6b62 6f78  ""Add a checkbox
+000068d0: 2074 6f20 6120 6375 7374 6f6d 2074 6b69   to a custom tki
+000068e0: 6e74 6572 2066 7261 6d65 2e0a 2020 2020  nter frame..    
+000068f0: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
+00006900: 2020 2020 2d20 6672 616d 6520 2863 746b      - frame (ctk
+00006910: 2e43 546b 4672 616d 6529 3a20 5468 6520  .CTkFrame): The 
+00006920: 6375 7374 6f6d 2074 6b69 6e74 6572 2066  custom tkinter f
+00006930: 7261 6d65 2074 6f20 6164 6420 7468 6520  rame to add the 
+00006940: 6368 6563 6b62 6f78 2074 6f2e 0a20 2020  checkbox to..   
+00006950: 2020 2020 202d 2063 6f6d 6d61 6e64 2028       - command (
+00006960: 6f62 6a65 6374 293a 2054 6865 2063 6f6d  object): The com
+00006970: 6d61 6e64 2074 6f20 6265 2065 7865 6375  mand to be execu
+00006980: 7465 6420 7768 656e 2074 6865 2063 6865  ted when the che
+00006990: 636b 626f 7820 6973 2063 6c69 636b 6564  ckbox is clicked
+000069a0: 2e0a 2020 2020 2020 2020 2d20 7465 7874  ..        - text
+000069b0: 2028 7374 7229 3a20 5468 6520 7465 7874   (str): The text
+000069c0: 2074 6f20 6265 2064 6973 706c 6179 6564   to be displayed
+000069d0: 206e 6578 7420 746f 2074 6865 2063 6865   next to the che
+000069e0: 636b 626f 782e 0a20 2020 2020 2020 202d  ckbox..        -
+000069f0: 2072 6f77 2028 696e 7429 3a20 5468 6520   row (int): The 
+00006a00: 726f 7720 746f 2070 6c61 6365 2074 6865  row to place the
+00006a10: 2063 6865 636b 626f 7820 696e 2e0a 2020   checkbox in..  
+00006a20: 2020 2020 2020 2d20 636f 6c75 6d6e 2028        - column (
+00006a30: 696e 7429 3a20 5468 6520 636f 6c75 6d6e  int): The column
+00006a40: 2074 6f20 706c 6163 6520 7468 6520 6368   to place the ch
+00006a50: 6563 6b62 6f78 2069 6e2e 0a20 2020 2020  eckbox in..     
+00006a60: 2020 202d 2070 6164 7820 2874 7570 6c65     - padx (tuple
+00006a70: 293a 2054 6865 2068 6f72 697a 6f6e 7461  ): The horizonta
+00006a80: 6c20 7061 6464 696e 6720 666f 7220 7468  l padding for th
+00006a90: 6520 6368 6563 6b62 6f78 2e0a 2020 2020  e checkbox..    
+00006aa0: 2020 2020 2d20 7061 6479 2028 7475 706c      - pady (tupl
+00006ab0: 6529 3a20 5468 6520 7665 7274 6963 616c  e): The vertical
+00006ac0: 2070 6164 6469 6e67 2066 6f72 2074 6865   padding for the
+00006ad0: 2063 6865 636b 626f 782e 0a20 2020 2020   checkbox..     
+00006ae0: 2020 202d 2073 7469 636b 7920 2873 7472     - sticky (str
+00006af0: 293a 2054 6865 2061 6c69 676e 6d65 6e74  ): The alignment
+00006b00: 206f 6620 7468 6520 6368 6563 6b62 6f78   of the checkbox
+00006b10: 2077 6974 6869 6e20 6974 7320 6772 6964   within its grid
+00006b20: 2063 656c 6c2e 0a20 2020 2020 2020 202d   cell..        -
+00006b30: 2062 6f72 6465 725f 636f 6c6f 7220 2873   border_color (s
+00006b40: 7472 293a 2054 6865 2063 6f6c 6f72 2074  tr): The color t
+00006b50: 6f20 6869 6768 6c69 6768 746e 2074 6865  o highlightn the
+00006b60: 2062 7574 746f 6e20 7769 7468 2e0a 2020   button with..  
+00006b70: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00006b80: 2020 202d 2063 6865 636b 626f 785f 6e61     - checkbox_na
+00006b90: 6d65 3a20 7468 6520 6e61 6d65 6420 6368  me: the named ch
+00006ba0: 6563 6b62 6f78 2e0a 2020 2020 5072 6f63  eckbox..    Proc
+00006bb0: 6573 7369 6e67 204c 6f67 6963 3a0a 2020  essing Logic:.  
+00006bc0: 2020 2020 2020 2d20 4372 6561 7465 2061        - Create a
+00006bd0: 2063 7573 746f 6d20 746b 696e 7465 7220   custom tkinter 
+00006be0: 6368 6563 6b62 6f78 2e0a 2020 2020 2020  checkbox..      
+00006bf0: 2020 2d20 4164 6420 7468 6520 6368 6563    - Add the chec
+00006c00: 6b62 6f78 2074 6f20 7468 6520 7370 6563  kbox to the spec
+00006c10: 6966 6965 6420 6672 616d 652e 0a20 2020  ified frame..   
+00006c20: 2020 2020 202d 2050 6c61 6365 2074 6865       - Place the
+00006c30: 2063 6865 636b 626f 7820 696e 2074 6865   checkbox in the
+00006c40: 2073 7065 6369 6669 6564 2072 6f77 2061   specified row a
+00006c50: 6e64 2063 6f6c 756d 6e2e 0a20 2020 2020  nd column..     
+00006c60: 2020 202d 2041 7070 6c79 2074 6865 2073     - Apply the s
+00006c70: 7065 6369 6669 6564 2070 6164 6469 6e67  pecified padding
+00006c80: 2074 6f20 7468 6520 6368 6563 6b62 6f78   to the checkbox
+00006c90: 2e0a 2020 2020 2020 2020 2d20 416c 6967  ..        - Alig
+00006ca0: 6e20 7468 6520 6368 6563 6b62 6f78 2077  n the checkbox w
+00006cb0: 6974 6869 6e20 6974 7320 6772 6964 2063  ithin its grid c
+00006cc0: 656c 6c2e 2222 220a 2020 2020 6368 6563  ell.""".    chec
+00006cd0: 6b62 6f78 5f6e 616d 6520 3d20 6374 6b2e  kbox_name = ctk.
+00006ce0: 4354 6b43 6865 636b 426f 7828 0a20 2020  CTkCheckBox(.   
+00006cf0: 2020 2020 2066 7261 6d65 2c0a 2020 2020       frame,.    
+00006d00: 2020 2020 636f 6d6d 616e 643d 636f 6d6d      command=comm
+00006d10: 616e 642c 0a20 2020 2020 2020 2074 6578  and,.        tex
+00006d20: 743d 7465 7874 2c0a 2020 2020 2020 2020  t=text,.        
+00006d30: 666f 6e74 3d63 746b 2e43 546b 466f 6e74  font=ctk.CTkFont
+00006d40: 2873 697a 653d 6465 6661 756c 745f 666f  (size=default_fo
+00006d50: 6e74 5f73 697a 652c 2077 6569 6768 743d  nt_size, weight=
+00006d60: 226e 6f72 6d61 6c22 292c 0a20 2020 2020  "normal"),.     
+00006d70: 2020 206f 6e76 616c 7565 3d54 7275 652c     onvalue=True,
+00006d80: 0a20 2020 2020 2020 206f 6666 7661 6c75  .        offvalu
+00006d90: 653d 4661 6c73 652c 0a20 2020 2029 0a20  e=False,.    ). 
+00006da0: 2020 2069 6620 626f 7264 6572 5f63 6f6c     if border_col
+00006db0: 6f72 3a0a 2020 2020 2020 2020 6368 6563  or:.        chec
+00006dc0: 6b62 6f78 5f6e 616d 652e 636f 6e66 6967  kbox_name.config
+00006dd0: 7572 6528 626f 7264 6572 5f63 6f6c 6f72  ure(border_color
+00006de0: 3d62 6f72 6465 725f 636f 6c6f 7229 0a20  =border_color). 
+00006df0: 2020 2063 6865 636b 626f 785f 6e61 6d65     checkbox_name
+00006e00: 2e67 7269 6428 726f 773d 726f 772c 2063  .grid(row=row, c
+00006e10: 6f6c 756d 6e3d 636f 6c75 6d6e 2c20 7061  olumn=column, pa
+00006e20: 6478 3d70 6164 782c 2070 6164 793d 7061  dx=padx, pady=pa
+00006e30: 6479 2c20 7374 6963 6b79 3d73 7469 636b  dy, sticky=stick
+00006e40: 7929 0a20 2020 2072 6574 7572 6e20 6368  y).    return ch
+00006e50: 6563 6b62 6f78 5f6e 616d 650a 0a0a 2320  eckbox_name...# 
+00006e60: 4372 6561 7465 2061 2062 7574 746f 6e20  Create a button 
+00006e70: 6765 6e65 7261 6c20 726f 7574 696e 650a  general routine.
+00006e80: 6465 6620 6164 645f 6275 7474 6f6e 280a  def add_button(.
+00006e90: 2020 2020 7365 6c66 2c20 2023 206e 6f71      self,  # noq
+00006ea0: 613a 2041 4e4e 3030 312c 2041 5247 3030  a: ANN001, ARG00
+00006eb0: 310a 2020 2020 6672 616d 653a 2063 746b  1.    frame: ctk
+00006ec0: 2e43 546b 4672 616d 652c 0a20 2020 2066  .CTkFrame,.    f
+00006ed0: 675f 636f 6c6f 723a 2073 7472 2c0a 2020  g_color: str,.  
+00006ee0: 2020 7465 7874 5f63 6f6c 6f72 3a20 7374    text_color: st
+00006ef0: 722c 0a20 2020 2062 6f72 6465 725f 636f  r,.    border_co
+00006f00: 6c6f 723a 2073 7472 2c0a 2020 2020 636f  lor: str,.    co
+00006f10: 6d6d 616e 643a 2043 616c 6c61 626c 652c  mmand: Callable,
+00006f20: 0a20 2020 2062 6f72 6465 725f 7769 6474  .    border_widt
+00006f30: 683a 2069 6e74 2c0a 2020 2020 7465 7874  h: int,.    text
+00006f40: 3a20 7374 722c 0a20 2020 2063 6f6c 756d  : str,.    colum
+00006f50: 6e73 7061 6e3a 2069 6e74 2c0a 2020 2020  nspan: int,.    
+00006f60: 726f 773a 2069 6e74 2c0a 2020 2020 636f  row: int,.    co
+00006f70: 6c75 6d6e 3a20 696e 742c 0a20 2020 2070  lumn: int,.    p
+00006f80: 6164 783a 2074 7570 6c65 2c0a 2020 2020  adx: tuple,.    
+00006f90: 7061 6479 3a20 7475 706c 652c 0a20 2020  pady: tuple,.   
+00006fa0: 2073 7469 636b 793a 2073 7472 2c0a 2920   sticky: str,.) 
+00006fb0: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+00006fc0: 4164 6420 6120 6275 7474 6f6e 2074 6f20  Add a button to 
+00006fd0: 6120 6375 7374 6f6d 2074 6b69 6e74 6572  a custom tkinter
+00006fe0: 2066 7261 6d65 2e0a 2020 2020 5061 7261   frame..    Para
+00006ff0: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
+00007000: 2d20 6672 616d 6520 2863 746b 2e43 546b  - frame (ctk.CTk
+00007010: 4672 616d 6529 3a20 5468 6520 6672 616d  Frame): The fram
+00007020: 6520 746f 2061 6464 2074 6865 2062 7574  e to add the but
+00007030: 746f 6e20 746f 2e0a 2020 2020 2020 2020  ton to..        
+00007040: 2d20 6667 5f63 6f6c 6f72 2028 7374 7229  - fg_color (str)
+00007050: 3a20 5468 6520 636f 6c6f 7220 6f66 2074  : The color of t
+00007060: 6865 2062 7574 746f 6e27 7320 7465 7874  he button's text
+00007070: 2e0a 2020 2020 2020 2020 2d20 7465 7874  ..        - text
+00007080: 5f63 6f6c 6f72 2028 7374 7229 2054 6865  _color (str) The
+00007090: 2063 6f6c 6f72 206f 6620 7468 6520 6275   color of the bu
+000070a0: 7474 6f6e 2773 2074 6578 742e 0a20 2020  tton's text..   
+000070b0: 2020 2020 202d 2063 6f6d 6d61 6e64 2028       - command (
+000070c0: 6f62 6a65 6374 293a 2054 6865 2066 756e  object): The fun
+000070d0: 6374 696f 6e20 746f 2062 6520 6578 6563  ction to be exec
+000070e0: 7574 6564 2077 6865 6e20 7468 6520 6275  uted when the bu
+000070f0: 7474 6f6e 2069 7320 636c 6963 6b65 642e  tton is clicked.
+00007100: 0a20 2020 2020 2020 202d 2062 6f72 6465  .        - borde
+00007110: 725f 7769 6474 6820 2869 6e74 293a 2054  r_width (int): T
+00007120: 6865 2077 6964 7468 206f 6620 7468 6520  he width of the 
+00007130: 6275 7474 6f6e 2773 2062 6f72 6465 722e  button's border.
+00007140: 0a20 2020 2020 2020 202d 2074 6578 7420  .        - text 
+00007150: 2873 7472 293a 2054 6865 2074 6578 7420  (str): The text 
+00007160: 746f 2062 6520 6469 7370 6c61 7965 6420  to be displayed 
+00007170: 6f6e 2074 6865 2062 7574 746f 6e2e 0a20  on the button.. 
+00007180: 2020 2020 2020 202d 2063 6f6c 756d 6e73         - columns
+00007190: 7061 6e20 2869 6e74 293a 2054 6865 206e  pan (int): The n
+000071a0: 756d 6265 7220 6f66 2063 6f6c 756d 6e73  umber of columns
+000071b0: 2074 6f20 7370 616e 2074 6865 2062 7574   to span the but
+000071c0: 746f 6e20 6163 726f 7373 2e0a 2020 2020  ton across..    
+000071d0: 2020 2020 2d20 726f 7720 2869 6e74 293a      - row (int):
+000071e0: 2054 6865 2072 6f77 2074 6f20 706c 6163   The row to plac
+000071f0: 6520 7468 6520 6275 7474 6f6e 2069 6e2e  e the button in.
+00007200: 0a20 2020 2020 2020 202d 2063 6f6c 756d  .        - colum
+00007210: 6e20 2869 6e74 293a 2054 6865 2063 6f6c  n (int): The col
+00007220: 756d 6e20 746f 2070 6c61 6365 2074 6865  umn to place the
+00007230: 2062 7574 746f 6e20 696e 2e0a 2020 2020   button in..    
+00007240: 2020 2020 2d20 7061 6478 2028 7475 706c      - padx (tupl
+00007250: 6529 3a20 5468 6520 616d 6f75 6e74 206f  e): The amount o
+00007260: 6620 7061 6464 696e 6720 6f6e 2074 6865  f padding on the
+00007270: 2078 2d61 7869 732e 0a20 2020 2020 2020   x-axis..       
+00007280: 202d 2070 6164 7920 2874 7570 6c65 293a   - pady (tuple):
+00007290: 2054 6865 2061 6d6f 756e 7420 6f66 2070   The amount of p
+000072a0: 6164 6469 6e67 206f 6e20 7468 6520 792d  adding on the y-
+000072b0: 6178 6973 2e0a 2020 2020 2020 2020 2d20  axis..        - 
+000072c0: 7374 6963 6b79 2028 7374 7229 3a20 5468  sticky (str): Th
+000072d0: 6520 616c 6967 6e6d 656e 7420 6f66 2074  e alignment of t
+000072e0: 6865 2062 7574 746f 6e20 7769 7468 696e  he button within
+000072f0: 2069 7473 2063 656c 6c2e 0a20 2020 2052   its cell..    R
+00007300: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00007310: 2d20 6275 7474 6f6e 5f6e 616d 653a 2074  - button_name: t
+00007320: 6865 206e 616d 6564 2062 7574 746f 6e2e  he named button.
+00007330: 0a20 2020 2050 726f 6365 7373 696e 6720  .    Processing 
+00007340: 4c6f 6769 633a 0a20 2020 2020 2020 202d  Logic:.        -
+00007350: 2043 7265 6174 6520 6120 6375 7374 6f6d   Create a custom
+00007360: 2074 6b69 6e74 6572 2062 7574 746f 6e20   tkinter button 
+00007370: 7769 7468 2074 6865 2067 6976 656e 2070  with the given p
+00007380: 6172 616d 6574 6572 732e 0a20 2020 2020  arameters..     
+00007390: 2020 202d 2050 6c61 6365 2074 6865 2062     - Place the b
+000073a0: 7574 746f 6e20 696e 2074 6865 2073 7065  utton in the spe
+000073b0: 6369 6669 6564 2072 6f77 2061 6e64 2063  cified row and c
+000073c0: 6f6c 756d 6e2e 0a20 2020 2020 2020 202d  olumn..        -
+000073d0: 2041 6464 2070 6164 6469 6e67 2061 6e64   Add padding and
+000073e0: 2061 6c69 676e 6d65 6e74 2074 6f20 7468   alignment to th
+000073f0: 6520 6275 7474 6f6e 2e22 2222 0a20 2020  e button.""".   
+00007400: 2069 6620 6e6f 7420 6667 5f63 6f6c 6f72   if not fg_color
+00007410: 3a0a 2020 2020 2020 2020 6667 5f63 6f6c  :.        fg_col
+00007420: 6f72 203d 2022 2332 3436 4642 3622 0a20  or = "#246FB6". 
+00007430: 2020 2069 6620 6e6f 7420 7465 7874 5f63     if not text_c
+00007440: 6f6c 6f72 3a0a 2020 2020 2020 2020 7465  olor:.        te
+00007450: 7874 5f63 6f6c 6f72 203d 2022 2346 4646  xt_color = "#FFF
+00007460: 4646 4622 0a20 2020 2069 6620 6e6f 7420  FFF".    if not 
+00007470: 626f 7264 6572 5f63 6f6c 6f72 3a0a 2020  border_color:.  
+00007480: 2020 2020 2020 626f 7264 6572 5f63 6f6c        border_col
+00007490: 6f72 203d 2022 4772 6179 220a 2020 2020  or = "Gray".    
+000074a0: 6966 206e 6f74 2063 6f6c 756d 6e73 7061  if not columnspa
+000074b0: 6e3a 0a20 2020 2020 2020 2063 6f6c 756d  n:.        colum
+000074c0: 6e73 7061 6e20 3d20 310a 2020 2020 6275  nspan = 1.    bu
+000074d0: 7474 6f6e 5f6e 616d 6520 3d20 6374 6b2e  tton_name = ctk.
+000074e0: 4354 6b42 7574 746f 6e28 0a20 2020 2020  CTkButton(.     
+000074f0: 2020 2066 7261 6d65 2c0a 2020 2020 2020     frame,.      
+00007500: 2020 6667 5f63 6f6c 6f72 3d66 675f 636f    fg_color=fg_co
+00007510: 6c6f 722c 0a20 2020 2020 2020 2074 6578  lor,.        tex
+00007520: 745f 636f 6c6f 723d 7465 7874 5f63 6f6c  t_color=text_col
+00007530: 6f72 2c0a 2020 2020 2020 2020 666f 6e74  or,.        font
+00007540: 3d63 746b 2e43 546b 466f 6e74 2873 697a  =ctk.CTkFont(siz
+00007550: 653d 6465 6661 756c 745f 666f 6e74 5f73  e=default_font_s
+00007560: 697a 652c 2077 6569 6768 743d 226e 6f72  ize, weight="nor
+00007570: 6d61 6c22 292c 0a20 2020 2020 2020 2062  mal"),.        b
+00007580: 6f72 6465 725f 636f 6c6f 723d 626f 7264  order_color=bord
+00007590: 6572 5f63 6f6c 6f72 2c0a 2020 2020 2020  er_color,.      
+000075a0: 2020 636f 6d6d 616e 643d 636f 6d6d 616e    command=comman
+000075b0: 642c 0a20 2020 2020 2020 2062 6f72 6465  d,.        borde
+000075c0: 725f 7769 6474 683d 626f 7264 6572 5f77  r_width=border_w
+000075d0: 6964 7468 2c0a 2020 2020 2020 2020 7465  idth,.        te
+000075e0: 7874 3d74 6578 742c 0a20 2020 2029 0a20  xt=text,.    ). 
+000075f0: 2020 2062 7574 746f 6e5f 6e61 6d65 2e67     button_name.g
+00007600: 7269 6428 726f 773d 726f 772c 2063 6f6c  rid(row=row, col
+00007610: 756d 6e3d 636f 6c75 6d6e 2c20 636f 6c75  umn=column, colu
+00007620: 6d6e 7370 616e 3d63 6f6c 756d 6e73 7061  mnspan=columnspa
+00007630: 6e2c 2070 6164 783d 7061 6478 2c20 7061  n, padx=padx, pa
+00007640: 6479 3d70 6164 792c 2073 7469 636b 793d  dy=pady, sticky=
+00007650: 7374 6963 6b79 290a 2020 2020 7265 7475  sticky).    retu
+00007660: 726e 2062 7574 746f 6e5f 6e61 6d65 0a0a  rn button_name..
+00007670: 0a23 2043 7265 6174 6520 6120 6275 7474  .# Create a butt
+00007680: 6f6e 2067 656e 6572 616c 2072 6f75 7469  on general routi
+00007690: 6e65 0a64 6566 2061 6464 5f6f 7074 696f  ne.def add_optio
+000076a0: 6e5f 6d65 6e75 280a 2020 2020 7365 6c66  n_menu(.    self
+000076b0: 2c20 2023 206e 6f71 613a 2041 4e4e 3030  ,  # noqa: ANN00
+000076c0: 312c 2041 5247 3030 310a 2020 2020 6672  1, ARG001.    fr
+000076d0: 616d 653a 2063 746b 2e43 546b 4672 616d  ame: ctk.CTkFram
+000076e0: 652c 0a20 2020 2063 6f6d 6d61 6e64 3a20  e,.    command: 
+000076f0: 4361 6c6c 6162 6c65 2c0a 2020 2020 7661  Callable,.    va
+00007700: 6c75 6573 3a20 7374 7220 7c20 6c69 7374  lues: str | list
+00007710: 2c0a 2020 2020 726f 773a 2069 6e74 2c0a  ,.    row: int,.
+00007720: 2020 2020 636f 6c75 6d6e 3a20 696e 742c      column: int,
+00007730: 0a20 2020 2070 6164 783a 2074 7570 6c65  .    padx: tuple
+00007740: 2c0a 2020 2020 7061 6479 3a20 7475 706c  ,.    pady: tupl
+00007750: 652c 0a20 2020 2073 7469 636b 793a 2073  e,.    sticky: s
+00007760: 7472 2c0a 2920 2d3e 204e 6f6e 653a 0a20  tr,.) -> None:. 
+00007770: 2020 2022 2222 4164 6473 2061 6e20 6f70     """Adds an op
+00007780: 7469 6f6e 206d 656e 7520 746f 2061 2067  tion menu to a g
+00007790: 6976 656e 2066 7261 6d65 2077 6974 6820  iven frame with 
+000077a0: 7370 6563 6966 6965 6420 7061 7261 6d65  specified parame
+000077b0: 7465 7273 2e0a 2020 2020 5061 7261 6d65  ters..    Parame
+000077c0: 7465 7273 3a0a 2020 2020 2020 2020 2d20  ters:.        - 
+000077d0: 6672 616d 6520 2863 746b 2e43 546b 4672  frame (ctk.CTkFr
+000077e0: 616d 6529 3a20 5468 6520 6672 616d 6520  ame): The frame 
+000077f0: 746f 2061 6464 2074 6865 206f 7074 696f  to add the optio
+00007800: 6e20 6d65 6e75 2074 6f2e 0a20 2020 2020  n menu to..     
+00007810: 2020 202d 2063 6f6d 6d61 6e64 2028 6f62     - command (ob
+00007820: 6a65 6374 293a 2054 6865 2066 756e 6374  ject): The funct
+00007830: 696f 6e20 746f 2062 6520 6361 6c6c 6564  ion to be called
+00007840: 2077 6865 6e20 616e 206f 7074 696f 6e20   when an option 
+00007850: 6973 2073 656c 6563 7465 642e 0a20 2020  is selected..   
+00007860: 2020 2020 202d 2076 616c 7565 7320 2873       - values (s
+00007870: 7472 207c 206c 6973 7429 3a20 5468 6520  tr | list): The 
+00007880: 6f70 7469 6f6e 7320 746f 2062 6520 6469  options to be di
+00007890: 7370 6c61 7965 6420 696e 2074 6865 206d  splayed in the m
+000078a0: 656e 752e 0a20 2020 2020 2020 202d 2072  enu..        - r
+000078b0: 6f77 2028 696e 7429 3a20 5468 6520 726f  ow (int): The ro
+000078c0: 7720 696e 2077 6869 6368 2074 6865 206f  w in which the o
+000078d0: 7074 696f 6e20 6d65 6e75 2073 686f 756c  ption menu shoul
+000078e0: 6420 6265 2070 6c61 6365 642e 0a20 2020  d be placed..   
+000078f0: 2020 2020 202d 2063 6f6c 756d 6e20 2869       - column (i
+00007900: 6e74 293a 2054 6865 2063 6f6c 756d 6e20  nt): The column 
+00007910: 696e 2077 6869 6368 2074 6865 206f 7074  in which the opt
+00007920: 696f 6e20 6d65 6e75 2073 686f 756c 6420  ion menu should 
+00007930: 6265 2070 6c61 6365 642e 0a20 2020 2020  be placed..     
+00007940: 2020 202d 2070 6164 7820 2874 7570 6c65     - padx (tuple
+00007950: 293a 2054 6865 2061 6d6f 756e 7420 6f66  ): The amount of
+00007960: 2070 6164 6469 6e67 2069 6e20 7468 6520   padding in the 
+00007970: 782d 6469 7265 6374 696f 6e2e 0a20 2020  x-direction..   
+00007980: 2020 2020 202d 2070 6164 7920 2874 7570       - pady (tup
+00007990: 6c65 293a 2054 6865 2061 6d6f 756e 7420  le): The amount 
+000079a0: 6f66 2070 6164 6469 6e67 2069 6e20 7468  of padding in th
+000079b0: 6520 792d 6469 7265 6374 696f 6e2e 0a20  e y-direction.. 
+000079c0: 2020 2020 2020 202d 2073 7469 636b 7920         - sticky 
+000079d0: 2873 7472 293a 2054 6865 2064 6972 6563  (str): The direc
+000079e0: 7469 6f6e 2069 6e20 7768 6963 6820 7468  tion in which th
+000079f0: 6520 6f70 7469 6f6e 206d 656e 7520 7368  e option menu sh
+00007a00: 6f75 6c64 2073 7469 636b 2074 6f20 7468  ould stick to th
+00007a10: 6520 6672 616d 652e 0a20 2020 2052 6574  e frame..    Ret
+00007a20: 7572 6e73 3a0a 2020 2020 2020 2020 2d20  urns:.        - 
+00007a30: 4e6f 6e65 3a20 5468 6973 2066 756e 6374  None: This funct
+00007a40: 696f 6e20 646f 6573 206e 6f74 2072 6574  ion does not ret
+00007a50: 7572 6e20 616e 7920 7661 6c75 652e 0a20  urn any value.. 
+00007a60: 2020 2050 726f 6365 7373 696e 6720 4c6f     Processing Lo
+00007a70: 6769 633a 0a20 2020 2020 2020 202d 2041  gic:.        - A
+00007a80: 6464 7320 616e 206f 7074 696f 6e20 6d65  dds an option me
+00007a90: 6e75 2074 6f20 6120 6672 616d 652e 0a20  nu to a frame.. 
+00007aa0: 2020 2020 2020 202d 2053 6574 7320 7468         - Sets th
+00007ab0: 6520 636f 6d6d 616e 6420 746f 2062 6520  e command to be 
+00007ac0: 6361 6c6c 6564 2077 6865 6e20 616e 206f  called when an o
+00007ad0: 7074 696f 6e20 6973 2073 656c 6563 7465  ption is selecte
+00007ae0: 642e 0a20 2020 2020 2020 202d 2044 6973  d..        - Dis
+00007af0: 706c 6179 7320 7468 6520 7370 6563 6966  plays the specif
+00007b00: 6965 6420 6f70 7469 6f6e 7320 696e 2074  ied options in t
+00007b10: 6865 206d 656e 752e 0a20 2020 2020 2020  he menu..       
+00007b20: 202d 2050 6c61 6365 7320 7468 6520 6f70   - Places the op
+00007b30: 7469 6f6e 206d 656e 7520 696e 2074 6865  tion menu in the
+00007b40: 2073 7065 6369 6669 6564 2072 6f77 2061   specified row a
+00007b50: 6e64 2063 6f6c 756d 6e2e 0a20 2020 2020  nd column..     
+00007b60: 2020 202d 2041 6464 7320 7061 6464 696e     - Adds paddin
+00007b70: 6720 746f 2074 6865 206f 7074 696f 6e20  g to the option 
+00007b80: 6d65 6e75 2e0a 2020 2020 2020 2020 2d20  menu..        - 
+00007b90: 5365 7473 2074 6865 2064 6972 6563 7469  Sets the directi
+00007ba0: 6f6e 2069 6e20 7768 6963 6820 7468 6520  on in which the 
+00007bb0: 6f70 7469 6f6e 206d 656e 7520 7368 6f75  option menu shou
+00007bc0: 6c64 2073 7469 636b 2074 6f20 7468 6520  ld stick to the 
+00007bd0: 6672 616d 652e 2222 220a 2020 2020 6f70  frame.""".    op
+00007be0: 7469 6f6e 5f6d 656e 755f 6e61 6d65 203d  tion_menu_name =
+00007bf0: 2063 746b 2e43 546b 4f70 7469 6f6e 4d65   ctk.CTkOptionMe
+00007c00: 6e75 280a 2020 2020 2020 2020 6672 616d  nu(.        fram
+00007c10: 652c 0a20 2020 2020 2020 2076 616c 7565  e,.        value
+00007c20: 733d 7661 6c75 6573 2c0a 2020 2020 2020  s=values,.      
+00007c30: 2020 636f 6d6d 616e 643d 636f 6d6d 616e    command=comman
+00007c40: 642c 0a20 2020 2029 0a20 2020 206f 7074  d,.    ).    opt
+00007c50: 696f 6e5f 6d65 6e75 5f6e 616d 652e 6772  ion_menu_name.gr
+00007c60: 6964 2872 6f77 3d72 6f77 2c20 636f 6c75  id(row=row, colu
+00007c70: 6d6e 3d63 6f6c 756d 6e2c 2070 6164 783d  mn=column, padx=
+00007c80: 7061 6478 2c20 7061 6479 3d70 6164 792c  padx, pady=pady,
+00007c90: 2073 7469 636b 793d 7374 6963 6b79 290a   sticky=sticky).
+00007ca0: 2020 2020 7265 7475 726e 206f 7074 696f      return optio
+00007cb0: 6e5f 6d65 6e75 5f6e 616d 650a 0a0a 2320  n_menu_name...# 
+00007cc0: 4465 6669 6e65 2061 6c6c 206f 6620 7468  Define all of th
+00007cd0: 6520 6d65 6e75 2065 6c65 6d65 6e74 730a  e menu elements.
+00007ce0: 6465 6620 696e 6974 6961 6c69 7a65 5f73  def initialize_s
+00007cf0: 6372 6565 6e28 7365 6c66 2920 2d3e 204e  creen(self) -> N
+00007d00: 6f6e 653a 2020 2320 6e6f 7161 3a20 414e  one:  # noqa: AN
+00007d10: 4e30 3031 0a20 2020 2023 2041 6464 2067  N001.    # Add g
+00007d20: 7269 6420 7469 746c 650a 2020 2020 2222  rid title.    ""
+00007d30: 2249 6e69 7469 616c 697a 6573 2074 6865  "Initializes the
+00007d40: 2073 6372 6565 6e20 7769 7468 2076 6172   screen with var
+00007d50: 696f 7573 2064 6973 706c 6179 206f 7074  ious display opt
+00007d60: 696f 6e73 2061 6e64 2073 6574 7469 6e67  ions and setting
+00007d70: 732e 0a20 2020 2050 6172 616d 6574 6572  s..    Parameter
+00007d80: 733a 0a20 2020 2020 2020 202d 2073 656c  s:.        - sel
+00007d90: 6620 286f 626a 6563 7429 3a20 5468 6520  f (object): The 
+00007da0: 6f62 6a65 6374 2074 6f20 7768 6963 6820  object to which 
+00007db0: 7468 6520 6675 6e63 7469 6f6e 2062 656c  the function bel
+00007dc0: 6f6e 6773 2e0a 2020 2020 5265 7475 726e  ongs..    Return
+00007dd0: 733a 0a20 2020 2020 2020 202d 204e 6f6e  s:.        - Non
+00007de0: 653a 2054 6869 7320 6675 6e63 7469 6f6e  e: This function
+00007df0: 2064 6f65 7320 6e6f 7420 7265 7475 726e   does not return
+00007e00: 2061 6e79 2076 616c 7565 2e0a 2020 2020   any value..    
+00007e10: 5072 6f63 6573 7369 6e67 204c 6f67 6963  Processing Logic
+00007e20: 3a0a 2020 2020 2020 2020 2d20 4372 6561  :.        - Crea
+00007e30: 7465 7320 6120 6772 6964 2074 6974 6c65  tes a grid title
+00007e40: 2061 6e64 2061 6464 7320 6974 2074 6f20   and adds it to 
+00007e50: 7468 6520 7369 6465 6261 7220 6672 616d  the sidebar fram
+00007e60: 652e 0a20 2020 2020 2020 202d 2044 6566  e..        - Def
+00007e70: 696e 6573 2074 6865 2066 6972 7374 2067  ines the first g
+00007e80: 7269 6420 2f20 636f 6c75 6d6e 2066 6f72  rid / column for
+00007e90: 2064 6973 706c 6179 2064 6574 6169 6c20   display detail 
+00007ea0: 6c65 7665 6c2e 0a20 2020 2020 2020 202d  level..        -
+00007eb0: 2044 6566 696e 6573 2074 6865 2073 6563   Defines the sec
+00007ec0: 6f6e 6420 6772 6964 202f 2063 6f6c 756d  ond grid / colum
+00007ed0: 6e20 666f 7220 6368 6563 6b62 6f78 6573  n for checkboxes
+00007ee0: 2072 656c 6174 6564 2074 6f20 6469 7370   related to disp
+00007ef0: 6c61 7920 6f70 7469 6f6e 732e 0a20 2020  lay options..   
+00007f00: 2020 2020 202d 2044 6566 696e 6573 2074       - Defines t
+00007f10: 6865 2074 6869 7264 2067 7269 6420 2f20  he third grid / 
+00007f20: 636f 6c75 6d6e 2066 6f72 2062 7574 746f  column for butto
+00007f30: 6e73 2072 656c 6174 6564 2074 6f20 7072  ns related to pr
+00007f40: 6f67 7261 6d20 7365 7474 696e 6773 2e0a  ogram settings..
+00007f50: 2020 2020 2020 2020 2d20 4372 6561 7465          - Create
+00007f60: 7320 6120 7465 7874 626f 7820 666f 7220  s a textbox for 
+00007f70: 6469 7370 6c61 7969 6e67 2068 656c 7020  displaying help 
+00007f80: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
+00007f90: 2020 2020 202d 2043 7265 6174 6573 2061       - Creates a
+00007fa0: 2074 6162 7669 6577 2066 6f72 2073 6574   tabview for set
+00007fb0: 7469 6e67 2073 7065 6369 6669 6320 6e61  ting specific na
+00007fc0: 6d65 732c 2063 6f6c 6f72 732c 2061 6e64  mes, colors, and
+00007fd0: 2064 6562 7567 206f 7074 696f 6e73 2e0a   debug options..
+00007fe0: 2020 2020 2020 2020 2d20 4465 6669 6e65          - Define
+00007ff0: 7320 7468 6520 666f 7572 7468 2067 7269  s the fourth gri
+00008000: 6420 2f20 636f 6c75 6d6e 2066 6f72 2063  d / column for c
+00008010: 6865 636b 626f 7865 7320 7265 6c61 7465  heckboxes relate
+00008020: 6420 746f 2064 6562 7567 206f 7074 696f  d to debug optio
+00008030: 6e73 2e0a 2020 2020 2020 2020 2d20 4465  ns..        - De
+00008040: 6669 6e65 7320 7468 6520 7369 7874 6820  fines the sixth 
+00008050: 6772 6964 202f 2063 6f6c 756d 6e20 666f  grid / column fo
+00008060: 7220 6368 6563 6b62 6f78 6573 2072 656c  r checkboxes rel
+00008070: 6174 6564 2074 6f20 7275 6e74 696d 6520  ated to runtime 
+00008080: 7365 7474 696e 6773 2e22 2222 0a0a 2020  settings."""..  
+00008090: 2020 2320 4469 7370 6c61 7920 7468 6520    # Display the 
+000080a0: 6672 616d 6520 7469 746c 650a 2020 2020  frame title.    
+000080b0: 7365 6c66 2e6c 6f67 6f5f 6c61 6265 6c20  self.logo_label 
+000080c0: 3d20 6164 645f 6c61 6265 6c28 7365 6c66  = add_label(self
+000080d0: 2c20 7365 6c66 2e73 6964 6562 6172 5f66  , self.sidebar_f
+000080e0: 7261 6d65 2c20 2244 6973 706c 6179 204f  rame, "Display O
+000080f0: 7074 696f 6e73 222c 2022 222c 2032 302c  ptions", "", 20,
+00008100: 2022 626f 6c64 222c 2030 2c20 302c 2032   "bold", 0, 0, 2
+00008110: 302c 2028 3630 2c20 3130 292c 2022 7322  0, (60, 10), "s"
+00008120: 290a 0a20 2020 2023 2053 7461 7274 2066  )..    # Start f
+00008130: 6972 7374 2067 7269 6420 2f20 636f 6c75  irst grid / colu
+00008140: 6d6e 2064 6566 696e 6974 696f 6e73 0a0a  mn definitions..
+00008150: 2020 2020 2320 4469 7370 6c61 7920 4465      # Display De
+00008160: 7461 696c 204c 6576 656c 0a20 2020 2073  tail Level.    s
+00008170: 656c 662e 6465 7461 696c 5f6c 6162 656c  elf.detail_label
+00008180: 203d 2061 6464 5f6c 6162 656c 280a 2020   = add_label(.  
+00008190: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000081a0: 2020 2020 7365 6c66 2e73 6964 6562 6172      self.sidebar
+000081b0: 5f66 7261 6d65 2c0a 2020 2020 2020 2020  _frame,.        
+000081c0: 2244 6973 706c 6179 2044 6574 6169 6c20  "Display Detail 
+000081d0: 4c65 7665 6c3a 222c 0a20 2020 2020 2020  Level:",.       
+000081e0: 2022 222c 0a20 2020 2020 2020 2030 2c0a   "",.        0,.
+000081f0: 2020 2020 2020 2020 226e 6f72 6d61 6c22          "normal"
+00008200: 2c0a 2020 2020 2020 2020 312c 0a20 2020  ,.        1,.   
+00008210: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
+00008220: 3230 2c0a 2020 2020 2020 2020 2831 302c  20,.        (10,
+00008230: 2030 292c 0a20 2020 2020 2020 2022 222c   0),.        "",
+00008240: 0a20 2020 2029 0a20 2020 2073 656c 662e  .    ).    self.
+00008250: 7369 6465 6261 725f 6465 7461 696c 5f6f  sidebar_detail_o
+00008260: 7074 696f 6e20 3d20 6164 645f 6f70 7469  ption = add_opti
+00008270: 6f6e 5f6d 656e 7528 0a20 2020 2020 2020  on_menu(.       
+00008280: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
+00008290: 656c 662e 7369 6465 6261 725f 6672 616d  elf.sidebar_fram
+000082a0: 652c 0a20 2020 2020 2020 2073 656c 662e  e,.        self.
+000082b0: 6465 7461 696c 5f73 656c 6563 7465 645f  detail_selected_
+000082c0: 6576 656e 742c 0a20 2020 2020 2020 205b  event,.        [
+000082d0: 2230 222c 2022 3122 2c20 2232 222c 2022  "0", "1", "2", "
+000082e0: 3322 2c20 2234 225d 2c0a 2020 2020 2020  3", "4"],.      
+000082f0: 2020 322c 0a20 2020 2020 2020 2030 2c0a    2,.        0,.
+00008300: 2020 2020 2020 2020 3230 2c0a 2020 2020          20,.    
+00008310: 2020 2020 2831 302c 2031 3029 2c0a 2020      (10, 10),.  
+00008320: 2020 2020 2020 2222 2c0a 2020 2020 290a        "",.    ).
+00008330: 0a20 2020 2023 2044 6973 706c 6179 2027  .    # Display '
+00008340: 4576 6572 7974 6869 6e67 2720 6368 6563  Everything' chec
+00008350: 6b62 6f78 0a20 2020 2073 656c 662e 6576  kbox.    self.ev
+00008360: 6572 7974 6869 6e67 5f63 6865 636b 626f  erything_checkbo
+00008370: 7820 3d20 6164 645f 6368 6563 6b62 6f78  x = add_checkbox
+00008380: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00008390: 2020 2020 2020 2020 7365 6c66 2e73 6964          self.sid
+000083a0: 6562 6172 5f66 7261 6d65 2c0a 2020 2020  ebar_frame,.    
+000083b0: 2020 2020 7365 6c66 2e65 7665 7279 7468      self.everyth
+000083c0: 696e 675f 6576 656e 742c 0a20 2020 2020  ing_event,.     
+000083d0: 2020 2022 4a75 7374 2044 6973 706c 6179     "Just Display
+000083e0: 2045 7665 7279 7468 696e 6721 222c 0a20   Everything!",. 
+000083f0: 2020 2020 2020 2033 2c0a 2020 2020 2020         3,.      
+00008400: 2020 302c 0a20 2020 2020 2020 2032 302c    0,.        20,
+00008410: 0a20 2020 2020 2020 2031 302c 0a20 2020  .        10,.   
+00008420: 2020 2020 2022 7722 2c0a 2020 2020 2020       "w",.      
+00008430: 2020 2222 2c0a 2020 2020 290a 0a20 2020    "",.    )..   
+00008440: 2023 2044 6973 706c 6179 2027 436f 6e64   # Display 'Cond
+00008450: 6974 696f 6e27 2063 6865 636b 626f 780a  ition' checkbox.
+00008460: 2020 2020 7365 6c66 2e63 6f6e 6469 7469      self.conditi
+00008470: 6f6e 5f63 6865 636b 626f 7820 3d20 6164  on_checkbox = ad
+00008480: 645f 6368 6563 6b62 6f78 280a 2020 2020  d_checkbox(.    
+00008490: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000084a0: 2020 7365 6c66 2e73 6964 6562 6172 5f66    self.sidebar_f
+000084b0: 7261 6d65 2c0a 2020 2020 2020 2020 7365  rame,.        se
+000084c0: 6c66 2e63 6f6e 6469 7469 6f6e 5f65 7665  lf.condition_eve
+000084d0: 6e74 2c0a 2020 2020 2020 2020 2244 6973  nt,.        "Dis
+000084e0: 706c 6179 2050 726f 6669 6c65 2061 6e64  play Profile and
+000084f0: 2054 6173 6b20 4163 7469 6f6e 2043 6f6e   Task Action Con
+00008500: 6469 7469 6f6e 7322 2c0a 2020 2020 2020  ditions",.      
+00008510: 2020 342c 0a20 2020 2020 2020 2030 2c0a    4,.        0,.
+00008520: 2020 2020 2020 2020 3230 2c0a 2020 2020          20,.    
+00008530: 2020 2020 3130 2c0a 2020 2020 2020 2020      10,.        
+00008540: 2277 222c 0a20 2020 2020 2020 2022 222c  "w",.        "",
+00008550: 0a20 2020 2029 0a0a 2020 2020 2320 4469  .    )..    # Di
+00008560: 7370 6c61 7920 2754 6173 6b65 724e 6574  splay 'TaskerNet
+00008570: 2720 6368 6563 6b62 6f78 0a20 2020 2073  ' checkbox.    s
+00008580: 656c 662e 7461 736b 6572 6e65 745f 6368  elf.taskernet_ch
+00008590: 6563 6b62 6f78 203d 2061 6464 5f63 6865  eckbox = add_che
+000085a0: 636b 626f 7828 0a20 2020 2020 2020 2073  ckbox(.        s
+000085b0: 656c 662c 0a20 2020 2020 2020 2073 656c  elf,.        sel
+000085c0: 662e 7369 6465 6261 725f 6672 616d 652c  f.sidebar_frame,
+000085d0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+000085e0: 736b 6572 6e65 745f 6576 656e 742c 0a20  skernet_event,. 
 000085f0: 2020 2020 2020 2022 4469 7370 6c61 7920         "Display 
-00008600: 4465 7461 696c 204c 6576 656c 3a22 2c0a  Detail Level:",.
-00008610: 2020 2020 2020 2020 2222 2c0a 2020 2020          "",.    
-00008620: 2020 2020 302c 0a20 2020 2020 2020 2022      0,.        "
-00008630: 6e6f 726d 616c 222c 0a20 2020 2020 2020  normal",.       
-00008640: 2031 2c0a 2020 2020 2020 2020 302c 0a20   1,.        0,. 
-00008650: 2020 2020 2020 2032 302c 0a20 2020 2020         20,.     
-00008660: 2020 2028 3130 2c20 3029 2c0a 2020 2020     (10, 0),.    
-00008670: 2020 2020 2222 2c0a 2020 2020 290a 2020      "",.    ).  
-00008680: 2020 7365 6c66 2e73 6964 6562 6172 5f64    self.sidebar_d
-00008690: 6574 6169 6c5f 6f70 7469 6f6e 203d 2061  etail_option = a
-000086a0: 6464 5f6f 7074 696f 6e5f 6d65 6e75 280a  dd_option_menu(.
-000086b0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000086c0: 2020 2020 2020 7365 6c66 2e73 6964 6562        self.sideb
-000086d0: 6172 5f66 7261 6d65 2c0a 2020 2020 2020  ar_frame,.      
-000086e0: 2020 7365 6c66 2e64 6574 6169 6c5f 7365    self.detail_se
-000086f0: 6c65 6374 6564 5f65 7665 6e74 2c0a 2020  lected_event,.  
-00008700: 2020 2020 2020 5b22 3022 2c20 2231 222c        ["0", "1",
-00008710: 2022 3222 2c20 2233 222c 2022 3422 5d2c   "2", "3", "4"],
-00008720: 0a20 2020 2020 2020 2032 2c0a 2020 2020  .        2,.    
-00008730: 2020 2020 302c 0a20 2020 2020 2020 2032      0,.        2
-00008740: 302c 0a20 2020 2020 2020 2028 3130 2c20  0,.        (10, 
-00008750: 3130 292c 0a20 2020 2020 2020 2022 222c  10),.        "",
-00008760: 0a20 2020 2029 0a0a 2020 2020 2320 4469  .    )..    # Di
-00008770: 7370 6c61 7920 2745 7665 7279 7468 696e  splay 'Everythin
-00008780: 6727 2063 6865 636b 626f 780a 2020 2020  g' checkbox.    
-00008790: 7365 6c66 2e65 7665 7279 7468 696e 675f  self.everything_
-000087a0: 6368 6563 6b62 6f78 203d 2061 6464 5f63  checkbox = add_c
-000087b0: 6865 636b 626f 7828 0a20 2020 2020 2020  heckbox(.       
-000087c0: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
-000087d0: 656c 662e 7369 6465 6261 725f 6672 616d  elf.sidebar_fram
-000087e0: 652c 0a20 2020 2020 2020 2073 656c 662e  e,.        self.
-000087f0: 6576 6572 7974 6869 6e67 5f65 7665 6e74  everything_event
-00008800: 2c0a 2020 2020 2020 2020 224a 7573 7420  ,.        "Just 
-00008810: 4469 7370 6c61 7920 4576 6572 7974 6869  Display Everythi
-00008820: 6e67 2122 2c0a 2020 2020 2020 2020 332c  ng!",.        3,
-00008830: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
-00008840: 2020 2020 3230 2c0a 2020 2020 2020 2020      20,.        
-00008850: 3130 2c0a 2020 2020 2020 2020 2277 222c  10,.        "w",
-00008860: 0a20 2020 2020 2020 2022 222c 0a20 2020  .        "",.   
-00008870: 2029 0a0a 2020 2020 2320 4469 7370 6c61   )..    # Displa
-00008880: 7920 2743 6f6e 6469 7469 6f6e 2720 6368  y 'Condition' ch
-00008890: 6563 6b62 6f78 0a20 2020 2073 656c 662e  eckbox.    self.
-000088a0: 636f 6e64 6974 696f 6e5f 6368 6563 6b62  condition_checkb
-000088b0: 6f78 203d 2061 6464 5f63 6865 636b 626f  ox = add_checkbo
-000088c0: 7828 0a20 2020 2020 2020 2073 656c 662c  x(.        self,
-000088d0: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
-000088e0: 6465 6261 725f 6672 616d 652c 0a20 2020  debar_frame,.   
-000088f0: 2020 2020 2073 656c 662e 636f 6e64 6974       self.condit
-00008900: 696f 6e5f 6576 656e 742c 0a20 2020 2020  ion_event,.     
-00008910: 2020 2022 4469 7370 6c61 7920 5072 6f66     "Display Prof
-00008920: 696c 6520 616e 6420 5461 736b 2041 6374  ile and Task Act
-00008930: 696f 6e20 436f 6e64 6974 696f 6e73 222c  ion Conditions",
-00008940: 0a20 2020 2020 2020 2034 2c0a 2020 2020  .        4,.    
-00008950: 2020 2020 302c 0a20 2020 2020 2020 2032      0,.        2
-00008960: 302c 0a20 2020 2020 2020 2031 302c 0a20  0,.        10,. 
-00008970: 2020 2020 2020 2022 7722 2c0a 2020 2020         "w",.    
-00008980: 2020 2020 2222 2c0a 2020 2020 290a 0a20      "",.    ).. 
-00008990: 2020 2023 2044 6973 706c 6179 2027 5461     # Display 'Ta
-000089a0: 736b 6572 4e65 7427 2063 6865 636b 626f  skerNet' checkbo
-000089b0: 780a 2020 2020 7365 6c66 2e74 6173 6b65  x.    self.taske
-000089c0: 726e 6574 5f63 6865 636b 626f 7820 3d20  rnet_checkbox = 
-000089d0: 6164 645f 6368 6563 6b62 6f78 280a 2020  add_checkbox(.  
-000089e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000089f0: 2020 2020 7365 6c66 2e73 6964 6562 6172      self.sidebar
-00008a00: 5f66 7261 6d65 2c0a 2020 2020 2020 2020  _frame,.        
-00008a10: 7365 6c66 2e74 6173 6b65 726e 6574 5f65  self.taskernet_e
-00008a20: 7665 6e74 2c0a 2020 2020 2020 2020 2244  vent,.        "D
-00008a30: 6973 706c 6179 2054 6173 6b65 724e 6574  isplay TaskerNet
-00008a40: 2049 6e66 6f22 2c0a 2020 2020 2020 2020   Info",.        
-00008a50: 352c 0a20 2020 2020 2020 2030 2c0a 2020  5,.        0,.  
-00008a60: 2020 2020 2020 3230 2c0a 2020 2020 2020        20,.      
-00008a70: 2020 3130 2c0a 2020 2020 2020 2020 2277    10,.        "w
-00008a80: 222c 0a20 2020 2020 2020 2022 222c 0a20  ",.        "",. 
-00008a90: 2020 2029 0a0a 2020 2020 2320 4469 7370     )..    # Disp
-00008aa0: 6c61 7920 2754 6173 6b65 7220 5072 6566  lay 'Tasker Pref
-00008ab0: 6572 656e 6365 7327 2063 6865 636b 626f  erences' checkbo
-00008ac0: 780a 2020 2020 7365 6c66 2e70 7265 6665  x.    self.prefe
-00008ad0: 7265 6e63 6573 5f63 6865 636b 626f 7820  rences_checkbox 
-00008ae0: 3d20 6164 645f 6368 6563 6b62 6f78 280a  = add_checkbox(.
-00008af0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00008b00: 2020 2020 2020 7365 6c66 2e73 6964 6562        self.sideb
-00008b10: 6172 5f66 7261 6d65 2c0a 2020 2020 2020  ar_frame,.      
-00008b20: 2020 7365 6c66 2e70 7265 6665 7265 6e63    self.preferenc
-00008b30: 6573 5f65 7665 6e74 2c0a 2020 2020 2020  es_event,.      
-00008b40: 2020 2244 6973 706c 6179 2054 6173 6b65    "Display Taske
-00008b50: 7220 5072 6566 6572 656e 6365 7322 2c0a  r Preferences",.
-00008b60: 2020 2020 2020 2020 362c 0a20 2020 2020          6,.     
-00008b70: 2020 2030 2c0a 2020 2020 2020 2020 3230     0,.        20
-00008b80: 2c0a 2020 2020 2020 2020 3130 2c0a 2020  ,.        10,.  
-00008b90: 2020 2020 2020 2277 222c 0a20 2020 2020        "w",.     
-00008ba0: 2020 2022 222c 0a20 2020 2029 0a0a 2020     "",.    )..  
-00008bb0: 2020 2320 4469 7370 6c61 7920 2754 7769    # Display 'Twi
-00008bc0: 7374 7927 2063 6865 636b 626f 780a 2020  sty' checkbox.  
-00008bd0: 2020 7365 6c66 2e74 7769 7374 795f 6368    self.twisty_ch
-00008be0: 6563 6b62 6f78 203d 2061 6464 5f63 6865  eckbox = add_che
-00008bf0: 636b 626f 7828 0a20 2020 2020 2020 2073  ckbox(.        s
-00008c00: 656c 662c 0a20 2020 2020 2020 2073 656c  elf,.        sel
-00008c10: 662e 7369 6465 6261 725f 6672 616d 652c  f.sidebar_frame,
-00008c20: 0a20 2020 2020 2020 2073 656c 662e 7477  .        self.tw
-00008c30: 6973 7479 5f65 7665 6e74 2c0a 2020 2020  isty_event,.    
-00008c40: 2020 2020 2248 6964 6520 5461 736b 2044      "Hide Task D
-00008c50: 6574 6169 6c73 2055 6e64 6572 2054 7769  etails Under Twi
-00008c60: 7374 7922 2c0a 2020 2020 2020 2020 372c  sty",.        7,
-00008c70: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
-00008c80: 2020 2020 3230 2c0a 2020 2020 2020 2020      20,.        
-00008c90: 3130 2c0a 2020 2020 2020 2020 2277 222c  10,.        "w",
-00008ca0: 0a20 2020 2020 2020 2022 222c 0a20 2020  .        "",.   
-00008cb0: 2029 0a0a 2020 2020 2320 4469 7370 6c61   )..    # Displa
-00008cc0: 7920 2764 6972 6563 746f 7279 2720 6368  y 'directory' ch
-00008cd0: 6563 6b62 6f78 0a20 2020 2073 656c 662e  eckbox.    self.
-00008ce0: 6469 7265 6374 6f72 795f 6368 6563 6b62  directory_checkb
-00008cf0: 6f78 203d 2061 6464 5f63 6865 636b 626f  ox = add_checkbo
-00008d00: 7828 0a20 2020 2020 2020 2073 656c 662c  x(.        self,
-00008d10: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
-00008d20: 6465 6261 725f 6672 616d 652c 0a20 2020  debar_frame,.   
-00008d30: 2020 2020 2073 656c 662e 6469 7265 6374       self.direct
-00008d40: 6f72 795f 6576 656e 742c 0a20 2020 2020  ory_event,.     
-00008d50: 2020 2022 4469 7370 6c61 7920 4469 7265     "Display Dire
-00008d60: 6374 6f72 7922 2c0a 2020 2020 2020 2020  ctory",.        
-00008d70: 382c 0a20 2020 2020 2020 2030 2c0a 2020  8,.        0,.  
-00008d80: 2020 2020 2020 3230 2c0a 2020 2020 2020        20,.      
-00008d90: 2020 3130 2c0a 2020 2020 2020 2020 2277    10,.        "w
-00008da0: 222c 0a20 2020 2020 2020 2022 222c 0a20  ",.        "",. 
-00008db0: 2020 2029 0a0a 2020 2020 2320 4f75 746c     )..    # Outl
-00008dc0: 696e 650a 2020 2020 7365 6c66 2e6f 7574  ine.    self.out
-00008dd0: 6c69 6e65 5f63 6865 636b 626f 7820 3d20  line_checkbox = 
-00008de0: 6164 645f 6368 6563 6b62 6f78 280a 2020  add_checkbox(.  
-00008df0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00008e00: 2020 2020 7365 6c66 2e73 6964 6562 6172      self.sidebar
-00008e10: 5f66 7261 6d65 2c0a 2020 2020 2020 2020  _frame,.        
-00008e20: 7365 6c66 2e6f 7574 6c69 6e65 5f65 7665  self.outline_eve
-00008e30: 6e74 2c0a 2020 2020 2020 2020 2244 6973  nt,.        "Dis
-00008e40: 706c 6179 2043 6f6e 6669 6775 7261 7469  play Configurati
-00008e50: 6f6e 204f 7574 6c69 6e65 222c 0a20 2020  on Outline",.   
-00008e60: 2020 2020 2039 2c0a 2020 2020 2020 2020       9,.        
-00008e70: 302c 0a20 2020 2020 2020 2032 302c 0a20  0,.        20,. 
-00008e80: 2020 2020 2020 2031 302c 0a20 2020 2020         10,.     
-00008e90: 2020 2022 7722 2c0a 2020 2020 2020 2020     "w",.        
-00008ea0: 2222 2c0a 2020 2020 290a 0a20 2020 2023  "",.    )..    #
-00008eb0: 2050 7265 7474 7920 4f75 7470 7574 0a20   Pretty Output. 
-00008ec0: 2020 2073 656c 662e 7072 6574 7479 5f63     self.pretty_c
-00008ed0: 6865 636b 626f 7820 3d20 6164 645f 6368  heckbox = add_ch
-00008ee0: 6563 6b62 6f78 280a 2020 2020 2020 2020  eckbox(.        
-00008ef0: 7365 6c66 2c0a 2020 2020 2020 2020 7365  self,.        se
-00008f00: 6c66 2e73 6964 6562 6172 5f66 7261 6d65  lf.sidebar_frame
-00008f10: 2c0a 2020 2020 2020 2020 7365 6c66 2e70  ,.        self.p
-00008f20: 7265 7474 795f 6576 656e 742c 0a20 2020  retty_event,.   
-00008f30: 2020 2020 2022 4469 7370 6c61 7920 5072       "Display Pr
-00008f40: 6574 7469 6572 204f 7574 7075 7422 2c0a  ettier Output",.
-00008f50: 2020 2020 2020 2020 3130 2c0a 2020 2020          10,.    
-00008f60: 2020 2020 302c 0a20 2020 2020 2020 2032      0,.        2
-00008f70: 302c 0a20 2020 2020 2020 2031 302c 0a20  0,.        10,. 
-00008f80: 2020 2020 2020 2022 7722 2c0a 2020 2020         "w",.    
-00008f90: 2020 2020 2222 2c0a 2020 2020 290a 0a20      "",.    ).. 
-00008fa0: 2020 2023 204e 616d 6573 3a20 426f 6c64     # Names: Bold
-00008fb0: 202f 2048 6967 686c 6967 6874 202f 2049   / Highlight / I
-00008fc0: 7461 6c69 6369 7365 202f 2055 6e64 6572  talicise / Under
-00008fd0: 6c69 6e65 0a20 2020 2073 656c 662e 6469  line.    self.di
-00008fe0: 7370 6c61 795f 6e61 6d65 735f 6c61 6265  splay_names_labe
-00008ff0: 6c20 3d20 6164 645f 6c61 6265 6c28 0a20  l = add_label(. 
-00009000: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00009010: 2020 2020 2073 656c 662e 7369 6465 6261       self.sideba
-00009020: 725f 6672 616d 652c 0a20 2020 2020 2020  r_frame,.       
-00009030: 2022 5072 6f6a 6563 742f 5072 6f66 696c   "Project/Profil
-00009040: 652f 5461 736b 2f53 6365 6e65 204e 616d  e/Task/Scene Nam
-00009050: 6573 3a22 2c0a 2020 2020 2020 2020 2222  es:",.        ""
-00009060: 2c0a 2020 2020 2020 2020 302c 0a20 2020  ,.        0,.   
-00009070: 2020 2020 2022 6e6f 726d 616c 222c 0a20       "normal",. 
-00009080: 2020 2020 2020 2031 312c 0a20 2020 2020         11,.     
-00009090: 2020 2030 2c0a 2020 2020 2020 2020 3230     0,.        20
-000090a0: 2c0a 2020 2020 2020 2020 3130 2c0a 2020  ,.        10,.  
-000090b0: 2020 2020 2020 2273 222c 0a20 2020 2029        "s",.    )
-000090c0: 0a0a 2020 2020 2320 426f 6c64 0a20 2020  ..    # Bold.   
-000090d0: 2073 656c 662e 626f 6c64 5f63 6865 636b   self.bold_check
-000090e0: 626f 7820 3d20 6164 645f 6368 6563 6b62  box = add_checkb
-000090f0: 6f78 2873 656c 662c 2073 656c 662e 7369  ox(self, self.si
-00009100: 6465 6261 725f 6672 616d 652c 2073 656c  debar_frame, sel
-00009110: 662e 6e61 6d65 735f 626f 6c64 5f65 7665  f.names_bold_eve
-00009120: 6e74 2c20 2242 6f6c 6422 2c20 3132 2c20  nt, "Bold", 12, 
-00009130: 302c 2032 302c 2030 2c20 226e 6522 2c20  0, 20, 0, "ne", 
-00009140: 2222 290a 0a20 2020 2023 2049 7461 6c69  "")..    # Itali
-00009150: 6369 7a65 0a20 2020 2073 656c 662e 6974  cize.    self.it
-00009160: 616c 6963 697a 655f 6368 6563 6b62 6f78  alicize_checkbox
-00009170: 203d 2061 6464 5f63 6865 636b 626f 7828   = add_checkbox(
-00009180: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00009190: 2020 2020 2020 2073 656c 662e 7369 6465         self.side
-000091a0: 6261 725f 6672 616d 652c 0a20 2020 2020  bar_frame,.     
-000091b0: 2020 2073 656c 662e 6e61 6d65 735f 6974     self.names_it
-000091c0: 616c 6963 697a 655f 6576 656e 742c 0a20  alicize_event,. 
-000091d0: 2020 2020 2020 2022 6974 616c 6963 697a         "italiciz
-000091e0: 6522 2c0a 2020 2020 2020 2020 3132 2c0a  e",.        12,.
-000091f0: 2020 2020 2020 2020 302c 0a20 2020 2020          0,.     
-00009200: 2020 2032 302c 0a20 2020 2020 2020 2030     20,.        0
-00009210: 2c0a 2020 2020 2020 2020 226e 7722 2c0a  ,.        "nw",.
-00009220: 2020 2020 2020 2020 2222 2c0a 2020 2020          "",.    
-00009230: 290a 0a20 2020 2023 2048 6967 686c 6967  )..    # Highlig
-00009240: 6874 0a20 2020 2073 656c 662e 6869 6768  ht.    self.high
-00009250: 6c69 6768 745f 6368 6563 6b62 6f78 203d  light_checkbox =
-00009260: 2061 6464 5f63 6865 636b 626f 7828 0a20   add_checkbox(. 
-00009270: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00009280: 2020 2020 2073 656c 662e 7369 6465 6261       self.sideba
-00009290: 725f 6672 616d 652c 0a20 2020 2020 2020  r_frame,.       
-000092a0: 2073 656c 662e 6e61 6d65 735f 6869 6768   self.names_high
-000092b0: 6c69 6768 745f 6576 656e 742c 0a20 2020  light_event,.   
-000092c0: 2020 2020 2022 4869 6768 6c69 6768 7422       "Highlight"
-000092d0: 2c0a 2020 2020 2020 2020 3133 2c0a 2020  ,.        13,.  
-000092e0: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
-000092f0: 2032 302c 0a20 2020 2020 2020 2035 2c0a   20,.        5,.
-00009300: 2020 2020 2020 2020 226e 6522 2c0a 2020          "ne",.  
-00009310: 2020 2020 2020 2222 2c0a 2020 2020 290a        "",.    ).
-00009320: 0a20 2020 2023 2055 6e64 6572 6c69 6e65  .    # Underline
-00009330: 0a20 2020 2073 656c 662e 756e 6465 726c  .    self.underl
-00009340: 696e 655f 6368 6563 6b62 6f78 203d 2061  ine_checkbox = a
-00009350: 6464 5f63 6865 636b 626f 7828 0a20 2020  dd_checkbox(.   
-00009360: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00009370: 2020 2073 656c 662e 7369 6465 6261 725f     self.sidebar_
-00009380: 6672 616d 652c 0a20 2020 2020 2020 2073  frame,.        s
-00009390: 656c 662e 6e61 6d65 735f 756e 6465 726c  elf.names_underl
-000093a0: 696e 655f 6576 656e 742c 0a20 2020 2020  ine_event,.     
-000093b0: 2020 2022 556e 6465 726c 696e 6522 2c0a     "Underline",.
-000093c0: 2020 2020 2020 2020 3133 2c0a 2020 2020          13,.    
-000093d0: 2020 2020 302c 0a20 2020 2020 2020 2032      0,.        2
-000093e0: 302c 0a20 2020 2020 2020 2035 2c0a 2020  0,.        5,.  
-000093f0: 2020 2020 2020 226e 7722 2c0a 2020 2020        "nw",.    
-00009400: 2020 2020 2222 2c0a 2020 2020 290a 0a20      "",.    ).. 
-00009410: 2020 2023 2049 6e64 656e 7461 7469 6f6e     # Indentation
-00009420: 0a20 2020 2073 656c 662e 696e 6465 6e74  .    self.indent
-00009430: 5f6c 6162 656c 203d 2061 6464 5f6c 6162  _label = add_lab
-00009440: 656c 280a 2020 2020 2020 2020 7365 6c66  el(.        self
-00009450: 2c0a 2020 2020 2020 2020 7365 6c66 2e73  ,.        self.s
-00009460: 6964 6562 6172 5f66 7261 6d65 2c0a 2020  idebar_frame,.  
-00009470: 2020 2020 2020 2249 662f 5468 656e 2f45        "If/Then/E
-00009480: 6c73 6520 496e 6465 6e74 6174 696f 6e20  lse Indentation 
-00009490: 416d 6f75 6e74 3a22 2c0a 2020 2020 2020  Amount:",.      
-000094a0: 2020 2222 2c0a 2020 2020 2020 2020 302c    "",.        0,
-000094b0: 0a20 2020 2020 2020 2022 6e6f 726d 616c  .        "normal
-000094c0: 222c 0a20 2020 2020 2020 2031 342c 0a20  ",.        14,. 
-000094d0: 2020 2020 2020 2030 2c0a 2020 2020 2020         0,.      
-000094e0: 2020 3230 2c0a 2020 2020 2020 2020 3130    20,.        10
-000094f0: 2c0a 2020 2020 2020 2020 2273 222c 0a20  ,.        "s",. 
-00009500: 2020 2029 0a0a 2020 2020 2320 496e 6465     )..    # Inde
-00009510: 6e74 6174 696f 6e20 416d 6f75 6e74 0a20  ntation Amount. 
-00009520: 2020 2073 656c 662e 696e 6465 6e74 5f6f     self.indent_o
-00009530: 7074 696f 6e20 3d20 6164 645f 6f70 7469  ption = add_opti
-00009540: 6f6e 5f6d 656e 7528 0a20 2020 2020 2020  on_menu(.       
-00009550: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
-00009560: 656c 662e 7369 6465 6261 725f 6672 616d  elf.sidebar_fram
-00009570: 652c 0a20 2020 2020 2020 2073 656c 662e  e,.        self.
-00009580: 696e 6465 6e74 5f73 656c 6563 7465 645f  indent_selected_
-00009590: 6576 656e 742c 0a20 2020 2020 2020 205b  event,.        [
-000095a0: 2230 222c 2022 3122 2c20 2232 222c 2022  "0", "1", "2", "
-000095b0: 3322 2c20 2234 222c 2022 3522 2c20 2236  3", "4", "5", "6
-000095c0: 222c 2022 3722 2c20 2238 222c 2022 3922  ", "7", "8", "9"
-000095d0: 2c20 2231 3022 5d2c 0a20 2020 2020 2020  , "10"],.       
-000095e0: 2031 352c 0a20 2020 2020 2020 2030 2c0a   15,.        0,.
-000095f0: 2020 2020 2020 2020 302c 0a20 2020 2020          0,.     
-00009600: 2020 2028 302c 2031 3029 2c0a 2020 2020     (0, 10),.    
-00009610: 2020 2020 226e 222c 0a20 2020 2029 0a0a      "n",.    )..
-00009620: 2020 2020 2320 5363 7265 656e 2041 7070      # Screen App
-00009630: 6561 7261 6e63 653a 204c 6967 6874 202f  earance: Light /
-00009640: 2044 6172 6b20 2f20 5379 7374 656d 0a20   Dark / System. 
-00009650: 2020 2073 656c 662e 6170 7065 6172 616e     self.appearan
-00009660: 6365 5f6d 6f64 655f 6c61 6265 6c20 3d20  ce_mode_label = 
-00009670: 6164 645f 6c61 6265 6c28 0a20 2020 2020  add_label(.     
-00009680: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00009690: 2073 656c 662e 7369 6465 6261 725f 6672   self.sidebar_fr
-000096a0: 616d 652c 0a20 2020 2020 2020 2022 4170  ame,.        "Ap
-000096b0: 7065 6172 616e 6365 204d 6f64 653a 222c  pearance Mode:",
-000096c0: 0a20 2020 2020 2020 2022 222c 0a20 2020  .        "",.   
-000096d0: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
-000096e0: 226e 6f72 6d61 6c22 2c0a 2020 2020 2020  "normal",.      
-000096f0: 2020 3136 2c0a 2020 2020 2020 2020 302c    16,.        0,
-00009700: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
-00009710: 2020 2020 2831 302c 2030 292c 0a20 2020      (10, 0),.   
-00009720: 2020 2020 2022 7322 2c0a 2020 2020 290a       "s",.    ).
-00009730: 0a20 2020 2073 656c 662e 6170 7065 6172  .    self.appear
-00009740: 616e 6365 5f6d 6f64 655f 6f70 7469 6f6e  ance_mode_option
-00009750: 656d 656e 7520 3d20 6164 645f 6f70 7469  emenu = add_opti
-00009760: 6f6e 5f6d 656e 7528 0a20 2020 2020 2020  on_menu(.       
-00009770: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
-00009780: 656c 662e 7369 6465 6261 725f 6672 616d  elf.sidebar_fram
-00009790: 652c 0a20 2020 2020 2020 2073 656c 662e  e,.        self.
-000097a0: 6368 616e 6765 5f61 7070 6561 7261 6e63  change_appearanc
-000097b0: 655f 6d6f 6465 5f65 7665 6e74 2c0a 2020  e_mode_event,.  
-000097c0: 2020 2020 2020 5b22 4c69 6768 7422 2c20        ["Light", 
-000097d0: 2244 6172 6b22 2c20 2253 7973 7465 6d22  "Dark", "System"
-000097e0: 5d2c 0a20 2020 2020 2020 2031 372c 0a20  ],.        17,. 
-000097f0: 2020 2020 2020 2030 2c0a 2020 2020 2020         0,.      
-00009800: 2020 302c 0a20 2020 2020 2020 2028 302c    0,.        (0,
-00009810: 2031 3029 2c0a 2020 2020 2020 2020 226e   10),.        "n
-00009820: 222c 0a20 2020 2029 0a0a 2020 2020 2320  ",.    )..    # 
-00009830: 2754 7265 6520 5669 6577 2720 6275 7474  'Tree View' butt
-00009840: 6f6e 2064 6566 696e 6974 696f 6e0a 2020  on definition.  
-00009850: 2020 7365 6c66 2e74 7265 6576 6965 775f    self.treeview_
-00009860: 6275 7474 6f6e 203d 2061 6464 5f62 7574  button = add_but
-00009870: 746f 6e28 0a20 2020 2020 2020 2073 656c  ton(.        sel
-00009880: 662c 0a20 2020 2020 2020 2073 656c 662e  f,.        self.
-00009890: 7369 6465 6261 725f 6672 616d 652c 0a20  sidebar_frame,. 
-000098a0: 2020 2020 2020 2022 2332 3436 4642 3622         "#246FB6"
-000098b0: 2c0a 2020 2020 2020 2020 2222 2c0a 2020  ,.        "",.  
-000098c0: 2020 2020 2020 2222 2c0a 2020 2020 2020        "",.      
-000098d0: 2020 7365 6c66 2e74 7265 6576 6965 775f    self.treeview_
-000098e0: 6576 656e 742c 0a20 2020 2020 2020 2032  event,.        2
-000098f0: 2c0a 2020 2020 2020 2020 2254 7265 6520  ,.        "Tree 
-00009900: 5669 6577 222c 0a20 2020 2020 2020 2031  View",.        1
-00009910: 2c0a 2020 2020 2020 2020 3138 2c0a 2020  ,.        18,.  
-00009920: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
-00009930: 2030 2c0a 2020 2020 2020 2020 302c 0a20   0,.        0,. 
-00009940: 2020 2020 2020 2022 222c 0a20 2020 2029         "",.    )
-00009950: 0a20 2020 2023 2020 5175 6572 7920 3f20  .    #  Query ? 
-00009960: 6275 7474 6f6e 0a20 2020 2073 656c 662e  button.    self.
-00009970: 7472 6565 7669 6577 5f71 7565 7279 5f62  treeview_query_b
-00009980: 7574 746f 6e20 3d20 6164 645f 6275 7474  utton = add_butt
-00009990: 6f6e 280a 2020 2020 2020 2020 7365 6c66  on(.        self
-000099a0: 2c0a 2020 2020 2020 2020 7365 6c66 2e73  ,.        self.s
-000099b0: 6964 6562 6172 5f66 7261 6d65 2c0a 2020  idebar_frame,.  
-000099c0: 2020 2020 2020 2223 3234 3646 4236 222c        "#246FB6",
-000099d0: 0a20 2020 2020 2020 2028 2223 3042 4630  .        ("#0BF0
-000099e0: 3735 222c 2022 2366 6664 3934 3122 292c  75", "#ffd941"),
-000099f0: 0a20 2020 2020 2020 2022 2331 6263 3966  .        "#1bc9f
-00009a00: 6622 2c0a 2020 2020 2020 2020 7365 6c66  f",.        self
-00009a10: 2e74 7265 6576 6965 775f 7175 6572 795f  .treeview_query_
-00009a20: 6576 656e 742c 0a20 2020 2020 2020 2031  event,.        1
-00009a30: 2c0a 2020 2020 2020 2020 223f 222c 0a20  ,.        "?",. 
-00009a40: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
-00009a50: 2020 3138 2c0a 2020 2020 2020 2020 302c    18,.        0,
-00009a60: 0a20 2020 2020 2020 2028 3230 302c 2030  .        (200, 0
-00009a70: 292c 0a20 2020 2020 2020 2028 302c 2030  ),.        (0, 0
-00009a80: 292c 0a20 2020 2020 2020 2022 222c 0a20  ),.        "",. 
-00009a90: 2020 2029 0a20 2020 2073 656c 662e 7472     ).    self.tr
-00009aa0: 6565 7669 6577 5f71 7565 7279 5f62 7574  eeview_query_but
-00009ab0: 746f 6e2e 636f 6e66 6967 7572 6528 7769  ton.configure(wi
-00009ac0: 6474 683d 3230 290a 0a20 2020 2023 2027  dth=20)..    # '
-00009ad0: 5265 7365 7420 5365 7474 696e 6773 2720  Reset Settings' 
-00009ae0: 6275 7474 6f6e 2064 6566 696e 6974 696f  button definitio
-00009af0: 6e0a 2020 2020 7365 6c66 2e72 6573 6574  n.    self.reset
-00009b00: 5f62 7574 746f 6e20 3d20 6164 645f 6275  _button = add_bu
-00009b10: 7474 6f6e 280a 2020 2020 2020 2020 7365  tton(.        se
-00009b20: 6c66 2c0a 2020 2020 2020 2020 7365 6c66  lf,.        self
-00009b30: 2e73 6964 6562 6172 5f66 7261 6d65 2c0a  .sidebar_frame,.
-00009b40: 2020 2020 2020 2020 2223 3234 3646 4236          "#246FB6
-00009b50: 222c 0a20 2020 2020 2020 2022 222c 0a20  ",.        "",. 
-00009b60: 2020 2020 2020 2022 222c 0a20 2020 2020         "",.     
-00009b70: 2020 2073 656c 662e 7265 7365 745f 7365     self.reset_se
-00009b80: 7474 696e 6773 5f65 7665 6e74 2c0a 2020  ttings_event,.  
-00009b90: 2020 2020 2020 322c 0a20 2020 2020 2020        2,.       
-00009ba0: 2022 5265 7365 7420 4f70 7469 6f6e 7322   "Reset Options"
-00009bb0: 2c0a 2020 2020 2020 2020 312c 0a20 2020  ,.        1,.   
-00009bc0: 2020 2020 2031 392c 0a20 2020 2020 2020       19,.       
-00009bd0: 2030 2c0a 2020 2020 2020 2020 3230 2c0a   0,.        20,.
-00009be0: 2020 2020 2020 2020 3230 2c0a 2020 2020          20,.    
-00009bf0: 2020 2020 2273 222c 0a20 2020 2029 0a0a      "s",.    )..
-00009c00: 2020 2020 2320 5374 6172 7420 7365 636f      # Start seco
-00009c10: 6e64 2067 7269 6420 2f20 636f 6c75 6d6e  nd grid / column
-00009c20: 2064 6566 696e 6974 696f 6e73 0a0a 2020   definitions..  
-00009c30: 2020 2320 466f 6e74 2074 6f20 7573 650a    # Font to use.
-00009c40: 2020 2020 7365 6c66 2e66 6f6e 745f 6c61      self.font_la
-00009c50: 6265 6c20 3d20 6164 645f 6c61 6265 6c28  bel = add_label(
-00009c60: 7365 6c66 2c20 7365 6c66 2c20 2246 6f6e  self, self, "Fon
-00009c70: 7420 546f 2055 7365 2049 6e20 4f75 7470  t To Use In Outp
-00009c80: 7574 3a22 2c20 2222 2c20 302c 2022 6e6f  ut:", "", 0, "no
-00009c90: 726d 616c 222c 2036 2c20 312c 2032 302c  rmal", 6, 1, 20,
-00009ca0: 2031 302c 2022 7377 2229 0a0a 2020 2020   10, "sw")..    
-00009cb0: 2320 4765 7420 666f 6e74 7320 6672 6f6d  # Get fonts from
-00009cc0: 2054 6b49 6e74 6572 0a20 2020 2066 6f6e   TkInter.    fon
-00009cd0: 745f 6974 656d 732c 2072 6573 203d 2067  t_items, res = g
-00009ce0: 6574 5f6d 6f6e 6f73 7061 6365 5f66 6f6e  et_monospace_fon
-00009cf0: 7473 2829 0a20 2020 2023 2044 656c 6574  ts().    # Delet
-00009d00: 6520 7468 6520 746b 726f 6f74 206f 6274  e the tkroot obt
-00009d10: 6169 6e65 6420 6279 2067 6574 5f6d 6f6e  ained by get_mon
-00009d20: 6f73 7061 6365 5f66 6f6e 7473 0a20 2020  ospace_fonts.   
-00009d30: 2069 6620 5072 696d 6549 7465 6d73 2e74   if PrimeItems.t
-00009d40: 6b72 6f6f 7420 6973 206e 6f74 204e 6f6e  kroot is not Non
-00009d50: 653a 0a20 2020 2020 2020 2064 656c 2050  e:.        del P
-00009d60: 7269 6d65 4974 656d 732e 746b 726f 6f74  rimeItems.tkroot
-00009d70: 0a20 2020 2020 2020 2050 7269 6d65 4974  .        PrimeIt
-00009d80: 656d 732e 746b 726f 6f74 203d 204e 6f6e  ems.tkroot = Non
-00009d90: 650a 2020 2020 7365 6c66 2e66 6f6e 745f  e.    self.font_
-00009da0: 6f70 7469 6f6e 656d 656e 7520 3d20 6164  optionemenu = ad
-00009db0: 645f 6f70 7469 6f6e 5f6d 656e 7528 0a20  d_option_menu(. 
-00009dc0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00009dd0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00009de0: 2020 2073 656c 662e 666f 6e74 5f65 7665     self.font_eve
-00009df0: 6e74 2c0a 2020 2020 2020 2020 666f 6e74  nt,.        font
-00009e00: 5f69 7465 6d73 2c0a 2020 2020 2020 2020  _items,.        
-00009e10: 372c 0a20 2020 2020 2020 2031 2c0a 2020  7,.        1,.  
-00009e20: 2020 2020 2020 3230 2c0a 2020 2020 2020        20,.      
-00009e30: 2020 302c 0a20 2020 2020 2020 2022 6e77    0,.        "nw
-00009e40: 222c 0a20 2020 2029 0a20 2020 2073 656c  ",.    ).    sel
-00009e50: 662e 666f 6e74 5f6f 7074 696f 6e65 6d65  f.font_optioneme
-00009e60: 6e75 2e73 6574 2872 6573 5b30 5d29 0a0a  nu.set(res[0])..
-00009e70: 2020 2020 2320 5361 7665 2073 6574 7469      # Save setti
-00009e80: 6e67 7320 6275 7474 6f6e 0a20 2020 2073  ngs button.    s
-00009e90: 656c 662e 7361 7665 5f73 6574 7469 6e67  elf.save_setting
-00009ea0: 735f 6275 7474 6f6e 203d 2061 6464 5f62  s_button = add_b
-00009eb0: 7574 746f 6e28 0a20 2020 2020 2020 2073  utton(.        s
-00009ec0: 656c 662c 0a20 2020 2020 2020 2073 656c  elf,.        sel
-00009ed0: 662c 0a20 2020 2020 2020 2022 2336 3536  f,.        "#656
-00009ee0: 3366 6622 2c0a 2020 2020 2020 2020 2222  3ff",.        ""
-00009ef0: 2c0a 2020 2020 2020 2020 2222 2c0a 2020  ,.        "",.  
-00009f00: 2020 2020 2020 7365 6c66 2e73 6176 655f        self.save_
-00009f10: 7365 7474 696e 6773 5f65 7665 6e74 2c0a  settings_event,.
-00009f20: 2020 2020 2020 2020 322c 0a20 2020 2020          2,.     
-00009f30: 2020 2022 5361 7665 2053 6574 7469 6e67     "Save Setting
-00009f40: 7322 2c0a 2020 2020 2020 2020 312c 0a20  s",.        1,. 
-00009f50: 2020 2020 2020 2038 2c0a 2020 2020 2020         8,.      
-00009f60: 2020 312c 0a20 2020 2020 2020 2032 302c    1,.        20,
-00009f70: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
-00009f80: 2020 2020 2273 7722 2c0a 2020 2020 290a      "sw",.    ).
-00009f90: 0a20 2020 2023 2052 6573 746f 7265 2073  .    # Restore s
-00009fa0: 6574 7469 6e67 7320 6275 7474 6f6e 0a20  ettings button. 
-00009fb0: 2020 2073 656c 662e 7265 7374 6f72 655f     self.restore_
-00009fc0: 7365 7474 696e 6773 5f62 7574 746f 6e20  settings_button 
-00009fd0: 3d20 6164 645f 6275 7474 6f6e 280a 2020  = add_button(.  
-00009fe0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00009ff0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000a000: 2020 2223 3635 3633 6666 222c 0a20 2020    "#6563ff",.   
-0000a010: 2020 2020 2022 222c 0a20 2020 2020 2020       "",.       
-0000a020: 2022 222c 0a20 2020 2020 2020 2073 656c   "",.        sel
-0000a030: 662e 7265 7374 6f72 655f 7365 7474 696e  f.restore_settin
-0000a040: 6773 5f65 7665 6e74 2c0a 2020 2020 2020  gs_event,.      
-0000a050: 2020 322c 0a20 2020 2020 2020 2022 5265    2,.        "Re
-0000a060: 7374 6f72 6520 5365 7474 696e 6773 222c  store Settings",
-0000a070: 0a20 2020 2020 2020 2031 2c0a 2020 2020  .        1,.    
-0000a080: 2020 2020 392c 0a20 2020 2020 2020 2031      9,.        1
-0000a090: 2c0a 2020 2020 2020 2020 3230 2c0a 2020  ,.        20,.  
-0000a0a0: 2020 2020 2020 3130 2c0a 2020 2020 2020        10,.      
-0000a0b0: 2020 226e 7722 2c0a 2020 2020 290a 0a20    "nw",.    ).. 
-0000a0c0: 2020 2023 2052 6570 6f72 7420 4973 7375     # Report Issu
-0000a0d0: 650a 2020 2020 7365 6c66 2e72 6570 6f72  e.    self.repor
-0000a0e0: 745f 6973 7375 655f 6275 7474 6f6e 203d  t_issue_button =
-0000a0f0: 2061 6464 5f62 7574 746f 6e28 0a20 2020   add_button(.   
-0000a100: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000a110: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000a120: 2022 222c 0a20 2020 2020 2020 2022 222c   "",.        "",
-0000a130: 0a20 2020 2020 2020 2022 222c 0a20 2020  .        "",.   
-0000a140: 2020 2020 2073 656c 662e 7265 706f 7274       self.report
-0000a150: 5f69 7373 7565 5f65 7665 6e74 2c0a 2020  _issue_event,.  
-0000a160: 2020 2020 2020 322c 0a20 2020 2020 2020        2,.       
-0000a170: 2022 5265 706f 7274 2049 7373 7565 222c   "Report Issue",
-0000a180: 0a20 2020 2020 2020 2031 2c0a 2020 2020  .        1,.    
-0000a190: 2020 2020 3130 2c0a 2020 2020 2020 2020      10,.        
-0000a1a0: 312c 0a20 2020 2020 2020 2032 302c 0a20  1,.        20,. 
-0000a1b0: 2020 2020 2020 2030 2c0a 2020 2020 2020         0,.      
-0000a1c0: 2020 226e 7722 2c0a 2020 2020 290a 0a20    "nw",.    ).. 
-0000a1d0: 2020 2023 2027 436c 6561 7220 4d65 7373     # 'Clear Mess
-0000a1e0: 6167 6573 2720 6275 7474 6f6e 2064 6566  ages' button def
-0000a1f0: 696e 6974 696f 6e0a 2020 2020 7365 6c66  inition.    self
-0000a200: 2e72 6573 6574 5f62 7574 746f 6e20 3d20  .reset_button = 
-0000a210: 6164 645f 6275 7474 6f6e 280a 2020 2020  add_button(.    
-0000a220: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000a230: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000a240: 2223 3234 3646 4236 222c 0a20 2020 2020  "#246FB6",.     
-0000a250: 2020 2022 222c 0a20 2020 2020 2020 2022     "",.        "
-0000a260: 222c 0a20 2020 2020 2020 2073 656c 662e  ",.        self.
-0000a270: 636c 6561 725f 6d65 7373 6167 6573 5f65  clear_messages_e
-0000a280: 7665 6e74 2c0a 2020 2020 2020 2020 322c  vent,.        2,
-0000a290: 0a20 2020 2020 2020 2022 436c 6561 7220  .        "Clear 
-0000a2a0: 4d65 7373 6167 6573 222c 0a20 2020 2020  Messages",.     
-0000a2b0: 2020 2031 2c0a 2020 2020 2020 2020 352c     1,.        5,
-0000a2c0: 0a20 2020 2020 2020 2031 2c0a 2020 2020  .        1,.    
-0000a2d0: 2020 2020 302c 0a20 2020 2020 2020 2030      0,.        0
-0000a2e0: 2c0a 2020 2020 2020 2020 2273 222c 0a20  ,.        "s",. 
-0000a2f0: 2020 2029 0a20 2020 2023 2027 4765 7420     ).    # 'Get 
-0000a300: 4261 636b 7570 2053 6574 7469 6e67 7327  Backup Settings'
-0000a310: 2062 7574 746f 6e20 6465 6669 6e69 7469   button definiti
-0000a320: 6f6e 0a20 2020 2073 656c 662e 6765 745f  on.    self.get_
-0000a330: 6261 636b 7570 5f62 7574 746f 6e20 3d20  backup_button = 
-0000a340: 7365 6c66 2e64 6973 706c 6179 5f62 6163  self.display_bac
-0000a350: 6b75 705f 6275 7474 6f6e 280a 2020 2020  kup_button(.    
-0000a360: 2020 2020 2247 6574 2058 4d4c 2066 726f      "Get XML fro
-0000a370: 6d20 416e 6472 6f69 6420 4465 7669 6365  m Android Device
-0000a380: 222c 0a20 2020 2020 2020 2022 2332 3436  ",.        "#246
-0000a390: 4642 3622 2c0a 2020 2020 2020 2020 2223  FB6",.        "#
-0000a3a0: 3635 3633 6666 222c 0a20 2020 2020 2020  6563ff",.       
-0000a3b0: 2073 656c 662e 6765 745f 6261 636b 7570   self.get_backup
-0000a3c0: 5f65 7665 6e74 2c0a 2020 2020 290a 2020  _event,.    ).  
-0000a3d0: 2020 2320 2747 6574 206c 6f63 616c 2058    # 'Get local X
-0000a3e0: 4d4c 2720 6275 7474 6f6e 0a20 2020 2073  ML' button.    s
-0000a3f0: 656c 662e 6765 7478 6d6c 5f62 7574 746f  elf.getxml_butto
-0000a400: 6e20 3d20 6164 645f 6275 7474 6f6e 280a  n = add_button(.
-0000a410: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000a420: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000a430: 2020 2020 2222 2c0a 2020 2020 2020 2020      "",.        
-0000a440: 2222 2c0a 2020 2020 2020 2020 2222 2c0a  "",.        "",.
-0000a450: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
-0000a460: 786d 6c5f 6576 656e 742c 0a20 2020 2020  xml_event,.     
-0000a470: 2020 2032 2c0a 2020 2020 2020 2020 2247     2,.        "G
-0000a480: 6574 204c 6f63 616c 2058 4d4c 222c 0a20  et Local XML",. 
-0000a490: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
-0000a4a0: 2020 362c 0a20 2020 2020 2020 2032 2c0a    6,.        2,.
-0000a4b0: 2020 2020 2020 2020 2832 302c 2032 3029          (20, 20)
-0000a4c0: 2c0a 2020 2020 2020 2020 2831 302c 2031  ,.        (10, 1
-0000a4d0: 3029 2c0a 2020 2020 2020 2020 2265 222c  0),.        "e",
-0000a4e0: 0a20 2020 2029 0a0a 2020 2020 2320 2744  .    )..    # 'D
-0000a4f0: 6973 706c 6179 2048 656c 7027 2062 7574  isplay Help' but
-0000a500: 746f 6e20 6465 6669 6e69 7469 6f6e 0a20  ton definition. 
-0000a510: 2020 2073 656c 662e 6865 6c70 5f62 7574     self.help_but
-0000a520: 746f 6e20 3d20 6164 645f 6275 7474 6f6e  ton = add_button
-0000a530: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000a540: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000a550: 2020 2020 2020 2223 3234 3646 4236 222c        "#246FB6",
-0000a560: 0a20 2020 2020 2020 2028 2223 3042 4630  .        ("#0BF0
-0000a570: 3735 222c 2022 2366 6664 3934 3122 292c  75", "#ffd941"),
-0000a580: 0a20 2020 2020 2020 2022 222c 0a20 2020  .        "",.   
-0000a590: 2020 2020 2073 656c 662e 6865 6c70 5f65       self.help_e
-0000a5a0: 7665 6e74 2c0a 2020 2020 2020 2020 322c  vent,.        2,
-0000a5b0: 0a20 2020 2020 2020 2022 4469 7370 6c61  .        "Displa
-0000a5c0: 7920 4865 6c70 222c 0a20 2020 2020 2020  y Help",.       
-0000a5d0: 2031 2c0a 2020 2020 2020 2020 372c 0a20   1,.        7,. 
-0000a5e0: 2020 2020 2020 2032 2c0a 2020 2020 2020         2,.      
-0000a5f0: 2020 2830 2c20 3230 292c 0a20 2020 2020    (0, 20),.     
-0000a600: 2020 2028 3130 2c20 3529 2c0a 2020 2020     (10, 5),.    
-0000a610: 2020 2020 2273 6522 2c0a 2020 2020 290a      "se",.    ).
-0000a620: 0a20 2020 2023 2027 4261 636b 7570 2048  .    # 'Backup H
-0000a630: 656c 7027 2062 7574 746f 6e20 6465 6669  elp' button defi
-0000a640: 6e69 7469 6f6e 0a20 2020 2073 656c 662e  nition.    self.
-0000a650: 6261 636b 7570 5f68 656c 705f 6275 7474  backup_help_butt
-0000a660: 6f6e 203d 2061 6464 5f62 7574 746f 6e28  on = add_button(
-0000a670: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0000a680: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000a690: 2020 2020 2022 2332 3436 4642 3622 2c0a       "#246FB6",.
-0000a6a0: 2020 2020 2020 2020 2822 2330 4246 3037          ("#0BF07
-0000a6b0: 3522 2c20 2223 6666 6439 3431 2229 2c0a  5", "#ffd941"),.
-0000a6c0: 2020 2020 2020 2020 2222 2c0a 2020 2020          "",.    
-0000a6d0: 2020 2020 7365 6c66 2e62 6163 6b75 705f      self.backup_
-0000a6e0: 6865 6c70 5f65 7665 6e74 2c0a 2020 2020  help_event,.    
-0000a6f0: 2020 2020 322c 0a20 2020 2020 2020 2022      2,.        "
-0000a700: 4765 7420 416e 6472 6f69 6420 4865 6c70  Get Android Help
-0000a710: 222c 0a20 2020 2020 2020 2031 2c0a 2020  ",.        1,.  
-0000a720: 2020 2020 2020 382c 0a20 2020 2020 2020        8,.       
-0000a730: 2032 2c0a 2020 2020 2020 2020 2830 2c20   2,.        (0, 
-0000a740: 3230 292c 0a20 2020 2020 2020 2028 352c  20),.        (5,
-0000a750: 2031 3029 2c0a 2020 2020 2020 2020 226e   10),.        "n
-0000a760: 6522 2c0a 2020 2020 290a 0a20 2020 2023  e",.    )..    #
-0000a770: 2027 5275 6e27 2062 7574 746f 6e20 6465   'Run' button de
-0000a780: 6669 6e69 7469 6f6e 0a20 2020 2073 656c  finition.    sel
-0000a790: 662e 7275 6e5f 6275 7474 6f6e 203d 2061  f.run_button = a
-0000a7a0: 6464 5f62 7574 746f 6e28 0a20 2020 2020  dd_button(.     
-0000a7b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000a7c0: 2073 656c 662c 0a20 2020 2020 2020 2022   self,.        "
-0000a7d0: 2332 3436 4642 3622 2c0a 2020 2020 2020  #246FB6",.      
-0000a7e0: 2020 2822 2330 4246 3037 3522 2c20 2223    ("#0BF075", "#
-0000a7f0: 3141 4436 3344 2229 2c0a 2020 2020 2020  1AD63D"),.      
-0000a800: 2020 2222 2c0a 2020 2020 2020 2020 7365    "",.        se
-0000a810: 6c66 2e72 756e 5f70 726f 6772 616d 2c0a  lf.run_program,.
-0000a820: 2020 2020 2020 2020 322c 0a20 2020 2020          2,.     
-0000a830: 2020 2022 5275 6e20 616e 6420 4578 6974     "Run and Exit
-0000a840: 222c 0a20 2020 2020 2020 2031 2c0a 2020  ",.        1,.  
-0000a850: 2020 2020 2020 392c 0a20 2020 2020 2020        9,.       
-0000a860: 2032 2c0a 2020 2020 2020 2020 2830 2c20   2,.        (0, 
-0000a870: 3230 292c 0a20 2020 2020 2020 2028 3130  20),.        (10
-0000a880: 2c20 3529 2c0a 2020 2020 2020 2020 2273  , 5),.        "s
-0000a890: 6522 2c0a 2020 2020 290a 0a20 2020 2023  e",.    )..    #
-0000a8a0: 2027 5265 5275 6e27 2062 7574 746f 6e20   'ReRun' button 
-0000a8b0: 6465 6669 6e69 7469 6f6e 0a20 2020 2073  definition.    s
-0000a8c0: 656c 662e 7265 7275 6e5f 6275 7474 6f6e  elf.rerun_button
-0000a8d0: 203d 2061 6464 5f62 7574 746f 6e28 0a20   = add_button(. 
-0000a8e0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000a8f0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000a900: 2020 2022 2332 3436 4642 3622 2c0a 2020     "#246FB6",.  
-0000a910: 2020 2020 2020 2822 2330 4246 3037 3522        ("#0BF075"
-0000a920: 2c20 2223 3141 4436 3344 2229 2c0a 2020  , "#1AD63D"),.  
-0000a930: 2020 2020 2020 2222 2c0a 2020 2020 2020        "",.      
-0000a940: 2020 7365 6c66 2e72 6572 756e 5f74 6865    self.rerun_the
-0000a950: 5f70 726f 6772 616d 2c0a 2020 2020 2020  _program,.      
-0000a960: 2020 322c 0a20 2020 2020 2020 2022 5265    2,.        "Re
-0000a970: 5275 6e22 2c0a 2020 2020 2020 2020 312c  Run",.        1,
-0000a980: 0a20 2020 2020 2020 2031 302c 0a20 2020  .        10,.   
-0000a990: 2020 2020 2032 2c0a 2020 2020 2020 2020       2,.        
-0000a9a0: 2830 2c20 3230 292c 0a20 2020 2020 2020  (0, 20),.       
-0000a9b0: 2028 352c 2031 3029 2c0a 2020 2020 2020   (5, 10),.      
-0000a9c0: 2020 226e 6522 2c0a 2020 2020 290a 0a20    "ne",.    ).. 
-0000a9d0: 2020 2023 2027 4578 6974 2720 6275 7474     # 'Exit' butt
-0000a9e0: 6f6e 2064 6566 696e 6974 696f 6e0a 2020  on definition.  
-0000a9f0: 2020 7365 6c66 2e65 7869 745f 6275 7474    self.exit_butt
-0000aa00: 6f6e 203d 2061 6464 5f62 7574 746f 6e28  on = add_button(
-0000aa10: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0000aa20: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000aa30: 2020 2020 2022 2332 3436 4642 3622 2c0a       "#246FB6",.
-0000aa40: 2020 2020 2020 2020 2252 6564 222c 0a20          "Red",. 
-0000aa50: 2020 2020 2020 2022 222c 0a20 2020 2020         "",.     
-0000aa60: 2020 2073 656c 662e 6578 6974 5f70 726f     self.exit_pro
-0000aa70: 6772 616d 2c0a 2020 2020 2020 2020 322c  gram,.        2,
-0000aa80: 0a20 2020 2020 2020 2022 4578 6974 222c  .        "Exit",
-0000aa90: 0a20 2020 2020 2020 2031 2c0a 2020 2020  .        1,.    
-0000aaa0: 2020 2020 3131 2c0a 2020 2020 2020 2020      11,.        
-0000aab0: 322c 0a20 2020 2020 2020 2028 3230 2c20  2,.        (20, 
-0000aac0: 3230 292c 0a20 2020 2020 2020 2028 3230  20),.        (20
-0000aad0: 2c20 3230 292c 0a20 2020 2020 2020 2022  , 20),.        "
-0000aae0: 6e65 222c 0a20 2020 2029 0a0a 2020 2020  ne",.    )..    
-0000aaf0: 2320 4372 6561 7465 2074 6578 7462 6f78  # Create textbox
-0000ab00: 2066 6f72 2048 656c 7020 696e 666f 726d   for Help inform
-0000ab10: 6174 696f 6e0a 2020 2020 7365 6c66 2e74  ation.    self.t
-0000ab20: 6578 7462 6f78 203d 2063 746b 2e43 546b  extbox = ctk.CTk
-0000ab30: 5465 7874 626f 7828 7365 6c66 2c20 6865  Textbox(self, he
-0000ab40: 6967 6874 3d36 3030 2c20 7769 6474 683d  ight=600, width=
-0000ab50: 3235 3029 0a20 2020 2073 656c 662e 7465  250).    self.te
-0000ab60: 7874 626f 782e 636f 6e66 6967 7572 6528  xtbox.configure(
-0000ab70: 7363 726f 6c6c 6261 725f 6275 7474 6f6e  scrollbar_button
-0000ab80: 5f63 6f6c 6f72 3d22 2336 3536 3366 6622  _color="#6563ff"
-0000ab90: 2c20 7772 6170 3d22 776f 7264 2229 0a20  , wrap="word"). 
-0000aba0: 2020 2073 656c 662e 7465 7874 626f 782e     self.textbox.
-0000abb0: 6772 6964 2872 6f77 3d30 2c20 636f 6c75  grid(row=0, colu
-0000abc0: 6d6e 3d31 2c20 7061 6478 3d28 3230 2c20  mn=1, padx=(20, 
-0000abd0: 3029 2c20 7061 6479 3d28 3230 2c20 3029  0), pady=(20, 0)
-0000abe0: 2c20 7374 6963 6b79 3d22 6577 2229 0a0a  , sticky="ew")..
-0000abf0: 2020 2020 2320 5374 6172 7420 7468 6972      # Start thir
-0000ac00: 6420 6772 6964 202f 2063 6f6c 756d 6e20  d grid / column 
-0000ac10: 6465 6669 6e69 7469 6f6e 730a 2020 2020  definitions.    
-0000ac20: 2320 6372 6561 7465 2074 6162 7669 6577  # create tabview
-0000ac30: 2066 6f72 204e 616d 652c 2043 6f6c 6f72   for Name, Color
-0000ac40: 2c20 616e 6420 4465 6275 670a 2020 2020  , and Debug.    
-0000ac50: 7365 6c66 2e74 6162 7669 6577 203d 2063  self.tabview = c
-0000ac60: 746b 2e43 546b 5461 6276 6965 7728 7365  tk.CTkTabview(se
-0000ac70: 6c66 2c20 7769 6474 683d 3235 302c 2073  lf, width=250, s
-0000ac80: 6567 6d65 6e74 6564 5f62 7574 746f 6e5f  egmented_button_
-0000ac90: 6667 5f63 6f6c 6f72 3d22 2336 3536 3366  fg_color="#6563f
-0000aca0: 6622 290a 2020 2020 7365 6c66 2e74 6162  f").    self.tab
-0000acb0: 7669 6577 2e67 7269 6428 726f 773d 302c  view.grid(row=0,
-0000acc0: 2063 6f6c 756d 6e3d 322c 2070 6164 783d   column=2, padx=
-0000acd0: 2832 302c 2030 292c 2070 6164 793d 2832  (20, 0), pady=(2
-0000ace0: 302c 2030 292c 2073 7469 636b 793d 226e  0, 0), sticky="n
-0000acf0: 7365 7722 290a 2020 2020 7365 6c66 2e74  sew").    self.t
-0000ad00: 6162 7669 6577 2e61 6464 2822 5370 6563  abview.add("Spec
-0000ad10: 6966 6963 204e 616d 6522 290a 2020 2020  ific Name").    
-0000ad20: 7365 6c66 2e74 6162 7669 6577 2e61 6464  self.tabview.add
-0000ad30: 2822 436f 6c6f 7273 2229 0a20 2020 2073  ("Colors").    s
-0000ad40: 656c 662e 7461 6276 6965 772e 6164 6428  elf.tabview.add(
-0000ad50: 2241 6e61 6c79 7a65 2229 0a20 2020 2073  "Analyze").    s
-0000ad60: 656c 662e 7461 6276 6965 772e 6164 6428  elf.tabview.add(
-0000ad70: 2244 6562 7567 2229 0a0a 2020 2020 7365  "Debug")..    se
-0000ad80: 6c66 2e74 6162 7669 6577 2e74 6162 2822  lf.tabview.tab("
-0000ad90: 5370 6563 6966 6963 204e 616d 6522 292e  Specific Name").
-0000ada0: 6772 6964 5f63 6f6c 756d 6e63 6f6e 6669  grid_columnconfi
-0000adb0: 6775 7265 2830 2c20 7765 6967 6874 3d31  gure(0, weight=1
-0000adc0: 2920 2023 2063 6f6e 6669 6775 7265 2067  )  # configure g
-0000add0: 7269 6420 6f66 2069 6e64 6976 6964 7561  rid of individua
-0000ade0: 6c20 7461 6273 0a20 2020 2073 656c 662e  l tabs.    self.
-0000adf0: 7461 6276 6965 772e 7461 6228 2243 6f6c  tabview.tab("Col
-0000ae00: 6f72 7322 292e 6772 6964 5f63 6f6c 756d  ors").grid_colum
-0000ae10: 6e63 6f6e 6669 6775 7265 2830 2c20 7765  nconfigure(0, we
-0000ae20: 6967 6874 3d31 290a 0a20 2020 2023 2050  ight=1)..    # P
-0000ae30: 726f 6a65 6374 204e 616d 650a 2020 2020  roject Name.    
-0000ae40: 7365 6c66 2e73 7472 696e 675f 696e 7075  self.string_inpu
-0000ae50: 745f 6275 7474 6f6e 3120 3d20 6374 6b2e  t_button1 = ctk.
-0000ae60: 4354 6b52 6164 696f 4275 7474 6f6e 280a  CTkRadioButton(.
-0000ae70: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
-0000ae80: 7669 6577 2e74 6162 2822 5370 6563 6966  view.tab("Specif
-0000ae90: 6963 204e 616d 6522 292c 0a20 2020 2020  ic Name"),.     
-0000aea0: 2020 2074 6578 743d 2250 726f 6a65 6374     text="Project
-0000aeb0: 204e 616d 6522 2c0a 2020 2020 2020 2020   Name",.        
-0000aec0: 666f 6e74 3d63 746b 2e43 546b 466f 6e74  font=ctk.CTkFont
-0000aed0: 2873 697a 653d 6465 6661 756c 745f 666f  (size=default_fo
-0000aee0: 6e74 5f73 697a 652c 2077 6569 6768 743d  nt_size, weight=
-0000aef0: 226e 6f72 6d61 6c22 292c 0a20 2020 2020  "normal"),.     
-0000af00: 2020 2063 6f6d 6d61 6e64 3d73 656c 662e     command=self.
-0000af10: 7369 6e67 6c65 5f70 726f 6a65 6374 5f6e  single_project_n
-0000af20: 616d 655f 6576 656e 742c 0a20 2020 2020  ame_event,.     
-0000af30: 2020 2066 675f 636f 6c6f 723d 2223 3635     fg_color="#65
-0000af40: 3633 6666 222c 0a20 2020 2020 2020 2062  63ff",.        b
-0000af50: 6f72 6465 725f 636f 6c6f 723d 2223 3162  order_color="#1b
-0000af60: 6339 6666 222c 0a20 2020 2029 0a20 2020  c9ff",.    ).   
-0000af70: 2073 656c 662e 7374 7269 6e67 5f69 6e70   self.string_inp
-0000af80: 7574 5f62 7574 746f 6e31 2e67 7269 6428  ut_button1.grid(
-0000af90: 726f 773d 312c 2063 6f6c 756d 6e3d 302c  row=1, column=0,
-0000afa0: 2070 6164 783d 3230 2c20 7061 6479 3d28   padx=20, pady=(
-0000afb0: 3130 2c20 3130 292c 2073 7469 636b 793d  10, 10), sticky=
-0000afc0: 226e 7365 7722 290a 0a20 2020 2023 2050  "nsew")..    # P
-0000afd0: 726f 6669 6c65 204e 616d 650a 2020 2020  rofile Name.    
-0000afe0: 7365 6c66 2e73 7472 696e 675f 696e 7075  self.string_inpu
-0000aff0: 745f 6275 7474 6f6e 3220 3d20 6374 6b2e  t_button2 = ctk.
-0000b000: 4354 6b52 6164 696f 4275 7474 6f6e 280a  CTkRadioButton(.
-0000b010: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
-0000b020: 7669 6577 2e74 6162 2822 5370 6563 6966  view.tab("Specif
-0000b030: 6963 204e 616d 6522 292c 0a20 2020 2020  ic Name"),.     
-0000b040: 2020 2074 6578 743d 2250 726f 6669 6c65     text="Profile
-0000b050: 204e 616d 6522 2c0a 2020 2020 2020 2020   Name",.        
-0000b060: 666f 6e74 3d63 746b 2e43 546b 466f 6e74  font=ctk.CTkFont
-0000b070: 2873 697a 653d 6465 6661 756c 745f 666f  (size=default_fo
-0000b080: 6e74 5f73 697a 652c 2077 6569 6768 743d  nt_size, weight=
-0000b090: 226e 6f72 6d61 6c22 292c 0a20 2020 2020  "normal"),.     
-0000b0a0: 2020 2063 6f6d 6d61 6e64 3d73 656c 662e     command=self.
-0000b0b0: 7369 6e67 6c65 5f70 726f 6669 6c65 5f6e  single_profile_n
-0000b0c0: 616d 655f 6576 656e 742c 0a20 2020 2020  ame_event,.     
-0000b0d0: 2020 2066 675f 636f 6c6f 723d 2223 3635     fg_color="#65
-0000b0e0: 3633 6666 222c 0a20 2020 2020 2020 2062  63ff",.        b
-0000b0f0: 6f72 6465 725f 636f 6c6f 723d 2223 3162  order_color="#1b
-0000b100: 6339 6666 222c 0a20 2020 2029 0a20 2020  c9ff",.    ).   
-0000b110: 2073 656c 662e 7374 7269 6e67 5f69 6e70   self.string_inp
-0000b120: 7574 5f62 7574 746f 6e32 2e67 7269 6428  ut_button2.grid(
-0000b130: 726f 773d 322c 2063 6f6c 756d 6e3d 302c  row=2, column=0,
-0000b140: 2070 6164 783d 3230 2c20 7061 6479 3d28   padx=20, pady=(
-0000b150: 3130 2c20 3130 292c 2073 7469 636b 793d  10, 10), sticky=
-0000b160: 226e 7365 7722 290a 0a20 2020 2023 2054  "nsew")..    # T
-0000b170: 6173 6b20 4e61 6d65 0a20 2020 2073 656c  ask Name.    sel
-0000b180: 662e 7374 7269 6e67 5f69 6e70 7574 5f62  f.string_input_b
-0000b190: 7574 746f 6e33 203d 2063 746b 2e43 546b  utton3 = ctk.CTk
-0000b1a0: 5261 6469 6f42 7574 746f 6e28 0a20 2020  RadioButton(.   
-0000b1b0: 2020 2020 2073 656c 662e 7461 6276 6965       self.tabvie
-0000b1c0: 772e 7461 6228 2253 7065 6369 6669 6320  w.tab("Specific 
-0000b1d0: 4e61 6d65 2229 2c0a 2020 2020 2020 2020  Name"),.        
-0000b1e0: 7465 7874 3d22 5461 736b 204e 616d 6522  text="Task Name"
-0000b1f0: 2c0a 2020 2020 2020 2020 666f 6e74 3d63  ,.        font=c
-0000b200: 746b 2e43 546b 466f 6e74 2873 697a 653d  tk.CTkFont(size=
-0000b210: 6465 6661 756c 745f 666f 6e74 5f73 697a  default_font_siz
-0000b220: 652c 2077 6569 6768 743d 226e 6f72 6d61  e, weight="norma
-0000b230: 6c22 292c 0a20 2020 2020 2020 2063 6f6d  l"),.        com
-0000b240: 6d61 6e64 3d73 656c 662e 7369 6e67 6c65  mand=self.single
-0000b250: 5f74 6173 6b5f 6e61 6d65 5f65 7665 6e74  _task_name_event
-0000b260: 2c0a 2020 2020 2020 2020 6667 5f63 6f6c  ,.        fg_col
-0000b270: 6f72 3d22 2336 3536 3366 6622 2c0a 2020  or="#6563ff",.  
-0000b280: 2020 2020 2020 626f 7264 6572 5f63 6f6c        border_col
-0000b290: 6f72 3d22 2331 6263 3966 6622 2c0a 2020  or="#1bc9ff",.  
-0000b2a0: 2020 290a 2020 2020 7365 6c66 2e73 7472    ).    self.str
-0000b2b0: 696e 675f 696e 7075 745f 6275 7474 6f6e  ing_input_button
-0000b2c0: 332e 6772 6964 2872 6f77 3d33 2c20 636f  3.grid(row=3, co
-0000b2d0: 6c75 6d6e 3d30 2c20 7061 6478 3d32 302c  lumn=0, padx=20,
-0000b2e0: 2070 6164 793d 2831 302c 2031 3029 2c20   pady=(10, 10), 
-0000b2f0: 7374 6963 6b79 3d22 6e73 6577 2229 0a0a  sticky="nsew")..
-0000b300: 2020 2020 2320 5072 6f6d 7074 2066 6f72      # Prompt for
-0000b310: 2074 6865 206e 616d 650a 2020 2020 7365   the name.    se
-0000b320: 6c66 2e6e 616d 655f 6c61 6265 6c20 3d20  lf.name_label = 
-0000b330: 6164 645f 6c61 6265 6c28 0a20 2020 2020  add_label(.     
-0000b340: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000b350: 2073 656c 662e 7461 6276 6965 772e 7461   self.tabview.ta
-0000b360: 6228 2253 7065 6369 6669 6320 4e61 6d65  b("Specific Name
-0000b370: 2229 2c0a 2020 2020 2020 2020 2228 5069  "),.        "(Pi
-0000b380: 636b 204f 4e4c 5920 4f6e 6529 222c 0a20  ck ONLY One)",. 
-0000b390: 2020 2020 2020 2022 222c 0a20 2020 2020         "",.     
-0000b3a0: 2020 2030 2c0a 2020 2020 2020 2020 226e     0,.        "n
-0000b3b0: 6f72 6d61 6c22 2c0a 2020 2020 2020 2020  ormal",.        
-0000b3c0: 342c 0a20 2020 2020 2020 2030 2c0a 2020  4,.        0,.  
-0000b3d0: 2020 2020 2020 3230 2c0a 2020 2020 2020        20,.      
-0000b3e0: 2020 2831 302c 2031 3029 2c0a 2020 2020    (10, 10),.    
-0000b3f0: 2020 2020 2277 222c 0a20 2020 2029 0a0a      "w",.    )..
-0000b400: 2020 2020 2320 5365 7475 7020 746f 2067      # Setup to g
-0000b410: 6574 2076 6172 696f 7573 2064 6973 706c  et various displ
-0000b420: 6179 2063 6f6c 6f72 730a 2020 2020 7365  ay colors.    se
-0000b430: 6c66 2e6c 6162 656c 5f74 6162 5f32 203d  lf.label_tab_2 =
-0000b440: 2061 6464 5f6c 6162 656c 280a 2020 2020   add_label(.    
-0000b450: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000b460: 2020 7365 6c66 2e74 6162 7669 6577 2e74    self.tabview.t
-0000b470: 6162 2822 5370 6563 6966 6963 204e 616d  ab("Specific Nam
-0000b480: 6522 292c 0a20 2020 2020 2020 2022 5365  e"),.        "Se
-0000b490: 7420 5661 7269 6f75 7320 4469 7370 6c61  t Various Displa
-0000b4a0: 7920 436f 6c6f 7273 2048 6572 653a 222c  y Colors Here:",
-0000b4b0: 0a20 2020 2020 2020 2022 222c 0a20 2020  .        "",.   
-0000b4c0: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
-0000b4d0: 226e 6f72 6d61 6c22 2c0a 2020 2020 2020  "normal",.      
-0000b4e0: 2020 302c 0a20 2020 2020 2020 2030 2c0a    0,.        0,.
-0000b4f0: 2020 2020 2020 2020 302c 0a20 2020 2020          0,.     
-0000b500: 2020 2030 2c0a 2020 2020 2020 2020 2222     0,.        ""
-0000b510: 2c0a 2020 2020 290a 2020 2020 7365 6c66  ,.    ).    self
-0000b520: 2e63 6f6c 6f72 735f 6f70 7469 6f6e 656d  .colors_optionem
-0000b530: 656e 7520 3d20 6164 645f 6f70 7469 6f6e  enu = add_option
-0000b540: 5f6d 656e 7528 0a20 2020 2020 2020 2073  _menu(.        s
-0000b550: 656c 662c 0a20 2020 2020 2020 2073 656c  elf,.        sel
-0000b560: 662e 7461 6276 6965 772e 7461 6228 2243  f.tabview.tab("C
-0000b570: 6f6c 6f72 7322 292c 0a20 2020 2020 2020  olors"),.       
-0000b580: 2073 656c 662e 636f 6c6f 7273 5f65 7665   self.colors_eve
-0000b590: 6e74 2c0a 2020 2020 2020 2020 5b0a 2020  nt,.        [.  
-0000b5a0: 2020 2020 2020 2020 2020 2250 726f 6a65            "Proje
-0000b5b0: 6374 7322 2c0a 2020 2020 2020 2020 2020  cts",.          
-0000b5c0: 2020 2250 726f 6669 6c65 7322 2c0a 2020    "Profiles",.  
-0000b5d0: 2020 2020 2020 2020 2020 2244 6973 6162            "Disab
-0000b5e0: 6c65 6420 5072 6f66 696c 6573 222c 0a20  led Profiles",. 
-0000b5f0: 2020 2020 2020 2020 2020 2022 4c61 756e             "Laun
-0000b600: 6368 6572 2054 6173 6b22 2c0a 2020 2020  cher Task",.    
-0000b610: 2020 2020 2020 2020 2250 726f 6669 6c65          "Profile
-0000b620: 2043 6f6e 6469 7469 6f6e 7322 2c0a 2020   Conditions",.  
-0000b630: 2020 2020 2020 2020 2020 2254 6173 6b73            "Tasks
-0000b640: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-0000b650: 2854 6173 6b29 2041 6374 696f 6e73 222c  (Task) Actions",
-0000b660: 0a20 2020 2020 2020 2020 2020 2022 4163  .            "Ac
-0000b670: 7469 6f6e 2043 6f6e 6469 7469 6f6e 7322  tion Conditions"
-0000b680: 2c0a 2020 2020 2020 2020 2020 2020 2241  ,.            "A
-0000b690: 6374 696f 6e20 4c61 6265 6c73 222c 0a20  ction Labels",. 
-0000b6a0: 2020 2020 2020 2020 2020 2022 4163 7469             "Acti
-0000b6b0: 6f6e 204e 616d 6573 222c 0a20 2020 2020  on Names",.     
-0000b6c0: 2020 2020 2020 2022 5363 656e 6573 222c         "Scenes",
-0000b6d0: 0a20 2020 2020 2020 2020 2020 2022 4261  .            "Ba
-0000b6e0: 636b 6772 6f75 6e64 222c 0a20 2020 2020  ckground",.     
-0000b6f0: 2020 2020 2020 2022 5461 736b 6572 4e65         "TaskerNe
-0000b700: 7420 496e 666f 726d 6174 696f 6e22 2c0a  t Information",.
-0000b710: 2020 2020 2020 2020 2020 2020 2254 6173              "Tas
-0000b720: 6b65 7220 5072 6566 6572 656e 6365 7322  ker Preferences"
-0000b730: 2c0a 2020 2020 2020 2020 2020 2020 2248  ,.            "H
-0000b740: 6967 686c 6967 6874 222c 0a20 2020 2020  ighlight",.     
-0000b750: 2020 2020 2020 2022 4865 6164 696e 6722         "Heading"
-0000b760: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
-0000b770: 2020 2020 2031 2c0a 2020 2020 2020 2020       1,.        
-0000b780: 302c 0a20 2020 2020 2020 2032 302c 0a20  0,.        20,. 
-0000b790: 2020 2020 2020 2028 3130 2c20 3130 292c         (10, 10),
-0000b7a0: 0a20 2020 2020 2020 2022 222c 0a20 2020  .        "",.   
-0000b7b0: 2029 0a0a 2020 2020 2320 5265 7365 7420   )..    # Reset 
-0000b7c0: 746f 2044 6566 6175 6c74 2043 6f6c 6f72  to Default Color
-0000b7d0: 7320 6275 7474 6f6e 0a20 2020 2073 656c  s button.    sel
-0000b7e0: 662e 636f 6c6f 725f 7265 7365 745f 6275  f.color_reset_bu
-0000b7f0: 7474 6f6e 203d 2061 6464 5f62 7574 746f  tton = add_butto
-0000b800: 6e28 0a20 2020 2020 2020 2073 656c 662c  n(.        self,
-0000b810: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0000b820: 6276 6965 772e 7461 6228 2243 6f6c 6f72  bview.tab("Color
-0000b830: 7322 292c 0a20 2020 2020 2020 2022 222c  s"),.        "",
-0000b840: 0a20 2020 2020 2020 2022 222c 0a20 2020  .        "",.   
-0000b850: 2020 2020 2022 222c 0a20 2020 2020 2020       "",.       
-0000b860: 2073 656c 662e 636f 6c6f 725f 7265 7365   self.color_rese
-0000b870: 745f 6576 656e 742c 0a20 2020 2020 2020  t_event,.       
-0000b880: 2032 2c0a 2020 2020 2020 2020 2252 6573   2,.        "Res
-0000b890: 6574 2074 6f20 4465 6661 756c 7420 436f  et to Default Co
-0000b8a0: 6c6f 7273 222c 0a20 2020 2020 2020 2031  lors",.        1
-0000b8b0: 2c0a 2020 2020 2020 2020 332c 0a20 2020  ,.        3,.   
-0000b8c0: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
-0000b8d0: 3230 2c0a 2020 2020 2020 2020 2831 302c  20,.        (10,
-0000b8e0: 2031 3029 2c0a 2020 2020 2020 2020 2222   10),.        ""
-0000b8f0: 2c0a 2020 2020 290a 0a20 2020 2023 2041  ,.    )..    # A
-0000b900: 4920 5461 6220 6669 656c 6473 0a20 2020  I Tab fields.   
-0000b910: 2023 2041 5049 204b 6579 0a20 2020 2063   # API Key.    c
-0000b920: 656e 7465 7220 3d20 3530 0a20 2020 2073  enter = 50.    s
-0000b930: 656c 662e 6169 5f61 7069 6b65 795f 6275  elf.ai_apikey_bu
-0000b940: 7474 6f6e 203d 2061 6464 5f62 7574 746f  tton = add_butto
-0000b950: 6e28 0a20 2020 2020 2020 2073 656c 662c  n(.        self,
-0000b960: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0000b970: 6276 6965 772e 7461 6228 2241 6e61 6c79  bview.tab("Analy
-0000b980: 7a65 2229 2c0a 2020 2020 2020 2020 2222  ze"),.        ""
-0000b990: 2c20 2023 2066 675f 636f 6c6f 723a 2073  ,  # fg_color: s
-0000b9a0: 7472 2c0a 2020 2020 2020 2020 2222 2c20  tr,.        "", 
-0000b9b0: 2023 2074 6578 745f 636f 6c6f 723a 2073   # text_color: s
-0000b9c0: 7472 2c0a 2020 2020 2020 2020 2222 2c20  tr,.        "", 
-0000b9d0: 2023 2062 6f72 6465 725f 636f 6c6f 723a   # border_color:
-0000b9e0: 2073 7472 2c0a 2020 2020 2020 2020 7365   str,.        se
-0000b9f0: 6c66 2e61 695f 6170 696b 6579 5f65 7665  lf.ai_apikey_eve
-0000ba00: 6e74 2c20 2023 2063 6f6d 6d61 6e64 0a20  nt,  # command. 
-0000ba10: 2020 2020 2020 2032 2c20 2023 2062 6f72         2,  # bor
-0000ba20: 6465 725f 7769 6474 683a 2069 6e74 2c0a  der_width: int,.
-0000ba30: 2020 2020 2020 2020 2253 686f 772f 4564          "Show/Ed
-0000ba40: 6974 204f 7065 6e41 4920 4150 4920 4b65  it OpenAI API Ke
-0000ba50: 7922 2c20 2023 2074 6578 743a 2073 7472  y",  # text: str
-0000ba60: 2c0a 2020 2020 2020 2020 312c 2020 2320  ,.        1,  # 
-0000ba70: 636f 6c75 6d6e 7370 616e 3a20 696e 742c  columnspan: int,
-0000ba80: 0a20 2020 2020 2020 2033 2c20 2023 2072  .        3,  # r
-0000ba90: 6f77 3a20 696e 742c 0a20 2020 2020 2020  ow: int,.       
-0000baa0: 2030 2c20 2023 2063 6f6c 756d 6e3a 2069   0,  # column: i
-0000bab0: 6e74 2c0a 2020 2020 2020 2020 6365 6e74  nt,.        cent
-0000bac0: 6572 2c20 2023 2070 6164 783a 2074 7570  er,  # padx: tup
-0000bad0: 6c65 2c0a 2020 2020 2020 2020 2831 302c  le,.        (10,
-0000bae0: 2031 3029 2c20 2023 2070 6164 793a 2074   10),  # pady: t
-0000baf0: 7570 6c65 2c0a 2020 2020 2020 2020 2222  uple,.        ""
-0000bb00: 2c0a 2020 2020 290a 2020 2020 2320 4d6f  ,.    ).    # Mo
-0000bb10: 6465 6c20 7365 6c65 6374 696f 6e0a 2020  del selection.  
-0000bb20: 2020 7365 6c66 2e61 695f 6d6f 6465 6c5f    self.ai_model_
-0000bb30: 6c61 6265 6c20 3d20 6164 645f 6c61 6265  label = add_labe
-0000bb40: 6c28 0a20 2020 2020 2020 2073 656c 662c  l(.        self,
-0000bb50: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0000bb60: 6276 6965 772e 7461 6228 2241 6e61 6c79  bview.tab("Analy
-0000bb70: 7a65 2229 2c0a 2020 2020 2020 2020 224d  ze"),.        "M
-0000bb80: 6f64 656c 2074 6f20 5573 653a 222c 0a20  odel to Use:",. 
-0000bb90: 2020 2020 2020 2022 222c 0a20 2020 2020         "",.     
-0000bba0: 2020 2030 2c0a 2020 2020 2020 2020 226e     0,.        "n
-0000bbb0: 6f72 6d61 6c22 2c0a 2020 2020 2020 2020  ormal",.        
-0000bbc0: 342c 0a20 2020 2020 2020 2030 2c0a 2020  4,.        0,.  
-0000bbd0: 2020 2020 2020 6365 6e74 6572 2c0a 2020        center,.  
-0000bbe0: 2020 2020 2020 2832 302c 2030 292c 0a20        (20, 0),. 
-0000bbf0: 2020 2020 2020 2022 7322 2c0a 2020 2020         "s",.    
-0000bc00: 290a 2020 2020 6469 7370 6c61 795f 6d6f  ).    display_mo
-0000bc10: 6465 6c73 203d 205b 226e 6f6e 6520 286c  dels = ["none (l
-0000bc20: 6c61 6d61 3329 222c 202a 4f50 454e 4149  lama3)", *OPENAI
-0000bc30: 5f4d 4f44 454c 532c 202a 4c4c 414d 415f  _MODELS, *LLAMA_
-0000bc40: 4d4f 4445 4c53 5d20 2023 2043 6f6d 6269  MODELS]  # Combi
-0000bc50: 6e65 206c 6973 7473 0a20 2020 2073 656c  ne lists.    sel
-0000bc60: 662e 6169 5f6d 6f64 656c 5f6f 7074 696f  f.ai_model_optio
-0000bc70: 6e20 3d20 6164 645f 6f70 7469 6f6e 5f6d  n = add_option_m
-0000bc80: 656e 7528 0a20 2020 2020 2020 2073 656c  enu(.        sel
-0000bc90: 662c 0a20 2020 2020 2020 2073 656c 662e  f,.        self.
-0000bca0: 7461 6276 6965 772e 7461 6228 2241 6e61  tabview.tab("Ana
-0000bcb0: 6c79 7a65 2229 2c0a 2020 2020 2020 2020  lyze"),.        
-0000bcc0: 7365 6c66 2e61 695f 6d6f 6465 6c5f 7365  self.ai_model_se
-0000bcd0: 6c65 6374 6564 5f65 7665 6e74 2c0a 2020  lected_event,.  
-0000bce0: 2020 2020 2020 6469 7370 6c61 795f 6d6f        display_mo
-0000bcf0: 6465 6c73 2c0a 2020 2020 2020 2020 352c  dels,.        5,
-0000bd00: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
-0000bd10: 2020 2020 6365 6e74 6572 2c0a 2020 2020      center,.    
-0000bd20: 2020 2020 2830 2c20 3130 292c 0a20 2020      (0, 10),.   
-0000bd30: 2020 2020 2022 6e22 2c0a 2020 2020 290a       "n",.    ).
-0000bd40: 0a20 2020 2023 2041 6e61 6c79 697a 6520  .    # Analyize 
-0000bd50: 6275 7474 6f6e 0a20 2020 2064 6973 706c  button.    displ
-0000bd60: 6179 5f61 6e61 6c79 7a65 5f62 7574 746f  ay_analyze_butto
-0000bd70: 6e28 7365 6c66 2c20 3130 290a 0a20 2020  n(self, 10)..   
-0000bd80: 2023 2052 6561 646d 6520 4865 6c70 2062   # Readme Help b
-0000bd90: 7574 746f 6e0a 2020 2020 7365 6c66 2e61  utton.    self.a
-0000bda0: 695f 6865 6c70 5f62 7574 746f 6e20 3d20  i_help_button = 
-0000bdb0: 6164 645f 6275 7474 6f6e 280a 2020 2020  add_button(.    
-0000bdc0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000bdd0: 2020 7365 6c66 2e74 6162 7669 6577 2e74    self.tabview.t
-0000bde0: 6162 2822 416e 616c 797a 6522 292c 0a20  ab("Analyze"),. 
-0000bdf0: 2020 2020 2020 2022 2332 3436 4642 3622         "#246FB6"
-0000be00: 2c0a 2020 2020 2020 2020 2822 2330 4246  ,.        ("#0BF
-0000be10: 3037 3522 2c20 2223 6666 6439 3431 2229  075", "#ffd941")
-0000be20: 2c0a 2020 2020 2020 2020 2223 3162 6339  ,.        "#1bc9
-0000be30: 6666 222c 2020 2320 626f 7264 6572 5f63  ff",  # border_c
-0000be40: 6f6c 6f72 3a20 7374 722c 0a20 2020 2020  olor: str,.     
-0000be50: 2020 2073 656c 662e 6169 5f68 656c 705f     self.ai_help_
-0000be60: 6576 656e 742c 2020 2320 636f 6d6d 616e  event,  # comman
-0000be70: 640a 2020 2020 2020 2020 312c 2020 2320  d.        1,  # 
-0000be80: 626f 7264 6572 5f77 6964 7468 3a20 696e  border_width: in
-0000be90: 742c 0a20 2020 2020 2020 2022 3f22 2c20  t,.        "?", 
-0000bea0: 2023 2074 6578 743a 2073 7472 2c0a 2020   # text: str,.  
-0000beb0: 2020 2020 2020 312c 2020 2320 636f 6c75        1,  # colu
-0000bec0: 6d6e 7370 616e 3a20 696e 742c 0a20 2020  mnspan: int,.   
-0000bed0: 2020 2020 2031 302c 2020 2320 726f 773a       10,  # row:
-0000bee0: 2069 6e74 2c0a 2020 2020 2020 2020 302c   int,.        0,
-0000bef0: 2020 2320 636f 6c75 6d6e 3a20 696e 742c    # column: int,
-0000bf00: 0a20 2020 2020 2020 2028 3139 302c 2030  .        (190, 0
-0000bf10: 292c 2020 2320 7061 6478 3a20 7475 706c  ),  # padx: tupl
-0000bf20: 652c 0a20 2020 2020 2020 2028 302c 2030  e,.        (0, 0
-0000bf30: 292c 2020 2320 7061 6479 3a20 7475 706c  ),  # pady: tupl
-0000bf40: 652c 0a20 2020 2020 2020 2022 222c 0a20  e,.        "",. 
-0000bf50: 2020 2029 0a20 2020 2073 656c 662e 6169     ).    self.ai
-0000bf60: 5f68 656c 705f 6275 7474 6f6e 2e63 6f6e  _help_button.con
-0000bf70: 6669 6775 7265 2877 6964 7468 3d32 3029  figure(width=20)
-0000bf80: 0a0a 2020 2020 2320 5468 6520 636f 6d6d  ..    # The comm
-0000bf90: 656e 7465 6420 636f 6465 2074 6573 7473  ented code tests
-0000bfa0: 206f 7574 2074 6865 2063 746b 656e 7472   out the ctkentr
-0000bfb0: 7920 6669 656c 640a 2020 2020 2320 656e  y field.    # en
-0000bfc0: 7472 795f 616e 7377 6572 203d 2022 220a  try_answer = "".
-0000bfd0: 2020 2020 2320 656e 7472 7920 3d20 6374      # entry = ct
-0000bfe0: 6b2e 4354 6b45 6e74 7279 2873 656c 662e  k.CTkEntry(self.
-0000bff0: 7461 6276 6965 772e 7461 6228 2241 6e61  tabview.tab("Ana
-0000c000: 6c79 7a65 2229 2c20 706c 6163 6568 6f6c  lyze"), placehol
-0000c010: 6465 725f 7465 7874 3d22 4354 6b45 6e74  der_text="CTkEnt
-0000c020: 7279 222c 2074 6578 7476 6172 6961 626c  ry", textvariabl
-0000c030: 653d 656e 7472 795f 616e 7377 6572 290a  e=entry_answer).
-0000c040: 2020 2020 2320 656e 7472 792e 6772 6964      # entry.grid
-0000c050: 280a 2020 2020 2320 2020 2072 6f77 3d31  (.    #    row=1
-0000c060: 312c 0a20 2020 2023 2020 2020 636f 6c75  1,.    #    colu
-0000c070: 6d6e 3d30 2c0a 2020 2020 2320 2020 2063  mn=0,.    #    c
-0000c080: 6f6c 756d 6e73 7061 6e3d 312c 0a20 2020  olumnspan=1,.   
-0000c090: 2023 2020 2020 7061 6478 3d28 302c 2030   #    padx=(0, 0
-0000c0a0: 292c 0a20 2020 2023 2020 2020 7061 6479  ),.    #    pady
-0000c0b0: 3d28 302c 2030 292c 0a20 2020 2023 2020  =(0, 0),.    #  
-0000c0c0: 2020 7374 6963 6b79 3d22 6e22 2c0a 2020    sticky="n",.  
-0000c0d0: 2020 2320 290a 0a20 2020 2023 2044 6562    # )..    # Deb
-0000c0e0: 7567 204d 6f64 6520 6368 6563 6b62 6f78  ug Mode checkbox
-0000c0f0: 0a20 2020 2073 656c 662e 6465 6275 675f  .    self.debug_
-0000c100: 6368 6563 6b62 6f78 203d 2061 6464 5f63  checkbox = add_c
-0000c110: 6865 636b 626f 7828 0a20 2020 2020 2020  heckbox(.       
-0000c120: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
-0000c130: 656c 662e 7461 6276 6965 772e 7461 6228  elf.tabview.tab(
-0000c140: 2244 6562 7567 2229 2c0a 2020 2020 2020  "Debug"),.      
-0000c150: 2020 7365 6c66 2e64 6562 7567 5f63 6865    self.debug_che
-0000c160: 636b 626f 785f 6576 656e 742c 0a20 2020  ckbox_event,.   
-0000c170: 2020 2020 2022 4465 6275 6720 4d6f 6465       "Debug Mode
-0000c180: 222c 0a20 2020 2020 2020 2034 2c0a 2020  ",.        4,.  
-0000c190: 2020 2020 2020 332c 0a20 2020 2020 2020        3,.       
-0000c1a0: 2032 302c 0a20 2020 2020 2020 2031 302c   20,.        10,
-0000c1b0: 0a20 2020 2020 2020 2022 7722 2c0a 2020  .        "w",.  
-0000c1c0: 2020 2020 2020 2223 3635 3633 6666 222c        "#6563ff",
-0000c1d0: 0a20 2020 2029 0a20 2020 2023 2052 756e  .    ).    # Run
-0000c1e0: 7469 6d65 0a20 2020 2073 656c 662e 7275  time.    self.ru
-0000c1f0: 6e74 696d 655f 6368 6563 6b62 6f78 203d  ntime_checkbox =
-0000c200: 2061 6464 5f63 6865 636b 626f 7828 0a20   add_checkbox(. 
-0000c210: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000c220: 2020 2020 2073 656c 662e 7461 6276 6965       self.tabvie
-0000c230: 772e 7461 6228 2244 6562 7567 2229 2c0a  w.tab("Debug"),.
-0000c240: 2020 2020 2020 2020 7365 6c66 2e72 756e          self.run
-0000c250: 7469 6d65 5f63 6865 636b 626f 785f 6576  time_checkbox_ev
-0000c260: 656e 742c 0a20 2020 2020 2020 2022 4469  ent,.        "Di
-0000c270: 7370 6c61 7920 5275 6e74 696d 6520 5365  splay Runtime Se
-0000c280: 7474 696e 6773 222c 0a20 2020 2020 2020  ttings",.       
-0000c290: 2033 2c0a 2020 2020 2020 2020 332c 0a20   3,.        3,. 
-0000c2a0: 2020 2020 2020 2032 302c 0a20 2020 2020         20,.     
-0000c2b0: 2020 2031 302c 0a20 2020 2020 2020 2022     10,.        "
-0000c2c0: 7722 2c0a 2020 2020 2020 2020 2223 3635  w",.        "#65
-0000c2d0: 3633 6666 222c 0a20 2020 2029 0a0a 0a23  63ff",.    )...#
-0000c2e0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-0000c2f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c330: 2323 230a 2320 4469 7370 6c61 7920 4169  ###.# Display Ai
-0000c340: 2027 416e 616c 797a 6522 2062 7574 746f   'Analyze" butto
-0000c350: 6e0a 2320 2323 2323 2323 2323 2323 2323  n.# ############
-0000c360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c3a0: 2323 2323 2323 0a64 6566 2064 6973 706c  ######.def displ
-0000c3b0: 6179 5f61 6e61 6c79 7a65 5f62 7574 746f  ay_analyze_butto
-0000c3c0: 6e28 7365 6c66 2c20 726f 773a 2069 6e74  n(self, row: int
-0000c3d0: 2920 2d3e 204e 6f6e 653a 2020 2320 6e6f  ) -> None:  # no
-0000c3e0: 7161 3a20 414e 4e30 3031 0a20 2020 2022  qa: ANN001.    "
-0000c3f0: 2222 0a20 2020 2044 6973 706c 6179 2074  "".    Display t
-0000c400: 6865 2027 416e 616c 797a 6527 2062 7574  he 'Analyze' but
-0000c410: 746f 6e20 666f 7220 7468 6520 4149 2041  ton for the AI A
-0000c420: 5049 206b 6579 2e0a 0a20 2020 2054 6869  PI key...    Thi
-0000c430: 7320 6675 6e63 7469 6f6e 2063 7265 6174  s function creat
-0000c440: 6573 2061 6e64 2064 6973 706c 6179 7320  es and displays 
-0000c450: 6120 6275 7474 6f6e 206f 6e20 7468 6520  a button on the 
-0000c460: 2741 6e61 6c79 7a65 2720 7461 6220 6f66  'Analyze' tab of
-0000c470: 2074 6865 2074 6162 7669 6577 2e20 5468   the tabview. Th
-0000c480: 6520 6275 7474 6f6e 2069 7320 7573 6564  e button is used
-0000c490: 2074 6f20 7275 6e20 7468 6520 616e 616c   to run the anal
-0000c4a0: 7973 6973 2066 6f72 2074 6865 2041 4920  ysis for the AI 
-0000c4b0: 4150 4920 6b65 792e 0a0a 2020 2020 5061  API key...    Pa
-0000c4c0: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-0000c4d0: 2020 7365 6c66 2028 6f62 6a65 6374 293a    self (object):
-0000c4e0: 2054 6865 2069 6e73 7461 6e63 6520 6f66   The instance of
-0000c4f0: 2074 6865 2063 6c61 7373 2e0a 2020 2020   the class..    
-0000c500: 2020 2020 726f 7720 2869 6e74 293a 2054      row (int): T
-0000c510: 6865 2072 6f77 206e 756d 6265 7220 746f  he row number to
-0000c520: 2064 6973 706c 6179 2074 6865 2062 7574   display the but
-0000c530: 746f 6e2e 0a0a 2020 2020 5265 7475 726e  ton...    Return
-0000c540: 733a 0a20 2020 2020 2020 204e 6f6e 653a  s:.        None:
-0000c550: 2054 6869 7320 6675 6e63 7469 6f6e 2064   This function d
-0000c560: 6f65 7320 6e6f 7420 7265 7475 726e 2061  oes not return a
-0000c570: 6e79 7468 696e 672e 0a20 2020 2022 2222  nything..    """
-0000c580: 0a20 2020 2023 2048 6967 686c 6967 6874  .    # Highlight
-0000c590: 2074 6865 2062 7574 746f 6e20 6966 2077   the button if w
-0000c5a0: 6520 6861 7665 2065 7665 7279 7468 696e  e have everythin
-0000c5b0: 6720 746f 2072 756e 2074 6865 2041 6e61  g to run the Ana
-0000c5c0: 6c79 7369 732e 0a20 2020 2069 6620 2828  lysis..    if ((
-0000c5d0: 7365 6c66 2e61 695f 6d6f 6465 6c20 696e  self.ai_model in
-0000c5e0: 204f 5045 4e41 495f 4d4f 4445 4c53 2061   OPENAI_MODELS a
-0000c5f0: 6e64 2073 656c 662e 6169 5f61 7069 6b65  nd self.ai_apike
-0000c600: 7929 206f 7220 7365 6c66 2e61 695f 6d6f  y) or self.ai_mo
-0000c610: 6465 6c29 2061 6e64 2028 0a20 2020 2020  del) and (.     
-0000c620: 2020 2073 656c 662e 7369 6e67 6c65 5f74     self.single_t
-0000c630: 6173 6b5f 6e61 6d65 206f 7220 7365 6c66  ask_name or self
-0000c640: 2e73 696e 676c 655f 7072 6f66 696c 655f  .single_profile_
-0000c650: 6e61 6d65 0a20 2020 2029 3a0a 2020 2020  name.    ):.    
-0000c660: 2020 2020 6667 5f63 6f6c 6f72 203d 2022      fg_color = "
-0000c670: 2366 3535 6466 6622 0a20 2020 2020 2020  #f55dff".       
-0000c680: 2074 6578 745f 636f 6c6f 7220 3d20 2223   text_color = "#
-0000c690: 3535 3534 6666 220a 2020 2020 656c 7365  5554ff".    else
-0000c6a0: 3a0a 2020 2020 2020 2020 6667 5f63 6f6c  :.        fg_col
-0000c6b0: 6f72 203d 2022 220a 2020 2020 2020 2020  or = "".        
-0000c6c0: 7465 7874 5f63 6f6c 6f72 203d 2022 220a  text_color = "".
-0000c6d0: 0a20 2020 2073 656c 662e 6169 5f61 6e61  .    self.ai_ana
-0000c6e0: 6c79 7a65 5f62 7574 746f 6e20 3d20 6164  lyze_button = ad
-0000c6f0: 645f 6275 7474 6f6e 280a 2020 2020 2020  d_button(.      
-0000c700: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000c710: 7365 6c66 2e74 6162 7669 6577 2e74 6162  self.tabview.tab
-0000c720: 2822 416e 616c 797a 6522 292c 0a20 2020  ("Analyze"),.   
-0000c730: 2020 2020 2066 675f 636f 6c6f 722c 2020       fg_color,  
-0000c740: 2320 6667 5f63 6f6c 6f72 3a20 7374 722c  # fg_color: str,
-0000c750: 0a20 2020 2020 2020 2074 6578 745f 636f  .        text_co
-0000c760: 6c6f 722c 2020 2320 7465 7874 5f63 6f6c  lor,  # text_col
-0000c770: 6f72 3a20 7374 722c 0a20 2020 2020 2020  or: str,.       
-0000c780: 2022 222c 2020 2320 626f 7264 6572 5f63   "",  # border_c
-0000c790: 6f6c 6f72 3a20 7374 722c 0a20 2020 2020  olor: str,.     
-0000c7a0: 2020 2073 656c 662e 6169 5f61 6e61 6c79     self.ai_analy
-0000c7b0: 7a65 5f65 7665 6e74 2c20 2023 2063 6f6d  ze_event,  # com
-0000c7c0: 6d61 6e64 0a20 2020 2020 2020 2032 2c20  mand.        2, 
-0000c7d0: 2023 2062 6f72 6465 725f 7769 6474 683a   # border_width:
-0000c7e0: 2069 6e74 2c0a 2020 2020 2020 2020 2252   int,.        "R
-0000c7f0: 756e 2041 6e61 6c79 7369 7322 2c20 2023  un Analysis",  #
-0000c800: 2074 6578 743a 2073 7472 2c0a 2020 2020   text: str,.    
-0000c810: 2020 2020 312c 2020 2320 636f 6c75 6d6e      1,  # column
-0000c820: 7370 616e 3a20 696e 742c 0a20 2020 2020  span: int,.     
-0000c830: 2020 2072 6f77 2c20 2023 2072 6f77 3a20     row,  # row: 
-0000c840: 696e 742c 0a20 2020 2020 2020 2030 2c20  int,.        0, 
-0000c850: 2023 2063 6f6c 756d 6e3a 2069 6e74 2c0a   # column: int,.
-0000c860: 2020 2020 2020 2020 3530 2c20 2023 2070          50,  # p
-0000c870: 6164 783a 2074 7570 6c65 2c0a 2020 2020  adx: tuple,.    
-0000c880: 2020 2020 2831 302c 2031 3029 2c20 2023      (10, 10),  #
-0000c890: 2070 6164 793a 2074 7570 6c65 2c0a 2020   pady: tuple,.  
-0000c8a0: 2020 2020 2020 2222 2c0a 2020 2020 290a        "",.    ).
-0000c8b0: 0a0a 2320 2323 2323 2323 2323 2323 2323  ..# ############
-0000c8c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c8d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c8e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c8f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c900: 2323 2323 2323 0a23 2044 6973 706c 6179  ######.# Display
-0000c910: 2074 6865 2063 7572 7265 6e74 2073 6574   the current set
-0000c920: 7469 6e67 7320 666f 7220 4169 0a23 2023  tings for Ai.# #
-0000c930: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c960: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c970: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000c980: 230a 6465 6620 6469 7370 6c61 795f 6169  #.def display_ai
-0000c990: 5f73 6574 7469 6e67 7328 7365 6c66 2920  _settings(self) 
-0000c9a0: 2d3e 204e 6f6e 653a 2020 2320 6e6f 7161  -> None:  # noqa
-0000c9b0: 3a20 414e 4e30 3031 0a20 2020 2022 2222  : ANN001.    """
-0000c9c0: 0a20 2020 2044 6973 706c 6179 2074 6865  .    Display the
-0000c9d0: 2063 7572 7265 6e74 2073 6574 7469 6e67   current setting
-0000c9e0: 7320 666f 7220 4169 0a20 2020 2022 2222  s for Ai.    """
-0000c9f0: 0a20 2020 2023 2052 6561 6420 7468 6520  .    # Read the 
-0000ca00: 6170 6920 6b65 792e 0a20 2020 2073 656c  api key..    sel
-0000ca10: 662e 6169 5f61 7069 6b65 7920 3d20 6765  f.ai_apikey = ge
-0000ca20: 745f 6170 695f 6b65 7928 290a 2020 2020  t_api_key().    
-0000ca30: 6b65 795f 746f 5f64 6973 706c 6179 203d  key_to_display =
-0000ca40: 2022 5365 7422 2069 6620 7365 6c66 2e61   "Set" if self.a
-0000ca50: 695f 6170 696b 6579 2065 6c73 6520 2255  i_apikey else "U
-0000ca60: 6e73 6574 220a 2020 2020 6d6f 6465 6c5f  nset".    model_
-0000ca70: 746f 5f64 6973 706c 6179 203d 2073 656c  to_display = sel
-0000ca80: 662e 6169 5f6d 6f64 656c 2069 6620 7365  f.ai_model if se
-0000ca90: 6c66 2e61 695f 6d6f 6465 6c20 656c 7365  lf.ai_model else
-0000caa0: 2022 6e6f 6e65 2028 6c6c 616d 6133 2922   "none (llama3)"
-0000cab0: 0a20 2020 2073 656c 662e 6169 5f73 6574  .    self.ai_set
-0000cac0: 5f6c 6162 656c 3120 3d20 6164 645f 6c61  _label1 = add_la
-0000cad0: 6265 6c28 0a20 2020 2020 2020 2073 656c  bel(.        sel
-0000cae0: 662c 0a20 2020 2020 2020 2073 656c 662e  f,.        self.
-0000caf0: 7461 6276 6965 772e 7461 6228 2241 6e61  tabview.tab("Ana
-0000cb00: 6c79 7a65 2229 2c0a 2020 2020 2020 2020  lyze"),.        
-0000cb10: 6622 4150 4920 4b65 793a 207b 6b65 795f  f"API Key: {key_
-0000cb20: 746f 5f64 6973 706c 6179 7d2c 204d 6f64  to_display}, Mod
-0000cb30: 656c 3a20 7b6d 6f64 656c 5f74 6f5f 6469  el: {model_to_di
-0000cb40: 7370 6c61 797d 222c 0a20 2020 2020 2020  splay}",.       
-0000cb50: 2022 222c 0a20 2020 2020 2020 2030 2c0a   "",.        0,.
-0000cb60: 2020 2020 2020 2020 226e 6f72 6d61 6c22          "normal"
-0000cb70: 2c0a 2020 2020 2020 2020 3132 2c0a 2020  ,.        12,.  
-0000cb80: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
-0000cb90: 2031 302c 0a20 2020 2020 2020 2028 3230   10,.        (20
-0000cba0: 2c20 3029 2c0a 2020 2020 2020 2020 2277  , 0),.        "w
-0000cbb0: 222c 0a20 2020 2029 0a0a 2020 2020 2320  ",.    )..    # 
-0000cbc0: 4e6f 7465 3a20 4e6f 7468 696e 6720 6265  Note: Nothing be
-0000cbd0: 796f 6e64 2074 6869 7320 706f 696e 7420  yond this point 
-0000cbe0: 7769 6c6c 2061 7070 6561 7220 696e 2074  will appear in t
-0000cbf0: 6865 2067 7269 642e 2020 526f 7720 3132  he grid.  Row 12
-0000cc00: 2069 7320 7468 6520 6d61 782e 0a20 2020   is the max..   
-0000cc10: 2023 2073 656c 662e 6169 5f73 6574 5f6c   # self.ai_set_l
-0000cc20: 6162 656c 3220 3d20 6164 645f 6c61 6265  abel2 = add_labe
-0000cc30: 6c28 0a20 2020 2023 2020 2020 7365 6c66  l(.    #    self
-0000cc40: 2c0a 2020 2020 2320 2020 2073 656c 662e  ,.    #    self.
-0000cc50: 7461 6276 6965 772e 7461 6228 2241 6e61  tabview.tab("Ana
-0000cc60: 6c79 7a65 2229 2c0a 2020 2020 2320 2020  lyze"),.    #   
-0000cc70: 2066 224d 6f64 656c 3a20 7b6d 6f64 656c   f"Model: {model
-0000cc80: 5f74 6f5f 6469 7370 6c61 797d 222c 0a20  _to_display}",. 
-0000cc90: 2020 2023 2020 2020 2222 2c0a 2020 2020     #    "",.    
-0000cca0: 2320 2020 2030 2c0a 2020 2020 2320 2020  #    0,.    #   
-0000ccb0: 2022 6e6f 726d 616c 222c 0a20 2020 2023   "normal",.    #
-0000ccc0: 2020 2020 3133 2c0a 2020 2020 2320 2020      13,.    #   
-0000ccd0: 2030 2c0a 2020 2020 2320 2020 2031 302c   0,.    #    10,
-0000cce0: 0a20 2020 2023 2020 2020 2832 302c 2030  .    #    (20, 0
-0000ccf0: 292c 0a20 2020 2023 2020 2020 2277 222c  ),.    #    "w",
-0000cd00: 0a20 2020 2023 2029 0a20 2020 2070 726f  .    # ).    pro
-0000cd10: 6669 6c65 5f74 6f5f 6469 7370 6c61 7920  file_to_display 
-0000cd20: 3d20 7365 6c66 2e73 696e 676c 655f 7072  = self.single_pr
-0000cd30: 6f66 696c 655f 6e61 6d65 2069 6620 7365  ofile_name if se
-0000cd40: 6c66 2e73 696e 676c 655f 7072 6f66 696c  lf.single_profil
-0000cd50: 655f 6e61 6d65 2065 6c73 6520 2255 6e64  e_name else "Und
-0000cd60: 6566 696e 6564 220a 2020 2020 7461 736b  efined".    task
-0000cd70: 5f74 6f5f 6469 7370 6c61 7920 3d20 7365  _to_display = se
-0000cd80: 6c66 2e73 696e 676c 655f 7461 736b 5f6e  lf.single_task_n
-0000cd90: 616d 6520 6966 2073 656c 662e 7369 6e67  ame if self.sing
-0000cda0: 6c65 5f74 6173 6b5f 6e61 6d65 2065 6c73  le_task_name els
-0000cdb0: 6520 2255 6e64 6566 696e 6564 220a 2020  e "Undefined".  
-0000cdc0: 2020 7365 6c66 2e61 695f 6d6f 6465 6c5f    self.ai_model_
-0000cdd0: 6f70 7469 6f6e 2e73 6574 286d 6f64 656c  option.set(model
-0000cde0: 5f74 6f5f 6469 7370 6c61 7929 2020 2320  _to_display)  # 
-0000cdf0: 5365 7420 7468 6520 6375 7272 656e 7420  Set the current 
-0000ce00: 6d6f 6465 6c20 696e 2074 6865 2070 756c  model in the pul
-0000ce10: 6c64 6f77 6e2e 0a0a 2020 2020 2320 5468  ldown...    # Th
-0000ce20: 6520 6c61 6265 6c20 7368 6f75 6c64 2068  e label should h
-0000ce30: 6176 6520 6265 656e 2064 6573 7472 6f79  ave been destroy
-0000ce40: 6564 2c20 6275 7420 6973 6e27 7420 6475  ed, but isn't du
-0000ce50: 6520 746f 2074 6b20 6275 672e 2020 536f  e to tk bug.  So
-0000ce60: 2077 6520 6861 7665 2074 6f20 626c 616e   we have to blan
-0000ce70: 6b20 6669 6c6c 2069 6620 6e65 6365 7373  k fill if necess
-0000ce80: 6172 792e 0a20 2020 2070 726f 6669 6c65  ary..    profile
-0000ce90: 5f6c 656e 6774 6820 3d20 6c65 6e28 7072  _length = len(pr
-0000cea0: 6f66 696c 655f 746f 5f64 6973 706c 6179  ofile_to_display
-0000ceb0: 290a 2020 2020 6669 6c6c 203d 2031 360a  ).    fill = 16.
-0000cec0: 2020 2020 6966 2070 726f 6669 6c65 5f6c      if profile_l
-0000ced0: 656e 6774 6820 3c20 6669 6c6c 3a0a 2020  ength < fill:.  
-0000cee0: 2020 2020 2020 7072 6f66 696c 655f 746f        profile_to
-0000cef0: 5f64 6973 706c 6179 203d 2070 726f 6669  _display = profi
-0000cf00: 6c65 5f74 6f5f 6469 7370 6c61 792e 6c6a  le_to_display.lj
-0000cf10: 7573 7428 6669 6c6c 202d 2070 726f 6669  ust(fill - profi
-0000cf20: 6c65 5f6c 656e 6774 682c 2022 2022 290a  le_length, " ").
-0000cf30: 0a20 2020 2023 2044 6973 706c 6179 2074  .    # Display t
-0000cf40: 6865 2050 726f 6669 6c65 2074 6f20 616e  he Profile to an
-0000cf50: 616c 797a 650a 2020 2020 7365 6c66 2e61  alyze.    self.a
-0000cf60: 695f 7365 745f 6c61 6265 6c33 203d 2061  i_set_label3 = a
-0000cf70: 6464 5f6c 6162 656c 280a 2020 2020 2020  dd_label(.      
-0000cf80: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000cf90: 7365 6c66 2e74 6162 7669 6577 2e74 6162  self.tabview.tab
-0000cfa0: 2822 416e 616c 797a 6522 292c 0a20 2020  ("Analyze"),.   
-0000cfb0: 2020 2020 2066 2250 726f 6669 6c65 2074       f"Profile t
-0000cfc0: 6f20 416e 616c 797a 653a 207b 7072 6f66  o Analyze: {prof
-0000cfd0: 696c 655f 746f 5f64 6973 706c 6179 7d22  ile_to_display}"
-0000cfe0: 2c0a 2020 2020 2020 2020 2222 2c0a 2020  ,.        "",.  
-0000cff0: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
-0000d000: 2022 6e6f 726d 616c 222c 0a20 2020 2020   "normal",.     
-0000d010: 2020 2031 342c 0a20 2020 2020 2020 2030     14,.        0
-0000d020: 2c0a 2020 2020 2020 2020 3130 2c0a 2020  ,.        10,.  
-0000d030: 2020 2020 2020 2832 302c 2030 292c 0a20        (20, 0),. 
-0000d040: 2020 2020 2020 2022 7722 2c0a 2020 2020         "w",.    
-0000d050: 290a 2020 2020 2320 4469 7370 6c61 7920  ).    # Display 
-0000d060: 7468 6520 5461 736b 2074 6f20 616e 616c  the Task to anal
-0000d070: 797a 650a 2020 2020 7365 6c66 2e61 695f  yze.    self.ai_
-0000d080: 7365 745f 6c61 6265 6c33 203d 2061 6464  set_label3 = add
-0000d090: 5f6c 6162 656c 280a 2020 2020 2020 2020  _label(.        
-0000d0a0: 7365 6c66 2c0a 2020 2020 2020 2020 7365  self,.        se
-0000d0b0: 6c66 2e74 6162 7669 6577 2e74 6162 2822  lf.tabview.tab("
-0000d0c0: 416e 616c 797a 6522 292c 0a20 2020 2020  Analyze"),.     
-0000d0d0: 2020 2066 2254 6173 6b20 746f 2041 6e61     f"Task to Ana
-0000d0e0: 6c79 7a65 3a20 7b74 6173 6b5f 746f 5f64  lyze: {task_to_d
-0000d0f0: 6973 706c 6179 7d22 2c0a 2020 2020 2020  isplay}",.      
-0000d100: 2020 2222 2c0a 2020 2020 2020 2020 302c    "",.        0,
-0000d110: 0a20 2020 2020 2020 2022 6e6f 726d 616c  .        "normal
-0000d120: 222c 0a20 2020 2020 2020 2031 352c 0a20  ",.        15,. 
-0000d130: 2020 2020 2020 2030 2c0a 2020 2020 2020         0,.      
-0000d140: 2020 3130 2c0a 2020 2020 2020 2020 2832    10,.        (2
-0000d150: 302c 2030 292c 0a20 2020 2020 2020 2022  0, 0),.        "
-0000d160: 7722 2c0a 2020 2020 290a 0a0a 2320 2323  w",.    )...# ##
-0000d170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d180: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d1a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d1b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d1c0: 0a23 2047 6574 2074 6865 2041 6920 6170  .# Get the Ai ap
-0000d1d0: 6920 6b65 790a 2320 2323 2323 2323 2323  i key.# ########
-0000d1e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d1f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d220: 2323 2323 2323 2323 2323 0a64 6566 2067  ##########.def g
-0000d230: 6574 5f61 7069 5f6b 6579 2829 202d 3e20  et_api_key() -> 
-0000d240: 7374 723a 0a20 2020 2022 2222 0a20 2020  str:.    """.   
-0000d250: 2052 6574 7269 6576 6573 2074 6865 2041   Retrieves the A
-0000d260: 5049 206b 6579 2066 726f 6d20 7468 6520  PI key from the 
-0000d270: 7370 6563 6966 6965 6420 6669 6c65 2e0a  specified file..
-0000d280: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
-0000d290: 6f6e 2063 6865 636b 7320 6966 2074 6865  on checks if the
-0000d2a0: 204b 4559 4649 4c45 2065 7869 7374 7320   KEYFILE exists 
-0000d2b0: 616e 6420 6966 2069 7420 646f 6573 2c20  and if it does, 
-0000d2c0: 6974 206f 7065 6e73 2074 6865 2066 696c  it opens the fil
-0000d2d0: 6520 616e 6420 7265 6164 7320 7468 6520  e and reads the 
-0000d2e0: 6669 7273 7420 6c69 6e65 2e20 5468 6520  first line. The 
-0000d2f0: 6669 7273 7420 6c69 6e65 2069 7320 6173  first line is as
-0000d300: 7375 6d65 6420 746f 2062 6520 7468 6520  sumed to be the 
-0000d310: 4150 4920 6b65 792e 2049 6620 7468 6520  API key. If the 
-0000d320: 4b45 5946 494c 4520 646f 6573 206e 6f74  KEYFILE does not
-0000d330: 2065 7869 7374 2c20 6974 2072 6574 7572   exist, it retur
-0000d340: 6e73 2074 6865 2073 7472 696e 6720 224e  ns the string "N
-0000d350: 6f6e 6522 2e0a 0a20 2020 2052 6574 7572  one"...    Retur
-0000d360: 6e73 3a0a 2020 2020 2020 2020 7374 723a  ns:.        str:
-0000d370: 2054 6865 2041 5049 206b 6579 2069 6620   The API key if 
-0000d380: 6974 2065 7869 7374 732c 206f 7468 6572  it exists, other
-0000d390: 7769 7365 2022 4e6f 6e65 222e 0a20 2020  wise "None"..   
-0000d3a0: 2022 2222 0a20 2020 2069 6620 6f73 2e70   """.    if os.p
-0000d3b0: 6174 682e 6973 6669 6c65 284b 4559 4649  ath.isfile(KEYFI
-0000d3c0: 4c45 293a 0a20 2020 2020 2020 2023 204f  LE):.        # O
-0000d3d0: 7065 6e20 6f75 7470 7574 2066 696c 650a  pen output file.
-0000d3e0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-0000d3f0: 6e28 4b45 5946 494c 4529 2061 7320 6b65  n(KEYFILE) as ke
-0000d400: 795f 6669 6c65 3a0a 2020 2020 2020 2020  y_file:.        
-0000d410: 2020 2020 7265 7475 726e 206b 6579 5f66      return key_f
-0000d420: 696c 652e 7265 6164 6c69 6e65 2829 0a20  ile.readline(). 
-0000d430: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000d440: 2072 6574 7572 6e20 224e 6f6e 6522 0a0a   return "None"..
-0000d450: 0a23 2023 2323 2323 2323 2323 2323 2323  .# #############
-0000d460: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d470: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d480: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d490: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d4a0: 2323 2323 230a 2320 4569 7468 6572 2076  #####.# Either v
-0000d4b0: 616c 6964 6174 6520 7468 6520 6669 6c65  alidate the file
-0000d4c0: 206c 6f63 6174 696f 6e20 7072 6f76 6964   location provid
-0000d4d0: 6564 206f 7220 7072 6f76 6964 6520 6120  ed or provide a 
-0000d4e0: 6669 6c65 6c69 7374 206f 6620 584d 4c20  filelist of XML 
-0000d4f0: 6669 6c65 730a 2320 2323 2323 2323 2323  files.# ########
-0000d500: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d510: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d530: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d540: 2323 2323 2323 2323 2323 0a64 6566 2076  ##########.def v
-0000d550: 616c 6964 6174 655f 6f72 5f66 696c 656c  alidate_or_filel
-0000d560: 6973 745f 786d 6c28 0a20 2020 2073 656c  ist_xml(.    sel
-0000d570: 662c 2020 2320 6e6f 7161 3a20 414e 4e30  f,  # noqa: ANN0
-0000d580: 3031 0a20 2020 2061 6e64 726f 6964 5f69  01.    android_i
-0000d590: 7061 6464 723a 2073 7472 2c0a 2020 2020  paddr: str,.    
-0000d5a0: 616e 6472 6f69 645f 706f 7274 3a20 7374  android_port: st
-0000d5b0: 722c 0a20 2020 2061 6e64 726f 6964 5f66  r,.    android_f
-0000d5c0: 696c 653a 2073 7472 2c0a 2920 2d3e 2074  ile: str,.) -> t
-0000d5d0: 7570 6c65 5b69 6e74 2c20 7374 725d 3a0a  uple[int, str]:.
-0000d5e0: 2020 2020 2320 4966 2077 6520 646f 6e27      # If we don'
-0000d5f0: 7420 6861 7665 2074 6865 2066 696c 6520  t have the file 
-0000d600: 6c6f 6361 7469 6f6e 2079 6574 2061 6e64  location yet and
-0000d610: 2077 6520 646f 6e27 7420 7965 7420 6861   we don't yet ha
-0000d620: 7665 2061 206c 6973 7420 6f66 2066 696c  ve a list of fil
-0000d630: 6573 2c20 7468 656e 2067 6574 2074 6865  es, then get the
-0000d640: 2058 4d4c 2066 696c 650a 2020 2020 2320   XML file.    # 
-0000d650: 746f 2076 616c 6964 6174 6520 7468 6174  to validate that
-0000d660: 2069 7420 6578 6973 7473 2e0a 2020 2020   it exists..    
-0000d670: 2222 2246 756e 6374 696f 6e20 746f 2076  """Function to v
-0000d680: 616c 6964 6174 6520 616e 2058 4d4c 2066  alidate an XML f
-0000d690: 696c 6520 6f6e 2061 6e20 416e 6472 6f69  ile on an Androi
-0000d6a0: 6420 6465 7669 6365 2061 6e64 2072 6574  d device and ret
-0000d6b0: 7572 6e20 7468 6520 6669 6c65 2773 2063  urn the file's c
-0000d6c0: 6f6e 7465 6e74 7320 6966 2069 7420 6578  ontents if it ex
-0000d6d0: 6973 7473 2e0a 2020 2020 5061 7261 6d65  ists..    Parame
-0000d6e0: 7465 7273 3a0a 2020 2020 2020 2020 2d20  ters:.        - 
-0000d6f0: 616e 6472 6f69 645f 6970 6164 6472 2028  android_ipaddr (
-0000d700: 7374 7229 3a20 4950 2061 6464 7265 7373  str): IP address
-0000d710: 206f 6620 7468 6520 416e 6472 6f69 6420   of the Android 
-0000d720: 6465 7669 6365 2e0a 2020 2020 2020 2020  device..        
-0000d730: 2d20 616e 6472 6f69 645f 706f 7274 2028  - android_port (
-0000d740: 7374 7229 3a20 506f 7274 206e 756d 6265  str): Port numbe
-0000d750: 7220 6f66 2074 6865 2041 6e64 726f 6964  r of the Android
-0000d760: 2064 6576 6963 652e 0a20 2020 2020 2020   device..       
-0000d770: 202d 2061 6e64 726f 6964 5f66 696c 6520   - android_file 
-0000d780: 2873 7472 293a 2046 696c 6520 6e61 6d65  (str): File name
-0000d790: 206f 6620 7468 6520 584d 4c20 6669 6c65   of the XML file
-0000d7a0: 2074 6f20 7661 6c69 6461 7465 2e0a 2020   to validate..  
-0000d7b0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000d7c0: 2020 202d 2054 7570 6c65 5b69 6e74 2c20     - Tuple[int, 
-0000d7d0: 7374 725d 3a20 4120 7475 706c 6520 636f  str]: A tuple co
-0000d7e0: 6e74 6169 6e69 6e67 2074 6865 2072 6574  ntaining the ret
-0000d7f0: 7572 6e20 636f 6465 2061 6e64 2074 6865  urn code and the
-0000d800: 2066 696c 6527 7320 636f 6e74 656e 7473   file's contents
-0000d810: 2069 6620 6974 2065 7869 7374 732e 0a20   if it exists.. 
-0000d820: 2020 2050 726f 6365 7373 696e 6720 4c6f     Processing Lo
-0000d830: 6769 633a 0a20 2020 2020 2020 202d 2047  gic:.        - G
-0000d840: 6574 2074 6865 2058 4d4c 2066 696c 6520  et the XML file 
-0000d850: 6672 6f6d 2074 6865 2041 6e64 726f 6964  from the Android
-0000d860: 2064 6576 6963 6520 6966 206e 6f20 6669   device if no fi
-0000d870: 6c65 206c 6f63 6174 696f 6e20 6973 2070  le location is p
-0000d880: 726f 7669 6465 642e 0a20 2020 2020 2020  rovided..       
-0000d890: 202d 2056 616c 6964 6174 6520 7468 6520   - Validate the 
-0000d8a0: 584d 4c20 6669 6c65 2e0a 2020 2020 2020  XML file..      
-0000d8b0: 2020 2d20 4966 2074 6865 2066 696c 6520    - If the file 
-0000d8c0: 646f 6573 206e 6f74 2065 7869 7374 2c20  does not exist, 
-0000d8d0: 6469 7370 6c61 7920 616e 2065 7272 6f72  display an error
-0000d8e0: 206d 6573 7361 6765 2e0a 2020 2020 2020   message..      
-0000d8f0: 2020 2d20 4966 2074 6865 2066 696c 6520    - If the file 
-0000d900: 6c6f 6361 7469 6f6e 2069 7320 6e6f 7420  location is not 
-0000d910: 7072 6f76 6964 6564 2c20 6765 7420 6120  provided, get a 
-0000d920: 6c69 7374 206f 6620 616c 6c20 584d 4c20  list of all XML 
-0000d930: 6669 6c65 7320 6672 6f6d 2074 6865 2041  files from the A
-0000d940: 6e64 726f 6964 2064 6576 6963 6520 616e  ndroid device an
-0000d950: 6420 7072 6573 656e 7420 6974 2074 6f20  d present it to 
-0000d960: 7468 6520 7573 6572 2e0a 2020 2020 2222  the user..    ""
-0000d970: 220a 2020 2020 2320 4966 2077 6520 646f  ".    # If we do
-0000d980: 6e27 7420 7965 7420 6861 7665 2074 6865  n't yet have the
-0000d990: 2066 696c 652c 2074 6865 6e20 6765 7420   file, then get 
-0000d9a0: 6974 2066 726f 6d20 7468 6520 416e 6472  it from the Andr
-0000d9b0: 6f69 6420 6465 7669 6365 2e0a 2020 2020  oid device..    
-0000d9c0: 6966 206c 656e 2861 6e64 726f 6964 5f66  if len(android_f
-0000d9d0: 696c 6529 2021 3d20 3020 616e 6420 616e  ile) != 0 and an
-0000d9e0: 6472 6f69 645f 6669 6c65 2021 3d20 2222  droid_file != ""
-0000d9f0: 2061 6e64 2073 656c 662e 6c69 7374 5f66   and self.list_f
-0000da00: 696c 6573 203d 3d20 4661 6c73 653a 0a20  iles == False:. 
-0000da10: 2020 2020 2020 2072 6574 7572 6e5f 636f         return_co
-0000da20: 6465 2c20 6669 6c65 5f63 6f6e 7465 6e74  de, file_content
-0000da30: 7320 3d20 6874 7470 5f72 6571 7565 7374  s = http_request
-0000da40: 2861 6e64 726f 6964 5f69 7061 6464 722c  (android_ipaddr,
-0000da50: 2061 6e64 726f 6964 5f70 6f72 742c 2061   android_port, a
-0000da60: 6e64 726f 6964 5f66 696c 652c 2022 6669  ndroid_file, "fi
-0000da70: 6c65 222c 2022 3f64 6f77 6e6c 6f61 643d  le", "?download=
-0000da80: 3122 290a 0a20 2020 2020 2020 2023 2056  1")..        # V
-0000da90: 616c 6964 6174 6520 584d 4c20 6669 6c65  alidate XML file
-0000daa0: 2e0a 2020 2020 2020 2020 6966 2072 6574  ..        if ret
-0000dab0: 7572 6e5f 636f 6465 203d 3d20 303a 0a20  urn_code == 0:. 
-0000dac0: 2020 2020 2020 2020 2020 2050 7269 6d65             Prime
-0000dad0: 4974 656d 732e 7072 6f67 7261 6d5f 6172  Items.program_ar
-0000dae0: 6775 6d65 6e74 735b 2267 7569 225d 203d  guments["gui"] =
-0000daf0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0000db00: 2020 7265 7475 726e 5f63 6f64 652c 2065    return_code, e
-0000db10: 7272 6f72 5f6d 6573 7361 6765 203d 2076  rror_message = v
-0000db20: 616c 6964 6174 655f 786d 6c5f 6669 6c65  alidate_xml_file
-0000db30: 2861 6e64 726f 6964 5f69 7061 6464 722c  (android_ipaddr,
-0000db40: 2061 6e64 726f 6964 5f70 6f72 742c 2061   android_port, a
-0000db50: 6e64 726f 6964 5f66 696c 6529 0a20 2020  ndroid_file).   
-0000db60: 2020 2020 2020 2020 2069 6620 7265 7475           if retu
-0000db70: 726e 5f63 6f64 6520 213d 2030 3a0a 2020  rn_code != 0:.  
-0000db80: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000db90: 6c66 2e64 6973 706c 6179 5f6d 6573 7361  lf.display_messa
-0000dba0: 6765 5f62 6f78 2865 7272 6f72 5f6d 6573  ge_box(error_mes
-0000dbb0: 7361 6765 2c20 2252 6564 2229 0a20 2020  sage, "Red").   
-0000dbc0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000dbd0: 7572 6e20 312c 2061 6e64 726f 6964 5f69  urn 1, android_i
-0000dbe0: 7061 6464 722c 2061 6e64 726f 6964 5f70  paddr, android_p
-0000dbf0: 6f72 742c 2061 6e64 726f 6964 5f66 696c  ort, android_fil
-0000dc00: 650a 2020 2020 2020 2020 656c 7365 3a0a  e.        else:.
-0000dc10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000dc20: 726e 2031 2c20 616e 6472 6f69 645f 6970  rn 1, android_ip
-0000dc30: 6164 6472 2c20 616e 6472 6f69 645f 706f  addr, android_po
-0000dc40: 7274 2c20 616e 6472 6f69 645f 6669 6c65  rt, android_file
-0000dc50: 0a0a 2020 2020 2320 4669 6c65 206c 6f63  ..    # File loc
-0000dc60: 6174 696f 6e20 6e6f 7420 7072 6f76 6964  ation not provid
-0000dc70: 6564 2e20 2047 6574 2074 6865 206c 6973  ed.  Get the lis
-0000dc80: 7420 6f66 2061 6c6c 2058 4d4c 2066 696c  t of all XML fil
-0000dc90: 6573 2066 726f 6d20 7468 6520 416e 6472  es from the Andr
-0000dca0: 6f69 6420 6465 7669 6365 2061 6e64 2070  oid device and p
-0000dcb0: 7265 7365 6e74 2069 7420 746f 2074 6865  resent it to the
-0000dcc0: 2075 7365 722e 0a20 2020 2065 6c73 653a   user..    else:
-0000dcd0: 0a20 2020 2020 2020 2063 6c65 6172 5f61  .        clear_a
-0000dce0: 6e64 726f 6964 5f62 7574 746f 6e73 2873  ndroid_buttons(s
-0000dcf0: 656c 6629 0a20 2020 2020 2020 2023 2047  elf).        # G
-0000dd00: 6574 206c 6973 7420 6672 6f6d 2054 6173  et list from Tas
-0000dd10: 6b65 7220 6469 7265 6374 6f72 7920 282f  ker directory (/
-0000dd20: 5461 736b 6572 2920 6f72 2073 7973 7465  Tasker) or syste
-0000dd30: 6d20 6469 7265 6374 6f72 7920 282f 7374  m directory (/st
-0000dd40: 6f72 6167 652f 656d 756c 6174 6564 2f30  orage/emulated/0
-0000dd50: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000dd60: 5f63 6f64 652c 2066 696c 656c 6973 7420  _code, filelist 
-0000dd70: 3d20 6765 745f 6c69 7374 5f6f 665f 6669  = get_list_of_fi
-0000dd80: 6c65 7328 616e 6472 6f69 645f 6970 6164  les(android_ipad
-0000dd90: 6472 2c20 616e 6472 6f69 645f 706f 7274  dr, android_port
-0000dda0: 2c20 222f 7374 6f72 6167 652f 656d 756c  , "/storage/emul
-0000ddb0: 6174 6564 2f30 2f54 6173 6b65 7222 290a  ated/0/Tasker").
-0000ddc0: 2020 2020 2020 2020 6966 2072 6574 7572          if retur
-0000ddd0: 6e5f 636f 6465 2021 3d20 303a 0a20 2020  n_code != 0:.   
-0000dde0: 2020 2020 2020 2020 2023 2045 7272 6f72           # Error
-0000ddf0: 2067 6574 7469 6e67 206c 6973 7420 6f66   getting list of
-0000de00: 2066 696c 6573 2e0a 2020 2020 2020 2020   files..        
-0000de10: 2020 2020 7365 6c66 2e64 6973 706c 6179      self.display
-0000de20: 5f6d 6573 7361 6765 5f62 6f78 2866 696c  _message_box(fil
-0000de30: 656c 6973 742c 2022 5265 6422 290a 2020  elist, "Red").  
-0000de40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000de50: 2031 2c20 616e 6472 6f69 645f 6970 6164   1, android_ipad
-0000de60: 6472 2c20 616e 6472 6f69 645f 706f 7274  dr, android_port
-0000de70: 2c20 616e 6472 6f69 645f 6669 6c65 0a0a  , android_file..
-0000de80: 2020 2020 2020 2020 2320 4469 7370 6c61          # Displa
-0000de90: 7920 4669 6c65 204c 6973 7420 666f 7220  y File List for 
-0000dea0: 6669 6c65 2073 656c 6563 7469 6f6e 0a20  file selection. 
-0000deb0: 2020 2020 2020 2073 656c 662e 6669 6c65         self.file
-0000dec0: 6c69 7374 5f6c 6162 656c 203d 2061 6464  list_label = add
-0000ded0: 5f6c 6162 656c 280a 2020 2020 2020 2020  _label(.        
-0000dee0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000def0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000df00: 2020 2020 2020 2020 2253 656c 6563 7420          "Select 
-0000df10: 584d 4c20 4669 6c65 2046 726f 6d20 416e  XML File From An
-0000df20: 6472 6f69 6420 4465 7669 6365 3a22 2c0a  droid Device:",.
-0000df30: 2020 2020 2020 2020 2020 2020 2222 2c0a              "",.
-0000df40: 2020 2020 2020 2020 2020 2020 302c 0a20              0,. 
-0000df50: 2020 2020 2020 2020 2020 2022 6e6f 726d             "norm
-0000df60: 616c 222c 0a20 2020 2020 2020 2020 2020  al",.           
-0000df70: 2038 2c0a 2020 2020 2020 2020 2020 2020   8,.            
-0000df80: 312c 0a20 2020 2020 2020 2020 2020 2028  1,.            (
-0000df90: 3138 352c 2030 292c 0a20 2020 2020 2020  185, 0),.       
-0000dfa0: 2020 2020 2028 302c 2031 3029 2c0a 2020       (0, 10),.  
-0000dfb0: 2020 2020 2020 2020 2020 2273 7722 2c0a            "sw",.
-0000dfc0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000dfd0: 2020 7365 6c66 2e66 696c 656c 6973 745f    self.filelist_
-0000dfe0: 6f70 7469 6f6e 203d 2061 6464 5f6f 7074  option = add_opt
-0000dff0: 696f 6e5f 6d65 6e75 280a 2020 2020 2020  ion_menu(.      
-0000e000: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000e010: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000e020: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-0000e030: 696c 655f 7365 6c65 6374 6564 5f65 7665  ile_selected_eve
-0000e040: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
-0000e050: 6669 6c65 6c69 7374 2c0a 2020 2020 2020  filelist,.      
-0000e060: 2020 2020 2020 392c 0a20 2020 2020 2020        9,.       
-0000e070: 2020 2020 2031 2c0a 2020 2020 2020 2020       1,.        
-0000e080: 2020 2020 2831 3835 2c20 3130 292c 0a20      (185, 10),. 
-0000e090: 2020 2020 2020 2020 2020 2028 302c 2031             (0, 1
-0000e0a0: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
-0000e0b0: 226e 7722 2c0a 2020 2020 2020 2020 290a  "nw",.        ).
-0000e0c0: 0a20 2020 2020 2020 2023 2053 6574 2062  .        # Set b
-0000e0d0: 6163 6b75 7020 4950 2061 6e64 2066 696c  ackup IP and fil
-0000e0e0: 6520 6c6f 6361 7469 6f6e 2061 7474 7269  e location attri
-0000e0f0: 6275 7465 7320 6966 2076 616c 6964 0a20  butes if valid. 
-0000e100: 2020 2020 2020 2073 656c 662e 616e 6472         self.andr
-0000e110: 6f69 645f 6970 6164 6472 203d 2061 6e64  oid_ipaddr = and
-0000e120: 726f 6964 5f69 7061 6464 720a 2020 2020  roid_ipaddr.    
-0000e130: 2020 2020 7365 6c66 2e61 6e64 726f 6964      self.android
-0000e140: 5f70 6f72 7420 3d20 616e 6472 6f69 645f  _port = android_
-0000e150: 706f 7274 0a20 2020 2020 2020 2072 6574  port.        ret
-0000e160: 7572 6e20 322c 2022 222c 2022 222c 2022  urn 2, "", "", "
-0000e170: 2220 2023 204a 7573 7420 7265 7475 726e  "  # Just return
-0000e180: 2077 6974 6820 6572 726f 7220 736f 2074   with error so t
-0000e190: 6865 2070 726f 6d70 7420 636f 6d65 7320  he prompt comes 
-0000e1a0: 7570 2074 6f20 7365 6c65 6374 2066 696c  up to select fil
-0000e1b0: 652e 0a0a 2020 2020 2320 416c 6c20 6973  e...    # All is
-0000e1c0: 206f 6b61 790a 2020 2020 7265 7475 726e   okay.    return
-0000e1d0: 2030 2c20 616e 6472 6f69 645f 6970 6164   0, android_ipad
-0000e1e0: 6472 2c20 616e 6472 6f69 645f 706f 7274  dr, android_port
-0000e1f0: 2c20 616e 6472 6f69 645f 6669 6c65 0a0a  , android_file..
-0000e200: 0a23 2023 2323 2323 2323 2323 2323 2323  .# #############
-0000e210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e220: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e250: 2323 2323 230a 2320 5072 6f76 6964 6520  #####.# Provide 
-0000e260: 6120 7075 6c6c 646f 776e 206c 6973 7420  a pulldown list 
-0000e270: 666f 7220 7468 6520 7365 6c65 6374 696f  for the selectio
-0000e280: 6e20 6f66 2061 2050 726f 6669 6c65 206e  n of a Profile n
-0000e290: 616d 650a 2320 2323 2323 2323 2323 2323  ame.# ##########
-0000e2a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e2b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e2c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e2d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e2e0: 2323 2323 2323 2323 0a64 6566 206c 6973  ########.def lis
-0000e2f0: 745f 7072 6f66 696c 6573 5f61 6e64 5f74  t_profiles_and_t
-0000e300: 6173 6b73 2873 656c 6629 202d 3e20 626f  asks(self) -> bo
-0000e310: 6f6c 3a20 2023 206e 6f71 613a 2041 4e4e  ol:  # noqa: ANN
-0000e320: 3030 310a 2020 2020 2222 220a 2020 2020  001.    """.    
-0000e330: 4c69 7374 7320 7468 6520 7072 6f66 696c  Lists the profil
-0000e340: 6573 2061 6e64 2074 6173 6b73 2061 7661  es and tasks ava
-0000e350: 696c 6162 6c65 2069 6e20 7468 6520 584d  ilable in the XM
-0000e360: 4c20 6669 6c65 2e20 2054 6865 206c 6973  L file.  The lis
-0000e370: 7420 666f 7220 6561 6368 2077 696c 6c20  t for each will 
-0000e380: 6170 7065 6172 2069 6e20 6120 7075 6c6c  appear in a pull
-0000e390: 646f 776e 206f 7074 696f 6e20 6c69 7374  down option list
-0000e3a0: 2e0a 0a20 2020 2054 6869 7320 6675 6e63  ...    This func
-0000e3b0: 7469 6f6e 2063 6865 636b 7320 6966 2074  tion checks if t
-0000e3c0: 6865 2058 4d4c 2066 696c 6520 6861 7320  he XML file has 
-0000e3d0: 616c 7265 6164 7920 6265 656e 206c 6f61  already been loa
-0000e3e0: 6465 642e 2049 6620 6e6f 742c 2069 7420  ded. If not, it 
-0000e3f0: 6c6f 6164 7320 7468 6520 584d 4c20 6669  loads the XML fi
-0000e400: 6c65 2061 6e64 2062 7569 6c64 7320 7468  le and builds th
-0000e410: 6520 7472 6565 2064 6174 612e 0a20 2020  e tree data..   
-0000e420: 2054 6865 6e2c 2069 7420 676f 6573 2074   Then, it goes t
-0000e430: 6872 6f75 6768 2065 6163 6820 7072 6f6a  hrough each proj
-0000e440: 6563 7420 616e 6420 7265 7472 6965 7665  ect and retrieve
-0000e450: 7320 616c 6c20 7468 6520 7072 6f66 696c  s all the profil
-0000e460: 6520 6e61 6d65 7320 616e 6420 7461 736b  e names and task
-0000e470: 732e 0a20 2020 2054 6865 2070 726f 6669  s..    The profi
-0000e480: 6c65 206e 616d 6573 2061 6e64 2074 6173  le names and tas
-0000e490: 6b73 2061 7265 2063 6c65 616e 6564 2075  ks are cleaned u
-0000e4a0: 7020 6279 2072 656d 6f76 696e 6720 7468  p by removing th
-0000e4b0: 6520 2250 726f 6669 6c65 3a20 556e 6e61  e "Profile: Unna
-0000e4c0: 6d65 642f 416e 6f6e 796d 6f75 7322 2061  med/Anonymous" a
-0000e4d0: 6e64 2022 5461 736b 3a20 556e 6e61 6d65  nd "Task: Unname
-0000e4e0: 642f 416e 6f6e 796d 6f75 732e 2220 656e  d/Anonymous." en
-0000e4f0: 7472 6965 732e 0a20 2020 2049 6620 7468  tries..    If th
-0000e500: 6572 6520 6172 6520 6e6f 2070 726f 6669  ere are no profi
-0000e510: 6c65 7320 6f72 2074 6173 6b73 2066 6f75  les or tasks fou
-0000e520: 6e64 2c20 6120 6d65 7373 6167 6520 626f  nd, a message bo
-0000e530: 7820 6973 2064 6973 706c 6179 6564 2061  x is displayed a
-0000e540: 6e64 2074 6865 2066 756e 6374 696f 6e20  nd the function 
-0000e550: 7265 7475 726e 7320 4661 6c73 652e 0a20  returns False.. 
-0000e560: 2020 2054 6865 2070 726f 6669 6c65 206e     The profile n
-0000e570: 616d 6573 2061 6e64 2074 6173 6b73 2061  ames and tasks a
-0000e580: 7265 2074 6865 6e20 736f 7274 6564 2061  re then sorted a
-0000e590: 6c70 6861 6265 7469 6361 6c6c 7920 616e  lphabetically an
-0000e5a0: 6420 6475 706c 6963 6174 6573 2061 7265  d duplicates are
-0000e5b0: 2072 656d 6f76 6564 2e0a 2020 2020 5468   removed..    Th
-0000e5c0: 6520 7072 6f66 696c 6520 6e61 6d65 7320  e profile names 
-0000e5d0: 6172 6520 6469 7370 6c61 7965 6420 696e  are displayed in
-0000e5e0: 2061 206c 6162 656c 2066 6f72 2073 656c   a label for sel
-0000e5f0: 6563 7469 6f6e 2c20 616e 6420 7468 6520  ection, and the 
-0000e600: 636f 7272 6573 706f 6e64 696e 6720 7461  corresponding ta
-0000e610: 736b 7320 6172 6520 6469 7370 6c61 7965  sks are displaye
-0000e620: 6420 696e 2061 6e6f 7468 6572 206c 6162  d in another lab
-0000e630: 656c 2066 6f72 2073 656c 6563 7469 6f6e  el for selection
-0000e640: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
-0000e650: 2020 2020 2020 2020 626f 6f6c 3a20 5472          bool: Tr
-0000e660: 7565 2069 6620 7468 6520 584d 4c20 6669  ue if the XML fi
-0000e670: 6c65 2068 6173 2050 726f 6669 6c65 7320  le has Profiles 
-0000e680: 6f72 2054 6173 6b73 2c20 4661 6c73 6520  or Tasks, False 
-0000e690: 6f74 6865 7277 6973 652e 0a20 2020 2022  otherwise..    "
-0000e6a0: 2222 0a20 2020 2023 2044 6f20 7765 2061  "".    # Do we a
-0000e6b0: 6c72 6561 6479 2068 6176 6520 7468 6520  lready have the 
-0000e6c0: 584d 4c3f 0a20 2020 2023 2049 6620 7765  XML?.    # If we
-0000e6d0: 2064 6f6e 2774 2068 6176 6520 616e 7920   don't have any 
-0000e6e0: 6461 7461 2c20 6765 7420 6974 2e0a 2020  data, get it..  
-0000e6f0: 2020 6966 206e 6f74 2073 656c 662e 6c6f    if not self.lo
-0000e700: 6164 5f78 6d6c 2829 3a0a 2020 2020 2020  ad_xml():.      
-0000e710: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-0000e720: 2020 2020 7072 6f66 696c 6573 203d 205b      profiles = [
-0000e730: 5d0a 2020 2020 7461 736b 7320 3d20 5b5d  ].    tasks = []
-0000e740: 0a0a 2020 2020 2320 4f6b 2c20 7765 2068  ..    # Ok, we h
-0000e750: 6176 6520 6f75 7220 726f 6f74 2054 6173  ave our root Tas
-0000e760: 6b65 7220 656c 656d 656e 7473 2e20 2042  ker elements.  B
-0000e770: 7569 6c64 2074 6865 2074 7265 652e 0a20  uild the tree.. 
-0000e780: 2020 2074 7265 655f 6461 7461 203d 2073     tree_data = s
-0000e790: 656c 662e 6275 696c 645f 7468 655f 7472  elf.build_the_tr
-0000e7a0: 6565 2829 0a20 2020 2023 2049 6620 6e6f  ee().    # If no
-0000e7b0: 2074 7265 652c 2074 6865 6e20 7468 6572   tree, then ther
-0000e7c0: 6520 6172 6520 6e6f 2050 726f 6a65 6374  e are no Project
-0000e7d0: 7320 696e 2074 6865 2058 4d4c 2e0a 2020  s in the XML..  
-0000e7e0: 2020 6966 206e 6f74 2074 7265 655f 6461    if not tree_da
-0000e7f0: 7461 3a0a 2020 2020 2020 2020 6966 2050  ta:.        if P
-0000e800: 7269 6d65 4974 656d 732e 7461 736b 6572  rimeItems.tasker
-0000e810: 5f72 6f6f 745f 656c 656d 656e 7473 5b22  _root_elements["
-0000e820: 616c 6c5f 7072 6f66 696c 6573 225d 3a0a  all_profiles"]:.
-0000e830: 2020 2020 2020 2020 2020 2020 7072 6f66              prof
-0000e840: 696c 6573 203d 205b 7661 6c75 655b 226e  iles = [value["n
-0000e850: 616d 6522 5d20 666f 7220 7661 6c75 6520  ame"] for value 
-0000e860: 696e 2050 7269 6d65 4974 656d 732e 7461  in PrimeItems.ta
-0000e870: 736b 6572 5f72 6f6f 745f 656c 656d 656e  sker_root_elemen
-0000e880: 7473 5b22 616c 6c5f 7072 6f66 696c 6573  ts["all_profiles
-0000e890: 225d 2e76 616c 7565 7328 295d 0a20 2020  "].values()].   
-0000e8a0: 2020 2020 2069 6620 5072 696d 6549 7465       if PrimeIte
-0000e8b0: 6d73 2e74 6173 6b65 725f 726f 6f74 5f65  ms.tasker_root_e
-0000e8c0: 6c65 6d65 6e74 735b 2261 6c6c 5f74 6173  lements["all_tas
-0000e8d0: 6b73 225d 3a0a 2020 2020 2020 2020 2020  ks"]:.          
-0000e8e0: 2020 7461 736b 7320 3d20 5b76 616c 7565    tasks = [value
-0000e8f0: 5b22 6e61 6d65 225d 2066 6f72 2076 616c  ["name"] for val
-0000e900: 7565 2069 6e20 5072 696d 6549 7465 6d73  ue in PrimeItems
-0000e910: 2e74 6173 6b65 725f 726f 6f74 5f65 6c65  .tasker_root_ele
-0000e920: 6d65 6e74 735b 2261 6c6c 5f74 6173 6b73  ments["all_tasks
-0000e930: 225d 2e76 616c 7565 7328 295d 0a0a 2020  "].values()]..  
-0000e940: 2020 2020 2020 2320 7365 6c66 2e64 6973        # self.dis
-0000e950: 706c 6179 5f6d 6573 7361 6765 5f62 6f78  play_message_box
-0000e960: 2822 4e6f 2050 726f 6a65 6374 7320 666f  ("No Projects fo
-0000e970: 756e 6420 696e 2058 4d4c 2066 696c 652e  und in XML file.
-0000e980: 2020 4c6f 6164 2061 6e6f 7468 6572 2058    Load another X
-0000e990: 4d4c 2066 696c 6520 7769 7468 2061 7420  ML file with at 
-0000e9a0: 6c65 6173 7420 6f6e 6520 5072 6f6a 6563  least one Projec
-0000e9b0: 7420 616e 6420 7472 7920 6167 6169 6e2e  t and try again.
-0000e9c0: 222c 2022 5265 6422 290a 2020 2020 2020  ", "Red").      
-0000e9d0: 2020 2320 7265 7475 726e 2046 616c 7365    # return False
-0000e9e0: 0a0a 2020 2020 2320 5765 2068 6176 6520  ..    # We have 
-0000e9f0: 6120 7472 6565 4275 696c 6420 6f75 7220  a treeBuild our 
-0000ea00: 6c69 7374 206f 6620 5072 6f66 696c 6573  list of Profiles
-0000ea10: 2061 6e64 2054 6173 6b73 2069 6e20 7468   and Tasks in th
-0000ea20: 6520 5072 6f6a 6563 7473 2e0a 2020 2020  e Projects..    
-0000ea30: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
-0000ea40: 476f 2074 6872 6f75 6768 2074 6865 2050  Go through the P
-0000ea50: 726f 6a65 6374 7320 616e 6420 6765 7420  rojects and get 
-0000ea60: 616c 6c20 6f66 2074 6865 2050 726f 6669  all of the Profi
-0000ea70: 6c65 206e 616d 6573 2e0a 2020 2020 2020  le names..      
-0000ea80: 2020 666f 7220 7072 6f6a 6563 7420 696e    for project in
-0000ea90: 2074 7265 655f 6461 7461 3a0a 2020 2020   tree_data:.    
-0000eaa0: 2020 2020 2020 2020 666f 7220 7072 6f66          for prof
-0000eab0: 696c 6520 696e 2070 726f 6a65 6374 5b22  ile in project["
-0000eac0: 6368 696c 6472 656e 225d 3a0a 2020 2020  children"]:.    
-0000ead0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000eae0: 2063 6f6e 7465 7874 6c69 622e 7375 7070   contextlib.supp
-0000eaf0: 7265 7373 2854 7970 6545 7272 6f72 293a  ress(TypeError):
-0000eb00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eb10: 2020 2020 2070 726f 6669 6c65 732e 6170       profiles.ap
-0000eb20: 7065 6e64 2870 726f 6669 6c65 5b22 6e61  pend(profile["na
-0000eb30: 6d65 225d 290a 2020 2020 2020 2020 2020  me"]).          
-0000eb40: 2020 2020 2020 2020 2020 7461 736b 732e            tasks.
-0000eb50: 6578 7465 6e64 2870 726f 6669 6c65 5b22  extend(profile["
-0000eb60: 6368 696c 6472 656e 225d 290a 0a20 2020  children"])..   
-0000eb70: 2023 2043 6c65 616e 7570 2074 6865 206c   # Cleanup the l
-0000eb80: 6973 7473 0a20 2020 2068 6176 655f 7072  ists.    have_pr
-0000eb90: 6f66 696c 6573 203d 2068 6176 655f 7461  ofiles = have_ta
-0000eba0: 736b 7320 3d20 5472 7565 2020 2320 4173  sks = True  # As
-0000ebb0: 7375 6d65 2077 6520 6861 7665 2050 726f  sume we have Pro
-0000ebc0: 6669 6c65 7320 616e 6420 5461 736b 730a  files and Tasks.
-0000ebd0: 2020 2020 7072 6f66 696c 6573 5f74 6f5f      profiles_to_
-0000ebe0: 6469 7370 6c61 7920 3d20 5b70 726f 6669  display = [profi
-0000ebf0: 6c65 2066 6f72 2070 726f 6669 6c65 2069  le for profile i
-0000ec00: 6e20 7072 6f66 696c 6573 2069 6620 7072  n profiles if pr
-0000ec10: 6f66 696c 6520 213d 2022 5072 6f66 696c  ofile != "Profil
-0000ec20: 653a 2055 6e6e 616d 6564 2f41 6e6f 6e79  e: Unnamed/Anony
-0000ec30: 6d6f 7573 225d 0a20 2020 2069 6620 6e6f  mous"].    if no
-0000ec40: 7420 7072 6f66 696c 6573 5f74 6f5f 6469  t profiles_to_di
-0000ec50: 7370 6c61 793a 0a20 2020 2020 2020 2070  splay:.        p
-0000ec60: 726f 6669 6c65 735f 746f 5f64 6973 706c  rofiles_to_displ
-0000ec70: 6179 203d 205b 224e 6f20 7072 6f66 696c  ay = ["No profil
-0000ec80: 6573 2066 6f75 6e64 225d 0a20 2020 2020  es found"].     
-0000ec90: 2020 2068 6176 655f 7072 6f66 696c 6573     have_profiles
-0000eca0: 203d 2046 616c 7365 0a20 2020 2074 6173   = False.    tas
-0000ecb0: 6b73 5f74 6f5f 6469 7370 6c61 7920 3d20  ks_to_display = 
-0000ecc0: 5b74 6173 6b20 666f 7220 7461 736b 2069  [task for task i
-0000ecd0: 6e20 7461 736b 7320 6966 2074 6173 6b20  n tasks if task 
-0000ece0: 213d 2022 5461 736b 3a20 556e 6e61 6d65  != "Task: Unname
-0000ecf0: 642f 416e 6f6e 796d 6f75 732e 225d 0a20  d/Anonymous."]. 
-0000ed00: 2020 2069 6620 6e6f 7420 7461 736b 735f     if not tasks_
-0000ed10: 746f 5f64 6973 706c 6179 3a0a 2020 2020  to_display:.    
-0000ed20: 2020 2020 7461 736b 735f 746f 5f64 6973      tasks_to_dis
-0000ed30: 706c 6179 203d 205b 224e 6f20 7461 736b  play = ["No task
-0000ed40: 7320 666f 756e 6422 5d0a 2020 2020 2020  s found"].      
-0000ed50: 2020 6861 7665 5f74 6173 6b73 203d 2046    have_tasks = F
-0000ed60: 616c 7365 0a20 2020 2069 6620 6e6f 7420  alse.    if not 
-0000ed70: 6861 7665 5f70 726f 6669 6c65 7320 616e  have_profiles an
-0000ed80: 6420 6e6f 7420 6861 7665 5f74 6173 6b73  d not have_tasks
-0000ed90: 3a0a 2020 2020 2020 2020 7365 6c66 2e64  :.        self.d
-0000eda0: 6973 706c 6179 5f6d 6573 7361 6765 5f62  isplay_message_b
-0000edb0: 6f78 280a 2020 2020 2020 2020 2020 2020  ox(.            
-0000edc0: 224e 6f20 7072 6f66 696c 6573 206f 7220  "No profiles or 
-0000edd0: 7461 736b 7320 666f 756e 6420 696e 2058  tasks found in X
-0000ede0: 4d4c 2066 696c 652e 2020 5573 696e 6720  ML file.  Using 
-0000edf0: 7468 6520 2747 6574 204c 6f63 616c 2058  the 'Get Local X
-0000ee00: 6d6c 2062 7574 746f 6e2c 206c 6f61 6420  ml button, load 
-0000ee10: 616e 6f74 6865 7220 584d 4c20 6669 6c65  another XML file
-0000ee20: 2061 6e64 2074 7279 2061 6761 696e 2e22   and try again."
-0000ee30: 2c0a 2020 2020 2020 2020 2020 2020 2252  ,.            "R
-0000ee40: 6564 222c 0a20 2020 2020 2020 2029 0a20  ed",.        ). 
-0000ee50: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-0000ee60: 6c73 650a 0a20 2020 2023 204d 616b 6520  lse..    # Make 
-0000ee70: 616c 7068 6162 6574 6963 616c 0a20 2020  alphabetical.   
-0000ee80: 2070 726f 6669 6c65 735f 746f 5f64 6973   profiles_to_dis
-0000ee90: 706c 6179 203d 2073 6f72 7465 6428 7072  play = sorted(pr
-0000eea0: 6f66 696c 6573 5f74 6f5f 6469 7370 6c61  ofiles_to_displa
-0000eeb0: 7929 0a20 2020 2070 726f 6669 6c65 735f  y).    profiles_
-0000eec0: 746f 5f64 6973 706c 6179 2e69 6e73 6572  to_display.inser
-0000eed0: 7428 302c 2022 4e6f 6e65 2229 0a0a 2020  t(0, "None")..  
-0000eee0: 2020 2320 5265 6d6f 7665 2064 7570 7320    # Remove dups 
-0000eef0: 6672 6f6d 2054 6173 6b73 2061 6e64 2073  from Tasks and s
-0000ef00: 6f72 7420 7468 656d 0a20 2020 2074 6173  ort them.    tas
-0000ef10: 6b73 5f74 6f5f 6469 7370 6c61 7920 3d20  ks_to_display = 
-0000ef20: 6c69 7374 2873 6574 2874 6173 6b73 5f74  list(set(tasks_t
-0000ef30: 6f5f 6469 7370 6c61 7929 290a 2020 2020  o_display)).    
-0000ef40: 7461 736b 735f 746f 5f64 6973 706c 6179  tasks_to_display
-0000ef50: 203d 2073 6f72 7465 6428 7461 736b 735f   = sorted(tasks_
-0000ef60: 746f 5f64 6973 706c 6179 290a 2020 2020  to_display).    
-0000ef70: 7461 736b 735f 746f 5f64 6973 706c 6179  tasks_to_display
-0000ef80: 2e69 6e73 6572 7428 302c 2022 4e6f 6e65  .insert(0, "None
-0000ef90: 2229 0a0a 2020 2020 2320 4469 7370 6c61  ")..    # Displa
-0000efa0: 7920 616c 6c20 6f66 2074 6865 2050 726f  y all of the Pro
-0000efb0: 6669 6c65 7320 666f 7220 7365 6c65 6374  files for select
-0000efc0: 696f 6e2e 0a20 2020 2073 656c 662e 6169  ion..    self.ai
-0000efd0: 5f70 726f 6669 6c65 5f6c 6162 656c 203d  _profile_label =
-0000efe0: 2061 6464 5f6c 6162 656c 280a 2020 2020   add_label(.    
-0000eff0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000f000: 2020 7365 6c66 2e74 6162 7669 6577 2e74    self.tabview.t
-0000f010: 6162 2822 416e 616c 797a 6522 292c 0a20  ab("Analyze"),. 
-0000f020: 2020 2020 2020 2022 5365 6c65 6374 2050         "Select P
-0000f030: 726f 6669 6c65 2074 6f20 416e 616c 797a  rofile to Analyz
-0000f040: 653a 222c 0a20 2020 2020 2020 2022 222c  e:",.        "",
-0000f050: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
-0000f060: 2020 2020 226e 6f72 6d61 6c22 2c0a 2020      "normal",.  
-0000f070: 2020 2020 2020 362c 0a20 2020 2020 2020        6,.       
-0000f080: 2030 2c0a 2020 2020 2020 2020 3230 2c0a   0,.        20,.
-0000f090: 2020 2020 2020 2020 2832 302c 2030 292c          (20, 0),
-0000f0a0: 0a20 2020 2020 2020 2022 7322 2c0a 2020  .        "s",.  
-0000f0b0: 2020 290a 2020 2020 2320 4765 7420 7468    ).    # Get th
-0000f0c0: 6520 7072 6f6a 6563 7420 6465 7369 7265  e project desire
-0000f0d0: 640a 2020 2020 7365 6c66 2e70 726f 6669  d.    self.profi
-0000f0e0: 6c65 5f6f 7074 696f 6e65 6d65 6e75 203d  le_optionemenu =
-0000f0f0: 2061 6464 5f6f 7074 696f 6e5f 6d65 6e75   add_option_menu
-0000f100: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000f110: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
-0000f120: 7669 6577 2e74 6162 2822 416e 616c 797a  view.tab("Analyz
-0000f130: 6522 292c 0a20 2020 2020 2020 2073 656c  e"),.        sel
-0000f140: 662e 6169 5f70 726f 6669 6c65 5f73 656c  f.ai_profile_sel
-0000f150: 6563 7465 645f 6576 656e 742c 0a20 2020  ected_event,.   
-0000f160: 2020 2020 2070 726f 6669 6c65 735f 746f       profiles_to
-0000f170: 5f64 6973 706c 6179 2c0a 2020 2020 2020  _display,.      
-0000f180: 2020 372c 0a20 2020 2020 2020 2030 2c0a    7,.        0,.
-0000f190: 2020 2020 2020 2020 3230 2c0a 2020 2020          20,.    
-0000f1a0: 2020 2020 2830 2c20 3130 292c 0a20 2020      (0, 10),.   
-0000f1b0: 2020 2020 2022 6e22 2c0a 2020 2020 290a       "n",.    ).
-0000f1c0: 0a20 2020 2023 2044 6973 706c 6179 2061  .    # Display a
-0000f1d0: 6c6c 206f 6620 7468 6520 5461 736b 7320  ll of the Tasks 
-0000f1e0: 666f 7220 7365 6c65 6374 696f 6e2e 0a20  for selection.. 
-0000f1f0: 2020 2073 656c 662e 6169 5f74 6173 6b5f     self.ai_task_
-0000f200: 6c61 6265 6c20 3d20 6164 645f 6c61 6265  label = add_labe
-0000f210: 6c28 0a20 2020 2020 2020 2073 656c 662c  l(.        self,
-0000f220: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0000f230: 6276 6965 772e 7461 6228 2241 6e61 6c79  bview.tab("Analy
-0000f240: 7a65 2229 2c0a 2020 2020 2020 2020 2253  ze"),.        "S
-0000f250: 656c 6563 7420 5461 736b 2074 6f20 416e  elect Task to An
-0000f260: 616c 797a 653a 222c 0a20 2020 2020 2020  alyze:",.       
-0000f270: 2022 222c 0a20 2020 2020 2020 2030 2c0a   "",.        0,.
-0000f280: 2020 2020 2020 2020 226e 6f72 6d61 6c22          "normal"
-0000f290: 2c0a 2020 2020 2020 2020 382c 0a20 2020  ,.        8,.   
-0000f2a0: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
-0000f2b0: 3230 2c0a 2020 2020 2020 2020 2832 302c  20,.        (20,
-0000f2c0: 2030 292c 0a20 2020 2020 2020 2022 7322   0),.        "s"
-0000f2d0: 2c0a 2020 2020 290a 2020 2020 2320 4765  ,.    ).    # Ge
-0000f2e0: 7420 7468 6520 7072 6f6a 6563 7420 6465  t the project de
-0000f2f0: 7369 7265 640a 2020 2020 7365 6c66 2e74  sired.    self.t
-0000f300: 6173 6b5f 6f70 7469 6f6e 656d 656e 7520  ask_optionemenu 
-0000f310: 3d20 6164 645f 6f70 7469 6f6e 5f6d 656e  = add_option_men
-0000f320: 7528 0a20 2020 2020 2020 2073 656c 662c  u(.        self,
-0000f330: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0000f340: 6276 6965 772e 7461 6228 2241 6e61 6c79  bview.tab("Analy
-0000f350: 7a65 2229 2c0a 2020 2020 2020 2020 7365  ze"),.        se
-0000f360: 6c66 2e61 695f 7461 736b 5f73 656c 6563  lf.ai_task_selec
-0000f370: 7465 645f 6576 656e 742c 0a20 2020 2020  ted_event,.     
-0000f380: 2020 2074 6173 6b73 5f74 6f5f 6469 7370     tasks_to_disp
-0000f390: 6c61 792c 0a20 2020 2020 2020 2039 2c0a  lay,.        9,.
-0000f3a0: 2020 2020 2020 2020 302c 0a20 2020 2020          0,.     
-0000f3b0: 2020 2032 302c 0a20 2020 2020 2020 2028     20,.        (
-0000f3c0: 302c 2031 3029 2c0a 2020 2020 2020 2020  0, 10),.        
-0000f3d0: 226e 222c 0a20 2020 2029 0a0a 2020 2020  "n",.    )..    
-0000f3e0: 7265 7475 726e 2054 7275 650a 0a0a 2320  return True...# 
-0000f3f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f420: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f430: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f440: 2323 0a23 2042 7569 6c64 2061 206c 6973  ##.# Build a lis
-0000f450: 7420 6f66 2050 726f 6669 6c65 7320 7468  t of Profiles th
-0000f460: 6174 2061 7265 2075 6e64 6572 2074 6865  at are under the
-0000f470: 2067 6976 656e 2070 726f 6a65 6374 0a23   given project.#
-0000f480: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-0000f490: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f4a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f4b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f4c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f4d0: 2323 230a 6465 6620 6275 696c 645f 7072  ###.def build_pr
-0000f4e0: 6f66 696c 6573 2872 6f6f 743a 2064 6963  ofiles(root: dic
-0000f4f0: 742c 2070 726f 6669 6c65 5f69 6473 3a20  t, profile_ids: 
-0000f500: 6c69 7374 2920 2d3e 206c 6973 743a 0a20  list) -> list:. 
-0000f510: 2020 2022 2222 5061 7261 6d65 7465 7273     """Parameters
-0000f520: 3a0a 2020 2020 2020 2020 2d20 726f 6f74  :.        - root
-0000f530: 2028 6469 6374 293a 2044 6963 7469 6f6e   (dict): Diction
-0000f540: 6172 7920 636f 6e74 6169 6e69 6e67 2061  ary containing a
-0000f550: 6c6c 2070 726f 6669 6c65 7320 616e 6420  ll profiles and 
-0000f560: 7468 6569 7220 7461 736b 732e 0a20 2020  their tasks..   
-0000f570: 2020 2020 202d 2070 726f 6669 6c65 5f69       - profile_i
-0000f580: 6473 2028 6c69 7374 293a 204c 6973 7420  ds (list): List 
-0000f590: 6f66 2070 726f 6669 6c65 2049 4473 2074  of profile IDs t
-0000f5a0: 6f20 6265 2070 726f 6365 7373 6564 2e0a  o be processed..
-0000f5b0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0000f5c0: 2020 2020 202d 206c 6973 743a 204c 6973       - list: Lis
-0000f5d0: 7420 6f66 2064 6963 7469 6f6e 6172 6965  t of dictionarie
-0000f5e0: 7320 636f 6e74 6169 6e69 6e67 2070 726f  s containing pro
-0000f5f0: 6669 6c65 206e 616d 6573 2061 6e64 2074  file names and t
-0000f600: 6865 6972 2063 6f72 7265 7370 6f6e 6469  heir correspondi
-0000f610: 6e67 2074 6173 6b73 2e0a 2020 2020 5072  ng tasks..    Pr
-0000f620: 6f63 6573 7369 6e67 204c 6f67 6963 3a0a  ocessing Logic:.
-0000f630: 2020 2020 2020 2020 2d20 4765 7420 616c          - Get al
-0000f640: 6c20 7072 6f66 696c 6573 2066 726f 6d20  l profiles from 
-0000f650: 726f 6f74 2064 6963 7469 6f6e 6172 792e  root dictionary.
-0000f660: 0a20 2020 2020 2020 202d 2043 7265 6174  .        - Creat
-0000f670: 6520 616e 2065 6d70 7479 206c 6973 7420  e an empty list 
-0000f680: 746f 2073 746f 7265 2070 726f 6669 6c65  to store profile
-0000f690: 206e 616d 6573 2061 6e64 2074 6173 6b73   names and tasks
-0000f6a0: 2e0a 2020 2020 2020 2020 2d20 4c6f 6f70  ..        - Loop
-0000f6b0: 2074 6872 6f75 6768 2065 6163 6820 7072   through each pr
-0000f6c0: 6f66 696c 6520 4944 2069 6e20 7468 6520  ofile ID in the 
-0000f6d0: 7072 6f76 6964 6564 206c 6973 742e 0a20  provided list.. 
-0000f6e0: 2020 2020 2020 202d 2047 6574 2074 6865         - Get the
-0000f6f0: 2074 6173 6b73 2066 6f72 2074 6865 2063   tasks for the c
-0000f700: 7572 7265 6e74 2070 726f 6669 6c65 2e0a  urrent profile..
-0000f710: 2020 2020 2020 2020 2d20 4966 2074 6173          - If tas
-0000f720: 6b73 2061 7265 2066 6f75 6e64 2c20 6372  ks are found, cr
-0000f730: 6561 7465 2061 206c 6973 7420 746f 2073  eate a list to s
-0000f740: 746f 7265 2074 6173 6b20 6e61 6d65 732e  tore task names.
-0000f750: 0a20 2020 2020 2020 202d 204c 6f6f 7020  .        - Loop 
-0000f760: 7468 726f 7567 6820 6561 6368 2074 6173  through each tas
-0000f770: 6b20 616e 6420 6164 6420 6974 7320 6e61  k and add its na
-0000f780: 6d65 2074 6f20 7468 6520 7461 736b 206c  me to the task l
-0000f790: 6973 742e 0a20 2020 2020 2020 202d 2049  ist..        - I
-0000f7a0: 6620 6e6f 2074 6173 6b73 2061 7265 2066  f no tasks are f
-0000f7b0: 6f75 6e64 2c20 6164 6420 6120 6465 6661  ound, add a defa
-0000f7c0: 756c 7420 6d65 7373 6167 6520 746f 2074  ult message to t
-0000f7d0: 6865 2074 6173 6b20 6c69 7374 2e0a 2020  he task list..  
-0000f7e0: 2020 2020 2020 2d20 4765 7420 7468 6520        - Get the 
-0000f7f0: 6e61 6d65 206f 6620 7468 6520 6375 7272  name of the curr
-0000f800: 656e 7420 7072 6f66 696c 652e 0a20 2020  ent profile..   
-0000f810: 2020 2020 202d 2049 6620 6e6f 206e 616d       - If no nam
-0000f820: 6520 6973 2066 6f75 6e64 2c20 6164 6420  e is found, add 
-0000f830: 6120 6465 6661 756c 7420 6d65 7373 6167  a default messag
-0000f840: 6520 746f 2074 6865 2070 726f 6669 6c65  e to the profile
-0000f850: 206e 616d 652e 0a20 2020 2020 2020 202d   name..        -
-0000f860: 2043 6f6d 6269 6e65 2074 6865 2070 726f   Combine the pro
-0000f870: 6669 6c65 206e 616d 6520 616e 6420 7461  file name and ta
-0000f880: 736b 206c 6973 7420 696e 746f 2061 2064  sk list into a d
-0000f890: 6963 7469 6f6e 6172 7920 616e 6420 6164  ictionary and ad
-0000f8a0: 6420 6974 2074 6f20 7468 6520 7072 6f66  d it to the prof
-0000f8b0: 696c 6520 6c69 7374 2e0a 2020 2020 2020  ile list..      
-0000f8c0: 2020 2d20 5265 7475 726e 2074 6865 2070    - Return the p
-0000f8d0: 726f 6669 6c65 206c 6973 742e 2222 220a  rofile list.""".
-0000f8e0: 2020 2020 7072 6f66 696c 6573 203d 2072      profiles = r
-0000f8f0: 6f6f 745b 2261 6c6c 5f70 726f 6669 6c65  oot["all_profile
-0000f900: 7322 5d0a 2020 2020 7072 6f66 696c 655f  s"].    profile_
-0000f910: 6c69 7374 203d 205b 5d0a 2020 2020 666f  list = [].    fo
-0000f920: 7220 7072 6f66 696c 6520 696e 2070 726f  r profile in pro
-0000f930: 6669 6c65 5f69 6473 3a0a 2020 2020 2020  file_ids:.      
-0000f940: 2020 2320 4765 7420 7468 6520 5072 6f66    # Get the Prof
-0000f950: 696c 6527 7320 5461 736b 730a 2020 2020  ile's Tasks.    
-0000f960: 2020 2020 5072 696d 6549 7465 6d73 2e74      PrimeItems.t
-0000f970: 6173 6b5f 636f 756e 745f 756e 6e61 6d65  ask_count_unname
-0000f980: 6420 3d20 3020 2023 2041 766f 6964 2061  d = 0  # Avoid a
-0000f990: 6e20 6572 726f 7220 696e 2067 6574 5f70  n error in get_p
-0000f9a0: 726f 6669 6c65 5f74 6173 6b73 0a20 2020  rofile_tasks.   
-0000f9b0: 2020 2020 2069 6620 7468 655f 7461 736b       if the_task
-0000f9c0: 7320 3a3d 2067 6574 5f70 726f 6669 6c65  s := get_profile
-0000f9d0: 5f74 6173 6b73 2870 726f 6669 6c65 735b  _tasks(profiles[
-0000f9e0: 7072 6f66 696c 655d 5b22 786d 6c22 5d2c  profile]["xml"],
-0000f9f0: 205b 5d2c 205b 5d29 3a0a 2020 2020 2020   [], []):.      
-0000fa00: 2020 2020 2020 7461 736b 5f6c 6973 7420        task_list 
-0000fa10: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-0000fa20: 2023 2050 726f 6365 7373 2065 6163 6820   # Process each 
-0000fa30: 5461 736b 2e20 2054 6173 6b73 2061 7265  Task.  Tasks are
-0000fa40: 2073 696d 706c 7920 6120 666c 6174 206c   simply a flat l
-0000fa50: 6973 7420 6f66 206e 616d 6573 2e0a 2020  ist of names..  
-0000fa60: 2020 2020 2020 2020 2020 666f 7220 7461            for ta
-0000fa70: 736b 2069 6e20 7468 655f 7461 736b 733a  sk in the_tasks:
-0000fa80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fa90: 2069 6620 7461 736b 5b22 6e61 6d65 225d   if task["name"]
-0000faa0: 203d 3d20 2222 3a0a 2020 2020 2020 2020   == "":.        
-0000fab0: 2020 2020 2020 2020 2020 2020 7461 736b              task
-0000fac0: 5f6c 6973 742e 6170 7065 6e64 2822 5461  _list.append("Ta
-0000fad0: 736b 3a20 556e 6e61 6d65 6420 5461 736b  sk: Unnamed Task
-0000fae0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0000faf0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000fb00: 2020 2020 2020 2020 2020 2020 2074 6173               tas
-0000fb10: 6b5f 6c69 7374 2e61 7070 656e 6428 6627  k_list.append(f'
-0000fb20: 5461 736b 3a20 7b74 6173 6b5b 226e 616d  Task: {task["nam
-0000fb30: 6522 5d7d 2729 0a20 2020 2020 2020 2065  e"]}').        e
-0000fb40: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000fb50: 2074 6173 6b5f 6c69 7374 203d 205b 224e   task_list = ["N
-0000fb60: 6f20 5072 6f66 696c 6520 5461 736b 7320  o Profile Tasks 
-0000fb70: 466f 756e 6422 5d0a 0a20 2020 2020 2020  Found"]..       
-0000fb80: 2023 2047 6574 2074 6865 2050 726f 6669   # Get the Profi
-0000fb90: 6c65 206e 616d 652e 0a20 2020 2020 2020  le name..       
-0000fba0: 2069 6620 7072 6f66 696c 6573 5b70 726f   if profiles[pro
-0000fbb0: 6669 6c65 5d5b 226e 616d 6522 5d20 3d3d  file]["name"] ==
-0000fbc0: 2022 223a 0a20 2020 2020 2020 2020 2020   "":.           
-0000fbd0: 2070 726f 6669 6c65 5f6e 616d 6520 3d20   profile_name = 
-0000fbe0: 2250 726f 6669 6c65 3a20 556e 6e61 6d65  "Profile: Unname
-0000fbf0: 642f 416e 6f6e 796d 6f75 7322 0a20 2020  d/Anonymous".   
-0000fc00: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000fc10: 2020 2020 2020 2070 726f 6669 6c65 5f6e         profile_n
-0000fc20: 616d 6520 3d20 6627 5072 6f66 696c 653a  ame = f'Profile:
-0000fc30: 207b 7072 6f66 696c 6573 5b70 726f 6669   {profiles[profi
-0000fc40: 6c65 5d5b 226e 616d 6522 5d7d 270a 0a20  le]["name"]}'.. 
-0000fc50: 2020 2020 2020 2023 2043 6f6d 6269 6e65         # Combine
-0000fc60: 2074 6865 2050 726f 6669 6c65 2077 6974   the Profile wit
-0000fc70: 6820 6974 2773 2054 6173 6b73 0a20 2020  h it's Tasks.   
-0000fc80: 2020 2020 2070 726f 6669 6c65 5f6c 6973       profile_lis
-0000fc90: 742e 6170 7065 6e64 287b 226e 616d 6522  t.append({"name"
-0000fca0: 3a20 7072 6f66 696c 655f 6e61 6d65 2c20  : profile_name, 
-0000fcb0: 2263 6869 6c64 7265 6e22 3a20 7461 736b  "children": task
-0000fcc0: 5f6c 6973 747d 290a 0a20 2020 2072 6574  _list})..    ret
-0000fcd0: 7572 6e20 7072 6f66 696c 655f 6c69 7374  urn profile_list
-0000fce0: 0a0a 0a23 2023 2323 2323 2323 2323 2323  ...# ###########
-0000fcf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fd00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fd10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fd20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fd30: 2323 2323 2323 230a 2320 4469 7370 6c61  #######.# Displa
-0000fd40: 7920 7374 6172 7475 7020 6d65 7373 6167  y startup messag
-0000fd50: 6573 2077 6869 6368 2061 7265 2061 2063  es which are a c
-0000fd60: 6172 7279 6f76 6572 2066 726f 6d20 7468  arryover from th
-0000fd70: 6520 6c61 7374 2072 756e 2e0a 2320 2323  e last run..# ##
-0000fd80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fd90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fda0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fdb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fdc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fdd0: 0a64 6566 2064 6973 706c 6179 5f6d 6573  .def display_mes
-0000fde0: 7361 6765 735f 6672 6f6d 5f6c 6173 745f  sages_from_last_
-0000fdf0: 7275 6e28 7365 6c66 2920 2d3e 204e 6f6e  run(self) -> Non
-0000fe00: 653a 2020 2320 6e6f 7161 3a20 414e 4e30  e:  # noqa: ANN0
-0000fe10: 3031 0a20 2020 2022 2222 0a20 2020 2044  01.    """.    D
-0000fe20: 6973 706c 6179 7320 6d65 7373 6167 6573  isplays messages
-0000fe30: 2066 726f 6d20 7468 6520 6c61 7374 2072   from the last r
-0000fe40: 756e 2e0a 0a20 2020 2054 6869 7320 6675  un...    This fu
-0000fe50: 6e63 7469 6f6e 2063 6865 636b 7320 6966  nction checks if
-0000fe60: 2074 6865 7265 2061 7265 2061 6e79 2063   there are any c
-0000fe70: 6172 7279 6f76 6572 2065 7272 6f72 206d  arryover error m
-0000fe80: 6573 7361 6765 7320 6672 6f6d 2074 6865  essages from the
-0000fe90: 206c 6173 7420 7275 6e20 2872 6572 756e   last run (rerun
-0000fea0: 292e 0a20 2020 2049 6620 7468 6572 6520  )..    If there 
-0000feb0: 6172 652c 2069 7420 7265 6164 7320 7468  are, it reads th
-0000fec0: 6520 6572 726f 7220 6d65 7373 6167 6520  e error message 
-0000fed0: 6672 6f6d 2074 6865 2066 696c 6520 7370  from the file sp
-0000fee0: 6563 6966 6965 6420 6279 2074 6865 2060  ecified by the `
-0000fef0: 4552 524f 525f 4649 4c45 6020 636f 6e73  ERROR_FILE` cons
-0000ff00: 7461 6e74 2061 6e64 2068 616e 646c 6573  tant and handles
-0000ff10: 0a20 2020 2070 6f74 656e 7469 616c 206d  .    potential m
-0000ff20: 6973 7369 6e67 206d 6f64 756c 6573 2e20  issing modules. 
-0000ff30: 4966 2074 6865 2065 7272 6f72 206d 6573  If the error mes
-0000ff40: 7361 6765 2063 6f6e 7461 696e 7320 7468  sage contains th
-0000ff50: 6520 7374 7269 6e67 2022 4169 2052 6573  e string "Ai Res
-0000ff60: 706f 6e73 6522 2c20 6974 2064 6973 706c  ponse", it displ
-0000ff70: 6179 7320 7468 650a 2020 2020 6572 726f  ays the.    erro
-0000ff80: 7220 6d65 7373 6167 6520 696e 2061 206e  r message in a n
-0000ff90: 6577 2074 6f70 6c65 7665 6c20 7769 6e64  ew toplevel wind
-0000ffa0: 6f77 2061 6e64 2064 6973 706c 6179 7320  ow and displays 
-0000ffb0: 6120 6d65 7373 6167 6520 626f 7820 696e  a message box in
-0000ffc0: 6469 6361 7469 6e67 2074 6861 7420 7468  dicating that th
-0000ffd0: 6520 616e 616c 7973 6973 2072 6573 706f  e analysis respo
-0000ffe0: 6e73 650a 2020 2020 6973 2069 6e20 6120  nse.    is in a 
-0000fff0: 7365 7061 7261 7465 2077 696e 646f 7720  separate window 
-00010000: 616e 6420 7361 7665 6420 6173 2060 414e  and saved as `AN
-00010010: 414c 5953 4953 5f46 494c 4560 2e20 4966  ALYSIS_FILE`. If
-00010020: 2074 6865 2065 7272 6f72 206d 6573 7361   the error messa
-00010030: 6765 2063 6f6e 7461 696e 7320 6e65 776c  ge contains newl
-00010040: 696e 6520 6368 6172 6163 7465 7273 2c0a  ine characters,.
-00010050: 2020 2020 6974 2062 7265 616b 7320 7468      it breaks th
-00010060: 6520 6d65 7373 6167 6520 7570 2069 6e74  e message up int
-00010070: 6f20 6d75 6c74 6970 6c65 206c 696e 6573  o multiple lines
-00010080: 2061 6e64 2064 6973 706c 6179 7320 6561   and displays ea
-00010090: 6368 206c 696e 6520 696e 2061 206d 6573  ch line in a mes
-000100a0: 7361 6765 2062 6f78 2e20 4966 2074 6865  sage box. If the
-000100b0: 2065 7272 6f72 206d 6573 7361 6765 0a20   error message. 
-000100c0: 2020 2064 6f65 7320 6e6f 7420 636f 6e74     does not cont
-000100d0: 6169 6e20 6e65 776c 696e 6520 6368 6172  ain newline char
-000100e0: 6163 7465 7273 2c20 6974 2064 6973 706c  acters, it displ
-000100f0: 6179 7320 7468 6520 6572 726f 7220 6d65  ays the error me
-00010100: 7373 6167 6520 696e 2061 206d 6573 7361  ssage in a messa
-00010110: 6765 2062 6f78 2e20 4166 7465 7220 6469  ge box. After di
-00010120: 7370 6c61 7969 6e67 2074 6865 0a20 2020  splaying the.   
-00010130: 2065 7272 6f72 206d 6573 7361 6765 2c20   error message, 
-00010140: 6974 2072 656d 6f76 6573 2074 6865 2065  it removes the e
-00010150: 7272 6f72 2066 696c 6520 746f 2070 7265  rror file to pre
-00010160: 7665 6e74 2069 7420 6672 6f6d 2062 6569  vent it from bei
-00010170: 6e67 2064 6973 706c 6179 6564 2061 6761  ng displayed aga
-00010180: 696e 2e0a 0a20 2020 2049 6620 7468 6572  in...    If ther
-00010190: 6520 6973 2061 6e20 6572 726f 7220 6d65  e is an error me
-000101a0: 7373 6167 6520 6672 6f6d 206f 7468 6572  ssage from other
-000101b0: 2072 6f75 7469 6e65 732c 2069 7420 6469   routines, it di
-000101c0: 7370 6c61 7973 2074 6865 2065 7272 6f72  splays the error
-000101d0: 206d 6573 7361 6765 2069 6e20 6120 6d65   message in a me
-000101e0: 7373 6167 6520 626f 7820 7769 7468 2074  ssage box with t
-000101f0: 6865 2072 6574 7572 6e20 636f 6465 2e0a  he return code..
-00010200: 0a20 2020 2050 6172 616d 6574 6572 733a  .    Parameters:
-00010210: 0a20 2020 202d 204e 6f6e 650a 0a20 2020  .    - None..   
-00010220: 2052 6574 7572 6e73 3a0a 2020 2020 2d20   Returns:.    - 
-00010230: 4e6f 6e65 0a20 2020 2022 2222 0a20 2020  None.    """.   
-00010240: 2023 2053 6565 2069 6620 7765 2068 6176   # See if we hav
-00010250: 6520 616e 7920 6361 7272 796f 7665 7220  e any carryover 
-00010260: 6572 726f 7220 6d65 7373 6167 6573 2066  error messages f
-00010270: 726f 6d20 6c61 7374 2072 756e 2028 7265  rom last run (re
-00010280: 7275 6e29 2e0a 2020 2020 6966 206f 732e  run)..    if os.
-00010290: 7061 7468 2e69 7366 696c 6528 4552 524f  path.isfile(ERRO
-000102a0: 525f 4649 4c45 293a 0a20 2020 2020 2020  R_FILE):.       
-000102b0: 2077 6974 6820 6f70 656e 2845 5252 4f52   with open(ERROR
-000102c0: 5f46 494c 4529 2061 7320 6572 726f 725f  _FILE) as error_
-000102d0: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
-000102e0: 2020 6572 726f 725f 6d73 6720 3d20 6572    error_msg = er
-000102f0: 726f 725f 6669 6c65 2e72 6561 6428 290a  ror_file.read().
-00010300: 2020 2020 2020 2020 2020 2020 2320 4861              # Ha
-00010310: 6e64 6c65 2070 6f74 656e 7469 616c 206d  ndle potential m
-00010320: 7373 696e 6720 6d6f 6475 6c65 730a 2020  ssing modules.  
-00010330: 2020 2020 2020 2020 2020 6966 2022 6372            if "cr
-00010340: 6961 2220 696e 2065 7272 6f72 5f6d 7367  ia" in error_msg
-00010350: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010360: 2020 7365 6c66 2e61 695f 6d69 7373 696e    self.ai_missin
-00010370: 675f 6d6f 6475 6c65 203d 2022 6372 6961  g_module = "cria
-00010380: 220a 2020 2020 2020 2020 2020 2020 656c  ".            el
-00010390: 6966 2022 6f70 656e 6169 2220 696e 2065  if "openai" in e
-000103a0: 7272 6f72 5f6d 7367 3a0a 2020 2020 2020  rror_msg:.      
-000103b0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000103c0: 695f 6d69 7373 696e 675f 6d6f 6475 6c65  i_missing_module
-000103d0: 203d 2022 6f70 656e 6169 220a 0a20 2020   = "openai"..   
-000103e0: 2020 2020 2020 2020 2023 2048 616e 646c           # Handl
-000103f0: 6520 4169 2052 6573 706f 6e73 6520 696e  e Ai Response in
-00010400: 206e 6577 2074 6f70 6c65 7665 6c20 7769   new toplevel wi
-00010410: 6e64 6f77 0a20 2020 2020 2020 2020 2020  ndow.           
-00010420: 2069 6620 2241 6920 5265 7370 6f6e 7365   if "Ai Response
-00010430: 2220 696e 2065 7272 6f72 5f6d 7367 3a0a  " in error_msg:.
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 7365 6c66 2e64 6973 706c 6179 5f61 695f  self.display_ai_
-00010460: 7265 7370 6f6e 7365 2865 7272 6f72 5f6d  response(error_m
-00010470: 7367 290a 2020 2020 2020 2020 2020 2020  sg).            
-00010480: 2020 2020 7365 6c66 2e64 6973 706c 6179      self.display
-00010490: 5f6d 6573 7361 6765 5f62 6f78 280a 2020  _message_box(.  
-000104a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104b0: 2020 6622 416e 616c 7973 6973 2072 6573    f"Analysis res
-000104c0: 706f 6e73 6520 6973 2069 6e20 6120 7370  ponse is in a sp
-000104d0: 6561 7261 7465 2057 696e 646f 7720 616e  earate Window an
-000104e0: 6420 7361 7665 6420 6173 207b 414e 414c  d saved as {ANAL
-000104f0: 5953 4953 5f46 494c 457d 2e22 2c0a 2020  YSIS_FILE}.",.  
-00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010510: 2020 2254 7572 7175 6f69 7365 222c 0a20    "Turquoise",. 
-00010520: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00010530: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
-00010540: 6f6d 6520 6f74 6865 7220 6d65 7373 6167  ome other messag
-00010550: 652e 2020 4a75 7374 2064 6973 706c 6179  e.  Just display
-00010560: 2069 7420 696e 2074 6865 206d 6573 7361   it in the messa
-00010570: 6765 2062 6f78 2061 6e64 2062 7265 616b  ge box and break
-00010580: 2069 7420 7570 2069 6620 6e65 6564 6564   it up if needed
-00010590: 2e0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-000105a0: 6966 2022 5c6e 2220 696e 2065 7272 6f72  if "\n" in error
-000105b0: 5f6d 7367 3a0a 2020 2020 2020 2020 2020  _msg:.          
-000105c0: 2020 2020 2020 6d65 7373 6167 6573 203d        messages =
-000105d0: 2065 7272 6f72 5f6d 7367 2e73 706c 6974   error_msg.split
-000105e0: 2822 5c6e 2229 0a20 2020 2020 2020 2020  ("\n").         
-000105f0: 2020 2020 2020 2066 6f72 206d 6573 7361         for messa
-00010600: 6765 5f6c 696e 6520 696e 206d 6573 7361  ge_line in messa
-00010610: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
-00010620: 2020 2020 2020 2020 2073 656c 662e 6469           self.di
-00010630: 7370 6c61 795f 6d65 7373 6167 655f 626f  splay_message_bo
-00010640: 7828 6d65 7373 6167 655f 6c69 6e65 2c20  x(message_line, 
-00010650: 2252 6564 2229 0a20 2020 2020 2020 2020  "Red").         
-00010660: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00010670: 2020 2020 2020 2020 2073 656c 662e 6469           self.di
-00010680: 7370 6c61 795f 6d65 7373 6167 655f 626f  splay_message_bo
-00010690: 7828 6572 726f 725f 6d73 672c 2022 5265  x(error_msg, "Re
-000106a0: 6422 290a 2020 2020 2020 2020 2020 2020  d").            
-000106b0: 6f73 2e72 656d 6f76 6528 4552 524f 525f  os.remove(ERROR_
-000106c0: 4649 4c45 2920 2023 2047 6574 2072 6964  FILE)  # Get rid
-000106d0: 206f 6620 6572 726f 7220 6d65 7373 6167   of error messag
-000106e0: 6520 736f 2077 6520 646f 6e27 7420 6469  e so we don't di
-000106f0: 7370 6c61 7920 6974 2061 6761 696e 2e0a  splay it again..
-00010700: 0a20 2020 2023 2044 6973 706c 6179 2061  .    # Display a
-00010710: 6e79 2065 7272 6f72 206d 6573 7361 6765  ny error message
-00010720: 2066 726f 6d20 6f74 6865 7220 726f 756e   from other roun
-00010730: 7469 6e65 730a 2020 2020 6966 2050 7269  tines.    if Pri
-00010740: 6d65 4974 656d 732e 6572 726f 725f 6d73  meItems.error_ms
-00010750: 673a 0a20 2020 2020 2020 2073 656c 662e  g:.        self.
-00010760: 6469 7370 6c61 795f 6d65 7373 6167 655f  display_message_
-00010770: 626f 7828 6622 7b50 7269 6d65 4974 656d  box(f"{PrimeItem
-00010780: 732e 6572 726f 725f 6d73 677d 2077 6974  s.error_msg} wit
-00010790: 6820 7265 7475 726e 2063 6f64 6520 7b50  h return code {P
-000107a0: 7269 6d65 4974 656d 732e 6572 726f 725f  rimeItems.error_
-000107b0: 636f 6465 7d2e 222c 2022 5265 6422 290a  code}.", "Red").
-000107c0: 0a0a 2320 2323 2323 2323 2323 2323 2323  ..# ############
-000107d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000107e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000107f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010810: 2323 2323 2323 0a23 2044 6973 706c 6179  ######.# Display
-00010820: 2074 6865 2063 7572 7265 6e74 2066 696c   the current fil
-00010830: 6520 6173 2061 206c 6162 656c 0a23 2023  e as a label.# #
-00010840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010880: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010890: 230a 6465 6620 6469 7370 6c61 795f 6375  #.def display_cu
-000108a0: 7272 656e 745f 6669 6c65 2873 656c 662c  rrent_file(self,
-000108b0: 2066 696c 655f 6e61 6d65 3a20 7374 7229   file_name: str)
-000108c0: 202d 3e20 4e6f 6e65 3a20 2023 206e 6f71   -> None:  # noq
-000108d0: 613a 2041 4e4e 3030 310a 2020 2020 2222  a: ANN001.    ""
-000108e0: 220a 2020 2020 4469 7370 6c61 7920 7468  ".    Display th
-000108f0: 6520 6375 7272 656e 7420 6669 6c65 206e  e current file n
-00010900: 616d 6520 696e 2061 2062 7574 746f 6e20  ame in a button 
-00010910: 6f6e 2074 6865 2047 5549 2e0a 0a20 2020  on the GUI...   
-00010920: 2041 7267 733a 0a20 2020 2020 2020 2066   Args:.        f
-00010930: 696c 655f 6e61 6d65 2028 7374 7229 3a20  ile_name (str): 
-00010940: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-00010950: 6375 7272 656e 7420 6669 6c65 2e0a 0a20  current file... 
-00010960: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00010970: 2020 2020 4e6f 6e65 3a20 5468 6973 2066      None: This f
-00010980: 756e 6374 696f 6e20 646f 6573 206e 6f74  unction does not
-00010990: 2072 6574 7572 6e20 616e 7974 6869 6e67   return anything
-000109a0: 2e0a 0a20 2020 2054 6869 7320 6675 6e63  ...    This func
-000109b0: 7469 6f6e 2063 7265 6174 6573 2061 2062  tion creates a b
-000109c0: 7574 746f 6e20 6f6e 2074 6865 2047 5549  utton on the GUI
-000109d0: 2074 6861 7420 6469 7370 6c61 7973 2074   that displays t
-000109e0: 6865 2063 7572 7265 6e74 2066 696c 6520  he current file 
-000109f0: 6e61 6d65 2e20 5468 6520 6275 7474 6f6e  name. The button
-00010a00: 2069 7320 6372 6561 7465 6420 7573 696e   is created usin
-00010a10: 6720 7468 6520 6061 6464 5f62 7574 746f  g the `add_butto
-00010a20: 6e60 2066 756e 6374 696f 6e20 616e 6420  n` function and 
-00010a30: 6973 2070 6c61 6365 6420 696e 2074 6865  is placed in the
-00010a40: 2073 6563 6f6e 6420 726f 7720 616e 6420   second row and 
-00010a50: 7465 6e74 6820 636f 6c75 6d6e 206f 6620  tenth column of 
-00010a60: 7468 6520 4755 492e 2054 6865 2062 7574  the GUI. The but
-00010a70: 746f 6e27 7320 7465 7874 2069 7320 7365  ton's text is se
-00010a80: 7420 746f 2022 4375 7272 656e 7420 4669  t to "Current Fi
-00010a90: 6c65 3a20 7b66 696c 655f 6e61 6d65 7d22  le: {file_name}"
-00010aa0: 2e20 5468 6520 6073 656c 662e 7265 706f  . The `self.repo
-00010ab0: 7274 5f69 7373 7565 5f65 7665 6e74 6020  rt_issue_event` 
-00010ac0: 6675 6e63 7469 6f6e 2069 7320 6173 7369  function is assi
-00010ad0: 676e 6564 2061 7320 7468 6520 6275 7474  gned as the butt
-00010ae0: 6f6e 2773 2063 6c69 636b 2065 7665 6e74  on's click event
-00010af0: 2068 616e 646c 6572 2e0a 0a20 2020 204e   handler...    N
-00010b00: 6f74 653a 0a20 2020 2020 2020 202d 2054  ote:.        - T
-00010b10: 6865 2060 6164 645f 6275 7474 6f6e 6020  he `add_button` 
-00010b20: 6675 6e63 7469 6f6e 2069 7320 6173 7375  function is assu
-00010b30: 6d65 6420 746f 2062 6520 6465 6669 6e65  med to be define
-00010b40: 6420 656c 7365 7768 6572 6520 696e 2074  d elsewhere in t
-00010b50: 6865 2063 6f64 6562 6173 652e 0a20 2020  he codebase..   
-00010b60: 2020 2020 202d 2054 6865 2060 7365 6c66       - The `self
-00010b70: 2e72 6570 6f72 745f 6973 7375 655f 6576  .report_issue_ev
-00010b80: 656e 7460 2066 756e 6374 696f 6e20 6973  ent` function is
-00010b90: 2061 7373 756d 6564 2074 6f20 6265 2064   assumed to be d
-00010ba0: 6566 696e 6564 2065 6c73 6577 6865 7265  efined elsewhere
-00010bb0: 2069 6e20 7468 6520 636f 6465 6261 7365   in the codebase
-00010bc0: 2e0a 0a20 2020 2045 7861 6d70 6c65 3a0a  ...    Example:.
-00010bd0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-00010be0: 6e0a 2020 2020 2020 2020 6775 695f 696e  n.        gui_in
-00010bf0: 7374 616e 6365 2e64 6973 706c 6179 5f63  stance.display_c
-00010c00: 7572 7265 6e74 5f66 696c 6528 2265 7861  urrent_file("exa
-00010c10: 6d70 6c65 2e74 7874 2229 0a20 2020 2020  mple.txt").     
-00010c20: 2020 2060 6060 0a20 2020 2022 2222 0a20     ```.    """. 
-00010c30: 2020 2023 2043 6c65 6172 2070 7265 7669     # Clear previ
-00010c40: 6f75 7320 6966 2066 696c 6c65 642e 0a20  ous if filled.. 
-00010c50: 2020 2077 6974 6820 636f 6e74 6578 746c     with contextl
-00010c60: 6962 2e73 7570 7072 6573 7328 4174 7472  ib.suppress(Attr
-00010c70: 6962 7574 6545 7272 6f72 293a 0a20 2020  ibuteError):.   
-00010c80: 2020 2020 2073 656c 662e 7265 706f 7274       self.report
-00010c90: 5f69 7373 7565 5f62 7574 746f 6e2e 6465  _issue_button.de
-00010ca0: 7374 726f 7928 290a 2020 2020 2320 4368  stroy().    # Ch
-00010cb0: 6563 6b20 666f 7220 736c 6173 6865 7320  eck for slashes 
-00010cc0: 616e 6420 7265 6d6f 7665 2069 6620 6e65  and remove if ne
-00010cd0: 7373 6573 6172 790a 2020 2020 6669 6c65  ssesary.    file
-00010ce0: 6e61 6d65 5f6c 6f63 6174 696f 6e20 3d20  name_location = 
-00010cf0: 6669 6c65 5f6e 616d 652e 7266 696e 6428  file_name.rfind(
-00010d00: 5072 696d 6549 7465 6d73 2e73 6c61 7368  PrimeItems.slash
-00010d10: 2920 2b20 310a 2020 2020 6966 2066 696c  ) + 1.    if fil
-00010d20: 656e 616d 655f 6c6f 6361 7469 6f6e 2021  ename_location !
-00010d30: 3d20 2d31 3a0a 2020 2020 2020 2020 6669  = -1:.        fi
-00010d40: 6c65 5f6e 616d 6520 3d20 6669 6c65 5f6e  le_name = file_n
-00010d50: 616d 655b 6669 6c65 6e61 6d65 5f6c 6f63  ame[filename_loc
-00010d60: 6174 696f 6e3a 5d0a 2020 2020 7365 6c66  ation:].    self
-00010d70: 2e72 6570 6f72 745f 6973 7375 655f 6275  .report_issue_bu
-00010d80: 7474 6f6e 203d 2061 6464 5f6c 6162 656c  tton = add_label
-00010d90: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00010da0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00010db0: 2020 2020 2020 6622 4375 7272 656e 7420        f"Current 
-00010dc0: 4669 6c65 3a20 7b66 696c 655f 6e61 6d65  File: {file_name
-00010dd0: 7d22 2c0a 2020 2020 2020 2020 2222 2c0a  }",.        "",.
-00010de0: 2020 2020 2020 2020 2222 2c0a 2020 2020          "",.    
-00010df0: 2020 2020 226e 6f72 6d61 6c22 2c0a 2020      "normal",.  
-00010e00: 2020 2020 2020 3131 2c0a 2020 2020 2020        11,.      
-00010e10: 2020 312c 0a20 2020 2020 2020 2032 302c    1,.        20,
-00010e20: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
-00010e30: 2020 2020 2277 222c 0a20 2020 2029 0a0a      "w",.    )..
-00010e40: 0a23 2023 2323 2323 2323 2323 2323 2323  .# #############
-00010e50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010e60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010e70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010e80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010e90: 2323 2323 230a 2320 4469 7370 6c61 7920  #####.# Display 
-00010ea0: 6120 7472 6565 2073 7472 7563 7475 7265  a tree structure
-00010eb0: 0a23 2023 2323 2323 2323 2323 2323 2323  .# #############
-00010ec0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010ed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010f00: 2323 2323 230a 636c 6173 7320 4354 6b54  #####.class CTkT
-00010f10: 7265 6576 6965 7728 6374 6b2e 4354 6b46  reeview(ctk.CTkF
-00010f20: 7261 6d65 293a 0a20 2020 2022 2222 436c  rame):.    """Cl
-00010f30: 6173 7320 746f 2068 616e 646c 6520 7468  ass to handle th
-00010f40: 6520 5472 6565 7669 6577 0a0a 2020 2020  e Treeview..    
-00010f50: 4172 6773 3a0a 2020 2020 2020 2020 6374  Args:.        ct
-00010f60: 6b20 2863 746b 293a 204f 7572 2047 5549  k (ctk): Our GUI
-00010f70: 2066 7261 6d65 776f 726b 0a20 2020 2022   framework.    "
-00010f80: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
-00010f90: 6974 5f5f 2873 656c 662c 206d 6173 7465  it__(self, maste
-00010fa0: 723a 2061 6e79 2c20 6974 656d 733a 206c  r: any, items: l
-00010fb0: 6973 7429 202d 3e20 4e6f 6e65 3a0a 2020  ist) -> None:.  
-00010fc0: 2020 2020 2020 2222 2246 756e 6374 696f        """Functio
-00010fd0: 6e3a 0a20 2020 2020 2020 2064 6566 205f  n:.        def _
-00010fe0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6d61  _init__(self, ma
-00010ff0: 7374 6572 3a20 616e 792c 2069 7465 6d73  ster: any, items
-00011000: 3a20 6c69 7374 293a 0a20 2020 2020 2020  : list):.       
-00011010: 2020 2020 2049 6e69 7469 616c 697a 6573       Initializes
-00011020: 2061 2054 7265 6576 6965 7720 7769 6467   a Treeview widg
-00011030: 6574 2077 6974 6820 6120 6769 7665 6e20  et with a given 
-00011040: 6d61 7374 6572 2061 6e64 206c 6973 7420  master and list 
-00011050: 6f66 2069 7465 6d73 2e0a 2020 2020 2020  of items..      
-00011060: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00011070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011080: 2020 6d61 7374 6572 2028 616e 7929 3a20    master (any): 
-00011090: 5468 6520 7061 7265 6e74 2077 6964 6765  The parent widge
-000110a0: 7420 666f 7220 7468 6520 5472 6565 7669  t for the Treevi
-000110b0: 6577 2e0a 2020 2020 2020 2020 2020 2020  ew..            
-000110c0: 2020 2020 6974 656d 7320 286c 6973 7429      items (list)
-000110d0: 3a20 4120 6c69 7374 206f 6620 6974 656d  : A list of item
-000110e0: 7320 746f 2062 6520 696e 7365 7274 6564  s to be inserted
-000110f0: 2069 6e74 6f20 7468 6520 5472 6565 7669   into the Treevi
-00011100: 6577 2e0a 2020 2020 2020 2020 2020 2020  ew..            
-00011110: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00011120: 2020 2020 2020 2020 204e 6f6e 652e 0a20           None.. 
-00011130: 2020 2020 2020 2020 2020 2050 726f 6365             Proce
-00011140: 7373 696e 6720 4c6f 6769 633a 0a20 2020  ssing Logic:.   
-00011150: 2020 2020 2020 2020 2020 2020 202d 2053               - S
-00011160: 6574 7320 7570 2074 6865 2054 7265 6576  ets up the Treev
-00011170: 6965 7720 7769 6467 6574 2077 6974 6820  iew widget with 
-00011180: 6170 7072 6f70 7269 6174 6520 7374 796c  appropriate styl
-00011190: 6573 2061 6e64 2062 696e 6469 6e67 732e  es and bindings.
-000111a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000111b0: 202d 2049 6e73 6572 7473 2074 6865 2067   - Inserts the g
-000111c0: 6976 656e 2069 7465 6d73 2069 6e74 6f20  iven items into 
-000111d0: 7468 6520 5472 6565 7669 6577 2e0a 0a20  the Treeview... 
-000111e0: 2020 2020 2020 2074 6b69 6e74 6572 2074         tkinter t
-000111f0: 7265 6576 6965 7720 636f 6e66 6967 7572  reeview configur
-00011200: 6162 6c65 2069 7465 6d73 3a0a 2020 2020  able items:.    
-00011210: 2020 2020 2020 2020 7474 6b3a 3a73 7479          ttk::sty
-00011220: 6c65 2063 6f6e 6669 6775 7265 2054 7265  le configure Tre
-00011230: 6576 6965 7720 2d62 6163 6b67 726f 756e  eview -backgroun
-00011240: 6420 636f 6c6f 720a 2020 2020 2020 2020  d color.        
-00011250: 2020 2020 7474 6b3a 3a73 7479 6c65 2063      ttk::style c
-00011260: 6f6e 6669 6775 7265 2054 7265 6576 6965  onfigure Treevie
-00011270: 7720 2d66 6f72 6567 726f 756e 6420 636f  w -foreground co
-00011280: 6c6f 720a 2020 2020 2020 2020 2020 2020  lor.            
-00011290: 7474 6b3a 3a73 7479 6c65 2063 6f6e 6669  ttk::style confi
-000112a0: 6775 7265 2054 7265 6576 6965 7720 2d66  gure Treeview -f
-000112b0: 6f6e 7420 6e61 6d65 6466 6f6e 740a 2020  ont namedfont.  
-000112c0: 2020 2020 2020 2020 2020 7474 6b3a 3a73            ttk::s
-000112d0: 7479 6c65 2063 6f6e 6669 6775 7265 2054  tyle configure T
-000112e0: 7265 6576 6965 7720 2d66 6965 6c64 6261  reeview -fieldba
-000112f0: 636b 6772 6f75 6e64 2063 6f6c 6f72 0a20  ckground color. 
-00011300: 2020 2020 2020 2020 2020 2074 746b 3a3a             ttk::
-00011310: 7374 796c 6520 6d61 7020 5472 6565 7669  style map Treevi
-00011320: 6577 202d 6261 636b 6772 6f75 6e64 205c  ew -background \
-00011330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011340: 205b 6c69 7374 2073 656c 6563 7465 6420   [list selected 
-00011350: 636f 6c6f 725d 0a20 2020 2020 2020 2020  color].         
-00011360: 2020 2074 746b 3a3a 7374 796c 6520 6d61     ttk::style ma
-00011370: 7020 5472 6565 7669 6577 202d 666f 7265  p Treeview -fore
-00011380: 6772 6f75 6e64 205c 0a20 2020 2020 2020  ground \.       
-00011390: 2020 2020 2020 2020 205b 6c69 7374 2073           [list s
-000113a0: 656c 6563 7465 6420 636f 6c6f 725d 0a20  elected color]. 
-000113b0: 2020 2020 2020 2020 2020 2074 746b 3a3a             ttk::
-000113c0: 7374 796c 6520 636f 6e66 6967 7572 6520  style configure 
-000113d0: 5472 6565 7669 6577 202d 726f 7768 6569  Treeview -rowhei
-000113e0: 6768 7420 5b65 7870 7220 7b5b 666f 6e74  ght [expr {[font
-000113f0: 206d 6574 7269 6373 206e 616d 6564 666f   metrics namedfo
-00011400: 6e74 202d 6c69 6e65 7370 6163 655d 202b  nt -linespace] +
-00011410: 2032 7d5d 0a20 2020 2020 2020 2020 2020   2}].           
-00011420: 2074 746b 3a3a 7374 796c 6520 636f 6e66   ttk::style conf
-00011430: 6967 7572 6520 4865 6164 696e 6720 2d66  igure Heading -f
-00011440: 6f6e 7420 6e61 6d65 6466 6f6e 740a 2020  ont namedfont.  
-00011450: 2020 2020 2020 2020 2020 7474 6b3a 3a73            ttk::s
-00011460: 7479 6c65 2063 6f6e 6669 6775 7265 2048  tyle configure H
-00011470: 6561 6469 6e67 202d 6261 636b 6772 6f75  eading -backgrou
-00011480: 6e64 2063 6f6c 6f72 0a20 2020 2020 2020  nd color.       
-00011490: 2020 2020 2074 746b 3a3a 7374 796c 6520       ttk::style 
-000114a0: 636f 6e66 6967 7572 6520 4865 6164 696e  configure Headin
-000114b0: 6720 2d66 6f72 6567 726f 756e 6420 636f  g -foreground co
-000114c0: 6c6f 720a 2020 2020 2020 2020 2020 2020  lor.            
-000114d0: 7474 6b3a 3a73 7479 6c65 2063 6f6e 6669  ttk::style confi
-000114e0: 6775 7265 2048 6561 6469 6e67 202d 7061  gure Heading -pa
-000114f0: 6464 696e 6720 7061 6464 696e 670a 2020  dding padding.  
-00011500: 2020 2020 2020 2020 2020 7474 6b3a 3a73            ttk::s
-00011510: 7479 6c65 2063 6f6e 6669 6775 7265 2049  tyle configure I
-00011520: 7465 6d20 2d66 6f72 6567 726f 756e 6420  tem -foreground 
-00011530: 636f 6c6f 720a 2020 2020 2020 2020 2020  color.          
-00011540: 2020 7474 6b3a 3a73 7479 6c65 2063 6f6e    ttk::style con
-00011550: 6669 6775 7265 2049 7465 6d20 2d66 6f63  figure Item -foc
-00011560: 7573 636f 6c6f 7220 636f 6c6f 720a 2020  uscolor color.  
-00011570: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011580: 2020 7365 6c66 2e72 6f6f 7420 3d20 6d61    self.root = ma
-00011590: 7374 6572 0a20 2020 2020 2020 2073 656c  ster.        sel
-000115a0: 662e 6974 656d 7320 3d20 6974 656d 730a  f.items = items.
-000115b0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-000115c0: 5f5f 696e 6974 5f5f 2873 656c 662e 726f  __init__(self.ro
-000115d0: 6f74 290a 0a20 2020 2020 2020 2073 656c  ot)..        sel
-000115e0: 662e 6772 6964 5f63 6f6c 756d 6e63 6f6e  f.grid_columncon
-000115f0: 6669 6775 7265 2830 2c20 7765 6967 6874  figure(0, weight
-00011600: 3d31 290a 0a20 2020 2020 2020 2023 204c  =1)..        # L
-00011610: 6162 656c 2077 6964 6765 740a 2020 2020  abel widget.    
-00011620: 2020 2020 6f75 725f 6c61 6265 6c20 3d20      our_label = 
-00011630: 2222 220a 4472 6167 2074 6865 2062 6f74  """.Drag the bot
-00011640: 746f 6d20 6f66 2074 6865 2077 696e 646f  tom of the windo
-00011650: 7720 746f 2065 7870 616e 6420 6173 206e  w to expand as n
-00011660: 6565 6465 642e 5c6e 0a43 6c69 636b 2069  eeded.\n.Click i
-00011670: 7465 6d20 616e 6420 7363 726f 6c6c 206d  tem and scroll m
-00011680: 6f75 7365 2d77 6865 656c 2f74 7261 636b  ouse-wheel/track
-00011690: 7061 645c 6e61 7320 6e65 6564 6564 2074  pad\nas needed t
-000116a0: 6f20 676f 2075 7020 6f72 2064 6f77 6e2e  o go up or down.
-000116b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000116c0: 2020 2020 2073 656c 662e 6c61 6265 6c20       self.label 
-000116d0: 3d20 6374 6b2e 4354 6b4c 6162 656c 286d  = ctk.CTkLabel(m
-000116e0: 6173 7465 723d 7365 6c66 2c20 7465 7874  aster=self, text
-000116f0: 3d6f 7572 5f6c 6162 656c 2c20 666f 6e74  =our_label, font
-00011700: 3d28 2222 2c20 3132 2929 0a20 2020 2020  =("", 12)).     
-00011710: 2020 2073 656c 662e 6c61 6265 6c2e 6772     self.label.gr
-00011720: 6964 2872 6f77 3d30 2c20 636f 6c75 6d6e  id(row=0, column
-00011730: 3d30 2c20 7061 6478 3d31 302c 2070 6164  =0, padx=10, pad
-00011740: 793d 3130 2c20 7374 6963 6b79 3d22 6577  y=10, sticky="ew
-00011750: 2229 0a0a 2020 2020 2020 2020 2320 4261  ")..        # Ba
-00011760: 7369 6320 6170 7065 6172 616e 6365 2066  sic appearance f
-00011770: 6f72 2074 6578 742c 2066 6f72 6567 726f  or text, foregro
-00011780: 756e 6420 616e 6420 6261 636b 6772 6f75  und and backgrou
-00011790: 6e64 2e0a 2020 2020 2020 2020 7365 6c66  nd..        self
-000117a0: 2e62 675f 636f 6c6f 7220 3d20 7365 6c66  .bg_color = self
-000117b0: 2e72 6f6f 742e 5f61 7070 6c79 5f61 7070  .root._apply_app
-000117c0: 6561 7261 6e63 655f 6d6f 6465 2863 746b  earance_mode(ctk
-000117d0: 2e54 6865 6d65 4d61 6e61 6765 722e 7468  .ThemeManager.th
-000117e0: 656d 655b 2243 546b 4672 616d 6522 5d5b  eme["CTkFrame"][
-000117f0: 2266 675f 636f 6c6f 7222 5d29 2020 2320  "fg_color"])  # 
-00011800: 6e6f 7161 3a20 534c 4630 3031 0a20 2020  noqa: SLF001.   
-00011810: 2020 2020 2073 656c 662e 7465 7874 5f63       self.text_c
-00011820: 6f6c 6f72 203d 2073 656c 662e 726f 6f74  olor = self.root
-00011830: 2e5f 6170 706c 795f 6170 7065 6172 616e  ._apply_appearan
-00011840: 6365 5f6d 6f64 6528 2020 2320 6e6f 7161  ce_mode(  # noqa
-00011850: 3a20 534c 4630 3031 0a20 2020 2020 2020  : SLF001.       
-00011860: 2020 2020 2063 746b 2e54 6865 6d65 4d61       ctk.ThemeMa
-00011870: 6e61 6765 722e 7468 656d 655b 2243 546b  nager.theme["CTk
-00011880: 4c61 6265 6c22 5d5b 2274 6578 745f 636f  Label"]["text_co
-00011890: 6c6f 7222 5d2c 0a20 2020 2020 2020 2029  lor"],.        )
-000118a0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-000118b0: 6c65 6374 6564 5f63 6f6c 6f72 203d 2073  lected_color = s
-000118c0: 656c 662e 726f 6f74 2e5f 6170 706c 795f  elf.root._apply_
-000118d0: 6170 7065 6172 616e 6365 5f6d 6f64 6528  appearance_mode(
-000118e0: 2020 2320 6e6f 7161 3a20 534c 4630 3031    # noqa: SLF001
-000118f0: 0a20 2020 2020 2020 2020 2020 2063 746b  .            ctk
-00011900: 2e54 6865 6d65 4d61 6e61 6765 722e 7468  .ThemeManager.th
-00011910: 656d 655b 2243 546b 4275 7474 6f6e 225d  eme["CTkButton"]
-00011920: 5b22 6667 5f63 6f6c 6f72 225d 2c0a 2020  ["fg_color"],.  
-00011930: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00011940: 2023 2053 6574 2075 7020 7468 6520 7374   # Set up the st
-00011950: 796c 652f 7468 656d 650a 2020 2020 2020  yle/theme.      
-00011960: 2020 7365 6c66 2e74 7265 655f 7374 796c    self.tree_styl
-00011970: 6520 3d20 7474 6b2e 5374 796c 6528 7365  e = ttk.Style(se
-00011980: 6c66 290a 2020 2020 2020 2020 7365 6c66  lf).        self
-00011990: 2e74 7265 655f 7374 796c 652e 7468 656d  .tree_style.them
-000119a0: 655f 7573 6528 2264 6566 6175 6c74 2229  e_use("default")
-000119b0: 0a0a 2020 2020 2020 2020 2320 4774 6574  ..        # Gtet
-000119c0: 6820 7468 6520 6963 6f6e 7320 746f 2062  h the icons to b
-000119d0: 6520 7573 6564 2069 6e20 7468 6520 5472  e used in the Tr
-000119e0: 6565 2076 6965 772e 0a20 2020 2020 2020  ee view..       
-000119f0: 2073 656c 662e 696d 5f6f 7065 6e20 3d20   self.im_open = 
-00011a00: 496d 6167 652e 6f70 656e 2849 434f 4e5f  Image.open(ICON_
-00011a10: 5041 5448 5b22 6172 726f 7722 5d29 0a20  PATH["arrow"]). 
-00011a20: 2020 2020 2020 2073 656c 662e 696d 5f63         self.im_c
-00011a30: 6c6f 7365 203d 2073 656c 662e 696d 5f6f  lose = self.im_o
-00011a40: 7065 6e2e 726f 7461 7465 2839 3029 0a20  pen.rotate(90). 
-00011a50: 2020 2020 2020 2073 656c 662e 696d 5f65         self.im_e
-00011a60: 6d70 7479 203d 2049 6d61 6765 2e6e 6577  mpty = Image.new
-00011a70: 2822 5247 4241 222c 2028 3135 2c20 3135  ("RGBA", (15, 15
-00011a80: 292c 2022 2330 3030 3030 3030 3022 290a  ), "#00000000").
-00011a90: 0a20 2020 2020 2020 2073 656c 662e 696d  .        self.im
-00011aa0: 675f 6f70 656e 203d 2049 6d61 6765 546b  g_open = ImageTk
-00011ab0: 2e50 686f 746f 496d 6167 6528 7365 6c66  .PhotoImage(self
-00011ac0: 2e69 6d5f 6f70 656e 2c20 6e61 6d65 3d22  .im_open, name="
-00011ad0: 696d 675f 6f70 656e 222c 2073 697a 653d  img_open", size=
-00011ae0: 2831 352c 2031 3529 290a 2020 2020 2020  (15, 15)).      
-00011af0: 2020 7365 6c66 2e69 6d67 5f63 6c6f 7365    self.img_close
-00011b00: 203d 2049 6d61 6765 546b 2e50 686f 746f   = ImageTk.Photo
-00011b10: 496d 6167 6528 7365 6c66 2e69 6d5f 636c  Image(self.im_cl
-00011b20: 6f73 652c 206e 616d 653d 2269 6d67 5f63  ose, name="img_c
-00011b30: 6c6f 7365 222c 2073 697a 653d 2831 352c  lose", size=(15,
-00011b40: 2031 3529 290a 2020 2020 2020 2020 7365   15)).        se
-00011b50: 6c66 2e69 6d67 5f65 6d70 7479 203d 2049  lf.img_empty = I
-00011b60: 6d61 6765 546b 2e50 686f 746f 496d 6167  mageTk.PhotoImag
-00011b70: 6528 7365 6c66 2e69 6d5f 656d 7074 792c  e(self.im_empty,
-00011b80: 206e 616d 653d 2269 6d67 5f65 6d70 7479   name="img_empty
-00011b90: 222c 2073 697a 653d 2831 352c 2031 3529  ", size=(15, 15)
-00011ba0: 290a 0a20 2020 2020 2020 2023 2041 7272  )..        # Arr
-00011bb0: 6f77 2065 6c65 6d65 6e74 2063 6f6e 6669  ow element confi
-00011bc0: 6775 7261 7469 6f6e 0a20 2020 2020 2020  guration.       
-00011bd0: 2077 6974 6820 636f 6e74 6578 746c 6962   with contextlib
-00011be0: 2e73 7570 7072 6573 7328 5463 6c45 7272  .suppress(TclErr
-00011bf0: 6f72 293a 2020 2320 446f 6e27 7420 7468  or):  # Don't th
-00011c00: 726f 7720 6572 726f 7220 6966 2074 6865  row error if the
-00011c10: 2065 6c65 6d65 6e74 2061 6c72 6561 6479   element already
-00011c20: 2065 7869 7374 732e 2020 4a75 7374 2072   exists.  Just r
-00011c30: 6575 7365 2069 742e 0a20 2020 2020 2020  euse it..       
-00011c40: 2020 2020 2073 656c 662e 7472 6565 5f73       self.tree_s
-00011c50: 7479 6c65 2e65 6c65 6d65 6e74 5f63 7265  tyle.element_cre
-00011c60: 6174 6528 0a20 2020 2020 2020 2020 2020  ate(.           
-00011c70: 2020 2020 2022 5472 6565 6974 656d 2e6d       "Treeitem.m
-00011c80: 7969 6e64 6963 6174 6f72 222c 0a20 2020  yindicator",.   
-00011c90: 2020 2020 2020 2020 2020 2020 2022 696d               "im
-00011ca0: 6167 6522 2c0a 2020 2020 2020 2020 2020  age",.          
-00011cb0: 2020 2020 2020 2269 6d67 5f63 6c6f 7365        "img_close
-00011cc0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00011cd0: 2020 2028 2275 7365 7231 222c 2022 2175     ("user1", "!u
-00011ce0: 7365 7232 222c 2022 696d 675f 6f70 656e  ser2", "img_open
-00011cf0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00011d00: 2020 2020 2822 7573 6572 3222 2c20 2269      ("user2", "i
-00011d10: 6d67 5f65 6d70 7479 2229 2c0a 2020 2020  mg_empty"),.    
-00011d20: 2020 2020 2020 2020 2020 2020 7374 6963              stic
-00011d30: 6b79 3d22 7722 2c0a 2020 2020 2020 2020  ky="w",.        
-00011d40: 2020 2020 2020 2020 7769 6474 683d 3135          width=15
-00011d50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011d60: 2020 6865 6967 6874 3d31 352c 0a20 2020    height=15,.   
-00011d70: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00011d80: 2020 2020 2320 5472 6565 7669 6577 2063      # Treeview c
-00011d90: 6f6e 6669 6775 7261 7469 6f6e 206f 6620  onfiguration of 
-00011da0: 7468 6520 7472 6565 7669 6577 0a20 2020  the treeview.   
-00011db0: 2020 2020 2073 656c 662e 7472 6565 5f73       self.tree_s
-00011dc0: 7479 6c65 2e6c 6179 6f75 7428 0a20 2020  tyle.layout(.   
-00011dd0: 2020 2020 2020 2020 2022 5472 6565 7669           "Treevi
-00011de0: 6577 2e49 7465 6d22 2c0a 2020 2020 2020  ew.Item",.      
-00011df0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00011e00: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
-00011e10: 2020 2020 2020 2020 2020 2020 2020 2254                "T
-00011e20: 7265 6569 7465 6d2e 7061 6464 696e 6722  reeitem.padding"
-00011e30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011e40: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e60: 2273 7469 636b 7922 3a20 226e 7365 7722  "sticky": "nsew"
-00011e70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011e80: 2020 2020 2020 2020 2020 2263 6869 6c64            "child
-00011e90: 7265 6e22 3a20 5b0a 2020 2020 2020 2020  ren": [.        
-00011ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011eb0: 2020 2020 2822 5472 6565 6974 656d 2e6d      ("Treeitem.m
-00011ec0: 7969 6e64 6963 6174 6f72 222c 207b 2273  yindicator", {"s
-00011ed0: 6964 6522 3a20 226c 6566 7422 2c20 2273  ide": "left", "s
-00011ee0: 7469 636b 7922 3a20 226e 7365 7722 7d29  ticky": "nsew"})
-00011ef0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011f00: 2020 2020 2020 2020 2020 2020 2020 2822                ("
-00011f10: 5472 6565 6974 656d 2e69 6d61 6765 222c  Treeitem.image",
-00011f20: 207b 2273 6964 6522 3a20 226c 6566 7422   {"side": "left"
-00011f30: 2c20 2273 7469 636b 7922 3a20 226e 7365  , "sticky": "nse
-00011f40: 7722 7d29 2c0a 2020 2020 2020 2020 2020  w"}),.          
-00011f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f60: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f80: 2020 2020 2254 7265 6569 7465 6d2e 666f      "Treeitem.fo
-00011f90: 6375 7322 2c0a 2020 2020 2020 2020 2020  cus",.          
-00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fb0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00011fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fd0: 2020 2020 2020 2020 2020 2020 2273 6964              "sid
-00011fe0: 6522 3a20 226c 6566 7422 2c0a 2020 2020  e": "left",.    
-00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012010: 2273 7469 636b 7922 3a20 226e 7365 7722  "sticky": "nsew"
-00012020: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012040: 2020 2020 2020 2263 6869 6c64 7265 6e22        "children"
-00012050: 3a20 5b28 2254 7265 6569 7465 6d2e 7465  : [("Treeitem.te
-00012060: 7874 222c 207b 2273 6964 6522 3a20 226c  xt", {"side": "l
-00012070: 6566 7422 2c20 2273 7469 636b 7922 3a20  eft", "sticky": 
-00012080: 226e 7365 7722 7d29 5d2c 0a20 2020 2020  "nsew"})],.     
-00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120a0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-000120b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120c0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-000120d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120e0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-000120f0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00012100: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00012110: 2c0a 2020 2020 2020 2020 2020 2020 5d2c  ,.            ],
-00012120: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00012130: 2020 2020 7365 6c66 2e74 7265 655f 7374      self.tree_st
-00012140: 796c 652e 636f 6e66 6967 7572 6528 0a20  yle.configure(. 
-00012150: 2020 2020 2020 2020 2020 2022 5472 6565             "Tree
-00012160: 7669 6577 222c 0a20 2020 2020 2020 2020  view",.         
-00012170: 2020 2062 6163 6b67 726f 756e 643d 7365     background=se
-00012180: 6c66 2e62 675f 636f 6c6f 722c 0a20 2020  lf.bg_color,.   
-00012190: 2020 2020 2020 2020 2066 6f72 6567 726f           foregro
-000121a0: 756e 643d 7365 6c66 2e74 6578 745f 636f  und=self.text_co
-000121b0: 6c6f 722c 0a20 2020 2020 2020 2020 2020  lor,.           
-000121c0: 2066 6965 6c64 6261 636b 6772 6f75 6e64   fieldbackground
-000121d0: 3d73 656c 662e 6267 5f63 6f6c 6f72 2c0a  =self.bg_color,.
-000121e0: 2020 2020 2020 2020 2020 2020 626f 7264              bord
-000121f0: 6572 7769 6474 683d 3130 2c20 2023 2044  erwidth=10,  # D
-00012200: 6566 696e 6520 6120 626f 7264 6572 2061  efine a border a
-00012210: 726f 756e 6420 7472 6565 206f 6620 3130  round tree of 10
-00012220: 2070 6978 656c 732e 0a20 2020 2020 2020   pixels..       
-00012230: 2020 2020 2066 6f6e 743d 2822 222c 2031       font=("", 1
-00012240: 3229 2c0a 2020 2020 2020 2020 290a 0a20  2),.        ).. 
-00012250: 2020 2020 2020 2073 656c 662e 7472 6565         self.tree
-00012260: 5f73 7479 6c65 2e6d 6170 280a 2020 2020  _style.map(.    
-00012270: 2020 2020 2020 2020 2254 7265 6576 6965          "Treevie
-00012280: 7722 2c0a 2020 2020 2020 2020 2020 2020  w",.            
-00012290: 6261 636b 6772 6f75 6e64 3d5b 2822 7365  background=[("se
-000122a0: 6c65 6374 6564 222c 2073 656c 662e 6267  lected", self.bg
-000122b0: 5f63 6f6c 6f72 295d 2c0a 2020 2020 2020  _color)],.      
-000122c0: 2020 2020 2020 666f 7265 6772 6f75 6e64        foreground
-000122d0: 3d5b 2822 7365 6c65 6374 6564 222c 2073  =[("selected", s
-000122e0: 656c 662e 7365 6c65 6374 6564 5f63 6f6c  elf.selected_col
-000122f0: 6f72 295d 2c0a 2020 2020 2020 2020 290a  or)],.        ).
-00012300: 2020 2020 2020 2020 7365 6c66 2e72 6f6f          self.roo
-00012310: 742e 6269 6e64 2822 3c3c 5472 6565 7669  t.bind("<<Treevi
-00012320: 6577 5365 6c65 6374 3e3e 222c 206c 616d  ewSelect>>", lam
-00012330: 6264 6120 6576 656e 743a 2073 656c 662e  bda event: self.
-00012340: 726f 6f74 2e66 6f63 7573 5f73 6574 2829  root.focus_set()
-00012350: 2920 2023 206e 6f71 613a 2041 5247 3030  )  # noqa: ARG00
-00012360: 350a 0a20 2020 2020 2020 2023 2044 6566  5..        # Def
-00012370: 696e 6520 7468 6520 6672 616d 6520 666f  ine the frame fo
-00012380: 7220 7468 6520 7472 6565 7669 6577 0a20  r the treeview. 
-00012390: 2020 2020 2020 2073 656c 662e 7472 6565         self.tree
-000123a0: 7669 6577 203d 2074 746b 2e54 7265 6576  view = ttk.Treev
-000123b0: 6965 7728 7365 6c66 2c20 7368 6f77 3d22  iew(self, show="
-000123c0: 7472 6565 222c 2068 6569 6768 743d 3530  tree", height=50
-000123d0: 2c20 7365 6c65 6374 6d6f 6465 3d22 6272  , selectmode="br
-000123e0: 6f77 7365 2229 0a0a 2020 2020 2020 2020  owse")..        
-000123f0: 2320 4465 6669 6e65 2074 6865 2077 6964  # Define the wid
-00012400: 7468 206f 6620 7468 6520 636f 6c75 6d6e  th of the column
-00012410: 2069 6e74 6f20 7768 6963 6820 7468 6520   into which the 
-00012420: 7472 6565 2077 696c 6c20 6265 2070 6c61  tree will be pla
-00012430: 6365 642e 0a20 2020 2020 2020 2073 656c  ced..        sel
-00012440: 662e 7472 6565 7669 6577 5b22 636f 6c75  f.treeview["colu
-00012450: 6d6e 7322 5d20 3d20 5b30 5d0a 2020 2020  mns"] = [0].    
-00012460: 2020 2020 2320 7365 6c66 2e74 7265 6576      # self.treev
-00012470: 6965 772e 636f 6c75 6d6e 2830 2c20 7374  iew.column(0, st
-00012480: 7265 7463 683d 302c 2061 6e63 686f 723d  retch=0, anchor=
-00012490: 2277 222c 2077 6964 7468 3d31 3530 2c20  "w", width=150, 
-000124a0: 6d69 6e77 6964 7468 3d31 3530 290a 2020  minwidth=150).  
-000124b0: 2020 2020 2020 2320 546f 2063 6f6e 6669        # To confi
-000124c0: 6775 7265 2074 6865 2074 7265 6520 636f  gure the tree co
-000124d0: 6c75 6d6e 2c20 6361 6c6c 2074 6869 7320  lumn, call this 
-000124e0: 7769 7468 2063 6f6c 756d 6e20 3d20 e280  with column = ..
-000124f0: 9c23 30e2 809d 0a20 2020 2020 2020 2073  .#0....        s
-00012500: 656c 662e 7472 6565 7669 6577 2e63 6f6c  elf.treeview.col
-00012510: 756d 6e28 2223 3022 2c20 7374 7265 7463  umn("#0", stretc
-00012520: 683d 302c 2061 6e63 686f 723d 2277 222c  h=0, anchor="w",
-00012530: 2077 6964 7468 3d33 3030 2c20 6d69 6e77   width=300, minw
-00012540: 6964 7468 3d32 3030 290a 0a20 2020 2020  idth=200)..     
-00012550: 2020 2073 656c 662e 7472 6565 7669 6577     self.treeview
-00012560: 2e67 7269 6428 726f 773d 312c 2063 6f6c  .grid(row=1, col
-00012570: 756d 6e3d 302c 2070 6164 783d 3130 2c20  umn=0, padx=10, 
-00012580: 7061 6479 3d31 302c 2073 7469 636b 793d  pady=10, sticky=
-00012590: 2277 2229 0a0a 2020 2020 2020 2020 2320  "w")..        # 
-000125a0: 4164 6420 6974 656d 7320 746f 2074 6865  Add items to the
-000125b0: 2074 7265 650a 2020 2020 2020 2020 7365   tree.        se
-000125c0: 6c66 2e69 6e73 6572 745f 6974 656d 7328  lf.insert_items(
-000125d0: 7365 6c66 2e69 7465 6d73 290a 0a20 2020  self.items)..   
-000125e0: 2023 2023 2323 2323 2323 2323 2323 2323   # #############
-000125f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012600: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012630: 2323 2323 230a 2020 2020 2320 496e 7365  #####.    # Inse
-00012640: 7420 6974 656d 7320 696e 746f 2074 6865  t items into the
-00012650: 2074 7265 6576 6965 772e 0a20 2020 2023   treeview..    #
-00012660: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00012670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012680: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000126a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000126b0: 2323 230a 2020 2020 6465 6620 696e 7365  ###.    def inse
-000126c0: 7274 5f69 7465 6d73 2873 656c 662c 2069  rt_items(self, i
-000126d0: 7465 6d73 3a20 6c69 7374 2c20 7061 7265  tems: list, pare
-000126e0: 6e74 3d22 2229 202d 3e20 4e6f 6e65 3a20  nt="") -> None: 
-000126f0: 2023 206e 6f71 613a 2041 4e4e 3030 310a   # noqa: ANN001.
-00012700: 2020 2020 2020 2020 2222 2249 6e73 6572          """Inser
-00012710: 7473 2069 7465 6d73 2069 6e74 6f20 6120  ts items into a 
-00012720: 7472 6565 7669 6577 2e0a 2020 2020 2020  treeview..      
-00012730: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
-00012740: 2020 2020 2020 2020 2020 6974 656d 7320            items 
-00012750: 286c 6973 7429 3a20 4c69 7374 206f 6620  (list): List of 
-00012760: 6974 656d 7320 746f 2062 6520 696e 7365  items to be inse
-00012770: 7274 6564 2e0a 2020 2020 2020 2020 2020  rted..          
-00012780: 2020 7061 7265 6e74 2028 7374 7229 3a20    parent (str): 
-00012790: 4f70 7469 6f6e 616c 2070 6172 656e 7420  Optional parent 
-000127a0: 6974 656d 2066 6f72 2074 6865 2069 6e73  item for the ins
-000127b0: 6572 7465 6420 6974 656d 732e 0a20 2020  erted items..   
-000127c0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-000127d0: 2020 2020 2020 2020 2020 4e6f 6e65 3a20            None: 
-000127e0: 446f 6573 206e 6f74 2072 6574 7572 6e20  Does not return 
-000127f0: 616e 7974 6869 6e67 2e0a 2020 2020 2020  anything..      
-00012800: 2020 5072 6f63 6573 7369 6e67 204c 6f67    Processing Log
-00012810: 6963 3a0a 2020 2020 2020 2020 2020 2020  ic:.            
-00012820: 2d20 496e 7365 7274 7320 6974 656d 7320  - Inserts items 
-00012830: 696e 746f 2074 7265 6576 6965 772e 0a20  into treeview.. 
-00012840: 2020 2020 2020 2020 2020 202d 2049 6620             - If 
-00012850: 6974 656d 2069 7320 6120 6469 6374 696f  item is a dictio
-00012860: 6e61 7279 2c20 696e 7365 7274 2077 6974  nary, insert wit
-00012870: 6820 6964 2e0a 2020 2020 2020 2020 2020  h id..          
-00012880: 2020 2d20 4966 2069 7465 6d20 6973 206e    - If item is n
-00012890: 6f74 2061 2064 6963 7469 6f6e 6172 792c  ot a dictionary,
-000128a0: 2069 6e73 6572 7420 7769 7468 6f75 7420   insert without 
-000128b0: 6964 2e22 2222 0a20 2020 2020 2020 2066  id.""".        f
-000128c0: 6f72 2069 7465 6d20 696e 2069 7465 6d73  or item in items
-000128d0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000128e0: 2069 7369 6e73 7461 6e63 6528 6974 656d   isinstance(item
-000128f0: 2c20 6469 6374 293a 0a20 2020 2020 2020  , dict):.       
-00012900: 2020 2020 2020 2020 2074 6865 5f69 6420           the_id 
-00012910: 3d20 7365 6c66 2e74 7265 6576 6965 772e  = self.treeview.
-00012920: 696e 7365 7274 2870 6172 656e 742c 2022  insert(parent, "
-00012930: 656e 6422 2c20 7465 7874 3d69 7465 6d5b  end", text=item[
-00012940: 226e 616d 6522 5d2e 6c6a 7573 7428 3530  "name"].ljust(50
-00012950: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00012960: 2020 2077 6974 6820 636f 6e74 6578 746c     with contextl
-00012970: 6962 2e73 7570 7072 6573 7328 4b65 7945  ib.suppress(KeyE
-00012980: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-00012990: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000129a0: 696e 7365 7274 5f69 7465 6d73 2869 7465  insert_items(ite
-000129b0: 6d5b 2263 6869 6c64 7265 6e22 5d2c 2074  m["children"], t
-000129c0: 6865 5f69 6429 0a20 2020 2020 2020 2020  he_id).         
-000129d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000129e0: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-000129f0: 6565 7669 6577 2e69 6e73 6572 7428 7061  eeview.insert(pa
-00012a00: 7265 6e74 2c20 2265 6e64 222c 2074 6578  rent, "end", tex
-00012a10: 743d 6974 656d 290a 0a0a 2320 2323 2323  t=item)...# ####
-00012a20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012a30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012a60: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
-00012a70: 2044 6566 696e 6520 7468 6520 5472 6565   Define the Tree
-00012a80: 7669 6577 2077 696e 646f 770a 2320 2323  view window.# ##
-00012a90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012ab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012ac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012ad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012ae0: 0a63 6c61 7373 2054 7265 6576 6965 7757  .class TreeviewW
-00012af0: 696e 646f 7728 6374 6b2e 4354 6b54 6f70  indow(ctk.CTkTop
-00012b00: 6c65 7665 6c29 3a0a 2020 2020 2222 2244  level):.    """D
-00012b10: 6566 696e 6520 6f75 7220 746f 7020 6c65  efine our top le
-00012b20: 7665 6c20 7769 6e64 6f77 2066 6f72 2074  vel window for t
-00012b30: 6865 2074 7265 6520 7669 6577 2e22 2222  he tree view."""
-00012b40: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-00012b50: 5f5f 2873 656c 662c 202a 6172 6773 2c20  __(self, *args, 
-00012b60: 2a2a 6b77 6172 6773 2920 2d3e 204e 6f6e  **kwargs) -> Non
-00012b70: 653a 2020 2320 6e6f 7161 3a20 414e 4e30  e:  # noqa: ANN0
-00012b80: 3032 2c20 414e 4e30 3033 0a20 2020 2020  02, ANN003.     
-00012b90: 2020 2022 2222 4372 6561 7465 7320 6120     """Creates a 
-00012ba0: 6c61 6265 6c20 7769 6467 6574 2066 6f72  label widget for
-00012bb0: 2061 2074 7265 6520 7669 6577 2e0a 2020   a tree view..  
-00012bc0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00012bd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012be0: 6c66 2028 6f62 6a65 6374 293a 2054 6865  lf (object): The
-00012bf0: 206f 626a 6563 7420 6265 696e 6720 7061   object being pa
-00012c00: 7373 6564 2e0a 2020 2020 2020 2020 2020  ssed..          
-00012c10: 2020 2a61 7267 7320 2861 6e79 293a 2041    *args (any): A
-00012c20: 6464 6974 696f 6e61 6c20 6172 6775 6d65  dditional argume
-00012c30: 6e74 732e 0a20 2020 2020 2020 2020 2020  nts..           
-00012c40: 202a 2a6b 7761 7267 7320 2861 6e79 293a   **kwargs (any):
-00012c50: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
-00012c60: 6f72 6420 6172 6775 6d65 6e74 732e 0a20  ord arguments.. 
-00012c70: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00012c80: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
-00012c90: 3a20 5468 6973 2066 756e 6374 696f 6e20  : This function 
-00012ca0: 646f 6573 206e 6f74 2072 6574 7572 6e20  does not return 
-00012cb0: 616e 7974 6869 6e67 2e0a 2020 2020 2020  anything..      
-00012cc0: 2020 5072 6f63 6573 7369 6e67 204c 6f67    Processing Log
-00012cd0: 6963 3a0a 2020 2020 2020 2020 2020 2020  ic:.            
-00012ce0: 2d20 496e 6974 6961 6c69 7a65 206c 6162  - Initialize lab
-00012cf0: 656c 2077 6964 6765 742e 0a20 2020 2020  el widget..     
-00012d00: 2020 2020 2020 202d 2050 6163 6b20 6c61         - Pack la
-00012d10: 6265 6c20 7769 6467 6574 2077 6974 6820  bel widget with 
-00012d20: 7061 6464 696e 672e 0a20 2020 2020 2020  padding..       
-00012d30: 2020 2020 202d 2053 6574 206c 6162 656c       - Set label
-00012d40: 2077 6964 6765 7420 7465 7874 2e22 2222   widget text."""
-00012d50: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00012d60: 2e5f 5f69 6e69 745f 5f28 2a61 7267 732c  .__init__(*args,
-00012d70: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
-00012d80: 2020 2073 656c 662e 6765 6f6d 6574 7279     self.geometry
-00012d90: 2822 3630 3078 3630 3022 290a 2020 2020  ("600x600").    
-00012da0: 2020 2020 7365 6c66 2e74 6974 6c65 2822      self.title("
-00012db0: 4d61 7054 6173 6b65 7220 436f 6e66 6967  MapTasker Config
-00012dc0: 7572 6174 696f 6e20 5472 6565 7669 6577  uration Treeview
-00012dd0: 2229 0a0a 0a23 2023 2323 2323 2323 2323  ")...# #########
-00012de0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012df0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012e00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012e10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012e20: 2323 2323 2323 2323 230a 2320 4469 7370  #########.# Disp
-00012e30: 6c61 7920 6120 416e 616c 7973 6973 2073  lay a Analysis s
-00012e40: 7472 7563 7475 7265 0a23 2023 2323 2323  tructure.# #####
-00012e50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012e60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012e70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012e80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012e90: 2323 2323 2323 2323 2323 2323 230a 636c  #############.cl
-00012ea0: 6173 7320 4354 6b41 6e61 6c79 7369 7376  ass CTkAnalysisv
-00012eb0: 6965 7728 6374 6b2e 4354 6b46 7261 6d65  iew(ctk.CTkFrame
-00012ec0: 293a 0a20 2020 2022 2222 436c 6173 7320  ):.    """Class 
-00012ed0: 746f 2068 616e 646c 6520 7468 6520 5472  to handle the Tr
-00012ee0: 6565 7669 6577 0a0a 2020 2020 4172 6773  eeview..    Args
-00012ef0: 3a0a 2020 2020 2020 2020 6374 6b20 2863  :.        ctk (c
-00012f00: 746b 293a 204f 7572 2047 5549 2066 7261  tk): Our GUI fra
-00012f10: 6d65 776f 726b 0a20 2020 2022 2222 0a0a  mework.    """..
-00012f20: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00012f30: 2873 656c 662c 206d 6173 7465 723a 2061  (self, master: a
-00012f40: 6e79 2c20 6d65 7373 6167 653a 2073 7472  ny, message: str
-00012f50: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00012f60: 2020 2022 2222 4675 6e63 7469 6f6e 3a0a     """Function:.
-00012f70: 2020 2020 2020 2020 6465 6620 5f5f 696e          def __in
-00012f80: 6974 5f5f 2873 656c 662c 206d 6173 7465  it__(self, maste
-00012f90: 723a 2061 6e79 2c20 6974 656d 733a 206c  r: any, items: l
-00012fa0: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
-00012fb0: 2020 496e 6974 6961 6c69 7a65 7320 6120    Initializes a 
-00012fc0: 416e 616c 7973 6973 7669 6577 2077 6964  Analysisview wid
-00012fd0: 6765 7420 7769 7468 2061 2067 6976 656e  get with a given
-00012fe0: 206d 6173 7465 7220 616e 6420 6c69 7374   master and list
-00012ff0: 206f 6620 6974 656d 732e 0a20 2020 2020   of items..     
-00013000: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00013010: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00013020: 2020 206d 6173 7465 7220 2861 6e79 293a     master (any):
-00013030: 2054 6865 2070 6172 656e 7420 7769 6467   The parent widg
-00013040: 6574 2066 6f72 2074 6865 2041 6e61 6c79  et for the Analy
-00013050: 7369 7376 6965 772e 0a20 2020 2020 2020  sisview..       
-00013060: 2020 2020 2020 2020 2069 7465 6d73 2028           items (
-00013070: 6c69 7374 293a 2041 206c 6973 7420 6f66  list): A list of
-00013080: 2069 7465 6d73 2074 6f20 6265 2069 6e73   items to be ins
-00013090: 6572 7465 6420 696e 746f 2074 6865 2041  erted into the A
-000130a0: 6e61 6c79 7369 7376 6965 772e 0a20 2020  nalysisview..   
-000130b0: 2020 2020 2020 2020 2052 6574 7572 6e73           Returns
-000130c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000130d0: 2020 4e6f 6e65 2e0a 2020 2020 2020 2020    None..        
-000130e0: 2020 2020 5072 6f63 6573 7369 6e67 204c      Processing L
-000130f0: 6f67 6963 3a0a 2020 2020 2020 2020 2020  ogic:.          
-00013100: 2020 2020 2020 2d20 5365 7473 2075 7020        - Sets up 
-00013110: 7468 6520 416e 616c 7973 6973 7669 6577  the Analysisview
-00013120: 2077 6964 6765 7420 7769 7468 2061 7070   widget with app
-00013130: 726f 7072 6961 7465 2073 7479 6c65 7320  ropriate styles 
-00013140: 616e 6420 6269 6e64 696e 6773 2e0a 2020  and bindings..  
-00013150: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00013160: 496e 7365 7274 7320 7468 6520 6769 7665  Inserts the give
-00013170: 6e20 6974 656d 7320 696e 746f 2074 6865  n items into the
-00013180: 2054 7265 6576 6965 772e 0a20 2020 2020   Treeview..     
-00013190: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-000131a0: 656c 662e 726f 6f74 203d 206d 6173 7465  elf.root = maste
-000131b0: 720a 2020 2020 2020 2020 7375 7065 7228  r.        super(
-000131c0: 292e 5f5f 696e 6974 5f5f 2873 656c 662e  ).__init__(self.
-000131d0: 726f 6f74 290a 0a20 2020 2020 2020 2073  root)..        s
-000131e0: 656c 662e 6772 6964 5f63 6f6c 756d 6e63  elf.grid_columnc
-000131f0: 6f6e 6669 6775 7265 2830 2c20 7765 6967  onfigure(0, weig
-00013200: 6874 3d31 290a 0a20 2020 2020 2020 2023  ht=1)..        #
-00013210: 2041 6464 2061 206c 6162 656c 2074 6f20   Add a label to 
-00013220: 7468 6520 746f 7020 6f66 2077 696e 646f  the top of windo
-00013230: 770a 2020 2020 2020 2020 2320 6f75 725f  w.        # our_
-00013240: 6c61 6265 6c20 3d20 2244 7261 6720 7468  label = "Drag th
-00013250: 6520 626f 7474 6f6d 206f 6620 7468 6520  e bottom of the 
-00013260: 7769 6e64 6f77 2074 6f20 6578 7061 6e64  window to expand
-00013270: 2061 7320 6e65 6564 6564 2e22 0a20 2020   as needed.".   
-00013280: 2020 2020 2023 2073 656c 662e 616e 616c       # self.anal
-00013290: 7973 6973 5f6c 6162 656c 203d 2063 746b  ysis_label = ctk
-000132a0: 2e43 546b 4c61 6265 6c28 6d61 7374 6572  .CTkLabel(master
-000132b0: 3d73 656c 662c 2074 6578 743d 6f75 725f  =self, text=our_
-000132c0: 6c61 6265 6c2c 2066 6f6e 743d 2822 222c  label, font=("",
-000132d0: 2031 3229 290a 2020 2020 2020 2020 2320   12)).        # 
-000132e0: 7365 6c66 2e61 6e61 6c79 7369 735f 6c61  self.analysis_la
-000132f0: 6265 6c2e 6772 6964 2872 6f77 3d30 2c20  bel.grid(row=0, 
-00013300: 636f 6c75 6d6e 3d31 2c20 7061 6478 3d31  column=1, padx=1
-00013310: 302c 2070 6164 793d 3130 2c20 7374 6963  0, pady=10, stic
-00013320: 6b79 3d22 6e22 290a 0a20 2020 2020 2020  ky="n")..       
-00013330: 2023 2042 6173 6963 2061 7070 6561 7261   # Basic appeara
-00013340: 6e63 6520 666f 7220 7465 7874 2c20 666f  nce for text, fo
-00013350: 7265 6772 6f75 6e64 2061 6e64 2062 6163  reground and bac
-00013360: 6b67 726f 756e 642e 0a20 2020 2020 2020  kground..       
-00013370: 2073 656c 662e 616e 616c 7973 6973 5f62   self.analysis_b
-00013380: 675f 636f 6c6f 7220 3d20 7365 6c66 2e72  g_color = self.r
-00013390: 6f6f 742e 5f61 7070 6c79 5f61 7070 6561  oot._apply_appea
-000133a0: 7261 6e63 655f 6d6f 6465 280a 2020 2020  rance_mode(.    
-000133b0: 2020 2020 2020 2020 6374 6b2e 5468 656d          ctk.Them
-000133c0: 654d 616e 6167 6572 2e74 6865 6d65 5b22  eManager.theme["
-000133d0: 4354 6b46 7261 6d65 225d 5b22 6667 5f63  CTkFrame"]["fg_c
-000133e0: 6f6c 6f72 225d 0a20 2020 2020 2020 2029  olor"].        )
-000133f0: 2020 2320 6e6f 7161 3a20 534c 4630 3031    # noqa: SLF001
-00013400: 0a20 2020 2020 2020 2073 656c 662e 616e  .        self.an
-00013410: 616c 7973 6973 5f74 6578 745f 636f 6c6f  alysis_text_colo
-00013420: 7220 3d20 7365 6c66 2e72 6f6f 742e 5f61  r = self.root._a
-00013430: 7070 6c79 5f61 7070 6561 7261 6e63 655f  pply_appearance_
-00013440: 6d6f 6465 2820 2023 206e 6f71 613a 2053  mode(  # noqa: S
-00013450: 4c46 3030 310a 2020 2020 2020 2020 2020  LF001.          
-00013460: 2020 6374 6b2e 5468 656d 654d 616e 6167    ctk.ThemeManag
-00013470: 6572 2e74 6865 6d65 5b22 4354 6b4c 6162  er.theme["CTkLab
-00013480: 656c 225d 5b22 7465 7874 5f63 6f6c 6f72  el"]["text_color
-00013490: 225d 2c0a 2020 2020 2020 2020 290a 2020  "],.        ).  
-000134a0: 2020 2020 2020 7365 6c66 2e73 656c 6563        self.selec
-000134b0: 7465 645f 636f 6c6f 7220 3d20 7365 6c66  ted_color = self
-000134c0: 2e72 6f6f 742e 5f61 7070 6c79 5f61 7070  .root._apply_app
-000134d0: 6561 7261 6e63 655f 6d6f 6465 2820 2023  earance_mode(  #
-000134e0: 206e 6f71 613a 2053 4c46 3030 310a 2020   noqa: SLF001.  
-000134f0: 2020 2020 2020 2020 2020 6374 6b2e 5468            ctk.Th
-00013500: 656d 654d 616e 6167 6572 2e74 6865 6d65  emeManager.theme
-00013510: 5b22 4354 6b42 7574 746f 6e22 5d5b 2266  ["CTkButton"]["f
-00013520: 675f 636f 6c6f 7222 5d2c 0a20 2020 2020  g_color"],.     
-00013530: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-00013540: 5365 7420 7570 2074 6865 2073 7479 6c65  Set up the style
-00013550: 2f74 6865 6d65 0a20 2020 2020 2020 2073  /theme.        s
-00013560: 656c 662e 616e 616c 7973 6973 5f73 7479  elf.analysis_sty
-00013570: 6c65 203d 2074 746b 2e53 7479 6c65 2873  le = ttk.Style(s
-00013580: 656c 6629 0a20 2020 2020 2020 2073 656c  elf).        sel
-00013590: 662e 616e 616c 7973 6973 5f73 7479 6c65  f.analysis_style
-000135a0: 2e74 6865 6d65 5f75 7365 2822 6465 6661  .theme_use("defa
-000135b0: 756c 7422 290a 0a20 2020 2020 2020 2023  ult")..        #
-000135c0: 2052 6563 7265 6174 6520 7465 7874 2062   Recreate text b
-000135d0: 6f78 0a20 2020 2020 2020 2073 656c 662e  ox.        self.
-000135e0: 616e 616c 7973 6973 5f74 6578 7462 6f78  analysis_textbox
-000135f0: 203d 2063 746b 2e43 546b 5465 7874 626f   = ctk.CTkTextbo
-00013600: 7828 7365 6c66 2c20 6865 6967 6874 3d37  x(self, height=7
-00013610: 3030 2c20 7769 6474 683d 3535 3029 0a20  00, width=550). 
-00013620: 2020 2020 2020 2073 656c 662e 616e 616c         self.anal
-00013630: 7973 6973 5f74 6578 7462 6f78 2e67 7269  ysis_textbox.gri
-00013640: 6428 726f 773d 312c 2063 6f6c 756d 6e3d  d(row=1, column=
-00013650: 312c 2070 6164 783d 3230 2c20 7061 6479  1, padx=20, pady
-00013660: 3d34 302c 2073 7469 636b 793d 226e 7365  =40, sticky="nse
-00013670: 7722 290a 0a20 2020 2020 2020 2023 2049  w")..        # I
-00013680: 6e73 6572 7420 7468 6520 7465 7874 2077  nsert the text w
-00013690: 6974 6820 6f75 7220 6e65 7720 6d65 7373  ith our new mess
-000136a0: 6167 6520 696e 746f 2074 6865 2074 6578  age into the tex
-000136b0: 7420 626f 782e 0a20 2020 2020 2020 2023  t box..        #
-000136c0: 2041 6464 2074 6865 2074 6573 7420 616e   Add the test an
-000136d0: 6420 636f 6c6f 7220 746f 2074 6865 2074  d color to the t
-000136e0: 6578 7420 626f 782e 0a20 2020 2020 2020  ext box..       
-000136f0: 2023 2066 6d74 3a20 6f66 660a 2020 2020   # fmt: off.    
-00013700: 2020 2020 7365 6c66 2e61 6e61 6c79 7369      self.analysi
-00013710: 735f 7465 7874 626f 782e 696e 7365 7274  s_textbox.insert
-00013720: 2822 302e 3022 2c20 6622 7b6d 6573 7361  ("0.0", f"{messa
-00013730: 6765 7d5c 6e22 290a 2020 2020 2020 2020  ge}\n").        
-00013740: 7365 6c66 2e61 6e61 6c79 7369 735f 7465  self.analysis_te
-00013750: 7874 626f 782e 636f 6e66 6967 7572 6528  xtbox.configure(
-00013760: 7374 6174 653d 2264 6973 6162 6c65 6422  state="disabled"
-00013770: 2920 2023 2063 6f6e 6669 6775 7265 2074  )  # configure t
-00013780: 6578 7462 6f78 2074 6f20 6265 2072 6561  extbox to be rea
-00013790: 642d 6f6e 6c79 0a20 2020 2020 2020 2073  d-only.        s
-000137a0: 656c 662e 616e 616c 7973 6973 5f74 6578  elf.analysis_tex
-000137b0: 7462 6f78 2e63 6f6e 6669 6775 7265 2877  tbox.configure(w
-000137c0: 7261 703d 2277 6f72 6422 290a 2020 2020  rap="word").    
-000137d0: 2020 2020 7365 6c66 2e61 6e61 6c79 7369      self.analysi
-000137e0: 735f 7465 7874 626f 782e 666f 6375 735f  s_textbox.focus_
-000137f0: 7365 7428 290a 0a0a 2320 2323 2323 2323  set()...# ######
-00013800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013840: 2323 2323 2323 2323 2323 2323 0a23 2044  ############.# D
-00013850: 6566 696e 6520 7468 6520 4169 2041 6e61  efine the Ai Ana
-00013860: 6c79 7369 7320 7769 6e64 6f77 0a23 2023  lysis window.# #
-00013870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013880: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013890: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000138a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000138b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000138c0: 230a 636c 6173 7320 416e 616c 7973 6973  #.class Analysis
-000138d0: 5769 6e64 6f77 2863 746b 2e43 546b 546f  Window(ctk.CTkTo
-000138e0: 706c 6576 656c 293a 0a20 2020 2022 2222  plevel):.    """
-000138f0: 4465 6669 6e65 206f 7572 2074 6f70 206c  Define our top l
-00013900: 6576 656c 2077 696e 646f 7720 666f 7220  evel window for 
-00013910: 7468 6520 616e 616c 7973 6973 2076 6965  the analysis vie
-00013920: 772e 2222 220a 0a20 2020 2064 6566 205f  w."""..    def _
-00013930: 5f69 6e69 745f 5f28 7365 6c66 2c20 2a61  _init__(self, *a
-00013940: 7267 732c 202a 2a6b 7761 7267 7329 202d  rgs, **kwargs) -
-00013950: 3e20 4e6f 6e65 3a20 2023 206e 6f71 613a  > None:  # noqa:
-00013960: 2041 4e4e 3030 322c 2041 4e4e 3030 330a   ANN002, ANN003.
-00013970: 2020 2020 2020 2020 2222 2243 7265 6174          """Creat
-00013980: 6573 2061 206c 6162 656c 2077 6964 6765  es a label widge
-00013990: 7420 666f 7220 6120 7472 6565 2076 6965  t for a tree vie
-000139a0: 772e 0a20 2020 2020 2020 2050 6172 616d  w..        Param
-000139b0: 6574 6572 733a 0a20 2020 2020 2020 2020  eters:.         
-000139c0: 2020 2073 656c 6620 286f 626a 6563 7429     self (object)
-000139d0: 3a20 5468 6520 6f62 6a65 6374 2062 6569  : The object bei
-000139e0: 6e67 2070 6173 7365 642e 0a20 2020 2020  ng passed..     
-000139f0: 2020 2020 2020 202a 6172 6773 2028 616e         *args (an
-00013a00: 7929 3a20 4164 6469 7469 6f6e 616c 2061  y): Additional a
-00013a10: 7267 756d 656e 7473 2e0a 2020 2020 2020  rguments..      
-00013a20: 2020 2020 2020 2a2a 6b77 6172 6773 2028        **kwargs (
-00013a30: 616e 7929 3a20 4164 6469 7469 6f6e 616c  any): Additional
-00013a40: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-00013a50: 7473 2e0a 2020 2020 2020 2020 5265 7475  ts..        Retu
-00013a60: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00013a70: 204e 6f6e 653a 2054 6869 7320 6675 6e63   None: This func
-00013a80: 7469 6f6e 2064 6f65 7320 6e6f 7420 7265  tion does not re
-00013a90: 7475 726e 2061 6e79 7468 696e 672e 0a20  turn anything.. 
-00013aa0: 2020 2020 2020 2050 726f 6365 7373 696e         Processin
-00013ab0: 6720 4c6f 6769 633a 0a20 2020 2020 2020  g Logic:.       
-00013ac0: 2020 2020 202d 2049 6e69 7469 616c 697a       - Initializ
-00013ad0: 6520 6c61 6265 6c20 7769 6467 6574 2e0a  e label widget..
-00013ae0: 2020 2020 2020 2020 2020 2020 2d20 5061              - Pa
-00013af0: 636b 206c 6162 656c 2077 6964 6765 7420  ck label widget 
-00013b00: 7769 7468 2070 6164 6469 6e67 2e0a 2020  with padding..  
-00013b10: 2020 2020 2020 2020 2020 2d20 5365 7420            - Set 
-00013b20: 6c61 6265 6c20 7769 6467 6574 2074 6578  label widget tex
-00013b30: 742e 2222 220a 2020 2020 2020 2020 7375  t.""".        su
-00013b40: 7065 7228 292e 5f5f 696e 6974 5f5f 282a  per().__init__(*
-00013b50: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
-00013b60: 2020 2020 2020 2020 7365 6c66 2e67 656f          self.geo
-00013b70: 6d65 7472 7928 2236 3030 7838 3030 2b36  metry("600x800+6
-00013b80: 3030 2b30 2229 0a20 2020 2020 2020 2073  00+0").        s
-00013b90: 656c 662e 7469 746c 6528 224d 6170 5461  elf.title("MapTa
-00013ba0: 736b 6572 2041 6e61 6c79 7369 7320 5265  sker Analysis Re
-00013bb0: 7370 6f6e 7365 2229 0a0a 0a23 2023 2323  sponse")...# ###
-00013bc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013bd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013bf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013c00: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00013c10: 2320 4465 6669 6e65 2074 6865 2041 6920  # Define the Ai 
-00013c20: 506f 7075 7020 7769 6e64 6f77 0a23 2023  Popup window.# #
-00013c30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013c40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013c50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013c60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013c70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013c80: 230a 636c 6173 7320 506f 7075 7057 696e  #.class PopupWin
-00013c90: 646f 7728 6374 6b2e 4354 6b29 3a0a 2020  dow(ctk.CTk):.  
-00013ca0: 2020 2222 2244 6566 696e 6520 6f75 7220    """Define our 
-00013cb0: 746f 7020 6c65 7665 6c20 7769 6e64 6f77  top level window
-00013cc0: 2066 6f72 2074 6865 2050 6f70 7570 2076   for the Popup v
-00013cd0: 6965 772e 2222 220a 0a20 2020 2064 6566  iew."""..    def
-00013ce0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00013cf0: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-00013d00: 202d 3e20 4e6f 6e65 3a20 2023 206e 6f71   -> None:  # noq
-00013d10: 613a 2041 4e4e 3030 322c 2041 4e4e 3030  a: ANN002, ANN00
-00013d20: 330a 2020 2020 2020 2020 2222 2243 7265  3.        """Cre
-00013d30: 6174 6573 2061 206c 6162 656c 2077 6964  ates a label wid
-00013d40: 6765 7420 666f 7220 6120 7472 6565 2076  get for a tree v
-00013d50: 6965 772e 0a20 2020 2020 2020 2050 6172  iew..        Par
-00013d60: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
-00013d70: 2020 2020 2073 656c 6620 286f 626a 6563       self (objec
-00013d80: 7429 3a20 5468 6520 6f62 6a65 6374 2062  t): The object b
-00013d90: 6569 6e67 2070 6173 7365 642e 0a20 2020  eing passed..   
-00013da0: 2020 2020 2020 2020 202a 6172 6773 2028           *args (
-00013db0: 616e 7929 3a20 4164 6469 7469 6f6e 616c  any): Additional
-00013dc0: 2061 7267 756d 656e 7473 2e0a 2020 2020   arguments..    
-00013dd0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-00013de0: 2028 616e 7929 3a20 4164 6469 7469 6f6e   (any): Addition
-00013df0: 616c 206b 6579 776f 7264 2061 7267 756d  al keyword argum
-00013e00: 656e 7473 2e0a 2020 2020 2020 2020 5265  ents..        Re
-00013e10: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00013e20: 2020 204e 6f6e 653a 2054 6869 7320 6675     None: This fu
-00013e30: 6e63 7469 6f6e 2064 6f65 7320 6e6f 7420  nction does not 
-00013e40: 7265 7475 726e 2061 6e79 7468 696e 672e  return anything.
-00013e50: 0a20 2020 2020 2020 2050 726f 6365 7373  .        Process
-00013e60: 696e 6720 4c6f 6769 633a 0a20 2020 2020  ing Logic:.     
-00013e70: 2020 2020 2020 202d 2049 6e69 7469 616c         - Initial
-00013e80: 697a 6520 6c61 6265 6c20 7769 6467 6574  ize label widget
-00013e90: 2e0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
-00013ea0: 5061 636b 206c 6162 656c 2077 6964 6765  Pack label widge
-00013eb0: 7420 7769 7468 2070 6164 6469 6e67 2e0a  t with padding..
-00013ec0: 2020 2020 2020 2020 2020 2020 2d20 5365              - Se
-00013ed0: 7420 6c61 6265 6c20 7769 6467 6574 2074  t label widget t
-00013ee0: 6578 742e 2222 220a 2020 2020 2020 2020  ext.""".        
-00013ef0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-00013f00: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
-00013f10: 290a 2020 2020 2020 2020 2320 4765 7420  ).        # Get 
-00013f20: 7468 6520 7363 7265 656e 2073 697a 650a  the screen size.
-00013f30: 2020 2020 2020 2020 7363 7265 656e 5f77          screen_w
-00013f40: 6964 7468 203d 2073 656c 662e 7769 6e66  idth = self.winf
-00013f50: 6f5f 7363 7265 656e 7769 6474 6828 290a  o_screenwidth().
-00013f60: 2020 2020 2020 2020 7363 7265 656e 5f68          screen_h
-00013f70: 6569 6768 7420 3d20 7365 6c66 2e77 696e  eight = self.win
-00013f80: 666f 5f73 6372 6565 6e68 6569 6768 7428  fo_screenheight(
-00013f90: 290a 0a20 2020 2020 2020 2023 2043 656e  )..        # Cen
-00013fa0: 7465 7220 7468 6520 7769 6467 6574 0a20  ter the widget. 
-00013fb0: 2020 2020 2020 2073 656c 662e 6765 6f6d         self.geom
-00013fc0: 6574 7279 2866 2235 3030 7835 302b 7b73  etry(f"500x50+{s
-00013fd0: 6372 6565 6e5f 7769 6474 682f 2f33 7d2b  creen_width//3}+
-00013fe0: 7b73 6372 6565 6e5f 6865 6967 6874 2f2f  {screen_height//
-00013ff0: 3130 7d22 290a 2020 2020 2020 2020 7365  10}").        se
-00014000: 6c66 2e74 6974 6c65 2822 4d61 7054 6173  lf.title("MapTas
-00014010: 6b65 7220 416e 616c 7973 6973 2229 0a0a  ker Analysis")..
-00014020: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
-00014030: 645f 636f 6c75 6d6e 636f 6e66 6967 7572  d_columnconfigur
-00014040: 6528 302c 2077 6569 6768 743d 3129 0a0a  e(0, weight=1)..
-00014050: 2020 2020 2020 2020 2320 4973 7375 6520          # Issue 
-00014060: 636f 6d6d 616e 6420 6166 7472 2035 2073  command aftr 5 s
-00014070: 6563 6f6e 6473 0a20 2020 2020 2020 2073  econds.        s
-00014080: 656c 662e 6166 7465 7228 3530 3030 2c20  elf.after(5000, 
-00014090: 7365 6c66 2e70 6f70 7570 5f62 7574 746f  self.popup_butto
-000140a0: 6e5f 6576 656e 7429 0a0a 2020 2020 2020  n_event)..      
-000140b0: 2020 2320 4c61 6265 6c20 7769 6467 6574    # Label widget
-000140c0: 0a20 2020 2020 2020 206f 7572 5f6c 6162  .        our_lab
-000140d0: 656c 203d 2022 416e 616c 7973 6973 2069  el = "Analysis i
-000140e0: 7320 7275 6e6e 696e 6720 696e 2074 6865  s running in the
-000140f0: 2062 6163 6b67 726f 756e 642e 2020 506c   background.  Pl
-00014100: 6561 7365 2073 7461 6e64 2062 792e 2e2e  ease stand by...
-00014110: 220a 2020 2020 2020 2020 7365 6c66 2e50  ".        self.P
-00014120: 6f70 7570 5f6c 6162 656c 203d 2063 746b  opup_label = ctk
-00014130: 2e43 546b 4c61 6265 6c28 6d61 7374 6572  .CTkLabel(master
-00014140: 3d73 656c 662c 2074 6578 743d 6f75 725f  =self, text=our_
-00014150: 6c61 6265 6c2c 2066 6f6e 743d 2822 222c  label, font=("",
-00014160: 2031 3229 290a 2020 2020 2020 2020 7365   12)).        se
-00014170: 6c66 2e50 6f70 7570 5f6c 6162 656c 2e67  lf.Popup_label.g
-00014180: 7269 6428 726f 773d 302c 2063 6f6c 756d  rid(row=0, colum
-00014190: 6e3d 302c 2070 6164 783d 302c 2070 6164  n=0, padx=0, pad
-000141a0: 793d 3130 2c20 7374 6963 6b79 3d22 6e22  y=10, sticky="n"
-000141b0: 290a 0a20 2020 2020 2020 2023 2042 6173  )..        # Bas
-000141c0: 6963 2061 7070 6561 7261 6e63 6520 666f  ic appearance fo
-000141d0: 7220 7465 7874 2c20 666f 7265 6772 6f75  r text, foregrou
-000141e0: 6e64 2061 6e64 2062 6163 6b67 726f 756e  nd and backgroun
-000141f0: 642e 0a20 2020 2020 2020 2073 656c 662e  d..        self.
-00014200: 506f 7075 705f 6267 5f63 6f6c 6f72 203d  Popup_bg_color =
-00014210: 2073 656c 662e 5f61 7070 6c79 5f61 7070   self._apply_app
-00014220: 6561 7261 6e63 655f 6d6f 6465 2863 746b  earance_mode(ctk
-00014230: 2e54 6865 6d65 4d61 6e61 6765 722e 7468  .ThemeManager.th
-00014240: 656d 655b 2243 546b 4672 616d 6522 5d5b  eme["CTkFrame"][
-00014250: 2266 675f 636f 6c6f 7222 5d29 0a20 2020  "fg_color"]).   
-00014260: 2020 2020 2073 656c 662e 506f 7075 705f       self.Popup_
-00014270: 7465 7874 5f63 6f6c 6f72 203d 2073 656c  text_color = sel
-00014280: 662e 5f61 7070 6c79 5f61 7070 6561 7261  f._apply_appeara
-00014290: 6e63 655f 6d6f 6465 280a 2020 2020 2020  nce_mode(.      
-000142a0: 2020 2020 2020 6374 6b2e 5468 656d 654d        ctk.ThemeM
-000142b0: 616e 6167 6572 2e74 6865 6d65 5b22 4354  anager.theme["CT
-000142c0: 6b4c 6162 656c 225d 5b22 7465 7874 5f63  kLabel"]["text_c
-000142d0: 6f6c 6f72 225d 2c0a 2020 2020 2020 2020  olor"],.        
-000142e0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-000142f0: 656c 6563 7465 645f 636f 6c6f 7220 3d20  elected_color = 
-00014300: 7365 6c66 2e5f 6170 706c 795f 6170 7065  self._apply_appe
-00014310: 6172 616e 6365 5f6d 6f64 6528 0a20 2020  arance_mode(.   
-00014320: 2020 2020 2020 2020 2063 746b 2e54 6865           ctk.The
-00014330: 6d65 4d61 6e61 6765 722e 7468 656d 655b  meManager.theme[
-00014340: 2243 546b 4275 7474 6f6e 225d 5b22 6667  "CTkButton"]["fg
-00014350: 5f63 6f6c 6f72 225d 2c0a 2020 2020 2020  _color"],.      
-00014360: 2020 290a 0a20 2020 2020 2020 2023 2053    )..        # S
-00014370: 6574 2075 7020 7468 6520 7374 796c 652f  et up the style/
-00014380: 7468 656d 650a 2020 2020 2020 2020 7365  theme.        se
-00014390: 6c66 2e50 6f70 7570 5f73 7479 6c65 203d  lf.Popup_style =
-000143a0: 2074 746b 2e53 7479 6c65 2873 656c 6629   ttk.Style(self)
-000143b0: 0a20 2020 2020 2020 2073 656c 662e 506f  .        self.Po
-000143c0: 7075 705f 7374 796c 652e 7468 656d 655f  pup_style.theme_
-000143d0: 7573 6528 2264 6566 6175 6c74 2229 0a0a  use("default")..
-000143e0: 2020 2020 2020 2020 2323 2052 6563 7265          ## Recre
-000143f0: 6174 6520 7465 7874 2062 6f78 0a20 2020  ate text box.   
-00014400: 2020 2020 2023 2073 656c 662e 706f 7075       # self.popu
-00014410: 705f 6275 7474 6f6e 203d 2063 746b 2e43  p_button = ctk.C
-00014420: 546b 4275 7474 6f6e 280a 2020 2020 2020  TkButton(.      
-00014430: 2020 2320 2020 206d 6173 7465 723d 7365    #    master=se
-00014440: 6c66 2c0a 2020 2020 2020 2020 2320 2020  lf,.        #   
-00014450: 2077 6964 7468 3d31 3230 2c0a 2020 2020   width=120,.    
-00014460: 2020 2020 2320 2020 2068 6569 6768 743d      #    height=
-00014470: 3332 2c0a 2020 2020 2020 2020 2320 2020  32,.        #   
-00014480: 2062 6f72 6465 725f 7769 6474 683d 302c   border_width=0,
-00014490: 0a20 2020 2020 2020 2023 2020 2020 636f  .        #    co
-000144a0: 726e 6572 5f72 6164 6975 733d 382c 0a20  rner_radius=8,. 
-000144b0: 2020 2020 2020 2023 2020 2020 7465 7874         #    text
-000144c0: 3d22 436c 6963 6b20 746f 2063 6c6f 7365  ="Click to close
-000144d0: 2074 6869 7320 7769 6e64 6f77 222c 0a20   this window",. 
-000144e0: 2020 2020 2020 2023 2020 2020 636f 6d6d         #    comm
-000144f0: 616e 643d 7365 6c66 2e70 6f70 7570 5f62  and=self.popup_b
-00014500: 7574 746f 6e5f 6576 656e 742c 0a20 2020  utton_event,.   
-00014510: 2020 2020 2023 2029 0a20 2020 2020 2020       # ).       
-00014520: 2023 2073 656c 662e 706f 7075 705f 6275   # self.popup_bu
-00014530: 7474 6f6e 2e70 6c61 6365 2872 656c 783d  tton.place(relx=
-00014540: 302e 352c 2072 656c 793d 302e 3529 0a20  0.5, rely=0.5). 
-00014550: 2020 2020 2020 2023 2073 656c 662e 706f         # self.po
-00014560: 7075 705f 6275 7474 6f6e 2e66 6f63 7573  pup_button.focus
-00014570: 5f73 6574 2829 0a0a 2020 2020 6465 6620  _set()..    def 
-00014580: 706f 7075 705f 6275 7474 6f6e 5f65 7665  popup_button_eve
-00014590: 6e74 2873 656c 6629 202d 3e20 4e6f 6e65  nt(self) -> None
-000145a0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000145b0: 2020 2020 2020 4465 6669 6e65 2074 6865        Define the
-000145c0: 2062 6568 6176 696f 7220 6f66 2074 6865   behavior of the
-000145d0: 2070 6f70 7570 2062 7574 746f 6e20 6576   popup button ev
-000145e0: 656e 7420 6675 6e63 7469 6f6e 2e20 2043  ent function.  C
-000145f0: 6c6f 7365 2074 6865 2077 696e 646f 7720  lose the window 
-00014600: 616e 6420 6578 6974 2e0a 2020 2020 2020  and exit..      
-00014610: 2020 2222 220a 2020 2020 2020 2020 5072    """.        Pr
-00014620: 696d 6549 7465 6d73 2e6c 6f6f 705f 6163  imeItems.loop_ac
-00014630: 7469 7665 203d 2046 616c 7365 0a20 2020  tive = False.   
-00014640: 2020 2020 2073 656c 662e 6578 6974 203d       self.exit =
-00014650: 2054 7275 650a 2020 2020 2020 2020 7365   True.        se
-00014660: 6c66 2e71 7569 7428 290a 2020 2020 2020  lf.quit().      
-00014670: 2020 7365 6c66 2e71 7569 7428 290a         self.quit().
+00008600: 5461 736b 6572 4e65 7420 496e 666f 222c  TaskerNet Info",
+00008610: 0a20 2020 2020 2020 2035 2c0a 2020 2020  .        5,.    
+00008620: 2020 2020 302c 0a20 2020 2020 2020 2032      0,.        2
+00008630: 302c 0a20 2020 2020 2020 2031 302c 0a20  0,.        10,. 
+00008640: 2020 2020 2020 2022 7722 2c0a 2020 2020         "w",.    
+00008650: 2020 2020 2222 2c0a 2020 2020 290a 0a20      "",.    ).. 
+00008660: 2020 2023 2044 6973 706c 6179 2027 5461     # Display 'Ta
+00008670: 736b 6572 2050 7265 6665 7265 6e63 6573  sker Preferences
+00008680: 2720 6368 6563 6b62 6f78 0a20 2020 2073  ' checkbox.    s
+00008690: 656c 662e 7072 6566 6572 656e 6365 735f  elf.preferences_
+000086a0: 6368 6563 6b62 6f78 203d 2061 6464 5f63  checkbox = add_c
+000086b0: 6865 636b 626f 7828 0a20 2020 2020 2020  heckbox(.       
+000086c0: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
+000086d0: 656c 662e 7369 6465 6261 725f 6672 616d  elf.sidebar_fram
+000086e0: 652c 0a20 2020 2020 2020 2073 656c 662e  e,.        self.
+000086f0: 7072 6566 6572 656e 6365 735f 6576 656e  preferences_even
+00008700: 742c 0a20 2020 2020 2020 2022 4469 7370  t,.        "Disp
+00008710: 6c61 7920 5461 736b 6572 2050 7265 6665  lay Tasker Prefe
+00008720: 7265 6e63 6573 222c 0a20 2020 2020 2020  rences",.       
+00008730: 2036 2c0a 2020 2020 2020 2020 302c 0a20   6,.        0,. 
+00008740: 2020 2020 2020 2032 302c 0a20 2020 2020         20,.     
+00008750: 2020 2031 302c 0a20 2020 2020 2020 2022     10,.        "
+00008760: 7722 2c0a 2020 2020 2020 2020 2222 2c0a  w",.        "",.
+00008770: 2020 2020 290a 0a20 2020 2023 2044 6973      )..    # Dis
+00008780: 706c 6179 2027 5477 6973 7479 2720 6368  play 'Twisty' ch
+00008790: 6563 6b62 6f78 0a20 2020 2073 656c 662e  eckbox.    self.
+000087a0: 7477 6973 7479 5f63 6865 636b 626f 7820  twisty_checkbox 
+000087b0: 3d20 6164 645f 6368 6563 6b62 6f78 280a  = add_checkbox(.
+000087c0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000087d0: 2020 2020 2020 7365 6c66 2e73 6964 6562        self.sideb
+000087e0: 6172 5f66 7261 6d65 2c0a 2020 2020 2020  ar_frame,.      
+000087f0: 2020 7365 6c66 2e74 7769 7374 795f 6576    self.twisty_ev
+00008800: 656e 742c 0a20 2020 2020 2020 2022 4869  ent,.        "Hi
+00008810: 6465 2054 6173 6b20 4465 7461 696c 7320  de Task Details 
+00008820: 556e 6465 7220 5477 6973 7479 222c 0a20  Under Twisty",. 
+00008830: 2020 2020 2020 2037 2c0a 2020 2020 2020         7,.      
+00008840: 2020 302c 0a20 2020 2020 2020 2032 302c    0,.        20,
+00008850: 0a20 2020 2020 2020 2031 302c 0a20 2020  .        10,.   
+00008860: 2020 2020 2022 7722 2c0a 2020 2020 2020       "w",.      
+00008870: 2020 2222 2c0a 2020 2020 290a 0a20 2020    "",.    )..   
+00008880: 2023 2044 6973 706c 6179 2027 6469 7265   # Display 'dire
+00008890: 6374 6f72 7927 2063 6865 636b 626f 780a  ctory' checkbox.
+000088a0: 2020 2020 7365 6c66 2e64 6972 6563 746f      self.directo
+000088b0: 7279 5f63 6865 636b 626f 7820 3d20 6164  ry_checkbox = ad
+000088c0: 645f 6368 6563 6b62 6f78 280a 2020 2020  d_checkbox(.    
+000088d0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000088e0: 2020 7365 6c66 2e73 6964 6562 6172 5f66    self.sidebar_f
+000088f0: 7261 6d65 2c0a 2020 2020 2020 2020 7365  rame,.        se
+00008900: 6c66 2e64 6972 6563 746f 7279 5f65 7665  lf.directory_eve
+00008910: 6e74 2c0a 2020 2020 2020 2020 2244 6973  nt,.        "Dis
+00008920: 706c 6179 2044 6972 6563 746f 7279 222c  play Directory",
+00008930: 0a20 2020 2020 2020 2038 2c0a 2020 2020  .        8,.    
+00008940: 2020 2020 302c 0a20 2020 2020 2020 2032      0,.        2
+00008950: 302c 0a20 2020 2020 2020 2031 302c 0a20  0,.        10,. 
+00008960: 2020 2020 2020 2022 7722 2c0a 2020 2020         "w",.    
+00008970: 2020 2020 2222 2c0a 2020 2020 290a 0a20      "",.    ).. 
+00008980: 2020 2023 204f 7574 6c69 6e65 0a20 2020     # Outline.   
+00008990: 2073 656c 662e 6f75 746c 696e 655f 6368   self.outline_ch
+000089a0: 6563 6b62 6f78 203d 2061 6464 5f63 6865  eckbox = add_che
+000089b0: 636b 626f 7828 0a20 2020 2020 2020 2073  ckbox(.        s
+000089c0: 656c 662c 0a20 2020 2020 2020 2073 656c  elf,.        sel
+000089d0: 662e 7369 6465 6261 725f 6672 616d 652c  f.sidebar_frame,
+000089e0: 0a20 2020 2020 2020 2073 656c 662e 6f75  .        self.ou
+000089f0: 746c 696e 655f 6576 656e 742c 0a20 2020  tline_event,.   
+00008a00: 2020 2020 2022 4469 7370 6c61 7920 436f       "Display Co
+00008a10: 6e66 6967 7572 6174 696f 6e20 4f75 746c  nfiguration Outl
+00008a20: 696e 6522 2c0a 2020 2020 2020 2020 392c  ine",.        9,
+00008a30: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
+00008a40: 2020 2020 3230 2c0a 2020 2020 2020 2020      20,.        
+00008a50: 3130 2c0a 2020 2020 2020 2020 2277 222c  10,.        "w",
+00008a60: 0a20 2020 2020 2020 2022 222c 0a20 2020  .        "",.   
+00008a70: 2029 0a0a 2020 2020 2320 5072 6574 7479   )..    # Pretty
+00008a80: 204f 7574 7075 740a 2020 2020 7365 6c66   Output.    self
+00008a90: 2e70 7265 7474 795f 6368 6563 6b62 6f78  .pretty_checkbox
+00008aa0: 203d 2061 6464 5f63 6865 636b 626f 7828   = add_checkbox(
+00008ab0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00008ac0: 2020 2020 2020 2073 656c 662e 7369 6465         self.side
+00008ad0: 6261 725f 6672 616d 652c 0a20 2020 2020  bar_frame,.     
+00008ae0: 2020 2073 656c 662e 7072 6574 7479 5f65     self.pretty_e
+00008af0: 7665 6e74 2c0a 2020 2020 2020 2020 2244  vent,.        "D
+00008b00: 6973 706c 6179 2050 7265 7474 6965 7220  isplay Prettier 
+00008b10: 4f75 7470 7574 222c 0a20 2020 2020 2020  Output",.       
+00008b20: 2031 302c 0a20 2020 2020 2020 2030 2c0a   10,.        0,.
+00008b30: 2020 2020 2020 2020 3230 2c0a 2020 2020          20,.    
+00008b40: 2020 2020 3130 2c0a 2020 2020 2020 2020      10,.        
+00008b50: 2277 222c 0a20 2020 2020 2020 2022 222c  "w",.        "",
+00008b60: 0a20 2020 2029 0a0a 2020 2020 2320 4e61  .    )..    # Na
+00008b70: 6d65 733a 2042 6f6c 6420 2f20 4869 6768  mes: Bold / High
+00008b80: 6c69 6768 7420 2f20 4974 616c 6963 6973  light / Italicis
+00008b90: 6520 2f20 556e 6465 726c 696e 650a 2020  e / Underline.  
+00008ba0: 2020 7365 6c66 2e64 6973 706c 6179 5f6e    self.display_n
+00008bb0: 616d 6573 5f6c 6162 656c 203d 2061 6464  ames_label = add
+00008bc0: 5f6c 6162 656c 280a 2020 2020 2020 2020  _label(.        
+00008bd0: 7365 6c66 2c0a 2020 2020 2020 2020 7365  self,.        se
+00008be0: 6c66 2e73 6964 6562 6172 5f66 7261 6d65  lf.sidebar_frame
+00008bf0: 2c0a 2020 2020 2020 2020 2250 726f 6a65  ,.        "Proje
+00008c00: 6374 2f50 726f 6669 6c65 2f54 6173 6b2f  ct/Profile/Task/
+00008c10: 5363 656e 6520 4e61 6d65 733a 222c 0a20  Scene Names:",. 
+00008c20: 2020 2020 2020 2022 222c 0a20 2020 2020         "",.     
+00008c30: 2020 2030 2c0a 2020 2020 2020 2020 226e     0,.        "n
+00008c40: 6f72 6d61 6c22 2c0a 2020 2020 2020 2020  ormal",.        
+00008c50: 3131 2c0a 2020 2020 2020 2020 302c 0a20  11,.        0,. 
+00008c60: 2020 2020 2020 2032 302c 0a20 2020 2020         20,.     
+00008c70: 2020 2031 302c 0a20 2020 2020 2020 2022     10,.        "
+00008c80: 7322 2c0a 2020 2020 290a 0a20 2020 2023  s",.    )..    #
+00008c90: 2042 6f6c 640a 2020 2020 7365 6c66 2e62   Bold.    self.b
+00008ca0: 6f6c 645f 6368 6563 6b62 6f78 203d 2061  old_checkbox = a
+00008cb0: 6464 5f63 6865 636b 626f 7828 7365 6c66  dd_checkbox(self
+00008cc0: 2c20 7365 6c66 2e73 6964 6562 6172 5f66  , self.sidebar_f
+00008cd0: 7261 6d65 2c20 7365 6c66 2e6e 616d 6573  rame, self.names
+00008ce0: 5f62 6f6c 645f 6576 656e 742c 2022 426f  _bold_event, "Bo
+00008cf0: 6c64 222c 2031 322c 2030 2c20 3230 2c20  ld", 12, 0, 20, 
+00008d00: 302c 2022 6e65 222c 2022 2229 0a0a 2020  0, "ne", "")..  
+00008d10: 2020 2320 4974 616c 6963 697a 650a 2020    # Italicize.  
+00008d20: 2020 7365 6c66 2e69 7461 6c69 6369 7a65    self.italicize
+00008d30: 5f63 6865 636b 626f 7820 3d20 6164 645f  _checkbox = add_
+00008d40: 6368 6563 6b62 6f78 280a 2020 2020 2020  checkbox(.      
+00008d50: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00008d60: 7365 6c66 2e73 6964 6562 6172 5f66 7261  self.sidebar_fra
+00008d70: 6d65 2c0a 2020 2020 2020 2020 7365 6c66  me,.        self
+00008d80: 2e6e 616d 6573 5f69 7461 6c69 6369 7a65  .names_italicize
+00008d90: 5f65 7665 6e74 2c0a 2020 2020 2020 2020  _event,.        
+00008da0: 2269 7461 6c69 6369 7a65 222c 0a20 2020  "italicize",.   
+00008db0: 2020 2020 2031 322c 0a20 2020 2020 2020       12,.       
+00008dc0: 2030 2c0a 2020 2020 2020 2020 3230 2c0a   0,.        20,.
+00008dd0: 2020 2020 2020 2020 302c 0a20 2020 2020          0,.     
+00008de0: 2020 2022 6e77 222c 0a20 2020 2020 2020     "nw",.       
+00008df0: 2022 222c 0a20 2020 2029 0a0a 2020 2020   "",.    )..    
+00008e00: 2320 4869 6768 6c69 6768 740a 2020 2020  # Highlight.    
+00008e10: 7365 6c66 2e68 6967 686c 6967 6874 5f63  self.highlight_c
+00008e20: 6865 636b 626f 7820 3d20 6164 645f 6368  heckbox = add_ch
+00008e30: 6563 6b62 6f78 280a 2020 2020 2020 2020  eckbox(.        
+00008e40: 7365 6c66 2c0a 2020 2020 2020 2020 7365  self,.        se
+00008e50: 6c66 2e73 6964 6562 6172 5f66 7261 6d65  lf.sidebar_frame
+00008e60: 2c0a 2020 2020 2020 2020 7365 6c66 2e6e  ,.        self.n
+00008e70: 616d 6573 5f68 6967 686c 6967 6874 5f65  ames_highlight_e
+00008e80: 7665 6e74 2c0a 2020 2020 2020 2020 2248  vent,.        "H
+00008e90: 6967 686c 6967 6874 222c 0a20 2020 2020  ighlight",.     
+00008ea0: 2020 2031 332c 0a20 2020 2020 2020 2030     13,.        0
+00008eb0: 2c0a 2020 2020 2020 2020 3230 2c0a 2020  ,.        20,.  
+00008ec0: 2020 2020 2020 352c 0a20 2020 2020 2020        5,.       
+00008ed0: 2022 6e65 222c 0a20 2020 2020 2020 2022   "ne",.        "
+00008ee0: 222c 0a20 2020 2029 0a0a 2020 2020 2320  ",.    )..    # 
+00008ef0: 556e 6465 726c 696e 650a 2020 2020 7365  Underline.    se
+00008f00: 6c66 2e75 6e64 6572 6c69 6e65 5f63 6865  lf.underline_che
+00008f10: 636b 626f 7820 3d20 6164 645f 6368 6563  ckbox = add_chec
+00008f20: 6b62 6f78 280a 2020 2020 2020 2020 7365  kbox(.        se
+00008f30: 6c66 2c0a 2020 2020 2020 2020 7365 6c66  lf,.        self
+00008f40: 2e73 6964 6562 6172 5f66 7261 6d65 2c0a  .sidebar_frame,.
+00008f50: 2020 2020 2020 2020 7365 6c66 2e6e 616d          self.nam
+00008f60: 6573 5f75 6e64 6572 6c69 6e65 5f65 7665  es_underline_eve
+00008f70: 6e74 2c0a 2020 2020 2020 2020 2255 6e64  nt,.        "Und
+00008f80: 6572 6c69 6e65 222c 0a20 2020 2020 2020  erline",.       
+00008f90: 2031 332c 0a20 2020 2020 2020 2030 2c0a   13,.        0,.
+00008fa0: 2020 2020 2020 2020 3230 2c0a 2020 2020          20,.    
+00008fb0: 2020 2020 352c 0a20 2020 2020 2020 2022      5,.        "
+00008fc0: 6e77 222c 0a20 2020 2020 2020 2022 222c  nw",.        "",
+00008fd0: 0a20 2020 2029 0a0a 2020 2020 2320 496e  .    )..    # In
+00008fe0: 6465 6e74 6174 696f 6e0a 2020 2020 7365  dentation.    se
+00008ff0: 6c66 2e69 6e64 656e 745f 6c61 6265 6c20  lf.indent_label 
+00009000: 3d20 6164 645f 6c61 6265 6c28 0a20 2020  = add_label(.   
+00009010: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00009020: 2020 2073 656c 662e 7369 6465 6261 725f     self.sidebar_
+00009030: 6672 616d 652c 0a20 2020 2020 2020 2022  frame,.        "
+00009040: 4966 2f54 6865 6e2f 456c 7365 2049 6e64  If/Then/Else Ind
+00009050: 656e 7461 7469 6f6e 2041 6d6f 756e 743a  entation Amount:
+00009060: 222c 0a20 2020 2020 2020 2022 222c 0a20  ",.        "",. 
+00009070: 2020 2020 2020 2030 2c0a 2020 2020 2020         0,.      
+00009080: 2020 226e 6f72 6d61 6c22 2c0a 2020 2020    "normal",.    
+00009090: 2020 2020 3134 2c0a 2020 2020 2020 2020      14,.        
+000090a0: 302c 0a20 2020 2020 2020 2032 302c 0a20  0,.        20,. 
+000090b0: 2020 2020 2020 2031 302c 0a20 2020 2020         10,.     
+000090c0: 2020 2022 7322 2c0a 2020 2020 290a 0a20     "s",.    ).. 
+000090d0: 2020 2023 2049 6e64 656e 7461 7469 6f6e     # Indentation
+000090e0: 2041 6d6f 756e 740a 2020 2020 7365 6c66   Amount.    self
+000090f0: 2e69 6e64 656e 745f 6f70 7469 6f6e 203d  .indent_option =
+00009100: 2061 6464 5f6f 7074 696f 6e5f 6d65 6e75   add_option_menu
+00009110: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00009120: 2020 2020 2020 2020 7365 6c66 2e73 6964          self.sid
+00009130: 6562 6172 5f66 7261 6d65 2c0a 2020 2020  ebar_frame,.    
+00009140: 2020 2020 7365 6c66 2e69 6e64 656e 745f      self.indent_
+00009150: 7365 6c65 6374 6564 5f65 7665 6e74 2c0a  selected_event,.
+00009160: 2020 2020 2020 2020 5b22 3022 2c20 2231          ["0", "1
+00009170: 222c 2022 3222 2c20 2233 222c 2022 3422  ", "2", "3", "4"
+00009180: 2c20 2235 222c 2022 3622 2c20 2237 222c  , "5", "6", "7",
+00009190: 2022 3822 2c20 2239 222c 2022 3130 225d   "8", "9", "10"]
+000091a0: 2c0a 2020 2020 2020 2020 3135 2c0a 2020  ,.        15,.  
+000091b0: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
+000091c0: 2030 2c0a 2020 2020 2020 2020 2830 2c20   0,.        (0, 
+000091d0: 3130 292c 0a20 2020 2020 2020 2022 6e22  10),.        "n"
+000091e0: 2c0a 2020 2020 290a 0a20 2020 2023 2053  ,.    )..    # S
+000091f0: 6372 6565 6e20 4170 7065 6172 616e 6365  creen Appearance
+00009200: 3a20 4c69 6768 7420 2f20 4461 726b 202f  : Light / Dark /
+00009210: 2053 7973 7465 6d0a 2020 2020 7365 6c66   System.    self
+00009220: 2e61 7070 6561 7261 6e63 655f 6d6f 6465  .appearance_mode
+00009230: 5f6c 6162 656c 203d 2061 6464 5f6c 6162  _label = add_lab
+00009240: 656c 280a 2020 2020 2020 2020 7365 6c66  el(.        self
+00009250: 2c0a 2020 2020 2020 2020 7365 6c66 2e73  ,.        self.s
+00009260: 6964 6562 6172 5f66 7261 6d65 2c0a 2020  idebar_frame,.  
+00009270: 2020 2020 2020 2241 7070 6561 7261 6e63        "Appearanc
+00009280: 6520 4d6f 6465 3a22 2c0a 2020 2020 2020  e Mode:",.      
+00009290: 2020 2222 2c0a 2020 2020 2020 2020 302c    "",.        0,
+000092a0: 0a20 2020 2020 2020 2022 6e6f 726d 616c  .        "normal
+000092b0: 222c 0a20 2020 2020 2020 2031 362c 0a20  ",.        16,. 
+000092c0: 2020 2020 2020 2030 2c0a 2020 2020 2020         0,.      
+000092d0: 2020 302c 0a20 2020 2020 2020 2028 3130    0,.        (10
+000092e0: 2c20 3029 2c0a 2020 2020 2020 2020 2273  , 0),.        "s
+000092f0: 222c 0a20 2020 2029 0a0a 2020 2020 7365  ",.    )..    se
+00009300: 6c66 2e61 7070 6561 7261 6e63 655f 6d6f  lf.appearance_mo
+00009310: 6465 5f6f 7074 696f 6e6d 656e 7520 3d20  de_optionmenu = 
+00009320: 6164 645f 6f70 7469 6f6e 5f6d 656e 7528  add_option_menu(
+00009330: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00009340: 2020 2020 2020 2073 656c 662e 7369 6465         self.side
+00009350: 6261 725f 6672 616d 652c 0a20 2020 2020  bar_frame,.     
+00009360: 2020 2073 656c 662e 6368 616e 6765 5f61     self.change_a
+00009370: 7070 6561 7261 6e63 655f 6d6f 6465 5f65  ppearance_mode_e
+00009380: 7665 6e74 2c0a 2020 2020 2020 2020 5b22  vent,.        ["
+00009390: 4c69 6768 7422 2c20 2244 6172 6b22 2c20  Light", "Dark", 
+000093a0: 2253 7973 7465 6d22 5d2c 0a20 2020 2020  "System"],.     
+000093b0: 2020 2031 372c 0a20 2020 2020 2020 2030     17,.        0
+000093c0: 2c0a 2020 2020 2020 2020 302c 0a20 2020  ,.        0,.   
+000093d0: 2020 2020 2028 302c 2031 3029 2c0a 2020       (0, 10),.  
+000093e0: 2020 2020 2020 226e 222c 0a20 2020 2029        "n",.    )
+000093f0: 0a0a 2020 2020 2320 2754 7265 6520 5669  ..    # 'Tree Vi
+00009400: 6577 2720 6275 7474 6f6e 2064 6566 696e  ew' button defin
+00009410: 6974 696f 6e0a 2020 2020 7365 6c66 2e74  ition.    self.t
+00009420: 7265 6576 6965 775f 6275 7474 6f6e 203d  reeview_button =
+00009430: 2061 6464 5f62 7574 746f 6e28 0a20 2020   add_button(.   
+00009440: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00009450: 2020 2073 656c 662e 7369 6465 6261 725f     self.sidebar_
+00009460: 6672 616d 652c 0a20 2020 2020 2020 2022  frame,.        "
+00009470: 2332 3436 4642 3622 2c0a 2020 2020 2020  #246FB6",.      
+00009480: 2020 2222 2c0a 2020 2020 2020 2020 2222    "",.        ""
+00009490: 2c0a 2020 2020 2020 2020 7365 6c66 2e74  ,.        self.t
+000094a0: 7265 6576 6965 775f 6576 656e 742c 0a20  reeview_event,. 
+000094b0: 2020 2020 2020 2032 2c0a 2020 2020 2020         2,.      
+000094c0: 2020 2254 7265 6520 5669 6577 222c 0a20    "Tree View",. 
+000094d0: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
+000094e0: 2020 3138 2c0a 2020 2020 2020 2020 302c    18,.        0,
+000094f0: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
+00009500: 2020 2020 302c 0a20 2020 2020 2020 2022      0,.        "
+00009510: 222c 0a20 2020 2029 0a20 2020 2023 2020  ",.    ).    #  
+00009520: 5175 6572 7920 3f20 6275 7474 6f6e 0a20  Query ? button. 
+00009530: 2020 2073 656c 662e 7472 6565 7669 6577     self.treeview
+00009540: 5f71 7565 7279 5f62 7574 746f 6e20 3d20  _query_button = 
+00009550: 6164 645f 6275 7474 6f6e 280a 2020 2020  add_button(.    
+00009560: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00009570: 2020 7365 6c66 2e73 6964 6562 6172 5f66    self.sidebar_f
+00009580: 7261 6d65 2c0a 2020 2020 2020 2020 2223  rame,.        "#
+00009590: 3234 3646 4236 222c 0a20 2020 2020 2020  246FB6",.       
+000095a0: 2028 2223 3042 4630 3735 222c 2022 2366   ("#0BF075", "#f
+000095b0: 6664 3934 3122 292c 0a20 2020 2020 2020  fd941"),.       
+000095c0: 2022 2331 6263 3966 6622 2c0a 2020 2020   "#1bc9ff",.    
+000095d0: 2020 2020 7365 6c66 2e74 7265 6576 6965      self.treevie
+000095e0: 775f 7175 6572 795f 6576 656e 742c 0a20  w_query_event,. 
+000095f0: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
+00009600: 2020 223f 222c 0a20 2020 2020 2020 2031    "?",.        1
+00009610: 2c0a 2020 2020 2020 2020 3138 2c0a 2020  ,.        18,.  
+00009620: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
+00009630: 2028 3230 302c 2030 292c 0a20 2020 2020   (200, 0),.     
+00009640: 2020 2028 302c 2030 292c 0a20 2020 2020     (0, 0),.     
+00009650: 2020 2022 222c 0a20 2020 2029 0a20 2020     "",.    ).   
+00009660: 2073 656c 662e 7472 6565 7669 6577 5f71   self.treeview_q
+00009670: 7565 7279 5f62 7574 746f 6e2e 636f 6e66  uery_button.conf
+00009680: 6967 7572 6528 7769 6474 683d 3230 290a  igure(width=20).
+00009690: 0a20 2020 2023 2027 5265 7365 7420 5365  .    # 'Reset Se
+000096a0: 7474 696e 6773 2720 6275 7474 6f6e 2064  ttings' button d
+000096b0: 6566 696e 6974 696f 6e0a 2020 2020 7365  efinition.    se
+000096c0: 6c66 2e72 6573 6574 5f62 7574 746f 6e20  lf.reset_button 
+000096d0: 3d20 6164 645f 6275 7474 6f6e 280a 2020  = add_button(.  
+000096e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000096f0: 2020 2020 7365 6c66 2e73 6964 6562 6172      self.sidebar
+00009700: 5f66 7261 6d65 2c0a 2020 2020 2020 2020  _frame,.        
+00009710: 2223 3234 3646 4236 222c 0a20 2020 2020  "#246FB6",.     
+00009720: 2020 2022 222c 0a20 2020 2020 2020 2022     "",.        "
+00009730: 222c 0a20 2020 2020 2020 2073 656c 662e  ",.        self.
+00009740: 7265 7365 745f 7365 7474 696e 6773 5f65  reset_settings_e
+00009750: 7665 6e74 2c0a 2020 2020 2020 2020 322c  vent,.        2,
+00009760: 0a20 2020 2020 2020 2022 5265 7365 7420  .        "Reset 
+00009770: 4f70 7469 6f6e 7322 2c0a 2020 2020 2020  Options",.      
+00009780: 2020 312c 0a20 2020 2020 2020 2031 392c    1,.        19,
+00009790: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
+000097a0: 2020 2020 3230 2c0a 2020 2020 2020 2020      20,.        
+000097b0: 3230 2c0a 2020 2020 2020 2020 2273 222c  20,.        "s",
+000097c0: 0a20 2020 2029 0a0a 2020 2020 2320 5374  .    )..    # St
+000097d0: 6172 7420 7365 636f 6e64 2067 7269 6420  art second grid 
+000097e0: 2f20 636f 6c75 6d6e 2064 6566 696e 6974  / column definit
+000097f0: 696f 6e73 0a0a 2020 2020 2320 466f 6e74  ions..    # Font
+00009800: 2074 6f20 7573 650a 2020 2020 7365 6c66   to use.    self
+00009810: 2e66 6f6e 745f 6c61 6265 6c20 3d20 6164  .font_label = ad
+00009820: 645f 6c61 6265 6c28 7365 6c66 2c20 7365  d_label(self, se
+00009830: 6c66 2c20 2246 6f6e 7420 546f 2055 7365  lf, "Font To Use
+00009840: 2049 6e20 4f75 7470 7574 3a22 2c20 2222   In Output:", ""
+00009850: 2c20 302c 2022 6e6f 726d 616c 222c 2036  , 0, "normal", 6
+00009860: 2c20 312c 2032 302c 2031 302c 2022 7377  , 1, 20, 10, "sw
+00009870: 2229 0a0a 2020 2020 2320 4765 7420 666f  ")..    # Get fo
+00009880: 6e74 7320 6672 6f6d 2054 6b49 6e74 6572  nts from TkInter
+00009890: 0a20 2020 2066 6f6e 745f 6974 656d 732c  .    font_items,
+000098a0: 2072 6573 203d 2067 6574 5f6d 6f6e 6f73   res = get_monos
+000098b0: 7061 6365 5f66 6f6e 7473 2829 0a20 2020  pace_fonts().   
+000098c0: 2023 2044 656c 6574 6520 7468 6520 746b   # Delete the tk
+000098d0: 726f 6f74 206f 6274 6169 6e65 6420 6279  root obtained by
+000098e0: 2067 6574 5f6d 6f6e 6f73 7061 6365 5f66   get_monospace_f
+000098f0: 6f6e 7473 0a20 2020 2069 6620 5072 696d  onts.    if Prim
+00009900: 6549 7465 6d73 2e74 6b72 6f6f 7420 6973  eItems.tkroot is
+00009910: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00009920: 2020 2064 656c 2050 7269 6d65 4974 656d     del PrimeItem
+00009930: 732e 746b 726f 6f74 0a20 2020 2020 2020  s.tkroot.       
+00009940: 2050 7269 6d65 4974 656d 732e 746b 726f   PrimeItems.tkro
+00009950: 6f74 203d 204e 6f6e 650a 2020 2020 7365  ot = None.    se
+00009960: 6c66 2e66 6f6e 745f 6f70 7469 6f6e 6d65  lf.font_optionme
+00009970: 6e75 203d 2061 6464 5f6f 7074 696f 6e5f  nu = add_option_
+00009980: 6d65 6e75 280a 2020 2020 2020 2020 7365  menu(.        se
+00009990: 6c66 2c0a 2020 2020 2020 2020 7365 6c66  lf,.        self
+000099a0: 2c0a 2020 2020 2020 2020 7365 6c66 2e66  ,.        self.f
+000099b0: 6f6e 745f 6576 656e 742c 0a20 2020 2020  ont_event,.     
+000099c0: 2020 2066 6f6e 745f 6974 656d 732c 0a20     font_items,. 
+000099d0: 2020 2020 2020 2037 2c0a 2020 2020 2020         7,.      
+000099e0: 2020 312c 0a20 2020 2020 2020 2032 302c    1,.        20,
+000099f0: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
+00009a00: 2020 2020 226e 7722 2c0a 2020 2020 290a      "nw",.    ).
+00009a10: 2020 2020 7365 6c66 2e66 6f6e 745f 6f70      self.font_op
+00009a20: 7469 6f6e 6d65 6e75 2e73 6574 2872 6573  tionmenu.set(res
+00009a30: 5b30 5d29 0a0a 2020 2020 2320 5361 7665  [0])..    # Save
+00009a40: 2073 6574 7469 6e67 7320 6275 7474 6f6e   settings button
+00009a50: 0a20 2020 2073 656c 662e 7361 7665 5f73  .    self.save_s
+00009a60: 6574 7469 6e67 735f 6275 7474 6f6e 203d  ettings_button =
+00009a70: 2061 6464 5f62 7574 746f 6e28 0a20 2020   add_button(.   
+00009a80: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00009a90: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00009aa0: 2022 2336 3536 3366 6622 2c0a 2020 2020   "#6563ff",.    
+00009ab0: 2020 2020 2222 2c0a 2020 2020 2020 2020      "",.        
+00009ac0: 2222 2c0a 2020 2020 2020 2020 7365 6c66  "",.        self
+00009ad0: 2e73 6176 655f 7365 7474 696e 6773 5f65  .save_settings_e
+00009ae0: 7665 6e74 2c0a 2020 2020 2020 2020 322c  vent,.        2,
+00009af0: 0a20 2020 2020 2020 2022 5361 7665 2053  .        "Save S
+00009b00: 6574 7469 6e67 7322 2c0a 2020 2020 2020  ettings",.      
+00009b10: 2020 312c 0a20 2020 2020 2020 2038 2c0a    1,.        8,.
+00009b20: 2020 2020 2020 2020 312c 0a20 2020 2020          1,.     
+00009b30: 2020 2032 302c 0a20 2020 2020 2020 2030     20,.        0
+00009b40: 2c0a 2020 2020 2020 2020 2273 7722 2c0a  ,.        "sw",.
+00009b50: 2020 2020 290a 0a20 2020 2023 2052 6573      )..    # Res
+00009b60: 746f 7265 2073 6574 7469 6e67 7320 6275  tore settings bu
+00009b70: 7474 6f6e 0a20 2020 2073 656c 662e 7265  tton.    self.re
+00009b80: 7374 6f72 655f 7365 7474 696e 6773 5f62  store_settings_b
+00009b90: 7574 746f 6e20 3d20 6164 645f 6275 7474  utton = add_butt
+00009ba0: 6f6e 280a 2020 2020 2020 2020 7365 6c66  on(.        self
+00009bb0: 2c0a 2020 2020 2020 2020 7365 6c66 2c0a  ,.        self,.
+00009bc0: 2020 2020 2020 2020 2223 3635 3633 6666          "#6563ff
+00009bd0: 222c 0a20 2020 2020 2020 2022 222c 0a20  ",.        "",. 
+00009be0: 2020 2020 2020 2022 222c 0a20 2020 2020         "",.     
+00009bf0: 2020 2073 656c 662e 7265 7374 6f72 655f     self.restore_
+00009c00: 7365 7474 696e 6773 5f65 7665 6e74 2c0a  settings_event,.
+00009c10: 2020 2020 2020 2020 322c 0a20 2020 2020          2,.     
+00009c20: 2020 2022 5265 7374 6f72 6520 5365 7474     "Restore Sett
+00009c30: 696e 6773 222c 0a20 2020 2020 2020 2031  ings",.        1
+00009c40: 2c0a 2020 2020 2020 2020 392c 0a20 2020  ,.        9,.   
+00009c50: 2020 2020 2031 2c0a 2020 2020 2020 2020       1,.        
+00009c60: 3230 2c0a 2020 2020 2020 2020 3130 2c0a  20,.        10,.
+00009c70: 2020 2020 2020 2020 226e 7722 2c0a 2020          "nw",.  
+00009c80: 2020 290a 0a20 2020 2023 2052 6570 6f72    )..    # Repor
+00009c90: 7420 4973 7375 650a 2020 2020 7365 6c66  t Issue.    self
+00009ca0: 2e72 6570 6f72 745f 6973 7375 655f 6275  .report_issue_bu
+00009cb0: 7474 6f6e 203d 2061 6464 5f62 7574 746f  tton = add_butto
+00009cc0: 6e28 0a20 2020 2020 2020 2073 656c 662c  n(.        self,
+00009cd0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00009ce0: 2020 2020 2020 2022 222c 0a20 2020 2020         "",.     
+00009cf0: 2020 2022 222c 0a20 2020 2020 2020 2022     "",.        "
+00009d00: 222c 0a20 2020 2020 2020 2073 656c 662e  ",.        self.
+00009d10: 7265 706f 7274 5f69 7373 7565 5f65 7665  report_issue_eve
+00009d20: 6e74 2c0a 2020 2020 2020 2020 322c 0a20  nt,.        2,. 
+00009d30: 2020 2020 2020 2022 5265 706f 7274 2049         "Report I
+00009d40: 7373 7565 222c 0a20 2020 2020 2020 2031  ssue",.        1
+00009d50: 2c0a 2020 2020 2020 2020 3130 2c0a 2020  ,.        10,.  
+00009d60: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
+00009d70: 2032 302c 0a20 2020 2020 2020 2030 2c0a   20,.        0,.
+00009d80: 2020 2020 2020 2020 226e 7722 2c0a 2020          "nw",.  
+00009d90: 2020 290a 0a20 2020 2023 2027 436c 6561    )..    # 'Clea
+00009da0: 7220 4d65 7373 6167 6573 2720 6275 7474  r Messages' butt
+00009db0: 6f6e 2064 6566 696e 6974 696f 6e0a 2020  on definition.  
+00009dc0: 2020 7365 6c66 2e72 6573 6574 5f62 7574    self.reset_but
+00009dd0: 746f 6e20 3d20 6164 645f 6275 7474 6f6e  ton = add_button
+00009de0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00009df0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00009e00: 2020 2020 2020 2223 3234 3646 4236 222c        "#246FB6",
+00009e10: 0a20 2020 2020 2020 2022 222c 0a20 2020  .        "",.   
+00009e20: 2020 2020 2022 222c 0a20 2020 2020 2020       "",.       
+00009e30: 2073 656c 662e 636c 6561 725f 6d65 7373   self.clear_mess
+00009e40: 6167 6573 5f65 7665 6e74 2c0a 2020 2020  ages_event,.    
+00009e50: 2020 2020 322c 0a20 2020 2020 2020 2022      2,.        "
+00009e60: 436c 6561 7220 4d65 7373 6167 6573 222c  Clear Messages",
+00009e70: 0a20 2020 2020 2020 2031 2c0a 2020 2020  .        1,.    
+00009e80: 2020 2020 352c 0a20 2020 2020 2020 2031      5,.        1
+00009e90: 2c0a 2020 2020 2020 2020 302c 0a20 2020  ,.        0,.   
+00009ea0: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
+00009eb0: 2273 222c 0a20 2020 2029 0a20 2020 2023  "s",.    ).    #
+00009ec0: 2027 4765 7420 4261 636b 7570 2053 6574   'Get Backup Set
+00009ed0: 7469 6e67 7327 2062 7574 746f 6e20 6465  tings' button de
+00009ee0: 6669 6e69 7469 6f6e 0a20 2020 2073 656c  finition.    sel
+00009ef0: 662e 6765 745f 6261 636b 7570 5f62 7574  f.get_backup_but
+00009f00: 746f 6e20 3d20 7365 6c66 2e64 6973 706c  ton = self.displ
+00009f10: 6179 5f62 6163 6b75 705f 6275 7474 6f6e  ay_backup_button
+00009f20: 280a 2020 2020 2020 2020 2247 6574 2058  (.        "Get X
+00009f30: 4d4c 2066 726f 6d20 416e 6472 6f69 6420  ML from Android 
+00009f40: 4465 7669 6365 222c 0a20 2020 2020 2020  Device",.       
+00009f50: 2022 2332 3436 4642 3622 2c0a 2020 2020   "#246FB6",.    
+00009f60: 2020 2020 2223 3635 3633 6666 222c 0a20      "#6563ff",. 
+00009f70: 2020 2020 2020 2073 656c 662e 6765 745f         self.get_
+00009f80: 6261 636b 7570 5f65 7665 6e74 2c0a 2020  backup_event,.  
+00009f90: 2020 290a 2020 2020 2320 2747 6574 206c    ).    # 'Get l
+00009fa0: 6f63 616c 2058 4d4c 2720 6275 7474 6f6e  ocal XML' button
+00009fb0: 0a20 2020 2073 656c 662e 6765 7478 6d6c  .    self.getxml
+00009fc0: 5f62 7574 746f 6e20 3d20 6164 645f 6275  _button = add_bu
+00009fd0: 7474 6f6e 280a 2020 2020 2020 2020 7365  tton(.        se
+00009fe0: 6c66 2c0a 2020 2020 2020 2020 7365 6c66  lf,.        self
+00009ff0: 2c0a 2020 2020 2020 2020 2222 2c0a 2020  ,.        "",.  
+0000a000: 2020 2020 2020 2222 2c0a 2020 2020 2020        "",.      
+0000a010: 2020 2222 2c0a 2020 2020 2020 2020 7365    "",.        se
+0000a020: 6c66 2e67 6574 786d 6c5f 6576 656e 742c  lf.getxml_event,
+0000a030: 0a20 2020 2020 2020 2032 2c0a 2020 2020  .        2,.    
+0000a040: 2020 2020 2247 6574 204c 6f63 616c 2058      "Get Local X
+0000a050: 4d4c 222c 0a20 2020 2020 2020 2031 2c0a  ML",.        1,.
+0000a060: 2020 2020 2020 2020 362c 0a20 2020 2020          6,.     
+0000a070: 2020 2032 2c0a 2020 2020 2020 2020 2832     2,.        (2
+0000a080: 302c 2032 3029 2c0a 2020 2020 2020 2020  0, 20),.        
+0000a090: 2831 302c 2031 3029 2c0a 2020 2020 2020  (10, 10),.      
+0000a0a0: 2020 2265 222c 0a20 2020 2029 0a0a 2020    "e",.    )..  
+0000a0b0: 2020 2320 2744 6973 706c 6179 2048 656c    # 'Display Hel
+0000a0c0: 7027 2062 7574 746f 6e20 6465 6669 6e69  p' button defini
+0000a0d0: 7469 6f6e 0a20 2020 2073 656c 662e 6865  tion.    self.he
+0000a0e0: 6c70 5f62 7574 746f 6e20 3d20 6164 645f  lp_button = add_
+0000a0f0: 6275 7474 6f6e 280a 2020 2020 2020 2020  button(.        
+0000a100: 7365 6c66 2c0a 2020 2020 2020 2020 7365  self,.        se
+0000a110: 6c66 2c0a 2020 2020 2020 2020 2223 3234  lf,.        "#24
+0000a120: 3646 4236 222c 0a20 2020 2020 2020 2028  6FB6",.        (
+0000a130: 2223 3042 4630 3735 222c 2022 2366 6664  "#0BF075", "#ffd
+0000a140: 3934 3122 292c 0a20 2020 2020 2020 2022  941"),.        "
+0000a150: 222c 0a20 2020 2020 2020 2073 656c 662e  ",.        self.
+0000a160: 6865 6c70 5f65 7665 6e74 2c0a 2020 2020  help_event,.    
+0000a170: 2020 2020 322c 0a20 2020 2020 2020 2022      2,.        "
+0000a180: 4469 7370 6c61 7920 4865 6c70 222c 0a20  Display Help",. 
+0000a190: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
+0000a1a0: 2020 372c 0a20 2020 2020 2020 2032 2c0a    7,.        2,.
+0000a1b0: 2020 2020 2020 2020 2830 2c20 3230 292c          (0, 20),
+0000a1c0: 0a20 2020 2020 2020 2028 3130 2c20 3529  .        (10, 5)
+0000a1d0: 2c0a 2020 2020 2020 2020 2273 6522 2c0a  ,.        "se",.
+0000a1e0: 2020 2020 290a 0a20 2020 2023 2027 4261      )..    # 'Ba
+0000a1f0: 636b 7570 2048 656c 7027 2062 7574 746f  ckup Help' butto
+0000a200: 6e20 6465 6669 6e69 7469 6f6e 0a20 2020  n definition.   
+0000a210: 2073 656c 662e 6261 636b 7570 5f68 656c   self.backup_hel
+0000a220: 705f 6275 7474 6f6e 203d 2061 6464 5f62  p_button = add_b
+0000a230: 7574 746f 6e28 0a20 2020 2020 2020 2073  utton(.        s
+0000a240: 656c 662c 0a20 2020 2020 2020 2073 656c  elf,.        sel
+0000a250: 662c 0a20 2020 2020 2020 2022 2332 3436  f,.        "#246
+0000a260: 4642 3622 2c0a 2020 2020 2020 2020 2822  FB6",.        ("
+0000a270: 2330 4246 3037 3522 2c20 2223 6666 6439  #0BF075", "#ffd9
+0000a280: 3431 2229 2c0a 2020 2020 2020 2020 2222  41"),.        ""
+0000a290: 2c0a 2020 2020 2020 2020 7365 6c66 2e62  ,.        self.b
+0000a2a0: 6163 6b75 705f 6865 6c70 5f65 7665 6e74  ackup_help_event
+0000a2b0: 2c0a 2020 2020 2020 2020 322c 0a20 2020  ,.        2,.   
+0000a2c0: 2020 2020 2022 4765 7420 416e 6472 6f69       "Get Androi
+0000a2d0: 6420 4865 6c70 222c 0a20 2020 2020 2020  d Help",.       
+0000a2e0: 2031 2c0a 2020 2020 2020 2020 382c 0a20   1,.        8,. 
+0000a2f0: 2020 2020 2020 2032 2c0a 2020 2020 2020         2,.      
+0000a300: 2020 2830 2c20 3230 292c 0a20 2020 2020    (0, 20),.     
+0000a310: 2020 2028 352c 2031 3029 2c0a 2020 2020     (5, 10),.    
+0000a320: 2020 2020 226e 6522 2c0a 2020 2020 290a      "ne",.    ).
+0000a330: 0a20 2020 2023 2027 5275 6e27 2062 7574  .    # 'Run' but
+0000a340: 746f 6e20 6465 6669 6e69 7469 6f6e 0a20  ton definition. 
+0000a350: 2020 2073 656c 662e 7275 6e5f 6275 7474     self.run_butt
+0000a360: 6f6e 203d 2061 6464 5f62 7574 746f 6e28  on = add_button(
+0000a370: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000a380: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000a390: 2020 2020 2022 2332 3436 4642 3622 2c0a       "#246FB6",.
+0000a3a0: 2020 2020 2020 2020 2822 2330 4246 3037          ("#0BF07
+0000a3b0: 3522 2c20 2223 3141 4436 3344 2229 2c0a  5", "#1AD63D"),.
+0000a3c0: 2020 2020 2020 2020 2222 2c0a 2020 2020          "",.    
+0000a3d0: 2020 2020 7365 6c66 2e72 756e 5f70 726f      self.run_pro
+0000a3e0: 6772 616d 2c0a 2020 2020 2020 2020 322c  gram,.        2,
+0000a3f0: 0a20 2020 2020 2020 2022 5275 6e20 616e  .        "Run an
+0000a400: 6420 4578 6974 222c 0a20 2020 2020 2020  d Exit",.       
+0000a410: 2031 2c0a 2020 2020 2020 2020 392c 0a20   1,.        9,. 
+0000a420: 2020 2020 2020 2032 2c0a 2020 2020 2020         2,.      
+0000a430: 2020 2830 2c20 3230 292c 0a20 2020 2020    (0, 20),.     
+0000a440: 2020 2028 3130 2c20 3529 2c0a 2020 2020     (10, 5),.    
+0000a450: 2020 2020 2273 6522 2c0a 2020 2020 290a      "se",.    ).
+0000a460: 0a20 2020 2023 2027 5265 5275 6e27 2062  .    # 'ReRun' b
+0000a470: 7574 746f 6e20 6465 6669 6e69 7469 6f6e  utton definition
+0000a480: 0a20 2020 2073 656c 662e 7265 7275 6e5f  .    self.rerun_
+0000a490: 6275 7474 6f6e 203d 2061 6464 5f62 7574  button = add_but
+0000a4a0: 746f 6e28 0a20 2020 2020 2020 2073 656c  ton(.        sel
+0000a4b0: 662c 0a20 2020 2020 2020 2073 656c 662c  f,.        self,
+0000a4c0: 0a20 2020 2020 2020 2022 2332 3436 4642  .        "#246FB
+0000a4d0: 3622 2c0a 2020 2020 2020 2020 2822 2330  6",.        ("#0
+0000a4e0: 4246 3037 3522 2c20 2223 3141 4436 3344  BF075", "#1AD63D
+0000a4f0: 2229 2c0a 2020 2020 2020 2020 2222 2c0a  "),.        "",.
+0000a500: 2020 2020 2020 2020 7365 6c66 2e72 6572          self.rer
+0000a510: 756e 5f74 6865 5f70 726f 6772 616d 2c0a  un_the_program,.
+0000a520: 2020 2020 2020 2020 322c 0a20 2020 2020          2,.     
+0000a530: 2020 2022 5265 5275 6e22 2c0a 2020 2020     "ReRun",.    
+0000a540: 2020 2020 312c 0a20 2020 2020 2020 2031      1,.        1
+0000a550: 302c 0a20 2020 2020 2020 2032 2c0a 2020  0,.        2,.  
+0000a560: 2020 2020 2020 2830 2c20 3230 292c 0a20        (0, 20),. 
+0000a570: 2020 2020 2020 2028 352c 2031 3029 2c0a         (5, 10),.
+0000a580: 2020 2020 2020 2020 226e 6522 2c0a 2020          "ne",.  
+0000a590: 2020 290a 0a20 2020 2023 2027 4578 6974    )..    # 'Exit
+0000a5a0: 2720 6275 7474 6f6e 2064 6566 696e 6974  ' button definit
+0000a5b0: 696f 6e0a 2020 2020 7365 6c66 2e65 7869  ion.    self.exi
+0000a5c0: 745f 6275 7474 6f6e 203d 2061 6464 5f62  t_button = add_b
+0000a5d0: 7574 746f 6e28 0a20 2020 2020 2020 2073  utton(.        s
+0000a5e0: 656c 662c 0a20 2020 2020 2020 2073 656c  elf,.        sel
+0000a5f0: 662c 0a20 2020 2020 2020 2022 2332 3436  f,.        "#246
+0000a600: 4642 3622 2c0a 2020 2020 2020 2020 2252  FB6",.        "R
+0000a610: 6564 222c 0a20 2020 2020 2020 2022 222c  ed",.        "",
+0000a620: 0a20 2020 2020 2020 2073 656c 662e 6578  .        self.ex
+0000a630: 6974 5f70 726f 6772 616d 2c0a 2020 2020  it_program,.    
+0000a640: 2020 2020 322c 0a20 2020 2020 2020 2022      2,.        "
+0000a650: 4578 6974 222c 0a20 2020 2020 2020 2031  Exit",.        1
+0000a660: 2c0a 2020 2020 2020 2020 3131 2c0a 2020  ,.        11,.  
+0000a670: 2020 2020 2020 322c 0a20 2020 2020 2020        2,.       
+0000a680: 2028 3230 2c20 3230 292c 0a20 2020 2020   (20, 20),.     
+0000a690: 2020 2028 3230 2c20 3230 292c 0a20 2020     (20, 20),.   
+0000a6a0: 2020 2020 2022 6e65 222c 0a20 2020 2029       "ne",.    )
+0000a6b0: 0a0a 2020 2020 2320 4372 6561 7465 2074  ..    # Create t
+0000a6c0: 6578 7462 6f78 2066 6f72 2048 656c 7020  extbox for Help 
+0000a6d0: 696e 666f 726d 6174 696f 6e0a 2020 2020  information.    
+0000a6e0: 7365 6c66 2e74 6578 7462 6f78 203d 2063  self.textbox = c
+0000a6f0: 746b 2e43 546b 5465 7874 626f 7828 7365  tk.CTkTextbox(se
+0000a700: 6c66 2c20 6865 6967 6874 3d36 3030 2c20  lf, height=600, 
+0000a710: 7769 6474 683d 3235 3029 0a20 2020 2073  width=250).    s
+0000a720: 656c 662e 7465 7874 626f 782e 636f 6e66  elf.textbox.conf
+0000a730: 6967 7572 6528 7363 726f 6c6c 6261 725f  igure(scrollbar_
+0000a740: 6275 7474 6f6e 5f63 6f6c 6f72 3d22 2336  button_color="#6
+0000a750: 3536 3366 6622 2c20 7772 6170 3d22 776f  563ff", wrap="wo
+0000a760: 7264 2229 0a20 2020 2073 656c 662e 7465  rd").    self.te
+0000a770: 7874 626f 782e 6772 6964 2872 6f77 3d30  xtbox.grid(row=0
+0000a780: 2c20 636f 6c75 6d6e 3d31 2c20 7061 6478  , column=1, padx
+0000a790: 3d28 3230 2c20 3029 2c20 7061 6479 3d28  =(20, 0), pady=(
+0000a7a0: 3230 2c20 3029 2c20 7374 6963 6b79 3d22  20, 0), sticky="
+0000a7b0: 6577 2229 0a0a 2020 2020 2320 5374 6172  ew")..    # Star
+0000a7c0: 7420 7468 6972 6420 6772 6964 202f 2063  t third grid / c
+0000a7d0: 6f6c 756d 6e20 6465 6669 6e69 7469 6f6e  olumn definition
+0000a7e0: 730a 2020 2020 2320 6372 6561 7465 2074  s.    # create t
+0000a7f0: 6162 7669 6577 2066 6f72 204e 616d 652c  abview for Name,
+0000a800: 2043 6f6c 6f72 2c20 616e 6420 4465 6275   Color, and Debu
+0000a810: 670a 2020 2020 7365 6c66 2e74 6162 7669  g.    self.tabvi
+0000a820: 6577 203d 2063 746b 2e43 546b 5461 6276  ew = ctk.CTkTabv
+0000a830: 6965 7728 7365 6c66 2c20 7769 6474 683d  iew(self, width=
+0000a840: 3235 302c 2073 6567 6d65 6e74 6564 5f62  250, segmented_b
+0000a850: 7574 746f 6e5f 6667 5f63 6f6c 6f72 3d22  utton_fg_color="
+0000a860: 2336 3536 3366 6622 290a 2020 2020 7365  #6563ff").    se
+0000a870: 6c66 2e74 6162 7669 6577 2e67 7269 6428  lf.tabview.grid(
+0000a880: 726f 773d 302c 2063 6f6c 756d 6e3d 322c  row=0, column=2,
+0000a890: 2070 6164 783d 2832 302c 2030 292c 2070   padx=(20, 0), p
+0000a8a0: 6164 793d 2832 302c 2030 292c 2073 7469  ady=(20, 0), sti
+0000a8b0: 636b 793d 226e 7365 7722 290a 2020 2020  cky="nsew").    
+0000a8c0: 7365 6c66 2e74 6162 7669 6577 2e61 6464  self.tabview.add
+0000a8d0: 2822 5370 6563 6966 6963 204e 616d 6522  ("Specific Name"
+0000a8e0: 290a 2020 2020 7365 6c66 2e74 6162 7669  ).    self.tabvi
+0000a8f0: 6577 2e61 6464 2822 436f 6c6f 7273 2229  ew.add("Colors")
+0000a900: 0a20 2020 2073 656c 662e 7461 6276 6965  .    self.tabvie
+0000a910: 772e 6164 6428 2241 6e61 6c79 7a65 2229  w.add("Analyze")
+0000a920: 0a20 2020 2073 656c 662e 7461 6276 6965  .    self.tabvie
+0000a930: 772e 6164 6428 2244 6562 7567 2229 0a0a  w.add("Debug")..
+0000a940: 2020 2020 7365 6c66 2e74 6162 7669 6577      self.tabview
+0000a950: 2e74 6162 2822 5370 6563 6966 6963 204e  .tab("Specific N
+0000a960: 616d 6522 292e 6772 6964 5f63 6f6c 756d  ame").grid_colum
+0000a970: 6e63 6f6e 6669 6775 7265 2830 2c20 7765  nconfigure(0, we
+0000a980: 6967 6874 3d31 2920 2023 2063 6f6e 6669  ight=1)  # confi
+0000a990: 6775 7265 2067 7269 6420 6f66 2069 6e64  gure grid of ind
+0000a9a0: 6976 6964 7561 6c20 7461 6273 0a20 2020  ividual tabs.   
+0000a9b0: 2073 656c 662e 7461 6276 6965 772e 7461   self.tabview.ta
+0000a9c0: 6228 2243 6f6c 6f72 7322 292e 6772 6964  b("Colors").grid
+0000a9d0: 5f63 6f6c 756d 6e63 6f6e 6669 6775 7265  _columnconfigure
+0000a9e0: 2830 2c20 7765 6967 6874 3d31 290a 2020  (0, weight=1).  
+0000a9f0: 2020 7365 6c66 2e74 6162 7669 6577 2e74    self.tabview.t
+0000aa00: 6162 2822 416e 616c 797a 6522 292e 6772  ab("Analyze").gr
+0000aa10: 6964 5f63 6f6c 756d 6e63 6f6e 6669 6775  id_columnconfigu
+0000aa20: 7265 2830 2c20 7765 6967 6874 3d31 290a  re(0, weight=1).
+0000aa30: 0a20 2020 2023 2050 726f 6d70 7420 666f  .    # Prompt fo
+0000aa40: 7220 7468 6520 6e61 6d65 0a20 2020 2073  r the name.    s
+0000aa50: 656c 662e 6e61 6d65 5f6c 6162 656c 203d  elf.name_label =
+0000aa60: 2061 6464 5f6c 6162 656c 280a 2020 2020   add_label(.    
+0000aa70: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000aa80: 2020 7365 6c66 2e74 6162 7669 6577 2e74    self.tabview.t
+0000aa90: 6162 2822 5370 6563 6966 6963 204e 616d  ab("Specific Nam
+0000aaa0: 6522 292c 0a20 2020 2020 2020 2022 2850  e"),.        "(P
+0000aab0: 6963 6b20 4f4e 4c59 204f 6e65 2922 2c0a  ick ONLY One)",.
+0000aac0: 2020 2020 2020 2020 2222 2c0a 2020 2020          "",.    
+0000aad0: 2020 2020 302c 0a20 2020 2020 2020 2022      0,.        "
+0000aae0: 6e6f 726d 616c 222c 0a20 2020 2020 2020  normal",.       
+0000aaf0: 2034 2c0a 2020 2020 2020 2020 302c 0a20   4,.        0,. 
+0000ab00: 2020 2020 2020 2032 302c 0a20 2020 2020         20,.     
+0000ab10: 2020 2028 3130 2c20 3130 292c 0a20 2020     (10, 10),.   
+0000ab20: 2020 2020 2022 7722 2c0a 2020 2020 290a       "w",.    ).
+0000ab30: 0a20 2020 2023 2053 6574 7570 2074 6f20  .    # Setup to 
+0000ab40: 6765 7420 7661 7269 6f75 7320 6469 7370  get various disp
+0000ab50: 6c61 7920 636f 6c6f 7273 0a20 2020 2073  lay colors.    s
+0000ab60: 656c 662e 6c61 6265 6c5f 7461 625f 3220  elf.label_tab_2 
+0000ab70: 3d20 6164 645f 6c61 6265 6c28 0a20 2020  = add_label(.   
+0000ab80: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000ab90: 2020 2073 656c 662e 7461 6276 6965 772e     self.tabview.
+0000aba0: 7461 6228 2243 6f6c 6f72 7322 292c 0a20  tab("Colors"),. 
+0000abb0: 2020 2020 2020 2022 5365 7420 5661 7269         "Set Vari
+0000abc0: 6f75 7320 4469 7370 6c61 7920 436f 6c6f  ous Display Colo
+0000abd0: 7273 2048 6572 653a 222c 0a20 2020 2020  rs Here:",.     
+0000abe0: 2020 2022 222c 0a20 2020 2020 2020 2030     "",.        0
+0000abf0: 2c0a 2020 2020 2020 2020 226e 6f72 6d61  ,.        "norma
+0000ac00: 6c22 2c0a 2020 2020 2020 2020 302c 0a20  l",.        0,. 
+0000ac10: 2020 2020 2020 2030 2c0a 2020 2020 2020         0,.      
+0000ac20: 2020 302c 0a20 2020 2020 2020 2030 2c0a    0,.        0,.
+0000ac30: 2020 2020 2020 2020 2222 2c0a 2020 2020          "",.    
+0000ac40: 290a 2020 2020 7365 6c66 2e63 6f6c 6f72  ).    self.color
+0000ac50: 735f 6f70 7469 6f6e 6d65 6e75 203d 2061  s_optionmenu = a
+0000ac60: 6464 5f6f 7074 696f 6e5f 6d65 6e75 280a  dd_option_menu(.
+0000ac70: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000ac80: 2020 2020 2020 7365 6c66 2e74 6162 7669        self.tabvi
+0000ac90: 6577 2e74 6162 2822 436f 6c6f 7273 2229  ew.tab("Colors")
+0000aca0: 2c0a 2020 2020 2020 2020 7365 6c66 2e63  ,.        self.c
+0000acb0: 6f6c 6f72 735f 6576 656e 742c 0a20 2020  olors_event,.   
+0000acc0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+0000acd0: 2020 2022 5072 6f6a 6563 7473 222c 0a20     "Projects",. 
+0000ace0: 2020 2020 2020 2020 2020 2022 5072 6f66             "Prof
+0000acf0: 696c 6573 222c 0a20 2020 2020 2020 2020  iles",.         
+0000ad00: 2020 2022 4469 7361 626c 6564 2050 726f     "Disabled Pro
+0000ad10: 6669 6c65 7322 2c0a 2020 2020 2020 2020  files",.        
+0000ad20: 2020 2020 224c 6175 6e63 6865 7220 5461      "Launcher Ta
+0000ad30: 736b 222c 0a20 2020 2020 2020 2020 2020  sk",.           
+0000ad40: 2022 5072 6f66 696c 6520 436f 6e64 6974   "Profile Condit
+0000ad50: 696f 6e73 222c 0a20 2020 2020 2020 2020  ions",.         
+0000ad60: 2020 2022 5461 736b 7322 2c0a 2020 2020     "Tasks",.    
+0000ad70: 2020 2020 2020 2020 2228 5461 736b 2920          "(Task) 
+0000ad80: 4163 7469 6f6e 7322 2c0a 2020 2020 2020  Actions",.      
+0000ad90: 2020 2020 2020 2241 6374 696f 6e20 436f        "Action Co
+0000ada0: 6e64 6974 696f 6e73 222c 0a20 2020 2020  nditions",.     
+0000adb0: 2020 2020 2020 2022 4163 7469 6f6e 204c         "Action L
+0000adc0: 6162 656c 7322 2c0a 2020 2020 2020 2020  abels",.        
+0000add0: 2020 2020 2241 6374 696f 6e20 4e61 6d65      "Action Name
+0000ade0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+0000adf0: 2253 6365 6e65 7322 2c0a 2020 2020 2020  "Scenes",.      
+0000ae00: 2020 2020 2020 2242 6163 6b67 726f 756e        "Backgroun
+0000ae10: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+0000ae20: 2254 6173 6b65 724e 6574 2049 6e66 6f72  "TaskerNet Infor
+0000ae30: 6d61 7469 6f6e 222c 0a20 2020 2020 2020  mation",.       
+0000ae40: 2020 2020 2022 5461 736b 6572 2050 7265       "Tasker Pre
+0000ae50: 6665 7265 6e63 6573 222c 0a20 2020 2020  ferences",.     
+0000ae60: 2020 2020 2020 2022 4869 6768 6c69 6768         "Highligh
+0000ae70: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+0000ae80: 2248 6561 6469 6e67 222c 0a20 2020 2020  "Heading",.     
+0000ae90: 2020 205d 2c0a 2020 2020 2020 2020 312c     ],.        1,
+0000aea0: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
+0000aeb0: 2020 2020 3230 2c0a 2020 2020 2020 2020      20,.        
+0000aec0: 2831 302c 2031 3029 2c0a 2020 2020 2020  (10, 10),.      
+0000aed0: 2020 2222 2c0a 2020 2020 290a 0a20 2020    "",.    )..   
+0000aee0: 2023 2052 6573 6574 2074 6f20 4465 6661   # Reset to Defa
+0000aef0: 756c 7420 436f 6c6f 7273 2062 7574 746f  ult Colors butto
+0000af00: 6e0a 2020 2020 7365 6c66 2e63 6f6c 6f72  n.    self.color
+0000af10: 5f72 6573 6574 5f62 7574 746f 6e20 3d20  _reset_button = 
+0000af20: 6164 645f 6275 7474 6f6e 280a 2020 2020  add_button(.    
+0000af30: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000af40: 2020 7365 6c66 2e74 6162 7669 6577 2e74    self.tabview.t
+0000af50: 6162 2822 436f 6c6f 7273 2229 2c0a 2020  ab("Colors"),.  
+0000af60: 2020 2020 2020 2222 2c0a 2020 2020 2020        "",.      
+0000af70: 2020 2222 2c0a 2020 2020 2020 2020 2222    "",.        ""
+0000af80: 2c0a 2020 2020 2020 2020 7365 6c66 2e63  ,.        self.c
+0000af90: 6f6c 6f72 5f72 6573 6574 5f65 7665 6e74  olor_reset_event
+0000afa0: 2c0a 2020 2020 2020 2020 322c 0a20 2020  ,.        2,.   
+0000afb0: 2020 2020 2022 5265 7365 7420 746f 2044       "Reset to D
+0000afc0: 6566 6175 6c74 2043 6f6c 6f72 7322 2c0a  efault Colors",.
+0000afd0: 2020 2020 2020 2020 312c 0a20 2020 2020          1,.     
+0000afe0: 2020 2033 2c0a 2020 2020 2020 2020 302c     3,.        0,
+0000aff0: 0a20 2020 2020 2020 2032 302c 0a20 2020  .        20,.   
+0000b000: 2020 2020 2028 3130 2c20 3130 292c 0a20       (10, 10),. 
+0000b010: 2020 2020 2020 2022 222c 0a20 2020 2029         "",.    )
+0000b020: 0a0a 2020 2020 2320 4149 2054 6162 2066  ..    # AI Tab f
+0000b030: 6965 6c64 730a 2020 2020 6365 6e74 6572  ields.    center
+0000b040: 203d 2035 300a 2020 2020 2320 4150 4920   = 50.    # API 
+0000b050: 4b65 790a 2020 2020 7365 6c66 2e61 695f  Key.    self.ai_
+0000b060: 6170 696b 6579 5f62 7574 746f 6e20 3d20  apikey_button = 
+0000b070: 6164 645f 6275 7474 6f6e 280a 2020 2020  add_button(.    
+0000b080: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000b090: 2020 7365 6c66 2e74 6162 7669 6577 2e74    self.tabview.t
+0000b0a0: 6162 2822 416e 616c 797a 6522 292c 0a20  ab("Analyze"),. 
+0000b0b0: 2020 2020 2020 2022 222c 2020 2320 6667         "",  # fg
+0000b0c0: 5f63 6f6c 6f72 3a20 7374 722c 0a20 2020  _color: str,.   
+0000b0d0: 2020 2020 2022 222c 2020 2320 7465 7874       "",  # text
+0000b0e0: 5f63 6f6c 6f72 3a20 7374 722c 0a20 2020  _color: str,.   
+0000b0f0: 2020 2020 2022 222c 2020 2320 626f 7264       "",  # bord
+0000b100: 6572 5f63 6f6c 6f72 3a20 7374 722c 0a20  er_color: str,. 
+0000b110: 2020 2020 2020 2073 656c 662e 6169 5f61         self.ai_a
+0000b120: 7069 6b65 795f 6576 656e 742c 2020 2320  pikey_event,  # 
+0000b130: 636f 6d6d 616e 640a 2020 2020 2020 2020  command.        
+0000b140: 322c 2020 2320 626f 7264 6572 5f77 6964  2,  # border_wid
+0000b150: 7468 3a20 696e 742c 0a20 2020 2020 2020  th: int,.       
+0000b160: 2022 5368 6f77 2f45 6469 7420 4f70 656e   "Show/Edit Open
+0000b170: 4149 2041 5049 204b 6579 222c 2020 2320  AI API Key",  # 
+0000b180: 7465 7874 3a20 7374 722c 0a20 2020 2020  text: str,.     
+0000b190: 2020 2031 2c20 2023 2063 6f6c 756d 6e73     1,  # columns
+0000b1a0: 7061 6e3a 2069 6e74 2c0a 2020 2020 2020  pan: int,.      
+0000b1b0: 2020 332c 2020 2320 726f 773a 2069 6e74    3,  # row: int
+0000b1c0: 2c0a 2020 2020 2020 2020 302c 2020 2320  ,.        0,  # 
+0000b1d0: 636f 6c75 6d6e 3a20 696e 742c 0a20 2020  column: int,.   
+0000b1e0: 2020 2020 2063 656e 7465 722c 2020 2320       center,  # 
+0000b1f0: 7061 6478 3a20 7475 706c 652c 0a20 2020  padx: tuple,.   
+0000b200: 2020 2020 2028 3130 2c20 3130 292c 2020       (10, 10),  
+0000b210: 2320 7061 6479 3a20 7475 706c 652c 0a20  # pady: tuple,. 
+0000b220: 2020 2020 2020 2022 222c 0a20 2020 2029         "",.    )
+0000b230: 0a20 2020 2023 2043 6861 6e67 6520 5072  .    # Change Pr
+0000b240: 6f6d 7074 0a20 2020 2073 656c 662e 6169  ompt.    self.ai
+0000b250: 5f61 7069 6b65 795f 6275 7474 6f6e 203d  _apikey_button =
+0000b260: 2061 6464 5f62 7574 746f 6e28 0a20 2020   add_button(.   
+0000b270: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000b280: 2020 2073 656c 662e 7461 6276 6965 772e     self.tabview.
+0000b290: 7461 6228 2241 6e61 6c79 7a65 2229 2c0a  tab("Analyze"),.
+0000b2a0: 2020 2020 2020 2020 2222 2c20 2023 2066          "",  # f
+0000b2b0: 675f 636f 6c6f 723a 2073 7472 2c0a 2020  g_color: str,.  
+0000b2c0: 2020 2020 2020 2222 2c20 2023 2074 6578        "",  # tex
+0000b2d0: 745f 636f 6c6f 723a 2073 7472 2c0a 2020  t_color: str,.  
+0000b2e0: 2020 2020 2020 2222 2c20 2023 2062 6f72        "",  # bor
+0000b2f0: 6465 725f 636f 6c6f 723a 2073 7472 2c0a  der_color: str,.
+0000b300: 2020 2020 2020 2020 7365 6c66 2e61 695f          self.ai_
+0000b310: 7072 6f6d 7074 5f65 7665 6e74 2c20 2023  prompt_event,  #
+0000b320: 2063 6f6d 6d61 6e64 0a20 2020 2020 2020   command.       
+0000b330: 2032 2c20 2023 2062 6f72 6465 725f 7769   2,  # border_wi
+0000b340: 6474 683a 2069 6e74 2c0a 2020 2020 2020  dth: int,.      
+0000b350: 2020 2243 6861 6e67 6520 5072 6f6d 7074    "Change Prompt
+0000b360: 222c 2020 2320 7465 7874 3a20 7374 722c  ",  # text: str,
+0000b370: 0a20 2020 2020 2020 2031 2c20 2023 2063  .        1,  # c
+0000b380: 6f6c 756d 6e73 7061 6e3a 2069 6e74 2c0a  olumnspan: int,.
+0000b390: 2020 2020 2020 2020 342c 2020 2320 726f          4,  # ro
+0000b3a0: 773a 2069 6e74 2c0a 2020 2020 2020 2020  w: int,.        
+0000b3b0: 302c 2020 2320 636f 6c75 6d6e 3a20 696e  0,  # column: in
+0000b3c0: 742c 0a20 2020 2020 2020 2063 656e 7465  t,.        cente
+0000b3d0: 722c 2020 2320 7061 6478 3a20 7475 706c  r,  # padx: tupl
+0000b3e0: 652c 0a20 2020 2020 2020 2028 3130 2c20  e,.        (10, 
+0000b3f0: 3130 292c 2020 2320 7061 6479 3a20 7475  10),  # pady: tu
+0000b400: 706c 652c 0a20 2020 2020 2020 2022 222c  ple,.        "",
+0000b410: 0a20 2020 2029 0a20 2020 2023 204d 6f64  .    ).    # Mod
+0000b420: 656c 2073 656c 6563 7469 6f6e 0a20 2020  el selection.   
+0000b430: 2073 656c 662e 6169 5f6d 6f64 656c 5f6c   self.ai_model_l
+0000b440: 6162 656c 203d 2061 6464 5f6c 6162 656c  abel = add_label
+0000b450: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000b460: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+0000b470: 7669 6577 2e74 6162 2822 416e 616c 797a  view.tab("Analyz
+0000b480: 6522 292c 0a20 2020 2020 2020 2022 4d6f  e"),.        "Mo
+0000b490: 6465 6c20 746f 2055 7365 3a22 2c0a 2020  del to Use:",.  
+0000b4a0: 2020 2020 2020 2222 2c0a 2020 2020 2020        "",.      
+0000b4b0: 2020 302c 0a20 2020 2020 2020 2022 6e6f    0,.        "no
+0000b4c0: 726d 616c 222c 0a20 2020 2020 2020 2036  rmal",.        6
+0000b4d0: 2c0a 2020 2020 2020 2020 302c 0a20 2020  ,.        0,.   
+0000b4e0: 2020 2020 2063 656e 7465 722c 0a20 2020       center,.   
+0000b4f0: 2020 2020 2028 302c 2030 292c 0a20 2020       (0, 0),.   
+0000b500: 2020 2020 2022 6e22 2c0a 2020 2020 290a       "n",.    ).
+0000b510: 2020 2020 6469 7370 6c61 795f 6d6f 6465      display_mode
+0000b520: 6c73 203d 205b 224e 6f6e 6520 286c 6c61  ls = ["None (lla
+0000b530: 6d61 3329 222c 202a 4f50 454e 4149 5f4d  ma3)", *OPENAI_M
+0000b540: 4f44 454c 532c 202a 4c4c 414d 415f 4d4f  ODELS, *LLAMA_MO
+0000b550: 4445 4c53 5d20 2023 2043 6f6d 6269 6e65  DELS]  # Combine
+0000b560: 206c 6973 7473 0a20 2020 2073 656c 662e   lists.    self.
+0000b570: 6169 5f6d 6f64 656c 5f6f 7074 696f 6e20  ai_model_option 
+0000b580: 3d20 6164 645f 6f70 7469 6f6e 5f6d 656e  = add_option_men
+0000b590: 7528 0a20 2020 2020 2020 2073 656c 662c  u(.        self,
+0000b5a0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+0000b5b0: 6276 6965 772e 7461 6228 2241 6e61 6c79  bview.tab("Analy
+0000b5c0: 7a65 2229 2c0a 2020 2020 2020 2020 7365  ze"),.        se
+0000b5d0: 6c66 2e61 695f 6d6f 6465 6c5f 7365 6c65  lf.ai_model_sele
+0000b5e0: 6374 6564 5f65 7665 6e74 2c0a 2020 2020  cted_event,.    
+0000b5f0: 2020 2020 6469 7370 6c61 795f 6d6f 6465      display_mode
+0000b600: 6c73 2c0a 2020 2020 2020 2020 362c 0a20  ls,.        6,. 
+0000b610: 2020 2020 2020 2030 2c0a 2020 2020 2020         0,.      
+0000b620: 2020 6365 6e74 6572 2c0a 2020 2020 2020    center,.      
+0000b630: 2020 2833 302c 2030 292c 0a20 2020 2020    (30, 0),.     
+0000b640: 2020 2022 7322 2c0a 2020 2020 290a 0a20     "s",.    ).. 
+0000b650: 2020 2023 2041 6e61 6c79 697a 6520 6275     # Analyize bu
+0000b660: 7474 6f6e 0a20 2020 2064 6973 706c 6179  tton.    display
+0000b670: 5f61 6e61 6c79 7a65 5f62 7574 746f 6e28  _analyze_button(
+0000b680: 7365 6c66 2c20 3133 290a 0a20 2020 2023  self, 13)..    #
+0000b690: 2052 6561 646d 6520 4865 6c70 2062 7574   Readme Help but
+0000b6a0: 746f 6e0a 2020 2020 7365 6c66 2e61 695f  ton.    self.ai_
+0000b6b0: 6865 6c70 5f62 7574 746f 6e20 3d20 6164  help_button = ad
+0000b6c0: 645f 6275 7474 6f6e 280a 2020 2020 2020  d_button(.      
+0000b6d0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000b6e0: 7365 6c66 2e74 6162 7669 6577 2e74 6162  self.tabview.tab
+0000b6f0: 2822 416e 616c 797a 6522 292c 0a20 2020  ("Analyze"),.   
+0000b700: 2020 2020 2022 2332 3436 4642 3622 2c0a       "#246FB6",.
+0000b710: 2020 2020 2020 2020 2822 2330 4246 3037          ("#0BF07
+0000b720: 3522 2c20 2223 6666 6439 3431 2229 2c0a  5", "#ffd941"),.
+0000b730: 2020 2020 2020 2020 2223 3162 6339 6666          "#1bc9ff
+0000b740: 222c 2020 2320 626f 7264 6572 5f63 6f6c  ",  # border_col
+0000b750: 6f72 3a20 7374 722c 0a20 2020 2020 2020  or: str,.       
+0000b760: 2073 656c 662e 6169 5f68 656c 705f 6576   self.ai_help_ev
+0000b770: 656e 742c 2020 2320 636f 6d6d 616e 640a  ent,  # command.
+0000b780: 2020 2020 2020 2020 312c 2020 2320 626f          1,  # bo
+0000b790: 7264 6572 5f77 6964 7468 3a20 696e 742c  rder_width: int,
+0000b7a0: 0a20 2020 2020 2020 2022 3f22 2c20 2023  .        "?",  #
+0000b7b0: 2074 6578 743a 2073 7472 2c0a 2020 2020   text: str,.    
+0000b7c0: 2020 2020 312c 2020 2320 636f 6c75 6d6e      1,  # column
+0000b7d0: 7370 616e 3a20 696e 742c 0a20 2020 2020  span: int,.     
+0000b7e0: 2020 2031 332c 2020 2320 726f 773a 2069     13,  # row: i
+0000b7f0: 6e74 2c0a 2020 2020 2020 2020 302c 2020  nt,.        0,  
+0000b800: 2320 636f 6c75 6d6e 3a20 696e 742c 0a20  # column: int,. 
+0000b810: 2020 2020 2020 2028 3139 302c 2030 292c         (190, 0),
+0000b820: 2020 2320 7061 6478 3a20 7475 706c 652c    # padx: tuple,
+0000b830: 2064 6f6e 2774 2063 6861 6e67 6520 7468   don't change th
+0000b840: 6973 2e0a 2020 2020 2020 2020 2831 302c  is..        (10,
+0000b850: 2031 3029 2c20 2023 2070 6164 793a 2074   10),  # pady: t
+0000b860: 7570 6c65 2c0a 2020 2020 2020 2020 226e  uple,.        "n
+0000b870: 222c 0a20 2020 2029 0a20 2020 2073 656c  ",.    ).    sel
+0000b880: 662e 6169 5f68 656c 705f 6275 7474 6f6e  f.ai_help_button
+0000b890: 2e63 6f6e 6669 6775 7265 2877 6964 7468  .configure(width
+0000b8a0: 3d32 3029 0a0a 2020 2020 2320 4465 6275  =20)..    # Debu
+0000b8b0: 6720 4d6f 6465 2063 6865 636b 626f 780a  g Mode checkbox.
+0000b8c0: 2020 2020 7365 6c66 2e64 6562 7567 5f63      self.debug_c
+0000b8d0: 6865 636b 626f 7820 3d20 6164 645f 6368  heckbox = add_ch
+0000b8e0: 6563 6b62 6f78 280a 2020 2020 2020 2020  eckbox(.        
+0000b8f0: 7365 6c66 2c0a 2020 2020 2020 2020 7365  self,.        se
+0000b900: 6c66 2e74 6162 7669 6577 2e74 6162 2822  lf.tabview.tab("
+0000b910: 4465 6275 6722 292c 0a20 2020 2020 2020  Debug"),.       
+0000b920: 2073 656c 662e 6465 6275 675f 6368 6563   self.debug_chec
+0000b930: 6b62 6f78 5f65 7665 6e74 2c0a 2020 2020  kbox_event,.    
+0000b940: 2020 2020 2244 6562 7567 204d 6f64 6522      "Debug Mode"
+0000b950: 2c0a 2020 2020 2020 2020 342c 0a20 2020  ,.        4,.   
+0000b960: 2020 2020 2033 2c0a 2020 2020 2020 2020       3,.        
+0000b970: 3230 2c0a 2020 2020 2020 2020 3130 2c0a  20,.        10,.
+0000b980: 2020 2020 2020 2020 2277 222c 0a20 2020          "w",.   
+0000b990: 2020 2020 2022 2336 3536 3366 6622 2c0a       "#6563ff",.
+0000b9a0: 2020 2020 290a 2020 2020 2320 5275 6e74      ).    # Runt
+0000b9b0: 696d 650a 2020 2020 7365 6c66 2e72 756e  ime.    self.run
+0000b9c0: 7469 6d65 5f63 6865 636b 626f 7820 3d20  time_checkbox = 
+0000b9d0: 6164 645f 6368 6563 6b62 6f78 280a 2020  add_checkbox(.  
+0000b9e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000b9f0: 2020 2020 7365 6c66 2e74 6162 7669 6577      self.tabview
+0000ba00: 2e74 6162 2822 4465 6275 6722 292c 0a20  .tab("Debug"),. 
+0000ba10: 2020 2020 2020 2073 656c 662e 7275 6e74         self.runt
+0000ba20: 696d 655f 6368 6563 6b62 6f78 5f65 7665  ime_checkbox_eve
+0000ba30: 6e74 2c0a 2020 2020 2020 2020 2244 6973  nt,.        "Dis
+0000ba40: 706c 6179 2052 756e 7469 6d65 2053 6574  play Runtime Set
+0000ba50: 7469 6e67 7322 2c0a 2020 2020 2020 2020  tings",.        
+0000ba60: 332c 0a20 2020 2020 2020 2033 2c0a 2020  3,.        3,.  
+0000ba70: 2020 2020 2020 3230 2c0a 2020 2020 2020        20,.      
+0000ba80: 2020 3130 2c0a 2020 2020 2020 2020 2277    10,.        "w
+0000ba90: 222c 0a20 2020 2020 2020 2022 2336 3536  ",.        "#656
+0000baa0: 3366 6622 2c0a 2020 2020 290a 0a0a 2320  3ff",.    )...# 
+0000bab0: 4469 7370 6c61 7920 4169 2027 416e 616c  Display Ai 'Anal
+0000bac0: 797a 6522 2062 7574 746f 6e0a 6465 6620  yze" button.def 
+0000bad0: 6469 7370 6c61 795f 616e 616c 797a 655f  display_analyze_
+0000bae0: 6275 7474 6f6e 2873 656c 662c 2072 6f77  button(self, row
+0000baf0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a20  : int) -> None: 
+0000bb00: 2023 206e 6f71 613a 2041 4e4e 3030 310a   # noqa: ANN001.
+0000bb10: 2020 2020 2222 220a 2020 2020 4469 7370      """.    Disp
+0000bb20: 6c61 7920 7468 6520 2741 6e61 6c79 7a65  lay the 'Analyze
+0000bb30: 2720 6275 7474 6f6e 2066 6f72 2074 6865  ' button for the
+0000bb40: 2041 4920 4150 4920 6b65 792e 0a0a 2020   AI API key...  
+0000bb50: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
+0000bb60: 6372 6561 7465 7320 616e 6420 6469 7370  creates and disp
+0000bb70: 6c61 7973 2061 2062 7574 746f 6e20 6f6e  lays a button on
+0000bb80: 2074 6865 2027 416e 616c 797a 6527 2074   the 'Analyze' t
+0000bb90: 6162 206f 6620 7468 6520 7461 6276 6965  ab of the tabvie
+0000bba0: 772e 2054 6865 2062 7574 746f 6e20 6973  w. The button is
+0000bbb0: 2075 7365 6420 746f 2072 756e 2074 6865   used to run the
+0000bbc0: 2061 6e61 6c79 7369 7320 666f 7220 7468   analysis for th
+0000bbd0: 6520 4149 2041 5049 206b 6579 2e0a 0a20  e AI API key... 
+0000bbe0: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
+0000bbf0: 2020 2020 2020 2073 656c 6620 286f 626a         self (obj
+0000bc00: 6563 7429 3a20 5468 6520 696e 7374 616e  ect): The instan
+0000bc10: 6365 206f 6620 7468 6520 636c 6173 732e  ce of the class.
+0000bc20: 0a20 2020 2020 2020 2072 6f77 2028 696e  .        row (in
+0000bc30: 7429 3a20 5468 6520 726f 7720 6e75 6d62  t): The row numb
+0000bc40: 6572 2074 6f20 6469 7370 6c61 7920 7468  er to display th
+0000bc50: 6520 6275 7474 6f6e 2e0a 0a20 2020 2052  e button...    R
+0000bc60: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000bc70: 4e6f 6e65 3a20 5468 6973 2066 756e 6374  None: This funct
+0000bc80: 696f 6e20 646f 6573 206e 6f74 2072 6574  ion does not ret
+0000bc90: 7572 6e20 616e 7974 6869 6e67 2e0a 2020  urn anything..  
+0000bca0: 2020 2222 220a 2020 2020 2320 4869 6768    """.    # High
+0000bcb0: 6c69 6768 7420 7468 6520 6275 7474 6f6e  light the button
+0000bcc0: 2069 6620 7765 2068 6176 6520 6576 6572   if we have ever
+0000bcd0: 7974 6869 6e67 2074 6f20 7275 6e20 7468  ything to run th
+0000bce0: 6520 416e 616c 7973 6973 2e0a 2020 2020  e Analysis..    
+0000bcf0: 6966 2028 2873 656c 662e 6169 5f6d 6f64  if ((self.ai_mod
+0000bd00: 656c 2069 6e20 4f50 454e 4149 5f4d 4f44  el in OPENAI_MOD
+0000bd10: 454c 5320 616e 6420 7365 6c66 2e61 695f  ELS and self.ai_
+0000bd20: 6170 696b 6579 2920 6f72 2073 656c 662e  apikey) or self.
+0000bd30: 6169 5f6d 6f64 656c 2920 616e 6420 280a  ai_model) and (.
+0000bd40: 2020 2020 2020 2020 7365 6c66 2e73 696e          self.sin
+0000bd50: 676c 655f 7461 736b 5f6e 616d 6520 6f72  gle_task_name or
+0000bd60: 2073 656c 662e 7369 6e67 6c65 5f70 726f   self.single_pro
+0000bd70: 6669 6c65 5f6e 616d 650a 2020 2020 293a  file_name.    ):
+0000bd80: 0a20 2020 2020 2020 2066 675f 636f 6c6f  .        fg_colo
+0000bd90: 7220 3d20 2223 6635 3564 6666 220a 2020  r = "#f55dff".  
+0000bda0: 2020 2020 2020 7465 7874 5f63 6f6c 6f72        text_color
+0000bdb0: 203d 2022 2335 3535 3466 6622 0a20 2020   = "#5554ff".   
+0000bdc0: 2065 6c73 653a 0a20 2020 2020 2020 2066   else:.        f
+0000bdd0: 675f 636f 6c6f 7220 3d20 2222 0a20 2020  g_color = "".   
+0000bde0: 2020 2020 2074 6578 745f 636f 6c6f 7220       text_color 
+0000bdf0: 3d20 2222 0a0a 2020 2020 7365 6c66 2e61  = ""..    self.a
+0000be00: 695f 616e 616c 797a 655f 6275 7474 6f6e  i_analyze_button
+0000be10: 203d 2061 6464 5f62 7574 746f 6e28 0a20   = add_button(. 
+0000be20: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000be30: 2020 2020 2073 656c 662e 7461 6276 6965       self.tabvie
+0000be40: 772e 7461 6228 2241 6e61 6c79 7a65 2229  w.tab("Analyze")
+0000be50: 2c0a 2020 2020 2020 2020 6667 5f63 6f6c  ,.        fg_col
+0000be60: 6f72 2c20 2023 2066 675f 636f 6c6f 723a  or,  # fg_color:
+0000be70: 2073 7472 2c0a 2020 2020 2020 2020 7465   str,.        te
+0000be80: 7874 5f63 6f6c 6f72 2c20 2023 2074 6578  xt_color,  # tex
+0000be90: 745f 636f 6c6f 723a 2073 7472 2c0a 2020  t_color: str,.  
+0000bea0: 2020 2020 2020 2222 2c20 2023 2062 6f72        "",  # bor
+0000beb0: 6465 725f 636f 6c6f 723a 2073 7472 2c0a  der_color: str,.
+0000bec0: 2020 2020 2020 2020 7365 6c66 2e61 695f          self.ai_
+0000bed0: 616e 616c 797a 655f 6576 656e 742c 2020  analyze_event,  
+0000bee0: 2320 636f 6d6d 616e 640a 2020 2020 2020  # command.      
+0000bef0: 2020 322c 2020 2320 626f 7264 6572 5f77    2,  # border_w
+0000bf00: 6964 7468 3a20 696e 742c 0a20 2020 2020  idth: int,.     
+0000bf10: 2020 2022 5275 6e20 416e 616c 7973 6973     "Run Analysis
+0000bf20: 222c 2020 2320 7465 7874 3a20 7374 722c  ",  # text: str,
+0000bf30: 0a20 2020 2020 2020 2031 2c20 2023 2063  .        1,  # c
+0000bf40: 6f6c 756d 6e73 7061 6e3a 2069 6e74 2c0a  olumnspan: int,.
+0000bf50: 2020 2020 2020 2020 726f 772c 2020 2320          row,  # 
+0000bf60: 726f 773a 2069 6e74 2c0a 2020 2020 2020  row: int,.      
+0000bf70: 2020 302c 2020 2320 636f 6c75 6d6e 3a20    0,  # column: 
+0000bf80: 696e 742c 0a20 2020 2020 2020 2035 302c  int,.        50,
+0000bf90: 2020 2320 7061 6478 3a20 7475 706c 652c    # padx: tuple,
+0000bfa0: 0a20 2020 2020 2020 2028 3130 2c20 3130  .        (10, 10
+0000bfb0: 292c 2020 2320 7061 6479 3a20 7475 706c  ),  # pady: tupl
+0000bfc0: 652c 0a20 2020 2020 2020 2022 6e22 2c0a  e,.        "n",.
+0000bfd0: 2020 2020 290a 0a0a 2320 2420 4465 6c65      )...# $ Dele
+0000bfe0: 7465 2065 7869 7374 696e 6720 4169 206c  te existing Ai l
+0000bff0: 6162 656c 730a 6465 6620 6465 6c65 7465  abels.def delete
+0000c000: 5f61 695f 6c61 6265 6c73 2873 656c 6629  _ai_labels(self)
+0000c010: 202d 3e20 4e6f 6e65 3a20 2023 206e 6f71   -> None:  # noq
+0000c020: 613a 2041 4e4e 3030 310a 2020 2020 2222  a: ANN001.    ""
+0000c030: 220a 2020 2020 4465 6c65 7465 7320 7468  ".    Deletes th
+0000c040: 6520 4149 206c 6162 656c 7320 6966 2074  e AI labels if t
+0000c050: 6865 7920 6578 6973 742e 0a20 2020 2022  hey exist..    "
+0000c060: 2222 0a20 2020 2077 6974 6820 636f 6e74  "".    with cont
+0000c070: 6578 746c 6962 2e73 7570 7072 6573 7328  extlib.suppress(
+0000c080: 4174 7472 6962 7574 6545 7272 6f72 293a  AttributeError):
+0000c090: 0a20 2020 2020 2020 2073 656c 662e 6169  .        self.ai
+0000c0a0: 5f73 6574 5f6c 6162 656c 312e 6465 7374  _set_label1.dest
+0000c0b0: 726f 7928 290a 2020 2020 7769 7468 2063  roy().    with c
+0000c0c0: 6f6e 7465 7874 6c69 622e 7375 7070 7265  ontextlib.suppre
+0000c0d0: 7373 2841 7474 7269 6275 7465 4572 726f  ss(AttributeErro
+0000c0e0: 7229 3a0a 2020 2020 2020 2020 7365 6c66  r):.        self
+0000c0f0: 2e61 695f 7365 745f 6c61 6265 6c32 2e64  .ai_set_label2.d
+0000c100: 6573 7472 6f79 2829 0a20 2020 2077 6974  estroy().    wit
+0000c110: 6820 636f 6e74 6578 746c 6962 2e73 7570  h contextlib.sup
+0000c120: 7072 6573 7328 4174 7472 6962 7574 6545  press(AttributeE
+0000c130: 7272 6f72 293a 0a20 2020 2020 2020 2073  rror):.        s
+0000c140: 656c 662e 6169 5f73 6574 5f6c 6162 656c  elf.ai_set_label
+0000c150: 332e 6465 7374 726f 7928 290a 2020 2020  3.destroy().    
+0000c160: 7769 7468 2063 6f6e 7465 7874 6c69 622e  with contextlib.
+0000c170: 7375 7070 7265 7373 2841 7474 7269 6275  suppress(Attribu
+0000c180: 7465 4572 726f 7229 3a0a 2020 2020 2020  teError):.      
+0000c190: 2020 7365 6c66 2e61 695f 7365 745f 6c61    self.ai_set_la
+0000c1a0: 6265 6c34 2e64 6573 7472 6f79 2829 0a0a  bel4.destroy()..
+0000c1b0: 0a23 2044 6973 706c 6179 2074 6865 2063  .# Display the c
+0000c1c0: 7572 7265 6e74 2073 6574 7469 6e67 7320  urrent settings 
+0000c1d0: 666f 7220 4169 0a64 6566 2064 6973 706c  for Ai.def displ
+0000c1e0: 6179 5f73 656c 6563 7465 645f 6f62 6a65  ay_selected_obje
+0000c1f0: 6374 5f6c 6162 656c 7328 7365 6c66 2920  ct_labels(self) 
+0000c200: 2d3e 204e 6f6e 653a 2020 2320 6e6f 7161  -> None:  # noqa
+0000c210: 3a20 414e 4e30 3031 0a20 2020 2022 2222  : ANN001.    """
+0000c220: 0a20 2020 2044 6973 706c 6179 2074 6865  .    Display the
+0000c230: 2063 7572 7265 6e74 2073 6574 7469 6e67   current setting
+0000c240: 7320 666f 7220 4169 0a20 2020 2022 2222  s for Ai.    """
+0000c250: 0a20 2020 2023 2044 656c 6574 6520 7072  .    # Delete pr
+0000c260: 6576 696f 7573 206c 6162 656c 7320 7369  evious labels si
+0000c270: 6e63 6520 7468 6579 206d 6179 2062 6520  nce they may be 
+0000c280: 6c6f 6e67 6572 2074 6861 6e20 6e65 7720  longer than new 
+0000c290: 6c61 6265 6c73 0a20 2020 2064 656c 6574  labels.    delet
+0000c2a0: 655f 6169 5f6c 6162 656c 7328 7365 6c66  e_ai_labels(self
+0000c2b0: 290a 0a20 2020 2023 2052 6561 6420 7468  )..    # Read th
+0000c2c0: 6520 6170 6920 6b65 792e 0a20 2020 2073  e api key..    s
+0000c2d0: 656c 662e 6169 5f61 7069 6b65 7920 3d20  elf.ai_apikey = 
+0000c2e0: 6765 745f 6170 695f 6b65 7928 290a 2020  get_api_key().  
+0000c2f0: 2020 6b65 795f 746f 5f64 6973 706c 6179    key_to_display
+0000c300: 203d 2022 5365 7422 2069 6620 7365 6c66   = "Set" if self
+0000c310: 2e61 695f 6170 696b 6579 2065 6c73 6520  .ai_apikey else 
+0000c320: 2255 6e73 6574 220a 2020 2020 6d6f 6465  "Unset".    mode
+0000c330: 6c5f 746f 5f64 6973 706c 6179 203d 2073  l_to_display = s
+0000c340: 656c 662e 6169 5f6d 6f64 656c 2069 6620  elf.ai_model if 
+0000c350: 7365 6c66 2e61 695f 6d6f 6465 6c20 656c  self.ai_model el
+0000c360: 7365 2022 4e6f 6e65 2028 6c6c 616d 6133  se "None (llama3
+0000c370: 2922 0a20 2020 2073 656c 662e 6169 5f73  )".    self.ai_s
+0000c380: 6574 5f6c 6162 656c 3120 3d20 6164 645f  et_label1 = add_
+0000c390: 6c61 6265 6c28 0a20 2020 2020 2020 2073  label(.        s
+0000c3a0: 656c 662c 0a20 2020 2020 2020 2073 656c  elf,.        sel
+0000c3b0: 662e 7461 6276 6965 772e 7461 6228 2241  f.tabview.tab("A
+0000c3c0: 6e61 6c79 7a65 2229 2c0a 2020 2020 2020  nalyze"),.      
+0000c3d0: 2020 6622 4150 4920 4b65 793a 207b 6b65    f"API Key: {ke
+0000c3e0: 795f 746f 5f64 6973 706c 6179 7d2c 204d  y_to_display}, M
+0000c3f0: 6f64 656c 3a20 7b6d 6f64 656c 5f74 6f5f  odel: {model_to_
+0000c400: 6469 7370 6c61 797d 222c 0a20 2020 2020  display}",.     
+0000c410: 2020 2022 222c 0a20 2020 2020 2020 2030     "",.        0
+0000c420: 2c0a 2020 2020 2020 2020 226e 6f72 6d61  ,.        "norma
+0000c430: 6c22 2c0a 2020 2020 2020 2020 3134 2c0a  l",.        14,.
+0000c440: 2020 2020 2020 2020 302c 0a20 2020 2020          0,.     
+0000c450: 2020 2031 302c 0a20 2020 2020 2020 2028     10,.        (
+0000c460: 302c 2032 3029 2c0a 2020 2020 2020 2020  0, 20),.        
+0000c470: 226e 7722 2c0a 2020 2020 290a 0a20 2020  "nw",.    )..   
+0000c480: 2070 726f 6669 6c65 5f74 6f5f 6469 7370   profile_to_disp
+0000c490: 6c61 7920 3d20 7365 6c66 2e73 696e 676c  lay = self.singl
+0000c4a0: 655f 7072 6f66 696c 655f 6e61 6d65 2069  e_profile_name i
+0000c4b0: 6620 7365 6c66 2e73 696e 676c 655f 7072  f self.single_pr
+0000c4c0: 6f66 696c 655f 6e61 6d65 2065 6c73 6520  ofile_name else 
+0000c4d0: 2255 6e64 6566 696e 6564 220a 2020 2020  "Undefined".    
+0000c4e0: 7461 736b 5f74 6f5f 6469 7370 6c61 7920  task_to_display 
+0000c4f0: 3d20 7365 6c66 2e73 696e 676c 655f 7461  = self.single_ta
+0000c500: 736b 5f6e 616d 6520 6966 2073 656c 662e  sk_name if self.
+0000c510: 7369 6e67 6c65 5f74 6173 6b5f 6e61 6d65  single_task_name
+0000c520: 2065 6c73 6520 2255 6e64 6566 696e 6564   else "Undefined
+0000c530: 220a 2020 2020 7365 6c66 2e61 695f 6d6f  ".    self.ai_mo
+0000c540: 6465 6c5f 6f70 7469 6f6e 2e73 6574 286d  del_option.set(m
+0000c550: 6f64 656c 5f74 6f5f 6469 7370 6c61 7929  odel_to_display)
+0000c560: 2020 2320 5365 7420 7468 6520 6375 7272    # Set the curr
+0000c570: 656e 7420 6d6f 6465 6c20 696e 2074 6865  ent model in the
+0000c580: 2070 756c 6c64 6f77 6e2e 0a0a 2020 2020   pulldown...    
+0000c590: 2320 5468 6520 6c61 6265 6c20 7368 6f75  # The label shou
+0000c5a0: 6c64 2068 6176 6520 6265 656e 2064 6573  ld have been des
+0000c5b0: 7472 6f79 6564 2c20 6275 7420 6973 6e27  troyed, but isn'
+0000c5c0: 7420 6475 6520 746f 2074 6b20 6275 672e  t due to tk bug.
+0000c5d0: 2020 536f 2077 6520 6861 7665 2074 6f20    So we have to 
+0000c5e0: 626c 616e 6b20 6669 6c6c 2069 6620 6e65  blank fill if ne
+0000c5f0: 6365 7373 6172 792e 0a20 2020 2023 2070  cessary..    # p
+0000c600: 726f 6669 6c65 5f6c 656e 6774 6820 3d20  rofile_length = 
+0000c610: 6c65 6e28 7072 6f66 696c 655f 746f 5f64  len(profile_to_d
+0000c620: 6973 706c 6179 290a 2020 2020 2320 6669  isplay).    # fi
+0000c630: 6c6c 203d 2031 360a 2020 2020 2320 6966  ll = 16.    # if
+0000c640: 2070 726f 6669 6c65 5f6c 656e 6774 6820   profile_length 
+0000c650: 3c20 6669 6c6c 3a0a 2020 2020 2320 2020  < fill:.    #   
+0000c660: 2070 726f 6669 6c65 5f74 6f5f 6469 7370   profile_to_disp
+0000c670: 6c61 7920 3d20 7072 6f66 696c 655f 746f  lay = profile_to
+0000c680: 5f64 6973 706c 6179 2e6c 6a75 7374 2866  _display.ljust(f
+0000c690: 696c 6c20 2d20 7072 6f66 696c 655f 6c65  ill - profile_le
+0000c6a0: 6e67 7468 2c20 2220 2229 0a0a 2020 2020  ngth, " ")..    
+0000c6b0: 2320 4469 7370 6c61 7920 7468 6520 5072  # Display the Pr
+0000c6c0: 6f66 696c 6520 746f 2061 6e61 6c79 7a65  ofile to analyze
+0000c6d0: 0a20 2020 2073 656c 662e 6169 5f73 6574  .    self.ai_set
+0000c6e0: 5f6c 6162 656c 3220 3d20 6164 645f 6c61  _label2 = add_la
+0000c6f0: 6265 6c28 0a20 2020 2020 2020 2073 656c  bel(.        sel
+0000c700: 662c 0a20 2020 2020 2020 2073 656c 662e  f,.        self.
+0000c710: 7461 6276 6965 772e 7461 6228 2241 6e61  tabview.tab("Ana
+0000c720: 6c79 7a65 2229 2c0a 2020 2020 2020 2020  lyze"),.        
+0000c730: 6622 5072 6f66 696c 6520 746f 2041 6e61  f"Profile to Ana
+0000c740: 6c79 7a65 3a20 7b70 726f 6669 6c65 5f74  lyze: {profile_t
+0000c750: 6f5f 6469 7370 6c61 797d 222c 0a20 2020  o_display}",.   
+0000c760: 2020 2020 2022 222c 0a20 2020 2020 2020       "",.       
+0000c770: 2030 2c0a 2020 2020 2020 2020 226e 6f72   0,.        "nor
+0000c780: 6d61 6c22 2c0a 2020 2020 2020 2020 3134  mal",.        14
+0000c790: 2c0a 2020 2020 2020 2020 302c 0a20 2020  ,.        0,.   
+0000c7a0: 2020 2020 2031 302c 0a20 2020 2020 2020       10,.       
+0000c7b0: 2028 3330 2c20 3029 2c0a 2020 2020 2020   (30, 0),.      
+0000c7c0: 2020 2273 7722 2c0a 2020 2020 290a 2020    "sw",.    ).  
+0000c7d0: 2020 2320 4469 7370 6c61 7920 7468 6520    # Display the 
+0000c7e0: 5461 736b 2074 6f20 616e 616c 797a 650a  Task to analyze.
+0000c7f0: 2020 2020 7365 6c66 2e61 695f 7365 745f      self.ai_set_
+0000c800: 6c61 6265 6c33 203d 2061 6464 5f6c 6162  label3 = add_lab
+0000c810: 656c 280a 2020 2020 2020 2020 7365 6c66  el(.        self
+0000c820: 2c0a 2020 2020 2020 2020 7365 6c66 2e74  ,.        self.t
+0000c830: 6162 7669 6577 2e74 6162 2822 416e 616c  abview.tab("Anal
+0000c840: 797a 6522 292c 0a20 2020 2020 2020 2066  yze"),.        f
+0000c850: 2254 6173 6b20 746f 2041 6e61 6c79 7a65  "Task to Analyze
+0000c860: 3a20 7b74 6173 6b5f 746f 5f64 6973 706c  : {task_to_displ
+0000c870: 6179 7d22 2c0a 2020 2020 2020 2020 2222  ay}",.        ""
+0000c880: 2c0a 2020 2020 2020 2020 302c 0a20 2020  ,.        0,.   
+0000c890: 2020 2020 2022 6e6f 726d 616c 222c 0a20       "normal",. 
+0000c8a0: 2020 2020 2020 2031 352c 0a20 2020 2020         15,.     
+0000c8b0: 2020 2030 2c0a 2020 2020 2020 2020 3130     0,.        10
+0000c8c0: 2c0a 2020 2020 2020 2020 2830 2c20 3235  ,.        (0, 25
+0000c8d0: 292c 0a20 2020 2020 2020 2022 6e77 222c  ),.        "nw",
+0000c8e0: 0a20 2020 2029 0a20 2020 2023 2044 6973  .    ).    # Dis
+0000c8f0: 706c 6179 2074 6865 2050 726f 6d70 742e  play the Prompt.
+0000c900: 2e6f 6e6c 7920 6669 7273 7420 3235 2063  .only first 25 c
+0000c910: 6861 7273 2e0a 2020 2020 6d61 786c 656e  hars..    maxlen
+0000c920: 203d 2032 350a 2020 2020 6469 7370 6c61   = 25.    displa
+0000c930: 795f 7072 6f6d 7074 203d 2073 656c 662e  y_prompt = self.
+0000c940: 6169 5f70 726f 6d70 745b 3a6d 6178 6c65  ai_prompt[:maxle
+0000c950: 6e5d 202b 2022 2e2e 2e22 2069 6620 6c65  n] + "..." if le
+0000c960: 6e28 7365 6c66 2e61 695f 7072 6f6d 7074  n(self.ai_prompt
+0000c970: 2920 3e20 6d61 786c 656e 2065 6c73 6520  ) > maxlen else 
+0000c980: 7365 6c66 2e61 695f 7072 6f6d 7074 0a20  self.ai_prompt. 
+0000c990: 2020 2073 656c 662e 6169 5f73 6574 5f6c     self.ai_set_l
+0000c9a0: 6162 656c 3420 3d20 6164 645f 6c61 6265  abel4 = add_labe
+0000c9b0: 6c28 0a20 2020 2020 2020 2073 656c 662c  l(.        self,
+0000c9c0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+0000c9d0: 6276 6965 772e 7461 6228 2241 6e61 6c79  bview.tab("Analy
+0000c9e0: 7a65 2229 2c0a 2020 2020 2020 2020 6622  ze"),.        f"
+0000c9f0: 5072 6f6d 7074 3a20 277b 6469 7370 6c61  Prompt: '{displa
+0000ca00: 795f 7072 6f6d 7074 7d27 222c 0a20 2020  y_prompt}'",.   
+0000ca10: 2020 2020 2022 222c 0a20 2020 2020 2020       "",.       
+0000ca20: 2030 2c0a 2020 2020 2020 2020 226e 6f72   0,.        "nor
+0000ca30: 6d61 6c22 2c0a 2020 2020 2020 2020 3135  mal",.        15
+0000ca40: 2c0a 2020 2020 2020 2020 302c 0a20 2020  ,.        0,.   
+0000ca50: 2020 2020 2031 302c 0a20 2020 2020 2020       10,.       
+0000ca60: 2028 3130 2c20 3029 2c0a 2020 2020 2020   (10, 0),.      
+0000ca70: 2020 2273 7722 2c0a 2020 2020 290a 0a20    "sw",.    ).. 
+0000ca80: 2020 2023 2044 6973 706c 6179 2074 6865     # Display the
+0000ca90: 206c 6162 656c 206f 6e20 2753 7065 6369   label on 'Speci
+0000caa0: 6669 6320 4e61 6d65 2720 7461 622e 0a20  fic Name' tab.. 
+0000cab0: 2020 2023 2046 6972 7374 2074 696d 6520     # First time 
+0000cac0: 7468 726f 7567 682c 2073 656c 662e 7370  through, self.sp
+0000cad0: 6563 6966 6963 5f6e 616d 655f 6d73 6720  ecific_name_msg 
+0000cae0: 3d20 2727 0a20 2020 206e 616d 655f 746f  = ''.    name_to
+0000caf0: 5f64 6973 706c 6179 203d 2073 656c 662e  _display = self.
+0000cb00: 7370 6563 6966 6963 5f6e 616d 655f 6d73  specific_name_ms
+0000cb10: 6720 6966 2073 656c 662e 7370 6563 6966  g if self.specif
+0000cb20: 6963 5f6e 616d 655f 6d73 6720 656c 7365  ic_name_msg else
+0000cb30: 2061 6c6c 5f6f 626a 6563 7473 0a0a 2020   all_objects..  
+0000cb40: 2020 7365 6c66 2e73 696e 676c 655f 6c61    self.single_la
+0000cb50: 6265 6c20 3d20 6164 645f 6c61 6265 6c28  bel = add_label(
+0000cb60: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000cb70: 2020 2020 2020 2073 656c 662e 7461 6276         self.tabv
+0000cb80: 6965 772e 7461 6228 2253 7065 6369 6669  iew.tab("Specifi
+0000cb90: 6320 4e61 6d65 2229 2c0a 2020 2020 2020  c Name"),.      
+0000cba0: 2020 6e61 6d65 5f74 6f5f 6469 7370 6c61    name_to_displa
+0000cbb0: 792c 0a20 2020 2020 2020 2028 2223 3042  y,.        ("#0B
+0000cbc0: 4630 3735 222c 2022 2333 6639 3966 6622  F075", "#3f99ff"
+0000cbd0: 292c 0a20 2020 2020 2020 2030 2c0a 2020  ),.        0,.  
+0000cbe0: 2020 2020 2020 226e 6f72 6d61 6c22 2c0a        "normal",.
+0000cbf0: 2020 2020 2020 2020 3130 2c0a 2020 2020          10,.    
+0000cc00: 2020 2020 302c 0a20 2020 2020 2020 2032      0,.        2
+0000cc10: 302c 0a20 2020 2020 2020 2028 3130 2c20  0,.        (10, 
+0000cc20: 3130 292c 0a20 2020 2020 2020 2022 7722  10),.        "w"
+0000cc30: 2c0a 2020 2020 290a 0a0a 2320 5570 6461  ,.    )...# Upda
+0000cc40: 7465 2074 6865 2050 726f 6a65 6374 2f50  te the Project/P
+0000cc50: 726f 6669 6c65 2f54 6173 6b20 7075 6c6c  rofile/Task pull
+0000cc60: 646f 776e 206f 7074 696f 6e20 6d65 6e75  down option menu
+0000cc70: 732e 0a64 6566 2075 7064 6174 655f 7461  s..def update_ta
+0000cc80: 736b 6572 5f6f 626a 6563 745f 6d65 6e75  sker_object_menu
+0000cc90: 7328 7365 6c66 2c20 6765 745f 6461 7461  s(self, get_data
+0000cca0: 3a20 626f 6f6c 2920 2d3e 204e 6f6e 653a  : bool) -> None:
+0000ccb0: 2020 2320 6e6f 7161 3a20 414e 4e30 3031    # noqa: ANN001
+0000ccc0: 0a20 2020 2022 2222 0a20 2020 2061 7267  .    """.    arg
+0000ccd0: 733a 0a20 2020 2020 2020 2067 6574 5f64  s:.        get_d
+0000cce0: 6174 613a 2062 6f6f 6c20 3d20 5472 7565  ata: bool = True
+0000ccf0: 2069 6620 7765 2073 686f 756c 6420 6765   if we should ge
+0000cd00: 7420 7468 6520 786d 6c20 6461 7461 2074  t the xml data t
+0000cd10: 7265 6520 616e 6420 6275 696c 6420 7468  ree and build th
+0000cd20: 6520 7075 6c6c 646f 776e 206d 656e 7573  e pulldown menus
+0000cd30: 2e0a 2020 2020 5570 6461 7465 7320 7468  ..    Updates th
+0000cd40: 6520 7461 736b 6572 206f 626a 6563 7420  e tasker object 
+0000cd50: 6d65 6e75 7320 6261 7365 6420 6f6e 2074  menus based on t
+0000cd60: 6865 2063 7572 7265 6e74 2063 6f6e 6469  he current condi
+0000cd70: 7469 6f6e 732e 0a0a 2020 2020 5468 6973  tions...    This
+0000cd80: 2066 756e 6374 696f 6e20 6465 7465 726d   function determ
+0000cd90: 696e 6573 2074 6865 2076 616c 7565 7320  ines the values 
+0000cda0: 746f 2062 6520 6469 7370 6c61 7965 6420  to be displayed 
+0000cdb0: 696e 2074 6865 206f 7074 696f 6e20 6d65  in the option me
+0000cdc0: 6e75 7320 666f 7220 7468 6520 7461 736b  nus for the task
+0000cdd0: 6572 206f 626a 6563 7473 2e20 5468 6520  er objects. The 
+0000cde0: 7661 6c75 6573 2061 7265 2064 6574 6572  values are deter
+0000cdf0: 6d69 6e65 6420 6261 7365 6420 6f6e 2074  mined based on t
+0000ce00: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6e  he following con
+0000ce10: 6469 7469 6f6e 733a 0a0a 2020 2020 2d20  ditions:..    - 
+0000ce20: 4966 2061 2073 696e 676c 6520 7072 6f6a  If a single proj
+0000ce30: 6563 7420 6e61 6d65 2069 7320 6176 6169  ect name is avai
+0000ce40: 6c61 626c 652c 2074 6865 2070 726f 6a65  lable, the proje
+0000ce50: 6374 206f 7074 696f 6e20 6d65 6e75 2069  ct option menu i
+0000ce60: 7320 7365 7420 746f 2074 6865 2070 726f  s set to the pro
+0000ce70: 6a65 6374 206e 616d 652c 2061 6e64 2074  ject name, and t
+0000ce80: 6865 2070 726f 6669 6c65 2061 6e64 2074  he profile and t
+0000ce90: 6173 6b20 6f70 7469 6f6e 206d 656e 7573  ask option menus
+0000cea0: 2061 7265 2073 6574 2074 6f20 7468 6569   are set to thei
+0000ceb0: 7220 6465 6661 756c 7420 7661 6c75 6573  r default values
+0000cec0: 2e0a 2020 2020 2d20 4966 2061 2073 696e  ..    - If a sin
+0000ced0: 676c 6520 7072 6f66 696c 6520 6e61 6d65  gle profile name
+0000cee0: 2069 7320 6176 6169 6c61 626c 652c 2074   is available, t
+0000cef0: 6865 2070 726f 6669 6c65 206f 7074 696f  he profile optio
+0000cf00: 6e20 6d65 6e75 2069 7320 7365 7420 746f  n menu is set to
+0000cf10: 2074 6865 2070 726f 6669 6c65 206e 616d   the profile nam
+0000cf20: 652c 2061 6e64 2074 6865 2070 726f 6a65  e, and the proje
+0000cf30: 6374 2061 6e64 2074 6173 6b20 6f70 7469  ct and task opti
+0000cf40: 6f6e 206d 656e 7573 2061 7265 2073 6574  on menus are set
+0000cf50: 2074 6f20 7468 6569 7220 6465 6661 756c   to their defaul
+0000cf60: 7420 7661 6c75 6573 2e0a 2020 2020 2d20  t values..    - 
+0000cf70: 4966 2061 2073 696e 676c 6520 7461 736b  If a single task
+0000cf80: 206e 616d 6520 6973 2061 7661 696c 6162   name is availab
+0000cf90: 6c65 2061 6e64 2074 6865 206c 6973 7420  le and the list 
+0000cfa0: 6f66 2074 6173 6b65 7220 6f62 6a65 6374  of tasker object
+0000cfb0: 7320 6973 206e 6f74 2065 6d70 7479 2c20  s is not empty, 
+0000cfc0: 7468 6520 7461 736b 206f 7074 696f 6e20  the task option 
+0000cfd0: 6d65 6e75 2069 7320 7365 7420 746f 2074  menu is set to t
+0000cfe0: 6865 2074 6173 6b20 6e61 6d65 2c20 616e  he task name, an
+0000cff0: 6420 7468 6520 7072 6f6a 6563 7420 616e  d the project an
+0000d000: 6420 7072 6f66 696c 6520 6f70 7469 6f6e  d profile option
+0000d010: 206d 656e 7573 2061 7265 2073 6574 2074   menus are set t
+0000d020: 6f20 7468 6569 7220 6465 6661 756c 7420  o their default 
+0000d030: 7661 6c75 6573 2e0a 2020 2020 2d20 4966  values..    - If
+0000d040: 206e 6f6e 6520 6f66 2074 6865 2061 626f   none of the abo
+0000d050: 7665 2063 6f6e 6469 7469 6f6e 7320 6172  ve conditions ar
+0000d060: 6520 6d65 742c 2061 6c6c 206f 7074 696f  e met, all optio
+0000d070: 6e20 6d65 6e75 7320 6172 6520 7365 7420  n menus are set 
+0000d080: 746f 2074 6865 6972 2064 6566 6175 6c74  to their default
+0000d090: 2076 616c 7565 732e 0a0a 2020 2020 5061   values...    Pa
+0000d0a0: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
+0000d0b0: 2020 7365 6c66 2028 6f62 6a65 6374 293a    self (object):
+0000d0c0: 2054 6865 2063 7572 7265 6e74 2069 6e73   The current ins
+0000d0d0: 7461 6e63 6520 6f66 2074 6865 2063 6c61  tance of the cla
+0000d0e0: 7373 2e0a 0a20 2020 2052 6574 7572 6e73  ss...    Returns
+0000d0f0: 3a0a 2020 2020 2020 2020 4e6f 6e65 3a20  :.        None: 
+0000d100: 5468 6973 2066 756e 6374 696f 6e20 646f  This function do
+0000d110: 6573 206e 6f74 2072 6574 7572 6e20 616e  es not return an
+0000d120: 7974 6869 6e67 2e0a 2020 2020 2222 220a  ything..    """.
+0000d130: 2020 2020 2320 4765 7420 6461 7461 2074      # Get data t
+0000d140: 7265 652c 206c 6973 7420 616e 6420 7365  ree, list and se
+0000d150: 7420 7468 6520 5072 6f6a 6563 742f 5072  t the Project/Pr
+0000d160: 6f66 696c 652f 5461 736b 206c 6973 7420  ofile/Task list 
+0000d170: 696e 2027 5370 6563 6966 6963 204e 616d  in 'Specific Nam
+0000d180: 6527 2061 6e64 2027 416e 616c 797a 6527  e' and 'Analyze'
+0000d190: 2074 6162 2e0a 2020 2020 2320 4f6e 6c79   tab..    # Only
+0000d1a0: 2064 6f20 7468 6973 2069 6620 7765 2068   do this if we h
+0000d1b0: 6176 6520 7468 6520 6f62 6a65 6374 206e  ave the object n
+0000d1c0: 616d 6520 7369 6e63 6520 6974 2066 6f72  ame since it for
+0000d1d0: 6365 7320 6120 7265 6164 206f 6620 584d  ces a read of XM
+0000d1e0: 4c2e 0a20 2020 2069 6620 6765 745f 6461  L..    if get_da
+0000d1f0: 7461 3a0a 2020 2020 2020 2020 5f20 3d20  ta:.        _ = 
+0000d200: 6c69 7374 5f74 6173 6b65 725f 6f62 6a65  list_tasker_obje
+0000d210: 6374 7328 7365 6c66 290a 0a20 2020 2023  cts(self)..    #
+0000d220: 2044 6574 6572 6d69 6e65 2076 616c 7565   Determine value
+0000d230: 7320 6261 7365 6420 6f6e 2063 6f6e 6469  s based on condi
+0000d240: 7469 6f6e 730a 2020 2020 2320 5570 6461  tions.    # Upda
+0000d250: 7465 2074 6865 2050 726f 6a65 6374 2f50  te the Project/P
+0000d260: 726f 6669 6c65 2f54 6173 6b20 7075 6c6c  rofile/Task pull
+0000d270: 646f 776e 206f 7074 696f 6e20 6d65 6e75  down option menu
+0000d280: 732e 0a20 2020 2073 6574 5f74 6173 6b65  s..    set_taske
+0000d290: 725f 6f62 6a65 6374 5f6e 616d 6573 2873  r_object_names(s
+0000d2a0: 656c 6629 0a0a 2020 2020 2320 5570 6461  elf)..    # Upda
+0000d2b0: 7465 2074 6865 2074 6578 7420 6c61 6265  te the text labe
+0000d2c0: 6c73 0a20 2020 2064 6973 706c 6179 5f73  ls.    display_s
+0000d2d0: 656c 6563 7465 645f 6f62 6a65 6374 5f6c  elected_object_l
+0000d2e0: 6162 656c 7328 7365 6c66 290a 0a0a 2320  abels(self)...# 
+0000d2f0: 4765 7420 7468 6520 4169 2061 7069 206b  Get the Ai api k
+0000d300: 6579 0a64 6566 2067 6574 5f61 7069 5f6b  ey.def get_api_k
+0000d310: 6579 2829 202d 3e20 7374 723a 0a20 2020  ey() -> str:.   
+0000d320: 2022 2222 0a20 2020 2052 6574 7269 6576   """.    Retriev
+0000d330: 6573 2074 6865 2041 5049 206b 6579 2066  es the API key f
+0000d340: 726f 6d20 7468 6520 7370 6563 6966 6965  rom the specifie
+0000d350: 6420 6669 6c65 2e0a 0a20 2020 2054 6869  d file...    Thi
+0000d360: 7320 6675 6e63 7469 6f6e 2063 6865 636b  s function check
+0000d370: 7320 6966 2074 6865 204b 4559 4649 4c45  s if the KEYFILE
+0000d380: 2065 7869 7374 7320 616e 6420 6966 2069   exists and if i
+0000d390: 7420 646f 6573 2c20 6974 206f 7065 6e73  t does, it opens
+0000d3a0: 2074 6865 2066 696c 6520 616e 6420 7265   the file and re
+0000d3b0: 6164 7320 7468 6520 6669 7273 7420 6c69  ads the first li
+0000d3c0: 6e65 2e20 5468 6520 6669 7273 7420 6c69  ne. The first li
+0000d3d0: 6e65 2069 7320 6173 7375 6d65 6420 746f  ne is assumed to
+0000d3e0: 2062 6520 7468 6520 4150 4920 6b65 792e   be the API key.
+0000d3f0: 2049 6620 7468 6520 4b45 5946 494c 4520   If the KEYFILE 
+0000d400: 646f 6573 206e 6f74 2065 7869 7374 2c20  does not exist, 
+0000d410: 6974 2072 6574 7572 6e73 2074 6865 2073  it returns the s
+0000d420: 7472 696e 6720 224e 6f6e 6522 2e0a 0a20  tring "None"... 
+0000d430: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000d440: 2020 2020 7374 723a 2054 6865 2041 5049      str: The API
+0000d450: 206b 6579 2069 6620 6974 2065 7869 7374   key if it exist
+0000d460: 732c 206f 7468 6572 7769 7365 2022 4e6f  s, otherwise "No
+0000d470: 6e65 222e 0a20 2020 2022 2222 0a20 2020  ne"..    """.   
+0000d480: 2069 6620 6f73 2e70 6174 682e 6973 6669   if os.path.isfi
+0000d490: 6c65 284b 4559 4649 4c45 293a 0a20 2020  le(KEYFILE):.   
+0000d4a0: 2020 2020 2023 204f 7065 6e20 6f75 7470       # Open outp
+0000d4b0: 7574 2066 696c 650a 2020 2020 2020 2020  ut file.        
+0000d4c0: 7769 7468 206f 7065 6e28 4b45 5946 494c  with open(KEYFIL
+0000d4d0: 4529 2061 7320 6b65 795f 6669 6c65 3a0a  E) as key_file:.
+0000d4e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000d4f0: 726e 206b 6579 5f66 696c 652e 7265 6164  rn key_file.read
+0000d500: 6c69 6e65 2829 0a20 2020 2065 6c73 653a  line().    else:
+0000d510: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000d520: 224e 6f6e 6522 0a0a 0a23 2045 6974 6865  "None"...# Eithe
+0000d530: 7220 7661 6c69 6461 7465 2074 6865 2066  r validate the f
+0000d540: 696c 6520 6c6f 6361 7469 6f6e 2070 726f  ile location pro
+0000d550: 7669 6465 6420 6f72 2070 726f 7669 6465  vided or provide
+0000d560: 2061 2066 696c 656c 6973 7420 6f66 2058   a filelist of X
+0000d570: 4d4c 2066 696c 6573 0a64 6566 2076 616c  ML files.def val
+0000d580: 6964 6174 655f 6f72 5f66 696c 656c 6973  idate_or_filelis
+0000d590: 745f 786d 6c28 0a20 2020 2073 656c 662c  t_xml(.    self,
+0000d5a0: 2020 2320 6e6f 7161 3a20 414e 4e30 3031    # noqa: ANN001
+0000d5b0: 0a20 2020 2061 6e64 726f 6964 5f69 7061  .    android_ipa
+0000d5c0: 6464 723a 2073 7472 2c0a 2020 2020 616e  ddr: str,.    an
+0000d5d0: 6472 6f69 645f 706f 7274 3a20 7374 722c  droid_port: str,
+0000d5e0: 0a20 2020 2061 6e64 726f 6964 5f66 696c  .    android_fil
+0000d5f0: 653a 2073 7472 2c0a 2920 2d3e 2074 7570  e: str,.) -> tup
+0000d600: 6c65 5b69 6e74 2c20 7374 725d 3a0a 2020  le[int, str]:.  
+0000d610: 2020 2320 4966 2077 6520 646f 6e27 7420    # If we don't 
+0000d620: 6861 7665 2074 6865 2066 696c 6520 6c6f  have the file lo
+0000d630: 6361 7469 6f6e 2079 6574 2061 6e64 2077  cation yet and w
+0000d640: 6520 646f 6e27 7420 7965 7420 6861 7665  e don't yet have
+0000d650: 2061 206c 6973 7420 6f66 2066 696c 6573   a list of files
+0000d660: 2c20 7468 656e 2067 6574 2074 6865 2058  , then get the X
+0000d670: 4d4c 2066 696c 650a 2020 2020 2320 746f  ML file.    # to
+0000d680: 2076 616c 6964 6174 6520 7468 6174 2069   validate that i
+0000d690: 7420 6578 6973 7473 2e0a 2020 2020 2222  t exists..    ""
+0000d6a0: 2246 756e 6374 696f 6e20 746f 2076 616c  "Function to val
+0000d6b0: 6964 6174 6520 616e 2058 4d4c 2066 696c  idate an XML fil
+0000d6c0: 6520 6f6e 2061 6e20 416e 6472 6f69 6420  e on an Android 
+0000d6d0: 6465 7669 6365 2061 6e64 2072 6574 7572  device and retur
+0000d6e0: 6e20 7468 6520 6669 6c65 2773 2063 6f6e  n the file's con
+0000d6f0: 7465 6e74 7320 6966 2069 7420 6578 6973  tents if it exis
+0000d700: 7473 2e0a 2020 2020 5061 7261 6d65 7465  ts..    Paramete
+0000d710: 7273 3a0a 2020 2020 2020 2020 2d20 616e  rs:.        - an
+0000d720: 6472 6f69 645f 6970 6164 6472 2028 7374  droid_ipaddr (st
+0000d730: 7229 3a20 4950 2061 6464 7265 7373 206f  r): IP address o
+0000d740: 6620 7468 6520 416e 6472 6f69 6420 6465  f the Android de
+0000d750: 7669 6365 2e0a 2020 2020 2020 2020 2d20  vice..        - 
+0000d760: 616e 6472 6f69 645f 706f 7274 2028 7374  android_port (st
+0000d770: 7229 3a20 506f 7274 206e 756d 6265 7220  r): Port number 
+0000d780: 6f66 2074 6865 2041 6e64 726f 6964 2064  of the Android d
+0000d790: 6576 6963 652e 0a20 2020 2020 2020 202d  evice..        -
+0000d7a0: 2061 6e64 726f 6964 5f66 696c 6520 2873   android_file (s
+0000d7b0: 7472 293a 2046 696c 6520 6e61 6d65 206f  tr): File name o
+0000d7c0: 6620 7468 6520 584d 4c20 6669 6c65 2074  f the XML file t
+0000d7d0: 6f20 7661 6c69 6461 7465 2e0a 2020 2020  o validate..    
+0000d7e0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0000d7f0: 202d 2054 7570 6c65 5b69 6e74 2c20 7374   - Tuple[int, st
+0000d800: 725d 3a20 4120 7475 706c 6520 636f 6e74  r]: A tuple cont
+0000d810: 6169 6e69 6e67 2074 6865 2072 6574 7572  aining the retur
+0000d820: 6e20 636f 6465 2061 6e64 2074 6865 2066  n code and the f
+0000d830: 696c 6527 7320 636f 6e74 656e 7473 2069  ile's contents i
+0000d840: 6620 6974 2065 7869 7374 732e 0a20 2020  f it exists..   
+0000d850: 2050 726f 6365 7373 696e 6720 4c6f 6769   Processing Logi
+0000d860: 633a 0a20 2020 2020 2020 202d 2047 6574  c:.        - Get
+0000d870: 2074 6865 2058 4d4c 2066 696c 6520 6672   the XML file fr
+0000d880: 6f6d 2074 6865 2041 6e64 726f 6964 2064  om the Android d
+0000d890: 6576 6963 6520 6966 206e 6f20 6669 6c65  evice if no file
+0000d8a0: 206c 6f63 6174 696f 6e20 6973 2070 726f   location is pro
+0000d8b0: 7669 6465 642e 0a20 2020 2020 2020 202d  vided..        -
+0000d8c0: 2056 616c 6964 6174 6520 7468 6520 584d   Validate the XM
+0000d8d0: 4c20 6669 6c65 2e0a 2020 2020 2020 2020  L file..        
+0000d8e0: 2d20 4966 2074 6865 2066 696c 6520 646f  - If the file do
+0000d8f0: 6573 206e 6f74 2065 7869 7374 2c20 6469  es not exist, di
+0000d900: 7370 6c61 7920 616e 2065 7272 6f72 206d  splay an error m
+0000d910: 6573 7361 6765 2e0a 2020 2020 2020 2020  essage..        
+0000d920: 2d20 4966 2074 6865 2066 696c 6520 6c6f  - If the file lo
+0000d930: 6361 7469 6f6e 2069 7320 6e6f 7420 7072  cation is not pr
+0000d940: 6f76 6964 6564 2c20 6765 7420 6120 6c69  ovided, get a li
+0000d950: 7374 206f 6620 616c 6c20 584d 4c20 6669  st of all XML fi
+0000d960: 6c65 7320 6672 6f6d 2074 6865 2041 6e64  les from the And
+0000d970: 726f 6964 2064 6576 6963 6520 616e 6420  roid device and 
+0000d980: 7072 6573 656e 7420 6974 2074 6f20 7468  present it to th
+0000d990: 6520 7573 6572 2e0a 2020 2020 2222 220a  e user..    """.
+0000d9a0: 2020 2020 2320 4966 2077 6520 646f 6e27      # If we don'
+0000d9b0: 7420 7965 7420 6861 7665 2074 6865 2066  t yet have the f
+0000d9c0: 696c 652c 2074 6865 6e20 6765 7420 6974  ile, then get it
+0000d9d0: 2066 726f 6d20 7468 6520 416e 6472 6f69   from the Androi
+0000d9e0: 6420 6465 7669 6365 2e0a 2020 2020 6966  d device..    if
+0000d9f0: 206c 656e 2861 6e64 726f 6964 5f66 696c   len(android_fil
+0000da00: 6529 2021 3d20 3020 616e 6420 616e 6472  e) != 0 and andr
+0000da10: 6f69 645f 6669 6c65 2021 3d20 2222 2061  oid_file != "" a
+0000da20: 6e64 2073 656c 662e 6c69 7374 5f66 696c  nd self.list_fil
+0000da30: 6573 203d 3d20 4661 6c73 653a 0a20 2020  es == False:.   
+0000da40: 2020 2020 2072 6574 7572 6e5f 636f 6465       return_code
+0000da50: 2c20 6669 6c65 5f63 6f6e 7465 6e74 7320  , file_contents 
+0000da60: 3d20 6874 7470 5f72 6571 7565 7374 2861  = http_request(a
+0000da70: 6e64 726f 6964 5f69 7061 6464 722c 2061  ndroid_ipaddr, a
+0000da80: 6e64 726f 6964 5f70 6f72 742c 2061 6e64  ndroid_port, and
+0000da90: 726f 6964 5f66 696c 652c 2022 6669 6c65  roid_file, "file
+0000daa0: 222c 2022 3f64 6f77 6e6c 6f61 643d 3122  ", "?download=1"
+0000dab0: 290a 0a20 2020 2020 2020 2023 2056 616c  )..        # Val
+0000dac0: 6964 6174 6520 584d 4c20 6669 6c65 2e0a  idate XML file..
+0000dad0: 2020 2020 2020 2020 6966 2072 6574 7572          if retur
+0000dae0: 6e5f 636f 6465 203d 3d20 303a 0a20 2020  n_code == 0:.   
+0000daf0: 2020 2020 2020 2020 2050 7269 6d65 4974           PrimeIt
+0000db00: 656d 732e 7072 6f67 7261 6d5f 6172 6775  ems.program_argu
+0000db10: 6d65 6e74 735b 2267 7569 225d 203d 2054  ments["gui"] = T
+0000db20: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0000db30: 7265 7475 726e 5f63 6f64 652c 2065 7272  return_code, err
+0000db40: 6f72 5f6d 6573 7361 6765 203d 2076 616c  or_message = val
+0000db50: 6964 6174 655f 786d 6c5f 6669 6c65 2861  idate_xml_file(a
+0000db60: 6e64 726f 6964 5f69 7061 6464 722c 2061  ndroid_ipaddr, a
+0000db70: 6e64 726f 6964 5f70 6f72 742c 2061 6e64  ndroid_port, and
+0000db80: 726f 6964 5f66 696c 6529 0a20 2020 2020  roid_file).     
+0000db90: 2020 2020 2020 2069 6620 7265 7475 726e         if return
+0000dba0: 5f63 6f64 6520 213d 2030 3a0a 2020 2020  _code != 0:.    
+0000dbb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000dbc0: 2e64 6973 706c 6179 5f6d 6573 7361 6765  .display_message
+0000dbd0: 5f62 6f78 2865 7272 6f72 5f6d 6573 7361  _box(error_messa
+0000dbe0: 6765 2c20 2252 6564 2229 0a20 2020 2020  ge, "Red").     
+0000dbf0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000dc00: 6e20 312c 2061 6e64 726f 6964 5f69 7061  n 1, android_ipa
+0000dc10: 6464 722c 2061 6e64 726f 6964 5f70 6f72  ddr, android_por
+0000dc20: 742c 2061 6e64 726f 6964 5f66 696c 650a  t, android_file.
+0000dc30: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000dc40: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000dc50: 2031 2c20 616e 6472 6f69 645f 6970 6164   1, android_ipad
+0000dc60: 6472 2c20 616e 6472 6f69 645f 706f 7274  dr, android_port
+0000dc70: 2c20 616e 6472 6f69 645f 6669 6c65 0a0a  , android_file..
+0000dc80: 2020 2020 2320 4669 6c65 206c 6f63 6174      # File locat
+0000dc90: 696f 6e20 6e6f 7420 7072 6f76 6964 6564  ion not provided
+0000dca0: 2e20 2047 6574 2074 6865 206c 6973 7420  .  Get the list 
+0000dcb0: 6f66 2061 6c6c 2058 4d4c 2066 696c 6573  of all XML files
+0000dcc0: 2066 726f 6d20 7468 6520 416e 6472 6f69   from the Androi
+0000dcd0: 6420 6465 7669 6365 2061 6e64 2070 7265  d device and pre
+0000dce0: 7365 6e74 2069 7420 746f 2074 6865 2075  sent it to the u
+0000dcf0: 7365 722e 0a20 2020 2065 6c73 653a 0a20  ser..    else:. 
+0000dd00: 2020 2020 2020 2063 6c65 6172 5f61 6e64         clear_and
+0000dd10: 726f 6964 5f62 7574 746f 6e73 2873 656c  roid_buttons(sel
+0000dd20: 6629 0a20 2020 2020 2020 2023 2047 6574  f).        # Get
+0000dd30: 206c 6973 7420 6672 6f6d 2054 6173 6b65   list from Taske
+0000dd40: 7220 6469 7265 6374 6f72 7920 282f 5461  r directory (/Ta
+0000dd50: 736b 6572 2920 6f72 2073 7973 7465 6d20  sker) or system 
+0000dd60: 6469 7265 6374 6f72 7920 282f 7374 6f72  directory (/stor
+0000dd70: 6167 652f 656d 756c 6174 6564 2f30 290a  age/emulated/0).
+0000dd80: 2020 2020 2020 2020 7265 7475 726e 5f63          return_c
+0000dd90: 6f64 652c 2066 696c 656c 6973 7420 3d20  ode, filelist = 
+0000dda0: 6765 745f 6c69 7374 5f6f 665f 6669 6c65  get_list_of_file
+0000ddb0: 7328 616e 6472 6f69 645f 6970 6164 6472  s(android_ipaddr
+0000ddc0: 2c20 616e 6472 6f69 645f 706f 7274 2c20  , android_port, 
+0000ddd0: 222f 7374 6f72 6167 652f 656d 756c 6174  "/storage/emulat
+0000dde0: 6564 2f30 2f54 6173 6b65 7222 290a 2020  ed/0/Tasker").  
+0000ddf0: 2020 2020 2020 6966 2072 6574 7572 6e5f        if return_
+0000de00: 636f 6465 2021 3d20 303a 0a20 2020 2020  code != 0:.     
+0000de10: 2020 2020 2020 2023 2045 7272 6f72 2067         # Error g
+0000de20: 6574 7469 6e67 206c 6973 7420 6f66 2066  etting list of f
+0000de30: 696c 6573 2e0a 2020 2020 2020 2020 2020  iles..          
+0000de40: 2020 7365 6c66 2e64 6973 706c 6179 5f6d    self.display_m
+0000de50: 6573 7361 6765 5f62 6f78 2866 696c 656c  essage_box(filel
+0000de60: 6973 742c 2022 5265 6422 290a 2020 2020  ist, "Red").    
+0000de70: 2020 2020 2020 2020 7265 7475 726e 2031          return 1
+0000de80: 2c20 616e 6472 6f69 645f 6970 6164 6472  , android_ipaddr
+0000de90: 2c20 616e 6472 6f69 645f 706f 7274 2c20  , android_port, 
+0000dea0: 616e 6472 6f69 645f 6669 6c65 0a0a 2020  android_file..  
+0000deb0: 2020 2020 2020 2320 4469 7370 6c61 7920        # Display 
+0000dec0: 4669 6c65 204c 6973 7420 666f 7220 6669  File List for fi
+0000ded0: 6c65 2073 656c 6563 7469 6f6e 0a20 2020  le selection.   
+0000dee0: 2020 2020 2073 656c 662e 6669 6c65 6c69       self.fileli
+0000def0: 7374 5f6c 6162 656c 203d 2061 6464 5f6c  st_label = add_l
+0000df00: 6162 656c 280a 2020 2020 2020 2020 2020  abel(.          
+0000df10: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000df20: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000df30: 2020 2020 2020 2253 656c 6563 7420 584d        "Select XM
+0000df40: 4c20 4669 6c65 2046 726f 6d20 416e 6472  L File From Andr
+0000df50: 6f69 6420 4465 7669 6365 3a22 2c0a 2020  oid Device:",.  
+0000df60: 2020 2020 2020 2020 2020 2222 2c0a 2020            "",.  
+0000df70: 2020 2020 2020 2020 2020 302c 0a20 2020            0,.   
+0000df80: 2020 2020 2020 2020 2022 6e6f 726d 616c           "normal
+0000df90: 222c 0a20 2020 2020 2020 2020 2020 2038  ",.            8
+0000dfa0: 2c0a 2020 2020 2020 2020 2020 2020 312c  ,.            1,
+0000dfb0: 0a20 2020 2020 2020 2020 2020 2028 3138  .            (18
+0000dfc0: 352c 2030 292c 0a20 2020 2020 2020 2020  5, 0),.         
+0000dfd0: 2020 2028 302c 2031 3029 2c0a 2020 2020     (0, 10),.    
+0000dfe0: 2020 2020 2020 2020 2273 7722 2c0a 2020          "sw",.  
+0000dff0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000e000: 7365 6c66 2e66 696c 656c 6973 745f 6f70  self.filelist_op
+0000e010: 7469 6f6e 203d 2061 6464 5f6f 7074 696f  tion = add_optio
+0000e020: 6e5f 6d65 6e75 280a 2020 2020 2020 2020  n_menu(.        
+0000e030: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000e040: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000e050: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
+0000e060: 655f 7365 6c65 6374 6564 5f65 7665 6e74  e_selected_event
+0000e070: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
+0000e080: 6c65 6c69 7374 2c0a 2020 2020 2020 2020  lelist,.        
+0000e090: 2020 2020 392c 0a20 2020 2020 2020 2020      9,.         
+0000e0a0: 2020 2031 2c0a 2020 2020 2020 2020 2020     1,.          
+0000e0b0: 2020 2831 3835 2c20 3130 292c 0a20 2020    (185, 10),.   
+0000e0c0: 2020 2020 2020 2020 2028 302c 2031 3029           (0, 10)
+0000e0d0: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+0000e0e0: 7722 2c0a 2020 2020 2020 2020 290a 0a20  w",.        ).. 
+0000e0f0: 2020 2020 2020 2023 2053 6574 2062 6163         # Set bac
+0000e100: 6b75 7020 4950 2061 6e64 2066 696c 6520  kup IP and file 
+0000e110: 6c6f 6361 7469 6f6e 2061 7474 7269 6275  location attribu
+0000e120: 7465 7320 6966 2076 616c 6964 0a20 2020  tes if valid.   
+0000e130: 2020 2020 2073 656c 662e 616e 6472 6f69       self.androi
+0000e140: 645f 6970 6164 6472 203d 2061 6e64 726f  d_ipaddr = andro
+0000e150: 6964 5f69 7061 6464 720a 2020 2020 2020  id_ipaddr.      
+0000e160: 2020 7365 6c66 2e61 6e64 726f 6964 5f70    self.android_p
+0000e170: 6f72 7420 3d20 616e 6472 6f69 645f 706f  ort = android_po
+0000e180: 7274 0a20 2020 2020 2020 2072 6574 7572  rt.        retur
+0000e190: 6e20 322c 2022 222c 2022 222c 2022 2220  n 2, "", "", "" 
+0000e1a0: 2023 204a 7573 7420 7265 7475 726e 2077   # Just return w
+0000e1b0: 6974 6820 6572 726f 7220 736f 2074 6865  ith error so the
+0000e1c0: 2070 726f 6d70 7420 636f 6d65 7320 7570   prompt comes up
+0000e1d0: 2074 6f20 7365 6c65 6374 2066 696c 652e   to select file.
+0000e1e0: 0a0a 2020 2020 2320 416c 6c20 6973 206f  ..    # All is o
+0000e1f0: 6b61 790a 2020 2020 7265 7475 726e 2030  kay.    return 0
+0000e200: 2c20 616e 6472 6f69 645f 6970 6164 6472  , android_ipaddr
+0000e210: 2c20 616e 6472 6f69 645f 706f 7274 2c20  , android_port, 
+0000e220: 616e 6472 6f69 645f 6669 6c65 0a0a 0a23  android_file...#
+0000e230: 2041 6464 2070 756c 6c64 6f77 6e20 6d65   Add pulldown me
+0000e240: 6e75 7320 666f 7220 7468 6520 5072 6f6a  nus for the Proj
+0000e250: 6563 7473 2f50 726f 6669 6c65 732f 5461  ects/Profiles/Ta
+0000e260: 736b 7320 666f 7220 7365 6c65 6374 696f  sks for selectio
+0000e270: 6e0a 6465 6620 6469 7370 6c61 795f 6f62  n.def display_ob
+0000e280: 6a65 6374 5f70 756c 6c64 6f77 6e73 280a  ject_pulldowns(.
+0000e290: 2020 2020 7365 6c66 2c20 2023 206e 6f71      self,  # noq
+0000e2a0: 613a 2041 4e4e 3030 310a 2020 2020 6672  a: ANN001.    fr
+0000e2b0: 616d 653a 2063 746b 2e43 546b 4672 616d  ame: ctk.CTkFram
+0000e2c0: 652c 0a20 2020 2072 6f77 3a20 696e 742c  e,.    row: int,
+0000e2d0: 0a20 2020 2070 726f 6a65 6374 735f 746f  .    projects_to
+0000e2e0: 5f64 6973 706c 6179 3a20 6c69 7374 2c0a  _display: list,.
+0000e2f0: 2020 2020 7072 6f66 696c 6573 5f74 6f5f      profiles_to_
+0000e300: 6469 7370 6c61 793a 206c 6973 742c 0a20  display: list,. 
+0000e310: 2020 2074 6173 6b73 5f74 6f5f 6469 7370     tasks_to_disp
+0000e320: 6c61 793a 206c 6973 742c 0a20 2020 2070  lay: list,.    p
+0000e330: 726f 6a65 6374 5f6e 616d 655f 6576 656e  roject_name_even
+0000e340: 743a 2043 616c 6c61 626c 652c 0a20 2020  t: Callable,.   
+0000e350: 2070 726f 6669 6c65 5f6e 616d 655f 6576   profile_name_ev
+0000e360: 656e 743a 2043 616c 6c61 626c 652c 0a20  ent: Callable,. 
+0000e370: 2020 2074 6173 6b5f 6e61 6d65 5f65 7665     task_name_eve
+0000e380: 6e74 3a20 4361 6c6c 6162 6c65 2c0a 2920  nt: Callable,.) 
+0000e390: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+0000e3a0: 0a20 2020 2044 6973 706c 6179 7320 7468  .    Displays th
+0000e3b0: 6520 7075 6c6c 646f 776e 206d 656e 7573  e pulldown menus
+0000e3c0: 2066 6f72 2073 656c 6563 7469 6e67 2070   for selecting p
+0000e3d0: 726f 6669 6c65 7320 616e 6420 7461 736b  rofiles and task
+0000e3e0: 732e 0a0a 2020 2020 5061 7261 6d65 7465  s...    Paramete
+0000e3f0: 7273 3a0a 2020 2020 2020 2020 6672 616d  rs:.        fram
+0000e400: 6520 2863 746b 2e43 546b 4672 616d 6529  e (ctk.CTkFrame)
+0000e410: 3a20 5468 6520 6672 616d 6520 746f 2064  : The frame to d
+0000e420: 6973 706c 6179 2074 6865 2070 756c 6c64  isplay the pulld
+0000e430: 6f77 6e20 6d65 6e75 7320 696e 2e0a 2020  own menus in..  
+0000e440: 2020 2020 2020 726f 7720 2869 6e74 293a        row (int):
+0000e450: 2054 6865 2072 6f77 206e 756d 6265 7220   The row number 
+0000e460: 746f 2073 7461 7274 2064 6973 706c 6179  to start display
+0000e470: 696e 6720 7468 6520 7075 6c6c 646f 776e  ing the pulldown
+0000e480: 206d 656e 7573 2e0a 2020 2020 2020 2020   menus..        
+0000e490: 7072 6f6a 6563 7473 5f74 6f5f 6469 7370  projects_to_disp
+0000e4a0: 6c61 7920 286c 6973 7429 3a20 5468 6520  lay (list): The 
+0000e4b0: 6c69 7374 206f 6620 7072 6f6a 6563 7473  list of projects
+0000e4c0: 2074 6f20 6469 7370 6c61 7920 696e 2074   to display in t
+0000e4d0: 6865 2070 726f 6a65 6374 7320 7075 6c6c  he projects pull
+0000e4e0: 646f 776e 206d 656e 752e 0a20 2020 2020  down menu..     
+0000e4f0: 2020 2070 726f 6669 6c65 735f 746f 5f64     profiles_to_d
+0000e500: 6973 706c 6179 2028 6c69 7374 293a 2054  isplay (list): T
+0000e510: 6865 206c 6973 7420 6f66 2070 726f 6669  he list of profi
+0000e520: 6c65 7320 746f 2064 6973 706c 6179 2069  les to display i
+0000e530: 6e20 7468 6520 7072 6f66 696c 6573 2070  n the profiles p
+0000e540: 756c 6c64 6f77 6e20 6d65 6e75 2e0a 2020  ulldown menu..  
+0000e550: 2020 2020 2020 7461 736b 735f 746f 5f64        tasks_to_d
+0000e560: 6973 706c 6179 2028 6c69 7374 293a 2054  isplay (list): T
+0000e570: 6865 206c 6973 7420 6f66 2074 6173 6b73  he list of tasks
+0000e580: 2074 6f20 6469 7370 6c61 7920 696e 2074   to display in t
+0000e590: 6865 2074 6173 6b73 2070 756c 6c64 6f77  he tasks pulldow
+0000e5a0: 6e20 6d65 6e75 2e0a 2020 2020 2020 2020  n menu..        
+0000e5b0: 7072 6f6a 6563 745f 6e61 6d65 5f65 7665  project_name_eve
+0000e5c0: 6e74 2028 6f62 6a65 6374 293a 2054 6865  nt (object): The
+0000e5d0: 2065 7665 6e74 2074 6f20 7472 6967 6765   event to trigge
+0000e5e0: 7220 7768 656e 2061 2070 726f 6a65 6374  r when a project
+0000e5f0: 2069 7320 7365 6c65 6374 6564 2e0a 2020   is selected..  
+0000e600: 2020 2020 2020 7072 6f66 696c 655f 6e61        profile_na
+0000e610: 6d65 5f65 7665 6e74 2028 6f62 6a65 6374  me_event (object
+0000e620: 293a 2054 6865 2065 7665 6e74 2074 6f20  ): The event to 
+0000e630: 7472 6967 6765 7220 7768 656e 2061 2070  trigger when a p
+0000e640: 726f 6669 6c65 2069 7320 7365 6c65 6374  rofile is select
+0000e650: 6564 2e0a 2020 2020 2020 2020 7461 736b  ed..        task
+0000e660: 5f6e 616d 655f 6576 656e 7420 286f 626a  _name_event (obj
+0000e670: 6563 7429 3a20 5468 6520 6576 656e 7420  ect): The event 
+0000e680: 746f 2074 7269 6767 6572 2077 6865 6e20  to trigger when 
+0000e690: 6120 7461 736b 2069 7320 7365 6c65 6374  a task is select
+0000e6a0: 6564 2e0a 0a20 2020 2052 6574 7572 6e73  ed...    Returns
+0000e6b0: 3a0a 2020 2020 2020 2020 4e6f 6e65 0a20  :.        None. 
+0000e6c0: 2020 2022 2222 0a20 2020 2023 2044 6973     """.    # Dis
+0000e6d0: 706c 6179 2061 6c6c 206f 6620 7468 6520  play all of the 
+0000e6e0: 5072 6f6a 6563 7473 2066 6f72 2073 656c  Projects for sel
+0000e6f0: 6563 7469 6f6e 2e0a 2020 2020 6966 2070  ection..    if p
+0000e700: 726f 6a65 6374 735f 746f 5f64 6973 706c  rojects_to_displ
+0000e710: 6179 3a0a 2020 2020 2020 2020 7072 6f66  ay:.        prof
+0000e720: 696c 655f 726f 7720 3d20 726f 7720 2b20  ile_row = row + 
+0000e730: 320a 2020 2020 2020 2020 7461 736b 5f72  2.        task_r
+0000e740: 6f77 203d 2072 6f77 202b 2034 0a20 2020  ow = row + 4.   
+0000e750: 2020 2020 2073 656c 662e 7072 6f6a 6563       self.projec
+0000e760: 745f 6c61 6265 6c20 3d20 6164 645f 6c61  t_label = add_la
+0000e770: 6265 6c28 0a20 2020 2020 2020 2020 2020  bel(.           
+0000e780: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+0000e790: 2020 2066 7261 6d65 2c0a 2020 2020 2020     frame,.      
+0000e7a0: 2020 2020 2020 2253 656c 6563 7420 5072        "Select Pr
+0000e7b0: 6f6a 6563 7420 746f 2070 726f 6365 7373  oject to process
+0000e7c0: 3a22 2c0a 2020 2020 2020 2020 2020 2020  :",.            
+0000e7d0: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+0000e7e0: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+0000e7f0: 6e6f 726d 616c 222c 0a20 2020 2020 2020  normal",.       
+0000e800: 2020 2020 2072 6f77 2c20 2023 2072 6f77       row,  # row
+0000e810: 202b 2033 2c0a 2020 2020 2020 2020 2020   + 3,.          
+0000e820: 2020 302c 0a20 2020 2020 2020 2020 2020    0,.           
+0000e830: 2032 302c 0a20 2020 2020 2020 2020 2020   20,.           
+0000e840: 2028 3230 2c20 3029 2c0a 2020 2020 2020   (20, 0),.      
+0000e850: 2020 2020 2020 2273 222c 0a20 2020 2020        "s",.     
+0000e860: 2020 2029 0a20 2020 2020 2020 2023 2047     ).        # G
+0000e870: 6574 2074 6865 2070 726f 6669 6c65 2064  et the profile d
+0000e880: 6573 6972 6564 0a20 2020 2020 2020 2073  esired.        s
+0000e890: 656c 662e 7370 6563 6966 6963 5f70 726f  elf.specific_pro
+0000e8a0: 6a65 6374 5f6f 7074 696f 6e6d 656e 7520  ject_optionmenu 
+0000e8b0: 3d20 6164 645f 6f70 7469 6f6e 5f6d 656e  = add_option_men
+0000e8c0: 7528 0a20 2020 2020 2020 2020 2020 2073  u(.            s
+0000e8d0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000e8e0: 2066 7261 6d65 2c0a 2020 2020 2020 2020   frame,.        
+0000e8f0: 2020 2020 7072 6f6a 6563 745f 6e61 6d65      project_name
+0000e900: 5f65 7665 6e74 2c0a 2020 2020 2020 2020  _event,.        
+0000e910: 2020 2020 7072 6f6a 6563 7473 5f74 6f5f      projects_to_
+0000e920: 6469 7370 6c61 792c 0a20 2020 2020 2020  display,.       
+0000e930: 2020 2020 2072 6f77 202b 2031 2c20 2023       row + 1,  #
+0000e940: 2072 6f77 202b 2034 2c0a 2020 2020 2020   row + 4,.      
+0000e950: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
+0000e960: 2020 2020 2032 302c 0a20 2020 2020 2020       20,.       
+0000e970: 2020 2020 2028 302c 2031 3029 2c0a 2020       (0, 10),.  
+0000e980: 2020 2020 2020 2020 2020 226e 222c 0a20            "n",. 
+0000e990: 2020 2020 2020 2029 0a0a 2020 2020 2320         )..    # 
+0000e9a0: 4a75 7374 2064 6f69 6e67 2050 726f 6669  Just doing Profi
+0000e9b0: 6c65 2061 6e64 2054 6173 6b20 7075 6c6c  le and Task pull
+0000e9c0: 646f 776e 0a20 2020 2065 6c73 653a 0a20  down.    else:. 
+0000e9d0: 2020 2020 2020 2070 726f 6669 6c65 5f72         profile_r
+0000e9e0: 6f77 203d 2072 6f77 0a20 2020 2020 2020  ow = row.       
+0000e9f0: 2074 6173 6b5f 726f 7720 3d20 726f 7720   task_row = row 
+0000ea00: 2b20 320a 0a20 2020 2023 2044 6973 706c  + 2..    # Displ
+0000ea10: 6179 2061 6c6c 206f 6620 7468 6520 5072  ay all of the Pr
+0000ea20: 6f66 696c 6573 2066 6f72 2073 656c 6563  ofiles for selec
+0000ea30: 7469 6f6e 2e0a 2020 2020 7365 6c66 2e70  tion..    self.p
+0000ea40: 726f 6669 6c65 5f6c 6162 656c 203d 2061  rofile_label = a
+0000ea50: 6464 5f6c 6162 656c 280a 2020 2020 2020  dd_label(.      
+0000ea60: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000ea70: 6672 616d 652c 0a20 2020 2020 2020 2022  frame,.        "
+0000ea80: 5365 6c65 6374 2050 726f 6669 6c65 2074  Select Profile t
+0000ea90: 6f20 7072 6f63 6573 733a 222c 0a20 2020  o process:",.   
+0000eaa0: 2020 2020 2022 222c 0a20 2020 2020 2020       "",.       
+0000eab0: 2030 2c0a 2020 2020 2020 2020 226e 6f72   0,.        "nor
+0000eac0: 6d61 6c22 2c0a 2020 2020 2020 2020 7072  mal",.        pr
+0000ead0: 6f66 696c 655f 726f 772c 0a20 2020 2020  ofile_row,.     
+0000eae0: 2020 2030 2c0a 2020 2020 2020 2020 3230     0,.        20
+0000eaf0: 2c0a 2020 2020 2020 2020 2832 302c 2030  ,.        (20, 0
+0000eb00: 292c 0a20 2020 2020 2020 2022 7322 2c0a  ),.        "s",.
+0000eb10: 2020 2020 290a 2020 2020 2320 4765 7420      ).    # Get 
+0000eb20: 7468 6520 7072 6f66 696c 6520 6465 7369  the profile desi
+0000eb30: 7265 640a 2020 2020 7072 6f66 696c 655f  red.    profile_
+0000eb40: 6f70 7469 6f6e 203d 2061 6464 5f6f 7074  option = add_opt
+0000eb50: 696f 6e5f 6d65 6e75 280a 2020 2020 2020  ion_menu(.      
+0000eb60: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000eb70: 6672 616d 652c 0a20 2020 2020 2020 2070  frame,.        p
+0000eb80: 726f 6669 6c65 5f6e 616d 655f 6576 656e  rofile_name_even
+0000eb90: 742c 0a20 2020 2020 2020 2070 726f 6669  t,.        profi
+0000eba0: 6c65 735f 746f 5f64 6973 706c 6179 2c0a  les_to_display,.
+0000ebb0: 2020 2020 2020 2020 7072 6f66 696c 655f          profile_
+0000ebc0: 726f 7720 2b20 312c 0a20 2020 2020 2020  row + 1,.       
+0000ebd0: 2030 2c0a 2020 2020 2020 2020 3230 2c0a   0,.        20,.
+0000ebe0: 2020 2020 2020 2020 2830 2c20 3130 292c          (0, 10),
+0000ebf0: 0a20 2020 2020 2020 2022 6e22 2c0a 2020  .        "n",.  
+0000ec00: 2020 290a 0a20 2020 2023 2044 6973 706c    )..    # Displ
+0000ec10: 6179 2061 6c6c 206f 6620 7468 6520 5461  ay all of the Ta
+0000ec20: 736b 7320 666f 7220 7365 6c65 6374 696f  sks for selectio
+0000ec30: 6e2e 0a20 2020 2073 656c 662e 7461 736b  n..    self.task
+0000ec40: 5f6c 6162 656c 203d 2061 6464 5f6c 6162  _label = add_lab
+0000ec50: 656c 280a 2020 2020 2020 2020 7365 6c66  el(.        self
+0000ec60: 2c0a 2020 2020 2020 2020 6672 616d 652c  ,.        frame,
+0000ec70: 0a20 2020 2020 2020 2022 5365 6c65 6374  .        "Select
+0000ec80: 2054 6173 6b20 746f 2070 726f 6365 7373   Task to process
+0000ec90: 3a22 2c0a 2020 2020 2020 2020 2222 2c0a  :",.        "",.
+0000eca0: 2020 2020 2020 2020 302c 0a20 2020 2020          0,.     
+0000ecb0: 2020 2022 6e6f 726d 616c 222c 0a20 2020     "normal",.   
+0000ecc0: 2020 2020 2074 6173 6b5f 726f 772c 0a20       task_row,. 
+0000ecd0: 2020 2020 2020 2030 2c0a 2020 2020 2020         0,.      
+0000ece0: 2020 3230 2c0a 2020 2020 2020 2020 2830    20,.        (0
+0000ecf0: 2c20 3029 2c0a 2020 2020 2020 2020 226e  , 0),.        "n
+0000ed00: 222c 0a20 2020 2029 0a20 2020 2023 2047  ",.    ).    # G
+0000ed10: 6574 2074 6865 2070 726f 6a65 6374 2064  et the project d
+0000ed20: 6573 6972 6564 0a20 2020 2074 6173 6b5f  esired.    task_
+0000ed30: 6f70 7469 6f6e 203d 2061 6464 5f6f 7074  option = add_opt
+0000ed40: 696f 6e5f 6d65 6e75 280a 2020 2020 2020  ion_menu(.      
+0000ed50: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000ed60: 6672 616d 652c 0a20 2020 2020 2020 2074  frame,.        t
+0000ed70: 6173 6b5f 6e61 6d65 5f65 7665 6e74 2c0a  ask_name_event,.
+0000ed80: 2020 2020 2020 2020 7461 736b 735f 746f          tasks_to
+0000ed90: 5f64 6973 706c 6179 2c0a 2020 2020 2020  _display,.      
+0000eda0: 2020 7461 736b 5f72 6f77 2c0a 2020 2020    task_row,.    
+0000edb0: 2020 2020 302c 0a20 2020 2020 2020 2032      0,.        2
+0000edc0: 302c 0a20 2020 2020 2020 2028 3330 2c20  0,.        (30, 
+0000edd0: 3029 2c0a 2020 2020 2020 2020 2273 222c  0),.        "s",
+0000ede0: 0a20 2020 2029 0a20 2020 2072 6574 7572  .    ).    retur
+0000edf0: 6e20 7072 6f66 696c 655f 6f70 7469 6f6e  n profile_option
+0000ee00: 2c20 7461 736b 5f6f 7074 696f 6e0a 0a0a  , task_option...
+0000ee10: 2320 4465 6c65 7465 206f 6c64 2070 756c  # Delete old pul
+0000ee20: 6c64 6f77 6e20 6d65 6e75 7320 7369 6e63  ldown menus sinc
+0000ee30: 6520 7468 6520 6f6c 6465 7220 7365 6c65  e the older sele
+0000ee40: 6374 6564 2069 7465 6d73 2063 6f75 6c64  cted items could
+0000ee50: 2062 6520 6c6f 6e67 6572 2074 6861 6e20   be longer than 
+0000ee60: 7468 6520 6e65 772c 0a23 2061 6e64 2062  the new,.# and b
+0000ee70: 6f74 6820 7769 6c6c 2061 7070 6561 722e  oth will appear.
+0000ee80: 0a64 6566 2064 656c 6574 655f 6f6c 645f  .def delete_old_
+0000ee90: 7075 6c6c 646f 776e 5f6d 656e 7573 2873  pulldown_menus(s
+0000eea0: 656c 6629 202d 3e20 4e6f 6e65 3a20 2023  elf) -> None:  #
+0000eeb0: 206e 6f71 613a 2041 4e4e 3030 310a 2020   noqa: ANN001.  
+0000eec0: 2020 2222 220a 2020 2020 4465 6c65 7465    """.    Delete
+0000eed0: 7320 7468 6520 6f6c 6420 7075 6c6c 646f  s the old pulldo
+0000eee0: 776e 206d 656e 7573 2e0a 0a20 2020 2054  wn menus...    T
+0000eef0: 6869 7320 6675 6e63 7469 6f6e 2064 656c  his function del
+0000ef00: 6574 6573 2074 6865 206f 6c64 2070 756c  etes the old pul
+0000ef10: 6c64 6f77 6e20 6d65 6e75 7320 7468 6174  ldown menus that
+0000ef20: 2077 6572 6520 6372 6561 7465 6420 696e   were created in
+0000ef30: 2074 6865 2047 5549 2e20 4974 2063 6865   the GUI. It che
+0000ef40: 636b 7320 6966 2065 6163 6820 6d65 6e75  cks if each menu
+0000ef50: 2065 7869 7374 7320 616e 6420 7468 656e   exists and then
+0000ef60: 2064 6573 7472 6f79 7320 6974 2e0a 0a20   destroys it... 
+0000ef70: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
+0000ef80: 2020 2020 2020 2073 656c 6620 286f 626a         self (obj
+0000ef90: 6563 7429 3a20 5468 6520 6375 7272 656e  ect): The curren
+0000efa0: 7420 696e 7374 616e 6365 206f 6620 7468  t instance of th
+0000efb0: 6520 636c 6173 732e 0a0a 2020 2020 5265  e class...    Re
+0000efc0: 7475 726e 733a 0a20 2020 2020 2020 204e  turns:.        N
+0000efd0: 6f6e 650a 2020 2020 2222 220a 2020 2020  one.    """.    
+0000efe0: 7769 7468 2063 6f6e 7465 7874 6c69 622e  with contextlib.
+0000eff0: 7375 7070 7265 7373 2841 7474 7269 6275  suppress(Attribu
+0000f000: 7465 4572 726f 7229 3a0a 2020 2020 2020  teError):.      
+0000f010: 2020 7365 6c66 2e73 7065 6369 6669 635f    self.specific_
+0000f020: 7072 6f6a 6563 745f 6f70 7469 6f6e 6d65  project_optionme
+0000f030: 6e75 2e64 6573 7472 6f79 2829 0a20 2020  nu.destroy().   
+0000f040: 2077 6974 6820 636f 6e74 6578 746c 6962   with contextlib
+0000f050: 2e73 7570 7072 6573 7328 4174 7472 6962  .suppress(Attrib
+0000f060: 7574 6545 7272 6f72 293a 0a20 2020 2020  uteError):.     
+0000f070: 2020 2073 656c 662e 7370 6563 6966 6963     self.specific
+0000f080: 5f70 726f 6669 6c65 5f6f 7074 696f 6e6d  _profile_optionm
+0000f090: 656e 752e 6465 7374 726f 7928 290a 2020  enu.destroy().  
+0000f0a0: 2020 7769 7468 2063 6f6e 7465 7874 6c69    with contextli
+0000f0b0: 622e 7375 7070 7265 7373 2841 7474 7269  b.suppress(Attri
+0000f0c0: 6275 7465 4572 726f 7229 3a0a 2020 2020  buteError):.    
+0000f0d0: 2020 2020 7365 6c66 2e73 7065 6369 6669      self.specifi
+0000f0e0: 635f 7461 736b 5f6f 7074 696f 6e6d 656e  c_task_optionmen
+0000f0f0: 752e 6465 7374 726f 7928 290a 2020 2020  u.destroy().    
+0000f100: 7769 7468 2063 6f6e 7465 7874 6c69 622e  with contextlib.
+0000f110: 7375 7070 7265 7373 2841 7474 7269 6275  suppress(Attribu
+0000f120: 7465 4572 726f 7229 3a0a 2020 2020 2020  teError):.      
+0000f130: 2020 7365 6c66 2e61 695f 7072 6f66 696c    self.ai_profil
+0000f140: 655f 6f70 7469 6f6e 6d65 6e75 2e64 6573  e_optionmenu.des
+0000f150: 7472 6f79 2829 0a20 2020 2077 6974 6820  troy().    with 
+0000f160: 636f 6e74 6578 746c 6962 2e73 7570 7072  contextlib.suppr
+0000f170: 6573 7328 4174 7472 6962 7574 6545 7272  ess(AttributeErr
+0000f180: 6f72 293a 0a20 2020 2020 2020 2073 656c  or):.        sel
+0000f190: 662e 6169 5f74 6173 6b5f 6f70 7469 6f6e  f.ai_task_option
+0000f1a0: 6d65 6e75 2e64 6573 7472 6f79 2829 0a20  menu.destroy(). 
+0000f1b0: 2020 2077 6974 6820 636f 6e74 6578 746c     with contextl
+0000f1c0: 6962 2e73 7570 7072 6573 7328 4174 7472  ib.suppress(Attr
+0000f1d0: 6962 7574 6545 7272 6f72 293a 0a20 2020  ibuteError):.   
+0000f1e0: 2020 2020 2073 656c 662e 7369 6e67 6c65       self.single
+0000f1f0: 5f6c 6162 656c 2e64 6573 7472 6f79 2829  _label.destroy()
+0000f200: 0a0a 0a23 2050 726f 7669 6465 2061 2070  ...# Provide a p
+0000f210: 756c 6c64 6f77 6e20 6c69 7374 2066 6f72  ulldown list for
+0000f220: 2074 6865 2073 656c 6563 7469 6f6e 206f   the selection o
+0000f230: 6620 6120 5072 6f66 696c 6520 6e61 6d65  f a Profile name
+0000f240: 0a64 6566 206c 6973 745f 7461 736b 6572  .def list_tasker
+0000f250: 5f6f 626a 6563 7473 2873 656c 6629 202d  _objects(self) -
+0000f260: 3e20 626f 6f6c 3a20 2023 206e 6f71 613a  > bool:  # noqa:
+0000f270: 2041 4e4e 3030 310a 2020 2020 2222 220a   ANN001.    """.
+0000f280: 2020 2020 4c69 7374 7320 7468 6520 7072      Lists the pr
+0000f290: 6f6a 6563 7473 2c20 7072 6f66 696c 6573  ojects, profiles
+0000f2a0: 2061 6e64 2074 6173 6b73 2061 7661 696c   and tasks avail
+0000f2b0: 6162 6c65 2069 6e20 7468 6520 584d 4c20  able in the XML 
+0000f2c0: 6669 6c65 2e20 2054 6865 206c 6973 7420  file.  The list 
+0000f2d0: 666f 7220 6561 6368 2077 696c 6c20 6170  for each will ap
+0000f2e0: 7065 6172 2069 6e20 6120 7075 6c6c 646f  pear in a pulldo
+0000f2f0: 776e 206f 7074 696f 6e20 6c69 7374 2e0a  wn option list..
+0000f300: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
+0000f310: 6f6e 2063 6865 636b 7320 6966 2074 6865  on checks if the
+0000f320: 2058 4d4c 2066 696c 6520 6861 7320 616c   XML file has al
+0000f330: 7265 6164 7920 6265 656e 206c 6f61 6465  ready been loade
+0000f340: 642e 2049 6620 6e6f 742c 2069 7420 6c6f  d. If not, it lo
+0000f350: 6164 7320 7468 6520 584d 4c20 6669 6c65  ads the XML file
+0000f360: 2061 6e64 2062 7569 6c64 7320 7468 6520   and builds the 
+0000f370: 7472 6565 2064 6174 612e 0a20 2020 2054  tree data..    T
+0000f380: 6865 6e2c 2069 7420 676f 6573 2074 6872  hen, it goes thr
+0000f390: 6f75 6768 2065 6163 6820 7072 6f6a 6563  ough each projec
+0000f3a0: 7420 616e 6420 7265 7472 6965 7665 7320  t and retrieves 
+0000f3b0: 616c 6c20 7468 6520 7072 6f66 696c 6520  all the profile 
+0000f3c0: 6e61 6d65 7320 616e 6420 7461 736b 732e  names and tasks.
+0000f3d0: 0a20 2020 2054 6865 2070 726f 6669 6c65  .    The profile
+0000f3e0: 206e 616d 6573 2061 6e64 2074 6173 6b73   names and tasks
+0000f3f0: 2061 7265 2063 6c65 616e 6564 2075 7020   are cleaned up 
+0000f400: 6279 2072 656d 6f76 696e 6720 7468 6520  by removing the 
+0000f410: 2250 726f 6669 6c65 3a20 556e 6e61 6d65  "Profile: Unname
+0000f420: 642f 416e 6f6e 796d 6f75 7322 2061 6e64  d/Anonymous" and
+0000f430: 2022 5461 736b 3a20 556e 6e61 6d65 642f   "Task: Unnamed/
+0000f440: 416e 6f6e 796d 6f75 732e 2220 656e 7472  Anonymous." entr
+0000f450: 6965 732e 0a20 2020 2049 6620 7468 6572  ies..    If ther
+0000f460: 6520 6172 6520 6e6f 2070 726f 6669 6c65  e are no profile
+0000f470: 7320 6f72 2074 6173 6b73 2066 6f75 6e64  s or tasks found
+0000f480: 2c20 6120 6d65 7373 6167 6520 626f 7820  , a message box 
+0000f490: 6973 2064 6973 706c 6179 6564 2061 6e64  is displayed and
+0000f4a0: 2074 6865 2066 756e 6374 696f 6e20 7265   the function re
+0000f4b0: 7475 726e 7320 4661 6c73 652e 0a20 2020  turns False..   
+0000f4c0: 2054 6865 2070 726f 6669 6c65 206e 616d   The profile nam
+0000f4d0: 6573 2061 6e64 2074 6173 6b73 2061 7265  es and tasks are
+0000f4e0: 2074 6865 6e20 736f 7274 6564 2061 6c70   then sorted alp
+0000f4f0: 6861 6265 7469 6361 6c6c 7920 616e 6420  habetically and 
+0000f500: 6475 706c 6963 6174 6573 2061 7265 2072  duplicates are r
+0000f510: 656d 6f76 6564 2e0a 2020 2020 5468 6520  emoved..    The 
+0000f520: 7072 6f66 696c 6520 6e61 6d65 7320 6172  profile names ar
+0000f530: 6520 6469 7370 6c61 7965 6420 696e 2061  e displayed in a
+0000f540: 206c 6162 656c 2066 6f72 2073 656c 6563   label for selec
+0000f550: 7469 6f6e 2c20 616e 6420 7468 6520 636f  tion, and the co
+0000f560: 7272 6573 706f 6e64 696e 6720 7461 736b  rresponding task
+0000f570: 7320 6172 6520 6469 7370 6c61 7965 6420  s are displayed 
+0000f580: 696e 2061 6e6f 7468 6572 206c 6162 656c  in another label
+0000f590: 2066 6f72 2073 656c 6563 7469 6f6e 2e0a   for selection..
+0000f5a0: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+0000f5b0: 2020 2020 2020 626f 6f6c 3a20 5472 7565        bool: True
+0000f5c0: 2069 6620 7468 6520 584d 4c20 6669 6c65   if the XML file
+0000f5d0: 2068 6173 2050 726f 6669 6c65 7320 6f72   has Profiles or
+0000f5e0: 2054 6173 6b73 2c20 4661 6c73 6520 6f74   Tasks, False ot
+0000f5f0: 6865 7277 6973 652e 0a20 2020 2022 2222  herwise..    """
+0000f600: 0a0a 2020 2020 2320 446f 2077 6520 616c  ..    # Do we al
+0000f610: 7265 6164 7920 6861 7665 2074 6865 2058  ready have the X
+0000f620: 4d4c 3f0a 2020 2020 2320 4966 2077 6520  ML?.    # If we 
+0000f630: 646f 6e27 7420 6861 7665 2061 6e79 2064  don't have any d
+0000f640: 6174 612c 2067 6574 2069 742e 0a20 2020  ata, get it..   
+0000f650: 2069 6620 6e6f 7420 7365 6c66 2e6c 6f61   if not self.loa
+0000f660: 645f 786d 6c28 293a 0a20 2020 2020 2020  d_xml():.       
+0000f670: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+0000f680: 2020 2320 496e 7469 616c 697a 6520 6c69    # Intialize li
+0000f690: 7374 730a 2020 2020 7072 6f6a 6563 7473  sts.    projects
+0000f6a0: 203d 205b 5d0a 2020 2020 7072 6f66 696c   = [].    profil
+0000f6b0: 6573 203d 205b 5d0a 2020 2020 7461 736b  es = [].    task
+0000f6c0: 7320 3d20 5b5d 0a0a 2020 2020 2320 4765  s = []..    # Ge
+0000f6d0: 7420 7269 6420 6f66 2070 7265 7669 6f75  t rid of previou
+0000f6e0: 7320 6461 7461 0a20 2020 2064 656c 6574  s data.    delet
+0000f6f0: 655f 6f6c 645f 7075 6c6c 646f 776e 5f6d  e_old_pulldown_m
+0000f700: 656e 7573 2873 656c 6629 0a20 2020 2023  enus(self).    #
+0000f710: 2077 6974 6820 636f 6e74 6578 746c 6962   with contextlib
+0000f720: 2e73 7570 7072 6573 7328 4174 7472 6962  .suppress(Attrib
+0000f730: 7574 6545 7272 6f72 293a 0a20 2020 2023  uteError):.    #
+0000f740: 2020 2020 7365 6c66 2e61 695f 7072 6f66      self.ai_prof
+0000f750: 696c 655f 6f70 7469 6f6e 6d65 6e75 2e64  ile_optionmenu.d
+0000f760: 6573 7472 6f79 2829 0a0a 2020 2020 2320  estroy()..    # 
+0000f770: 4f6b 2c20 7765 2068 6176 6520 6f75 7220  Ok, we have our 
+0000f780: 726f 6f74 2054 6173 6b65 7220 656c 656d  root Tasker elem
+0000f790: 656e 7473 2e20 2042 7569 6c64 2074 6865  ents.  Build the
+0000f7a0: 2074 7265 652e 0a20 2020 2074 7265 655f   tree..    tree_
+0000f7b0: 6461 7461 203d 2073 656c 662e 6275 696c  data = self.buil
+0000f7c0: 645f 7468 655f 7472 6565 2829 0a20 2020  d_the_tree().   
+0000f7d0: 2023 2049 6620 6e6f 2074 7265 652c 2074   # If no tree, t
+0000f7e0: 6865 6e20 7468 6572 6520 6172 6520 6e6f  hen there are no
+0000f7f0: 2050 726f 6a65 6374 7320 696e 2074 6865   Projects in the
+0000f800: 2058 4d4c 2e0a 2020 2020 6966 206e 6f74   XML..    if not
+0000f810: 2074 7265 655f 6461 7461 3a0a 2020 2020   tree_data:.    
+0000f820: 2020 2020 6966 2050 7269 6d65 4974 656d      if PrimeItem
+0000f830: 732e 7461 736b 6572 5f72 6f6f 745f 656c  s.tasker_root_el
+0000f840: 656d 656e 7473 5b22 616c 6c5f 7072 6f66  ements["all_prof
+0000f850: 696c 6573 225d 3a0a 2020 2020 2020 2020  iles"]:.        
+0000f860: 2020 2020 7072 6f66 696c 6573 203d 205b      profiles = [
+0000f870: 7661 6c75 655b 226e 616d 6522 5d20 666f  value["name"] fo
+0000f880: 7220 7661 6c75 6520 696e 2050 7269 6d65  r value in Prime
+0000f890: 4974 656d 732e 7461 736b 6572 5f72 6f6f  Items.tasker_roo
+0000f8a0: 745f 656c 656d 656e 7473 5b22 616c 6c5f  t_elements["all_
+0000f8b0: 7072 6f66 696c 6573 225d 2e76 616c 7565  profiles"].value
+0000f8c0: 7328 295d 0a20 2020 2020 2020 2069 6620  s()].        if 
+0000f8d0: 5072 696d 6549 7465 6d73 2e74 6173 6b65  PrimeItems.taske
+0000f8e0: 725f 726f 6f74 5f65 6c65 6d65 6e74 735b  r_root_elements[
+0000f8f0: 2261 6c6c 5f74 6173 6b73 225d 3a0a 2020  "all_tasks"]:.  
+0000f900: 2020 2020 2020 2020 2020 7461 736b 7320            tasks 
+0000f910: 3d20 5b76 616c 7565 5b22 6e61 6d65 225d  = [value["name"]
+0000f920: 2066 6f72 2076 616c 7565 2069 6e20 5072   for value in Pr
+0000f930: 696d 6549 7465 6d73 2e74 6173 6b65 725f  imeItems.tasker_
+0000f940: 726f 6f74 5f65 6c65 6d65 6e74 735b 2261  root_elements["a
+0000f950: 6c6c 5f74 6173 6b73 225d 2e76 616c 7565  ll_tasks"].value
+0000f960: 7328 295d 0a0a 2020 2020 2320 5765 2068  s()]..    # We h
+0000f970: 6176 6520 6120 7472 6565 4275 696c 6420  ave a treeBuild 
+0000f980: 6f75 7220 6c69 7374 206f 6620 5072 6f66  our list of Prof
+0000f990: 696c 6573 2061 6e64 2054 6173 6b73 2069  iles and Tasks i
+0000f9a0: 6e20 7468 6520 5072 6f6a 6563 7473 2e0a  n the Projects..
+0000f9b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000f9c0: 2020 2320 476f 2074 6872 6f75 6768 2074    # Go through t
+0000f9d0: 6865 2050 726f 6a65 6374 7320 616e 6420  he Projects and 
+0000f9e0: 6765 7420 616c 6c20 6f66 2074 6865 2050  get all of the P
+0000f9f0: 726f 6669 6c65 206e 616d 6573 2e0a 2020  rofile names..  
+0000fa00: 2020 2020 2020 666f 7220 7072 6f6a 6563        for projec
+0000fa10: 7420 696e 2074 7265 655f 6461 7461 3a0a  t in tree_data:.
+0000fa20: 2020 2020 2020 2020 2020 2020 7072 6f6a              proj
+0000fa30: 6563 7473 2e61 7070 656e 6428 7072 6f6a  ects.append(proj
+0000fa40: 6563 745b 226e 616d 6522 5d29 0a20 2020  ect["name"]).   
+0000fa50: 2020 2020 2020 2020 2066 6f72 2070 726f           for pro
+0000fa60: 6669 6c65 2069 6e20 7072 6f6a 6563 745b  file in project[
+0000fa70: 2263 6869 6c64 7265 6e22 5d3a 0a20 2020  "children"]:.   
+0000fa80: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+0000fa90: 6820 636f 6e74 6578 746c 6962 2e73 7570  h contextlib.sup
+0000faa0: 7072 6573 7328 5479 7065 4572 726f 7229  press(TypeError)
+0000fab0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000fac0: 2020 2020 2020 7072 6f66 696c 6573 2e61        profiles.a
+0000fad0: 7070 656e 6428 7072 6f66 696c 655b 226e  ppend(profile["n
+0000fae0: 616d 6522 5d29 0a20 2020 2020 2020 2020  ame"]).         
+0000faf0: 2020 2020 2020 2020 2020 2074 6173 6b73             tasks
+0000fb00: 2e65 7874 656e 6428 7072 6f66 696c 655b  .extend(profile[
+0000fb10: 2263 6869 6c64 7265 6e22 5d29 0a0a 2020  "children"])..  
+0000fb20: 2020 2320 436c 6561 6e75 7020 7468 6520    # Cleanup the 
+0000fb30: 6c69 7374 730a 2020 2020 6861 7665 5f70  lists.    have_p
+0000fb40: 726f 6669 6c65 7320 3d20 6861 7665 5f74  rofiles = have_t
+0000fb50: 6173 6b73 203d 2054 7275 6520 2023 2041  asks = True  # A
+0000fb60: 7373 756d 6520 7765 2068 6176 6520 5072  ssume we have Pr
+0000fb70: 6f66 696c 6573 2061 6e64 2054 6173 6b73  ofiles and Tasks
+0000fb80: 0a20 2020 2070 726f 6669 6c65 735f 746f  .    profiles_to
+0000fb90: 5f64 6973 706c 6179 203d 205b 7072 6f66  _display = [prof
+0000fba0: 696c 6520 666f 7220 7072 6f66 696c 6520  ile for profile 
+0000fbb0: 696e 2070 726f 6669 6c65 7320 6966 2070  in profiles if p
+0000fbc0: 726f 6669 6c65 2021 3d20 2250 726f 6669  rofile != "Profi
+0000fbd0: 6c65 3a20 556e 6e61 6d65 642f 416e 6f6e  le: Unnamed/Anon
+0000fbe0: 796d 6f75 7322 5d0a 2020 2020 6966 206e  ymous"].    if n
+0000fbf0: 6f74 2070 726f 6669 6c65 735f 746f 5f64  ot profiles_to_d
+0000fc00: 6973 706c 6179 3a0a 2020 2020 2020 2020  isplay:.        
+0000fc10: 7072 6f66 696c 6573 5f74 6f5f 6469 7370  profiles_to_disp
+0000fc20: 6c61 7920 3d20 5b22 4e6f 2070 726f 6669  lay = ["No profi
+0000fc30: 6c65 7320 666f 756e 6422 5d0a 2020 2020  les found"].    
+0000fc40: 2020 2020 6861 7665 5f70 726f 6669 6c65      have_profile
+0000fc50: 7320 3d20 4661 6c73 650a 2020 2020 7461  s = False.    ta
+0000fc60: 736b 735f 746f 5f64 6973 706c 6179 203d  sks_to_display =
+0000fc70: 205b 7461 736b 2066 6f72 2074 6173 6b20   [task for task 
+0000fc80: 696e 2074 6173 6b73 2069 6620 7461 736b  in tasks if task
+0000fc90: 206e 6f74 2069 6e20 5b22 5461 736b 3a20   not in ["Task: 
+0000fca0: 556e 6e61 6d65 642f 416e 6f6e 796d 6f75  Unnamed/Anonymou
+0000fcb0: 732e 222c 2022 225d 5d0a 2020 2020 2320  s.", ""]].    # 
+0000fcc0: 436c 6561 6e75 7020 5461 736b 730a 2020  Cleanup Tasks.  
+0000fcd0: 2020 6966 206e 6f74 2074 6173 6b73 5f74    if not tasks_t
+0000fce0: 6f5f 6469 7370 6c61 793a 0a20 2020 2020  o_display:.     
+0000fcf0: 2020 2074 6173 6b73 5f74 6f5f 6469 7370     tasks_to_disp
+0000fd00: 6c61 7920 3d20 5b22 4e6f 2074 6173 6b73  lay = ["No tasks
+0000fd10: 2066 6f75 6e64 225d 0a20 2020 2020 2020   found"].       
+0000fd20: 2068 6176 655f 7461 736b 7320 3d20 4661   have_tasks = Fa
+0000fd30: 6c73 650a 2020 2020 656c 7365 3a0a 2020  lse.    else:.  
+0000fd40: 2020 2020 2020 2320 5265 6d6f 7665 2064        # Remove d
+0000fd50: 7570 7320 6672 6f6d 2054 6173 6b73 2061  ups from Tasks a
+0000fd60: 6e64 2073 6f72 7420 7468 656d 0a20 2020  nd sort them.   
+0000fd70: 2020 2020 2074 6173 6b73 5f74 6f5f 6469       tasks_to_di
+0000fd80: 7370 6c61 7920 3d20 6c69 7374 2873 6574  splay = list(set
+0000fd90: 2874 6173 6b73 5f74 6f5f 6469 7370 6c61  (tasks_to_displa
+0000fda0: 7929 290a 2020 2020 2020 2020 7461 736b  y)).        task
+0000fdb0: 735f 746f 5f64 6973 706c 6179 203d 2073  s_to_display = s
+0000fdc0: 6f72 7465 6428 7461 736b 735f 746f 5f64  orted(tasks_to_d
+0000fdd0: 6973 706c 6179 290a 2020 2020 2020 2020  isplay).        
+0000fde0: 2320 7461 736b 735f 746f 5f64 6973 706c  # tasks_to_displ
+0000fdf0: 6179 2e69 6e73 6572 7428 302c 2022 4e6f  ay.insert(0, "No
+0000fe00: 6e65 2229 0a20 2020 2023 2043 6c65 616e  ne").    # Clean
+0000fe10: 7570 2050 726f 6669 6c65 730a 2020 2020  up Profiles.    
+0000fe20: 6966 206e 6f74 2068 6176 655f 7072 6f66  if not have_prof
+0000fe30: 696c 6573 2061 6e64 206e 6f74 2068 6176  iles and not hav
+0000fe40: 655f 7461 736b 733a 0a20 2020 2020 2020  e_tasks:.       
+0000fe50: 2073 656c 662e 6469 7370 6c61 795f 6d65   self.display_me
+0000fe60: 7373 6167 655f 626f 7828 0a20 2020 2020  ssage_box(.     
+0000fe70: 2020 2020 2020 2022 4e6f 2070 726f 6669         "No profi
+0000fe80: 6c65 7320 6f72 2074 6173 6b73 2066 6f75  les or tasks fou
+0000fe90: 6e64 2069 6e20 584d 4c20 6669 6c65 2e20  nd in XML file. 
+0000fea0: 2055 7369 6e67 2074 6865 2027 4765 7420   Using the 'Get 
+0000feb0: 4c6f 6361 6c20 586d 6c20 6275 7474 6f6e  Local Xml button
+0000fec0: 2c20 6c6f 6164 2061 6e6f 7468 6572 2058  , load another X
+0000fed0: 4d4c 2066 696c 6520 616e 6420 7472 7920  ML file and try 
+0000fee0: 6167 6169 6e2e 222c 0a20 2020 2020 2020  again.",.       
+0000fef0: 2020 2020 2022 5265 6422 2c0a 2020 2020       "Red",.    
+0000ff00: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+0000ff10: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+0000ff20: 2320 4d61 6b65 2061 6c70 6861 6265 7469  # Make alphabeti
+0000ff30: 6361 6c0a 2020 2020 6966 2070 726f 6a65  cal.    if proje
+0000ff40: 6374 733a 0a20 2020 2020 2020 2070 726f  cts:.        pro
+0000ff50: 6a65 6374 7320 3d20 736f 7274 6564 2870  jects = sorted(p
+0000ff60: 726f 6a65 6374 7329 0a20 2020 2070 726f  rojects).    pro
+0000ff70: 6669 6c65 735f 746f 5f64 6973 706c 6179  files_to_display
+0000ff80: 203d 2073 6f72 7465 6428 7072 6f66 696c   = sorted(profil
+0000ff90: 6573 5f74 6f5f 6469 7370 6c61 7929 0a20  es_to_display). 
+0000ffa0: 2020 2023 2070 726f 6669 6c65 735f 746f     # profiles_to
+0000ffb0: 5f64 6973 706c 6179 2e69 6e73 6572 7428  _display.insert(
+0000ffc0: 302c 2022 4e6f 6e65 2229 0a0a 2020 2020  0, "None")..    
+0000ffd0: 2320 4469 7370 6c61 7920 7468 6520 6f62  # Display the ob
+0000ffe0: 6a65 6374 2070 756c 6c64 6f77 6e73 2069  ject pulldowns i
+0000fff0: 6e20 2741 6e61 6c79 7a65 2720 7461 620a  n 'Analyze' tab.
+00010000: 2020 2020 7365 6c66 2e61 695f 7072 6f66      self.ai_prof
+00010010: 696c 655f 6f70 7469 6f6e 6d65 6e75 2c20  ile_optionmenu, 
+00010020: 7365 6c66 2e61 695f 7461 736b 5f6f 7074  self.ai_task_opt
+00010030: 696f 6e6d 656e 7520 3d20 6469 7370 6c61  ionmenu = displa
+00010040: 795f 6f62 6a65 6374 5f70 756c 6c64 6f77  y_object_pulldow
+00010050: 6e73 280a 2020 2020 2020 2020 7365 6c66  ns(.        self
+00010060: 2c0a 2020 2020 2020 2020 7365 6c66 2e74  ,.        self.t
+00010070: 6162 7669 6577 2e74 6162 2822 416e 616c  abview.tab("Anal
+00010080: 797a 6522 292c 0a20 2020 2020 2020 2038  yze"),.        8
+00010090: 2c0a 2020 2020 2020 2020 5b5d 2c0a 2020  ,.        [],.  
+000100a0: 2020 2020 2020 7072 6f66 696c 6573 5f74        profiles_t
+000100b0: 6f5f 6469 7370 6c61 792c 0a20 2020 2020  o_display,.     
+000100c0: 2020 2074 6173 6b73 5f74 6f5f 6469 7370     tasks_to_disp
+000100d0: 6c61 792c 0a20 2020 2020 2020 204e 6f6e  lay,.        Non
+000100e0: 652c 0a20 2020 2020 2020 2073 656c 662e  e,.        self.
+000100f0: 7369 6e67 6c65 5f70 726f 6669 6c65 5f6e  single_profile_n
+00010100: 616d 655f 6576 656e 742c 0a20 2020 2020  ame_event,.     
+00010110: 2020 2073 656c 662e 7369 6e67 6c65 5f74     self.single_t
+00010120: 6173 6b5f 6e61 6d65 5f65 7665 6e74 2c0a  ask_name_event,.
+00010130: 2020 2020 290a 0a20 2020 2023 2044 6973      )..    # Dis
+00010140: 706c 6179 2074 6865 206f 626a 6563 7420  play the object 
+00010150: 7075 6c6c 646f 776e 7320 696e 2027 5370  pulldowns in 'Sp
+00010160: 6563 6966 6963 204e 616d 6527 2074 6162  ecific Name' tab
+00010170: 0a20 2020 2069 6620 6e6f 7420 7072 6f6a  .    if not proj
+00010180: 6563 7473 3a20 2023 2049 6620 6e6f 2050  ects:  # If no P
+00010190: 726f 6a65 6374 7320 746f 2064 6973 706c  rojects to displ
+000101a0: 6179 0a20 2020 2020 2020 2070 726f 6a65  ay.        proje
+000101b0: 6374 7320 3d20 5b22 4e6f 6e65 225d 0a20  cts = ["None"]. 
+000101c0: 2020 2073 656c 662e 7370 6563 6966 6963     self.specific
+000101d0: 5f70 726f 6669 6c65 5f6f 7074 696f 6e6d  _profile_optionm
+000101e0: 656e 752c 2073 656c 662e 7370 6563 6966  enu, self.specif
+000101f0: 6963 5f74 6173 6b5f 6f70 7469 6f6e 6d65  ic_task_optionme
+00010200: 6e75 203d 2064 6973 706c 6179 5f6f 626a  nu = display_obj
+00010210: 6563 745f 7075 6c6c 646f 776e 7328 0a20  ect_pulldowns(. 
+00010220: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00010230: 2020 2020 2073 656c 662e 7461 6276 6965       self.tabvie
+00010240: 772e 7461 6228 2253 7065 6369 6669 6320  w.tab("Specific 
+00010250: 4e61 6d65 2229 2c0a 2020 2020 2020 2020  Name"),.        
+00010260: 352c 0a20 2020 2020 2020 2070 726f 6a65  5,.        proje
+00010270: 6374 732c 0a20 2020 2020 2020 2070 726f  cts,.        pro
+00010280: 6669 6c65 735f 746f 5f64 6973 706c 6179  files_to_display
+00010290: 2c0a 2020 2020 2020 2020 7461 736b 735f  ,.        tasks_
+000102a0: 746f 5f64 6973 706c 6179 2c0a 2020 2020  to_display,.    
+000102b0: 2020 2020 7365 6c66 2e73 696e 676c 655f      self.single_
+000102c0: 7072 6f6a 6563 745f 6e61 6d65 5f65 7665  project_name_eve
+000102d0: 6e74 2c0a 2020 2020 2020 2020 7365 6c66  nt,.        self
+000102e0: 2e73 696e 676c 655f 7072 6f66 696c 655f  .single_profile_
+000102f0: 6e61 6d65 5f65 7665 6e74 2c0a 2020 2020  name_event,.    
+00010300: 2020 2020 7365 6c66 2e73 696e 676c 655f      self.single_
+00010310: 7461 736b 5f6e 616d 655f 6576 656e 742c  task_name_event,
+00010320: 0a20 2020 2029 0a0a 2020 2020 7265 7475  .    )..    retu
+00010330: 726e 2054 7275 650a 0a0a 2320 4275 696c  rn True...# Buil
+00010340: 6420 6120 6c69 7374 206f 6620 5072 6f66  d a list of Prof
+00010350: 696c 6573 2074 6861 7420 6172 6520 756e  iles that are un
+00010360: 6465 7220 7468 6520 6769 7665 6e20 7072  der the given pr
+00010370: 6f6a 6563 740a 6465 6620 6275 696c 645f  oject.def build_
+00010380: 7072 6f66 696c 6573 2872 6f6f 743a 2064  profiles(root: d
+00010390: 6963 742c 2070 726f 6669 6c65 5f69 6473  ict, profile_ids
+000103a0: 3a20 6c69 7374 2920 2d3e 206c 6973 743a  : list) -> list:
+000103b0: 0a20 2020 2022 2222 5061 7261 6d65 7465  .    """Paramete
+000103c0: 7273 3a0a 2020 2020 2020 2020 2d20 726f  rs:.        - ro
+000103d0: 6f74 2028 6469 6374 293a 2044 6963 7469  ot (dict): Dicti
+000103e0: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+000103f0: 2061 6c6c 2070 726f 6669 6c65 7320 616e   all profiles an
+00010400: 6420 7468 6569 7220 7461 736b 732e 0a20  d their tasks.. 
+00010410: 2020 2020 2020 202d 2070 726f 6669 6c65         - profile
+00010420: 5f69 6473 2028 6c69 7374 293a 204c 6973  _ids (list): Lis
+00010430: 7420 6f66 2070 726f 6669 6c65 2049 4473  t of profile IDs
+00010440: 2074 6f20 6265 2070 726f 6365 7373 6564   to be processed
+00010450: 2e0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+00010460: 2020 2020 2020 202d 206c 6973 743a 204c         - list: L
+00010470: 6973 7420 6f66 2064 6963 7469 6f6e 6172  ist of dictionar
+00010480: 6965 7320 636f 6e74 6169 6e69 6e67 2070  ies containing p
+00010490: 726f 6669 6c65 206e 616d 6573 2061 6e64  rofile names and
+000104a0: 2074 6865 6972 2063 6f72 7265 7370 6f6e   their correspon
+000104b0: 6469 6e67 2074 6173 6b73 2e0a 2020 2020  ding tasks..    
+000104c0: 5072 6f63 6573 7369 6e67 204c 6f67 6963  Processing Logic
+000104d0: 3a0a 2020 2020 2020 2020 2d20 4765 7420  :.        - Get 
+000104e0: 616c 6c20 7072 6f66 696c 6573 2066 726f  all profiles fro
+000104f0: 6d20 726f 6f74 2064 6963 7469 6f6e 6172  m root dictionar
+00010500: 792e 0a20 2020 2020 2020 202d 2043 7265  y..        - Cre
+00010510: 6174 6520 616e 2065 6d70 7479 206c 6973  ate an empty lis
+00010520: 7420 746f 2073 746f 7265 2070 726f 6669  t to store profi
+00010530: 6c65 206e 616d 6573 2061 6e64 2074 6173  le names and tas
+00010540: 6b73 2e0a 2020 2020 2020 2020 2d20 4c6f  ks..        - Lo
+00010550: 6f70 2074 6872 6f75 6768 2065 6163 6820  op through each 
+00010560: 7072 6f66 696c 6520 4944 2069 6e20 7468  profile ID in th
+00010570: 6520 7072 6f76 6964 6564 206c 6973 742e  e provided list.
+00010580: 0a20 2020 2020 2020 202d 2047 6574 2074  .        - Get t
+00010590: 6865 2074 6173 6b73 2066 6f72 2074 6865  he tasks for the
+000105a0: 2063 7572 7265 6e74 2070 726f 6669 6c65   current profile
+000105b0: 2e0a 2020 2020 2020 2020 2d20 4966 2074  ..        - If t
+000105c0: 6173 6b73 2061 7265 2066 6f75 6e64 2c20  asks are found, 
+000105d0: 6372 6561 7465 2061 206c 6973 7420 746f  create a list to
+000105e0: 2073 746f 7265 2074 6173 6b20 6e61 6d65   store task name
+000105f0: 732e 0a20 2020 2020 2020 202d 204c 6f6f  s..        - Loo
+00010600: 7020 7468 726f 7567 6820 6561 6368 2074  p through each t
+00010610: 6173 6b20 616e 6420 6164 6420 6974 7320  ask and add its 
+00010620: 6e61 6d65 2074 6f20 7468 6520 7461 736b  name to the task
+00010630: 206c 6973 742e 0a20 2020 2020 2020 202d   list..        -
+00010640: 2049 6620 6e6f 2074 6173 6b73 2061 7265   If no tasks are
+00010650: 2066 6f75 6e64 2c20 6164 6420 6120 6465   found, add a de
+00010660: 6661 756c 7420 6d65 7373 6167 6520 746f  fault message to
+00010670: 2074 6865 2074 6173 6b20 6c69 7374 2e0a   the task list..
+00010680: 2020 2020 2020 2020 2d20 4765 7420 7468          - Get th
+00010690: 6520 6e61 6d65 206f 6620 7468 6520 6375  e name of the cu
+000106a0: 7272 656e 7420 7072 6f66 696c 652e 0a20  rrent profile.. 
+000106b0: 2020 2020 2020 202d 2049 6620 6e6f 206e         - If no n
+000106c0: 616d 6520 6973 2066 6f75 6e64 2c20 6164  ame is found, ad
+000106d0: 6420 6120 6465 6661 756c 7420 6d65 7373  d a default mess
+000106e0: 6167 6520 746f 2074 6865 2070 726f 6669  age to the profi
+000106f0: 6c65 206e 616d 652e 0a20 2020 2020 2020  le name..       
+00010700: 202d 2043 6f6d 6269 6e65 2074 6865 2070   - Combine the p
+00010710: 726f 6669 6c65 206e 616d 6520 616e 6420  rofile name and 
+00010720: 7461 736b 206c 6973 7420 696e 746f 2061  task list into a
+00010730: 2064 6963 7469 6f6e 6172 7920 616e 6420   dictionary and 
+00010740: 6164 6420 6974 2074 6f20 7468 6520 7072  add it to the pr
+00010750: 6f66 696c 6520 6c69 7374 2e0a 2020 2020  ofile list..    
+00010760: 2020 2020 2d20 5265 7475 726e 2074 6865      - Return the
+00010770: 2070 726f 6669 6c65 206c 6973 742e 2222   profile list.""
+00010780: 220a 2020 2020 7072 6f66 696c 6573 203d  ".    profiles =
+00010790: 2072 6f6f 745b 2261 6c6c 5f70 726f 6669   root["all_profi
+000107a0: 6c65 7322 5d0a 2020 2020 7072 6f66 696c  les"].    profil
+000107b0: 655f 6c69 7374 203d 205b 5d0a 2020 2020  e_list = [].    
+000107c0: 666f 7220 7072 6f66 696c 6520 696e 2070  for profile in p
+000107d0: 726f 6669 6c65 5f69 6473 3a0a 2020 2020  rofile_ids:.    
+000107e0: 2020 2020 2320 4765 7420 7468 6520 5072      # Get the Pr
+000107f0: 6f66 696c 6527 7320 5461 736b 730a 2020  ofile's Tasks.  
+00010800: 2020 2020 2020 5072 696d 6549 7465 6d73        PrimeItems
+00010810: 2e74 6173 6b5f 636f 756e 745f 756e 6e61  .task_count_unna
+00010820: 6d65 6420 3d20 3020 2023 2041 766f 6964  med = 0  # Avoid
+00010830: 2061 6e20 6572 726f 7220 696e 2067 6574   an error in get
+00010840: 5f70 726f 6669 6c65 5f74 6173 6b73 0a20  _profile_tasks. 
+00010850: 2020 2020 2020 2069 6620 7468 655f 7461         if the_ta
+00010860: 736b 7320 3a3d 2067 6574 5f70 726f 6669  sks := get_profi
+00010870: 6c65 5f74 6173 6b73 2870 726f 6669 6c65  le_tasks(profile
+00010880: 735b 7072 6f66 696c 655d 5b22 786d 6c22  s[profile]["xml"
+00010890: 5d2c 205b 5d2c 205b 5d29 3a0a 2020 2020  ], [], []):.    
+000108a0: 2020 2020 2020 2020 7461 736b 5f6c 6973          task_lis
+000108b0: 7420 3d20 5b5d 0a20 2020 2020 2020 2020  t = [].         
+000108c0: 2020 2023 2050 726f 6365 7373 2065 6163     # Process eac
+000108d0: 6820 5461 736b 2e20 2054 6173 6b73 2061  h Task.  Tasks a
+000108e0: 7265 2073 696d 706c 7920 6120 666c 6174  re simply a flat
+000108f0: 206c 6973 7420 6f66 206e 616d 6573 2e0a   list of names..
+00010900: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00010910: 7461 736b 2069 6e20 7468 655f 7461 736b  task in the_task
+00010920: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00010930: 2020 2069 6620 7461 736b 5b22 6e61 6d65     if task["name
+00010940: 225d 203d 3d20 2222 3a0a 2020 2020 2020  "] == "":.      
+00010950: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00010960: 736b 5f6c 6973 742e 6170 7065 6e64 2822  sk_list.append("
+00010970: 5461 736b 3a20 556e 6e61 6d65 6420 5461  Task: Unnamed Ta
+00010980: 736b 2229 0a20 2020 2020 2020 2020 2020  sk").           
+00010990: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000109a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000109b0: 6173 6b5f 6c69 7374 2e61 7070 656e 6428  ask_list.append(
+000109c0: 6627 5461 736b 3a20 7b74 6173 6b5b 226e  f'Task: {task["n
+000109d0: 616d 6522 5d7d 2729 0a20 2020 2020 2020  ame"]}').       
+000109e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000109f0: 2020 2074 6173 6b5f 6c69 7374 203d 205b     task_list = [
+00010a00: 224e 6f20 5072 6f66 696c 6520 5461 736b  "No Profile Task
+00010a10: 7320 466f 756e 6422 5d0a 0a20 2020 2020  s Found"]..     
+00010a20: 2020 2023 2047 6574 2074 6865 2050 726f     # Get the Pro
+00010a30: 6669 6c65 206e 616d 652e 0a20 2020 2020  file name..     
+00010a40: 2020 2069 6620 7072 6f66 696c 6573 5b70     if profiles[p
+00010a50: 726f 6669 6c65 5d5b 226e 616d 6522 5d20  rofile]["name"] 
+00010a60: 3d3d 2022 223a 0a20 2020 2020 2020 2020  == "":.         
+00010a70: 2020 2070 726f 6669 6c65 5f6e 616d 6520     profile_name 
+00010a80: 3d20 2250 726f 6669 6c65 3a20 556e 6e61  = "Profile: Unna
+00010a90: 6d65 642f 416e 6f6e 796d 6f75 7322 0a20  med/Anonymous". 
+00010aa0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00010ab0: 2020 2020 2020 2020 2070 726f 6669 6c65           profile
+00010ac0: 5f6e 616d 6520 3d20 6627 5072 6f66 696c  _name = f'Profil
+00010ad0: 653a 207b 7072 6f66 696c 6573 5b70 726f  e: {profiles[pro
+00010ae0: 6669 6c65 5d5b 226e 616d 6522 5d7d 270a  file]["name"]}'.
+00010af0: 0a20 2020 2020 2020 2023 2043 6f6d 6269  .        # Combi
+00010b00: 6e65 2074 6865 2050 726f 6669 6c65 2077  ne the Profile w
+00010b10: 6974 6820 6974 2773 2054 6173 6b73 0a20  ith it's Tasks. 
+00010b20: 2020 2020 2020 2070 726f 6669 6c65 5f6c         profile_l
+00010b30: 6973 742e 6170 7065 6e64 287b 226e 616d  ist.append({"nam
+00010b40: 6522 3a20 7072 6f66 696c 655f 6e61 6d65  e": profile_name
+00010b50: 2c20 2263 6869 6c64 7265 6e22 3a20 7461  , "children": ta
+00010b60: 736b 5f6c 6973 747d 290a 0a20 2020 2072  sk_list})..    r
+00010b70: 6574 7572 6e20 7072 6f66 696c 655f 6c69  eturn profile_li
+00010b80: 7374 0a0a 0a23 2044 6973 706c 6179 2073  st...# Display s
+00010b90: 7461 7274 7570 206d 6573 7361 6765 7320  tartup messages 
+00010ba0: 7768 6963 6820 6172 6520 6120 6361 7272  which are a carr
+00010bb0: 796f 7665 7220 6672 6f6d 2074 6865 206c  yover from the l
+00010bc0: 6173 7420 7275 6e2e 0a64 6566 2064 6973  ast run..def dis
+00010bd0: 706c 6179 5f6d 6573 7361 6765 735f 6672  play_messages_fr
+00010be0: 6f6d 5f6c 6173 745f 7275 6e28 7365 6c66  om_last_run(self
+00010bf0: 2920 2d3e 204e 6f6e 653a 2020 2320 6e6f  ) -> None:  # no
+00010c00: 7161 3a20 414e 4e30 3031 0a20 2020 2022  qa: ANN001.    "
+00010c10: 2222 0a20 2020 2044 6973 706c 6179 7320  "".    Displays 
+00010c20: 6d65 7373 6167 6573 2066 726f 6d20 7468  messages from th
+00010c30: 6520 6c61 7374 2072 756e 2e0a 0a20 2020  e last run...   
+00010c40: 2054 6869 7320 6675 6e63 7469 6f6e 2063   This function c
+00010c50: 6865 636b 7320 6966 2074 6865 7265 2061  hecks if there a
+00010c60: 7265 2061 6e79 2063 6172 7279 6f76 6572  re any carryover
+00010c70: 2065 7272 6f72 206d 6573 7361 6765 7320   error messages 
+00010c80: 6672 6f6d 2074 6865 206c 6173 7420 7275  from the last ru
+00010c90: 6e20 2872 6572 756e 292e 0a20 2020 2049  n (rerun)..    I
+00010ca0: 6620 7468 6572 6520 6172 652c 2069 7420  f there are, it 
+00010cb0: 7265 6164 7320 7468 6520 6572 726f 7220  reads the error 
+00010cc0: 6d65 7373 6167 6520 6672 6f6d 2074 6865  message from the
+00010cd0: 2066 696c 6520 7370 6563 6966 6965 6420   file specified 
+00010ce0: 6279 2074 6865 2060 4552 524f 525f 4649  by the `ERROR_FI
+00010cf0: 4c45 6020 636f 6e73 7461 6e74 2061 6e64  LE` constant and
+00010d00: 2068 616e 646c 6573 0a20 2020 2070 6f74   handles.    pot
+00010d10: 656e 7469 616c 206d 6973 7369 6e67 206d  ential missing m
+00010d20: 6f64 756c 6573 2e20 4966 2074 6865 2065  odules. If the e
+00010d30: 7272 6f72 206d 6573 7361 6765 2063 6f6e  rror message con
+00010d40: 7461 696e 7320 7468 6520 7374 7269 6e67  tains the string
+00010d50: 2022 4169 2052 6573 706f 6e73 6522 2c20   "Ai Response", 
+00010d60: 6974 2064 6973 706c 6179 7320 7468 650a  it displays the.
+00010d70: 2020 2020 6572 726f 7220 6d65 7373 6167      error messag
+00010d80: 6520 696e 2061 206e 6577 2074 6f70 6c65  e in a new tople
+00010d90: 7665 6c20 7769 6e64 6f77 2061 6e64 2064  vel window and d
+00010da0: 6973 706c 6179 7320 6120 6d65 7373 6167  isplays a messag
+00010db0: 6520 626f 7820 696e 6469 6361 7469 6e67  e box indicating
+00010dc0: 2074 6861 7420 7468 6520 616e 616c 7973   that the analys
+00010dd0: 6973 2072 6573 706f 6e73 650a 2020 2020  is response.    
+00010de0: 6973 2069 6e20 6120 7365 7061 7261 7465  is in a separate
+00010df0: 2077 696e 646f 7720 616e 6420 7361 7665   window and save
+00010e00: 6420 6173 2060 414e 414c 5953 4953 5f46  d as `ANALYSIS_F
+00010e10: 494c 4560 2e20 4966 2074 6865 2065 7272  ILE`. If the err
+00010e20: 6f72 206d 6573 7361 6765 2063 6f6e 7461  or message conta
+00010e30: 696e 7320 6e65 776c 696e 6520 6368 6172  ins newline char
+00010e40: 6163 7465 7273 2c0a 2020 2020 6974 2062  acters,.    it b
+00010e50: 7265 616b 7320 7468 6520 6d65 7373 6167  reaks the messag
+00010e60: 6520 7570 2069 6e74 6f20 6d75 6c74 6970  e up into multip
+00010e70: 6c65 206c 696e 6573 2061 6e64 2064 6973  le lines and dis
+00010e80: 706c 6179 7320 6561 6368 206c 696e 6520  plays each line 
+00010e90: 696e 2061 206d 6573 7361 6765 2062 6f78  in a message box
+00010ea0: 2e20 4966 2074 6865 2065 7272 6f72 206d  . If the error m
+00010eb0: 6573 7361 6765 0a20 2020 2064 6f65 7320  essage.    does 
+00010ec0: 6e6f 7420 636f 6e74 6169 6e20 6e65 776c  not contain newl
+00010ed0: 696e 6520 6368 6172 6163 7465 7273 2c20  ine characters, 
+00010ee0: 6974 2064 6973 706c 6179 7320 7468 6520  it displays the 
+00010ef0: 6572 726f 7220 6d65 7373 6167 6520 696e  error message in
+00010f00: 2061 206d 6573 7361 6765 2062 6f78 2e20   a message box. 
+00010f10: 4166 7465 7220 6469 7370 6c61 7969 6e67  After displaying
+00010f20: 2074 6865 0a20 2020 2065 7272 6f72 206d   the.    error m
+00010f30: 6573 7361 6765 2c20 6974 2072 656d 6f76  essage, it remov
+00010f40: 6573 2074 6865 2065 7272 6f72 2066 696c  es the error fil
+00010f50: 6520 746f 2070 7265 7665 6e74 2069 7420  e to prevent it 
+00010f60: 6672 6f6d 2062 6569 6e67 2064 6973 706c  from being displ
+00010f70: 6179 6564 2061 6761 696e 2e0a 0a20 2020  ayed again...   
+00010f80: 2049 6620 7468 6572 6520 6973 2061 6e20   If there is an 
+00010f90: 6572 726f 7220 6d65 7373 6167 6520 6672  error message fr
+00010fa0: 6f6d 206f 7468 6572 2072 6f75 7469 6e65  om other routine
+00010fb0: 732c 2069 7420 6469 7370 6c61 7973 2074  s, it displays t
+00010fc0: 6865 2065 7272 6f72 206d 6573 7361 6765  he error message
+00010fd0: 2069 6e20 6120 6d65 7373 6167 6520 626f   in a message bo
+00010fe0: 7820 7769 7468 2074 6865 2072 6574 7572  x with the retur
+00010ff0: 6e20 636f 6465 2e0a 0a20 2020 2050 6172  n code...    Par
+00011000: 616d 6574 6572 733a 0a20 2020 202d 204e  ameters:.    - N
+00011010: 6f6e 650a 0a20 2020 2052 6574 7572 6e73  one..    Returns
+00011020: 3a0a 2020 2020 2d20 4e6f 6e65 0a20 2020  :.    - None.   
+00011030: 2022 2222 0a20 2020 2023 2053 6565 2069   """.    # See i
+00011040: 6620 7765 2068 6176 6520 616e 7920 6361  f we have any ca
+00011050: 7272 796f 7665 7220 6572 726f 7220 6d65  rryover error me
+00011060: 7373 6167 6573 2066 726f 6d20 6c61 7374  ssages from last
+00011070: 2072 756e 2028 7265 7275 6e29 2e0a 2020   run (rerun)..  
+00011080: 2020 6966 206f 732e 7061 7468 2e69 7366    if os.path.isf
+00011090: 696c 6528 4552 524f 525f 4649 4c45 293a  ile(ERROR_FILE):
+000110a0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
+000110b0: 656e 2845 5252 4f52 5f46 494c 4529 2061  en(ERROR_FILE) a
+000110c0: 7320 6572 726f 725f 6669 6c65 3a0a 2020  s error_file:.  
+000110d0: 2020 2020 2020 2020 2020 6572 726f 725f            error_
+000110e0: 6d73 6720 3d20 6572 726f 725f 6669 6c65  msg = error_file
+000110f0: 2e72 6561 6428 290a 2020 2020 2020 2020  .read().        
+00011100: 2020 2020 2320 4861 6e64 6c65 2070 6f74      # Handle pot
+00011110: 656e 7469 616c 206d 7373 696e 6720 6d6f  ential mssing mo
+00011120: 6475 6c65 730a 2020 2020 2020 2020 2020  dules.          
+00011130: 2020 6966 2022 6372 6961 2220 696e 2065    if "cria" in e
+00011140: 7272 6f72 5f6d 7367 3a0a 2020 2020 2020  rror_msg:.      
+00011150: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00011160: 695f 6d69 7373 696e 675f 6d6f 6475 6c65  i_missing_module
+00011170: 203d 2022 6372 6961 220a 2020 2020 2020   = "cria".      
+00011180: 2020 2020 2020 656c 6966 2022 6f70 656e        elif "open
+00011190: 6169 2220 696e 2065 7272 6f72 5f6d 7367  ai" in error_msg
+000111a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000111b0: 2020 7365 6c66 2e61 695f 6d69 7373 696e    self.ai_missin
+000111c0: 675f 6d6f 6475 6c65 203d 2022 6f70 656e  g_module = "open
+000111d0: 6169 220a 0a20 2020 2020 2020 2020 2020  ai"..           
+000111e0: 2023 2048 616e 646c 6520 4169 2052 6573   # Handle Ai Res
+000111f0: 706f 6e73 6520 696e 206e 6577 2074 6f70  ponse in new top
+00011200: 6c65 7665 6c20 7769 6e64 6f77 0a20 2020  level window.   
+00011210: 2020 2020 2020 2020 2069 6620 2241 6920           if "Ai 
+00011220: 5265 7370 6f6e 7365 2220 696e 2065 7272  Response" in err
+00011230: 6f72 5f6d 7367 3a0a 2020 2020 2020 2020  or_msg:.        
+00011240: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
+00011250: 706c 6179 5f61 695f 7265 7370 6f6e 7365  play_ai_response
+00011260: 2865 7272 6f72 5f6d 7367 290a 2020 2020  (error_msg).    
+00011270: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011280: 2e64 6973 706c 6179 5f6d 6573 7361 6765  .display_message
+00011290: 5f62 6f78 280a 2020 2020 2020 2020 2020  _box(.          
+000112a0: 2020 2020 2020 2020 2020 6622 416e 616c            f"Anal
+000112b0: 7973 6973 2072 6573 706f 6e73 6520 6973  ysis response is
+000112c0: 2069 6e20 6120 7370 6561 7261 7465 2057   in a spearate W
+000112d0: 696e 646f 7720 616e 6420 7361 7665 6420  indow and saved 
+000112e0: 6173 207b 414e 414c 5953 4953 5f46 494c  as {ANALYSIS_FIL
+000112f0: 457d 2e22 2c0a 2020 2020 2020 2020 2020  E}.",.          
+00011300: 2020 2020 2020 2020 2020 2254 7572 7175            "Turqu
+00011310: 6f69 7365 222c 0a20 2020 2020 2020 2020  oise",.         
+00011320: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00011330: 2020 2020 2023 2053 6f6d 6520 6f74 6865       # Some othe
+00011340: 7220 6d65 7373 6167 652e 2020 4a75 7374  r message.  Just
+00011350: 2064 6973 706c 6179 2069 7420 696e 2074   display it in t
+00011360: 6865 206d 6573 7361 6765 2062 6f78 2061  he message box a
+00011370: 6e64 2062 7265 616b 2069 7420 7570 2069  nd break it up i
+00011380: 6620 6e65 6564 6564 2e0a 2020 2020 2020  f needed..      
+00011390: 2020 2020 2020 656c 6966 2022 5c6e 2220        elif "\n" 
+000113a0: 696e 2065 7272 6f72 5f6d 7367 3a0a 2020  in error_msg:.  
+000113b0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+000113c0: 7373 6167 6573 203d 2065 7272 6f72 5f6d  ssages = error_m
+000113d0: 7367 2e73 706c 6974 2822 5c6e 2229 0a20  sg.split("\n"). 
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000113f0: 6f72 206d 6573 7361 6765 5f6c 696e 6520  or message_line 
+00011400: 696e 206d 6573 7361 6765 733a 0a20 2020  in messages:.   
+00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011420: 2073 656c 662e 6469 7370 6c61 795f 6d65   self.display_me
+00011430: 7373 6167 655f 626f 7828 6d65 7373 6167  ssage_box(messag
+00011440: 655f 6c69 6e65 2c20 2252 6564 2229 0a20  e_line, "Red"). 
+00011450: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00011460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011470: 2073 656c 662e 6469 7370 6c61 795f 6d65   self.display_me
+00011480: 7373 6167 655f 626f 7828 6572 726f 725f  ssage_box(error_
+00011490: 6d73 672c 2022 5265 6422 290a 2020 2020  msg, "Red").    
+000114a0: 2020 2020 2020 2020 6f73 2e72 656d 6f76          os.remov
+000114b0: 6528 4552 524f 525f 4649 4c45 2920 2023  e(ERROR_FILE)  #
+000114c0: 2047 6574 2072 6964 206f 6620 6572 726f   Get rid of erro
+000114d0: 7220 6d65 7373 6167 6520 736f 2077 6520  r message so we 
+000114e0: 646f 6e27 7420 6469 7370 6c61 7920 6974  don't display it
+000114f0: 2061 6761 696e 2e0a 0a20 2020 2023 2044   again...    # D
+00011500: 6973 706c 6179 2061 6e79 2065 7272 6f72  isplay any error
+00011510: 206d 6573 7361 6765 2066 726f 6d20 6f74   message from ot
+00011520: 6865 7220 726f 756e 7469 6e65 730a 2020  her rountines.  
+00011530: 2020 6966 2050 7269 6d65 4974 656d 732e    if PrimeItems.
+00011540: 6572 726f 725f 6d73 673a 0a20 2020 2020  error_msg:.     
+00011550: 2020 2073 656c 662e 6469 7370 6c61 795f     self.display_
+00011560: 6d65 7373 6167 655f 626f 7828 6622 7b50  message_box(f"{P
+00011570: 7269 6d65 4974 656d 732e 6572 726f 725f  rimeItems.error_
+00011580: 6d73 677d 2077 6974 6820 7265 7475 726e  msg} with return
+00011590: 2063 6f64 6520 7b50 7269 6d65 4974 656d   code {PrimeItem
+000115a0: 732e 6572 726f 725f 636f 6465 7d2e 222c  s.error_code}.",
+000115b0: 2022 5265 6422 290a 0a0a 2320 4469 7370   "Red")...# Disp
+000115c0: 6c61 7920 7468 6520 6375 7272 656e 7420  lay the current 
+000115d0: 6669 6c65 2061 7320 6120 6c61 6265 6c0a  file as a label.
+000115e0: 6465 6620 6469 7370 6c61 795f 6375 7272  def display_curr
+000115f0: 656e 745f 6669 6c65 2873 656c 662c 2066  ent_file(self, f
+00011600: 696c 655f 6e61 6d65 3a20 7374 7229 202d  ile_name: str) -
+00011610: 3e20 4e6f 6e65 3a20 2023 206e 6f71 613a  > None:  # noqa:
+00011620: 2041 4e4e 3030 310a 2020 2020 2222 220a   ANN001.    """.
+00011630: 2020 2020 4469 7370 6c61 7920 7468 6520      Display the 
+00011640: 6375 7272 656e 7420 6669 6c65 206e 616d  current file nam
+00011650: 6520 696e 2061 2062 7574 746f 6e20 6f6e  e in a button on
+00011660: 2074 6865 2047 5549 2e0a 0a20 2020 2041   the GUI...    A
+00011670: 7267 733a 0a20 2020 2020 2020 2066 696c  rgs:.        fil
+00011680: 655f 6e61 6d65 2028 7374 7229 3a20 5468  e_name (str): Th
+00011690: 6520 6e61 6d65 206f 6620 7468 6520 6375  e name of the cu
+000116a0: 7272 656e 7420 6669 6c65 2e0a 0a20 2020  rrent file...   
+000116b0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+000116c0: 2020 4e6f 6e65 3a20 5468 6973 2066 756e    None: This fun
+000116d0: 6374 696f 6e20 646f 6573 206e 6f74 2072  ction does not r
+000116e0: 6574 7572 6e20 616e 7974 6869 6e67 2e0a  eturn anything..
+000116f0: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
+00011700: 6f6e 2063 7265 6174 6573 2061 2062 7574  on creates a but
+00011710: 746f 6e20 6f6e 2074 6865 2047 5549 2074  ton on the GUI t
+00011720: 6861 7420 6469 7370 6c61 7973 2074 6865  hat displays the
+00011730: 2063 7572 7265 6e74 2066 696c 6520 6e61   current file na
+00011740: 6d65 2e20 5468 6520 6275 7474 6f6e 2069  me. The button i
+00011750: 7320 6372 6561 7465 6420 7573 696e 6720  s created using 
+00011760: 7468 6520 6061 6464 5f62 7574 746f 6e60  the `add_button`
+00011770: 2066 756e 6374 696f 6e20 616e 6420 6973   function and is
+00011780: 2070 6c61 6365 6420 696e 2074 6865 2073   placed in the s
+00011790: 6563 6f6e 6420 726f 7720 616e 6420 7465  econd row and te
+000117a0: 6e74 6820 636f 6c75 6d6e 206f 6620 7468  nth column of th
+000117b0: 6520 4755 492e 2054 6865 2062 7574 746f  e GUI. The butto
+000117c0: 6e27 7320 7465 7874 2069 7320 7365 7420  n's text is set 
+000117d0: 746f 2022 4375 7272 656e 7420 4669 6c65  to "Current File
+000117e0: 3a20 7b66 696c 655f 6e61 6d65 7d22 2e20  : {file_name}". 
+000117f0: 5468 6520 6073 656c 662e 7265 706f 7274  The `self.report
+00011800: 5f69 7373 7565 5f65 7665 6e74 6020 6675  _issue_event` fu
+00011810: 6e63 7469 6f6e 2069 7320 6173 7369 676e  nction is assign
+00011820: 6564 2061 7320 7468 6520 6275 7474 6f6e  ed as the button
+00011830: 2773 2063 6c69 636b 2065 7665 6e74 2068  's click event h
+00011840: 616e 646c 6572 2e0a 0a20 2020 204e 6f74  andler...    Not
+00011850: 653a 0a20 2020 2020 2020 202d 2054 6865  e:.        - The
+00011860: 2060 6164 645f 6275 7474 6f6e 6020 6675   `add_button` fu
+00011870: 6e63 7469 6f6e 2069 7320 6173 7375 6d65  nction is assume
+00011880: 6420 746f 2062 6520 6465 6669 6e65 6420  d to be defined 
+00011890: 656c 7365 7768 6572 6520 696e 2074 6865  elsewhere in the
+000118a0: 2063 6f64 6562 6173 652e 0a20 2020 2020   codebase..     
+000118b0: 2020 202d 2054 6865 2060 7365 6c66 2e72     - The `self.r
+000118c0: 6570 6f72 745f 6973 7375 655f 6576 656e  eport_issue_even
+000118d0: 7460 2066 756e 6374 696f 6e20 6973 2061  t` function is a
+000118e0: 7373 756d 6564 2074 6f20 6265 2064 6566  ssumed to be def
+000118f0: 696e 6564 2065 6c73 6577 6865 7265 2069  ined elsewhere i
+00011900: 6e20 7468 6520 636f 6465 6261 7365 2e0a  n the codebase..
+00011910: 0a20 2020 2045 7861 6d70 6c65 3a0a 2020  .    Example:.  
+00011920: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+00011930: 2020 2020 2020 2020 6775 695f 696e 7374          gui_inst
+00011940: 616e 6365 2e64 6973 706c 6179 5f63 7572  ance.display_cur
+00011950: 7265 6e74 5f66 696c 6528 2265 7861 6d70  rent_file("examp
+00011960: 6c65 2e74 7874 2229 0a20 2020 2020 2020  le.txt").       
+00011970: 2060 6060 0a20 2020 2022 2222 0a20 2020   ```.    """.   
+00011980: 2023 2043 6c65 6172 2070 7265 7669 6f75   # Clear previou
+00011990: 7320 6966 2066 696c 6c65 642e 0a20 2020  s if filled..   
+000119a0: 2077 6974 6820 636f 6e74 6578 746c 6962   with contextlib
+000119b0: 2e73 7570 7072 6573 7328 4174 7472 6962  .suppress(Attrib
+000119c0: 7574 6545 7272 6f72 293a 0a20 2020 2020  uteError):.     
+000119d0: 2020 2073 656c 662e 7265 706f 7274 5f69     self.report_i
+000119e0: 7373 7565 5f62 7574 746f 6e2e 6465 7374  ssue_button.dest
+000119f0: 726f 7928 290a 2020 2020 2320 4368 6563  roy().    # Chec
+00011a00: 6b20 666f 7220 736c 6173 6865 7320 616e  k for slashes an
+00011a10: 6420 7265 6d6f 7665 2069 6620 6e65 7373  d remove if ness
+00011a20: 6573 6172 790a 2020 2020 6669 6c65 6e61  esary.    filena
+00011a30: 6d65 5f6c 6f63 6174 696f 6e20 3d20 6669  me_location = fi
+00011a40: 6c65 5f6e 616d 652e 7266 696e 6428 5072  le_name.rfind(Pr
+00011a50: 696d 6549 7465 6d73 2e73 6c61 7368 2920  imeItems.slash) 
+00011a60: 2b20 310a 2020 2020 6966 2066 696c 656e  + 1.    if filen
+00011a70: 616d 655f 6c6f 6361 7469 6f6e 2021 3d20  ame_location != 
+00011a80: 2d31 3a0a 2020 2020 2020 2020 6669 6c65  -1:.        file
+00011a90: 5f6e 616d 6520 3d20 6669 6c65 5f6e 616d  _name = file_nam
+00011aa0: 655b 6669 6c65 6e61 6d65 5f6c 6f63 6174  e[filename_locat
+00011ab0: 696f 6e3a 5d0a 2020 2020 7365 6c66 2e72  ion:].    self.r
+00011ac0: 6570 6f72 745f 6973 7375 655f 6275 7474  eport_issue_butt
+00011ad0: 6f6e 203d 2061 6464 5f6c 6162 656c 280a  on = add_label(.
+00011ae0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00011af0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00011b00: 2020 2020 6622 4375 7272 656e 7420 4669      f"Current Fi
+00011b10: 6c65 3a20 7b66 696c 655f 6e61 6d65 7d22  le: {file_name}"
+00011b20: 2c0a 2020 2020 2020 2020 2222 2c0a 2020  ,.        "",.  
+00011b30: 2020 2020 2020 2222 2c0a 2020 2020 2020        "",.      
+00011b40: 2020 226e 6f72 6d61 6c22 2c0a 2020 2020    "normal",.    
+00011b50: 2020 2020 3131 2c0a 2020 2020 2020 2020      11,.        
+00011b60: 312c 0a20 2020 2020 2020 2032 302c 0a20  1,.        20,. 
+00011b70: 2020 2020 2020 2030 2c0a 2020 2020 2020         0,.      
+00011b80: 2020 2277 222c 0a20 2020 2029 0a0a 0a23    "w",.    )...#
+00011b90: 2053 6574 2075 7020 6572 726f 7220 6d65   Set up error me
+00011ba0: 7373 6167 6520 666f 7220 7369 6e67 6c65  ssage for single
+00011bb0: 2050 726f 6a65 6374 2f50 726f 6669 6c65   Project/Profile
+00011bc0: 2f54 6173 6b20 6e61 6d65 2074 6861 7420  /Task name that 
+00011bd0: 7761 7320 656e 7465 7265 642e 2020 4361  was entered.  Ca
+00011be0: 6c6c 6564 2062 7920 6368 6563 6b5f 6e61  lled by check_na
+00011bf0: 6d65 2069 6e20 7573 6572 696e 7472 2e0a  me in userintr..
+00011c00: 6465 6620 7365 7475 705f 6e61 6d65 5f65  def setup_name_e
+00011c10: 7272 6f72 286f 626a 6563 7431 5f6e 616d  rror(object1_nam
+00011c20: 653a 2073 7472 2c20 6f62 6a65 6374 325f  e: str, object2_
+00011c30: 6e61 6d65 3a20 7374 722c 2073 696e 676c  name: str, singl
+00011c40: 655f 6e61 6d65 313a 2073 7472 2c20 7369  e_name1: str, si
+00011c50: 6e67 6c65 5f6e 616d 6532 3a20 7374 7229  ngle_name2: str)
+00011c60: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
+00011c70: 220a 2020 2020 5365 7420 7570 2061 6e20  ".    Set up an 
+00011c80: 6572 726f 7220 6d65 7373 6167 6520 666f  error message fo
+00011c90: 7220 7768 656e 2062 6f74 6820 6120 5072  r when both a Pr
+00011ca0: 6f6a 6563 7420 616e 6420 6120 5072 6f66  oject and a Prof
+00011cb0: 696c 6520 6e61 6d65 2061 7265 2065 6e74  ile name are ent
+00011cc0: 6572 6564 2e0a 0a20 2020 2041 7267 733a  ered...    Args:
+00011cd0: 0a20 2020 2020 2020 206f 626a 6563 7431  .        object1
+00011ce0: 5f6e 616d 6520 2873 7472 293a 2054 6865  _name (str): The
+00011cf0: 206e 616d 6520 6f66 2074 6865 2066 6972   name of the fir
+00011d00: 7374 206f 626a 6563 7420 2850 726f 6a65  st object (Proje
+00011d10: 6374 292e 0a20 2020 2020 2020 206f 626a  ct)..        obj
+00011d20: 6563 7432 5f6e 616d 6520 2873 7472 293a  ect2_name (str):
+00011d30: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+00011d40: 2073 6563 6f6e 6420 6f62 6a65 6374 2028   second object (
+00011d50: 5072 6f66 696c 6529 2e0a 2020 2020 2020  Profile)..      
+00011d60: 2020 7369 6e67 6c65 5f6e 616d 6531 2028    single_name1 (
+00011d70: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
+00011d80: 6620 7468 6520 5072 6f6a 6563 742e 0a20  f the Project.. 
+00011d90: 2020 2020 2020 2073 696e 676c 655f 6e61         single_na
+00011da0: 6d65 3220 2873 7472 293a 2054 6865 206e  me2 (str): The n
+00011db0: 616d 6520 6f66 2074 6865 2050 726f 6669  ame of the Profi
+00011dc0: 6c65 2e0a 0a20 2020 2052 6574 7572 6e73  le...    Returns
+00011dd0: 3a0a 2020 2020 2020 2020 4e6f 6e65 3a20  :.        None: 
+00011de0: 5468 6973 2066 756e 6374 696f 6e20 646f  This function do
+00011df0: 6573 206e 6f74 2072 6574 7572 6e20 616e  es not return an
+00011e00: 7974 6869 6e67 2e0a 2020 2020 2222 220a  ything..    """.
+00011e10: 2020 2020 7265 7475 726e 205b 0a20 2020      return [.   
+00011e20: 2020 2020 2022 4572 726f 723a 5c6e 5c6e       "Error:\n\n
+00011e30: 222c 0a20 2020 2020 2020 2066 2259 6f75  ",.        f"You
+00011e40: 2068 6176 6520 656e 7465 7265 6420 626f   have entered bo
+00011e50: 7468 2061 207b 6f62 6a65 6374 315f 6e61  th a {object1_na
+00011e60: 6d65 7d20 616e 6420 6120 7b6f 626a 6563  me} and a {objec
+00011e70: 7432 5f6e 616d 657d 206e 616d 6521 5c6e  t2_name} name!\n
+00011e80: 222c 0a20 2020 2020 2020 2066 2228 5072  ",.        f"(Pr
+00011e90: 6f6a 6563 7420 7b73 696e 676c 655f 6e61  oject {single_na
+00011ea0: 6d65 317d 2061 6e64 2050 726f 6669 6c65  me1} and Profile
+00011eb0: 207b 7369 6e67 6c65 5f6e 616d 6532 7d29   {single_name2})
+00011ec0: 5c6e 222c 0a20 2020 2020 2020 2022 5472  \n",.        "Tr
+00011ed0: 7920 6167 6169 6e20 616e 6420 6f6e 6c79  y again and only
+00011ee0: 2073 656c 6563 7420 6f6e 652e 5c6e 222c   select one.\n",
+00011ef0: 0a20 2020 205d 0a0a 0a23 2053 6574 2074  .    ]...# Set t
+00011f00: 6865 2063 7572 7265 6e74 2050 726f 6a65  he current Proje
+00011f10: 6374 2f50 726f 6669 6c65 2f54 6173 6b20  ct/Profile/Task 
+00011f20: 6e61 6d65 7320 696e 2074 6865 2070 756c  names in the pul
+00011f30: 6c64 6f77 6e20 6d65 6e75 730a 6465 6620  ldown menus.def 
+00011f40: 7365 745f 7461 736b 6572 5f6f 626a 6563  set_tasker_objec
+00011f50: 745f 6e61 6d65 7328 7365 6c66 2920 2d3e  t_names(self) ->
+00011f60: 204e 6f6e 653a 2020 2320 6e6f 7161 3a20   None:  # noqa: 
+00011f70: 414e 4e30 3031 0a20 2020 2022 2222 0a20  ANN001.    """. 
+00011f80: 2020 2053 6574 7320 7468 6520 6e61 6d65     Sets the name
+00011f90: 7320 746f 2064 6973 706c 6179 2069 6e20  s to display in 
+00011fa0: 7468 6520 7075 6c6c 646f 776e 206d 656e  the pulldown men
+00011fb0: 7573 2062 6173 6564 206f 6e20 7468 6520  us based on the 
+00011fc0: 6375 7272 656e 7420 7461 736b 6572 206f  current tasker o
+00011fd0: 626a 6563 7420 6e61 6d65 732e 0a0a 2020  bject names...  
+00011fe0: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
+00011ff0: 6465 7465 726d 696e 6573 2074 6865 2076  determines the v
+00012000: 616c 7565 7320 746f 2062 6520 6469 7370  alues to be disp
+00012010: 6c61 7965 6420 696e 2074 6865 206f 7074  layed in the opt
+00012020: 696f 6e20 6d65 6e75 7320 666f 7220 7468  ion menus for th
+00012030: 6520 7461 736b 6572 206f 626a 6563 7473  e tasker objects
+00012040: 2e20 5468 6520 7661 6c75 6573 2061 7265  . The values are
+00012050: 2064 6574 6572 6d69 6e65 6420 6261 7365   determined base
+00012060: 6420 6f6e 2074 6865 2066 6f6c 6c6f 7769  d on the followi
+00012070: 6e67 2063 6f6e 6469 7469 6f6e 733a 0a0a  ng conditions:..
+00012080: 2020 2020 2d20 4966 2061 2073 696e 676c      - If a singl
+00012090: 6520 7072 6f6a 6563 7420 6e61 6d65 2069  e project name i
+000120a0: 7320 6176 6169 6c61 626c 652c 2074 6865  s available, the
+000120b0: 2070 726f 6a65 6374 206f 7074 696f 6e20   project option 
+000120c0: 6d65 6e75 2069 7320 7365 7420 746f 2074  menu is set to t
+000120d0: 6865 2070 726f 6a65 6374 206e 616d 652c  he project name,
+000120e0: 2061 6e64 2074 6865 2070 726f 6669 6c65   and the profile
+000120f0: 2061 6e64 2074 6173 6b20 6f70 7469 6f6e   and task option
+00012100: 206d 656e 7573 2061 7265 2073 6574 2074   menus are set t
+00012110: 6f20 7468 6569 7220 6465 6661 756c 7420  o their default 
+00012120: 7661 6c75 6573 2e0a 2020 2020 2d20 4966  values..    - If
+00012130: 2061 2073 696e 676c 6520 7072 6f66 696c   a single profil
+00012140: 6520 6e61 6d65 2069 7320 6176 6169 6c61  e name is availa
+00012150: 626c 652c 2074 6865 2070 726f 6669 6c65  ble, the profile
+00012160: 206f 7074 696f 6e20 6d65 6e75 2069 7320   option menu is 
+00012170: 7365 7420 746f 2074 6865 2070 726f 6669  set to the profi
+00012180: 6c65 206e 616d 652c 2061 6e64 2074 6865  le name, and the
+00012190: 2070 726f 6a65 6374 2061 6e64 2074 6173   project and tas
+000121a0: 6b20 6f70 7469 6f6e 206d 656e 7573 2061  k option menus a
+000121b0: 7265 2073 6574 2074 6f20 7468 6569 7220  re set to their 
+000121c0: 6465 6661 756c 7420 7661 6c75 6573 2e0a  default values..
+000121d0: 2020 2020 2d20 4966 2061 2073 696e 676c      - If a singl
+000121e0: 6520 7461 736b 206e 616d 6520 6973 2061  e task name is a
+000121f0: 7661 696c 6162 6c65 2061 6e64 2074 6865  vailable and the
+00012200: 206c 6973 7420 6f66 2074 6173 6b65 7220   list of tasker 
+00012210: 6f62 6a65 6374 7320 6973 206e 6f74 2065  objects is not e
+00012220: 6d70 7479 2c20 7468 6520 7461 736b 206f  mpty, the task o
+00012230: 7074 696f 6e20 6d65 6e75 2069 7320 7365  ption menu is se
+00012240: 7420 746f 2074 6865 2074 6173 6b20 6e61  t to the task na
+00012250: 6d65 2c20 616e 6420 7468 6520 7072 6f6a  me, and the proj
+00012260: 6563 7420 616e 6420 7072 6f66 696c 6520  ect and profile 
+00012270: 6f70 7469 6f6e 206d 656e 7573 2061 7265  option menus are
+00012280: 2073 6574 2074 6f20 7468 6569 7220 6465   set to their de
+00012290: 6661 756c 7420 7661 6c75 6573 2e0a 2020  fault values..  
+000122a0: 2020 2d20 4966 206e 6f6e 6520 6f66 2074    - If none of t
+000122b0: 6865 2061 626f 7665 2063 6f6e 6469 7469  he above conditi
+000122c0: 6f6e 7320 6172 6520 6d65 742c 2061 6c6c  ons are met, all
+000122d0: 206f 7074 696f 6e20 6d65 6e75 7320 6172   option menus ar
+000122e0: 6520 7365 7420 746f 2074 6865 6972 2064  e set to their d
+000122f0: 6566 6175 6c74 2076 616c 7565 732e 0a0a  efault values...
+00012300: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
+00012310: 2020 2020 2d20 7365 6c66 2028 6f62 6a65      - self (obje
+00012320: 6374 293a 2054 6865 2063 7572 7265 6e74  ct): The current
+00012330: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
+00012340: 2063 6c61 7373 2e0a 0a20 2020 2052 6574   class...    Ret
+00012350: 7572 6e73 3a0a 2020 2020 2d20 4e6f 6e65  urns:.    - None
+00012360: 3a20 5468 6973 2066 756e 6374 696f 6e20  : This function 
+00012370: 646f 6573 206e 6f74 2072 6574 7572 6e20  does not return 
+00012380: 616e 7974 6869 6e67 2e0a 2020 2020 2222  anything..    ""
+00012390: 220a 2020 2020 2320 4465 6669 6e65 2064  ".    # Define d
+000123a0: 6566 6175 6c74 730a 2020 2020 6465 6661  efaults.    defa
+000123b0: 756c 745f 7072 6f6a 6563 7420 3d20 224e  ult_project = "N
+000123c0: 6f6e 6522 0a20 2020 2064 6566 6175 6c74  one".    default
+000123d0: 5f70 726f 6669 6c65 203d 2022 4e6f 6e65  _profile = "None
+000123e0: 220a 2020 2020 6465 6661 756c 745f 7461  ".    default_ta
+000123f0: 736b 203d 2022 4e6f 6e65 220a 2020 2020  sk = "None".    
+00012400: 6465 6661 756c 745f 6469 7370 6c61 795f  default_display_
+00012410: 6f6e 6c79 203d 2022 4469 7370 6c61 7920  only = "Display 
+00012420: 6f6e 6c79 2022 0a0a 2020 2020 2320 4465  only "..    # De
+00012430: 7465 726d 696e 6520 7661 6c75 6573 2062  termine values b
+00012440: 6173 6564 206f 6e20 636f 6e64 6974 696f  ased on conditio
+00012450: 6e73 0a20 2020 2023 2055 7064 6174 6520  ns.    # Update 
+00012460: 7468 6520 5072 6f6a 6563 742f 5072 6f66  the Project/Prof
+00012470: 696c 652f 5461 736b 2070 756c 6c64 6f77  ile/Task pulldow
+00012480: 6e20 6f70 7469 6f6e 206d 656e 7573 2e0a  n option menus..
+00012490: 2020 2020 6966 2073 656c 662e 7369 6e67      if self.sing
+000124a0: 6c65 5f70 726f 6a65 6374 5f6e 616d 653a  le_project_name:
+000124b0: 0a20 2020 2020 2020 2070 726f 6a65 6374  .        project
+000124c0: 5f74 6f5f 6469 7370 6c61 7920 3d20 6622  _to_display = f"
+000124d0: 7b64 6566 6175 6c74 5f64 6973 706c 6179  {default_display
+000124e0: 5f6f 6e6c 797d 5072 6f6a 6563 7420 277b  _only}Project '{
+000124f0: 7365 6c66 2e73 696e 676c 655f 7072 6f6a  self.single_proj
+00012500: 6563 745f 6e61 6d65 7d27 220a 2020 2020  ect_name}'".    
+00012510: 2020 2020 7365 6c66 2e73 7065 6369 6669      self.specifi
+00012520: 635f 6e61 6d65 5f6d 7367 203d 2070 726f  c_name_msg = pro
+00012530: 6a65 6374 5f74 6f5f 6469 7370 6c61 790a  ject_to_display.
+00012540: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
+00012550: 6369 6669 635f 7072 6f6a 6563 745f 6f70  cific_project_op
+00012560: 7469 6f6e 6d65 6e75 2e73 6574 2870 726f  tionmenu.set(pro
+00012570: 6a65 6374 5f74 6f5f 6469 7370 6c61 7929  ject_to_display)
+00012580: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
+00012590: 6563 6966 6963 5f70 726f 6669 6c65 5f6f  ecific_profile_o
+000125a0: 7074 696f 6e6d 656e 752e 7365 7428 6465  ptionmenu.set(de
+000125b0: 6661 756c 745f 7072 6f66 696c 6529 0a20  fault_profile). 
+000125c0: 2020 2020 2020 2073 656c 662e 6169 5f70         self.ai_p
+000125d0: 726f 6669 6c65 5f6f 7074 696f 6e6d 656e  rofile_optionmen
+000125e0: 752e 7365 7428 6465 6661 756c 745f 7072  u.set(default_pr
+000125f0: 6f66 696c 6529 0a20 2020 2020 2020 2073  ofile).        s
+00012600: 656c 662e 7370 6563 6966 6963 5f74 6173  elf.specific_tas
+00012610: 6b5f 6f70 7469 6f6e 6d65 6e75 2e73 6574  k_optionmenu.set
+00012620: 2864 6566 6175 6c74 5f74 6173 6b29 0a20  (default_task). 
+00012630: 2020 2020 2020 2073 656c 662e 6169 5f74         self.ai_t
+00012640: 6173 6b5f 6f70 7469 6f6e 6d65 6e75 2e73  ask_optionmenu.s
+00012650: 6574 2864 6566 6175 6c74 5f74 6173 6b29  et(default_task)
+00012660: 0a20 2020 2065 6c69 6620 7365 6c66 2e73  .    elif self.s
+00012670: 696e 676c 655f 7072 6f66 696c 655f 6e61  ingle_profile_na
+00012680: 6d65 3a0a 2020 2020 2020 2020 7072 6f66  me:.        prof
+00012690: 696c 655f 746f 5f64 6973 706c 6179 203d  ile_to_display =
+000126a0: 2073 656c 662e 7369 6e67 6c65 5f70 726f   self.single_pro
+000126b0: 6669 6c65 5f6e 616d 650a 2020 2020 2020  file_name.      
+000126c0: 2020 7365 6c66 2e73 7065 6369 6669 635f    self.specific_
+000126d0: 6e61 6d65 5f6d 7367 203d 2066 227b 6465  name_msg = f"{de
+000126e0: 6661 756c 745f 6469 7370 6c61 795f 6f6e  fault_display_on
+000126f0: 6c79 7d50 726f 6669 6c65 2027 7b70 726f  ly}Profile '{pro
+00012700: 6669 6c65 5f74 6f5f 6469 7370 6c61 797d  file_to_display}
+00012710: 2722 0a20 2020 2020 2020 2073 656c 662e  '".        self.
+00012720: 7370 6563 6966 6963 5f70 726f 6669 6c65  specific_profile
+00012730: 5f6f 7074 696f 6e6d 656e 752e 7365 7428  _optionmenu.set(
+00012740: 7072 6f66 696c 655f 746f 5f64 6973 706c  profile_to_displ
+00012750: 6179 290a 2020 2020 2020 2020 7365 6c66  ay).        self
+00012760: 2e61 695f 7072 6f66 696c 655f 6f70 7469  .ai_profile_opti
+00012770: 6f6e 6d65 6e75 2e73 6574 2870 726f 6669  onmenu.set(profi
+00012780: 6c65 5f74 6f5f 6469 7370 6c61 7929 0a20  le_to_display). 
+00012790: 2020 2020 2020 2073 656c 662e 7370 6563         self.spec
+000127a0: 6966 6963 5f70 726f 6a65 6374 5f6f 7074  ific_project_opt
+000127b0: 696f 6e6d 656e 752e 7365 7428 6465 6661  ionmenu.set(defa
+000127c0: 756c 745f 7072 6f6a 6563 7429 0a20 2020  ult_project).   
+000127d0: 2020 2020 2073 656c 662e 7370 6563 6966       self.specif
+000127e0: 6963 5f74 6173 6b5f 6f70 7469 6f6e 6d65  ic_task_optionme
+000127f0: 6e75 2e73 6574 2864 6566 6175 6c74 5f74  nu.set(default_t
+00012800: 6173 6b29 0a20 2020 2020 2020 2073 656c  ask).        sel
+00012810: 662e 6169 5f74 6173 6b5f 6f70 7469 6f6e  f.ai_task_option
+00012820: 6d65 6e75 2e73 6574 2864 6566 6175 6c74  menu.set(default
+00012830: 5f74 6173 6b29 0a20 2020 2065 6c69 6620  _task).    elif 
+00012840: 7365 6c66 2e73 696e 676c 655f 7461 736b  self.single_task
+00012850: 5f6e 616d 653a 0a20 2020 2020 2020 2074  _name:.        t
+00012860: 6173 6b5f 746f 5f64 6973 706c 6179 203d  ask_to_display =
+00012870: 2073 656c 662e 7369 6e67 6c65 5f74 6173   self.single_tas
+00012880: 6b5f 6e61 6d65 0a20 2020 2020 2020 2073  k_name.        s
+00012890: 656c 662e 7370 6563 6966 6963 5f6e 616d  elf.specific_nam
+000128a0: 655f 6d73 6720 3d20 6622 7b64 6566 6175  e_msg = f"{defau
+000128b0: 6c74 5f64 6973 706c 6179 5f6f 6e6c 797d  lt_display_only}
+000128c0: 5461 736b 2027 7b74 6173 6b5f 746f 5f64  Task '{task_to_d
+000128d0: 6973 706c 6179 7d27 220a 2020 2020 2020  isplay}'".      
+000128e0: 2020 7365 6c66 2e73 7065 6369 6669 635f    self.specific_
+000128f0: 7461 736b 5f6f 7074 696f 6e6d 656e 752e  task_optionmenu.
+00012900: 7365 7428 7461 736b 5f74 6f5f 6469 7370  set(task_to_disp
+00012910: 6c61 7929 0a20 2020 2020 2020 2073 656c  lay).        sel
+00012920: 662e 6169 5f74 6173 6b5f 6f70 7469 6f6e  f.ai_task_option
+00012930: 6d65 6e75 2e73 6574 2874 6173 6b5f 746f  menu.set(task_to
+00012940: 5f64 6973 706c 6179 290a 2020 2020 2020  _display).      
+00012950: 2020 7365 6c66 2e73 7065 6369 6669 635f    self.specific_
+00012960: 7072 6f6a 6563 745f 6f70 7469 6f6e 6d65  project_optionme
+00012970: 6e75 2e73 6574 2864 6566 6175 6c74 5f70  nu.set(default_p
+00012980: 726f 6a65 6374 290a 2020 2020 2020 2020  roject).        
+00012990: 7365 6c66 2e73 7065 6369 6669 635f 7072  self.specific_pr
+000129a0: 6f66 696c 655f 6f70 7469 6f6e 6d65 6e75  ofile_optionmenu
+000129b0: 2e73 6574 2864 6566 6175 6c74 5f70 726f  .set(default_pro
+000129c0: 6669 6c65 290a 2020 2020 2020 2020 7365  file).        se
+000129d0: 6c66 2e61 695f 7072 6f66 696c 655f 6f70  lf.ai_profile_op
+000129e0: 7469 6f6e 6d65 6e75 2e73 6574 2864 6566  tionmenu.set(def
+000129f0: 6175 6c74 5f70 726f 6669 6c65 290a 2020  ault_profile).  
+00012a00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00012a10: 2320 5365 7420 6465 6661 756c 7473 2066  # Set defaults f
+00012a20: 6f72 2061 6c6c 206f 7074 696f 6e20 6d65  or all option me
+00012a30: 6e75 730a 2020 2020 2020 2020 7365 6c66  nus.        self
+00012a40: 2e73 7065 6369 6669 635f 6e61 6d65 5f6d  .specific_name_m
+00012a50: 7367 203d 2022 220a 2020 2020 2020 2020  sg = "".        
+00012a60: 7365 6c66 2e73 7065 6369 6669 635f 7072  self.specific_pr
+00012a70: 6f6a 6563 745f 6f70 7469 6f6e 6d65 6e75  oject_optionmenu
+00012a80: 2e73 6574 2864 6566 6175 6c74 5f70 726f  .set(default_pro
+00012a90: 6a65 6374 290a 2020 2020 2020 2020 7365  ject).        se
+00012aa0: 6c66 2e73 7065 6369 6669 635f 7072 6f66  lf.specific_prof
+00012ab0: 696c 655f 6f70 7469 6f6e 6d65 6e75 2e73  ile_optionmenu.s
+00012ac0: 6574 2864 6566 6175 6c74 5f70 726f 6669  et(default_profi
+00012ad0: 6c65 290a 2020 2020 2020 2020 7365 6c66  le).        self
+00012ae0: 2e61 695f 7072 6f66 696c 655f 6f70 7469  .ai_profile_opti
+00012af0: 6f6e 6d65 6e75 2e73 6574 2864 6566 6175  onmenu.set(defau
+00012b00: 6c74 5f70 726f 6669 6c65 290a 2020 2020  lt_profile).    
+00012b10: 2020 2020 7365 6c66 2e73 7065 6369 6669      self.specifi
+00012b20: 635f 7461 736b 5f6f 7074 696f 6e6d 656e  c_task_optionmen
+00012b30: 752e 7365 7428 6465 6661 756c 745f 7461  u.set(default_ta
+00012b40: 736b 290a 2020 2020 2020 2020 7365 6c66  sk).        self
+00012b50: 2e61 695f 7461 736b 5f6f 7074 696f 6e6d  .ai_task_optionm
+00012b60: 656e 752e 7365 7428 6465 6661 756c 745f  enu.set(default_
+00012b70: 7461 736b 290a 0a0a 2320 436c 6561 7220  task)...# Clear 
+00012b80: 616c 6c20 5461 736b 6572 2058 4d4c 2064  all Tasker XML d
+00012b90: 6174 6120 6672 6f6d 206d 656d 6f72 7920  ata from memory 
+00012ba0: 736f 2077 6520 7374 6172 7420 616e 6577  so we start anew
+00012bb0: 2e0a 6465 6620 636c 6561 725f 7461 736b  ..def clear_task
+00012bc0: 6572 5f64 6174 6128 2920 2d3e 204e 6f6e  er_data() -> Non
+00012bd0: 653a 0a20 2020 2022 2222 0a20 2020 2043  e:.    """.    C
+00012be0: 6c65 6172 7320 616c 6c20 7468 6520 7461  lears all the ta
+00012bf0: 736b 6572 2064 6174 6120 7374 6f72 6564  sker data stored
+00012c00: 2069 6e20 7468 6520 5072 696d 6549 7465   in the PrimeIte
+00012c10: 6d73 2063 6c61 7373 2e0a 0a20 2020 2054  ms class...    T
+00012c20: 6869 7320 6675 6e63 7469 6f6e 2063 6c65  his function cle
+00012c30: 6172 7320 7468 6520 7461 736b 6572 2064  ars the tasker d
+00012c40: 6174 6120 6279 2063 6c65 6172 696e 6720  ata by clearing 
+00012c50: 7468 6520 666f 6c6c 6f77 696e 6720 6c69  the following li
+00012c60: 7374 733a 0a20 2020 202d 2061 6c6c 5f70  sts:.    - all_p
+00012c70: 726f 6a65 6374 733a 2061 206c 6973 7420  rojects: a list 
+00012c80: 6f66 2061 6c6c 2074 6865 2070 726f 6a65  of all the proje
+00012c90: 6374 730a 2020 2020 2d20 616c 6c5f 7072  cts.    - all_pr
+00012ca0: 6f66 696c 6573 3a20 6120 6c69 7374 206f  ofiles: a list o
+00012cb0: 6620 616c 6c20 7468 6520 7072 6f66 696c  f all the profil
+00012cc0: 6573 0a20 2020 202d 2061 6c6c 5f74 6173  es.    - all_tas
+00012cd0: 6b73 3a20 6120 6c69 7374 206f 6620 616c  ks: a list of al
+00012ce0: 6c20 7468 6520 7461 736b 730a 2020 2020  l the tasks.    
+00012cf0: 2d20 616c 6c5f 7363 656e 6573 3a20 6120  - all_scenes: a 
+00012d00: 6c69 7374 206f 6620 616c 6c20 7468 6520  list of all the 
+00012d10: 7363 656e 6573 0a0a 2020 2020 5468 6973  scenes..    This
+00012d20: 2066 756e 6374 696f 6e20 646f 6573 206e   function does n
+00012d30: 6f74 2074 616b 6520 616e 7920 7061 7261  ot take any para
+00012d40: 6d65 7465 7273 2e0a 0a20 2020 2054 6869  meters...    Thi
+00012d50: 7320 6675 6e63 7469 6f6e 2064 6f65 7320  s function does 
+00012d60: 6e6f 7420 7265 7475 726e 2061 6e79 7468  not return anyth
+00012d70: 696e 672e 0a20 2020 2022 2222 0a20 2020  ing..    """.   
+00012d80: 2023 2047 6574 2072 6964 206f 6620 616e   # Get rid of an
+00012d90: 7920 6461 7461 2077 6520 6375 7272 656e  y data we curren
+00012da0: 746c 7920 6861 7665 0a20 2020 2050 7269  tly have.    Pri
+00012db0: 6d65 4974 656d 732e 7461 736b 6572 5f72  meItems.tasker_r
+00012dc0: 6f6f 745f 656c 656d 656e 7473 5b22 616c  oot_elements["al
+00012dd0: 6c5f 7072 6f6a 6563 7473 225d 2e63 6c65  l_projects"].cle
+00012de0: 6172 2829 0a20 2020 2050 7269 6d65 4974  ar().    PrimeIt
+00012df0: 656d 732e 7461 736b 6572 5f72 6f6f 745f  ems.tasker_root_
+00012e00: 656c 656d 656e 7473 5b22 616c 6c5f 7072  elements["all_pr
+00012e10: 6f66 696c 6573 225d 2e63 6c65 6172 2829  ofiles"].clear()
+00012e20: 0a20 2020 2050 7269 6d65 4974 656d 732e  .    PrimeItems.
+00012e30: 7461 736b 6572 5f72 6f6f 745f 656c 656d  tasker_root_elem
+00012e40: 656e 7473 5b22 616c 6c5f 7461 736b 7322  ents["all_tasks"
+00012e50: 5d2e 636c 6561 7228 290a 2020 2020 5072  ].clear().    Pr
+00012e60: 696d 6549 7465 6d73 2e74 6173 6b65 725f  imeItems.tasker_
+00012e70: 726f 6f74 5f65 6c65 6d65 6e74 735b 2261  root_elements["a
+00012e80: 6c6c 5f73 6365 6e65 7322 5d2e 636c 6561  ll_scenes"].clea
+00012e90: 7228 290a 0a0a 2320 4469 7370 6c61 7920  r()...# Display 
+00012ea0: 6120 7472 6565 2073 7472 7563 7475 7265  a tree structure
+00012eb0: 0a63 6c61 7373 2043 546b 5472 6565 7669  .class CTkTreevi
+00012ec0: 6577 2863 746b 2e43 546b 4672 616d 6529  ew(ctk.CTkFrame)
+00012ed0: 3a0a 2020 2020 2222 2243 6c61 7373 2074  :.    """Class t
+00012ee0: 6f20 6861 6e64 6c65 2074 6865 2054 7265  o handle the Tre
+00012ef0: 6576 6965 770a 0a20 2020 2041 7267 733a  eview..    Args:
+00012f00: 0a20 2020 2020 2020 2063 746b 2028 6374  .        ctk (ct
+00012f10: 6b29 3a20 4f75 7220 4755 4920 6672 616d  k): Our GUI fram
+00012f20: 6577 6f72 6b0a 2020 2020 2222 220a 0a20  ework.    """.. 
+00012f30: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00012f40: 7365 6c66 2c20 6d61 7374 6572 3a20 616e  self, master: an
+00012f50: 792c 2069 7465 6d73 3a20 6c69 7374 2920  y, items: list) 
+00012f60: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00012f70: 2022 2222 4675 6e63 7469 6f6e 3a0a 2020   """Function:.  
+00012f80: 2020 2020 2020 6465 6620 5f5f 696e 6974        def __init
+00012f90: 5f5f 2873 656c 662c 206d 6173 7465 723a  __(self, master:
+00012fa0: 2061 6e79 2c20 6974 656d 733a 206c 6973   any, items: lis
+00012fb0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00012fc0: 496e 6974 6961 6c69 7a65 7320 6120 5472  Initializes a Tr
+00012fd0: 6565 7669 6577 2077 6964 6765 7420 7769  eeview widget wi
+00012fe0: 7468 2061 2067 6976 656e 206d 6173 7465  th a given maste
+00012ff0: 7220 616e 6420 6c69 7374 206f 6620 6974  r and list of it
+00013000: 656d 732e 0a20 2020 2020 2020 2020 2020  ems..           
+00013010: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
+00013020: 2020 2020 2020 2020 2020 2020 206d 6173               mas
+00013030: 7465 7220 2861 6e79 293a 2054 6865 2070  ter (any): The p
+00013040: 6172 656e 7420 7769 6467 6574 2066 6f72  arent widget for
+00013050: 2074 6865 2054 7265 6576 6965 772e 0a20   the Treeview.. 
+00013060: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00013070: 7465 6d73 2028 6c69 7374 293a 2041 206c  tems (list): A l
+00013080: 6973 7420 6f66 2069 7465 6d73 2074 6f20  ist of items to 
+00013090: 6265 2069 6e73 6572 7465 6420 696e 746f  be inserted into
+000130a0: 2074 6865 2054 7265 6576 6965 772e 0a20   the Treeview.. 
+000130b0: 2020 2020 2020 2020 2020 2052 6574 7572             Retur
+000130c0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+000130d0: 2020 2020 4e6f 6e65 2e0a 2020 2020 2020      None..      
+000130e0: 2020 2020 2020 5072 6f63 6573 7369 6e67        Processing
+000130f0: 204c 6f67 6963 3a0a 2020 2020 2020 2020   Logic:.        
+00013100: 2020 2020 2020 2020 2d20 5365 7473 2075          - Sets u
+00013110: 7020 7468 6520 5472 6565 7669 6577 2077  p the Treeview w
+00013120: 6964 6765 7420 7769 7468 2061 7070 726f  idget with appro
+00013130: 7072 6961 7465 2073 7479 6c65 7320 616e  priate styles an
+00013140: 6420 6269 6e64 696e 6773 2e0a 2020 2020  d bindings..    
+00013150: 2020 2020 2020 2020 2020 2020 2d20 496e              - In
+00013160: 7365 7274 7320 7468 6520 6769 7665 6e20  serts the given 
+00013170: 6974 656d 7320 696e 746f 2074 6865 2054  items into the T
+00013180: 7265 6576 6965 772e 0a0a 2020 2020 2020  reeview...      
+00013190: 2020 746b 696e 7465 7220 7472 6565 7669    tkinter treevi
+000131a0: 6577 2063 6f6e 6669 6775 7261 626c 6520  ew configurable 
+000131b0: 6974 656d 733a 0a20 2020 2020 2020 2020  items:.         
+000131c0: 2020 2074 746b 3a3a 7374 796c 6520 636f     ttk::style co
+000131d0: 6e66 6967 7572 6520 5472 6565 7669 6577  nfigure Treeview
+000131e0: 202d 6261 636b 6772 6f75 6e64 2063 6f6c   -background col
+000131f0: 6f72 0a20 2020 2020 2020 2020 2020 2074  or.            t
+00013200: 746b 3a3a 7374 796c 6520 636f 6e66 6967  tk::style config
+00013210: 7572 6520 5472 6565 7669 6577 202d 666f  ure Treeview -fo
+00013220: 7265 6772 6f75 6e64 2063 6f6c 6f72 0a20  reground color. 
+00013230: 2020 2020 2020 2020 2020 2074 746b 3a3a             ttk::
+00013240: 7374 796c 6520 636f 6e66 6967 7572 6520  style configure 
+00013250: 5472 6565 7669 6577 202d 666f 6e74 206e  Treeview -font n
+00013260: 616d 6564 666f 6e74 0a20 2020 2020 2020  amedfont.       
+00013270: 2020 2020 2074 746b 3a3a 7374 796c 6520       ttk::style 
+00013280: 636f 6e66 6967 7572 6520 5472 6565 7669  configure Treevi
+00013290: 6577 202d 6669 656c 6462 6163 6b67 726f  ew -fieldbackgro
+000132a0: 756e 6420 636f 6c6f 720a 2020 2020 2020  und color.      
+000132b0: 2020 2020 2020 7474 6b3a 3a73 7479 6c65        ttk::style
+000132c0: 206d 6170 2054 7265 6576 6965 7720 2d62   map Treeview -b
+000132d0: 6163 6b67 726f 756e 6420 5c0a 2020 2020  ackground \.    
+000132e0: 2020 2020 2020 2020 2020 2020 5b6c 6973              [lis
+000132f0: 7420 7365 6c65 6374 6564 2063 6f6c 6f72  t selected color
+00013300: 5d0a 2020 2020 2020 2020 2020 2020 7474  ].            tt
+00013310: 6b3a 3a73 7479 6c65 206d 6170 2054 7265  k::style map Tre
+00013320: 6576 6965 7720 2d66 6f72 6567 726f 756e  eview -foregroun
+00013330: 6420 5c0a 2020 2020 2020 2020 2020 2020  d \.            
+00013340: 2020 2020 5b6c 6973 7420 7365 6c65 6374      [list select
+00013350: 6564 2063 6f6c 6f72 5d0a 2020 2020 2020  ed color].      
+00013360: 2020 2020 2020 7474 6b3a 3a73 7479 6c65        ttk::style
+00013370: 2063 6f6e 6669 6775 7265 2054 7265 6576   configure Treev
+00013380: 6965 7720 2d72 6f77 6865 6967 6874 205b  iew -rowheight [
+00013390: 6578 7072 207b 5b66 6f6e 7420 6d65 7472  expr {[font metr
+000133a0: 6963 7320 6e61 6d65 6466 6f6e 7420 2d6c  ics namedfont -l
+000133b0: 696e 6573 7061 6365 5d20 2b20 327d 5d0a  inespace] + 2}].
+000133c0: 2020 2020 2020 2020 2020 2020 7474 6b3a              ttk:
+000133d0: 3a73 7479 6c65 2063 6f6e 6669 6775 7265  :style configure
+000133e0: 2048 6561 6469 6e67 202d 666f 6e74 206e   Heading -font n
+000133f0: 616d 6564 666f 6e74 0a20 2020 2020 2020  amedfont.       
+00013400: 2020 2020 2074 746b 3a3a 7374 796c 6520       ttk::style 
+00013410: 636f 6e66 6967 7572 6520 4865 6164 696e  configure Headin
+00013420: 6720 2d62 6163 6b67 726f 756e 6420 636f  g -background co
+00013430: 6c6f 720a 2020 2020 2020 2020 2020 2020  lor.            
+00013440: 7474 6b3a 3a73 7479 6c65 2063 6f6e 6669  ttk::style confi
+00013450: 6775 7265 2048 6561 6469 6e67 202d 666f  gure Heading -fo
+00013460: 7265 6772 6f75 6e64 2063 6f6c 6f72 0a20  reground color. 
+00013470: 2020 2020 2020 2020 2020 2074 746b 3a3a             ttk::
+00013480: 7374 796c 6520 636f 6e66 6967 7572 6520  style configure 
+00013490: 4865 6164 696e 6720 2d70 6164 6469 6e67  Heading -padding
+000134a0: 2070 6164 6469 6e67 0a20 2020 2020 2020   padding.       
+000134b0: 2020 2020 2074 746b 3a3a 7374 796c 6520       ttk::style 
+000134c0: 636f 6e66 6967 7572 6520 4974 656d 202d  configure Item -
+000134d0: 666f 7265 6772 6f75 6e64 2063 6f6c 6f72  foreground color
+000134e0: 0a20 2020 2020 2020 2020 2020 2074 746b  .            ttk
+000134f0: 3a3a 7374 796c 6520 636f 6e66 6967 7572  ::style configur
+00013500: 6520 4974 656d 202d 666f 6375 7363 6f6c  e Item -focuscol
+00013510: 6f72 2063 6f6c 6f72 0a20 2020 2020 2020  or color.       
+00013520: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
+00013530: 662e 726f 6f74 203d 206d 6173 7465 720a  f.root = master.
+00013540: 2020 2020 2020 2020 7365 6c66 2e69 7465          self.ite
+00013550: 6d73 203d 2069 7465 6d73 0a20 2020 2020  ms = items.     
+00013560: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00013570: 745f 5f28 7365 6c66 2e72 6f6f 7429 0a0a  t__(self.root)..
+00013580: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
+00013590: 645f 636f 6c75 6d6e 636f 6e66 6967 7572  d_columnconfigur
+000135a0: 6528 302c 2077 6569 6768 743d 3129 0a0a  e(0, weight=1)..
+000135b0: 2020 2020 2020 2020 2320 4c61 6265 6c20          # Label 
+000135c0: 7769 6467 6574 0a20 2020 2020 2020 206f  widget.        o
+000135d0: 7572 5f6c 6162 656c 203d 2022 2222 0a44  ur_label = """.D
+000135e0: 7261 6720 7468 6520 626f 7474 6f6d 206f  rag the bottom o
+000135f0: 6620 7468 6520 7769 6e64 6f77 2074 6f20  f the window to 
+00013600: 6578 7061 6e64 2061 7320 6e65 6564 6564  expand as needed
+00013610: 2e5c 6e0a 436c 6963 6b20 6974 656d 2061  .\n.Click item a
+00013620: 6e64 2073 6372 6f6c 6c20 6d6f 7573 652d  nd scroll mouse-
+00013630: 7768 6565 6c2f 7472 6163 6b70 6164 5c6e  wheel/trackpad\n
+00013640: 6173 206e 6565 6465 6420 746f 2067 6f20  as needed to go 
+00013650: 7570 206f 7220 646f 776e 2e0a 2020 2020  up or down..    
+00013660: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00013670: 7365 6c66 2e6c 6162 656c 203d 2063 746b  self.label = ctk
+00013680: 2e43 546b 4c61 6265 6c28 6d61 7374 6572  .CTkLabel(master
+00013690: 3d73 656c 662c 2074 6578 743d 6f75 725f  =self, text=our_
+000136a0: 6c61 6265 6c2c 2066 6f6e 743d 2822 222c  label, font=("",
+000136b0: 2031 3229 290a 2020 2020 2020 2020 7365   12)).        se
+000136c0: 6c66 2e6c 6162 656c 2e67 7269 6428 726f  lf.label.grid(ro
+000136d0: 773d 302c 2063 6f6c 756d 6e3d 302c 2070  w=0, column=0, p
+000136e0: 6164 783d 3130 2c20 7061 6479 3d31 302c  adx=10, pady=10,
+000136f0: 2073 7469 636b 793d 2265 7722 290a 0a20   sticky="ew").. 
+00013700: 2020 2020 2020 2023 2042 6173 6963 2061         # Basic a
+00013710: 7070 6561 7261 6e63 6520 666f 7220 7465  ppearance for te
+00013720: 7874 2c20 666f 7265 6772 6f75 6e64 2061  xt, foreground a
+00013730: 6e64 2062 6163 6b67 726f 756e 642e 0a20  nd background.. 
+00013740: 2020 2020 2020 2073 656c 662e 6267 5f63         self.bg_c
+00013750: 6f6c 6f72 203d 2073 656c 662e 726f 6f74  olor = self.root
+00013760: 2e5f 6170 706c 795f 6170 7065 6172 616e  ._apply_appearan
+00013770: 6365 5f6d 6f64 6528 6374 6b2e 5468 656d  ce_mode(ctk.Them
+00013780: 654d 616e 6167 6572 2e74 6865 6d65 5b22  eManager.theme["
+00013790: 4354 6b46 7261 6d65 225d 5b22 6667 5f63  CTkFrame"]["fg_c
+000137a0: 6f6c 6f72 225d 2920 2023 206e 6f71 613a  olor"])  # noqa:
+000137b0: 2053 4c46 3030 310a 2020 2020 2020 2020   SLF001.        
+000137c0: 7365 6c66 2e74 6578 745f 636f 6c6f 7220  self.text_color 
+000137d0: 3d20 7365 6c66 2e72 6f6f 742e 5f61 7070  = self.root._app
+000137e0: 6c79 5f61 7070 6561 7261 6e63 655f 6d6f  ly_appearance_mo
+000137f0: 6465 2820 2023 206e 6f71 613a 2053 4c46  de(  # noqa: SLF
+00013800: 3030 310a 2020 2020 2020 2020 2020 2020  001.            
+00013810: 6374 6b2e 5468 656d 654d 616e 6167 6572  ctk.ThemeManager
+00013820: 2e74 6865 6d65 5b22 4354 6b4c 6162 656c  .theme["CTkLabel
+00013830: 225d 5b22 7465 7874 5f63 6f6c 6f72 225d  "]["text_color"]
+00013840: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00013850: 2020 2020 7365 6c66 2e73 656c 6563 7465      self.selecte
+00013860: 645f 636f 6c6f 7220 3d20 7365 6c66 2e72  d_color = self.r
+00013870: 6f6f 742e 5f61 7070 6c79 5f61 7070 6561  oot._apply_appea
+00013880: 7261 6e63 655f 6d6f 6465 2820 2023 206e  rance_mode(  # n
+00013890: 6f71 613a 2053 4c46 3030 310a 2020 2020  oqa: SLF001.    
+000138a0: 2020 2020 2020 2020 6374 6b2e 5468 656d          ctk.Them
+000138b0: 654d 616e 6167 6572 2e74 6865 6d65 5b22  eManager.theme["
+000138c0: 4354 6b42 7574 746f 6e22 5d5b 2266 675f  CTkButton"]["fg_
+000138d0: 636f 6c6f 7222 5d2c 0a20 2020 2020 2020  color"],.       
+000138e0: 2029 0a0a 2020 2020 2020 2020 2320 5365   )..        # Se
+000138f0: 7420 7570 2074 6865 2073 7479 6c65 2f74  t up the style/t
+00013900: 6865 6d65 0a20 2020 2020 2020 2073 656c  heme.        sel
+00013910: 662e 7472 6565 5f73 7479 6c65 203d 2074  f.tree_style = t
+00013920: 746b 2e53 7479 6c65 2873 656c 6629 0a20  tk.Style(self). 
+00013930: 2020 2020 2020 2073 656c 662e 7472 6565         self.tree
+00013940: 5f73 7479 6c65 2e74 6865 6d65 5f75 7365  _style.theme_use
+00013950: 2822 6465 6661 756c 7422 290a 0a20 2020  ("default")..   
+00013960: 2020 2020 2023 2047 7465 7468 2074 6865       # Gteth the
+00013970: 2069 636f 6e73 2074 6f20 6265 2075 7365   icons to be use
+00013980: 6420 696e 2074 6865 2054 7265 6520 7669  d in the Tree vi
+00013990: 6577 2e0a 2020 2020 2020 2020 7365 6c66  ew..        self
+000139a0: 2e69 6d5f 6f70 656e 203d 2049 6d61 6765  .im_open = Image
+000139b0: 2e6f 7065 6e28 4943 4f4e 5f50 4154 485b  .open(ICON_PATH[
+000139c0: 2261 7272 6f77 225d 290a 2020 2020 2020  "arrow"]).      
+000139d0: 2020 7365 6c66 2e69 6d5f 636c 6f73 6520    self.im_close 
+000139e0: 3d20 7365 6c66 2e69 6d5f 6f70 656e 2e72  = self.im_open.r
+000139f0: 6f74 6174 6528 3930 290a 2020 2020 2020  otate(90).      
+00013a00: 2020 7365 6c66 2e69 6d5f 656d 7074 7920    self.im_empty 
+00013a10: 3d20 496d 6167 652e 6e65 7728 2252 4742  = Image.new("RGB
+00013a20: 4122 2c20 2831 352c 2031 3529 2c20 2223  A", (15, 15), "#
+00013a30: 3030 3030 3030 3030 2229 0a0a 2020 2020  00000000")..    
+00013a40: 2020 2020 7365 6c66 2e69 6d67 5f6f 7065      self.img_ope
+00013a50: 6e20 3d20 496d 6167 6554 6b2e 5068 6f74  n = ImageTk.Phot
+00013a60: 6f49 6d61 6765 2873 656c 662e 696d 5f6f  oImage(self.im_o
+00013a70: 7065 6e2c 206e 616d 653d 2269 6d67 5f6f  pen, name="img_o
+00013a80: 7065 6e22 2c20 7369 7a65 3d28 3135 2c20  pen", size=(15, 
+00013a90: 3135 2929 0a20 2020 2020 2020 2073 656c  15)).        sel
+00013aa0: 662e 696d 675f 636c 6f73 6520 3d20 496d  f.img_close = Im
+00013ab0: 6167 6554 6b2e 5068 6f74 6f49 6d61 6765  ageTk.PhotoImage
+00013ac0: 2873 656c 662e 696d 5f63 6c6f 7365 2c20  (self.im_close, 
+00013ad0: 6e61 6d65 3d22 696d 675f 636c 6f73 6522  name="img_close"
+00013ae0: 2c20 7369 7a65 3d28 3135 2c20 3135 2929  , size=(15, 15))
+00013af0: 0a20 2020 2020 2020 2073 656c 662e 696d  .        self.im
+00013b00: 675f 656d 7074 7920 3d20 496d 6167 6554  g_empty = ImageT
+00013b10: 6b2e 5068 6f74 6f49 6d61 6765 2873 656c  k.PhotoImage(sel
+00013b20: 662e 696d 5f65 6d70 7479 2c20 6e61 6d65  f.im_empty, name
+00013b30: 3d22 696d 675f 656d 7074 7922 2c20 7369  ="img_empty", si
+00013b40: 7a65 3d28 3135 2c20 3135 2929 0a0a 2020  ze=(15, 15))..  
+00013b50: 2020 2020 2020 2320 4172 726f 7720 656c        # Arrow el
+00013b60: 656d 656e 7420 636f 6e66 6967 7572 6174  ement configurat
+00013b70: 696f 6e0a 2020 2020 2020 2020 7769 7468  ion.        with
+00013b80: 2063 6f6e 7465 7874 6c69 622e 7375 7070   contextlib.supp
+00013b90: 7265 7373 2854 636c 4572 726f 7229 3a20  ress(TclError): 
+00013ba0: 2023 2044 6f6e 2774 2074 6872 6f77 2065   # Don't throw e
+00013bb0: 7272 6f72 2069 6620 7468 6520 656c 656d  rror if the elem
+00013bc0: 656e 7420 616c 7265 6164 7920 6578 6973  ent already exis
+00013bd0: 7473 2e20 204a 7573 7420 7265 7573 6520  ts.  Just reuse 
+00013be0: 6974 2e0a 2020 2020 2020 2020 2020 2020  it..            
+00013bf0: 7365 6c66 2e74 7265 655f 7374 796c 652e  self.tree_style.
+00013c00: 656c 656d 656e 745f 6372 6561 7465 280a  element_create(.
+00013c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c20: 2254 7265 6569 7465 6d2e 6d79 696e 6469  "Treeitem.myindi
+00013c30: 6361 746f 7222 2c0a 2020 2020 2020 2020  cator",.        
+00013c40: 2020 2020 2020 2020 2269 6d61 6765 222c          "image",
+00013c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013c60: 2022 696d 675f 636c 6f73 6522 2c0a 2020   "img_close",.  
+00013c70: 2020 2020 2020 2020 2020 2020 2020 2822                ("
+00013c80: 7573 6572 3122 2c20 2221 7573 6572 3222  user1", "!user2"
+00013c90: 2c20 2269 6d67 5f6f 7065 6e22 292c 0a20  , "img_open"),. 
+00013ca0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00013cb0: 2275 7365 7232 222c 2022 696d 675f 656d  "user2", "img_em
+00013cc0: 7074 7922 292c 0a20 2020 2020 2020 2020  pty"),.         
+00013cd0: 2020 2020 2020 2073 7469 636b 793d 2277         sticky="w
+00013ce0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00013cf0: 2020 2077 6964 7468 3d31 352c 0a20 2020     width=15,.   
+00013d00: 2020 2020 2020 2020 2020 2020 2068 6569               hei
+00013d10: 6768 743d 3135 2c0a 2020 2020 2020 2020  ght=15,.        
+00013d20: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+00013d30: 2054 7265 6576 6965 7720 636f 6e66 6967   Treeview config
+00013d40: 7572 6174 696f 6e20 6f66 2074 6865 2074  uration of the t
+00013d50: 7265 6576 6965 770a 2020 2020 2020 2020  reeview.        
+00013d60: 7365 6c66 2e74 7265 655f 7374 796c 652e  self.tree_style.
+00013d70: 6c61 796f 7574 280a 2020 2020 2020 2020  layout(.        
+00013d80: 2020 2020 2254 7265 6576 6965 772e 4974      "Treeview.It
+00013d90: 656d 222c 0a20 2020 2020 2020 2020 2020  em",.           
+00013da0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00013db0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
+00013dc0: 2020 2020 2020 2020 2022 5472 6565 6974           "Treeit
+00013dd0: 656d 2e70 6164 6469 6e67 222c 0a20 2020  em.padding",.   
+00013de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013df0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00013e00: 2020 2020 2020 2020 2020 2022 7374 6963             "stic
+00013e10: 6b79 223a 2022 6e73 6577 222c 0a20 2020  ky": "nsew",.   
+00013e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e30: 2020 2020 2022 6368 696c 6472 656e 223a       "children":
+00013e40: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00013e50: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00013e60: 2254 7265 6569 7465 6d2e 6d79 696e 6469  "Treeitem.myindi
+00013e70: 6361 746f 7222 2c20 7b22 7369 6465 223a  cator", {"side":
+00013e80: 2022 6c65 6674 222c 2022 7374 6963 6b79   "left", "sticky
+00013e90: 223a 2022 6e73 6577 227d 292c 0a20 2020  ": "nsew"}),.   
+00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013eb0: 2020 2020 2020 2020 2028 2254 7265 6569           ("Treei
+00013ec0: 7465 6d2e 696d 6167 6522 2c20 7b22 7369  tem.image", {"si
+00013ed0: 6465 223a 2022 6c65 6674 222c 2022 7374  de": "left", "st
+00013ee0: 6963 6b79 223a 2022 6e73 6577 227d 292c  icky": "nsew"}),
+00013ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013f00: 2020 2020 2020 2020 2020 2020 2028 0a20               (. 
+00013f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00013f30: 5472 6565 6974 656d 2e66 6f63 7573 222c  Treeitem.focus",
+00013f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f60: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00013f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f80: 2020 2020 2020 2022 7369 6465 223a 2022         "side": "
+00013f90: 6c65 6674 222c 0a20 2020 2020 2020 2020  left",.         
+00013fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fb0: 2020 2020 2020 2020 2020 2022 7374 6963             "stic
+00013fc0: 6b79 223a 2022 6e73 6577 222c 0a20 2020  ky": "nsew",.   
+00013fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ff0: 2022 6368 696c 6472 656e 223a 205b 2822   "children": [("
+00014000: 5472 6565 6974 656d 2e74 6578 7422 2c20  Treeitem.text", 
+00014010: 7b22 7369 6465 223a 2022 6c65 6674 222c  {"side": "left",
+00014020: 2022 7374 6963 6b79 223a 2022 6e73 6577   "sticky": "nsew
+00014030: 227d 295d 2c0a 2020 2020 2020 2020 2020  "})],.          
+00014040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014050: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00014060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014070: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014090: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+000140a0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000140b0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+000140c0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+000140d0: 2020 2020 290a 0a20 2020 2020 2020 2073      )..        s
+000140e0: 656c 662e 7472 6565 5f73 7479 6c65 2e63  elf.tree_style.c
+000140f0: 6f6e 6669 6775 7265 280a 2020 2020 2020  onfigure(.      
+00014100: 2020 2020 2020 2254 7265 6576 6965 7722        "Treeview"
+00014110: 2c0a 2020 2020 2020 2020 2020 2020 6261  ,.            ba
+00014120: 636b 6772 6f75 6e64 3d73 656c 662e 6267  ckground=self.bg
+00014130: 5f63 6f6c 6f72 2c0a 2020 2020 2020 2020  _color,.        
+00014140: 2020 2020 666f 7265 6772 6f75 6e64 3d73      foreground=s
+00014150: 656c 662e 7465 7874 5f63 6f6c 6f72 2c0a  elf.text_color,.
+00014160: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
+00014170: 6462 6163 6b67 726f 756e 643d 7365 6c66  dbackground=self
+00014180: 2e62 675f 636f 6c6f 722c 0a20 2020 2020  .bg_color,.     
+00014190: 2020 2020 2020 2062 6f72 6465 7277 6964         borderwid
+000141a0: 7468 3d31 302c 2020 2320 4465 6669 6e65  th=10,  # Define
+000141b0: 2061 2062 6f72 6465 7220 6172 6f75 6e64   a border around
+000141c0: 2074 7265 6520 6f66 2031 3020 7069 7865   tree of 10 pixe
+000141d0: 6c73 2e0a 2020 2020 2020 2020 2020 2020  ls..            
+000141e0: 666f 6e74 3d28 2222 2c20 3132 292c 0a20  font=("", 12),. 
+000141f0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00014200: 2020 7365 6c66 2e74 7265 655f 7374 796c    self.tree_styl
+00014210: 652e 6d61 7028 0a20 2020 2020 2020 2020  e.map(.         
+00014220: 2020 2022 5472 6565 7669 6577 222c 0a20     "Treeview",. 
+00014230: 2020 2020 2020 2020 2020 2062 6163 6b67             backg
+00014240: 726f 756e 643d 5b28 2273 656c 6563 7465  round=[("selecte
+00014250: 6422 2c20 7365 6c66 2e62 675f 636f 6c6f  d", self.bg_colo
+00014260: 7229 5d2c 0a20 2020 2020 2020 2020 2020  r)],.           
+00014270: 2066 6f72 6567 726f 756e 643d 5b28 2273   foreground=[("s
+00014280: 656c 6563 7465 6422 2c20 7365 6c66 2e73  elected", self.s
+00014290: 656c 6563 7465 645f 636f 6c6f 7229 5d2c  elected_color)],
+000142a0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000142b0: 2020 2073 656c 662e 726f 6f74 2e62 696e     self.root.bin
+000142c0: 6428 223c 3c54 7265 6576 6965 7753 656c  d("<<TreeviewSel
+000142d0: 6563 743e 3e22 2c20 6c61 6d62 6461 2065  ect>>", lambda e
+000142e0: 7665 6e74 3a20 7365 6c66 2e72 6f6f 742e  vent: self.root.
+000142f0: 666f 6375 735f 7365 7428 2929 2020 2320  focus_set())  # 
+00014300: 6e6f 7161 3a20 4152 4730 3035 0a0a 2020  noqa: ARG005..  
+00014310: 2020 2020 2020 2320 4465 6669 6e65 2074        # Define t
+00014320: 6865 2066 7261 6d65 2066 6f72 2074 6865  he frame for the
+00014330: 2074 7265 6576 6965 770a 2020 2020 2020   treeview.      
+00014340: 2020 7365 6c66 2e74 7265 6576 6965 7720    self.treeview 
+00014350: 3d20 7474 6b2e 5472 6565 7669 6577 2873  = ttk.Treeview(s
+00014360: 656c 662c 2073 686f 773d 2274 7265 6522  elf, show="tree"
+00014370: 2c20 6865 6967 6874 3d35 302c 2073 656c  , height=50, sel
+00014380: 6563 746d 6f64 653d 2262 726f 7773 6522  ectmode="browse"
+00014390: 290a 0a20 2020 2020 2020 2023 2044 6566  )..        # Def
+000143a0: 696e 6520 7468 6520 7769 6474 6820 6f66  ine the width of
+000143b0: 2074 6865 2063 6f6c 756d 6e20 696e 746f   the column into
+000143c0: 2077 6869 6368 2074 6865 2074 7265 6520   which the tree 
+000143d0: 7769 6c6c 2062 6520 706c 6163 6564 2e0a  will be placed..
+000143e0: 2020 2020 2020 2020 7365 6c66 2e74 7265          self.tre
+000143f0: 6576 6965 775b 2263 6f6c 756d 6e73 225d  eview["columns"]
+00014400: 203d 205b 305d 0a20 2020 2020 2020 2023   = [0].        #
+00014410: 2073 656c 662e 7472 6565 7669 6577 2e63   self.treeview.c
+00014420: 6f6c 756d 6e28 302c 2073 7472 6574 6368  olumn(0, stretch
+00014430: 3d30 2c20 616e 6368 6f72 3d22 7722 2c20  =0, anchor="w", 
+00014440: 7769 6474 683d 3135 302c 206d 696e 7769  width=150, minwi
+00014450: 6474 683d 3135 3029 0a20 2020 2020 2020  dth=150).       
+00014460: 2023 2054 6f20 636f 6e66 6967 7572 6520   # To configure 
+00014470: 7468 6520 7472 6565 2063 6f6c 756d 6e2c  the tree column,
+00014480: 2063 616c 6c20 7468 6973 2077 6974 6820   call this with 
+00014490: 636f 6c75 6d6e 203d 20e2 809c 2330 e280  column = ...#0..
+000144a0: 9d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+000144b0: 7265 6576 6965 772e 636f 6c75 6d6e 2822  reeview.column("
+000144c0: 2330 222c 2073 7472 6574 6368 3d30 2c20  #0", stretch=0, 
+000144d0: 616e 6368 6f72 3d22 7722 2c20 7769 6474  anchor="w", widt
+000144e0: 683d 3330 302c 206d 696e 7769 6474 683d  h=300, minwidth=
+000144f0: 3230 3029 0a0a 2020 2020 2020 2020 7365  200)..        se
+00014500: 6c66 2e74 7265 6576 6965 772e 6772 6964  lf.treeview.grid
+00014510: 2872 6f77 3d31 2c20 636f 6c75 6d6e 3d30  (row=1, column=0
+00014520: 2c20 7061 6478 3d31 302c 2070 6164 793d  , padx=10, pady=
+00014530: 3130 2c20 7374 6963 6b79 3d22 7722 290a  10, sticky="w").
+00014540: 0a20 2020 2020 2020 2023 2041 6464 2069  .        # Add i
+00014550: 7465 6d73 2074 6f20 7468 6520 7472 6565  tems to the tree
+00014560: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00014570: 7365 7274 5f69 7465 6d73 2873 656c 662e  sert_items(self.
+00014580: 6974 656d 7329 0a0a 2020 2020 2320 496e  items)..    # In
+00014590: 7365 7420 6974 656d 7320 696e 746f 2074  set items into t
+000145a0: 6865 2074 7265 6576 6965 772e 0a20 2020  he treeview..   
+000145b0: 2064 6566 2069 6e73 6572 745f 6974 656d   def insert_item
+000145c0: 7328 7365 6c66 2c20 6974 656d 733a 206c  s(self, items: l
+000145d0: 6973 742c 2070 6172 656e 743d 2222 2920  ist, parent="") 
+000145e0: 2d3e 204e 6f6e 653a 2020 2320 6e6f 7161  -> None:  # noqa
+000145f0: 3a20 414e 4e30 3031 0a20 2020 2020 2020  : ANN001.       
+00014600: 2022 2222 496e 7365 7274 7320 6974 656d   """Inserts item
+00014610: 7320 696e 746f 2061 2074 7265 6576 6965  s into a treevie
+00014620: 772e 0a20 2020 2020 2020 2050 6172 616d  w..        Param
+00014630: 6574 6572 733a 0a20 2020 2020 2020 2020  eters:.         
+00014640: 2020 2069 7465 6d73 2028 6c69 7374 293a     items (list):
+00014650: 204c 6973 7420 6f66 2069 7465 6d73 2074   List of items t
+00014660: 6f20 6265 2069 6e73 6572 7465 642e 0a20  o be inserted.. 
+00014670: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+00014680: 7420 2873 7472 293a 204f 7074 696f 6e61  t (str): Optiona
+00014690: 6c20 7061 7265 6e74 2069 7465 6d20 666f  l parent item fo
+000146a0: 7220 7468 6520 696e 7365 7274 6564 2069  r the inserted i
+000146b0: 7465 6d73 2e0a 2020 2020 2020 2020 5265  tems..        Re
+000146c0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+000146d0: 2020 204e 6f6e 653a 2044 6f65 7320 6e6f     None: Does no
+000146e0: 7420 7265 7475 726e 2061 6e79 7468 696e  t return anythin
+000146f0: 672e 0a20 2020 2020 2020 2050 726f 6365  g..        Proce
+00014700: 7373 696e 6720 4c6f 6769 633a 0a20 2020  ssing Logic:.   
+00014710: 2020 2020 2020 2020 202d 2049 6e73 6572           - Inser
+00014720: 7473 2069 7465 6d73 2069 6e74 6f20 7472  ts items into tr
+00014730: 6565 7669 6577 2e0a 2020 2020 2020 2020  eeview..        
+00014740: 2020 2020 2d20 4966 2069 7465 6d20 6973      - If item is
+00014750: 2061 2064 6963 7469 6f6e 6172 792c 2069   a dictionary, i
+00014760: 6e73 6572 7420 7769 7468 2069 642e 0a20  nsert with id.. 
+00014770: 2020 2020 2020 2020 2020 202d 2049 6620             - If 
+00014780: 6974 656d 2069 7320 6e6f 7420 6120 6469  item is not a di
+00014790: 6374 696f 6e61 7279 2c20 696e 7365 7274  ctionary, insert
+000147a0: 2077 6974 686f 7574 2069 642e 2222 220a   without id.""".
+000147b0: 2020 2020 2020 2020 666f 7220 6974 656d          for item
+000147c0: 2069 6e20 6974 656d 733a 0a20 2020 2020   in items:.     
+000147d0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+000147e0: 616e 6365 2869 7465 6d2c 2064 6963 7429  ance(item, dict)
+000147f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014800: 2020 7468 655f 6964 203d 2073 656c 662e    the_id = self.
+00014810: 7472 6565 7669 6577 2e69 6e73 6572 7428  treeview.insert(
+00014820: 7061 7265 6e74 2c20 2265 6e64 222c 2074  parent, "end", t
+00014830: 6578 743d 6974 656d 5b22 6e61 6d65 225d  ext=item["name"]
+00014840: 2e6c 6a75 7374 2835 3029 290a 2020 2020  .ljust(50)).    
+00014850: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00014860: 2063 6f6e 7465 7874 6c69 622e 7375 7070   contextlib.supp
+00014870: 7265 7373 284b 6579 4572 726f 7229 3a0a  ress(KeyError):.
+00014880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014890: 2020 2020 7365 6c66 2e69 6e73 6572 745f      self.insert_
+000148a0: 6974 656d 7328 6974 656d 5b22 6368 696c  items(item["chil
+000148b0: 6472 656e 225d 2c20 7468 655f 6964 290a  dren"], the_id).
+000148c0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000148d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000148e0: 2020 7365 6c66 2e74 7265 6576 6965 772e    self.treeview.
+000148f0: 696e 7365 7274 2870 6172 656e 742c 2022  insert(parent, "
+00014900: 656e 6422 2c20 7465 7874 3d69 7465 6d29  end", text=item)
+00014910: 0a0a 0a23 2044 6566 696e 6520 7468 6520  ...# Define the 
+00014920: 5472 6565 7669 6577 2077 696e 646f 770a  Treeview window.
+00014930: 636c 6173 7320 5472 6565 7669 6577 5769  class TreeviewWi
+00014940: 6e64 6f77 2863 746b 2e43 546b 546f 706c  ndow(ctk.CTkTopl
+00014950: 6576 656c 293a 0a20 2020 2022 2222 4465  evel):.    """De
+00014960: 6669 6e65 206f 7572 2074 6f70 206c 6576  fine our top lev
+00014970: 656c 2077 696e 646f 7720 666f 7220 7468  el window for th
+00014980: 6520 7472 6565 2076 6965 772e 2222 220a  e tree view.""".
+00014990: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000149a0: 5f28 7365 6c66 2c20 2a61 7267 732c 202a  _(self, *args, *
+000149b0: 2a6b 7761 7267 7329 202d 3e20 4e6f 6e65  *kwargs) -> None
+000149c0: 3a20 2023 206e 6f71 613a 2041 4e4e 3030  :  # noqa: ANN00
+000149d0: 322c 2041 4e4e 3030 330a 2020 2020 2020  2, ANN003.      
+000149e0: 2020 2222 2243 7265 6174 6573 2061 206c    """Creates a l
+000149f0: 6162 656c 2077 6964 6765 7420 666f 7220  abel widget for 
+00014a00: 6120 7472 6565 2076 6965 772e 0a20 2020  a tree view..   
+00014a10: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
+00014a20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00014a30: 6620 286f 626a 6563 7429 3a20 5468 6520  f (object): The 
+00014a40: 6f62 6a65 6374 2062 6569 6e67 2070 6173  object being pas
+00014a50: 7365 642e 0a20 2020 2020 2020 2020 2020  sed..           
+00014a60: 202a 6172 6773 2028 616e 7929 3a20 4164   *args (any): Ad
+00014a70: 6469 7469 6f6e 616c 2061 7267 756d 656e  ditional argumen
+00014a80: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
+00014a90: 2a2a 6b77 6172 6773 2028 616e 7929 3a20  **kwargs (any): 
+00014aa0: 4164 6469 7469 6f6e 616c 206b 6579 776f  Additional keywo
+00014ab0: 7264 2061 7267 756d 656e 7473 2e0a 2020  rd arguments..  
+00014ac0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00014ad0: 2020 2020 2020 2020 2020 204e 6f6e 653a             None:
+00014ae0: 2054 6869 7320 6675 6e63 7469 6f6e 2064   This function d
+00014af0: 6f65 7320 6e6f 7420 7265 7475 726e 2061  oes not return a
+00014b00: 6e79 7468 696e 672e 0a20 2020 2020 2020  nything..       
+00014b10: 2050 726f 6365 7373 696e 6720 4c6f 6769   Processing Logi
+00014b20: 633a 0a20 2020 2020 2020 2020 2020 202d  c:.            -
+00014b30: 2049 6e69 7469 616c 697a 6520 6c61 6265   Initialize labe
+00014b40: 6c20 7769 6467 6574 2e0a 2020 2020 2020  l widget..      
+00014b50: 2020 2020 2020 2d20 5061 636b 206c 6162        - Pack lab
+00014b60: 656c 2077 6964 6765 7420 7769 7468 2070  el widget with p
+00014b70: 6164 6469 6e67 2e0a 2020 2020 2020 2020  adding..        
+00014b80: 2020 2020 2d20 5365 7420 6c61 6265 6c20      - Set label 
+00014b90: 7769 6467 6574 2074 6578 742e 2222 220a  widget text.""".
+00014ba0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00014bb0: 5f5f 696e 6974 5f5f 282a 6172 6773 2c20  __init__(*args, 
+00014bc0: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
+00014bd0: 2020 7365 6c66 2e67 656f 6d65 7472 7928    self.geometry(
+00014be0: 2236 3030 7836 3030 2229 0a20 2020 2020  "600x600").     
+00014bf0: 2020 2073 656c 662e 7469 746c 6528 224d     self.title("M
+00014c00: 6170 5461 736b 6572 2043 6f6e 6669 6775  apTasker Configu
+00014c10: 7261 7469 6f6e 2054 7265 6576 6965 7722  ration Treeview"
+00014c20: 290a 0a0a 2320 4469 7370 6c61 7920 6120  )...# Display a 
+00014c30: 416e 616c 7973 6973 2073 7472 7563 7475  Analysis structu
+00014c40: 7265 0a63 6c61 7373 2043 546b 416e 616c  re.class CTkAnal
+00014c50: 7973 6973 7669 6577 2863 746b 2e43 546b  ysisview(ctk.CTk
+00014c60: 4672 616d 6529 3a0a 2020 2020 2222 2243  Frame):.    """C
+00014c70: 6c61 7373 2074 6f20 6861 6e64 6c65 2074  lass to handle t
+00014c80: 6865 2054 7265 6576 6965 770a 0a20 2020  he Treeview..   
+00014c90: 2041 7267 733a 0a20 2020 2020 2020 2063   Args:.        c
+00014ca0: 746b 2028 6374 6b29 3a20 4f75 7220 4755  tk (ctk): Our GU
+00014cb0: 4920 6672 616d 6577 6f72 6b0a 2020 2020  I framework.    
+00014cc0: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
+00014cd0: 6e69 745f 5f28 7365 6c66 2c20 6d61 7374  nit__(self, mast
+00014ce0: 6572 3a20 616e 792c 206d 6573 7361 6765  er: any, message
+00014cf0: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
+00014d00: 2020 2020 2020 2020 2222 2246 756e 6374          """Funct
+00014d10: 696f 6e3a 0a20 2020 2020 2020 2064 6566  ion:.        def
+00014d20: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00014d30: 6d61 7374 6572 3a20 616e 792c 2069 7465  master: any, ite
+00014d40: 6d73 3a20 6c69 7374 293a 0a20 2020 2020  ms: list):.     
+00014d50: 2020 2020 2020 2049 6e69 7469 616c 697a         Initializ
+00014d60: 6573 2061 2041 6e61 6c79 7369 7376 6965  es a Analysisvie
+00014d70: 7720 7769 6467 6574 2077 6974 6820 6120  w widget with a 
+00014d80: 6769 7665 6e20 6d61 7374 6572 2061 6e64  given master and
+00014d90: 206c 6973 7420 6f66 2069 7465 6d73 2e0a   list of items..
+00014da0: 2020 2020 2020 2020 2020 2020 5061 7261              Para
+00014db0: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
+00014dc0: 2020 2020 2020 2020 6d61 7374 6572 2028          master (
+00014dd0: 616e 7929 3a20 5468 6520 7061 7265 6e74  any): The parent
+00014de0: 2077 6964 6765 7420 666f 7220 7468 6520   widget for the 
+00014df0: 416e 616c 7973 6973 7669 6577 2e0a 2020  Analysisview..  
+00014e00: 2020 2020 2020 2020 2020 2020 2020 6974                it
+00014e10: 656d 7320 286c 6973 7429 3a20 4120 6c69  ems (list): A li
+00014e20: 7374 206f 6620 6974 656d 7320 746f 2062  st of items to b
+00014e30: 6520 696e 7365 7274 6564 2069 6e74 6f20  e inserted into 
+00014e40: 7468 6520 416e 616c 7973 6973 7669 6577  the Analysisview
+00014e50: 2e0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
+00014e60: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00014e70: 2020 2020 2020 204e 6f6e 652e 0a20 2020         None..   
+00014e80: 2020 2020 2020 2020 2050 726f 6365 7373           Process
+00014e90: 696e 6720 4c6f 6769 633a 0a20 2020 2020  ing Logic:.     
+00014ea0: 2020 2020 2020 2020 2020 202d 2053 6574             - Set
+00014eb0: 7320 7570 2074 6865 2041 6e61 6c79 7369  s up the Analysi
+00014ec0: 7376 6965 7720 7769 6467 6574 2077 6974  sview widget wit
+00014ed0: 6820 6170 7072 6f70 7269 6174 6520 7374  h appropriate st
+00014ee0: 796c 6573 2061 6e64 2062 696e 6469 6e67  yles and binding
+00014ef0: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+00014f00: 2020 202d 2049 6e73 6572 7473 2074 6865     - Inserts the
+00014f10: 2067 6976 656e 2069 7465 6d73 2069 6e74   given items int
+00014f20: 6f20 7468 6520 5472 6565 7669 6577 2e0a  o the Treeview..
+00014f30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014f40: 2020 2020 7365 6c66 2e72 6f6f 7420 3d20      self.root = 
+00014f50: 6d61 7374 6572 0a20 2020 2020 2020 2073  master.        s
+00014f60: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+00014f70: 7365 6c66 2e72 6f6f 7429 0a0a 2020 2020  self.root)..    
+00014f80: 2020 2020 7365 6c66 2e67 7269 645f 636f      self.grid_co
+00014f90: 6c75 6d6e 636f 6e66 6967 7572 6528 302c  lumnconfigure(0,
+00014fa0: 2077 6569 6768 743d 3129 0a0a 2020 2020   weight=1)..    
+00014fb0: 2020 2020 2320 4164 6420 6120 6c61 6265      # Add a labe
+00014fc0: 6c20 746f 2074 6865 2074 6f70 206f 6620  l to the top of 
+00014fd0: 7769 6e64 6f77 0a20 2020 2020 2020 2023  window.        #
+00014fe0: 206f 7572 5f6c 6162 656c 203d 2022 4472   our_label = "Dr
+00014ff0: 6167 2074 6865 2062 6f74 746f 6d20 6f66  ag the bottom of
+00015000: 2074 6865 2077 696e 646f 7720 746f 2065   the window to e
+00015010: 7870 616e 6420 6173 206e 6565 6465 642e  xpand as needed.
+00015020: 220a 2020 2020 2020 2020 2320 7365 6c66  ".        # self
+00015030: 2e61 6e61 6c79 7369 735f 6c61 6265 6c20  .analysis_label 
+00015040: 3d20 6374 6b2e 4354 6b4c 6162 656c 286d  = ctk.CTkLabel(m
+00015050: 6173 7465 723d 7365 6c66 2c20 7465 7874  aster=self, text
+00015060: 3d6f 7572 5f6c 6162 656c 2c20 666f 6e74  =our_label, font
+00015070: 3d28 2222 2c20 3132 2929 0a20 2020 2020  =("", 12)).     
+00015080: 2020 2023 2073 656c 662e 616e 616c 7973     # self.analys
+00015090: 6973 5f6c 6162 656c 2e67 7269 6428 726f  is_label.grid(ro
+000150a0: 773d 302c 2063 6f6c 756d 6e3d 312c 2070  w=0, column=1, p
+000150b0: 6164 783d 3130 2c20 7061 6479 3d31 302c  adx=10, pady=10,
+000150c0: 2073 7469 636b 793d 226e 2229 0a0a 2020   sticky="n")..  
+000150d0: 2020 2020 2020 2320 4261 7369 6320 6170        # Basic ap
+000150e0: 7065 6172 616e 6365 2066 6f72 2074 6578  pearance for tex
+000150f0: 742c 2066 6f72 6567 726f 756e 6420 616e  t, foreground an
+00015100: 6420 6261 636b 6772 6f75 6e64 2e0a 2020  d background..  
+00015110: 2020 2020 2020 7365 6c66 2e61 6e61 6c79        self.analy
+00015120: 7369 735f 6267 5f63 6f6c 6f72 203d 2073  sis_bg_color = s
+00015130: 656c 662e 726f 6f74 2e5f 6170 706c 795f  elf.root._apply_
+00015140: 6170 7065 6172 616e 6365 5f6d 6f64 6528  appearance_mode(
+00015150: 0a20 2020 2020 2020 2020 2020 2063 746b  .            ctk
+00015160: 2e54 6865 6d65 4d61 6e61 6765 722e 7468  .ThemeManager.th
+00015170: 656d 655b 2243 546b 4672 616d 6522 5d5b  eme["CTkFrame"][
+00015180: 2266 675f 636f 6c6f 7222 5d0a 2020 2020  "fg_color"].    
+00015190: 2020 2020 2920 2023 206e 6f71 613a 2053      )  # noqa: S
+000151a0: 4c46 3030 310a 2020 2020 2020 2020 7365  LF001.        se
+000151b0: 6c66 2e61 6e61 6c79 7369 735f 7465 7874  lf.analysis_text
+000151c0: 5f63 6f6c 6f72 203d 2073 656c 662e 726f  _color = self.ro
+000151d0: 6f74 2e5f 6170 706c 795f 6170 7065 6172  ot._apply_appear
+000151e0: 616e 6365 5f6d 6f64 6528 2020 2320 6e6f  ance_mode(  # no
+000151f0: 7161 3a20 534c 4630 3031 0a20 2020 2020  qa: SLF001.     
+00015200: 2020 2020 2020 2063 746b 2e54 6865 6d65         ctk.Theme
+00015210: 4d61 6e61 6765 722e 7468 656d 655b 2243  Manager.theme["C
+00015220: 546b 4c61 6265 6c22 5d5b 2274 6578 745f  TkLabel"]["text_
+00015230: 636f 6c6f 7222 5d2c 0a20 2020 2020 2020  color"],.       
+00015240: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+00015250: 7365 6c65 6374 6564 5f63 6f6c 6f72 203d  selected_color =
+00015260: 2073 656c 662e 726f 6f74 2e5f 6170 706c   self.root._appl
+00015270: 795f 6170 7065 6172 616e 6365 5f6d 6f64  y_appearance_mod
+00015280: 6528 2020 2320 6e6f 7161 3a20 534c 4630  e(  # noqa: SLF0
+00015290: 3031 0a20 2020 2020 2020 2020 2020 2063  01.            c
+000152a0: 746b 2e54 6865 6d65 4d61 6e61 6765 722e  tk.ThemeManager.
+000152b0: 7468 656d 655b 2243 546b 4275 7474 6f6e  theme["CTkButton
+000152c0: 225d 5b22 6667 5f63 6f6c 6f72 225d 2c0a  "]["fg_color"],.
+000152d0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000152e0: 2020 2023 2053 6574 2075 7020 7468 6520     # Set up the 
+000152f0: 7374 796c 652f 7468 656d 650a 2020 2020  style/theme.    
+00015300: 2020 2020 7365 6c66 2e61 6e61 6c79 7369      self.analysi
+00015310: 735f 7374 796c 6520 3d20 7474 6b2e 5374  s_style = ttk.St
+00015320: 796c 6528 7365 6c66 290a 2020 2020 2020  yle(self).      
+00015330: 2020 7365 6c66 2e61 6e61 6c79 7369 735f    self.analysis_
+00015340: 7374 796c 652e 7468 656d 655f 7573 6528  style.theme_use(
+00015350: 2264 6566 6175 6c74 2229 0a0a 2020 2020  "default")..    
+00015360: 2020 2020 2320 5265 6372 6561 7465 2074      # Recreate t
+00015370: 6578 7420 626f 780a 2020 2020 2020 2020  ext box.        
+00015380: 7365 6c66 2e61 6e61 6c79 7369 735f 7465  self.analysis_te
+00015390: 7874 626f 7820 3d20 6374 6b2e 4354 6b54  xtbox = ctk.CTkT
+000153a0: 6578 7462 6f78 2873 656c 662c 2068 6569  extbox(self, hei
+000153b0: 6768 743d 3730 302c 2077 6964 7468 3d35  ght=700, width=5
+000153c0: 3530 290a 2020 2020 2020 2020 7365 6c66  50).        self
+000153d0: 2e61 6e61 6c79 7369 735f 7465 7874 626f  .analysis_textbo
+000153e0: 782e 6772 6964 2872 6f77 3d31 2c20 636f  x.grid(row=1, co
+000153f0: 6c75 6d6e 3d31 2c20 7061 6478 3d32 302c  lumn=1, padx=20,
+00015400: 2070 6164 793d 3430 2c20 7374 6963 6b79   pady=40, sticky
+00015410: 3d22 6e73 6577 2229 0a0a 2020 2020 2020  ="nsew")..      
+00015420: 2020 2320 496e 7365 7274 2074 6865 2074    # Insert the t
+00015430: 6578 7420 7769 7468 206f 7572 206e 6577  ext with our new
+00015440: 206d 6573 7361 6765 2069 6e74 6f20 7468   message into th
+00015450: 6520 7465 7874 2062 6f78 2e0a 2020 2020  e text box..    
+00015460: 2020 2020 2320 4164 6420 7468 6520 7465      # Add the te
+00015470: 7374 2061 6e64 2063 6f6c 6f72 2074 6f20  st and color to 
+00015480: 7468 6520 7465 7874 2062 6f78 2e0a 2020  the text box..  
+00015490: 2020 2020 2020 2320 666d 743a 206f 6666        # fmt: off
+000154a0: 0a20 2020 2020 2020 2073 656c 662e 616e  .        self.an
+000154b0: 616c 7973 6973 5f74 6578 7462 6f78 2e69  alysis_textbox.i
+000154c0: 6e73 6572 7428 2230 2e30 222c 2066 227b  nsert("0.0", f"{
+000154d0: 6d65 7373 6167 657d 5c6e 2229 0a20 2020  message}\n").   
+000154e0: 2020 2020 2073 656c 662e 616e 616c 7973       self.analys
+000154f0: 6973 5f74 6578 7462 6f78 2e63 6f6e 6669  is_textbox.confi
+00015500: 6775 7265 2873 7461 7465 3d22 6469 7361  gure(state="disa
+00015510: 626c 6564 2229 2020 2320 636f 6e66 6967  bled")  # config
+00015520: 7572 6520 7465 7874 626f 7820 746f 2062  ure textbox to b
+00015530: 6520 7265 6164 2d6f 6e6c 790a 2020 2020  e read-only.    
+00015540: 2020 2020 7365 6c66 2e61 6e61 6c79 7369      self.analysi
+00015550: 735f 7465 7874 626f 782e 636f 6e66 6967  s_textbox.config
+00015560: 7572 6528 7772 6170 3d22 776f 7264 2229  ure(wrap="word")
+00015570: 0a20 2020 2020 2020 2073 656c 662e 616e  .        self.an
+00015580: 616c 7973 6973 5f74 6578 7462 6f78 2e66  alysis_textbox.f
+00015590: 6f63 7573 5f73 6574 2829 0a0a 0a23 2044  ocus_set()...# D
+000155a0: 6566 696e 6520 7468 6520 4169 2041 6e61  efine the Ai Ana
+000155b0: 6c79 7369 7320 7769 6e64 6f77 0a63 6c61  lysis window.cla
+000155c0: 7373 2041 6e61 6c79 7369 7357 696e 646f  ss AnalysisWindo
+000155d0: 7728 6374 6b2e 4354 6b54 6f70 6c65 7665  w(ctk.CTkTopleve
+000155e0: 6c29 3a0a 2020 2020 2222 2244 6566 696e  l):.    """Defin
+000155f0: 6520 6f75 7220 746f 7020 6c65 7665 6c20  e our top level 
+00015600: 7769 6e64 6f77 2066 6f72 2074 6865 2061  window for the a
+00015610: 6e61 6c79 7369 7320 7669 6577 2e22 2222  nalysis view."""
+00015620: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00015630: 5f5f 2873 656c 662c 202a 6172 6773 2c20  __(self, *args, 
+00015640: 2a2a 6b77 6172 6773 2920 2d3e 204e 6f6e  **kwargs) -> Non
+00015650: 653a 2020 2320 6e6f 7161 3a20 414e 4e30  e:  # noqa: ANN0
+00015660: 3032 2c20 414e 4e30 3033 0a20 2020 2020  02, ANN003.     
+00015670: 2020 2022 2222 4372 6561 7465 7320 6120     """Creates a 
+00015680: 6c61 6265 6c20 7769 6467 6574 2066 6f72  label widget for
+00015690: 2061 2074 7265 6520 7669 6577 2e0a 2020   a tree view..  
+000156a0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+000156b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000156c0: 6c66 2028 6f62 6a65 6374 293a 2054 6865  lf (object): The
+000156d0: 206f 626a 6563 7420 6265 696e 6720 7061   object being pa
+000156e0: 7373 6564 2e0a 2020 2020 2020 2020 2020  ssed..          
+000156f0: 2020 2a61 7267 7320 2861 6e79 293a 2041    *args (any): A
+00015700: 6464 6974 696f 6e61 6c20 6172 6775 6d65  dditional argume
+00015710: 6e74 732e 0a20 2020 2020 2020 2020 2020  nts..           
+00015720: 202a 2a6b 7761 7267 7320 2861 6e79 293a   **kwargs (any):
+00015730: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
+00015740: 6f72 6420 6172 6775 6d65 6e74 732e 0a20  ord arguments.. 
+00015750: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00015760: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
+00015770: 3a20 5468 6973 2066 756e 6374 696f 6e20  : This function 
+00015780: 646f 6573 206e 6f74 2072 6574 7572 6e20  does not return 
+00015790: 616e 7974 6869 6e67 2e0a 2020 2020 2020  anything..      
+000157a0: 2020 5072 6f63 6573 7369 6e67 204c 6f67    Processing Log
+000157b0: 6963 3a0a 2020 2020 2020 2020 2020 2020  ic:.            
+000157c0: 2d20 496e 6974 6961 6c69 7a65 206c 6162  - Initialize lab
+000157d0: 656c 2077 6964 6765 742e 0a20 2020 2020  el widget..     
+000157e0: 2020 2020 2020 202d 2050 6163 6b20 6c61         - Pack la
+000157f0: 6265 6c20 7769 6467 6574 2077 6974 6820  bel widget with 
+00015800: 7061 6464 696e 672e 0a20 2020 2020 2020  padding..       
+00015810: 2020 2020 202d 2053 6574 206c 6162 656c       - Set label
+00015820: 2077 6964 6765 7420 7465 7874 2e22 2222   widget text."""
+00015830: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00015840: 2e5f 5f69 6e69 745f 5f28 2a61 7267 732c  .__init__(*args,
+00015850: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+00015860: 2020 2073 656c 662e 6765 6f6d 6574 7279     self.geometry
+00015870: 2822 3630 3078 3830 302b 3630 302b 3022  ("600x800+600+0"
+00015880: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+00015890: 6974 6c65 2822 4d61 7054 6173 6b65 7220  itle("MapTasker 
+000158a0: 416e 616c 7973 6973 2052 6573 706f 6e73  Analysis Respons
+000158b0: 6522 290a 0a0a 2320 4465 6669 6e65 2074  e")...# Define t
+000158c0: 6865 2041 6920 506f 7075 7020 7769 6e64  he Ai Popup wind
+000158d0: 6f77 0a63 6c61 7373 2050 6f70 7570 5769  ow.class PopupWi
+000158e0: 6e64 6f77 2863 746b 2e43 546b 293a 0a20  ndow(ctk.CTk):. 
+000158f0: 2020 2022 2222 4465 6669 6e65 206f 7572     """Define our
+00015900: 2074 6f70 206c 6576 656c 2077 696e 646f   top level windo
+00015910: 7720 666f 7220 7468 6520 506f 7075 7020  w for the Popup 
+00015920: 7669 6577 2e22 2222 0a0a 2020 2020 6465  view."""..    de
+00015930: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00015940: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+00015950: 2920 2d3e 204e 6f6e 653a 2020 2320 6e6f  ) -> None:  # no
+00015960: 7161 3a20 414e 4e30 3032 2c20 414e 4e30  qa: ANN002, ANN0
+00015970: 3033 0a20 2020 2020 2020 2022 2222 4372  03.        """Cr
+00015980: 6561 7465 7320 6120 6c61 6265 6c20 7769  eates a label wi
+00015990: 6467 6574 2066 6f72 2061 2074 7265 6520  dget for a tree 
+000159a0: 7669 6577 2e0a 2020 2020 2020 2020 5061  view..        Pa
+000159b0: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
+000159c0: 2020 2020 2020 7365 6c66 2028 6f62 6a65        self (obje
+000159d0: 6374 293a 2054 6865 206f 626a 6563 7420  ct): The object 
+000159e0: 6265 696e 6720 7061 7373 6564 2e0a 2020  being passed..  
+000159f0: 2020 2020 2020 2020 2020 2a61 7267 7320            *args 
+00015a00: 2861 6e79 293a 2041 6464 6974 696f 6e61  (any): Additiona
+00015a10: 6c20 6172 6775 6d65 6e74 732e 0a20 2020  l arguments..   
+00015a20: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
+00015a30: 7320 2861 6e79 293a 2041 6464 6974 696f  s (any): Additio
+00015a40: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
+00015a50: 6d65 6e74 732e 0a20 2020 2020 2020 2052  ments..        R
+00015a60: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00015a70: 2020 2020 4e6f 6e65 3a20 5468 6973 2066      None: This f
+00015a80: 756e 6374 696f 6e20 646f 6573 206e 6f74  unction does not
+00015a90: 2072 6574 7572 6e20 616e 7974 6869 6e67   return anything
+00015aa0: 2e0a 2020 2020 2020 2020 5072 6f63 6573  ..        Proces
+00015ab0: 7369 6e67 204c 6f67 6963 3a0a 2020 2020  sing Logic:.    
+00015ac0: 2020 2020 2020 2020 2d20 496e 6974 6961          - Initia
+00015ad0: 6c69 7a65 206c 6162 656c 2077 6964 6765  lize label widge
+00015ae0: 742e 0a20 2020 2020 2020 2020 2020 202d  t..            -
+00015af0: 2050 6163 6b20 6c61 6265 6c20 7769 6467   Pack label widg
+00015b00: 6574 2077 6974 6820 7061 6464 696e 672e  et with padding.
+00015b10: 0a20 2020 2020 2020 2020 2020 202d 2053  .            - S
+00015b20: 6574 206c 6162 656c 2077 6964 6765 7420  et label widget 
+00015b30: 7465 7874 2e22 2222 0a20 2020 2020 2020  text.""".       
+00015b40: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+00015b50: 5f28 2a61 7267 732c 202a 2a6b 7761 7267  _(*args, **kwarg
+00015b60: 7329 0a20 2020 2020 2020 2023 2047 6574  s).        # Get
+00015b70: 2074 6865 2073 6372 6565 6e20 7369 7a65   the screen size
+00015b80: 0a20 2020 2020 2020 2073 6372 6565 6e5f  .        screen_
+00015b90: 7769 6474 6820 3d20 7365 6c66 2e77 696e  width = self.win
+00015ba0: 666f 5f73 6372 6565 6e77 6964 7468 2829  fo_screenwidth()
+00015bb0: 0a20 2020 2020 2020 2073 6372 6565 6e5f  .        screen_
+00015bc0: 6865 6967 6874 203d 2073 656c 662e 7769  height = self.wi
+00015bd0: 6e66 6f5f 7363 7265 656e 6865 6967 6874  nfo_screenheight
+00015be0: 2829 0a0a 2020 2020 2020 2020 2320 4365  ()..        # Ce
+00015bf0: 6e74 6572 2074 6865 2077 6964 6765 740a  nter the widget.
+00015c00: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00015c10: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+00015c20: 6f6d 6574 7279 2873 656c 662e 6169 5f70  ometry(self.ai_p
+00015c30: 6f70 7570 5f77 696e 646f 775f 706f 7369  opup_window_posi
+00015c40: 7469 6f6e 290a 2020 2020 2020 2020 2020  tion).          
+00015c50: 2020 7072 696e 7428 2267 7569 7574 696c    print("guiutil
+00015c60: 7320 7769 6e64 6f77 2072 6573 746f 7265  s window restore
+00015c70: 6422 290a 2020 2020 2020 2020 6578 6365  d").        exce
+00015c80: 7074 2041 7474 7269 6275 7465 4572 726f  pt AttributeErro
+00015c90: 723a 0a20 2020 2020 2020 2020 2020 2073  r:.            s
+00015ca0: 656c 662e 6765 6f6d 6574 7279 2866 2235  elf.geometry(f"5
+00015cb0: 3030 7835 302b 7b73 6372 6565 6e5f 7769  00x50+{screen_wi
+00015cc0: 6474 682f 2f33 7d2b 7b73 6372 6565 6e5f  dth//3}+{screen_
+00015cd0: 6865 6967 6874 2f2f 3130 7d22 290a 2020  height//10}").  
+00015ce0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00015cf0: 6974 6c65 2822 4d61 7054 6173 6b65 7220  itle("MapTasker 
+00015d00: 416e 616c 7973 6973 2229 0a0a 2020 2020  Analysis")..    
+00015d10: 2020 2020 7365 6c66 2e67 7269 645f 636f      self.grid_co
+00015d20: 6c75 6d6e 636f 6e66 6967 7572 6528 302c  lumnconfigure(0,
+00015d30: 2077 6569 6768 743d 3129 0a0a 2020 2020   weight=1)..    
+00015d40: 2020 2020 2320 5365 7420 706f 7075 7020      # Set popup 
+00015d50: 7769 6e64 6f77 2077 6169 7420 7469 6d65  window wait time
+00015d60: 2074 6f20 2e35 2073 6563 6f6e 6473 2c20   to .5 seconds, 
+00015d70: 6166 7465 7220 7768 6963 6820 706f 7075  after which popu
+00015d80: 705f 6275 7474 6f6e 5f65 7665 6e74 2077  p_button_event w
+00015d90: 696c 6c20 6265 2063 616c 6c65 642e 0a20  ill be called.. 
+00015da0: 2020 2020 2020 2073 656c 662e 6166 7465         self.afte
+00015db0: 7228 3530 302c 2073 656c 662e 706f 7075  r(500, self.popu
+00015dc0: 705f 6275 7474 6f6e 5f65 7665 6e74 290a  p_button_event).
+00015dd0: 0a20 2020 2020 2020 2023 204c 6162 656c  .        # Label
+00015de0: 2077 6964 6765 740a 2020 2020 2020 2020   widget.        
+00015df0: 6f75 725f 6c61 6265 6c20 3d20 2241 6e61  our_label = "Ana
+00015e00: 6c79 7369 7320 6973 2072 756e 6e69 6e67  lysis is running
+00015e10: 2069 6e20 7468 6520 6261 636b 6772 6f75   in the backgrou
+00015e20: 6e64 2e20 2050 6c65 6173 6520 7374 616e  nd.  Please stan
+00015e30: 6420 6279 2e2e 2e22 0a20 2020 2020 2020  d by...".       
+00015e40: 2073 656c 662e 506f 7075 705f 6c61 6265   self.Popup_labe
+00015e50: 6c20 3d20 6374 6b2e 4354 6b4c 6162 656c  l = ctk.CTkLabel
+00015e60: 286d 6173 7465 723d 7365 6c66 2c20 7465  (master=self, te
+00015e70: 7874 3d6f 7572 5f6c 6162 656c 2c20 666f  xt=our_label, fo
+00015e80: 6e74 3d28 2222 2c20 3132 292c 2074 6578  nt=("", 12), tex
+00015e90: 745f 636f 6c6f 723d 2274 7572 7175 6f69  t_color="turquoi
+00015ea0: 7365 2229 0a20 2020 2020 2020 2073 656c  se").        sel
+00015eb0: 662e 506f 7075 705f 6c61 6265 6c2e 6772  f.Popup_label.gr
+00015ec0: 6964 2872 6f77 3d30 2c20 636f 6c75 6d6e  id(row=0, column
+00015ed0: 3d30 2c20 7061 6478 3d30 2c20 7061 6479  =0, padx=0, pady
+00015ee0: 3d31 302c 2073 7469 636b 793d 226e 2229  =10, sticky="n")
+00015ef0: 0a0a 2020 2020 2020 2020 2320 4261 7369  ..        # Basi
+00015f00: 6320 6170 7065 6172 616e 6365 2066 6f72  c appearance for
+00015f10: 2074 6578 742c 2066 6f72 6567 726f 756e   text, foregroun
+00015f20: 6420 616e 6420 6261 636b 6772 6f75 6e64  d and background
+00015f30: 2e0a 2020 2020 2020 2020 7365 6c66 2e50  ..        self.P
+00015f40: 6f70 7570 5f62 675f 636f 6c6f 7220 3d20  opup_bg_color = 
+00015f50: 7365 6c66 2e5f 6170 706c 795f 6170 7065  self._apply_appe
+00015f60: 6172 616e 6365 5f6d 6f64 6528 6374 6b2e  arance_mode(ctk.
+00015f70: 5468 656d 654d 616e 6167 6572 2e74 6865  ThemeManager.the
+00015f80: 6d65 5b22 4354 6b46 7261 6d65 225d 5b22  me["CTkFrame"]["
+00015f90: 6667 5f63 6f6c 6f72 225d 290a 2020 2020  fg_color"]).    
+00015fa0: 2020 2020 7365 6c66 2e50 6f70 7570 5f74      self.Popup_t
+00015fb0: 6578 745f 636f 6c6f 7220 3d20 7365 6c66  ext_color = self
+00015fc0: 2e5f 6170 706c 795f 6170 7065 6172 616e  ._apply_appearan
+00015fd0: 6365 5f6d 6f64 6528 0a20 2020 2020 2020  ce_mode(.       
+00015fe0: 2020 2020 2063 746b 2e54 6865 6d65 4d61       ctk.ThemeMa
+00015ff0: 6e61 6765 722e 7468 656d 655b 2243 546b  nager.theme["CTk
+00016000: 4c61 6265 6c22 5d5b 2274 6578 745f 636f  Label"]["text_co
+00016010: 6c6f 7222 5d2c 0a20 2020 2020 2020 2029  lor"],.        )
+00016020: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00016030: 6c65 6374 6564 5f63 6f6c 6f72 203d 2073  lected_color = s
+00016040: 656c 662e 5f61 7070 6c79 5f61 7070 6561  elf._apply_appea
+00016050: 7261 6e63 655f 6d6f 6465 280a 2020 2020  rance_mode(.    
+00016060: 2020 2020 2020 2020 6374 6b2e 5468 656d          ctk.Them
+00016070: 654d 616e 6167 6572 2e74 6865 6d65 5b22  eManager.theme["
+00016080: 4354 6b42 7574 746f 6e22 5d5b 2266 675f  CTkButton"]["fg_
+00016090: 636f 6c6f 7222 5d2c 0a20 2020 2020 2020  color"],.       
+000160a0: 2029 0a0a 2020 2020 2020 2020 2320 5365   )..        # Se
+000160b0: 7420 7570 2074 6865 2073 7479 6c65 2f74  t up the style/t
+000160c0: 6865 6d65 0a20 2020 2020 2020 2073 656c  heme.        sel
+000160d0: 662e 506f 7075 705f 7374 796c 6520 3d20  f.Popup_style = 
+000160e0: 7474 6b2e 5374 796c 6528 7365 6c66 290a  ttk.Style(self).
+000160f0: 2020 2020 2020 2020 7365 6c66 2e50 6f70          self.Pop
+00016100: 7570 5f73 7479 6c65 2e74 6865 6d65 5f75  up_style.theme_u
+00016110: 7365 2822 6465 6661 756c 7422 290a 0a20  se("default").. 
+00016120: 2020 2023 2054 6865 2022 6166 7465 7222     # The "after"
+00016130: 206e 2073 6563 6f6e 6420 7469 6d65 7220   n second timer 
+00016140: 7472 6970 7065 6420 6672 6f6d 2070 6f70  tripped from pop
+00016150: 7570 2077 696e 646f 772e 2020 436c 6f73  up window.  Clos
+00016160: 6520 7468 6520 7769 6e64 6f77 2e0a 2020  e the window..  
+00016170: 2020 2320 4e6f 7465 3a20 7275 6e67 7569    # Note: rungui
+00016180: 2077 696c 6c20 6861 7665 2061 6c72 6561   will have alrea
+00016190: 6479 2063 6f6d 706c 6574 656c 7920 7275  dy completely ru
+000161a0: 6e20 6279 2074 6869 7320 7469 6d65 2e0a  n by this time..
+000161b0: 2020 2020 6465 6620 706f 7075 705f 6275      def popup_bu
+000161c0: 7474 6f6e 5f65 7665 6e74 2873 656c 6629  tton_event(self)
+000161d0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000161e0: 2020 2222 220a 2020 2020 2020 2020 4465    """.        De
+000161f0: 6669 6e65 2074 6865 2062 6568 6176 696f  fine the behavio
+00016200: 7220 6f66 2074 6865 2070 6f70 7570 2062  r of the popup b
+00016210: 7574 746f 6e20 6576 656e 7420 6675 6e63  utton event func
+00016220: 7469 6f6e 2e20 2043 6c6f 7365 2074 6865  tion.  Close the
+00016230: 2077 696e 646f 7720 616e 6420 6578 6974   window and exit
+00016240: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00016250: 2020 2020 2020 5072 696d 6549 7465 6d73        PrimeItems
+00016260: 2e6c 6f6f 705f 6163 7469 7665 203d 2046  .loop_active = F
+00016270: 616c 7365 0a20 2020 2020 2020 2073 656c  alse.        sel
+00016280: 662e 6169 5f70 6f70 7570 5f77 696e 646f  f.ai_popup_windo
+00016290: 775f 706f 7369 7469 6f6e 203d 2073 656c  w_position = sel
+000162a0: 662e 7769 6e66 6f5f 6765 6f6d 6574 7279  f.winfo_geometry
+000162b0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000162c0: 6578 6974 203d 2054 7275 650a 2020 2020  exit = True.    
+000162d0: 2020 2020 7365 6c66 2e71 7569 7428 290a      self.quit().
+000162e0: 2020 2020 2020 2020 7365 6c66 2e71 7569          self.qui
+000162f0: 7428 290a                                t().
```

### Comparing `maptasker-4.0.2/maptasker/src/initparg.py` & `maptasker-4.0.5/maptasker/src/initparg.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         :return: runtime arguments in dictionary
     """
 
     return {
         "ai_analyze": False,  # Do local AI processing
         "ai_apikey": "",  # AI API key
         "ai_model": "",  # AI model
+        "ai_prompt": "",  # AI prompt
         "android_ipaddr": ANDROID_IPADDR,  # IP address of Android device
         "android_port": ANDROID_PORT,  # Port of Android device
         "android_file": ANDROID_FILE,
         "appearance_mode": "system",  # Appearance mode: "system", "dark", or "light"
         "bold": False,  # Display Project/Profile?Task/Scene names in bold text
         "debug": False,  # Run in debug mode (create log file)
         "directory": False,  # Display directory
@@ -55,8 +56,10 @@
         "runtime": False,  # Display the runtime arguments/settings
         "single_profile_name": "",  # Display single Profile name only
         "single_project_name": "",  # Display single Project name only
         "single_task_name": "",  # Display single Task name only
         "twisty": False,  # Add Task twisty "▶︎" clickable icons for Task details
         "underline": False,  # Underline Project/Profile?Task/Scene names
         "pretty": False,  # Pretty up the output (takes many more output lines)
+        "window_position": "",  # Last-used window position
+        "ai_popup_window_position": "",  # Last-used ai popup window position
     }
```

### Comparing `maptasker-4.0.2/maptasker/src/kidapp.py` & `maptasker-4.0.5/maptasker/src/kidapp.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/lineout.py` & `maptasker-4.0.5/maptasker/src/lineout.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/mapai.py` & `maptasker-4.0.5/maptasker/src/mapai.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
+import contextlib
 import importlib.util
+import os
 import sys
 
 import cria
 from openai import OpenAI, OpenAIError
 
 from maptasker.src.config import AI_PROMPT
 from maptasker.src.error import error_handler
-from maptasker.src.guiutils import PopupWindow
+from maptasker.src.guiutils import PopupWindow, get_api_key
 from maptasker.src.primitem import PrimeItems
-from maptasker.src.sysconst import ANALYSIS_FILE, ERROR_FILE, OPENAI_MODELS
+from maptasker.src.sysconst import ANALYSIS_FILE, ERROR_FILE, KEYFILE, OPENAI_MODELS
 
 
 # ##################################################################################
 # Determine if a module is available or not.
 # ##################################################################################
 def module_is_available(module_name: str) -> bool:
     """
@@ -102,15 +104,15 @@
         # Output: "Paris"
     """
     if PrimeItems.program_arguments["ai_analyze"] and not module_is_available("cria"):
         error_handler("Module 'cria' not found.  Please install the 'cria' module and the Ollama app.", 12)
         return
 
     # Fix the model name
-    if PrimeItems.program_arguments["ai_model"] == "none (llama3)":
+    if PrimeItems.program_arguments["ai_model"] == "None (llama3)":
         PrimeItems.program_arguments["ai_model"] = "llama3"
 
     # Open the model and get the response
     try:
         with cria.Model(PrimeItems.program_arguments["ai_model"]) as ai:
             response = ai.chat(query, stream=False)
 
@@ -169,19 +171,22 @@
         None: This function does not return anything.
     """
     # Make sure openai is available.
     if PrimeItems.program_arguments["ai_analyze"] and not module_is_available("openai"):
         error_handler("Module 'cria' not found.  Please install the 'cria' module and Ollama.", 12)
         return
 
+    # Get the api key
+    if PrimeItems.program_arguments["ai_apikey"] == "Hidden" and os.path.isfile(KEYFILE):
+        apikey = get_api_key  # Get the key from the file
+    else:
+        apikey = PrimeItems.program_arguments["ai_apikey"]
+
     # Set up the OpenAI client and send the query
-    client = OpenAI(
-        # This is the default and can be omitted
-        api_key=PrimeItems.program_arguments["ai_apikey"],
-    )
+    client = OpenAI(api_key=apikey)
 
     try:
         stream_feed = client.chat.completions.create(
             model=PrimeItems.program_arguments["ai_model"],
             messages=[{"role": "system", "content": "You are a Tasker programmer"}, {"role": "user", "content": query}],
             stream=True,
         )
@@ -238,34 +243,41 @@
 # ##################################################################################
 def map_ai() -> None:
     """
     A function that determines whether to call the OpenAI or local AI routine based on the model specified in PrimeItems.
 
     Does the setup for the query by concatenating the lines in PrimeItems.ai["output_lines"].
     """
-    # Display a popup telling user we are analyzing
+    # Display a popup window telling user we are analyzing
     popup = PopupWindow()
     popup.mainloop()
 
     # Clean up the output list since it has all the front matter and we only need the object (Project/Profile/Task)
     temp_output = cleanup_output()
 
+    # Save the ai popup window position
+    with contextlib.suppress(AttributeError):
+        PrimeItems.program_arguments["ai_popup_window_position"] = popup.ai_popup_window_position
+
     # Setup the query
     if PrimeItems.program_arguments["single_project_name"]:
         ai_object = "Project"
         item = PrimeItems.program_arguments["single_project_name"]
     elif PrimeItems.program_arguments["single_profile_name"]:
         ai_object = "Profile"
         item = PrimeItems.program_arguments["single_profile_name"]
     elif PrimeItems.program_arguments["single_task_name"]:
         ai_object = "Task"
         item = PrimeItems.program_arguments["single_task_name"]
 
     # Put the query together
-    query = f"Given the following {ai_object} in Tasker, {AI_PROMPT}"
+    prompt = PrimeItems.program_arguments["ai_prompt"] if PrimeItems.program_arguments["ai_prompt"] else AI_PROMPT
+    if not prompt.endswith(":"):
+        prompt = f"{prompt}:"
+    query = f"Given the following {ai_object} in Tasker, {prompt}"
     for line in temp_output:
         query += f"{line}\n"
 
     # Let the user know what is going on.
     print(f"MapTasker analysis for {ai_object} {item} is running in the background.  Please wait...")
 
     # Call appropriate AI routine: OpenAI or local Ollama
```

### Comparing `maptasker-4.0.2/maptasker/src/mapit.py` & `maptasker-4.0.5/maptasker/src/mapit.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/maputils.py` & `maptasker-4.0.5/maptasker/src/maputils.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     try:
         response = requests.get(url, timeout=5)
     except InvalidSchema:
         error_message = f"Request failed for url: {url} .  Invalid url!"
     except ConnectionError:
         error_message = f"Request failed for url: {url} .  Connection error! Unable to get XML from Android device."
     except Timeout:
-        error_message = f"Request failed for url: {url} .  Timeout error.\n\nOr perhaps the profile 'MapTasker List' has not been imported into Tasker!"
+        error_message = f"Request failed for url: {url} .  Timeout error.  Or perhaps the profile 'MapTasker List' has not been imported into Tasker on the Android device!"
     except Exception as e:
         error_message = f"Request failed for url: {url}, error: {e} ."
 
     # If we have an error message, return as error.
     if error_message:
         logger.debug(error_message)
         return 8, error_message
```

### Comparing `maptasker-4.0.2/maptasker/src/nameattr.py` & `maptasker-4.0.5/maptasker/src/nameattr.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/outline.py` & `maptasker-4.0.5/maptasker/src/outline.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/parsearg.py` & `maptasker-4.0.5/maptasker/src/parsearg.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/prefers.py` & `maptasker-4.0.5/maptasker/src/prefers.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/primitem.py` & `maptasker-4.0.5/maptasker/src/primitem.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/proclist.py` & `maptasker-4.0.5/maptasker/src/proclist.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/profiles.py` & `maptasker-4.0.5/maptasker/src/profiles.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/progargs.py` & `maptasker-4.0.5/maptasker/src/progargs.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/proginit.py` & `maptasker-4.0.5/maptasker/src/proginit.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/projects.py` & `maptasker-4.0.5/maptasker/src/projects.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/property.py` & `maptasker-4.0.5/maptasker/src/property.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/runcli.py` & `maptasker-4.0.5/maptasker/src/runcli.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/rungui.py` & `maptasker-4.0.5/maptasker/src/rungui.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
     PrimeItems.program_arguments["indent"] = convert_to_integer(PrimeItems.program_arguments["indent"], 4)
     # Get the font
     if the_font := user_input.font:
         PrimeItems.program_arguments["font"] = the_font
 
     # If user selected the "Exit" button, call it quits.
     if user_input.exit:
-        # Save our runtime settings for next time.
+        # Save the runtijme settings first.
         _, _ = save_restore_args(PrimeItems.program_arguments, PrimeItems.colors_to_use, True)
         # Spit out the message and log it.
         error_handler("Program exited. Goodbye.", 0)
         sys.exit(0)
 
     # Return the program arguments and colors to use.
     return (PrimeItems.program_arguments, do_colors(user_input))
```

### Comparing `maptasker-4.0.2/maptasker/src/scenes.py` & `maptasker-4.0.5/maptasker/src/scenes.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     This function processes the list element associated with the given child element. It first checks if the child element
     has an action associated with it. If it does, it retrieves the label and action line for the element. Then, it fixes
     the indentation level and adds the action and action details to the output lines.
     """
     # Get the task Action associated with this listitem
     action = child.find("Action")
-    if action is not None and action:
+    if action is not None:
         label = child.find("label").text
         action_line = get_actions(child)
 
         # Now fix our indentation
         subline_indentation = f"{blank*len(element_name)}{blank*(9+indentation)}"
         PrimeItems.output_lines.add_line_to_output(
             2,
```

### Comparing `maptasker-4.0.2/maptasker/src/servicec.py` & `maptasker-4.0.5/maptasker/src/servicec.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/share.py` & `maptasker-4.0.5/maptasker/src/share.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/shelsort.py` & `maptasker-4.0.5/maptasker/src/shelsort.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/sysconst.py` & `maptasker-4.0.5/maptasker/src/sysconst.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,25 +22,27 @@
 from typing import ClassVar
 
 import darkdetect
 
 # Global constants
 UNKNOWN_TASK_NAME = "Unnamed/Anonymous."
 
-VERSION = "4.0.2"
+VERSION = "4.0.5"
 MY_VERSION = f"MapTasker version {VERSION}"
 
 MY_LICENSE = "MIT License"
 NO_PROJECT = "-none found."
 COUNTER_FILE = ".MapTasker_RunCount.txt"
 OLD_ARGUMENTS_FILE = ".MapTasker_arguments.json"
 ARGUMENTS_FILE = "MapTasker_Settings.toml"
 FONT_FAMILY = ";font-family:"
 NO_PROFILE = "None or unnamed!"
 CHANGELOG_FILE = ".maptasker_changelog.txt"
+CHANGELOG_JSON_FILE = "maptasker_changelog.json"
+CHANGELOG_JSON_URL = "https://raw.githubusercontent.com/mctinker/Map-Tasker/Master/maptasker_changelog.json"
 KEYFILE = ".maptasker.key"
 ERROR_FILE = ".maptasker_error.txt"
 ANALYSIS_FILE = "MapTasker_Analysis.txt"
 
 #  List of color arguments and their names
 #  Two different key/value structures in one:
 #    1- Used as lookup for color selection in GUI.  E.g. key=Disabled Profiles
@@ -106,14 +108,15 @@
 }
 
 # Runtime argument names/keywords that are used throughout the program
 ARGUMENT_NAMES = {
     "ai_analyze": "Analyze AI",
     "ai_model": "AI Model",
     "ai_apikey": "AI Api Key",
+    "ai_prompt": "AI Prompt",
     "android_ipaddr": "Android IP Address",
     "android_file": "Android Backup File location on Android device",
     "android_port": "Android Port Number",
     "appearance_mode": "Appearance Mode",
     "bold": "Bold Names",
     "debug": "Debug Mode",
     "directory": "Display Directory",
@@ -133,14 +136,16 @@
     "rerun": "ReRun Program",
     "runtime": "Display Runtime Arguments/Settings",
     "single_profile_name": "Single Profile Name",
     "single_project_name": "Single Project Name",
     "single_task_name": "Single Task Name",
     "twisty": "Hide Task Details under Twisty",
     "underline": "Underline Names",
+    "window_position": "Last Window Position",
+    "ai_popup_window_position": "Last Ai Popup Window Position",
 }
 
 # Debug stuff
 logger = logging.getLogger("MapTasker")
 debug_out = False  # Prints the line to be added to the output
 DEBUG_PROGRAM = False
 debug_file = "maptasker_debug.log"
@@ -180,17 +185,16 @@
 class FormatLine(Enum):
     """Definitions for creating an output line in the output list."""
 
     dont_format_line: ClassVar[list] = []
     add_end_span = True
     dont_add_end_span = False
 
-    """Definitions for defining the output display level."""
-
 
+"""Definitions for defining the output display level."""
 DISPLAY_DETAIL_LEVEL_summary: int = 0
 DISPLAY_DETAIL_LEVEL_anon_tasks_only: int = 1
 DISPLAY_DETAIL_LEVEL_all_tasks: int = 2
 DISPLAY_DETAIL_LEVEL_all_parameters: int = 3
 DISPLAY_DETAIL_LEVEL_all_variables: int = 4
 DISPLAY_DETAIL_LEVEL_everything: int = 5
 
@@ -216,9 +220,9 @@
         } \
     </style>"
 )
 
 
 NOW_TIME = datetime.now()  # noqa: DTZ005
 
-OPENAI_MODELS = ["gpt-3.5-turbo", "gpt-4", "gpt-4-turbo"]
+OPENAI_MODELS = ["gpt-3.5-turbo", "gpt-4o", "gpt-4", "gpt-4-turbo"]
 LLAMA_MODELS = ["llama2", "llama3"]
```

### Comparing `maptasker-4.0.2/maptasker/src/taskactn.py` & `maptasker-4.0.5/maptasker/src/taskactn.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/taskerd.py` & `maptasker-4.0.5/maptasker/src/taskerd.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/taskflag.py` & `maptasker-4.0.5/maptasker/src/taskflag.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/tasks.py` & `maptasker-4.0.5/maptasker/src/tasks.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/taskuniq.py` & `maptasker-4.0.5/maptasker/src/taskuniq.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/twisty.py` & `maptasker-4.0.5/maptasker/src/twisty.py`

 * *Files identical despite different names*

### Comparing `maptasker-4.0.2/maptasker/src/userintr.py` & `maptasker-4.0.5/maptasker/src/userintr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 """Code to manage the graphical user interface."""
 
 #! /usr/bin/env python3
 
-# #################################################################################### #
 #                                                                                      #
 # userintr: provide GUI and process input for program arguments                        #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
-# #################################################################################### #
 import contextlib
+import json
 import webbrowser
 from pathlib import Path
+from typing import Callable
 
 import customtkinter
+import requests
 from CTkColorPicker.ctk_color_picker import AskColor
 
 from maptasker.src.colrmode import set_color_mode
-from maptasker.src.config import DEFAULT_DISPLAY_DETAIL_LEVEL, OUTPUT_FONT
+from maptasker.src.config import AI_PROMPT, DEFAULT_DISPLAY_DETAIL_LEVEL, OUTPUT_FONT
 from maptasker.src.getids import get_ids
 from maptasker.src.getputer import save_restore_args
 from maptasker.src.guiutils import (
     CHANGELOG,
     AnalysisWindow,
     CTkAnalysisview,
     CTkTreeview,
     TreeviewWindow,
     add_button,
     add_label,
     build_profiles,
     check_for_changelog,
     clear_android_buttons,
+    clear_tasker_data,
     create_changelog,
-    display_ai_settings,
     display_analyze_button,
     display_current_file,
     display_messages_from_last_run,
+    display_selected_object_labels,
     get_api_key,
     get_xml,
     initialize_gui,
     initialize_screen,
     is_new_version,
-    list_profiles_and_tasks,
+    list_tasker_objects,
     ping_android_device,
+    set_tasker_object_names,
+    setup_name_error,
+    update_tasker_object_menus,
     valid_item,
     validate_or_filelist_xml,
 )
 from maptasker.src.initparg import initialize_runtime_arguments
 from maptasker.src.lineout import LineOut
 from maptasker.src.mapit import clean_up_memory, do_rerun
 from maptasker.src.maputils import update, validate_xml_file
 from maptasker.src.primitem import PrimeItems
 from maptasker.src.sysconst import (
     ARGUMENT_NAMES,
+    CHANGELOG_JSON_URL,
     KEYFILE,
     OPENAI_MODELS,
     TYPES_OF_COLOR_NAMES,
     VERSION,
     DISPLAY_DETAIL_LEVEL_all_parameters,
 )
 from maptasker.src.taskerd import get_the_xml_data
@@ -175,31 +181,30 @@
     " Android device or the program is run with the '-reset' option."
 )
 
 AI_HELP_TEXT = (
     "The Analyze tab is used to run the Ai analysis on your Profile, using either the local llama model or the server-based Open Ai model.\n\n"
     "The following steps are required in order to run Ai against your Profile.\n\n"
     "1- If using Open Ai, you must have a valid Open Ai api key.  You can use the 'Show/Edit Open AI key' button to enter your key.\n\n"
-    "2- If using the local model, you must manually download and install Ollama via 'https://ollama.com/download'.  Then, run it once to load the model and then 'Run Analysis' Again.\n\n"
+    "2- The default prompt is:'how could it be improved:', and is automatically preceded by the 'Given the following (Project/Profile/Task) in Tasker, '.  If modifying the prompt, you are only modifing the 'how could it be improved:' portion.\n\n"
+    "3- If using the local model, you must manually download and install Ollama via 'https://ollama.com/download'.  Then, run it once to load the model and then 'Run Analysis' Again.\n\n"
     "   If you select a model that has not yet been loaded, it will be loaded in the background once the analysis begins.\n\n"
-    "2- Select the model you want to use.  The default is None (llama3):\n\n"
-    "3- Click the 'Run Analysis' button.\n\n"
+    "4- Select the model you want to use.  The default is None (llama3):\n\n"
+    "5- Click the 'Run Analysis' button.\n\n"
     "   If you have not yet selected a Profile or Task from the 'Specify Name' tab, then you will be prompted to do so.\n\n"
-    "   Once the Profile or Task has been selected, it will check to see if you have the supporting program to run against the model (e.g. openai) you selected.\n\n"
     "The process may take some time and runs in the background.  The results will appear in a separate window.\n\n"
-    "Your designated api-key (if any), model, and selected profile or task will be saved across sessions.\n\n"
+    "Your designated api-key (if any), model, selected profile or task and prompt will all be saved across sessions.\n\n"
     "The 'Rerun' feature will be used to display the results of the analysis in a new window.\n\n"
 )
 
 HELP = f"MapTasker {VERSION} Help\n\n{INFO_TEXT}{CHANGELOG}"
+all_objects = "Display all Projects, Profiles, and Tasks."
 
 
-# ##################################################################################
 # Class to define the GUI configuration
-# ##################################################################################
 class MyGui(customtkinter.CTk):
     """
     Main class for GUI.
         Args:
             customtkinter (_type_): GUI class from customtkinter library.
     """
 
@@ -222,42 +227,28 @@
         self.set_defaults(True)
 
         # See if we have any carryover error messages from last run (rerun).
         display_messages_from_last_run(self)
 
         # Now restore the settings and update the fields if not resetting.
         if not PrimeItems.program_arguments["reset"]:
-            self.restore_settings_event()
+            self.restore_settings_event(first_time=True)
         else:
             self.display_message_box("GUI started with the '-reset' option.\n", "Green")
 
+        # Restore the last-used window position
+        if self.window_position:
+            self.geometry(self.window_position)
+
         if self.android_ipaddr:
             # Display backup details as a label
             self.display_backup_details()
 
-        # Display Ai settings
-        display_ai_settings(self)
-
-        # Check for single item only to be displayed. and let user know.
-        if self.single_project_name:
-            self.single_name_status(f"Display only Project '{self.single_project_name}'.", "#3f99ff")
-        if self.single_profile_name:
-            self.single_name_status(f"Display only Profile '{self.single_profile_name}'.", "#3f99ff")
-        if self.single_task_name:
-            self.single_name_status(f"Display only Task '{self.single_task_name}'.", "#3f99ff")
-
-        # Get the Profile or Task list in Analyze tab.  Only do this if we have the Profile name since it forces a read of XML.
-        if self.single_profile_name and list_profiles_and_tasks(self):
-            profile_to_display = self.single_profile_name if self.single_profile_name else "none"
-            self.profile_optionemenu.set(profile_to_display)
-            self.task_optionemenu.set("None")
-        elif self.single_task_name and list_profiles_and_tasks(self):
-            task_to_display = self.single_task_name if self.single_task_name else "none"
-            self.task_optionemenu.set(task_to_display)
-            self.profile_optionemenu.set("None")
+        # Update the Project/Profile/Task pulldown option menus and text labels.
+        update_tasker_object_menus(self, get_data=True)
 
         # Check if newer version of our code is available on Pypi (only check every 24 hours).
         # If so, add a button to enable user to update.
         # TODO For testing only = True.  False for production
         test_button = False
         if is_new_version() or test_button:
             self.new_version = True
@@ -274,36 +265,59 @@
                 "1",
                 6,
                 2,
                 (0, 170),
                 (0, 10),
                 "sw",
             )
-
+            #  Query ? button
+            self.list_files_query_button = add_button(
+                self,
+                self,
+                "#246FB6",
+                "#79ff94",
+                "#6563ff",
+                # ("#0BF075", "#ffd941"),
+                # "#1bc9ff",
+                self.whatsnew_event,
+                1,
+                "What's New?",
+                2,
+                7,
+                2,
+                (0, 180),
+                (0, 10),
+                "",
+            )
+            # self.list_files_query_button.configure(width=20)
             self.message = self.message + "\n\nA new version of MapTasker is available."
         else:
             self.new_version = False
 
         # See if we have a changelog, and get it if we do.
         check_for_changelog(self)
 
         # See if we have any current messages to display.
         if self.message:
             self.display_message_box(self.message, "Green")
             self.message = ""
 
+        if self.ai_prompt:
+            prompt = self.ai_prompt
+        else:
+            prompt = AI_PROMPT
+            self.ai_prompt = prompt
+
         # Now that we have loaded our settings, reconfigure the ai analyze button
         if ((self.ai_model in OPENAI_MODELS and self.ai_apikey) or self.ai_model) and (
             self.single_task_name or self.single_profile_name
         ):
             self.ai_analyze_button.configure(fg_color="#f55dff", text_color="#5554ff")
 
-    # ##################################################################################
     # Establish all of the default values used
-    # ##################################################################################
     def set_defaults(self, first_time: bool) -> None:
         # Item names must be the same as their value in
         #  PrimeItems.program_arguments
         """
         Sets default values for attributes.
         Args:
             first_time: {bool}: Indicates if it is the first time running the program.
@@ -323,17 +337,20 @@
         self.conditions = self.preferences = self.taskernet = self.debug = self.everything = self.clear_settings = (
             self.reset
         ) = self.restore = self.exit = self.bold = self.highlight = self.italicize = self.underline = (
             self.go_program
         ) = self.outline = self.rerun = self.list_files = self.runtime = self.save = self.twisty = self.directory = (
             self.pretty
         ) = self.fetched_backup_from_android = False
-        self.single_project_name = self.single_profile_name = self.single_task_name = self.file = ""
+        self.single_project_name = ""
+        self.single_profile_name = ""
+        self.single_task_name = ""
+        self.file = ""
         self.color_text_row = 2
-        self.appearance_mode_optionemenu.set("System")
+        self.appearance_mode_optionmenu.set("System")
         self.appearance_mode = "system"
         self.indent_option.set(DEFAULT_DISPLAY_DETAIL_LEVEL)
         self.indent = 4
         self.color_labels = []
         self.android_ipaddr = ""
         self.android_port = ""
         self.android_file = ""
@@ -343,22 +360,23 @@
         self.font = OUTPUT_FONT
         self.gui = True
         self.color_row = 4
         self.message = ""
         self.ai_model = ""
         self.ai_analyze = False
         self.ai_model = ""
+        self.ai_prompt = AI_PROMPT
+        self.specific_name_msg = ""
 
         # Display current Items setting.
-        self.single_name_status("Display all Projects, Profiles, and Tasks.", "#3f99ff")
+        with contextlib.suppress(AttributeError):  # single_name_status may not be defined yet.
+            self.single_name_status(all_objects, "#3f99ff")
 
-    # ##################################################################################
     # Display the Backup button
-    # ##################################################################################
-    def display_backup_button(self, the_text: str, color1: str, color2: str, routine: object) -> None:
+    def display_backup_button(self, the_text: str, color1: str, color2: str, routine: Callable) -> None:
         """
         Displays a backup button on the GUI.
         Args:
             the_text: The text to display on the button in one line
             color1: The foreground color of the button in one line
             color2: The border color of the button in one line
         Returns:
@@ -383,17 +401,15 @@
             1,
             (200, 200),
             (0, 10),
             "nw",
         )
         return self.get_backup_button
 
-    # ##################################################################################
     # Display Message Box
-    # ##################################################################################
     def display_message_box(self, message: str, color: str) -> None:
         """
         Display Message Box
 
         Args:
             message (str): The text to display in the textbox.
             color (str): The color of the text.
@@ -448,17 +464,15 @@
         self.textbox.configure(state="disabled", font=(self.font, 14), wrap="word")
         self.textbox.tag_add(line_num_str, f"{line_num_str}.0", f"{line_num_str}.{len(message)!s}")
         # fmt: on
         self.textbox.tag_config(line_num_str, foreground=self.all_messages[line_num]["color"])
 
         self.textbox.focus_set()
 
-    # ##################################################################################
     # Validate name entered
-    # ##################################################################################
     def check_name(self, the_name: str, element_name: str) -> bool:
         """
         Checks name validity
         Args:
             the_name: str - Name to check
             element_name: str - Element type being named
         Returns:
@@ -477,44 +491,35 @@
                 f"Either the name entered for the {element_name} is blank or the 'Cancel' button was clicked.\n",
                 "All Projects, Profiles, and Tasks will be displayed.\n",
             ]
 
             self.named_item = False
         # Check to make sure only one named item has been entered
         elif self.single_project_name and self.single_profile_name:
-            error_message = [
-                "Error:\n\n",
-                "You have entered both a Project and a Profile name!\n",
-                f"(Project {self.single_project_name} and Profile {self.single_profile_name})\n",
-                "Try again and only select one.\n",
-            ]
+            error_message = setup_name_error("Project", "Profile", self.single_project_name, self.single_profile_name)
         elif self.single_project_name and self.single_task_name:
-            error_message = [
-                "Error:\n\n",
-                "You have entered both a Project and a Task name!\n",
-                f"(Project {self.single_project_name} and Task {self.single_task_name})\n",
-                "Try again and only select one.\n",
-            ]
+            error_message = setup_name_error("Project", "Task", self.single_project_name, self.single_task_name)
         elif self.single_profile_name and self.single_task_name:
-            error_message = [
-                "Error:\n\n",
-                "You have entered both a Profile and a Task name!\n",
-                f"(Profile {self.single_profile_name} and Task {self.single_task_name})\n",
-                "Try again and only select one.\n",
-            ]
+            error_message = setup_name_error("Profile", "Task", self.single_profile_name, self.single_task_name)
+
         # Make sure the named item exists
         elif not valid_item(self, the_name, element_name, self.debug, self.appearance_mode):
             front_error = f'Error: Trying to validate "{the_name}" {element_name}'
             if not PrimeItems.file_to_get:
                 error_message = [
                     f'{front_error}, but the "Cancel" was selected!\n',
                 ]
+                set_tasker_object_names(self)  # Update pulldown menus
             else:
+                try:
+                    file_name = PrimeItems.file_to_get.name
+                except AttributeError:
+                    file_name = PrimeItems.file_to_get
                 error_message = [
-                    f"{front_error} but it was not found in {PrimeItems.file_to_get.name}!  All Projects, Profiles and Tasks will be displayed.\n"
+                    f"{front_error} but it was not found in {file_name}!  All Projects, Profiles and Tasks will be displayed.\n",
                 ]
 
         # If we have an error, display it and blank out the various individual names
         if error_message:
             self.display_multiple_messages(error_message, False)
             (
                 self.single_project_name,
@@ -526,120 +531,76 @@
         # No error.
         self.display_message_box(
             f"Display only the '{the_name}' {element_name} (overrides any previous set name).",
             "Green",
         )
         return True
 
-    # ##################################################################################
-    # Display single item status.
-    # ##################################################################################
-    def single_name_status(self, status_message: str, color_to_use: str) -> None:
-        # Display The selection
-        """
-        Display a status message with a given color.
-        Args:
-            status_message: The status message to display in one line.
-            color_to_use: The color to use for the text in one line.
-        Returns:
-            None: No value is returned.
-        - The status message and color are passed to a CTkLabel widget.
-        - The label is placed in a grid layout on the "Specific Name" tab.
-        - Text color is set using the passed color."""
-
-        # Clear out any previous label
-        with contextlib.suppress(AttributeError):
-            self.single_label.destroy()
-        # Display the label.
-        self.single_label = add_label(
-            self,
-            self.tabview.tab("Specific Name"),
-            status_message,
-            ("#0BF075", f"{color_to_use}"),
-            0,
-            "normal",
-            5,
-            0,
-            20,
-            (10, 10),
-            "w",
-        )
-
-    # ##################################################################################
     # Process single name selection/event
-    # ##################################################################################
     def process_name_event(
         self,
         my_name: str,
-        checkbox1: customtkinter.CHECKBUTTON,
-        checkbox2: customtkinter.CHECKBUTTON,
-        checkbox3: customtkinter.CHECKBUTTON,
+        name_entered: str,
     ) -> None:
         #  Clear any prior error message.
         """
         Processes name event from checkboxes.
         Args:
             my_name: Name of item to filter by
-            checkbox1: First checkbox
-            checkbox2: Second checkbox
-            checkbox3: Checkbox clicked
+            name_entered: Name entered
         Returns:
             None
         Processing Logic:
             - Clear any prior error message
             - Deselect the other two checkboxes
             - Display prompt to enter name
             - Get name entered
             - Check if name is valid
             - If valid, deselect other buttons and set name
             - Notify user of filter
             - Deselect checkbox clicked
         """
-        self.textbox.destroy()
-        # Deselect the other two check boxes.
-        checkbox1.deselect()
-        checkbox2.deselect()
-        # Display prompt for name
-        dialog = customtkinter.CTkInputDialog(
-            text=f"Enter {my_name} name (case sensitive):",
-            title=f"Display Specific {my_name}",
-        )
-        # Get the name entered
-        name_entered = dialog.get_input()
-        # Name sure it is a valid name and display message.
+        if name_entered == "None":
+            self.display_message_box("'None' selected.  No change.", "Orange")
+            # Update the pulldown menus since without this the 'None' would display for some reason.
+            update_tasker_object_menus(self, get_data=True)
+            return
+        if name_entered in ["No profiles found", "No tasks found"]:
+            self.display_message_box("Selection ignored.", "Orange")
+            return
+        # Make sure it is a valid name and display message.
         if self.check_name(name_entered, my_name):
             # Name is valid... deselect other buttons and set the name
             self.single_project_name = self.single_profile_name = self.single_task_name = ""
             # Get the name entered
             match my_name:
                 case "Project":
                     self.single_project_name = name_entered
+                    # Clear out all of the old data for this new Project.
+                    # They will get repopulated by call to...
+                    # update_tasker_object_menus() > list_tasker_objects() > load_xml()
+                    clear_tasker_data()
 
                 case "Profile":
                     self.single_profile_name = name_entered
-                    with contextlib.suppress(AttributeError):
-                        self.profile_optionemenu.set(name_entered)
 
                 case "Task":
                     self.single_task_name = name_entered
-                    with contextlib.suppress(AttributeError):
-                        self.task_optionemenu.set(name_entered)
 
             # Let the user know...
-            self.single_name_status(f"Display only {my_name} '{name_entered}'.", "#3f99ff")
+            self.specific_name_msg = f"Display only {my_name} '{name_entered}'."
 
         else:
-            self.single_name_status("Display all Projects, Profiles, and Tasks.", "#3f99ff")
+            self.single_name_msg = all_objects
 
-        # Deselect the check box just selected
-        checkbox3.deselect()
+        # Update the pulldown menus and text labels, and set the color for Analyze button
+        update_tasker_object_menus(self, get_data=True)
+        display_analyze_button(self, 13)
 
-    # ##################################################################################
     # Process single name restore
-    # ##################################################################################
     def process_single_name_restore(
         self,
         my_name: str,
         name_entered: str,
     ) -> None:
         """
         Restores a single name based on the provided name type.
@@ -674,91 +635,64 @@
                 case "Profile":
                     self.single_profile_name = name_entered
                 case "Task":
                     self.single_task_name = name_entered
                 case _:
                     pass
 
-    # ##################################################################################
     # Process the Project Name entry
-    # ##################################################################################
-    def single_project_name_event(self) -> None:
+    def single_project_name_event(self, name_selected: str) -> None:
         """Generates a single project name event from button inputs
         Args:
             self: The class instance
+            name_selected: The name selected
         Returns:
             None: No value is returned
-        - Gets the project name from the second button
-        - Gets the event type from the third button
-        - Gets the timestamp from the first button
         - Calls process_name_event() to generate the event"""
-        self.process_name_event(
-            "Project",
-            self.string_input_button2,
-            self.string_input_button3,
-            self.string_input_button1,
-        )
+        name_selected = name_selected.replace("Project: ", "")
+        self.process_name_event("Project", name_selected)
 
-    # ##################################################################################
     # Process the Profile Name entry
-    # ##################################################################################
-    def single_profile_name_event(self) -> None:
+    def single_profile_name_event(self, name_selected: str) -> None:
         """Generates a single profile name event from button inputs
         Args:
             self: The class instance
+            name_selected: The name selected
         Returns:
             None: No value is returned
-        - Gets name from button1 input
-        - Gets category from button3 input
-        - Gets action from button2 input
         - Calls process_name_event to generate the event"""
-        self.process_name_event(
-            "Profile",
-            self.string_input_button1,
-            self.string_input_button3,
-            self.string_input_button2,
-        )
+        name_selected = name_selected.replace("Profile: ", "")
+        self.process_name_event("Profile", name_selected)
 
-    # ##################################################################################
     # Process the Task Name entry
-    # ##################################################################################
-    def single_task_name_event(self) -> None:
+    def single_task_name_event(self, name_selected: str) -> None:
         """Processes a single task name event.
         Args:
             self: The class instance.
+            name_selected: The name selected
         Returns:
             None: Does not return anything.
-        - Gets the task name from the first string input button
-        - Gets additional details from the other string input buttons
         - Calls process_name_event() to handle the full event"""
-        self.process_name_event(
-            "Task",
-            self.string_input_button1,
-            self.string_input_button2,
-            self.string_input_button3,
-        )
+        name_selected = name_selected.replace("Task: ", "")
+        self.process_name_event("Task", name_selected)
 
-    # ##################################################################################
     # Process the screen mode: dark, light, system
-    # ##################################################################################
     def change_appearance_mode_event(self, new_appearance_mode: str) -> None:
         """
         Change the appearance mode of the GUI
         Args:
             new_appearance_mode: The new appearance mode as a string
         Returns:
             None: Does not return anything
         - Set the global appearance mode to the new mode
         - Update the local appearance mode attribute to the new lowercased mode"""
         customtkinter.set_appearance_mode(new_appearance_mode)
         self.appearance_mode = new_appearance_mode.lower()
 
-    # ##################################################################################
     # Process the screen mode: dark, light, system
-    # ##################################################################################
     def font_event(self, font_selected: str) -> None:
         """
         Sets the font for the GUI
         Args:
             font_selected: The font name selected by the user
         Returns:
             None: No value is returned
@@ -777,33 +711,29 @@
             text=f"Monospaced Font To Use: {font_selected}",
             anchor="sw",
             font=(font_selected, 14),
         )
         self.font_out_label.grid(row=6, column=1, padx=10, pady=10, sticky="sw")
         self.display_message_box(f"Font To Use set to {font_selected}", "Green")
 
-    # ##################################################################################
     # Clear the message text box.
-    # ##################################################################################
     def clear_messages_event(self) -> None:
         """
         Clears the message box
         Args:
             None
         Returns:
             None
         Processing Logic:
             - Destroys the message box
         """
         self.all_messages = {}
         self.textbox.destroy()
 
-    # ##################################################################################
     # Process the Display Detail Level selection
-    # ##################################################################################
     def detail_selected_event(self, display_detail: str) -> None:
         """
         Set display detail level and update UI
         Args:
             display_detail (str): The selected display detail level
         Returns:
             None
@@ -839,33 +769,29 @@
         - Get value of checkbox passed as argument
         - Display message box with title and checkbox value
         - Return checkbox value"""
         checkbox_value = checkbox.get()
         self.inform_message(title, checkbox_value, "")
         return checkbox_value
 
-    # ##################################################################################
     # Process the Identation Amount selection
-    # ##################################################################################
     def indent_selected_event(self, ident_amount: str) -> None:
         """Indent selected text or code block
         Args:
             ident_amount: The amount of indentation to apply as a string
         Returns:
             None: No value is returned
         - Set the indent attribute to the passed ident_amount
         - Update the indent option dropdown to the selected amount
         - Display confirmation message of indentation amount"""
         self.indent = ident_amount
         self.indent_option.set(ident_amount)
         self.inform_message("Indentation Amount", True, ident_amount)
 
-    # ##################################################################################
     # Process color selection
-    # ##################################################################################
     def colors_event(self, color_selected_item: str) -> None:
         """
         Changes the color for a selected item
         Args:
             color_selected_item (str): The item whose color is to be changed
         Returns:
             None
@@ -918,17 +844,15 @@
                 text_color=color,
             )
             self.color_change.grid(row=self.color_row, column=0, padx=0, pady=0)
             self.color_row += 1
             if self.color_row > max_row:
                 self.color_row = 4
 
-    # ##################################################################################
     # Color selected...process it.
-    # ##################################################################################
     def extract_color_from_event(self, color: str, color_selected_item: str) -> None:
         """Maps a color name to a selected item
         Args:
             color: str - The color name
             color_selected_item: str - The name of the selected item
         Returns:
             None - No return value
@@ -936,17 +860,15 @@
             - Looks up the color name in a dictionary of color types
             - Adds the color as a value to the color lookup dictionary using the looked up color type as the key
             - This associates the given color with the given selected item"""
         self.color_lookup[TYPES_OF_COLOR_NAMES[color_selected_item]] = (
             color  # Add color for the selected item to our dictionary
         )
 
-    # ##################################################################################
     # Process the 'conditions' checkbox
-    # ##################################################################################
     def condition_event(self) -> None:
         """
         Get input and put message for condition checkbox
         Args:
             self: The class instance
             condition_checkbox: Condition checkbox input
             message: Message to display
@@ -956,49 +878,43 @@
         - Display message to user
         - Store input value in self.conditions"""
         self.conditions = self.get_input_and_put_message(
             self.condition_checkbox,
             "Display Profile and Task Action Conditions",
         )
 
-    # ##################################################################################
     # Process the 'Outline' checkbox
-    # ##################################################################################
     def outline_event(self) -> None:
         """
         Display Configuration Outline
         Args:
             self: The class instance
         Returns:
             None: Does not return anything
         - Get the input value of the outline_checkbox attribute
         - Call the get_input_and_put_message method to get user input and display a message
         - Assign the return value to the outline attribute
         """
         self.outline = self.get_input_and_put_message(self.outline_checkbox, "Display Configuration Outline")
 
-    # ##################################################################################
     # Process the 'Prettier' checkbox
-    # ##################################################################################
     def pretty_event(self) -> None:
         """
         Display Configuration Outline
         Args:
             self: The class instance
         Returns:
             None: Does not return anything
         - Get the input value of the outline_checkbox attribute
         - Call the get_input_and_put_message method to get user input and display a message
         - Assign the return value to the outline attribute
         """
         self.pretty = self.get_input_and_put_message(self.pretty_checkbox, "Display Pretty Output")
 
-    # ##################################################################################
     # Process the 'everything' checkbox
-    # ##################################################################################
     def everything_event(self) -> None:
         # Dictionary of program arguments and function to run for each upon restoration.
         """
         Handles toggling all options in the Everything event
         Args:
             self: The class instance
         Returns:
@@ -1059,32 +975,28 @@
             # Check if key is an attribute on self before setting
             if hasattr(self, key) and key != "display_detail_level":
                 setattr(self, key, value)
 
         # Handle Display Detail Level
         self.display_detail_level = DEFAULT_DISPLAY_DETAIL_LEVEL
 
-    # ##################################################################################
     # Process the 'Tasker Preferences' checkbox
-    # ##################################################################################
     def preferences_event(self) -> None:
         """
         Get user input on whether to display tasker preferences
         Args:
             self: The class instance
         Returns:
             None: Does not return anything
         - Get user input from preferences_checkbox checkbox
         - Store input in self.preferences
         - Display message based on input to confirm action"""
         self.preferences = self.get_input_and_put_message(self.preferences_checkbox, "Display Tasker Preferences")
 
-    # ##################################################################################
     # Process the 'Twisty' checkbox
-    # ##################################################################################
     def twisty_event(self) -> None:
         """
         Toggle display of task details under a twisty
         Args:
             self: The class instance
         Returns:
             None: No value is returned
@@ -1105,49 +1017,43 @@
         if self.twisty and self.everything:
             self.display_message_box(
                 "'Twisty' and 'Everything' are mutually exclusive.  Unchecking 'Twisty'.", "Orange"
             )
             self.twisty = False
             self.twisty_checkbox.deselect()
 
-    # ##################################################################################
     # Process the 'Display Directory' checkbox
-    # ##################################################################################
     def directory_event(self) -> None:
         """
         Get input and put message for directory checkbox
         Args:
             self: The class instance
             directory_checkbox: The directory checkbox
             "Display Directory": The message to display
         Returns:
             None: Does not return anything
         - Get input value from directory_checkbox
         - If checked, put message "Display Directory"
         - Does not return anything, just updates class attribute"""
         self.directory = self.get_input_and_put_message(self.directory_checkbox, "Display Directory")
 
-    # ##################################################################################
     # Process the 'Bold Names' checkbox
-    # ##################################################################################
     def names_bold_event(self) -> None:
         """
         Get input to display names in bold and put message
         Args:
             self: The class instance
         Returns:
             None: No value is returned
         - Get input value from bold_checkbox attribute
         - Put message "Display Names in Bold" based on input
         - No return value, function updates attribute on class instance"""
         self.bold = self.get_input_and_put_message(self.bold_checkbox, "Display Names in Bold")
 
-    # ##################################################################################
     # Process the 'Highlight Names' checkbox
-    # ##################################################################################
     def names_highlight_event(self) -> None:
         """
         Get input and put message for names highlight checkbox
         Args:
             self: The class instance
             highlight_checkbox: The checkbox input element
             "Display Names Highlighted": The message to display
@@ -1155,80 +1061,70 @@
             None: No value is returned
         - Get the value of the highlight_checkbox input
         - If checked, put the "Display Names Highlighted" message
         - If not checked, do not put any message
         """
         self.highlight = self.get_input_and_put_message(self.highlight_checkbox, "Display Names Highlighted")
 
-    # ##################################################################################
     # Process the 'Italicize Names' checkbox
-    # ##################################################################################
     def names_italicize_event(self) -> None:
         """
         Italicize names based on checkbox input
         Args:
             self: The class instance
         Returns:
             None: No value is returned
         - Get input value from italicize_checkbox checkbox
         - Put message based on input value to "Display Names Italicized" label
         - No return value, function updates UI state directly
         """
         self.italicize = self.get_input_and_put_message(self.italicize_checkbox, "Display Names Italicized")
 
-    # ##################################################################################
     # Process the 'Underline Names' checkbox
-    # ##################################################################################
     def names_underline_event(self) -> None:
         """
                 Gets user input to display names underlined or not
                 Args:
                     self: The class instance
                 Returns:
                     None: No value is returned
                 - Gets user input from the underline_checkbox checkbox
                 - Passes the input value and a label to get_input_and_put_message()
         #Loading.
         """
         self.underline = self.get_input_and_put_message(self.underline_checkbox, "Display Names Underlined")
 
-    # ##################################################################################
     # Process the 'Taskernet' checkbox
-    # ##################################################################################
     def taskernet_event(self) -> None:
         """
         Display TaskerNet Information
         Args:
             self: The TaskerNet object
         Returns:
             None: Does not return anything
         - Check if TaskerNet checkbox is checked
         - Get user input for displaying TaskerNet information
         - Put message dialog to display TaskerNet information
         """
         self.taskernet = self.get_input_and_put_message(self.taskernet_checkbox, "Display TaskerNet Information")
 
-    # ##################################################################################
     # Process the 'Runtime' checkbox
-    # ##################################################################################
     def runtime_checkbox_event(self) -> None:
         """
         Get input and put message for runtime checkbox
         Args:
             self: The class instance
         Returns:
             None: No return value
         - Get value of runtime_checkbox input
         - If checked, put message "Display Runtime Settings"
         - No return value, function modifies instance attributes"""
         self.runtime = self.get_input_and_put_message(self.runtime_checkbox, "Display Runtime Settings")
 
-    # ##################################################################################
     # Rebuilld message box with new text (e.g. for Help).
-    # ##################################################################################
     def new_message_box(self, message: str) -> None:
         # Clear any prior error message
         """
         Displays a message in a textbox widget.
         Args:
             message (str): The message to display
         Returns:
@@ -1256,61 +1152,53 @@
             "color",
             "1.0",
             f"1.{len(message)}",
         )  # '1.5' means first line, 5th character; '1.11' means first line, 11th character
         self.textbox.tag_config("color", foreground="green")
         self.all_messages = {}
 
-    # ##################################################################################
     # Process the 'Display Help' button
-    # ##################################################################################
     def help_event(self) -> None:
         """Displays help information in a message box.
         Args:
             self: The class instance.
         Returns:
             None: Does not return anything.
         - Constructs a message with help text information
         - Opens a new message box window
         - Displays the help message text in the message box"""
         self.new_message_box(HELP)
 
-    # ##################################################################################
     # Process the 'Get Backup Help' button
-    # ##################################################################################
     def backup_help_event(self) -> None:
         """Backs up help text and displays it in a message box
         Args:
             self: The class instance
         Returns:
             None: Does not return anything
         Processes:
             - Fetches the backup help text from a constant
             - Creates a new message box window
             - Displays the backup help text in the message box"""
         self.new_message_box("Fetch Backup Help\n\n" + BACKUP_HELP_TEXT)
 
-    # ##################################################################################
     # Process the '?' List XML Files query button
-    # ##################################################################################
     def listfile_query_event(self) -> None:
         """Function to display help text for the listfile_query_event method.
         Parameters:
             - self (object): The object that the method is being called on.
         Returns:
             - None: This method does not return anything.
         Processing Logic:
             - Displays help text for listfile_query_event method.
             - Uses new_message_box method.
             - Help text is stored in LISTFILES_HELP_TEXT variable."""
         self.new_message_box("List XML Files Help\n\n" + LISTFILES_HELP_TEXT)
 
-    # ##################################################################################
     # Process the '?' Tree View query button
-    # ##################################################################################
     def treeview_query_event(self) -> None:
         """Function to display help text for the listfile_query_event method.
         Parameters:
             - self (object): The object that the method is being called on.
         Returns:
             - None: This method does not return anything.
         Processing Logic:
@@ -1342,17 +1230,15 @@
             extra = " to "
         elif toggle_value:
             response = "On"
         else:
             response = "Off"
         self.display_message_box(f"{toggle_name} set{extra}{response}", "Green")
 
-    # ##################################################################################
     # Process the 'Save Settings' checkbox
-    # ##################################################################################
     def save_settings_event(self) -> None:
         # Get program arguments from GUI and store in a temporary dictionary
         """
         Saves program settings from GUI to file.
         Args:
             self: The class instance.
         Returns:
@@ -1394,17 +1280,15 @@
             status: A string indicating if the checkbox was selected or deselected
         - Check if checked is True, call checkbox.select() to select it
         - Check if checked is False, call checkbox.deselect() to deselect it
         - Return a string with the argument name and checked status"""
         checkbox.select() if checked else checkbox.deselect()
         return f"{argument_name} set to {checked}.\n"
 
-    # ##################################################################################
     # Restore displays setting from restored value!
-    # ##################################################################################
     def restore_display(self, key: str, value: str) -> str:
         # Dictionary of program arguments and function to run for each upon restoration.
         """
         Restores display settings
         Args:
             key: str - Setting name
             value: str - Setting value
@@ -1504,32 +1388,31 @@
         if message.endswith(the_empty_ending):
             message = f"{message[:-the_empty_ending_length]} is not set.\n"
         elif message.endswith(named_ending):
             message = f"{message[:-named_ending_length]} is not named.\n"
 
         return message
 
-    # ##################################################################################
     # Process the 'Restore Settings' checkbox
-    # ##################################################################################
-    def restore_settings_event(self) -> None:
+    def restore_settings_event(self, first_time: bool) -> None:
         """
         Resets settings to defaults and restores from saved settings file
         Args:
             self: The class instance
+            first_time: bool - True if this is the first time the checkbox is clicked
         Returns:
             None: No value is returned
         Processing Logic:
             - Reset all values to defaults
             - Restore saved settings from file
             - Check for errors and display messages
             - Extract restored settings into class attributes
             - Empty message queue after restoring
         """
-        self.set_defaults(False)  # Reset all values
+        self.set_defaults(first_time)  # Reset all values
         temp_args = self.color_lookup = {}
         # Restore all changes that have been saved
         temp_args, self.color_lookup = save_restore_args(temp_args, self.color_lookup, False)
 
         # Check for errors
         with contextlib.suppress(KeyError):
             if temp_args["msg"]:
@@ -1551,17 +1434,15 @@
             #    self.all_messages = {}
             #    self.display_message_box("Settings restored.", "Green")
 
         # No arguments mean no settings.
         else:  # Empty?
             self.display_message_box("No settings file found.", "Orange")
 
-    # ##################################################################################
     # We have read colors and runtime args from backup file.  Now extract them for use.
-    # ##################################################################################
     def extract_settings(self, temp_args: dict) -> None:
         """
         Extract settings from arguments dictionary
         Args:
             temp_args: Dictionary of settings
         Returns:
             None: Does not return anything
@@ -1590,17 +1471,15 @@
                         text_out = f"{value} (displayed as white)"
                     with contextlib.suppress(KeyError):
                         self.display_message_box(f"{inv_color_names[key]} color set to {text_out}\n", color)
 
         # Display completion
         self.display_message_box("Settings restored.\n", "Green")
 
-    # ##################################################################################
     # Display an input field and a label for the user to input a value
-    # ##################################################################################
     def display_label_and_input(
         self,
         label: str,
         default_value: str,
         starting_row: int,
         indentation_x_label: int,
         indentation_y_label: int,
@@ -1668,17 +1547,15 @@
                 columnspan=1,
                 padx=(0, 90),
                 pady=(0, 0),
                 sticky=sticky,
             )
         return input_name, label_name
 
-    # ##################################################################################
     # Process the 'Backup' IP Address/port/file location
-    # ##################################################################################
     def get_backup_event(self) -> None:
         # Set up default values
         """
         Gets backup event details from user.
         Args:
             self: The class instance.
         Returns:
@@ -1812,17 +1689,15 @@
             "Enter 1-3 and Click Here to Set XML Details",
             "#D62CFF",
             "#6563ff",
             self.fetch_backup_event,
         )
         self.get_backup_button.configure(anchor="center", width=600)
 
-    # ##################################################################################
     # Fetch Backup info error...process it.
-    # ##################################################################################
     def backup_error(self, error_message: str) -> None:
         # Setup error message
         """
         Displays an error message and resets the UI.
 
         Args:
             error_message (str): The error message to display.
@@ -1833,36 +1708,32 @@
             - Display the error message in a message box
             - Delete any text in the entry field
             - Reset the 'Get Backup Settings' button definition and grid placement
         """
         if error_message:
             self.display_message_box(error_message, "Red")
 
-    # ##################################################################################
     # Get list of lines and output them.
-    # ##################################################################################
     def display_multiple_messages(self, details: list, good_or_bad: bool) -> None:
         """
         Display Android settings based on the given details list.
 
         :param self: The instance of the class.
         :param details: A list containing the details to be displayed.
         :param good_or_bad: True = good (green), False = bad (red).
         :return: None
         """
         color = "Green" if good_or_bad else "Red"
         for line in details:
             self.display_message_box(line, color)
 
-    # ##################################################################################
     # Fetch the backup ip and file details, and validate.
     # This function can be entered through two paths:
     # 1- User clicked on the 'Get Backup Settings' button
     # 2- User clicked on the 'List XML Files' button
-    # ##################################################################################
     def fetch_backup_event(self) -> None:
         """Fetches backup event details from user input
 
         Args:
             self: The class instance
         Returns:
             None: No value is returned
@@ -1937,20 +1808,18 @@
             ],
             True,
         )
 
         # Display backup details as a label again.
         self.display_backup_details()
 
-        # Display the profile or task names
-        self.display_ai_profile_task_names()
+        # Update the Project/Profile/Task pulldown option menus and labels.
+        update_tasker_object_menus(self, get_data=False)
 
-    # ##################################################################################
     # Fetching backup from Android.  Let the user know the specific details.
-    # ##################################################################################
     def display_backup_details(self) -> None:
         """
         Displays backup details from Android device.
         Args:
             self: The class instance.
         Returns:
             None: Does not return anything.
@@ -2002,17 +1871,15 @@
             (0, 50),
             "ne",
         )
 
         # Display the current file in sidebar
         display_current_file(self, self.android_file)
 
-    # ##################################################################################
     # Cancel the entry of backup parameters
-    # ##################################################################################
     def backup_cancel_event(self) -> None:
         """
         Closes the backup details window.
         Args:
             self: The class instance
         Returns:
             None
@@ -2020,32 +1887,28 @@
         clear_android_buttons(self)
         self.fetched_backup_from_android = False
         self.android_file = ""
         self.android_ipaddr = ""
         self.android_port = ""
         self.display_message_box("'Get XML From Android' Cancelled.", "Orange")
 
-    # ##################################################################################
-    # List files event
-    # ##################################################################################
+    # List (Android) XML files event
     def list_files_event(self) -> None:
         """
         Closes the backup details window.
         Args:
             self: The class instance
         Returns:
             None
         """
         self.list_files = True
         self.list_files_button.configure(text="List Files Selected")
         self.fetch_backup_event()
 
-    # ##################################################################################
-    # User has selected a specific XML file from pulldown menu.
-    # ##################################################################################
+    # User has selected a specific XML file to get from Android device from pulldown menu.
     def file_selected_event(self, android_file: str) -> None:
         """User has selected a specific XML file from pulldown menu.
         Returns:
             - None: Adds android_file to file_list."""
         self.android_file = android_file
         clear_android_buttons(self)
         self.display_multiple_messages(
@@ -2064,23 +1927,24 @@
 
         # Not valid XML...
         if return_code > 0:
             self.display_message_box(error_message, "Red")  # Error out and exit
             self.android_file = ""
             return
 
-        # Display backup details as a label again.
+        # Get rid of any data we currently have
+        clear_tasker_data()
+
+        # Display backup details as a labels again.
         self.display_backup_details()
 
-        # Display the profile or task names
-        self.display_ai_profile_task_names()
+        # Refresh the Projects/Profiles/Tasks pulldown menus and labels
+        update_tasker_object_menus(self, get_data=False)
 
-    # ##################################################################################
     # Process the 'Reset Settings' button
-    # ##################################################################################
     def reset_settings_event(self) -> None:
         """
         Resets all class settings to default values.
         Args:
             self: The class instance.
         Returns:
             None
@@ -2091,15 +1955,15 @@
         self.android_file = ""
         self.sidebar_detail_option.set(DEFAULT_DISPLAY_DETAIL_LEVEL)  # display detail level
         self.indent_option.set("4")  # Indentation amount
         self.condition_checkbox.deselect()  # Conditions
         self.preferences_checkbox.deselect()  # Tasker Preferences
         self.pretty_checkbox.deselect()  # Pretty output
         self.taskernet_checkbox.deselect()  # TaskerNet
-        self.appearance_mode_optionemenu.set("System")  # Appearance
+        self.appearance_mode_optionmenu.set("System")  # Appearance
         customtkinter.set_appearance_mode("System")  # Enforce appearance
         self.debug_checkbox.deselect()  # Debug
         self.display_message_box("Settings reset.", "Green")
         self.twisty_checkbox.deselect()  # Twisty
         self.directory_checkbox.deselect()  # directory
         self.bold_checkbox.deselect()  # bold
         self.italicize_checkbox.deselect()  # italicize
@@ -2120,25 +1984,27 @@
         PrimeItems.colors_to_use = set_color_mode(self.appearance_mode)
         PrimeItems.output_lines = LineOut()
         PrimeItems.program_arguments = initialize_runtime_arguments()
         PrimeItems.program_arguments["debug"] = self.debug
 
         # Reset/display our Ai settings.
         with contextlib.suppress(AttributeError):
-            self.ai_set_label2.destroy()
-            self.profile_optionemenu.set("None")
-            self.task_optionemenu.set("None")
-        display_ai_settings(self)
+            self.profile_optionmenu.set("None")
+        with contextlib.suppress(AttributeError):
+            self.task_optionmenu.set("None")
+        self.ai_prompt = AI_PROMPT
+        self.ai_model = "None (llama3)"
+
+        # Update the Tasker selected object pulldown names and labels
+        update_tasker_object_menus(self, get_data=False)
 
         # Reset current file
         display_current_file(self, "None")
 
-    # ##################################################################################
     # Process Debug Mode checkbox
-    # ##################################################################################
     def debug_checkbox_event(self) -> None:
         """
         Handle debug checkbox event
         Args:
             self: The class instance
         Returns:
             None
@@ -2160,17 +2026,15 @@
                     ("Debug mode requires Tasker XML file to be named: 'backup.xml', which is missing.  No change."),
                     "Red",
                 )
                 self.debug = False
         else:
             self.display_message_box("Debug mode disabled.", "Green")
 
-    # ##################################################################################
     # User has requested that the colors be result to their defaults.
-    # ##################################################################################
     def color_reset_event(self) -> None:
         """Resets the color mode for Tasker items.
         Parameters:
             self (object): The current instance of the class.
         Returns:
             None: This function does not return anything.
         Processing Logic:
@@ -2181,17 +2045,15 @@
 
         PrimeItems.colors_to_use = set_color_mode(self.appearance_mode)
         self.color_lookup = {}
         self.display_message_box("Tasker items set back to their default colors.", "Green")
         with contextlib.suppress(Exception):
             self.color_change.destroy()
 
-    # ##################################################################################
     # Close the GUI.
-    # ##################################################################################
     def cleanup(self, run_only: bool) -> None:
         """Function:
         Closes the application.
         Parameters:
             run_only (bool): If True, only closes the application. If False, closes the application and withdraws the funds.
         Returns:
             None: Does not return anything.
@@ -2203,28 +2065,29 @@
             self.quit()
         else:
             self.withdraw()
             self.quit()
             self.quit()
             self.sidebar_frame.destroy()
 
-    # ##################################################################################
     # Validate XML and close the GUI.
-    # ##################################################################################
     def cleanup_and_run(self, run_only: bool) -> None:
         """Function: cleanup_and_run
         Parameters:
             run_only (bool): Flag to determine if program should only run and not display GUI.
         Returns:
             None: Does not return any value.
         Processing Logic:
             - Display "Program running..." message.
             - If XML is not valid, return to GUI.
             - If XML is valid, exit and return to process_gui.
             - If XML is not valid, return to GUI."""
+        # Save our last window position
+        self.window_position = self.winfo_geometry()
+
         self.display_message_box("Program running...", "Green")
 
         # If XML is not valid, simply return to GUI.  Otherwise, exit and return to process_gui.
         if PrimeItems.xml_tree is None:
             PrimeItems.program_arguments["gui"] = True
             # Get and validate the XML.
             if self.load_xml():  # If true, the XML is valid.  Signal exit.
@@ -2236,17 +2099,15 @@
 
         # We already have the XML.  Just exit.
         if not self.ai_analyze:
             self.cleanup(run_only)
         else:
             self.quit()
 
-    # ##################################################################################
     # The 'Run' program button has been pressed.  Set the run flag and close the GUI
-    # ##################################################################################
     def run_program(self) -> None:
         """
         Starts a program and displays a message box.
         Args:
             self: The class instance.
         Returns:
             None: Does not return anything.
@@ -2255,33 +2116,29 @@
         - Calls the quit() method to exit the program"""
         self.go_program = True
         self.rerun = False
 
         # Validate the XML and cleanup
         self.cleanup_and_run(run_only=True)
 
-    # ##################################################################################
     # The 'ReRun' program button has been pressed.  Set the run flag and close the GUI
-    # ##################################################################################
     def rerun_the_program(self) -> None:
         """
         Resets the program state and exits.
         Args:
             self: The class instance.
         Returns:
             None: Does not return anything.
         - Sets the rerun flag to True to restart the program on next run
         - Calls withdraw() to reset the program state
         - Calls quit() twice to ensure program exits"""
         self.rerun = True
         self.cleanup_and_run(run_only=False)
 
-    # ##################################################################################
     # The Upgrade Version button has been pressed.
-    # ##################################################################################
     def upgrade_event(self) -> None:
         """ "Runs an update and reruns the program."
         Parameters:
             - self (object): Instance of the class.
         Returns:
             - None: No return value.
         Processing Logic:
@@ -2289,17 +2146,15 @@
             - Reruns the program to pick up the update."""
         update()
         self.display_message_box("Program updated.  Restarting...", "Green")
         # Create the Change Log file to be read and displayed after a program update.
         create_changelog()
         do_rerun()
 
-    # ##################################################################################
     # The Upgrade Version button has been pressed.
-    # ##################################################################################
     def report_issue_event(self) -> None:
         """Opens a web browser and directs the user to create a new issue on GitHub for the Map-Tasker project.
         Parameters:
             - self (object): The instance of the class calling the function.
         Returns:
             - None: This function does not return any values.
         Processing Logic:
@@ -2314,35 +2169,35 @@
         try:
             webbrowser.open(f"https:{PrimeItems.slash*2}{url}", new=2)
         except webbrowser.Error:
             self.display_message_box("Error: Failed to open output in browser: your browser is not supported.", "Red")
             return
         self.new_message_box("Report an Issue or Request a Feature\n\n" + issue_text)
 
-    # ##################################################################################
     # The 'Exit' program button has been pressed.  Call it quits
-    # ##################################################################################
     def exit_program(self) -> None:
         """
         Exits the program by setting exit flag and calling quit twice
         Args:
             self: The object instance
         Returns:
             None: Does not return anything
         - Sets the exit flag to True to indicate program exit
         - Calls quit() twice to ensure program exits cleanly
         - Calling quit() twice is done as a precaution in case one call fails to exit for some reason
         """
         self.exit = True
+
+        # Save our last window position
+        self.window_position = self.winfo_geometry()
+
         self.quit()
         self.quit()
 
-    # ##################################################################################
     # Prompt for and get the XML file from the local drive.
-    # ##################################################################################
     def prompt_and_get_file(self, debug: bool, appearance_mode: str) -> bool:
         """
         Prompt for and get the XML file from the local drive.
 
         Args:
             self: The object instance.
             debug: Debug flag.
@@ -2358,19 +2213,21 @@
                 self.display_message_box("Cancel button pressed.\n", "Orange")
             else:
                 self.display_multiple_messages(
                     [f"{PrimeItems.error_msg}\n", "Click 'Reset Options' to try a different XML file."],
                     "Red",
                 )
             return False
+
+        # Good return from getting the XML
+        if PrimeItems.file_to_get.name:
+            self.display_and_set_file(PrimeItems.file_to_get.name)
         return True
 
-    # ##################################################################################
     # Load the XML if not already loaded.
-    # ##################################################################################
     def load_xml(self) -> bool:
         """Load XML from a file or URL.
         Parameters:
             self (Tasker): Instance of Tasker class.
         Returns:
             - bool: True if successful, False otherwise.
         Processing Logic:
@@ -2409,17 +2266,15 @@
                 PrimeItems.program_arguments["gui"] = True
                 return_code = get_the_xml_data()
                 if return_code != 0:
                     return False
 
         return True
 
-    # ##################################################################################
     # Display a treeview of the XML.
-    # ##################################################################################
     def treeview_event(self) -> None:
         """Handles the event of clicking on the treeview.
         Parameters:
             - self (object): The object calling the function.
         Returns:
             - None: This function does not return anything.
         Processing Logic:
@@ -2440,17 +2295,15 @@
 
             # Build our tree from XML data
             tree_data = self.build_the_tree()
 
             # Display the tree
             self.display_tree(tree_data)
 
-    # ##################################################################################
     # Build a hierarchical list of all of the Tasker elements.
-    # ##################################################################################
     def build_the_tree(self) -> list:
         """Builds the hierarchical list of all of the Tasker elements.
         Parameters:
             self (object): The object calling the function.
         Returns:
             tree_data (list): The hierarchical list of all of the Tasker elements.
         Processing Logic:
@@ -2490,17 +2343,15 @@
 
                 # Put it all together: Project, Profiles, and Tasks
                 tree_data.append({"name": f"Project: {project_name}", "children": profile_list})
 
         # Return our data tree
         return tree_data
 
-    # ##################################################################################
     # Display the tree view.
-    # ##################################################################################
     def display_tree(self, tree_data: list) -> None:
         """Displays a treeview window with given data.
         Parameters:
             tree_data (list): List of data to be displayed in the treeview.
         Returns:
             None: This function does not return anything.
         Processing Logic:
@@ -2516,17 +2367,15 @@
 
             # Display the tree in the toplevel window.
             tree_view = CTkTreeview(master=self.toplevel_window, items=tree_data)
             tree_view.pack(padx=10, pady=10, fill="both", expand=True)
         else:
             self.display_message_box("No Project(s) Found in XML!", "Red")
 
-    # ##################################################################################
     # Displayh Ai Analysis response in a separate top level window.
-    # ##################################################################################
     def display_ai_response(self, error_msg: str) -> None:
         """
         Display AI response in a GUI window.
 
         Args:
             error_msg (str): The error message to display in the GUI.
 
@@ -2539,17 +2388,15 @@
             self.toplevel_window.focus()  # if window exists focus it
 
         # Display the analysis in the toplevel window.
         analysis_view = CTkAnalysisview(master=self.toplevel_window, message=error_msg)
         analysis_view.pack(padx=10, pady=10, fill="both", expand=True)
         analysis_view.after(10, self.toplevel_window.lift)
 
-    # ##################################################################################
     # Set and display the file name.
-    # ##################################################################################
     def display_and_set_file(self, filename: str) -> None:
         """
         Display the current file name in a button on the GUI and set it as the current file.
 
         Args:
             filename (str): The name of the current file.
 
@@ -2567,43 +2414,41 @@
             gui_instance.display_and_set_file("example.txt")
             ```
         """
         display_current_file(self, filename)
         self.display_message_box(f"Current file set to {filename}", "Green")
         self.file = filename  # Set this so it is saved in settings.
 
-    # ##################################################################################
     # Get XML button clicked.  Prompt usere for XML and load it.
-    # ##################################################################################
     def getxml_event(self) -> None:
         """
         Get rid of any existing data, clear tasker root elements, and negate file indications.
         Set IP address, port, and file to empty strings.
         Prompt user for a new XML file and display the current file if successful.
         """
         # Get rid of any data we currently have
         PrimeItems.tasker_root_elements["all_projects"].clear()
         PrimeItems.tasker_root_elements["all_profiles"].clear()
         PrimeItems.tasker_root_elements["all_tasks"].clear()
         PrimeItems.tasker_root_elements["all_scenes"].clear()
+        self.single_project_name = ""
+        self.single_profile_name = ""
+        self.single_task_name = ""
+        self.specific_name_msg = ""
         # Negate any indication that we have a file
         PrimeItems.file_to_get = ""
         PrimeItems.program_arguments["file"] = ""
         self.android_ipaddr = ""
         self.android_port = ""
         self.android_file = ""
 
-        # Get the new XML file
-        if self.prompt_and_get_file(False, self.appearance_mode):
-            # Set the name and display it
-            self.display_and_set_file(PrimeItems.file_to_get.name)
+        # Redisplay the Projects/Profiles/Tasks pulldown menus for selection
+        update_tasker_object_menus(self, get_data=True)
 
-    # ##################################################################################
     # Show for edit the AI API Key
-    # ##################################################################################
     def ai_apikey_event(self) -> None:
         """
         Prompts the user to enter their API key, or leaves it as is if it already exists.
         If the user enters a new API key, it is saved to a file.
 
         Parameters:
             None
@@ -2627,76 +2472,43 @@
             # Write out the new key
             with open(KEYFILE, "w") as key_file:
                 key_file.write(new_key)
                 self.display_message_box(f"API key saved: '{new_key}' .", "Green")
                 self.ai_apikey = new_key
 
             # Redisplay ai settings with new key.
-            self.ai_set_label1.destroy()
-            display_ai_settings(self)
+            display_selected_object_labels(self)
 
         # Usaer hit 'Cancel' or didn't input anything
         else:
             self.display_message_box("No change to the API key!", "Orange")
 
-    # ##################################################################################
     # Show for edit the AI API Key
-    # ##################################################################################
     def ai_model_selected_event(self, model: str) -> None:
         """
         Set the AI model to the specified model.
 
         Parameters:
             model (str): The model to set.
 
         Returns:
             None
         """
-        if model == "none (llama3)":
+        if model == "None (llama3)":
             model = "llama3"
         self.ai_model = model
         self.display_message_box("Model set to " + model + ".", "Green")
 
         # Redisplay the Analyze button.
-        display_analyze_button(self, 10)
-
-        # Get the Profile or Task to analyize if we don't already have it.
-        if self.single_profile_name or self.single_task_name:
-            return
-
-        # Get the Profile or Task to analyze
-        _ = list_profiles_and_tasks(self)
+        display_analyze_button(self, 13)
 
         # Redisplay the ai settings
-        with contextlib.suppress(AttributeError):
-            self.ai_set_label2.destroy()
-        display_ai_settings(self)
-
-    # ##################################################################################
-    #  Displays the profile and task names in the "Analyze" tab of the tabview.
-    # ##################################################################################
-    def display_ai_profile_task_names(self) -> None:
-        """
-        Displays the profile and task names in the "Analyze" tab of the tabview.
-
-        Parameters:
-            None
+        display_selected_object_labels(self)
 
-        Returns:
-            None
-        """
-        profile_to_display = self.single_profile_name if self.single_profile_name else "None"
-        task_to_display = self.single_task_name if self.single_task_name else "None"
-        with contextlib.suppress(AttributeError):
-            self.profile_optionemenu.set(profile_to_display)
-            self.task_optionemenu.set(task_to_display)
-
-    # ##################################################################################
     # Kickoff the AI analysis
-    # ##################################################################################
     def ai_analyze_event(self) -> None:
         """
         Analyzes a single item identified by the current instance.
 
         This function checks if the instance has a single project name, profile name, or task name.
         If so, it sets the `ai_analyze` attribute to True, displays a message box indicating the analysis is running
         with the current model, and reruns the program.
@@ -2711,111 +2523,103 @@
             None
         """
         if self.single_profile_name == "None or unnamed!":
             self.single_profile_name = ""
         # Do we have a single item identified?
         if self.single_project_name or self.single_profile_name or self.single_task_name:
             self.ai_analyze = True
-            self.all_messages = {}  # Clear out all displayed messages.
+            self.clear_messages_event()  # Clear out all displayed messages.
             self.display_message_box(f"Running analysis with model {self.ai_model}.", "Green")
             self.rerun_the_program()
         else:
             self.display_message_box(
                 "Single Project/Profile/Task has not been selected!  Select only one and try again.",
                 "Orange",
             )
             # Get the Profile or Task to analyze
             self.ai_analyze_button.destroy()
             # If there are no Profiles or Tasks, redisplay the Analyze button
-            if not list_profiles_and_tasks(self):
+            if not list_tasker_objects(self):
                 # Drop here if we don't have any XML loaded yet.
-                display_analyze_button(self, 10)
+                display_analyze_button(self, 13)
 
-            # Display the profile or task names
-            self.display_ai_profile_task_names()
+            # Update the Project/Profile/Task pulldown option menus.
+            set_tasker_object_names(self)
 
-    # ##################################################################################
-    # The user has selected a Profile from the pulldown list
-    # ##################################################################################
-    def ai_profile_selected_event(self, profile_name: str) -> None:
+    # Process the '?' Tree View query button
+    def ai_help_event(self) -> None:
+        """Function to display help text for the Analysis tab.
+        Parameters:
+            - self (object): The object that the method is being called on.
+        Returns:
+            - None: This method does not return anything.
+        Processing Logic:
+            - Displays help text for Analysis tab.
+            - Uses new_message_box method.
+            - Help text is stored in AI_HELP_TEXT variable."""
+        self.new_message_box("Analyze Help\n\n" + AI_HELP_TEXT)
+
+    # Handle Ai Prompt change event.
+    def ai_prompt_event(self) -> None:
         """
-        Handles the event when a profile is selected.
+        Handles the event when the AI prompt is changed.
 
-        Args:
-            profile_name (str): The name of the selected profile.
+        Opens a dialog box for the user to enter a new AI prompt. Displays the current prompt and prompts the user to
+        enter a new prompt.
+
+        If the user cancels the prompt change, a message box is displayed indicating that the prompt change was cancelled.
+        If the user enters the same prompt as the current prompt, a message box is displayed indicating that the prompt did not change.
+        If the user enters a new prompt, the AI prompt is updated and a message box is displayed indicating the new prompt.
+
+        Parameters:
+            self (object): The instance of the class.
 
         Returns:
             None
         """
-        if profile_name and profile_name != "None":
-            if profile_name == "No profiles found":
-                self.display_message_box("Profile selection ignored.", "Orange")
-                return
-            self.single_profile_name = profile_name.replace("Profile: ", "")
-            self.display_message_box(f"Single Profile: {self.single_profile_name} selected.", "Green")
-            if self.single_task_name:
-                self.display_message_box(f"Single Task '{self.single_task_name}' ignored.", "Orange")
-                self.single_task_name = ""
-                self.task_optionemenu.set("None")
-
-            # Cleanup the buttons
-            # self.ai_profile_label.destroy()
-            # self.profile_optionemenu.destroy()
-            self.ai_set_label3.destroy()
-            display_analyze_button(self, 10)
-
-            # Redisplay the ai settings
-            display_ai_settings(self)
-
-        # None was selected
+        dialog = customtkinter.CTkInputDialog(
+            text=f"Current prompt: '{self.ai_prompt}'\n\nEnter a new prompt for the AI to use:",
+            title="Change the Ai Prompt",
+        )
+        # Get the name entered
+        name_entered = dialog.get_input()
+        # Canceled?
+        if name_entered is None:
+            self.display_message_box("Prompt change cancelled.", "Orange")
+        # The same?
+        elif name_entered == self.ai_prompt:
+            self.display_message_box("Prompt did not change.", "Orange")
         else:
-            self.display_message_box("Profile selection of 'None' ignored.", "Orange")
+            # Valid response.
+            self.ai_prompt = name_entered
+            self.display_message_box(f"Prompt changed to '{self.ai_prompt}'.", "Green")
+            display_selected_object_labels(self)
 
-    # ##################################################################################
-    # The user has selected a Task from the pulldown list
-    # ##################################################################################
-    def ai_task_selected_event(self, task_name: str) -> None:
+    # Display what is in the changelog for the new release.
+    def whatsnew_event(self) -> None:
         """
-        Handles the event when a profile is selected.
+        Retrieves the latest changelog from the Map-Tasker GitHub repository and displays it in the user interface.
 
-        Args:
-            task_name (str): The name of the selected profile.
+        This function sends a GET request to the specified URL to retrieve the changelog in JSON format. It then iterates through the changelog dictionary and displays each line in the user interface using the `display_message_box` method. The changelog is displayed starting from the latest version until the "Older History" section is reached. The function also clears any previously displayed messages before displaying the changelog.
+
+        Parameters:
+            self (object): The instance of the class.
 
         Returns:
             None
         """
-        if task_name and task_name != "None":
-            if task_name == "No tasks found":
-                self.display_message_box("Task selection ignored.  Try again.", "Orange")
-                return
-            self.single_task_name = task_name.replace("Task: ", "")
-            self.display_message_box(f"Single Task: {self.single_task_name} selected.", "Green")
-            if self.single_profile_name:
-                self.display_message_box(f"Single Profile '{self.single_profile_name}' ignored.", "Orange")
-                self.single_profile_name = ""
-                self.profile_optionemenu.set("None")
-
-            # Cleanup the buttons
-            self.ai_set_label3.destroy()
-            display_analyze_button(self, 10)
-
-            # Redisplay the ai settings
-            display_ai_settings(self)
-
-        # None was selected
-        else:
-            self.display_message_box("Task selection of 'None' ignored.  Try again.", "Orange")
+        try:
+            changelog = requests.get(CHANGELOG_JSON_URL).json()  # noqa: S113
+        except (json.decoder.JSONDecodeError, ConnectionError, Exception):
+            self.display_message_box("Failed to get changelog.", "Red")
+            return
+        self.clear_messages_event()  # Clear out all displayed messages.
+        # Go through loaded dictionary and display each line
+        for key, value in changelog.items():
+            if "Older History" in value:  # Get out if we hit then of the the new version changes.
+                break
+            if key == "version":
+                self.display_message_box(f"Changes in the new version {value}:", "Green")
+            else:
+                self.display_message_box(f"{value}", "Green")
 
-    # ##################################################################################
-    # Process the '?' Tree View query button
-    # ##################################################################################
-    def ai_help_event(self) -> None:
-        """Function to display help text for the Analysis tab.
-        Parameters:
-            - self (object): The object that the method is being called on.
-        Returns:
-            - None: This method does not return anything.
-        Processing Logic:
-            - Displays help text for Analysis tab.
-            - Uses new_message_box method.
-            - Help text is stored in AI_HELP_TEXT variable."""
-        self.new_message_box("Analyze Help\n\n" + AI_HELP_TEXT)
+        self.display_message_box("End of changelog.", "Green")
```

### Comparing `maptasker-4.0.2/maptasker/src/xmldata.py` & `maptasker-4.0.5/maptasker/src/xmldata.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,29 +155,28 @@
     - Loops through child elements looking for matching "Str" tag
     - Checks if tag attribute matches arg
     - Appends child text to list with argeval prefix
     - Returns first item after processing or empty string
     """
     from maptasker.src.action import drop_trailing_comma
 
-    # TODO Optimize this code to find the argn match
     match_results = []
-    for child in action:
-        if child.tag == "Str":
-            the_arg = child.attrib.get("sr")
-            if arg == the_arg:
-                if child.text is not None:
-                    # Catch the situation in which a newline has been entered for the value (carriage return)
-                    if child.text == "\n":
-                        match_results.append(f"{argeval}(carriage return)")
-                    else:
-                        match_results.append(f"{argeval}{child.text}")
+    all_strings = action.findall("Str")
+    for child in all_strings:
+        the_arg = child.attrib.get("sr")
+        if arg == the_arg:
+            if child.text is not None:
+                # Catch the situation in which a newline has been entered for the value (carriage return)
+                if child.text == "\n":
+                    match_results.append(f"{argeval}(carriage return)")
                 else:
-                    match_results.append("")
-                break  # We have what we want.  Go to next child
+                    match_results.append(f"{argeval}{child.text}")
+            else:
+                match_results.append("")
+            break  # We have what we want.  Go to next child
     if match_results:
         return drop_trailing_comma(match_results)[0]
     return ""
 
 
 # ##################################################################################
 # Given a string, remove all HTML (anything between < >) tags from it
```

### Comparing `maptasker-4.0.2/pyproject.toml` & `maptasker-4.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "maptasker"
 
-version = "4.0.2"
+version = "4.0.5"
 
 description = "Utility to display your entire Android 'Tasker' configuration on your MAC."
 authors = ["Michael Rubin <mikrubin@gmail.com>"]
 readme = "README_PyPl.md"
 license = "MIT License (MIT)"
 repository = "https://github.com/mctinker/Map-Tasker"
 # changelog = "https://github.com/mctinker/Map-Tasker/blob/Master/Changelog.md"
@@ -24,15 +24,15 @@
 ctkcolorpicker = "^0.9.0"  # Color picker in GUI
 pillow = "^10.3.0"  # Image support in GUI
 darkdetect = "^0.8.0"  # Appearance mode detection
 defusedxml = "^0.7.1"  # More secure xml parser
 requests = "^2.31.0"  # HTTP Server function request
 tomli_w = "^1.0.0"  # Write toml file
 cria = "^1.6.5"  #  Ai Ollama support
-openai = "^1.25.1"  #  Ai OpenAi support
+openai = "^1.28.2"  #  Ai OpenAi support
 
 [tool.poetry.scripts]
 maptasker = "maptasker.main:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/mctinker/Map-Tasker/issues"
 "Change Log" = "https://github.com/mctinker/Map-Tasker/CHANGELOG.md"
```

### Comparing `maptasker-4.0.2/PKG-INFO` & `maptasker-4.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maptasker
-Version: 4.0.2
+Version: 4.0.5
 Summary: Utility to display your entire Android 'Tasker' configuration on your MAC.
 Home-page: https://github.com/mctinker/Map-Tasker
 License: MIT License (MIT)
 Keywords: tasker,Tasker,map tasker
 Author: Michael Rubin
 Author-email: mikrubin@gmail.com
 Requires-Python: >=3.11,<=3.13
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cria (>=1.6.5,<2.0.0)
 Requires-Dist: ctkcolorpicker (>=0.9.0,<0.10.0)
 Requires-Dist: customtkinter (>=5.2.2,<6.0.0)
 Requires-Dist: darkdetect (>=0.8.0,<0.9.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: openai (>=1.25.1,<2.0.0)
+Requires-Dist: openai (>=1.28.2,<2.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tomli_w (>=1.0.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/mctinker/Map-Tasker/issues
 Project-URL: Change Log, https://github.com/mctinker/Map-Tasker/CHANGELOG.md
 Project-URL: Repository, https://github.com/mctinker/Map-Tasker
 Description-Content-Type: text/markdown
```

