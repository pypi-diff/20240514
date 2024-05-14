# Comparing `tmp/luma-ml-0.7.5.tar.gz` & `tmp/luma-ml-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.7.5.tar", last modified: Sun May 12 19:40:38 2024, max compression
+gzip compressed data, was "luma-ml-0.8.0.tar", last modified: Tue May 14 16:47:33 2024, max compression
```

## Comparing `luma-ml-0.7.5.tar` & `luma-ml-0.8.0.tar`

### file list

```diff
@@ -1,101 +1,100 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.232830 luma-ml-0.7.5/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.5/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-12 19:40:38.232426 luma-ml-0.7.5/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4946 2024-05-12 19:40:28.000000 luma-ml-0.7.5/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.215067 luma-ml-0.7.5/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)    10872 2024-05-12 19:39:10.000000 luma-ml-0.7.5/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.5/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.216627 luma-ml-0.7.5/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12302 2024-04-27 19:24:30.000000 luma-ml-0.7.5/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7629 2024-04-21 11:35:40.000000 luma-ml-0.7.5/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.7.5/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8953 2024-04-21 11:35:43.000000 luma-ml-0.7.5/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8887 2024-04-21 11:35:41.000000 luma-ml-0.7.5/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9536 2024-04-21 11:35:42.000000 luma-ml-0.7.5/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.217976 luma-ml-0.7.5/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    17291 2024-04-21 11:35:45.000000 luma-ml-0.7.5/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17401 2024-04-21 11:35:47.000000 luma-ml-0.7.5/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7672 2024-04-21 11:35:48.000000 luma-ml-0.7.5/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17695 2024-04-21 11:35:49.000000 luma-ml-0.7.5/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8019 2024-04-21 11:35:50.000000 luma-ml-0.7.5/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11404 2024-04-21 11:35:51.000000 luma-ml-0.7.5/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.218537 luma-ml-0.7.5/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5923 2024-05-08 18:17:58.000000 luma-ml-0.7.5/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      394 2024-04-28 05:47:04.000000 luma-ml-0.7.5/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10856 2024-05-04 18:13:20.000000 luma-ml-0.7.5/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.219503 luma-ml-0.7.5/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)     9749 2024-04-21 11:35:52.000000 luma-ml-0.7.5/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19258 2024-04-21 11:35:53.000000 luma-ml-0.7.5/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9633 2024-04-21 11:35:54.000000 luma-ml-0.7.5/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    13550 2024-04-21 11:35:55.000000 luma-ml-0.7.5/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6513 2024-04-21 11:35:56.000000 luma-ml-0.7.5/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.220122 luma-ml-0.7.5/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.5/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)     4881 2024-04-28 23:46:05.000000 luma-ml-0.7.5/luma/interface/typing.py
--rw-r--r--   0 chanlee    (501) staff       (20)    15102 2024-05-09 18:36:55.000000 luma-ml-0.7.5/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.220873 luma-ml-0.7.5/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.7.5/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5821 2024-04-24 15:56:48.000000 luma-ml-0.7.5/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-04-24 15:55:30.000000 luma-ml-0.7.5/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-04-24 15:57:32.000000 luma-ml-0.7.5/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.221050 luma-ml-0.7.5/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.5/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.221775 luma-ml-0.7.5/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3269 2024-04-21 11:36:03.000000 luma-ml-0.7.5/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7681 2024-04-21 11:36:04.000000 luma-ml-0.7.5/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11846 2024-04-21 11:36:05.000000 luma-ml-0.7.5/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5221 2024-05-06 08:57:35.000000 luma-ml-0.7.5/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.223339 luma-ml-0.7.5/luma/neural/
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.225175 luma-ml-0.7.5/luma/neural/_layers/
--rw-r--r--   0 chanlee    (501) staff       (20)     6748 2024-05-12 09:16:35.000000 luma-ml-0.7.5/luma/neural/_layers/_act.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17921 2024-05-12 08:56:53.000000 luma-ml-0.7.5/luma/neural/_layers/_conv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1108 2024-05-12 09:15:57.000000 luma-ml-0.7.5/luma/neural/_layers/_drop.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2313 2024-05-12 09:17:05.000000 luma-ml-0.7.5/luma/neural/_layers/_linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10640 2024-05-12 19:37:14.000000 luma-ml-0.7.5/luma/neural/_layers/_norm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9291 2024-05-12 09:04:21.000000 luma-ml-0.7.5/luma/neural/_layers/_pool.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.226081 luma-ml-0.7.5/luma/neural/_models/
--rw-r--r--   0 chanlee    (501) staff       (20)    14219 2024-05-12 19:37:23.000000 luma-ml-0.7.5/luma/neural/_models/_imagenet.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12645 2024-05-11 19:57:06.000000 luma-ml-0.7.5/luma/neural/_models/_lenet.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9602 2024-05-12 07:21:21.000000 luma-ml-0.7.5/luma/neural/_models/_simple.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10514 2024-05-11 20:28:21.000000 luma-ml-0.7.5/luma/neural/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)    14447 2024-05-11 20:04:44.000000 luma-ml-0.7.5/luma/neural/block.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.7.5/luma/neural/init.py
--rw-r--r--   0 chanlee    (501) staff       (20)    21528 2024-05-12 19:37:14.000000 luma-ml-0.7.5/luma/neural/layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-04 07:19:22.000000 luma-ml-0.7.5/luma/neural/loss.py
--rw-r--r--   0 chanlee    (501) staff       (20)    23492 2024-05-12 19:40:34.000000 luma-ml-0.7.5/luma/neural/network.py
--rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.7.5/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8210 2024-04-21 11:36:12.000000 luma-ml-0.7.5/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.226269 luma-ml-0.7.5/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7219 2024-04-21 11:36:13.000000 luma-ml-0.7.5/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.227092 luma-ml-0.7.5/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.7.5/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.7.5/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3602 2024-04-21 11:36:16.000000 luma-ml-0.7.5/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2555 2024-04-21 11:36:18.000000 luma-ml-0.7.5/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.227707 luma-ml-0.7.5/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    18479 2024-04-21 11:36:19.000000 luma-ml-0.7.5/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    39141 2024-04-21 11:36:22.000000 luma-ml-0.7.5/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16204 2024-04-21 11:36:23.000000 luma-ml-0.7.5/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.229530 luma-ml-0.7.5/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    19093 2024-04-21 11:36:25.000000 luma-ml-0.7.5/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12211 2024-04-21 11:36:26.000000 luma-ml-0.7.5/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6638 2024-04-21 11:36:27.000000 luma-ml-0.7.5/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2962 2024-04-21 11:36:28.000000 luma-ml-0.7.5/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10680 2024-04-21 11:36:29.000000 luma-ml-0.7.5/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7519 2024-04-21 11:36:30.000000 luma-ml-0.7.5/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7189 2024-04-21 11:36:31.000000 luma-ml-0.7.5/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.229957 luma-ml-0.7.5/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.5/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    24473 2024-04-21 11:36:32.000000 luma-ml-0.7.5/luma/visual/evaluation.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.231404 luma-ml-0.7.5/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-12 19:40:38.000000 luma-ml-0.7.5/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     1966 2024-05-12 19:40:38.000000 luma-ml-0.7.5/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-12 19:40:38.000000 luma-ml-0.7.5/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-12 19:40:38.000000 luma-ml-0.7.5/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-12 19:40:38.000000 luma-ml-0.7.5/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-12 19:40:38.232913 luma-ml-0.7.5/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-12 19:40:33.000000 luma-ml-0.7.5/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.231960 luma-ml-0.7.5/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.7.5/test/__act.py
--rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-04-20 19:16:53.000000 luma-ml-0.7.5/test/__local__.py
--rw-r--r--   0 chanlee    (501) staff       (20)      516 2024-05-12 19:25:07.000000 luma-ml-0.7.5/test/__test.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.180191 luma-ml-0.8.0/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.8.0/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-14 16:47:33.179664 luma-ml-0.8.0/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4946 2024-05-14 16:40:36.000000 luma-ml-0.8.0/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.126357 luma-ml-0.8.0/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10872 2024-05-12 19:39:10.000000 luma-ml-0.8.0/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.8.0/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.133221 luma-ml-0.8.0/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12563 2024-05-13 11:38:17.000000 luma-ml-0.8.0/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7935 2024-05-13 11:35:13.000000 luma-ml-0.8.0/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.8.0/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9070 2024-05-13 11:30:20.000000 luma-ml-0.8.0/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9174 2024-05-13 11:33:07.000000 luma-ml-0.8.0/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9806 2024-05-13 11:36:04.000000 luma-ml-0.8.0/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.142844 luma-ml-0.8.0/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18057 2024-05-13 11:42:50.000000 luma-ml-0.8.0/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17889 2024-05-13 11:50:11.000000 luma-ml-0.8.0/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7697 2024-05-13 11:51:42.000000 luma-ml-0.8.0/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    18307 2024-05-13 11:55:03.000000 luma-ml-0.8.0/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8192 2024-05-13 11:55:57.000000 luma-ml-0.8.0/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11602 2024-05-13 11:57:37.000000 luma-ml-0.8.0/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.144920 luma-ml-0.8.0/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5924 2024-05-13 11:58:02.000000 luma-ml-0.8.0/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      446 2024-05-13 11:58:51.000000 luma-ml-0.8.0/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11013 2024-05-13 12:05:21.000000 luma-ml-0.8.0/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.148692 luma-ml-0.8.0/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10046 2024-05-13 12:09:42.000000 luma-ml-0.8.0/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19721 2024-05-13 12:15:52.000000 luma-ml-0.8.0/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10280 2024-05-13 12:20:38.000000 luma-ml-0.8.0/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    14109 2024-05-13 12:31:18.000000 luma-ml-0.8.0/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6779 2024-05-13 12:36:00.000000 luma-ml-0.8.0/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.150594 luma-ml-0.8.0/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-05-13 12:36:06.000000 luma-ml-0.8.0/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     4885 2024-05-13 12:44:14.000000 luma-ml-0.8.0/luma/interface/typing.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16195 2024-05-13 15:45:21.000000 luma-ml-0.8.0/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.152982 luma-ml-0.8.0/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.8.0/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5917 2024-05-13 15:46:55.000000 luma-ml-0.8.0/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-05-13 15:46:57.000000 luma-ml-0.8.0/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-05-13 15:46:59.000000 luma-ml-0.8.0/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.153317 luma-ml-0.8.0/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3764 2024-05-13 16:18:47.000000 luma-ml-0.8.0/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.155579 luma-ml-0.8.0/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3438 2024-05-13 16:20:58.000000 luma-ml-0.8.0/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8041 2024-05-13 16:29:29.000000 luma-ml-0.8.0/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12244 2024-05-13 16:35:00.000000 luma-ml-0.8.0/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5736 2024-05-13 16:40:23.000000 luma-ml-0.8.0/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.159938 luma-ml-0.8.0/luma/neural/
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.162910 luma-ml-0.8.0/luma/neural/_layers/
+-rw-r--r--   0 chanlee    (501) staff       (20)     6748 2024-05-12 09:16:35.000000 luma-ml-0.8.0/luma/neural/_layers/_act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17921 2024-05-12 08:56:53.000000 luma-ml-0.8.0/luma/neural/_layers/_conv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1108 2024-05-12 09:15:57.000000 luma-ml-0.8.0/luma/neural/_layers/_drop.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2313 2024-05-12 09:17:05.000000 luma-ml-0.8.0/luma/neural/_layers/_linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10640 2024-05-12 19:37:14.000000 luma-ml-0.8.0/luma/neural/_layers/_norm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9291 2024-05-12 09:04:21.000000 luma-ml-0.8.0/luma/neural/_layers/_pool.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.164149 luma-ml-0.8.0/luma/neural/_models/
+-rw-r--r--   0 chanlee    (501) staff       (20)    14219 2024-05-12 19:37:23.000000 luma-ml-0.8.0/luma/neural/_models/_imagenet.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12645 2024-05-11 19:57:06.000000 luma-ml-0.8.0/luma/neural/_models/_lenet.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9602 2024-05-12 07:21:21.000000 luma-ml-0.8.0/luma/neural/_models/_simple.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12024 2024-05-13 17:00:56.000000 luma-ml-0.8.0/luma/neural/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    15726 2024-05-13 17:44:43.000000 luma-ml-0.8.0/luma/neural/block.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.8.0/luma/neural/init.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    22917 2024-05-13 19:10:14.000000 luma-ml-0.8.0/luma/neural/layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-13 19:10:16.000000 luma-ml-0.8.0/luma/neural/loss.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    25998 2024-05-13 19:25:58.000000 luma-ml-0.8.0/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.8.0/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8582 2024-05-13 19:27:55.000000 luma-ml-0.8.0/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.164395 luma-ml-0.8.0/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7308 2024-05-13 19:32:18.000000 luma-ml-0.8.0/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.167026 luma-ml-0.8.0/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.8.0/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.8.0/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3653 2024-05-13 19:32:35.000000 luma-ml-0.8.0/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2624 2024-05-13 19:33:29.000000 luma-ml-0.8.0/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.169823 luma-ml-0.8.0/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19132 2024-05-13 19:40:06.000000 luma-ml-0.8.0/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    40387 2024-05-13 19:55:48.000000 luma-ml-0.8.0/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17019 2024-05-14 09:45:27.000000 luma-ml-0.8.0/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.175673 luma-ml-0.8.0/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19882 2024-05-14 09:56:22.000000 luma-ml-0.8.0/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12687 2024-05-14 10:03:42.000000 luma-ml-0.8.0/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6755 2024-05-14 10:04:13.000000 luma-ml-0.8.0/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3098 2024-05-14 10:05:44.000000 luma-ml-0.8.0/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11070 2024-05-14 14:33:09.000000 luma-ml-0.8.0/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7805 2024-05-14 14:45:46.000000 luma-ml-0.8.0/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7415 2024-05-14 14:59:17.000000 luma-ml-0.8.0/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.176714 luma-ml-0.8.0/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.8.0/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    25027 2024-05-14 16:39:15.000000 luma-ml-0.8.0/luma/visual/evaluation.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.178430 luma-ml-0.8.0/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-14 16:47:33.000000 luma-ml-0.8.0/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     1948 2024-05-14 16:47:33.000000 luma-ml-0.8.0/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-14 16:47:33.000000 luma-ml-0.8.0/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-14 16:47:33.000000 luma-ml-0.8.0/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-14 16:47:33.000000 luma-ml-0.8.0/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-14 16:47:33.180270 luma-ml-0.8.0/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-14 16:47:29.000000 luma-ml-0.8.0/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.178977 luma-ml-0.8.0/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.8.0/test/__act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      499 2024-05-14 15:56:10.000000 luma-ml-0.8.0/test/__test.py
```

### Comparing `luma-ml-0.7.5/LICENSE` & `luma-ml-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/PKG-INFO` & `luma-ml-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.5
+Version: 0.8.0
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.50k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.56k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.5</td>
+                    <td>0.8.0</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~21K</td>
+                    <td>~22K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.5 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.8.0 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.50k-red][GitHub code size in bytes][Code Style]
+5.56k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.5
-Lines of Code  ~21K
+Latest Version 0.8.0
+Lines of Code  ~22K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.5/README.md` & `luma-ml-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.50k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.56k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -89,19 +89,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.5</td>
+                    <td>0.8.0</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~21K</td>
+                    <td>~22K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.50k-red][GitHub code size in bytes][Code Style]
+5.56k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.5
-Lines of Code  ~21K
+Latest Version 0.8.0
+Lines of Code  ~22K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.5/luma/__import__.py` & `luma-ml-0.8.0/luma/__import__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/__init__.py` & `luma-ml-0.8.0/luma/__init__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/classifier/discriminant.py` & `luma-ml-0.8.0/luma/classifier/discriminant.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,18 +166,20 @@
     enhancing classification performance. RDA is particularly effective in
     scenarios with high-dimensional data or when the number of samples is
     limited. The method employs regularization parameters to balance bias
     and variance, aiming to optimize model accuracy.
 
     Parameters
     ----------
-    `alpha` : Balancing parameter between the class-specific covariance matrices
-    (0 for LDA-like, 1 for QDA-like approach)
-    `gamma` : Shrinkage applied to the covariance matrices
-    (0 for large shrinkage, i.e. max regularization)
+    `alpha` : float, default=0.5
+        Balancing parameter between the class-specific covariance matrices
+        (0 for LDA-like, 1 for QDA-like approach)
+    `gamma` : float, default=0.5
+        Shrinkage applied to the covariance matrices
+        (0 for large shrinkage, i.e. max regularization)
 
     """
 
     def __init__(self, alpha: float = 0.5, gamma: float = 0.5) -> None:
         self.alpha = alpha
         self.gamma = gamma
         self.classes = None
@@ -271,31 +273,35 @@
     separable. The KDA classifier operates by projecting input data into
     a space where classes are maximally distant from each other, using
     the calculated projections to classify new instances based on their
     proximity to class centroids.
 
     Parameters
     ----------
-    `deg` : Polynomial degree of `poly` kernel
-    `gamma` : Shape parameter of `rbf`, `sigmoid`, `laplacian`
-    `coef` : Additional coefficient of `poly`, `sigmoid`
-    `kernel` : Type of kernel functions
+    `deg` : int, default=2
+        Polynomial degree of polynomial kernel
+    `gamma` : float, default=1.0
+        Shape parameter of RBF, sigmoid, laplacian kernels
+    `coef` : float, default=0.0
+        Additional coefficient of polynomial and sigmoid kernels
+    `kernel` : FuncType, default="rbf"
+        Type of kernel functions
 
     Notes
     -----
     * To use KDA for dimensionality reduction, refer to
         `luma.reduction.linear.KDA`
 
     """
 
     def __init__(
         self,
         deg: int = 2,
         gamma: float = 1.0,
-        coef: int = 0.0,
+        coef: float = 0.0,
         kernel: KernelUtil.FuncType = "rbf",
     ) -> None:
         self.deg = deg
         self.gamma = gamma
         self.coef = coef
         self.kernel = kernel
         self.X_ = None
@@ -304,15 +310,20 @@
         self.kernel_params = {
             "deg": self.deg,
             "alpha": self.alpha,
             "gamma": self.gamma,
             "coef": self.coef,
         }
 
-        self.set_param_ranges({"deg": ("0,+inf", int), "gamma": ("0<,+inf", None)})
+        self.set_param_ranges(
+            {
+                "deg": ("0,+inf", int),
+                "gamma": ("0<,+inf", None),
+            }
+        )
         self.check_param_ranges()
 
     def fit(self, X: Matrix, y: Vector) -> Self:
         m, _ = X.shape
         self._X = X
         self.classes = np.unique(y)
         self.n_classes = len(self.classes)
```

### Comparing `luma-ml-0.7.5/luma/classifier/logistic.py` & `luma-ml-0.8.0/luma/classifier/logistic.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,29 +15,34 @@
     Logistic regression is a statistical model used for binary classification,
     which means it's employed to predict one of two possible outcomes.
     It does this by modeling the relationship between one or more
     input variables and the probability of the binary outcome.
 
     Parameters
     ----------
-    `learning_rate` : Step size of the gradient descent update
-    `max_iter` : Number of iteration
-    `l1_ratio` : Balancing parameter of `elastic-net`
-    `alpha` : Regularization strength
-    `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
+    `learning_rate` : float, default=0.01
+        Step size of the gradient descent update
+    `max_iter` : int, default=100
+        Number of iteration
+    `l1_ratio` : float, default=0.5, range=[0,1]
+        Balancing parameter of elastic-net
+    `alpha` : float, default=0.01
+        Regularization strength
+    `regularization` : {"l1", "l2", "elastic-net"}, optional, default=None
+        Regularization type
 
     """
 
     def __init__(
         self,
         learning_rate: float = 0.01,
         max_iter: int = 100,
         l1_ratio: float = 0.5,
         alpha: float = 0.01,
-        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        regularization: Literal["l1", "l2", "elastic-net"] | None = None,
         verbose: bool = False,
     ):
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.l1_ratio = l1_ratio
         self.regularization = regularization
         self.alpha = alpha
@@ -116,29 +121,34 @@
     Softmax regression, also known as multinomial logistic regression,
     is a supervised machine learning technique used for classification tasks.
     It's an extension of logistic regression,
     but it can handle multiple classes (more than two).
 
     Parameters
     ----------
-    `learning_rate` : Step size of the gradient descent update
-    `max_iter` : Number of iteration
-    `l1_ratio` : Balancing parameter of `elastic-net`
-    `alpha` : Regularization strength
-    `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
+    `learning_rate` : float, default=0.01
+        Step size of the gradient descent update
+    `max_iter` : int, default=100
+        Number of iteration
+    `l1_ratio` : float, default=0.5, range=[0,1]
+        Balancing parameter of elastic-net
+    `alpha` : float, default=0.01
+        Regularization strength
+    `regularization` : {"l1", "l2", "elastic-net"}, optional, default=None
+        Regularization type
 
     """
 
     def __init__(
         self,
         learning_rate: float = 0.01,
         max_iter: int = 100,
         l1_ratio: float = 0.5,
         alpha: float = 0.01,
-        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        regularization: Literal["l1", "l2", "elastic-net"] | None = None,
         verbose: bool = False,
     ) -> None:
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.l1_ratio = l1_ratio
         self.alpha = alpha
         self.regularization = regularization
```

### Comparing `luma-ml-0.7.5/luma/classifier/naive_bayes.py` & `luma-ml-0.8.0/luma/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/classifier/neighbors.py` & `luma-ml-0.8.0/luma/classifier/neighbors.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     calculating the distance (such as Euclidean distance) between the
     new point and all points in the training set, identifying the 'k'
     nearest neighbors, and then performing a majority vote among these
     neighbors to determine the class label.
 
     Parameters
     ----------
-    `n_neighbors` : Number of neighbors to be considered close
+    `n_neighbors` : int, default=5
+        Number of neighbors to be considered close
 
     """
 
     def __init__(self, n_neighbors: int = 5):
         self.n_neighbors = n_neighbors
         self._neighbors = None
         self._y = None
@@ -90,17 +91,20 @@
     the number of neighbors (k) is adaptively determined based on the local
     density of the training data. This adaptive approach allows the algorithm
     to be more flexible and effective, especially in datasets with varying
     densities.
 
     Parameters
     ----------
-    `n_density` : Number of nearest neighbors to estimate the local density
-    `min_neighbors` : Minimum number of neighbors to be considered for averaging
-    `max_neighbors` : Maximum number of neighbors to be considered
+    `n_density` : int, default=10
+        Number of nearest neighbors to estimate the local density
+    `min_neighbors` : int, default=5
+        Minimum number of neighbors to be considered for averaging
+    `max_neighbors` : int, default=20
+        Maximum number of neighbors to be considered
 
     """
 
     def __init__(
         self, n_density: int = 10, min_neighbors: int = 5, max_neighbors: int = 20
     ):
         self.n_density = n_density
@@ -187,15 +191,16 @@
     where neighbors contribute to the classification decision based on their distance
     from the query point. Closer neighbors have more influence as they are assigned
     higher weights, typically using inverse distance weighting. This approach enhances
     prediction accuracy, especially in unevenly distributed datasets.
 
     Parameters
     ----------
-    `n_neighbors` : Number of neighbors to be considered close
+    `n_neighbors` : int, default=5
+        Number of neighbors to be considered close
 
     """
 
     def __init__(self, n_neighbors: int = 5):
         self.n_neighbors = n_neighbors
         self._X = None
         self._y = None
```

### Comparing `luma-ml-0.7.5/luma/classifier/svm.py` & `luma-ml-0.8.0/luma/classifier/svm.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,22 @@
     algorithm mainly used for classification tasks. It operates by
     determining a hyperplane that best separates different classes in
     the input data, aiming to maximize the margin between the hyperplane
     and the nearest data points from each class.
 
     Parameters
     ----------
-    `C` : Regularization parameter
-    `batch_size` : Size of a single batch
-    `learning_rate` : Step-size of gradient descent update
-    `max_iter` : Number of iteration
+    `C` : float, default=1.0
+        Regularization parameter
+    `batch_size` : int, default=100
+        Size of a single batch
+    `learning_rate` : float, default=0.001
+        Step-size of gradient descent update
+    `max_iter` : int, default=1000
+        Number of iteration
 
     """
 
     def __init__(
         self,
         C: float = 1.0,
         batch_size: int = 100,
@@ -115,22 +119,30 @@
     """
     Kernel Support Vector Classification (SVC) with batch-based learning.
     This approach processes the training data in batches, making it suitable
     for large datasets that cannot fit into memory at once.
 
     Parameters
     ----------
-    `C` : Regularization parameter
-    `deg` : Polynomial Degree for `poly` kernel
-    `gamma` : Shape parameter of Gaussian curve for `rbf` kernel
-    `coef` : Coefficient for `poly`, `sigmoid` kernel
-    `learning_rate` : Step-size for gradient descent update
-    `max_iter` : Number of iteration
-    `batch_size`: Size of the batch for batch-based learning
-    `kernel` : Type of kernel (e.g., `linear`, `poly`, `rbf`, `sigmoid`)
+    `C` : float, default=1.0
+        Regularization parameter
+    `deg` : int, default=3
+        Polynomial Degree for polynomial kernel
+    `gamma` : float, default=0.0
+        Shape parameter of Gaussian curve for RBF kernel
+    `coef` : float, default=1.0
+        Coefficient for polynomial and sigmoid kernel
+    `learning_rate` : float, default=0.001
+        Step-size for gradient descent update
+    `max_iter` : int, default=1000
+        Number of iteration
+    `batch_size`: int, default=100
+        Size of the batch for batch-based learning
+    `kernel` : FuncType, default="rbf"
+        Type of kernel
 
     """
 
     def __init__(
         self,
         C: float = 1.0,
         deg: int = 3,
```

### Comparing `luma-ml-0.7.5/luma/classifier/tree.py` & `luma-ml-0.8.0/luma/classifier/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,35 +20,43 @@
     branch. The process continues recursively until it reaches a
     leaf node, where the final decision or classification is made.
     This model is intuitive and can easily handle categorical and
     numerical data.
 
     Parameters
     ----------
-    `max_depth` : Maximum depth of the tree
-    `criterion` : Function used to measure the quality of a split
-    `min_samples_split` : Minimum samples required to split a node
-    `min_samples_leaf` : Minimum samples required to be at a leaf node
-    `max_features` : Number of features to consider
-    `min_impurity_decrease` : Minimum decrement of impurity for a split
-    `max_leaf_nodes` : Maximum amount of leaf nodes
-    `random_state` : The randomness seed of the estimator
+    `max_depth` : int, default=10
+        Maximum depth of the tree
+    `criterion` : {"gini", "entropy"}, default="gini"
+        Function used to measure the quality of a split
+    `min_samples_split` : int, default=2
+        Minimum samples required to split a node
+    `min_samples_leaf` : int, default=1
+        Minimum samples required to be at a leaf node
+    `max_features` : int, optional, default=None
+        Number of features to consider
+    `min_impurity_decrease` : float, default=0.0
+        Minimum decrement of impurity for a split
+    `max_leaf_nodes` : int, optional, default=None
+        Maximum amount of leaf nodes
+    `random_state` : int, optional, default=None
+        The randomness seed of the estimator
 
     """
 
     def __init__(
         self,
         max_depth: int = 10,
         criterion: Literal["gini", "entropy"] = "gini",
         min_samples_split: int = 2,
         min_samples_leaf: int = 1,
-        max_features: int = None,
+        max_features: int | None = None,
         min_impurity_decrease: float = 0.0,
-        max_leaf_nodes: int = None,
-        random_state: int = None,
+        max_leaf_nodes: int | None = None,
+        random_state: int | None = None,
     ) -> None:
         self.max_depth = max_depth
         self.criterion = criterion
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.max_features = max_features
         self.min_impurity_decrease = min_impurity_decrease
```

### Comparing `luma-ml-0.7.5/luma/clustering/affinity.py` & `luma-ml-0.8.0/luma/clustering/affinity.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,43 +23,49 @@
     and corresponding clusters emerges. The algorithm doesn't require the
     number of clusters to be specified in advance. Affinity Propagation is
     particularly useful for problems where the optimal number of clusters
     is unknown or hard to estimate.
 
     Parameters
     ----------
-    `max_iter` : Maximum iterations for message exchange
-    `damping` : Balancing factor for ensuring numerical stability and convergence
-    `tol` : Early-stopping threshold
-    `preference` : Parameter which determines the selectivity of choosing exemplars
-
-    * Self-Similarity Setting:
+    `max_iter` : int, default=100
+        Maximum iterations for message exchange
+    `damping` : float, default=0.7
+        Balancing factor for ensuring numerical stability and convergence
+    `preference` : Scalar or Vector or {"median", "min"}, default="median"
+        Parameter which determines the selectivity of choosing exemplars
+    `tol` : float, optional, default=None
+        Early-stopping threshold
+
+    Notes
+    -----
+    - Self-Similarity Setting:
         The preference value represents the "self-similarity" of each data point.
         It is the value on the diagonal of the similarity matrix, which influences
         how likely a data point is to be chosen as an exemplar (a cluster center).
 
-    * Influencing Cluster Count:
+    - Influencing Cluster Count:
         A higher preference value suggests a greater likelihood for a data point to
         become an exemplar, potentially leading to more clusters. Conversely, a lower
         preference value tends to produce fewer clusters, as fewer points are strong
         candidates for being exemplars.
 
-    * Default Setting:
+    - Default Setting:
         If not explicitly set, the preference is often chosen automatically based on
         the input data. Common practices include setting it to the median or mean of
         the similarity values.
 
     """
 
     def __init__(
         self,
         max_iter: int = 100,
         damping: float = 0.7,
         preference: Scalar | Vector | Literal["median", "min"] = "median",
-        tol: float = None,
+        tol: float | None = None,
         verbose: bool = False,
     ) -> None:
         self.max_iter = max_iter
         self.damping = damping
         self.preference = preference
         self.tol = tol
         self.verbose = verbose
@@ -186,30 +192,38 @@
     an appropriate number of clusters, especially in complex or ambiguous
     datasets. This approach enhances the standard Affinity Propagation
     algorithm by offering potentially improved clustering accuracy
     and adaptability.
 
     Parameters
     ----------
-    `max_iter` : Maximum iterations for message exchange
-    `damping` : Balancing factor for ensuring numerical stability and convergence
-    `tol` : Early-stopping threshold
-    `lambda_param` : Preference updating factor
-    `preference` : Parameter which determines the selectivity of choosing exemplars
-    (more details in `AffinityPropagation`)
+    `max_iter` : int, default=100
+        Maximum iterations for message exchange
+    `damping` : float, default=0.7
+        Balancing factor for ensuring numerical stability and convergence
+    `preference` : Scalar or Vector or {"median", "min"}, default="median"
+        Parameter which determines the selectivity of choosing exemplars
+    `lambda_param` : float, default=0.5
+        Preference updating factor
+    `tol` : float, optional, default=None
+        Early-stopping threshold
+
+    See Also
+    --------
+    For more detailed explanation of `preference`, refer to `AffinityPropagation`.
 
     """
 
     def __init__(
         self,
         max_iter: int = 100,
         damping: float = 0.7,
         preference: Scalar | Vector | Literal["median", "min"] = "median",
         lambda_param: float = 0.5,
-        tol: float = None,
+        tol: float | None = None,
         verbose: bool = False,
     ) -> None:
         self.max_iter = max_iter
         self.damping = damping
         self.preference = preference
         self.tol = tol
         self.lambda_param = lambda_param
@@ -350,29 +364,39 @@
     clustering of complex, non-linear datasets. This approach enhances
     the standard Affinity Propagation by uncovering intricate cluster
     structures in transformed feature spaces, suitable for non-linearly
     separable data.
 
     Parameters
     ----------
-    `max_iter` : Maximum iterations for message exchange
-    `damping` : Balancing factor for ensuring numerical stability and convergence
-    `preference` : Parameter which determines the selectivity of choosing exemplars
-    `tol` : Early-stopping threshold
-    `kernel`: Kernel method (`rbf`, `sigmoid`, `laplacian` are supported)
-    `gamma` : Scaling factor for kernel function
+    `max_iter` : int, default=1000
+        Maximum iterations for message exchange
+    `damping` : float, default=0.7
+        Balancing factor for ensuring numerical stability and convergence
+    `preference` : Scalar or Vector or {"median", "min"}, default="median"
+        Parameter which determines the selectivity of choosing exemplars
+    `tol` : float, optional, default=None
+        Early-stopping threshold
+    `kernel`: FuncType, default="rbf"
+        Kernel method (`rbf`, `sigmoid`, `laplacian` are supported)
+    `gamma` : float, default=1.0
+        Scaling factor for kernel function
+
+    See Also
+    --------
+    For more detailed explanation of `preference`, refer to `AffinityPropagation`.
 
     """
 
     def __init__(
         self,
         max_iter: int = 100,
         damping: float = 0.7,
         preference: Scalar | Vector | Literal["median", "min"] = "median",
-        tol: float = None,
+        tol: float | None = None,
         kernel: KernelUtil.FuncType = "rbf",
         gamma: float = 1.0,
         verbose: bool = False,
     ) -> None:
         self.max_iter = max_iter
         self.damping = damping
         self.preference = preference
```

### Comparing `luma-ml-0.7.5/luma/clustering/density.py` & `luma-ml-0.8.0/luma/clustering/density.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,20 @@
     by their proximity and density. It identifies clusters as areas of high
     point density, separated by regions of low density. Points in sparse
     regions are classified as noise. DBSCAN is particularly effective at
     discovering clusters of arbitrary shapes and dealing with outliers.
 
     Parameters
     ----------
-    `epsilon` : Radius of a neighborhood hypersphere
-    `min_points` : Minimum required points to form a cluster
+    `epsilon` : float, default=0.1
+        Radius of a neighborhood hypersphere
+    `min_points` : int, default=5
+        Minimum required points to form a cluster
+    `metric` : {"euclidean", "minkowski"}, default="euclidean"
+        Distance metric for radius measurement
 
     """
 
     def __init__(
         self,
         epsilon: float = 0.1,
         min_points: int = 5,
@@ -126,17 +130,20 @@
     doesn't require a global density threshold, making it versatile
     for complex datasets. The result is often visualized as a
     reachability plot, revealing the data's clustering hierarchy and
     density variations.
 
     Parameters
     ----------
-    `epsilon` : Radius of neighborhood hypersphere
-    `min_points` : Minimum nuber of points to form a cluster
-    `threshold` : Threshold for filtering samples with large reachabilities
+    `epsilon` : float, default=1.0
+        Radius of neighborhood hypersphere
+    `min_points` : int, default=5
+        Minimum nuber of points to form a cluster
+    `threshold` : float, default=1.5
+        Threshold for filtering samples with large reachabilities
 
     """
 
     def __init__(
         self,
         epsilon: float = 1.0,
         min_points: int = 5,
@@ -281,36 +288,41 @@
     functions, typically Gaussian kernels, to estimate data density.
     Cluster centers are determined by the peaks of these density functions.
     The algorithm excels in handling clusters of arbitrary shapes and noise,
     but is sensitive to parameter settings.
 
     Parameters
     ----------
-    `h` : Smoothing parameter of local density estimation
-    `tol` : Threshold for early convergence
-    `max_climb` : Maximum number of climbing process for finding local maxima
-    `min_density` : Minimum local densities to be considered
-    `sample_weight` : Custom individual weights for sample data
+    `h` : float or {"auto"}, default="auto"
+        Smoothing parameter of local density estimation
+    `tol` : float, default=1e-3
+        Threshold for early convergence
+    `max_climb` : int, default=100
+        Maximum number of climbing process for finding local maxima
+    `min_density` : float, default=0.0
+        Minimum local densities to be considered
+    `sample_weight` : Vector, optional, default=None
+        Custom individual weights for sample data
 
     Reference
     ---------
-    Hinneburg, A., & Gabriel, H. H. (2007, September). Denclue 2.0: Fast
+    1. Hinneburg, A., & Gabriel, H. H. (2007, September). Denclue 2.0: Fast
     clustering based on kernel density estimation. In International symposium
     on intelligent data analysis (pp. 70-80). Berlin, Heidelberg: Springer
     Berlin Heidelberg.
 
     """
 
     def __init__(
         self,
         h: float | Literal["auto"] = "auto",
         tol: float = 1e-3,
         max_climb: int = 100,
         min_density: float = 0.0,
-        sample_weight: Vector = None,
+        sample_weight: Vector | None = None,
     ) -> None:
         self.h = h
         self.tol = tol
         self.max_climb = max_climb
         self.min_density = min_density
         self.sample_weight = sample_weight
         self._X = None
@@ -448,17 +460,20 @@
     The process repeats until convergence, where centers no longer
     significantly shift. It automatically determines the number of
     clusters based on the data distribution. Mean Shift is especially
     effective in discovering clusters of arbitrary shapes and sizes.
 
     Parameters
     ----------
-    `bandwidth` : Window size for kernel density estimation
-    `max_iter` : Maximum iteration
-    `tol` : Tolerence threshold for early convergence
+    `bandwidth` : float, default=2.0
+        Window size for kernel density estimation
+    `max_iter` : int, default=300
+        Maximum iteration
+    `tol` : float, default=1e-3
+        Tolerence threshold for early convergence
 
     """
 
     def __init__(
         self,
         bandwidth: float = 2.0,
         max_iter: int = 300,
```

### Comparing `luma-ml-0.7.5/luma/clustering/hierarchy.py` & `luma-ml-0.8.0/luma/clustering/hierarchy.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,29 @@
     by treating each data point as a single cluster. It iteratively merges the
     closest pairs of clusters based on a chosen distance metric. This process
     continues until a specified number of clusters is reached or all points
     are merged into a single cluster.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters to estimate
-    `linkage` : Linkage method (e.g. `single`, `complete`, `average`, `ward`)
+    `n_clusters` : int, default=2
+        Number of clusters to estimate
+    `linkage` : {"single", "complete", "average"}, default="single"
+        Linkage method
 
     Methods
     -------
     Plot hierarchical dendrogram:
     ```py
-    def plot_dendrogram(self,
-                        ax: Optional[plt.Axes] = None,
-                        hide_indices: bool = True,
-                        show: bool = False) -> plt.Axes
+    def plot_dendrogram(
+        self,
+        ax: Optional[plt.Axes] = None,
+        hide_indices: bool = True,
+        show: bool = False
+    ) -> plt.Axes
     ```
     Examples
     --------
     >>> agg = AgglomerativeClustering()
     >>> agg.fit(X, y)
     >>> lables = agg.labels # Get assigned labels
 
@@ -168,15 +172,16 @@
     algorithms like K-means for splitting. The process continues until a
     specified number of clusters is reached or other stopping criteria are met.
     This method is particularly effective for datasets with well-defined,
     separate clusters.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters to estimate
+    `n_clusters` : int, default=2
+        Number of clusters to estimate
 
     Examples
     --------
     >>> div = DivisiveClustering()
     >>> div.fit(X)
     >>> labels = div.labels # Get assigned labels
```

### Comparing `luma-ml-0.7.5/luma/clustering/kmeans.py` & `luma-ml-0.8.0/luma/clustering/kmeans.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,26 @@
     points into clusters. It works by iteratively assigning data points to the
     nearest cluster center (centroid) and updating the centroids based on
     the assigned data points. This process continues
     until convergence.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters
-    `max_iter` : Number of iteration
+    `n_clusters` : int, optional, default=None
+        Number of clusters
+    `max_iter` : int, default=100
+        Number of iteration
 
     """
 
     def __init__(
-        self, n_clusters: int = None, max_iter: int = 100, verbose: bool = False
+        self,
+        n_clusters: int | None = None,
+        max_iter: int = 100,
+        verbose: bool = False,
     ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.verbose = verbose
         self._X = None
         self._fitted = False
 
@@ -97,21 +102,26 @@
     designed to address some of its shortcomings and produce more robust and
     efficient clustering results. K-means++ was introduced by David Arthur and
     Sergei Vassilvitskii in a 2007 research paper titled "k-means++:
     The Advantages of Careful Seeding."
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters
-    `max_iter` : Number of iteration
+    `n_clusters` : int, optional, default=None
+        Number of clusters
+    `max_iter` : int, default=100
+        Number of iteration
 
     """
 
     def __init__(
-        self, n_clusters: int = None, max_iter: int = 100, verbose: bool = False
+        self,
+        n_clusters: int | None = None,
+        max_iter: int = 100,
+        verbose: bool = False,
     ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.verbose = verbose
         self._X = None
         self._fitted = False
 
@@ -175,21 +185,26 @@
     K clusters with each cluster having a median point as its representative.
     It uses distance metrics like Manhattan or Euclidean distance to minimize
     the sum of distances between data points and their cluster medians,
     making it less sensitive to outliers and adaptable to non-Euclidean data.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters
-    `max_iter` : Number of iteration
+    `n_clusters` : int, optional, default=None
+        Number of clusters
+    `max_iter` : int, default=100
+        Number of iteration
 
     """
 
     def __init__(
-        self, n_clusters: int = None, max_iter: int = 100, verbose: bool = False
+        self,
+        n_clusters: int | None = None,
+        max_iter: int = 100,
+        verbose: bool = False,
     ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.verbose = verbose
         self._X = None
         self._fitted = False
 
@@ -250,25 +265,28 @@
     point designated as the medoid of that cluster. During each iteration, it
     reassigns points to the closest medoid and updates medoids based on the
     current cluster assignments. K-Medoids is more robust to noise and outliers
     compared to K-Means.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters to estimate
-    `max_iter` : Maximum iteration for PAM (Partitioning Around Medoids) algorithm
-    `random_state` : Seed for randomized initialization of medoids
+    `n_clusters` : int
+        Number of clusters to estimate
+    `max_iter` : int, default=300
+        Maximum iteration for PAM (Partitioning Around Medoids) algorithm
+    `random_state` : int, optional, default=None
+        Seed for randomized initialization of medoids
 
     """
 
     def __init__(
         self,
         n_clusters: int,
         max_iter: int = 300,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.random_state = random_state
         self.medoids = None
         self.verbose = verbose
@@ -340,22 +358,28 @@
     and using these subsets, rather than the entire dataset, to update the
     cluster centroids in each iteration. This approach significantly reduces
     the computational cost and memory requirements, making it well-suited
     for big data applications.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters to estimate
-    `batch_size` : Size of a single mini-batch
-    `max_iter` : Maximum amount of iteration
+    `n_clusters` : int, optional, default=None
+        Number of clusters to estimate
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `max_iter` : int, default=100
+        Maximum amount of iteration
 
     """
 
     def __init__(
-        self, n_clusters: int = None, batch_size: int = 100, max_iter: int = 100
+        self,
+        n_clusters: int | None = None,
+        batch_size: int = 100,
+        max_iter: int = 100,
     ) -> None:
         self.n_clusters = n_clusters
         self.batch_size = batch_size
         self.max_iter = max_iter
         self.centroids = None
         self._X = None
         self._fitted = False
@@ -414,29 +438,34 @@
     distance of points to centroids, weighted by their membership. The
     algorithm is suitable for data with overlapping or unclear boundaries
     between clusters. FKM provides a soft partitioning of the data, allowing
     more flexible cluster assignments compared to hard clustering methods.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters to estimate
-    `max_iter` : Maximum iteration
-    `m`: Fuzziness parameter (larger makes labels softer)
-    `tol` : Threshold for early convergence
-    `random_state` : Seed for randomized initialization of centers
+    `n_clusters` : int
+        Number of clusters to estimate
+    `max_iter` : int, default=100
+        Maximum iteration
+    `m`: float, default=2.0
+        Fuzziness parameter (larger makes labels softer)
+    `tol` : float, default=1e-5
+        Threshold for early convergence
+    `random_state` : int, optional, default=None
+        Seed for randomized initialization of centers
 
     """
 
     def __init__(
         self,
         n_clusters: int,
         max_iter: int = 100,
         m: float = 2.0,
         tol: float = 1e-5,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.m = m
         self.tol = tol
         self.random_state = random_state
```

### Comparing `luma-ml-0.7.5/luma/clustering/mixture.py` & `luma-ml-0.8.0/luma/clustering/mixture.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,27 +17,31 @@
     used in clustering by assuming each cluster follows a different Gaussian
     distribution. GMM provides soft clustering, assigning probabilities to
     each data point for belonging to each cluster. The model parameters are
     estimated using the Expectation-Maximization algorithm.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters to estimate
-    `max_iter` : Maximum amount of iteration
-    `tol` : Tolerance for early convergence
-    `random_state` : Seed for random permutation
+    `n_clusters` : int
+        Number of clusters to estimate
+    `max_iter` : int, default=100
+        Maximum amount of iteration
+    `tol` : float, default=1e-5
+        Tolerance for early convergence
+    `random_state` : int, optional, default=None
+        Seed for random permutation
 
     """
 
     def __init__(
         self,
         n_clusters: int,
         max_iter: int = 100,
         tol: float = 1e-5,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ) -> None:
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.tol = tol
         self.random_state = random_state
         self.verbose = verbose
@@ -132,17 +136,20 @@
     typically used to estimate model parameters, including cluster
     probabilities and multinomial parameters. MMM is commonly applied in text
     analysis and other scenarios involving discrete data, like document
     clustering or topic modeling.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters to estimate
-    `max_iter` : Maximum amount of iteration
-    `tol` : Tolerance for early convergence
+    `n_clusters` : int
+        Number of clusters to estimate
+    `max_iter` : int, default=100
+        Maximum amount of iteration
+    `tol` : float, default=1e-5
+        Tolerance for early convergence
 
     """
 
     def __init__(
         self,
         n_clusters: int,
         max_iter: int = 100,
```

### Comparing `luma-ml-0.7.5/luma/clustering/spectral.py` & `luma-ml-0.8.0/luma/clustering/spectral.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,16 +29,18 @@
     dimensionality reduction followed by a traditional clustering
     method, like K-means, in this transformed space. This approach
     is effective for identifying clusters with irregular shapes
     and non-linearly separable data.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters to estimate
-    `gamma` : Scaling factor for Gaussian kernel
+    `n_clusters` : int
+        Number of clusters to estimate
+    `gamma` : float, default=1.0
+        Scaling factor for Gaussian kernel
 
     Examples
     --------
     >>> sp = SpectralClustering()
     >>> sp.fit(X, y)
     >>> lables = sp.labels # Get assigned labels
 
@@ -99,17 +101,20 @@
     applied to this normalized Laplacian, and the resulting eigenvectors are
     used to transform the data into a new space. Finally, a clustering algorithm,
     such as k-means, is applied in this transformed space, effectively revealing
     clusters that are not easily distinguishable in the original space.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters to estimate
-    `gamma` : Scaling factor for Gaussian kernel
-    `strategy` : Normalization strategy (e.g. `symmetric`, `random-walk`)
+    `n_clusters` : int
+        Number of clusters to estimate
+    `gamma` : float, default=1.0
+        Scaling factor for Gaussian kernel
+    `strategy` : {"symmetric", "random-walk"}, default="symmetric"
+        Normalization strategy
 
     """
 
     def __init__(
         self,
         n_clusters: int,
         gamma: float = 1.0,
@@ -180,20 +185,22 @@
     clustered using hierarchical methods, either agglomerative (building
     clusters by merging smaller ones) or divisive (splitting larger clusters
     into smaller ones). This approach reveals multi-level structures in the
     data, uncovering both broad and fine-grained clustering patterns.
 
     Parameters
     ----------
-    `n_clusters` : Number of clusters to estimate
-    `method` : Method for hierarchical clustering
-    (e.g. `agglomerative`, `divisive`)
-    `linkage` : Linkage method for `agglomerative` clustering
-    (e.g. `single`, `complete`, `average`, `ward`)
-    `gamma` : Scaling factor for Gaussian kernel
+    `n_clusters` : int
+        Number of clusters to estimate
+    `method` : {"agglomerative", "divisive"}
+        Method for hierarchical clustering
+    `linkage` : {"single", "complete", "average"}, default="single"
+        Linkage method for agglomerative clustering
+    `gamma` : float, default=1.0
+        Scaling factor for Gaussian kernel
 
     """
 
     def __init__(
         self,
         n_clusters: int,
         method: Literal["agglomerative", "divisive"],
@@ -274,16 +281,18 @@
     tuning. It constructs a similarity matrix, typically using a Gaussian kernel
     with an adaptively chosen scale. Eigenvalue decomposition on the Laplacian of
     this matrix reveals the data's structure, and the eigen-gap heuristic is
     employed to select the optimal number of clusters.
 
     Parameters
     ----------
-    `gamma` : Scaling factor for Gaussian kernel
-    `max_clusters` : Upper-bound of the number of clusters to estimate
+    `gamma` : float, default=1.0
+        Scaling factor for Gaussian kernel
+    `max_clusters` : int, default=10
+        Upper-bound of the number of clusters to estimate
 
     """
 
     def __init__(self, gamma: float = 1.0, max_clusters: int = 10) -> None:
         self.gamma = gamma
         self.max_clusters = max_clusters
         self._X = None
```

### Comparing `luma-ml-0.7.5/luma/core/base.py` & `luma-ml-0.8.0/luma/core/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
     Set the parameters of an estimator or a transformer:
     ```py
         def set_params(self, **kwargs) -> None
     ```
     This method iterates over the given keyword arguments and sets the
     attributes of the instance accordingly.
+
     If an attribute corresponding to a given keyword does not exist,
     a message is printed indicating that the attribute was not found.
 
     Notes
     -----
     Upon the call of `set_params`, the method `check_param_ranges` is
     automatically called after resetting the parameters.
```

### Comparing `luma-ml-0.7.5/luma/core/super.py` & `luma-ml-0.8.0/luma/core/super.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,27 +29,24 @@
     Methods
     -------
     For training:
     ```py
         @abstractmethod
         def fit(self, *args) -> Self
     ```
-
     For prediction:
     ```py
         @abstractmethod
         def predict(self, *args) -> Vector
     ```
-
     For scoring
     ```py
         @abstractmethod
         def score(self, *args) -> float
     ```
-
     For setting parameters when tuning
     ```py
         def set_params(self, *args) -> None
     ```
     """
 
     class Meta:
@@ -118,27 +115,24 @@
     Methods
     -------
     For fitting:
     ```py
         @abstractmethod
         def fit(self, *args) -> Self
     ```
-
     For transformation:
     ```py
         @abstractmethod
         def transform(self, *args) -> Matrix
     ```
-
     For fitting and transformation at once:
     ```py
         @abstractmethod
         def fit_transform(self, *args) -> Matrix
     ```
-
     For setting parameters when tuning:
     ```py
         def set_params(self, *args) -> None
     ```
     """
 
     class Feature:
@@ -190,15 +184,15 @@
             To ignore `y`, replace with placeholder `_`:
             ```py
             def fit(self, X: Matrix, _ = None) -> Transformer
             ```
         * `transform` method gets `X` and `y` and returns transformed `X` and `y`
 
             ```py
-            def transform(self, X: Matrix, y: Vector) -> Tuple[Matrix, Matrix | Vector]
+            def transform(self, X: Matrix, y: Vector) -> tuple[Matrix, Matrix | Vector]
             ```
         """
 
     @abstractmethod
     def fit(self, *args) -> Self: ...
 
     @abstractmethod
@@ -229,27 +223,32 @@
 
     Properties
     ----------
     Get the best(optimized) estimator or transformer (not for `Neural`):
     ```py
         @property
         def best_model(self) -> Estimator | Transformer
-
+    ```
     """
 
     class Neural:
         """
         An inner class of `Optimizer` dedicated to neural optimizing techniques.
 
         Methods
         -------
         For updating weights:
         ```py
-        @abstractmethod
-        def update(self, **kwargs) -> tuple
+        def update(
+            self,
+            weights: TensorLike | None,
+            biases: TensorLike | None,
+            grad_weights: TensorLike,
+            grad_biases: TensorLike,
+        ) -> None
         ```
         """
 
         def __init__(self) -> None:
             self.updated_weights = None
             self.updated_biases = None
 
@@ -286,21 +285,21 @@
     how well a model is performing on a particular task,
     such as classification or regression.
 
     Methods
     -------
     For scoring:
     ```py
-        @staticmethod
+        @classmethod
         @abstractmethod
         def score(*args) -> float
     ```
     """
 
-    @staticmethod
+    @classmethod
     @abstractmethod
     def score(*args) -> float: ...
 
 
 class Visualizer(VisualBase, metaclass=ABCMeta):
     """
     A visualizer is a tool that helps visualize and understand various aspects
@@ -358,15 +357,16 @@
     or "difference" there is between two points, objects, or distributions. Different
     types of distances serve various purposes, and they are used in different contexts.
 
     Methods
     -------
     For computing the distance:
     ```py
-        @staticmethod
+        @classmethod
         @abstractmethod
         def compute(*args) -> float
     ```
     """
 
+    @classmethod
     @abstractmethod
     def score(*args) -> float: ...
```

### Comparing `luma-ml-0.7.5/luma/ensemble/bagging.py` & `luma-ml-0.8.0/luma/ensemble/bagging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Self
+from typing import Any, Self
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.typing import Matrix, Vector
 from luma.interface.util import Clone
 from luma.interface.exception import NotFittedError
 
@@ -24,49 +24,58 @@
     random subset of features. The final prediction is made by aggregating
     the predictions of all models, typically through voting for
     classification or averaging for regression. This approach reduces
     variance, improves model stability, and can prevent overfitting.
 
     Parameters
     ----------
-    `base_estimator` : Base estimator for training multiple models
-    (Default `DecisionTreeClassifier`)
-    `n_estimators` : Number of base estimators to fit
-    `max_samples` : Maximum number of data to sample (`0~1` proportion)
-    `max_features` : Maximum number of features to sample (`0~1` proporton)
-    `bootstrap` : Whether to bootstrap data samples
-    `bootstrap_feature`: Whether to bootstrap features
-    `random_state` : Seed for random sampling
-    `**kwargs` : Additional parameters for base estimator (i.e. `max_depth`)
+    `base_estimator` : Estimator, default=DecisionTreeClassifier()
+        Base estimator for training multiple models
+    `n_estimators` : int, default=50
+        Number of base estimators to fit
+    `max_samples` : float or int, default=1.0
+        Maximum number of data to sample (`0~1` proportion)
+    `max_features` : float or int, default=1.0
+        Maximum number of features to sample (`0~1` proporton)
+    `bootstrap` : bool, default=True
+        Whether to bootstrap data samples
+    `bootstrap_feature`: bool, default=False
+        Whether to bootstrap features
+    `random_state` : int, optional, default=None
+        Seed for random sampling
+    `**kwargs` : dict[str, Any]
+        Additional parameters for base estimator (i.e. `max_depth`)
 
     Examples
     --------
-    >>> bag = BaggingClassifier(base_estimator=AnyEstimator(),
-                                n_estimators=100,
-                                max_samples=1.0,
-                                max_features=1.0,
-                                bootstrap=True,
-                                bootstrap_feature=False)
+    >>> bag = BaggingClassifier(
+            base_estimator=AnyEstimator(),
+            n_estimators=100,
+            max_samples=1.0,
+            max_features=1.0,
+            bootstrap=True,
+            bootstrap_feature=False,
+        )
     >>> bag.fit(X, y)
     >>> y_pred = bag.predict(X)
     >>> est = bag[i] # Get i-th base estimator from `bag`
 
     """
 
     def __init__(
         self,
         base_estimator: Estimator = DecisionTreeClassifier(),
         n_estimators: int = 50,
         max_samples: float | int = 1.0,
         max_features: float | int = 1.0,
         bootstrap: bool = True,
         bootstrap_feature: bool = False,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
-        **kwargs: Dict[str, Any],
+        **kwargs: dict[str, Any],
     ) -> None:
         self.base_estimator = base_estimator
         self.n_estimators = n_estimators
         self.max_samples = max_samples
         self.max_features = max_features
         self.bootstrap = bootstrap
         self.bootstrap_feature = bootstrap_feature
@@ -150,49 +159,58 @@
     regressors each on random subsets of the original dataset and then
     averages their predictions to form the final prediction. It aims to
     improve the stability and accuracy of machine learning algorithms,
     especially overfitting in decision trees or other similar models.
 
     Parameters
     ----------
-    `base_estimator` : Base estimator for training multiple models
-    (Default `DecisionTreeRegressor`)
-    `n_estimators` : Number of base estimators to fit
-    `max_samples` : Maximum number of data to sample (`0~1` proportion)
-    `max_features` : Maximum number of features to sample (`0~1` proporton)
-    `bootstrap` : Whether to bootstrap data samples
-    `bootstrap_feature`: Whether to bootstrap features
-    `random_state` : Seed for random sampling
-    `**kwargs` : Additional parameters for base estimator (i.e. `max_depth`)
+    `base_estimator` : Estimator, default=DecisionTreeRegressor()
+        Base estimator for training multiple models
+    `n_estimators` : int, default=50
+        Number of base estimators to fit
+    `max_samples` : float or int, default=1.0
+        Maximum number of data to sample (`0~1` proportion)
+    `max_features` : float or int, default=1.0
+        Maximum number of features to sample (`0~1` proporton)
+    `bootstrap` : bool, default=True
+        Whether to bootstrap data samples
+    `bootstrap_feature`: bool, default=False
+        Whether to bootstrap features
+    `random_state` : int, optional, default=None
+        Seed for random sampling
+    `**kwargs` : dict[str, Any]
+        Additional parameters for base estimator (i.e. `max_depth`)
 
     Examples
     --------
-    >>> bag = BaggingRegressor(base_estimator=AnyEstimator(),
-                               n_estimators=100,
-                               max_samples=1.0,
-                               max_features=1.0,
-                               bootstrap=True,
-                               bootstrap_feature=False)
+    >>> bag = BaggingRegressor(
+            base_estimator=AnyEstimator(),
+            n_estimators=100,
+            max_samples=1.0,
+            max_features=1.0,
+            bootstrap=True,
+            bootstrap_feature=False,
+        )
     >>> bag.fit(X, y)
     >>> y_pred = bag.predict(X)
     >>> est = bag[i] # Get i-th base estimator from `bag`
 
     """
 
     def __init__(
         self,
         base_estimator: Estimator = DecisionTreeRegressor(),
         n_estimators: int = 50,
         max_samples: float | int = 1.0,
         max_features: float | int = 1.0,
         bootstrap: bool = True,
         bootstrap_feature: bool = False,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
-        **kwargs: Dict[str, Any],
+        **kwargs: dict[str, Any],
     ) -> None:
         self.base_estimator = base_estimator
         self.n_estimators = n_estimators
         self.max_samples = max_samples
         self.max_features = max_features
         self.bootstrap = bootstrap
         self.bootstrap_feature = bootstrap_feature
```

### Comparing `luma-ml-0.7.5/luma/ensemble/boost.py` & `luma-ml-0.8.0/luma/ensemble/boost.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,22 @@
     weighted based on its accuracy. AdaBoost is adaptive in the sense that
     subsequent weak learners are tweaked in favor of instances that previous
     learners misclassified. The final model makes preds based on the
     weighted majority vote of its weak learners.
 
     Parameters
     ----------
-    `base_estimator` : Base est for training multiple models
-    (Default `DecisionTreeClassifier`)
-    `n_estimators` : Number of base estimators to fit
-    `learning_rate` : Step size of class weights(`alpha`) update
-    `**kwargs` : Additional parameters for base est (i.e. `max_depth`)
+    `base_estimator` : Estimator, default=DecisionTreeClassifier()
+        Base est for training multiple models
+    `n_estimators` : int, default=50
+        Number of base estimators to fit
+    `learning_rate` : float, default=1.0
+        Step size of class weights(`alpha`) update
+    `**kwargs` : dict[str, Any]
+        Additional parameters for base est (i.e. `max_depth`)
 
     Examples
     --------
     >>> ada_est = AdaBoostClassifier(learning_rate=1.0, ...)
     >>> ada_est.fit(X, y)
 
     >>> y_pred = ada_est.predict(X)
@@ -158,20 +161,24 @@
     residual errors of the previous learners. The final output is a
     combination of the weak learners' outputs, weighted by their individual
     contributions to the ensemble's performance, which aims to produce
     a more accurate regression model.
 
     Parameters
     ----------
-    `base_estimator` : Base est for training multiple models
-    (Default `DecisionTreeRegressor`)
-    `n_estimators` : Number of base estimators to fit
-    `learning_rate` : Step size of class weights(`alpha`) update
-    `loss` : Type of loss function (e.g. `linear`, `square`, `exp`)
-    `**kwargs` : Additional parameters for base est (i.e. `max_depth`)
+    `base_estimator` : Estimator, default=DecisionTreeRegressor()
+        Base est for training multiple models
+    `n_estimators` : int, default=50
+        Number of base estimators to fit
+    `learning_rate` : float, default=1.0
+        Step size of class weights(`alpha`) update
+    `loss` : {"linear", "square", "exp"}, default="linear"
+        Type of loss function
+    `**kwargs` : dict[str, Any]
+        Additional parameters for base est (i.e. `max_depth`)
 
     Examples
     --------
     >>> ada_reg = AdaBoostRegressor(learning_rate=1.0, ...)
     >>> ada_reg.fit(X_train, y_train)
 
     >>> y_pred = ada_reg.predict(X_test)
@@ -293,25 +300,29 @@
     ones. It introduces randomness and prevents overfitting through techniques
     like subsampling and feature selection. GBC is versatile, effective for a
     wide range of classification and regression tasks, and performs well on
     both linear and non-linear problems.
 
     Parameters
     ----------
-    `base_estimator` : Base est for training multiple models
-    (Default `DecisionTreeRegressor`)
-    `n_estimators` : Number of boosting stages to be run
-    `learning_rate` : Shrinking factor of the contribution of each est
-    `subsample` : Fraction of samples to be used for fitting each est
-    `**kwargs` : Additional parameters for base est (i.e. `max_depth`)
+    `base_estimator` : Estimator, default=DecisionTreeRegressor()
+        Base est for training multiple models
+    `n_estimators` : int, default=50
+        Number of boosting stages to be run
+    `learning_rate` : float, default=0.01
+        Shrinking factor of the contribution of each est
+    `subsample` : float, default=1.0, range=[0,1]
+        Fraction of samples to be used for fitting each est
+    `**kwargs` : dict[str, Any]
+        Additional parameters for base est (i.e. `max_depth`)
 
     Notes
     -----
     - Upon using `__getitem__`, it returns a list of base estimators
-    of the passed class index:
+        of the passed class index:
 
         ```py
         gb_model = GradientBoostingClassifier(...)
         ...
         gb_model[1] # List of estimators of the class '1'
         gb_model[2][0] # First estimator of the class '2'
         ```
@@ -423,24 +434,28 @@
     manner, where each tree tries to correct the errors of its predecessor
     by fitting to the residual errors. It combines weak learners to create
     a strong predictive model and minimizes a loss function, often mean
     squared error, iteratively.
 
     Parameters
     ----------
-    `base_estimator` : Base est for training multiple models
-    (Default `DecisionTreeRegressor`)
-    `n_estimators` : Number of boosting stages to be run
-    `learning_rate` : Rate of contribution of each est
-    `subsample` : Fraction of samples to be used for fitting each est
-    `loss` : Type of loss function (Default `mse`)
-    `delta` : Balancing factor between `mse` and `mae`
-    `verbose` : Whether to output progress messages
-    `**kwargs` : Additional parameters for the base est
-    (i.e. `max_depth`)
+    `base_estimator` : Estimator, default=DecisionTreeRegressor()
+        Base est for training multiple models
+    `n_estimators` : int, default=50
+        Number of boosting stages to be run
+    `learning_rate` : float, default=0.01
+        Rate of contribution of each est
+    `subsample` : float, default=1.0, range=[0,1]
+        Fraction of samples to be used for fitting each est
+    `loss` : {"mse", "mae", "huber"}, default="mse"
+        Type of loss function
+    `delta` : float, default=1.0
+        Balancing factor between `mse` and `mae`
+    `**kwargs` : dict[str, Any]
+        Additional parameters for the base estimator (i.e. `max_depth`)
 
     """
 
     def __init__(
         self,
         base_estimator: Estimator = DecisionTreeRegressor(),
         n_estimators: int = 50,
```

### Comparing `luma-ml-0.7.5/luma/ensemble/forest.py` & `luma-ml-0.8.0/luma/ensemble/forest.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,38 +19,49 @@
     A Random Forest Classifier is an ensemble learning method in machine learning,
     widely used for both classification and regression tasks. It operates by
     constructing a multitude of decision trees during the training phase and
     outputs the mode of the classes for classification.
 
     Parameters
     ----------
-    `n_trees` : Number of trees in the forest
-    `max_depth` :  Maximum depth of each trees
-    `criterion` : Function used to measure the quality of a split
-    `min_samples_split` : Minimum samples required to split a node
-    `min_samples_leaf` : Minimum samples required to be at a leaf node
-    `max_features` : Number of features to consider
-    `min_impurity_decrease` : Minimum decrement of impurity for a split
-    `max_leaf_nodes` : Maximum amount of leaf nodes
-    `bootstrap` : Whether to bootstrap the samples of dataset
-    `bootstrap_feature` : Whether to bootstrap the features of each data
-    `n_features` : Number of features to be sampled when bootstrapping features
+    `n_trees` : int, default=10
+        Number of trees in the forest
+    `max_depth` :  int, default=100
+        Maximum depth of each trees
+    `criterion` : {"gini", "entropy"}, default="gini"
+        Function used to measure the quality of a split
+    `min_samples_split` : int, default=2
+        Minimum samples required to split a node
+    `min_samples_leaf` : int, default=1
+        Minimum samples required to be at a leaf node
+    `max_features` : int, optional, default=None
+        Number of features to consider
+    `min_impurity_decrease` : float, default=0.0
+        Minimum decrement of impurity for a split
+    `max_leaf_nodes` : int, optional, default=None
+        Maximum amount of leaf nodes
+    `bootstrap` : bool, default=True
+        Whether to bootstrap the samples of dataset
+    `bootstrap_feature` : bool, default=False
+        Whether to bootstrap the features of each data
+    `n_features` : int or {"auto"}, default="auto"
+        Number of features to be sampled when bootstrapping features
 
     """
 
     def __init__(
         self,
         n_trees: int = 10,
         max_depth: int = 100,
         criterion: Literal["gini", "entropy"] = "gini",
         min_samples_split: int = 2,
         min_samples_leaf: int = 1,
-        max_features: int = None,
+        max_features: int | None = None,
         min_impurity_decrease: float = 0.0,
-        max_leaf_nodes: int = None,
+        max_leaf_nodes: int | None = None,
         bootstrap: bool = True,
         bootstrap_feature: bool = False,
         n_features: int | Literal["auto"] = "auto",
         verbose: bool = False,
     ) -> None:
         self.n_trees = n_trees
         self.max_depth = max_depth
@@ -137,36 +148,46 @@
     A Random Forest Regressor is an ensemble learning algorithm for regression
     tasks. It builds multiple decision trees during training, each on a random
     subset of features and bootstrapped data. The final prediction is the average
     of individual tree predictions, providing a robust and accurate result.
 
     Parameters
     ----------
-    `n_trees` : Number of trees in the forest
-    `max_depth` :  Maximum depth of each trees
-    `min_samples_split` : Minimum samples required to split a node
-    `min_samples_leaf` : Minimum samples required to be at a leaf node
-    `max_features` : Number of features to consider
-    `min_variance_decrease` : Minimum decrement of variance for a split
-    `max_leaf_nodes` : Maximum amount of leaf nodes
-    `bootstrap` : Whether to bootstrap the samples of dataset
-    `bootstrap_feature` : Whether to bootstrap the features of each data
-    `n_features` : Number of features to be sampled when bootstrapping features
+    `n_trees` : int, default=10
+        Number of trees in the forest
+    `max_depth` : int, default=10
+        Maximum depth of each trees
+    `min_samples_split` : int, default=2
+        Minimum samples required to split a node
+    `min_samples_leaf` : int, default=1
+        Minimum samples required to be at a leaf node
+    `max_features` : int, optional, default=None
+        Number of features to consider
+    `min_variance_decrease` : float, default=0.0
+        Minimum decrement of variance for a split
+    `max_leaf_nodes` : int, optional, default=None
+        Maximum amount of leaf nodes
+    `bootstrap` : bool, default=True
+        Whether to bootstrap the samples of dataset
+    `bootstrap_feature` : bool, default=False
+        Whether to bootstrap the features of each data
+    `n_features` : int or {"auto"}, default="auto"
+        Number of features to be sampled when bootstrapping features
 
     """
 
     def __init__(
         self,
         n_trees: int = 10,
         max_depth: int = 10,
         min_samples_split: int = 2,
         min_samples_leaf: int = 1,
-        max_features: int = None,
+        max_features: int | None = None,
         min_variance_decrease: float = 0.0,
-        max_leaf_nodes: int = None,
+        max_leaf_nodes: int | None = None,
         bootstrap: bool = True,
         bootstrap_feature: bool = False,
         n_features: int | Literal["auto"] = "auto",
         sample_weights: Vector = None,
         verbose: bool = False,
     ) -> None:
         self.n_trees = n_trees
@@ -242,9 +263,9 @@
 
     def score(
         self, X: Matrix, y: Matrix, metric: Evaluator = MeanSquaredError
     ) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
-    def __gettiem__(self, index: int) -> DecisionTreeClassifier:
+    def __gettiem__(self, index: int) -> DecisionTreeRegressor:
         return self.trees[index]
```

### Comparing `luma-ml-0.7.5/luma/ensemble/stack.py` & `luma-ml-0.8.0/luma/ensemble/stack.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,68 +22,78 @@
     classifier, often called a meta-classifier, is trained to make a final
     prediction based on the outputs of the base classifiers. Stacking aims to
     leverage the strengths of each base model to improve overall prediction
     accuracy.
 
     Parameters
     ----------
-    `estimators` : List of base estimators
-    `final_estimator` : Final meta-estimator (Default `SoftmaxRegressor`)
-    `pass_original` : Whether to pass the original data to final estimator
-    `drop_threshold` : Omitting threshold for base estimators
-    (`None` not to omit any estimators)
-    `metric` : Scoring metric
-    `method` : Methods called for each base estimator
-    `cv` : Number of folds for cross-validation
-    `fold_type` : Fold type (Default `KFold`)
-    `shuffle` : Whether to shuffle the dataset when cross-validating
-    `random_state` : Seed for random splitting
-    `**kwargs` : Additional parameters for final estimator
-    (i.e. `learning_rate`)
+    `estimators` : list of Estimator
+        List of base estimators
+    `final_estimator` : Estimator, default=SoftmaxRegressor()
+        Final meta-estimator
+    `pass_original` : bool, default=False
+        Whether to pass the original data to final estimator
+    `drop_threshold` : float, optional, default=None
+        Omitting threshold for base estimators (None not to omit any estimators)
+    `metric` : Evaluator, default=Accuracy
+        Scoring metric
+    `method` : {"label", "prob"}, default="label"
+        Methods called for each base estimator
+    `cv` : int, default=5
+        Number of folds for cross-validation
+    `fold_type` : FoldType, default=KFold
+        Fold type (pass the class itself, not its instance)
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset when cross-validating
+    `random_state` : int, optional, default=None
+        Seed for random splitting
+    `**kwargs` : dict[str, Any]
+        Additional parameters for final estimator (i.e. `learning_rate`)
 
     Notes
     -----
     `StackingClassifier` can also be utilized as `Transformer`.
 
     - The method `transform` returns class labels or probabilities by each
         base estimator as a stacked form:
 
         ```py
         def transform(self, X: Matrix) -> Matrix
         ```
-
     Each base estimators can be accessed via indexing of its instance:
     >>> estimator = stack[0]
 
     Examples
     --------
     ```py
-    stack = StackingClassifier(estimators=[...],
-                               final_estimator=SoftmaxRegressor(),
-                               method='label',
-                               cv=5,
-                               fold_type=KFold)
+    stack = StackingClassifier(
+        estimators=[...],
+        final_estimator=SoftmaxRegressor(),
+        method='label',
+        cv=5,
+        fold_type=KFold,
+    )
     stack.fit(X, y)
     X_new = stack.transform(X)
     y_pred = stack.predict(X)
     ```
     """
 
     def __init__(
         self,
         estimators: List[Estimator],
         final_estimator: Estimator = SoftmaxRegressor(),
         pass_original: bool = False,
-        drop_threshold: float = None,
+        drop_threshold: float | None = None,
         metric: Evaluator = Accuracy,
         method: Literal["label", "prob"] = "label",
         cv: int = 5,
         fold_type: FoldType = KFold,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
         **kwargs: Dict[str, Any],
     ) -> None:
         self.estimators = estimators
         self.final_estimator = final_estimator
         self.pass_original = pass_original
         self.drop_threshold = drop_threshold
@@ -105,15 +115,19 @@
         self.check_param_ranges()
 
     def fit(self, X: Matrix, y: Vector) -> Self:
         m, _ = X.shape
         self.n_classes = len(np.unique(y))
 
         fold = self.fold_type(
-            X, y, n_folds=self.cv, shuffle=self.shuffle, random_state=self.random_state
+            X,
+            y,
+            n_folds=self.cv,
+            shuffle=self.shuffle,
+            random_state=self.random_state,
         )
 
         if self.method == "label":
             X_new = np.zeros((m, len(self.estimators)))
         else:
             X_new = np.zeros((m, len(self.estimators) * self.n_classes))
 
@@ -242,46 +256,55 @@
     regressor, often called a meta-regressor, is trained to make a final
     prediction based on the outputs of the base regressors. Stacking aims to
     leverage the strengths of each base model to improve overall prediction
     accuracy.
 
     Parameters
     ----------
-    `estimators` : List of base estimators
-    `final_estimator` : Final meta-estimator (Default `LinearRegressor`)
-    `pass_original` : Whether to pass the original data to final estimator
-    `cv` : Number of folds for cross-validation
-    `fold_type` : Fold type (Default `KFold`)
-    `metric` : Scoring metric
-    `shuffle` : Whether to shuffle the dataset when cross-validating
-    `random_state` : Seed for random splitting
-    `**kwargs` : Additional parameters for final estimator
-    (i.e. `learning_rate`)
+    `estimators` : list of Estimator
+        List of base estimators
+    `final_estimator` : Estimator, default=LinearRegressor()
+        Final meta-estimator
+    `pass_original` : bool, default=False
+        Whether to pass the original data to final estimator
+    `cv` : int, default=5
+        Number of folds for cross-validation
+    `fold_type` : FoldType, default=KFold
+        Fold type (pass the class itself, not its instance)
+    `metric` : Evaluator, default=MeanSquaredError
+        Scoring metric
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset when cross-validating
+    `random_state` : int, optional, default=None
+        Seed for random splitting
+    `**kwargs` : dict[str, Any]
+        Additional parameters for final estimator (i.e. `learning_rate`)
 
     Notes
     -----
     `StackingRegressor` can also be utilized as `Transformer`.
 
     - The method `transform` returns class labels or probabilities by each
         base estimator as a stacked form:
 
         ```py
         def transform(self, X: Matrix) -> Matrix
         ```
-
     Each base estimators can be accessed via indexing of its instance:
     >>> estimator = stack[0]
 
     Examples
     --------
     ```py
-    stack = StackingRegressor(estimators=[...],
-                              final_estimator=LinearRegressor(),
-                              cv=5,
-                              fold_type=KFold)
+    stack = StackingRegressor(
+        estimators=[...],
+        final_estimator=LinearRegressor(),
+        cv=5,
+        fold_type=KFold,
+    )
     stack.fit(X, y)
     X_new = stack.transform(X)
     y_pred = stack.predict(X)
     ```
     """
 
     def __init__(
@@ -289,15 +312,15 @@
         estimators: List[Estimator],
         final_estimator: Estimator = LinearRegressor(),
         pass_original: bool = False,
         cv: int = 5,
         fold_type: FoldType = KFold,
         metric: Evaluator = MeanSquaredError,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
         **kwargs: Dict[str, Any],
     ) -> None:
         self.estimators = estimators
         self.final_estimator = final_estimator
         self.pass_original = pass_original
         self.cv = cv
```

### Comparing `luma-ml-0.7.5/luma/ensemble/vote.py` & `luma-ml-0.8.0/luma/ensemble/vote.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,36 +23,40 @@
     robustness by leveraging the strengths of diverse models. It's
     particularly useful when individual models have different error patterns.
     The Voting Classifier is widely used in classification tasks to improve
     performance over single models.
 
     Parameters
     ----------
-    `estimators` : List of estimators to vote
-    `voting` : Voting criterion
-    (`label` to vote the most frequent and `prob` to vote the most probable)
-    `weights` : Weights for each classifier on voting
-    (`None` for uniform weights)
+    `estimators` : list of Esimators, required optional, default=None
+        List of estimators to vote
+    `voting` : {"label", "prob"}, default="label"
+        Voting criterion ("label" to vote the most frequent and
+        "prob" to vote the most probable)
+    `weights` : Vector[Scalar], optional, default=None
+        Weights for each classifier on voting (None for uniform weights)
 
     Examples
     --------
-    >>> vot = VotingClassifier(estimators=[AnyClassifier(), ...],
-                               voting='label',
-                               weights=[0.25, 0.5, ...])
+    >>> vot = VotingClassifier(
+            estimators=[AnyClassifier(), ...],
+            voting="label",
+            weights=[0.25, 0.5, ...],
+        )
     >>> vot.fit(X, y)
     >>> pred = vot.predict(X)
     >>> clf = vot[i] # Get i-th classifier from `vot`
 
     """
 
     def __init__(
         self,
-        estimators: List[Estimator] = None,
+        estimators: List[Estimator] | None = None,
         voting: Literal["label", "prob"] = "label",
-        weights: Vector[Scalar] = None,
+        weights: Vector[Scalar] | None = None,
         verbose: bool = False,
     ) -> None:
         self.estimators = estimators
         self.voting = voting
         self.weights = weights
         self.verbose = verbose
         self._fitted = False
@@ -123,32 +127,35 @@
     This approach can increase prediction accuracy and robustness by leveraging
     the strengths of diverse models. It's particularly useful when individual
     models have different error patterns. The Voting Regressor is widely used in
     regression tasks to improve performance over single models.
 
     Parameters
     ----------
-    `estimators` : List of regressors to vote
-    `weights` : Weights for each regressor on voting
-    (`None` for uniform weights)
+    `estimators` : list of Esimators, required optional, default=None
+        List of estimators to vote
+    `weights` : Vector[Scalar], optional, default=None
+        Weights for each classifier on voting (None for uniform weights)
 
     Examples
     --------
-    >>> vot = VotingRegressor(estimators=[AnyRegressor(), ...],
-                              weights=[0.25, 0.5, ...])
+    >>> vot = VotingRegressor(
+            estimators=[AnyRegressor(), ...],
+            weights=[0.25, 0.5, ...],
+        )
     >>> vot.fit(X, y)
     >>> pred = vot.predict(X)
     >>> reg = vot[i] # Get i-th regressor from `vot`
 
     """
 
     def __init__(
         self,
-        estimators: List[Estimator] = None,
-        weights: Vector[Scalar] = None,
+        estimators: List[Estimator] | None = None,
+        weights: Vector[Scalar] | None = None,
         verbose: bool = False,
     ) -> None:
         self.estimators = estimators
         self.weights = weights
         self.verbose = verbose
         self._fitted = False
```

### Comparing `luma-ml-0.7.5/luma/interface/exception.py` & `luma-ml-0.8.0/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/interface/typing.py` & `luma-ml-0.8.0/luma/interface/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,33 +107,33 @@
     """
     A placeholder class for scalar type.
 
     This class encompasses `int` and `float`.
     """
 
     def __new__(cls, value: int | float) -> Self:
-        return float(value)
+        return value
 
 
 class ClassType:
     """
     An interface class designed to facilitate the annotation of
     dedicated types for classes in a systematic way.
 
     The `ClassType` class includes several classmethods that act
     as decorator factories. These decorators can be applied to classes
     to specify their types or roles within the application more
     explicitly.
 
     Decorator Factories
     -------------------
-    - `non_instantiable` : Makes a class non-instantiable.
-
-    - `private` : Makes a class private; accesses are restricted
-                  outside its module.
+    `non_instantiable` : callable
+        Makes a class non-instantiable.
+    `private` : callable
+        Makes a class private; accesses are restricted outside its module.
 
     """
 
     T = TypeVar("T", bound=type)
 
     @classmethod
     def non_instantiable(cls) -> Callable:
```

### Comparing `luma-ml-0.7.5/luma/interface/util.py` & `luma-ml-0.8.0/luma/interface/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Any, Callable, Iterable, Literal, Type, TypeGuard
+from typing import Any, Callable, Iterable, Literal, Self, Type, TypeGuard
 from rich.progress import Progress, BarColumn, TextColumn
 import numpy as np
 
 from luma.interface.exception import UnsupportedParameterError, InvalidRangeError
-from luma.interface.typing import Matrix, Scalar
+from luma.interface.typing import Matrix, Scalar, Vector
 from luma.neural import init
 
 
 __all__ = (
     "DecisionTreeNode",
     "NearestNeighbors",
     "SilhouetteUtil",
@@ -23,29 +23,34 @@
 
 class DecisionTreeNode:
     """
     Internal class for node used in tree-based models.
 
     Parameters
     ----------
-    `feature_index` : Feature of node
-    `threshold` : Threshold for split point
-    `left` : Left-child node
-    `right` : Right-child node
-    `value` : Most popular label of leaf node
+    `feature_index` : int, optional, default=None
+        Feature of node
+    `threshold` : float, optional, default=None
+        Threshold for split point
+    `left` : Self, optional, default=None
+        Left-child node
+    `right` : Self, optional, default=None
+        Right-child node
+    `value` : Any, optional, default=None
+        Most popular label of leaf node
 
     """
 
     def __init__(
         self,
-        feature_index: int = None,
-        threshold: float = None,
-        left: "DecisionTreeNode" = None,
-        right: "DecisionTreeNode" = None,
-        value: Any = None,
+        feature_index: int | None = None,
+        threshold: float | None = None,
+        left: Self | None = None,
+        right: Self | None = None,
+        value: Any | None = None,
     ) -> None:
         self.feature_index = feature_index
         self.threshold = threshold
         self.left = left
         self.right = right
         self.value = value
 
@@ -56,16 +61,18 @@
 
 class NearestNeighbors:
     """
     Internal class for computing nearest neighbors of given data.
 
     Parameters
     ----------
-    `data` : Data to be handled
-    `n_neighbors` : Number of nearest neighbors
+    `data` : Matrix
+        Data to be handled
+    `n_neighbors` : int
+        Number of nearest neighbors
 
     """
 
     def __init__(self, data: Matrix, n_neighbors: int) -> None:
         self.data = data
         self.n_neighbors = n_neighbors
         self._size = data.shape[0]
@@ -90,23 +97,27 @@
 class SilhouetteUtil:
     """
     Internal class for computing various distances used in
     Silhouette Coefficient calculation.
 
     Parameters
     ----------
-    `idx` : Index of a single data point
-    `cluster` : Current cluster number
-    `labels` : Labels assigned by clustering estimator
-    `distances` : Square-form distance matrix of the data
+    `idx` : int
+        Index of a single data point
+    `cluster` : int
+        Current cluster number
+    `labels` : Vector
+        Labels assigned by clustering estimator
+    `distances` : Matrix
+        Square-form distance matrix of the data
 
     """
 
     def __init__(
-        self, idx: int, cluster: int, labels: Matrix, distances: Matrix
+        self, idx: int, cluster: int, labels: Vector, distances: Matrix
     ) -> None:
         self.idx = idx
         self.cluster = cluster
         self.labels = labels
         self.distances = distances
 
     @property
@@ -131,20 +142,22 @@
 
 class DBUtil:
     """
     Internal class for supporting Davies-Bouldin Index (DBI) computation.
 
     Parameters
     ----------
-    `data` : Original data
-    `labels` : Labels assigned by clustering estimator
+    `data` : Matrix
+        Original data
+    `labels` : Vector
+        Labels assigned by clustering estimator
 
     """
 
-    def __init__(self, data: Matrix, labels: Matrix) -> None:
+    def __init__(self, data: Matrix, labels: Vector) -> None:
         self.data = data
         self.labels = labels
 
     @property
     def cluster_centroids(self) -> Matrix:
         unique_labels = np.unique(self.labels)
         centroids = [
@@ -183,14 +196,27 @@
 class KernelUtil:
     """
     Internal class for kernel methods(tricks).
 
     This class facilitates transferring kernel type strings
     into actual specific kernel function.
 
+    Parameters
+    ----------
+    `kernel` : FuncType
+        Type of kernel
+    `alpha` : float, default=1.0
+        Shape parameter for RBF and sigmoid kernels
+     `gamma` : float, default=0.0
+        Shape parameter of Gaussian curve for RBF kernel
+    `coef` : float, default=1.0
+        Coefficient for polynomial and sigmoid kernel
+    `deg` : int, default=3
+        Polynomial Degree for polynomial kernel
+
     Example
     -------
     >>> util = KernelUtil(kernel='rbf', **params)
     >>> util.kernel_func
     KernelUtil.rbf_kernel: Callable[[Matrix, Matrix | None], Matrix]
 
     """
@@ -207,15 +233,15 @@
         "sigmoid",
         "lap",
         "laplacian",
     ]
 
     def __init__(
         self,
-        kernel: str,
+        kernel: FuncType,
         alpha: float = 1.0,
         gamma: float = 1.0,
         coef: float = 0.0,
         deg: int = 2,
     ) -> None:
         self.kernel = kernel
         self.alpha = alpha
@@ -277,25 +303,31 @@
     which can be either an Estimator or a Transformer.
     The clone includes all parameters of the original model.
     Optionally, the trained state of the model can also be copied
     if applicable.
 
     Parameters
     ----------
-    `model` : The model to be cloned
-    `pass_fitted` : Whether to copy the fitted state of the original model
+    `model` : object, optional, default=None
+        The model to be cloned
+    `pass_fitted` : bool, default=True
+        Whether to copy the fitted state of the original model
 
     Examples
     --------
     >>> original_model = AnyModel(...)
     >>> cloned_model = Clone(model=original_model, pass_fitted=True).get
 
     """
 
-    def __init__(self, model: object = None, pass_fitted: bool = False) -> None:
+    def __init__(
+        self,
+        model: object | None = None,
+        pass_fitted: bool = False,
+    ) -> None:
         self.model = model
         self.pass_fitted = pass_fitted
 
     @property
     def get(self) -> object:
         model_cls = type(self.model)
         new_model = model_cls()
@@ -318,17 +350,19 @@
 
     This class provides a user-friendly functionality which checks whether
     a certain parameter value falls within its preferred numerical range
     depending on its algorithm.
 
     Parameters
     ----------
-    `param_range` : An interval of a parameter (customizable)
-    `param_type` : Data type of a parameter to be forced to have
-    (`None` for both `int` and `float` types)
+    `param_range` : RangeStr
+        An interval of a parameter (customizable)
+    `param_type` : Type[Scalar], optional, default=None
+        Data type of a parameter to be forced to have
+        (None for both `int` and `float` types)
 
     Method
     ------
     To check its validity:
     ```py
     def check(self, param_value: Any) -> None
     ```
@@ -420,15 +454,16 @@
 
 class InitUtil:
     """
     An utility class for weight initializers used in neural networks.
 
     Parameters
     ----------
-    `initializer` : Name of an initializer (`InitStr`)
+    `initializer` : InitStr, optional, default=True
+        Name of an initializer
 
     Properties
     ----------
     To get the corresponding initializer type:
     ```py
     @property
     def initializer_type(self) -> type | None
@@ -454,14 +489,21 @@
 class TrainProgress:
     """
     An utility class for managing auto-updating progress bar during training.
 
     It facilitates the progress bar from the module `rich`, which provides
     well-structured progress bar with colored indications for better readability.
 
+    Parameters
+    ----------
+    `n_iter` : int
+        Number of iterations(or epochs)
+    `bar_width` : int, default=50
+        Width size of a progress bar
+
     Property
     --------
     To get an iterable object from `rich.progress.Progress`:
     ```py
     (property) progress: (self: Self@TrainProgress) -> Iterable
     ```
```

### Comparing `luma-ml-0.7.5/luma/metric/classification.py` & `luma-ml-0.8.0/luma/metric/classification.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/metric/clustering.py` & `luma-ml-0.8.0/luma/metric/clustering.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 from scipy.spatial.distance import pdist, squareform
 import matplotlib.pyplot as plt
 import numpy as np
 
 from luma.core.super import Evaluator, Visualizer
 from luma.interface.util import SilhouetteUtil, DBUtil
-from luma.interface.typing import Matrix, ClassType
+from luma.interface.typing import Matrix, Vector, ClassType
 
 
 __all__ = ("SilhouetteCoefficient", "DaviesBouldin", "Inertia")
 
 
 class SilhouetteCoefficient(Evaluator, Visualizer):
     """
@@ -18,35 +18,35 @@
     own cluster compared to other clusters. The coefficient ranges from -1
     (poorly clustered) to +1 (well clustered), with values near 0 indicating
     overlapping clusters. High average scores across a dataset suggest clear,
     well-separated clusters.
 
     Parameters
     ----------
-    `data` : Original data
-    `labels` : Labels assigned by clustering estimator
+    `data` : Matrix
+        Original data
+    `labels` : Vector
+        Labels assigned by clustering estimator
 
     Examples
     --------
     With Instantiation
     ```py
         sil = SilhouetteCoefficient(data, labels)
         score = sil.score(data, labels) # compute() is a static method
         sil.plot(...)
     ```
-
     Without Instantiation
     ```py
         score = SilhouetteCoefficient.score(data, labels)
         SilhouetteCoefficient.plot(...) # Error; plot() is an instance method
     ```
-
     """
 
-    def __init__(self, data: Matrix, labels: Matrix) -> None:
+    def __init__(self, data: Matrix, labels: Vector) -> None:
         self.data = data
         self.labels = labels
         self.dist = squareform(pdist(self.data))
 
     @staticmethod
     def score(data: Matrix, labels: Matrix) -> Matrix[float]:
         scores = []
@@ -117,21 +117,23 @@
     The Davies-Bouldin Index (DBI) is a metric for evaluating clustering
     algorithms. It compares the average distance within clusters to the
     distance between clusters. Lower DBI values indicate better clustering,
     with compact and well-separated clusters.
 
     Parameters
     ----------
-    `data` : Original data
-    `labels` : Labels assigned by clustering estimator
+    `data` : Matrix
+        Original data
+    `labels` : Vector
+        Labels assigned by clustering estimator
 
     """
 
     @classmethod
-    def score(cls, data: Matrix, labels: Matrix) -> float:
+    def score(cls, data: Matrix, labels: Vector) -> float:
         util = DBUtil(data=data, labels=labels)
         centroids = util.cluster_centroids
         scatter = util.within_cluster_scatter
         separation = util.separation
 
         n_clusters = len(centroids)
         db_values = np.zeros(n_clusters)
@@ -160,16 +162,18 @@
     cluster assignments in algorithms like K-means. A lower inertia value
     indicates more cohesive clusters, where data points are closer to their
     centroids. However, minimizing inertia excessively can lead to overfitting,
     with a large number of clusters.
 
     Parameters
     ----------
-    `data` : Original data
-    `centroids`: Centroids(or medoids for certain algorithm)
+    `data` : Matrix
+        Original data
+    `centroids`: Matrix
+        Centroids(or medoids for certain algorithm)
 
     """
 
     @classmethod
     def score(cls, data: Matrix, centroids: Matrix) -> float:
         sq_dist = (data[:, np.newaxis, :] - centroids[np.newaxis, :, :]) ** 2
         dist = np.sqrt(sq_dist.sum(axis=2))
```

### Comparing `luma-ml-0.7.5/luma/metric/distance.py` & `luma-ml-0.8.0/luma/metric/distance.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/metric/regression.py` & `luma-ml-0.8.0/luma/metric/regression.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/migrate/port.py` & `luma-ml-0.8.0/luma/migrate/port.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,25 @@
     """
     A utility class for exporting and importing machine learning models,
     specifically designed to handle `Estimator` and `Transformer` instances
     within the `luma` framework. It supports saving models to disk with
     automatic naming and enforcing model extension, as well as loading models
     ensuring the correct file extension is used.
 
+    Parameters
+    ----------
+    `model` : Estimator or Transformer
+        A model to port
+    `path` : str
+        Filepath of the model (both for import and export)
+    `filename` : str or {"auto"}, default="auto"
+        Filename of the model
+    `replace` : bool, default=False
+        Whether to replace the existing original file
+
     Methods
     -------
     To save(export) models:
     ```py
     def save(self, model, path, filename, replace) -> str
     ```
     It saves a given model to the specified path with an optional filename.
```

### Comparing `luma-ml-0.7.5/luma/model_selection/cv.py` & `luma-ml-0.8.0/luma/model_selection/cv.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,25 +18,33 @@
     different partitions, providing a robust estimate of the model's
     performance. It's especially useful in scenarios with limited data,
     ensuring that all available data is effectively utilized for both
     training and validation.
 
     Parameters
     ----------
-    `estimator` : An estimator to validate
-    `metric` : Evaluation metric for validation
-    `cv` : Number of folds in splitting data
-    `fold_type` : Fold type (Default `KFold`)
-    `shuffle` : Whether to shuffle the dataset
-    `random_state` : Seed for random sampling upon splitting data
+    `estimator` : Estimator
+        An estimator to validate
+    `metric` : Evaluator
+        Evaluation metric for validation
+    `cv` : int, default=5
+        Number of folds in splitting data
+    `fold_type` : FoldType, default=KFold
+        Fold type
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset
+    `random_state` : int, optional, default=None
+        Seed for random sampling upon splitting data
 
     Attributes
     ----------
-    `train_scores_` : List of training scores for each fold
-    `test_scores_` : List of test(validation) scores for each fold
+    `train_scores_` : list
+        List of training scores for each fold
+    `test_scores_` : list
+        List of test(validation) scores for each fold
 
     Methods
     -------
     For getting mean train score and mean test score respectvely:
     ```py
         def score(self, X: Matrix, y: Vector) -> Tuple[float, float]
     ```
@@ -45,15 +53,15 @@
     def __init__(
         self,
         estimator: Estimator,
         metric: Evaluator,
         cv: int = 5,
         fold_type: FoldType = KFold,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ) -> None:
         self.estimator = estimator
         self.metric = metric
         self.cv = cv
         self.fold_type = fold_type
         self.shuffle = shuffle
```

### Comparing `luma-ml-0.7.5/luma/model_selection/fold.py` & `luma-ml-0.8.0/luma/model_selection/fold.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,19 +20,24 @@
     process ensures that every data point gets to be in the test set
     exactly once and in the training set `k-1` times. It's widely used
     to assess the performance of a model with limited data, providing
     a robust estimate of its generalization capability.
 
     Parameters
     ----------
-    `X` : Input data
-    `y` : Target data
-    `n_folds` : Number of folds
-    `shuffle` : Whether to shuffle the dataset
-    `random_state` : Seed for random shuffling
+    `X` : Matrix
+        Input data
+    `y` : Vector
+        Target data
+    `n_folds` : int, default=5
+        Number of folds
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset
+    `random_state` : int, optional, default=True
+        Seed for random shuffling
 
     Properties
     ----------
     ```py
     @property
     def split(self)
     ```
@@ -41,15 +46,14 @@
     Generator[Tuple[Vector, Vector], None, None]
     ```
     yielding train indices and test indices.
 
     Examples
     --------
     Usage of the generator returned by the property `split`:
-
     ```py
     kfold = KFold(X, y, n_folds=5, shuffle=True)
 
     for train_indices, test_indices in kfold.split:
         X_train, y_train = X[train_indices], y[train_indices]
         ...
     ```
@@ -96,19 +100,24 @@
     percentage of samples for each class. This is especially useful for
     handling imbalances in the dataset. It ensures each fold is a good
     representative of the whole by maintaining the same class distribution
     in each fold as in the complete dataset.
 
     Parameters
     ----------
-    `X` : Input data
-    `y` : Target data
-    `n_folds` : Number of folds
-    `shuffle` : Whether to shuffle the dataset
-    `random_state` : Seed for random shuffling
+    `X` : Matrix
+        Input data
+    `y` : Vector
+        Target data
+    `n_folds` : int, default=5
+        Number of folds
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset
+    `random_state` : int, optional, default=None
+        Seed for random shuffling
 
     Properties
     ----------
     ```py
     @property
     def split(self)
     ```
@@ -117,15 +126,14 @@
     Generator[Tuple[Vector, Vector], None, None]
     ```
     yielding train indices and test indices.
 
     Examples
     --------
     Usage of the generator returned by the property `split`:
-
     ```py
     kfold = StratifiedKFold(X, y, n_folds=5, shuffle=True)
 
     for train_indices, test_indices in kfold.split:
         X_train, y_train = X[train_indices], y[train_indices]
         ...
     ```
@@ -184,20 +192,26 @@
     train/test sets. Each set contains group samples that are entirely in the set
     of training or test. This cross-validation object is a variation of KFold
     that ensures samples from the same group are not split between training and
     testing sets.
 
     Parameters
     ----------
-    `X` : Input data
-    `y` : Target data
-    `groups` : Array of group labels for the samples
-    `n_folds` : Number of folds. Must be at least 2.
-    `shuffle` : Whether to shuffle the dataset
-    `random_state` : Seed for random shuffling
+    `X` : Matrix
+        Input data
+    `y` : Vector
+        Target data
+    `groups` : Vector
+        Array of group labels for the samples
+    `n_folds` : int, default=5
+        Number of folds. Must be at least 2.
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset
+    `random_state` : int, optional, default=None
+        Seed for random shuffling
 
     Properties
     ----------
     ```py
     @property
     def split(self)
     ```
@@ -206,15 +220,14 @@
     Generator[Tuple[Vector, Vector], None, None]
     ```
     yielding train indices and test indices.
 
     Examples
     --------
     Usage of the generator returned by the property `split`:
-
     ```py
     kfold = GroupKFold(X, y, n_folds=5, shuffle=True)
 
     for train_indices, test_indices in kfold.split:
         X_train, y_train = X[train_indices], y[train_indices]
         ...
     ```
```

### Comparing `luma-ml-0.7.5/luma/model_selection/search.py` & `luma-ml-0.8.0/luma/model_selection/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,32 +22,40 @@
     combinations of parameter values to find the best combination. This process
     is performed using cross-validation to ensure model performance is not biased
     to a specific data split. The result is the optimal set of parameters that
     yield the best model performance according to a chosen metric.
 
     Parameters
     ----------
-    `estimator` : An estimator to fit and evaluate
-    `param_grid` : Parameter grid for repetitive search
-    `cv` : K-fold size for cross validation
-    `metric` : Scoring metric for evaluation
-    `maximize` : Whether to optimize in a way of maximizing certain metric
-    `shuffle` : Whether to shuffle the dataset
-    `fold_type` : Fold type (Default `KFold`)
-    `refit` : Whether to re-fit the estimator with the best parameters found
-    `random_state` : Seed for random sampling for cross validation
+    `estimator` : Estimator
+        An estimator to fit and evaluate
+    `param_grid` : dict
+        Parameter grid for repetitive search
+    `cv` : int, default=5
+        K-fold size for cross validation
+    `metric` : Evaluator, optional, default = None
+        Scoring metric for evaluation
+    `maximize` : bool, default=True
+        Whether to optimize in a way of maximizing certain metric
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset
+    `fold_type` : FoldType, default=KFold
+        Fold type (pass the class itself, not its instance)
+    `refit` : bool, default=True
+        Whether to re-fit the estimator with the best parameters found
+    `random_state` : int, optional, default=None
+        Seed for random sampling for cross validation
 
     Properties
     ----------
     Get the best(optimized) estimator:
         ```py
         @property
         def best_model(self) -> Estimator
         ```
-
     Notes
     -----
     * An instance of the estimator must be passed to `estimator`
     * For `metric`, both class or instance are possible
     * Only `Pipeline` is allowed for meta estimator
 
     Examples
@@ -70,20 +78,20 @@
     """
 
     def __init__(
         self,
         estimator: Estimator,
         param_grid: dict,
         cv: int = 5,
-        metric: Evaluator = None,
+        metric: Evaluator | None = None,
         maximize: bool = True,
         refit: bool = True,
         shuffle: bool = True,
         fold_type: FoldType = KFold,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ) -> None:
         self.estimator = estimator
         self.param_grid = param_grid
         self.cv = cv
         self.metric = metric
         self.maximize = maximize
@@ -185,74 +193,85 @@
     the best combination. This process is performed using cross-validation to
     ensure model performance is not biased to a specific data split. The result
     is the optimal set of parameters that yield the best model performance
     according to a chosen metric.
 
     Parameters
     ----------
-    `estimator` : An estimator to fit and evaluate
-    `param_dist` : Parameter distributions for random search
-    `max_iter` : Number of parameter settings that are sampled
-    `cv` : K-fold size for cross-validation
-    `metric` : Scoring metric for evaluation
-    `maximize` : Whether to optimize in a way of maximizing certain metric
-    `refit` : Whether to re-fit the estimator with the best parameters found
-    `shuffle` : Whether to shuffle the dataset
-    `fold_type` : Fold type (Default `KFold`)
-    `random_state` : Seed for random sampling for cross-validation and random search
-    `verbose` : Whether to print progress messages
+    `estimator` : Estimator
+        An estimator to fit and evaluate
+    `param_dist` : dict[str, Vector | DT]
+        Parameter distributions for random search
+    `max_iter` : int, default=100
+        Number of parameter settings that are sampled
+    `cv` : int, default=5
+        K-fold size for cross-validation
+    `metric` : Evaluator, optional, default=None
+        Scoring metric for evaluation
+    `maximize` : bool, default=True
+        Whether to optimize in a way of maximizing certain metric
+    `refit` : bool, default=True
+        Whether to re-fit the estimator with the best parameters found
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset
+    `fold_type` : FoldType, default=KFold
+        Fold type
+    `random_state` : int, optional, default=None
+        Seed for random sampling for cross-validation and random search
 
     Properties
     ----------
     Get the best(optimized) estimator:
         ```py
         @property
         def best_model(self) -> Estimator
         ```
-
     Notes
     -----
-    * An instance of the estimator must be passed to `estimator`
-    * For `metric`, both class or instance are possible
-    * Only `Pipeline` is allowed for meta estimator
-    * Type `DT` is a generic type for `scipy`'s distribution types
+    - An instance of the estimator must be passed to `estimator`
+    - For `metric`, both class or instance are possible
+    - Only `Pipeline` is allowed for meta estimator
+    - Type `DT` is a generic type for `scipy`'s distribution types
         (e.g. `rv_continuous`, `rv_discrete`)
 
     Examples
     --------
-    >>> param_dist = {'param_1': [...],
-                      'param_2': [...],
-                      ...,
-                      AnyStr: Vector | DT }
-
-    >>> rand = RandomizedSearchCV(estimator=AnyEstimator(),
-                                  param_dist=param_dist,
-                                  max_iter=100,
-                                  cv=5,
-                                  metric=AnyEvaluator,
-                                  refit=True,
-                                  random_state=None)
+    >>> param_dist = {
+            'param_1': [...],
+            'param_2': [...],
+            ...,
+            AnyStr: Vector | DT,
+        }
+    >>> rand = RandomizedSearchCV(
+            estimator=AnyEstimator(),
+            param_dist=param_dist,
+            max_iter=100,
+            cv=5,
+            metric=AnyEvaluator,
+            refit=True,
+            random_state=None,
+        )
     >>> rand.fit(X, y)
     >>> score = rand.best_score
     >>> model = rand.best_model
 
     """
 
     def __init__(
         self,
         estimator: Estimator,
         param_dist: Dict[str, Vector | DT],
         max_iter: int = 100,
         cv: int = 5,
-        metric: Evaluator = None,
+        metric: Evaluator | None = None,
         maximize: bool = True,
         refit: bool = True,
         shuffle: bool = True,
         fold_type: FoldType = KFold,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ) -> None:
         self.estimator = estimator
         self.param_dist = param_dist
         self.max_iter = max_iter
         self.cv = cv
         self.metric = metric
```

### Comparing `luma-ml-0.7.5/luma/model_selection/split.py` & `luma-ml-0.8.0/luma/model_selection/split.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,24 +9,35 @@
 
 class TrainTestSplit:
     """
     Splits the original dataset into the train set and the test set.
 
     Parameters
     ----------
-    `X` : Feature data
-    `y` : Target data (as a 1-D `Vector`)
-    `test_size` : Proportional size of the test set (e.g. `0.2`, `0.3`)
-    `shuffle` : Whether to shuffle the dataset
-    `stratify` : Whether to perform stratified split (Default `False`)
-    `random_state` : Seed for random sampling for split
+    `X` : Matrix
+        Feature data
+    `y` : Vector
+        Target data
+    `test_size` : int or float, default=0.3
+        Proportional size of the test set
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset
+    `stratify` : bool, default=False
+        Whether to perform stratified split
+    `random_state` : int, optional, default=None
+        Seed for random sampling for split
 
     Properties
     ----------
-    `get` : Returns the split data as a 4-tuple
+    `get` : tuple[Matrix, Matrix, Vector, Vector]
+        Returns the split data as a 4-tuple
+
+    Notes
+    -----
+    For `stratify == True`, one-hot encoded `y` is not compatible.
 
     Examples
     --------
     ```py
     X_train, X_test, y_train, y_test = TrainTestSplit(X, y, ...).get
     ```
     """
@@ -118,19 +129,30 @@
 class BatchGenerator:
     """
     A class for generating mini-batches of data for training machine
     learning models including neural networks.
 
     Parameters
     ----------
-    `X` : Input features
-    `y` : Targets or labels
-    `batch_size` : Size of a mini-batch
-    `shuffle` : Whether to shuffle the data for every batch generation
+    `X` : TensorLike
+        Input features
+    `y` : TensorLike
+        Targets or labels
+    `batch_size` : int, default=100
+        Size of a mini-batch
+    `shuffle` : bool, default=True
+        Whether to shuffle the data for every batch generation
 
+    Iterator
+    --------
+    The iterator of `BatchGenerator` returns a 2-tuple of
+    `TensorLike` objects.
+    ```py
+    def __iter__(self) -> Iterator[Tuple[TensorLike, TensorLike]]
+    ```
     Examples
     --------
     An instance of `BatchGenerator` can be used as an iterator.
 
     - With instantiation:
 
         ```py
```

### Comparing `luma-ml-0.7.5/luma/neural/_layers/_act.py` & `luma-ml-0.8.0/luma/neural/_layers/_act.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/_layers/_conv.py` & `luma-ml-0.8.0/luma/neural/_layers/_conv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/_layers/_drop.py` & `luma-ml-0.8.0/luma/neural/_layers/_drop.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/_layers/_linear.py` & `luma-ml-0.8.0/luma/neural/_layers/_linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/_layers/_norm.py` & `luma-ml-0.8.0/luma/neural/_layers/_norm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/_layers/_pool.py` & `luma-ml-0.8.0/luma/neural/_layers/_pool.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/_models/_imagenet.py` & `luma-ml-0.8.0/luma/neural/_models/_imagenet.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/_models/_lenet.py` & `luma-ml-0.8.0/luma/neural/_models/_lenet.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/_models/_simple.py` & `luma-ml-0.8.0/luma/neural/_models/_simple.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/base.py` & `luma-ml-0.8.0/luma/neural/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,28 +22,53 @@
     Neural network layers are composed of interconnected nodes,
     each performing computations on input data. Common types include
     fully connected, convolutional, and recurrent layers, each
     serving distinct roles in learning from data.
 
     Attributes
     ----------
-    - `weights_` : Weight tensor
-    - `biases_` : Bias tensor
-    - `dX` : Gradient w.r.t. the input
-    - `dW` : Gradient w.r.t. the weights
-    - `dB` : Gradient w.r.t. the biases
-    - `optimizer` : Optimizer for certain layer
-    - `out_shape` : Shape of the output when forwarding
+    `weights_` : TensorLike
+        Weight tensor
+    `biases_` : TensorLike
+        Bias tensor
+    `dX` : TensorLike
+        Gradient w.r.t. the input
+    `dW` : TensorLike
+        Gradient w.r.t. the weights
+    `dB` : TensorLike
+        Gradient w.r.t. the biases
+    `optimizer` : object (possibly Optimizer)
+        Optimizer for certain layer
 
     Properties
     ----------
     To get its parameter size (weights, biases):
     ```py
     (property) param_size: Tuple[int, int]
     ```
+    Methods
+    -------
+    - To feed-forward a layer:
+
+        ```py
+        @abstractmethod
+        def forward(self, X: TensorLike, ...) -> TensorLike
+        ```
+    - To perform backward pass:
+
+        ```py
+        @abstractmethod
+        def backward(self, d_out: TensorLike, ...) -> TensorLike
+        ```
+    - To get an output shape:
+
+        ```py
+        @abstractmethod
+        def out_shape(self, in_shape: tuple[int]) -> tuple[int]
+        ```
     """
 
     def __init__(self) -> None:
         self.input_: TensorLike = None
         self.output_: TensorLike = None
 
         self.weights_: TensorLike = None
@@ -142,15 +167,15 @@
     This class provides a structured way to implement weight
     initialization methods for different types of layers in a
     neural network.
     The class must be inherited by specific initializer implementations
     that define methods for 2D and 4D weight tensors.
     """
 
-    def __init__(self, random_state: int) -> None:
+    def __init__(self, random_state: int | None) -> None:
         self.rs_ = np.random.RandomState(random_state)
 
     @classmethod
     def __class_alias__(cls) -> None: ...
 
     @abstractmethod
     def init_nd(self) -> TensorLike: ...
@@ -159,14 +184,50 @@
 class NeuralModel(ABC, NeuralBase):
     """
     Neural networks are computational models inspired by the human brain,
     consisting of layers of interconnected nodes (neurons) that process
     information through weighted connections. These models include an input
     layer to receive data, hidden layers that perform computations, and an
     output layer to deliver results.
+
+    Parameters
+    ----------
+    `batch_size` : int
+        Size of a single mini-batch
+    `n_epochs` : int
+        Number of epochs for training
+    `learning_rate` : float
+        Step size during optimization process
+    `valid_size` : float, range=[0,1]
+        Fractional size of validation set
+    `early_stopping` : bool
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int
+        Number of epochs to wait until early-stopping
+    `deep_verbose` : bool
+        Whether to log deeply (for all the batches)
+
+    Methods
+    -------
+    - To initialize fundamental attributes of a neural model(mandatory):
+
+        ```py
+        def __init_model__(self) -> None:
+        ```
+    - To construct a neural model(mandatory):
+
+        ```py
+        @abstractmethod
+        def _build_model(self) -> None
+        ```
+    - To summarize a neural model:
+
+        ```py
+        def summarize(self, in_shape: tuple[int]) -> None
+        ```
     """
 
     def __init__(
         self,
         batch_size: int,
         n_epochs: int,
         learning_rate: float,
```

### Comparing `luma-ml-0.7.5/luma/neural/block.py` & `luma-ml-0.8.0/luma/neural/block.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,29 +31,44 @@
     Structure
     ---------
     ```py
     Convolution1D -> Optional[BatchNorm1D] -> Activation -> Optional[Pooling1D]
     ```
     Parameters
     ----------
-    `in_channels` : Number of input channels
-    `out_channels` : Number of output channels
-    `filter_size` : Size of the convolution filter
-    `activation` : Type of activation function
-    `padding` : Padding method
-    `optimizer` : Type of optimizer for weight updating
-    `initializer` : Type of weight initializer
-    `stride` : Step size for filters during convolution
-    `lambda_` : L2 regularization strength
-    `do_batch_norm` : Whether to perform batch normalization (default `True`)
-    `momentum` : Momentum for batch normalization
-    `do_pooling` : Whether to perform pooling (default `True`)
-    `pool_filter_size` : Filter size for pooling
-    `pool_stride` : Step size for pooling process
-    `pool_mode` : Pooling strategy
+    `in_channels` : int
+        Number of input channels
+    `out_channels` : int
+        Number of output channels
+    `filter_size` : int
+        Size of the convolution filter
+    `activation` : FuncType
+        Type of activation function
+    `padding` : {"same", "valid"}, default="same"
+        Padding method
+    `optimizer` : Optimizer, optional, default=None
+        Type of optimizer for weight updating
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `stride` : int, default=1
+        Step size for filters during convolution
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `do_batch_norm` : bool, default=True
+        Whether to perform batch normalization
+    `momentum` : float, default=0.9
+        Momentum for batch normalization
+    `do_pooling` : bool, default=True
+        Whether to perform pooling
+    `pool_filter_size` : int, default=2
+        Filter size for pooling
+    `pool_stride` : int, default=2
+        Step size for pooling process
+    `pool_mode` : {"max", "avg"}, default="max"
+        Pooling strategy
 
     Notes
     -----
     - The input `X` must have the form of 3D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, width)
@@ -62,15 +77,15 @@
 
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         filter_size: int,
         activation: Activation.FuncType,
-        optimizer: Optimizer = None,
+        optimizer: Optimizer | None = None,
         initializer: InitUtil.InitStr = None,
         padding: Literal["same", "valid"] = "same",
         stride: int = 1,
         lambda_: float = 0.0,
         do_batch_norm: bool = True,
         momentum: float = 0.9,
         do_pooling: bool = True,
@@ -141,29 +156,44 @@
     Structure
     ---------
     ```py
     Convolution2D -> Optional[BatchNorm2D] -> Activation -> Optional[Pooling2D]
     ```
     Parameters
     ----------
-    `in_channels` : Number of input channels
-    `out_channels` : Number of output channels
-    `filter_size` : Size of the convolution filter
-    `activation` : Type of activation function
-    `padding` : Padding method
-    `optimizer` : Type of optimizer for weight updating
-    `initializer` : Type of weight initializer
-    `stride` : Step size for filters during convolution
-    `lambda_` : L2 regularization strength
-    `do_batch_norm` : Whether to perform batch normalization (default `True`)
-    `momentum` : Momentum for batch normalization
-    `do_pooling` : Whether to perform pooling (default `True`)
-    `pool_filter_size` : Filter size for pooling
-    `pool_stride` : Step size for pooling process
-    `pool_mode` : Pooling strategy
+    `in_channels` : int
+        Number of input channels
+    `out_channels` : int
+        Number of output channels
+    `filter_size` : int
+        Size of the convolution filter
+    `activation` : FuncType
+        Type of activation function
+    `padding` : {"same", "valid"}, default="same"
+        Padding method
+    `optimizer` : Optimizer, optional, default=None
+        Type of optimizer for weight updating
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `stride` : int, default=1
+        Step size for filters during convolution
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `do_batch_norm` : bool, default=True
+        Whether to perform batch normalization
+    `momentum` : float, default=0.9
+        Momentum for batch normalization
+    `do_pooling` : bool, default=True
+        Whether to perform pooling
+    `pool_filter_size` : int, default=2
+        Filter size for pooling
+    `pool_stride` : int, default=2
+        Step size for pooling process
+    `pool_mode` : {"max", "avg"}, default="max"
+        Pooling strategy
 
     Notes
     -----
     - The input `X` must have the form of 4D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, height, width)
@@ -172,15 +202,15 @@
 
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         filter_size: int,
         activation: Activation.FuncType,
-        optimizer: Optimizer = None,
+        optimizer: Optimizer | None = None,
         initializer: InitUtil.InitStr = None,
         padding: Literal["same", "valid"] = "same",
         stride: int = 1,
         lambda_: float = 0.0,
         do_batch_norm: bool = True,
         momentum: float = 0.9,
         do_pooling: bool = True,
@@ -251,29 +281,44 @@
     Structure
     ---------
     ```py
     Convolution3D -> Optional[BatchNorm3D] -> Activation -> Optional[Pooling3D]
     ```
     Parameters
     ----------
-    `in_channels` : Number of input channels
-    `out_channels` : Number of output channels
-    `filter_size` : Size of the convolution filter
-    `activation` : Type of activation function
-    `padding` : Padding method
-    `optimizer` : Type of optimizer for weight updating
-    `initializer` : Type of weight initializer
-    `stride` : Step size for filters during convolution
-    `lambda_` : L2 regularization strength
-    `do_batch_norm` : Whether to perform batch normalization (default `True`)
-    `momentum` : Momentum for batch normalization
-    `do_pooling` : Whether to perform pooling (default `True`)
-    `pool_filter_size` : Filter size for pooling
-    `pool_stride` : Step size for pooling process
-    `pool_mode` : Pooling strategy
+    `in_channels` : int
+        Number of input channels
+    `out_channels` : int
+        Number of output channels
+    `filter_size` : int
+        Size of the convolution filter
+    `activation` : FuncType
+        Type of activation function
+    `padding` : {"same", "valid"}, default="same"
+        Padding method
+    `optimizer` : Optimizer, optional, default=None
+        Type of optimizer for weight updating
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `stride` : int, default=1
+        Step size for filters during convolution
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `do_batch_norm` : bool, default=True
+        Whether to perform batch normalization
+    `momentum` : float, default=0.9
+        Momentum for batch normalization
+    `do_pooling` : bool, default=True
+        Whether to perform pooling
+    `pool_filter_size` : int, default=2
+        Filter size for pooling
+    `pool_stride` : int, default=2
+        Step size for pooling process
+    `pool_mode` : {"max", "avg"}, default="max"
+        Pooling strategy
 
     Notes
     -----
     - The input `X` must have the form of 5D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, depth, height, width)
@@ -282,15 +327,15 @@
 
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         filter_size: int,
         activation: Activation.FuncType,
-        optimizer: Optimizer = None,
+        optimizer: Optimizer | None = None,
         initializer: InitUtil.InitStr = None,
         padding: Literal["same", "valid"] = "same",
         stride: int = 1,
         lambda_: float = 0.0,
         do_batch_norm: bool = True,
         momentum: float = 0.9,
         do_pooling: bool = True,
@@ -361,24 +406,34 @@
     Structure
     ---------
     ```py
     Dense -> Optional[BatchNorm1D] -> Activation -> Optional[Dropout]
     ```
     Parameters
     ----------
-    `in_features` : Number of input features
-    `out_features` : Number of output features
-    `activation` : Type of activation function
-    `optimizer` : Type of optimizer for weight update
-    `initializer` : Type of weight initializer
-    `lambda_` : L2 regularization strength
-    `do_batch_norm` : Whether to perform batch normalization (default `True`)
-    `momentum` : Momentum for batch normalization
-    `do_dropout` : Whethter to perform dropout (default `True`)
-    `dropout_rate` : Dropout rate
+    `in_features` : int
+        Number of input features
+    `out_features` : int
+        Number of output features
+    `activation` : FuncType
+        Type of activation function
+    `optimizer` : Optimizer, optional, default=None
+        Type of optimizer for weight update
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `do_batch_norm` : bool, default=True
+        Whether to perform batch normalization
+    `momentum` : float, default=0.9
+        Momentum for batch normalization
+    `do_dropout` : bool, default=True
+        Whethter to perform dropout
+    `dropout_rate` : float, default=0.5
+        Dropout rate
 
     """
 
     def __init__(
         self,
         in_features: int,
         out_features: int,
```

### Comparing `luma-ml-0.7.5/luma/neural/init.py` & `luma-ml-0.8.0/luma/neural/init.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/layer.py` & `luma-ml-0.8.0/luma/neural/layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,24 +43,32 @@
     across input data, detecting patterns like edges or textures, producing
     feature maps essential for tasks such as image recognition within CNNs.
     By sharing parameters, it efficiently extracts hierarchical representations,
     enabling the network to learn complex visual features.
 
     Parameters
     ----------
-    `in_channels` : Number of input channels
-    `out_channels` : Number of output channels (filters)
-    `filter_size`: Length of each filter
-    `stride` : Step size for filters during convolution
-    `padding` : Padding strategies
-    (`valid` for no padding, `same` for zero-padding)
-    `initializer` : Type of weight initializer (default `None`)
-    `optimizer` : Optimizer for weight update (default `SGDOptimizer`)
-    `lambda_` : L2-regularization strength
-    `random_state` : Seed for various random sampling processes
+    `in_channels` : int
+        Number of input channels
+    `out_channels` : int
+        Number of output channels(filters)
+    `filter_size`: int
+        Length of each filter
+    `stride` : int, default=1
+        Step size for filters during convolution
+    `padding` : {"valid", "same"}, default="same"
+        Padding strategies ("valid" for no padding, "same" for zero-padding)
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `optimizer` : Optimizer, optional, default=None
+        Optimizer for weight update
+    `lambda_` : float, default=0.0
+        L2-regularization strength
+    `random_state` : int, optional, default=None
+        Seed for various random sampling processes
 
     Notes
     -----
     - The input `X` must have the form of 3D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, width)
@@ -71,17 +79,17 @@
         self,
         in_channels: int,
         out_channels: int,
         filter_size: int,
         stride: int = 1,
         padding: Literal["valid", "same"] = "same",
         initializer: InitUtil.InitStr = None,
-        optimizer: Optimizer = None,
+        optimizer: Optimizer | None = None,
         lambda_: float = 0,
-        random_state: int = None,
+        random_state: int | None = None,
     ) -> None:
         super().__init__(
             in_channels,
             out_channels,
             filter_size,
             stride,
             padding,
@@ -100,24 +108,32 @@
     across input data, detecting patterns like edges or textures, producing
     feature maps essential for tasks such as image recognition within CNNs.
     By sharing parameters, it efficiently extracts hierarchical representations,
     enabling the network to learn complex visual features.
 
     Parameters
     ----------
-    `in_channels` : Number of input channels
-    `out_channels` : Number of output channels(filters)
-    `filter_size`: Size of each filter
-    `stride` : Step size for filters during convolution
-    `padding` : Padding stratagies
-    (`valid` for no padding, `same` for typical 0-padding)
-    `initializer` : Type of weight initializer (default `None`)
-    `optimizer` : Optimizer for weight update (default `SGDOptimizer`)
-    `lambda_` : L2-regularization strength
-    `random_state` : Seed for various random sampling processes
+    `in_channels` : int
+        Number of input channels
+    `out_channels` : int
+        Number of output channels(filters)
+    `filter_size`: int
+        Length of each filter
+    `stride` : int, default=1
+        Step size for filters during convolution
+    `padding` : {"valid", "same"}, default="same"
+        Padding strategies ("valid" for no padding, "same" for zero-padding)
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `optimizer` : Optimizer, optional, default=None
+        Optimizer for weight update
+    `lambda_` : float, default=0.0
+        L2-regularization strength
+    `random_state` : int, optional, default=None
+        Seed for various random sampling processes
 
     Notes
     -----
     - The input `X` must have the form of 4D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, height, width)
@@ -157,24 +173,32 @@
     across input data, detecting patterns like edges or textures, producing
     feature maps essential for tasks such as image recognition within CNNs.
     By sharing parameters, it efficiently extracts hierarchical representations,
     enabling the network to learn complex visual features.
 
     Parameters
     ----------
-    `in_channels` : Number of input channels
-    `out_channels` : Number of output channels(filters)
-    `filter_size`: Size of each filter
-    `stride` : Step size for filters during convolution
-    `padding` : Padding stratagies
-    (`valid` for no padding, `same` for typical 0-padding)
-    `initializer` : Type of weight initializer (default `None`)
-    `optimizer` : Optimizer for weight update (default `SGDOptimizer`)
-    `lambda_` : L2-regularization strength
-    `random_state` : Seed for various random sampling processes
+    `in_channels` : int
+        Number of input channels
+    `out_channels` : int
+        Number of output channels(filters)
+    `filter_size`: int
+        Length of each filter
+    `stride` : int, default=1
+        Step size for filters during convolution
+    `padding` : {"valid", "same"}, default="same"
+        Padding strategies ("valid" for no padding, "same" for zero-padding)
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `optimizer` : Optimizer, optional, default=None
+        Optimizer for weight update
+    `lambda_` : float, default=0.0
+        L2-regularization strength
+    `random_state` : int, optional, default=None
+        Seed for various random sampling processes
 
     Notes
     -----
     - The input `X` must have the form of 5D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, depth, height, width)
@@ -216,17 +240,20 @@
     to extract dominant features. Pooling helps in achieving translation invariance
     and reducing overfitting by summarizing the presence of features in local
     regions. It downsamples feature maps, preserving important information while
     discarding redundant details.
 
     Parameters
     ----------
-    `filter_size` : Size of the pooling filter
-    `stride` : Step size of the filter during pooling
-    `mode` : Pooling strategy (i.e., 'max' or 'avg')
+    `filter_size` : int, default=2
+        Size of the pooling filter
+    `stride` : int, default=2
+        Step size of the filter during pooling
+    `mode` : {"max", "avg"}, default="max"
+        Pooling strategy (i.e., 'max' or 'avg')
 
     Notes
     -----
     - The input `X` must have the form of 3D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, width)
@@ -252,17 +279,20 @@
     to extract dominant features. Pooling helps in achieving translation invariance
     and reducing overfitting by summarizing the presence of features in local
     regions. It downsamples feature maps, preserving important information while
     discarding redundant details.
 
     Parameters
     ----------
-    `size` : Size of pooling filter
-    `stride` : Step size of filter during pooling
-    `mode` : Pooling strategy (i.e. max, average)
+    `filter_size` : int, default=2
+        Size of the pooling filter
+    `stride` : int, default=2
+        Step size of the filter during pooling
+    `mode` : {"max", "avg"}, default="max"
+        Pooling strategy (i.e., 'max' or 'avg')
 
     Notes
     -----
     - The input `X` must have the form of 4D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, height, width)
@@ -288,17 +318,20 @@
     to extract dominant features. Pooling helps in achieving translation invariance
     and reducing overfitting by summarizing the presence of features in local
     regions. It downsamples feature maps, preserving important information while
     discarding redundant details.
 
     Parameters
     ----------
-    `filter_size` : Size of the pooling filter (cubic)
-    `stride` : Step size of the filter during pooling
-    `mode` : Pooling strategy (i.e., 'max' or 'avg')
+    `filter_size` : int, default=2
+        Size of the pooling filter
+    `stride` : int, default=2
+        Step size of the filter during pooling
+    `mode` : {"max", "avg"}, default="max"
+        Pooling strategy (i.e., 'max' or 'avg')
 
     Notes
     -----
     - The input `X` must have the form of 5D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, depth, height, width)
@@ -322,20 +355,26 @@
     enabling complex relationships between input and output. Dense layers
     are fundamental in deep learning models for learning representations from
     data. They play a crucial role in capturing intricate patterns and
     features during the training process.
 
     Parameters
     ----------
-    `in_features` : Number of input features
-    `out_features`:  Number of output features
-    `initializer` : Type of weight initializer (default `None`)
-    `optimizer` : Optimizer for weight update
-    `lambda_` : L2-regularization strength
-    `random_state` : Seed for various random sampling processes
+    `in_features` : int
+        Number of input features
+    `out_features`:  int
+        Number of output features
+    `initializer` : InitStr, default = None
+        Type of weight initializer
+    `optimizer` : Optimizer, optional, default=None
+        Optimizer for weight update
+    `lambda_` : float, default=0.0
+        L2-regularization strength
+    `random_state` : int, optional, default=None
+        Seed for various random sampling processes
 
     Notes
     -----
     - The input `X` must have the form of 2D-array(`Matrix`).
 
         ```py
         X.shape = (batch_size, n_features)
@@ -343,17 +382,17 @@
     """
 
     def __init__(
         self,
         in_features: int,
         out_features: int,
         initializer: InitUtil.InitStr = None,
-        optimizer: Optimizer = None,
+        optimizer: Optimizer | None = None,
         lambda_: float = 0,
-        random_state: int = None,
+        random_state: int | None = None,
     ) -> None:
         super().__init__(
             in_features,
             out_features,
             initializer,
             optimizer,
             lambda_,
@@ -366,25 +405,29 @@
     Dropout is a regularization technique used during training to prevent
     overfitting by randomly setting a fraction of input units to zero during
     the forward pass. This helps in reducing co-adaptation of neurons and
     encourages the network to learn more robust features.
 
     Parameters
     ----------
-    `dropout_rate` : The fraction of input units to drop during training
-    `random_state` : Seed for various random sampling processes
+    `dropout_rate` : float, default=0.5
+        The fraction of input units to drop during training
+    `random_state` : int, optional, default=None
+        Seed for various random sampling processes
 
     Notes
     -----
     - During inference, dropout is typically turned off, and the layer behaves
       as the identity function.
 
     """
 
-    def __init__(self, dropout_rate: float = 0.5, random_state: int = None) -> None:
+    def __init__(
+        self, dropout_rate: float = 0.5, random_state: int | None = None
+    ) -> None:
         super().__init__(dropout_rate, random_state)
 
 
 class Flatten(_linear._Flatten):
     """
     A flatten layer reshapes the input tensor into a 2D array(`Matrix`),
     collapsing all dimensions except the batch dimension.
@@ -430,16 +473,18 @@
     Batch normalization standardizes layer inputs across mini-batches to stabilize
     learning, accelerate convergence, and reduce sensitivity to initialization.
     It adjusts normalized outputs using learnable parameters, mitigating internal
     covariate shift in deep networks.
 
     Parameters
     ----------
-    `in_features` : Number of input features
-    `momentum` : Momentum for updating the running averages
+    `in_features` : int
+        Number of input features
+    `momentum` : float, default=0.9
+        Momentum for updating the running averages
 
     Notes
     -----
     - The input `X` must have the form of 3D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, width)
@@ -459,16 +504,18 @@
     Batch normalization standardizes layer inputs across mini-batches to stabilize
     learning, accelerate convergence, and reduce sensitivity to initialization.
     It adjusts normalized outputs using learnable parameters, mitigating internal
     covariate shift in deep networks.
 
     Parameters
     ----------
-    `in_features` : Number of input features
-    `momentum` : Momentum for updating the running averages
+    `in_features` : int
+        Number of input features
+    `momentum` : float, default=0.9
+        Momentum for updating the running averages
 
     Notes
     -----
     - The input `X` must have the form of 4D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, height, width)
@@ -488,16 +535,18 @@
     Batch normalization standardizes layer inputs across mini-batches to stabilize
     learning, accelerate convergence, and reduce sensitivity to initialization.
     It adjusts normalized outputs using learnable parameters, mitigating internal
     covariate shift in deep networks.
 
     Parameters
     ----------
-    `in_features` : Number of input features
-    `momentum` : Momentum for updating the running averages
+    `in_features` : int
+        Number of input features
+    `momentum` : float, default=0.9
+        Momentum for updating the running averages
 
     Notes
     -----
     - The input `X` must have the form of 5D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, depth, height, width)
@@ -516,18 +565,22 @@
     to promote competition among neighboring feature maps. By normalizing the
     activities in local regions across channels, LRN helps to enhance generalization
     by suppressing activations that are uniformly large across the entire map and
     boosting those that are uniquely larger in a local neighborhood.
 
     Parameters
     ----------
-    `depth` : Number of adjacent channels to normalize across
-    `alpha` : Scaling parameter for the squared sum
-    `beta` : Exponent for the normalization
-    `k` : Offset to avoid division by zero
+    `depth` : int
+        Number of adjacent channels to normalize across
+    `alpha` : float, default=1e-4
+        Scaling parameter for the squared sum
+    `beta` : float, default=0.75
+        Exponent for the normalization
+    `k` : float, default=2
+        Offset to avoid division by zero
 
     Notes
     -----
     - The input `X` must have the form of >=3D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, *spatial)
@@ -554,42 +607,48 @@
     Layer normalization is a technique used in neural networks to normalize the
     inputs across the features for each data sample in a batch independently.
     It stabilizes the learning process by reducing the variance of the inputs
     within a layer, helping to speed up training and improve performance.
 
     Parameters
     ----------
-    `in_shape` : Shape of the input
+    `in_shape` : int or tuple of int
+        Shape of the input
 
     Notes
     -----
     - The input `X` must have the form of >=2D-array(`Matrix`).
 
         ```py
         X.shape = (batch_size, *spatial)
         ```
     """
 
-    def __init__(self, in_shape: Tuple[int] | int, epsilon: float = 1e-5) -> None:
+    def __init__(
+        self,
+        in_shape: Tuple[int] | int,
+        epsilon: float = 1e-5,
+    ) -> None:
         super().__init__(in_shape, epsilon)
 
 
 class Sequential(Layer):
     """
     Sequential represents a linear arrangement of layers in a neural network
     model. Each layer is added sequentially, with data flowing from one layer
     to the next in the order they are added. This organization simplifies the
     construction of neural networks, especially for straightforward architectures,
     by mirroring the logical flow of data from input through hidden layers to
     output.
 
     Parameters
     ----------
-    `*layers` : Layers or layers with its name assigned
-    (class name of the layer assigned by default)
+    `*layers` : Layer or tuple[str, Layer]
+        Layers or layers with its name assigned
+        (class name of the layer assigned by default)
 
     Methods
     -------
     For setting an optimizer of each layer:
     ```py
     def set_optimizer(self, optimizer: Optimizer) -> None
     ```
```

### Comparing `luma-ml-0.7.5/luma/neural/loss.py` & `luma-ml-0.8.0/luma/neural/loss.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/network.py` & `luma-ml-0.8.0/luma/neural/network.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,32 +36,46 @@
     Structure
     ---------
     ```py
     (Dense -> Activation -> Dropout) -> ... -> Dense
     ```
     Parameters
     ----------
-    `in_features` : Number of input features
-    `out_features` : Number of output features
-    `hidden_layers` : Numbers of the features in hidden layers
-    (`int` for a single layer)
-    `batch_size` : Size of a single mini-batch
-    `n_epochs` : Number of epochs for training
-    `learning_rate` : Step size during optimization process
-    `valid_size` : Fractional size of validation set
-    `initializer` : Type of weight initializer
-    `activation` : Type of activation function
-    `optimizer` : An optimizer used in weight update process
-    `loss` : Type of loss function
-    `dropout_rate` : Dropout rate
-    `lambda_` : L2 regularization strength
-    `early_stopping` : Whether to early-stop the training when the valid
-    score stagnates
-    `patience` : Number of epochs to wait until early-stopping
-    `shuffle` : Whethter to shuffle the data at the beginning of every epoch
+    `in_features` : int
+        Number of input features
+    `out_features` : int
+        Number of output features
+    `hidden_layers` : int of list of int
+        Numbers of the features in hidden layers (int for a single layer)
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.001
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `activation` : FuncType
+        Type of activation function
+    `optimizer` : Optimizer
+        An optimizer used in weight update process
+    `loss` : Loss
+        Type of loss function
+    `dropout_rate` : float, default=0.5
+        Dropout rate
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
 
     Notes
     -----
     - If the data or the target is a 1D-Array(`Vector`), reshape it into a
         higher dimensional array.
 
     - For classification tasks, the target vector `y` must be
@@ -71,28 +85,28 @@
 
     def __init__(
         self,
         in_features: int,
         out_features: int,
         hidden_layers: list[int] | int,
         *,
-        activation: Activation,
+        activation: Activation.FuncType,
         optimizer: Optimizer,
         loss: Loss,
         initializer: InitUtil.InitStr = None,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.001,
         valid_size: float = 0.1,
         dropout_rate: float = 0.5,
         lambda_: float = 0,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         deep_verbose: bool = False
     ) -> None:
         super().__init__(
             in_features,
             out_features,
             hidden_layers,
             activation,
@@ -127,42 +141,68 @@
     Structure
     ---------
     ```py
     ConvBlock2D -> ... -> Flatten -> DenseBlock -> ... -> Dense
     ```
     Parameters
     ----------
-    `in_channels_list` : List of input channels for convolutional blocks
-    `in_features_list` : List of input features for dense blocks
-    `out_channels` : Output channels for the last convolutional layer
-    `out_features` : Output features for the last dense layer
-    `filter_size` : Size of filters for convolution layers
-    `activation` : Type of activation function
-    `optimizer` : Type of optimizer for weight update
-    `loss` : Type of loss function
-    `initializer` : Type of weight initializer (`None` for dense layers)
-    `padding` : Padding strategy (default `same`)
-    `stride` : Step size of filters during convolution
-    `do_batch_norm` : Whether to perform batch normalization (default `True`)
-    `momentum` : Momentum for batch normalization
-    `do_pooling` : Whether to perform pooling
-    `pool_filter_size` : Size of filters for pooling layers
-    `pool_stride` : Step size of filters during pooling
-    `pool_mode` : Pooling strategy (default `max`)
-    `do_dropout` : Whether to perform dropout
-    `dropout_rate` : Dropout rate
-    `batch_size` : Size of a single mini-batch
-    `n_epochs` : Number of epochs for training
-    `learning_rate` : Step size during optimization process
-    `valid_size` : Fractional size of validation set
-    `lambda_` : L2 regularization strength
-    `early_stopping` : Whether to early-stop the training when the valid
-    score stagnates
-    `patience` : Number of epochs to wait until early-stopping
-    `shuffle` : Whethter to shuffle the data at the beginning of every epoch
+    `in_channels_list` : int or list of int
+        List of input channels for convolutional blocks
+    `in_features_list` : int or list of int
+        List of input features for dense blocks
+    `out_channels` : int
+        Output channels for the last convolutional layer
+    `out_features` : int
+        Output features for the last dense layer
+    `filter_size` : int
+        Size of filters for convolution layers
+    `activation` : FuncType
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer (None for dense layers)
+    `padding` : {"same", "valid"}, default="same"
+        Padding strategy
+    `stride` : int, default=1
+        Step size of filters during convolution
+    `do_batch_norm` : bool, default=True
+        Whether to perform batch normalization
+    `momentum` : float, default=0.9
+        Momentum for batch normalization
+    `do_pooling` : bool, default=True
+        Whether to perform pooling
+    `pool_filter_size` : int, default=2
+        Size of filters for pooling layers
+    `pool_stride` : int, default=2
+        Step size of filters during pooling
+    `pool_mode` : {"max", "avg"}, default="max"
+        Pooling strategy (default `max`)
+    `do_dropout` : bool, default=True
+        Whether to perform dropout
+    `dropout_rate` : float, default=0.5
+        Dropout rate
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.001
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
 
     Notes
     -----
     - Input `X` must have the shape of 4D-array(`Tensor`)
 
     - For classification tasks, the target vector `y` must be
         one-hot encoded.
@@ -204,15 +244,15 @@
         self,
         in_channels_list: list[int] | int,
         in_features_list: list[int] | int,
         out_channels: int,
         out_features: int,
         *,
         filter_size: int,
-        activation: Activation,
+        activation: Activation.FuncType,
         optimizer: Optimizer,
         loss: Loss,
         initializer: InitUtil.InitStr = None,
         padding: Literal["same", "valid"] = "same",
         stride: int = 1,
         do_batch_norm: bool = True,
         momentum: float = 0.9,
@@ -226,15 +266,15 @@
         n_epochs: int = 100,
         learning_rate: float = 0.001,
         valid_size: float = 0.1,
         lambda_: float = 0,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         deep_verbose: bool = False
     ) -> None:
         super().__init__(
             in_channels_list,
             in_features_list,
             out_channels,
             out_features,
@@ -298,52 +338,64 @@
     ```
     Parameter Size:
     ```txt
     2,180 weights, 22 biases -> 2,202 params
     ```
     Parameters
     ----------
-    `activation` : Type of activation function (Default `Tanh`)
-    `optimizer` : Type of optimizer for weight update
-    `loss` : Type of loss function (Default `CrossEntropy`)
-    `initializer` : Type of weight initializer (`None` for dense layers)
-    `out_features` : Number of output features (Default `10`)
-    `batch_size` : Size of a single mini-batch
-    `n_epochs` : Number of epochs for training
-    `learning_rate` : Step size during optimization process
-    `valid_size` : Fractional size of validation set
-    `lambda_` : L2 regularization strength
-    `early_stopping` : Whether to early-stop the training when the valid
-    score stagnates
-    `patience` : Number of epochs to wait until early-stopping
-    `shuffle` : Whethter to shuffle the data at the beginning of every epoch
+    `activation` : FuncType, default=Activation.Tanh()
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss, default=CrossEntropy()
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `out_features` : int, default=10
+        Number of output features
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.001
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
 
     References
     ----------
     1. LeCun, Yann, et al. "Backpropagation Applied to Handwritten Zip
     Code Recognition." Neural Computation, vol. 1, no. 4, 1989, pp. 541-551.
 
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation = Activation.Tanh(),
+        activation: Activation.FuncType = Activation.Tanh(),
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         deep_verbose: bool = False,
     ) -> None:
         super().__init__(
             optimizer,
             activation,
             loss,
             initializer,
@@ -388,52 +440,64 @@
     ```
     Parameter Size:
     ```txt
     50,902 weights, 150 biases -> 51,052 params
     ```
     Parameters
     ----------
-    `activation` : Type of activation function (Default `Tanh`)
-    `optimizer` : Type of optimizer for weight update
-    `loss` : Type of loss function (Default `CrossEntropy`)
-    `initializer` : Type of weight initializer (`None` for dense layers)
-    `out_features` : Number of output features (Default `10`)
-    `batch_size` : Size of a single mini-batch
-    `n_epochs` : Number of epochs for training
-    `learning_rate` : Step size during optimization process
-    `valid_size` : Fractional size of validation set
-    `lambda_` : L2 regularization strength
-    `early_stopping` : Whether to early-stop the training when the valid
-    score stagnates
-    `patience` : Number of epochs to wait until early-stopping
-    `shuffle` : Whethter to shuffle the data at the beginning of every epoch
+    `activation` : FuncType, default=Activation.Tanh()
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss, default=CrossEntropy()
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `out_features` : int, default=10
+        Number of output features
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.001
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
 
     References
     ----------
     1. LeCun, Yann, et al. "Backpropagation Applied to Handwritten Zip
     Code Recognition." Neural Computation, vol. 1, no. 4, 1989, pp. 541-551.
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation = Activation.Tanh(),
+        activation: Activation.FuncType = Activation.Tanh(),
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         deep_verbose: bool = False,
     ) -> None:
         super().__init__(
             optimizer,
             activation,
             loss,
             initializer,
@@ -480,52 +544,64 @@
     ```
     Parameter Size:
     ```txt
     61,474 weights, 236 biases -> 61,710 params
     ```
     Parameters
     ----------
-    `activation` : Type of activation function (Default `Tanh`)
-    `optimizer` : Type of optimizer for weight update
-    `loss` : Type of loss function (Default `CrossEntropy`)
-    `initializer` : Type of weight initializer (`None` for dense layers)
-    `out_features` : Number of output features (Default `10`)
-    `batch_size` : Size of a single mini-batch
-    `n_epochs` : Number of epochs for training
-    `learning_rate` : Step size during optimization process
-    `valid_size` : Fractional size of validation set
-    `lambda_` : L2 regularization strength
-    `early_stopping` : Whether to early-stop the training when the valid
-    score stagnates
-    `patience` : Number of epochs to wait until early-stopping
-    `shuffle` : Whethter to shuffle the data at the beginning of every epoch
+    `activation` : FuncType, default=Activation.Tanh()
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss, default=CrossEntropy()
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `out_features` : int, default=10
+        Number of output features
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.001
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
 
     References
     ----------
     1. LeCun, Yann, et al. "Backpropagation Applied to Handwritten Zip
     Code Recognition." Neural Computation, vol. 1, no. 4, 1989, pp. 541-551.
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation = Activation.Tanh(),
+        activation: Activation.FuncType = Activation.Tanh(),
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         deep_verbose: bool = False,
     ) -> None:
         super().__init__(
             optimizer,
             activation,
             loss,
             initializer,
@@ -580,54 +656,66 @@
     ```
     Parameter Size:
     ```txt
     62,367,776 weights, 10,568 biases -> 62,378,344 params
     ```
     Parameters
     ----------
-    `activation` : Type of activation function (Default `ReLU`)
-    `optimizer` : Type of optimizer for weight update
-    `loss` : Type of loss function (Default `CrossEntropy`)
-    `initializer` : Type of weight initializer (Default None)
-    `out_features` : Number of output features (Default `1000`)
-    `batch_size` : Size of a single mini-batch
-    `n_epochs` : Number of epochs for training
-    `learning_rate` : Step size during optimization process
-    `valid_size` : Fractional size of validation set
-    `lambda_` : L2 regularization strength
-    `early_stopping` : Whether to early-stop the training when the valid
-    score stagnates
-    `patience` : Number of epochs to wait until early-stopping
-    `shuffle` : Whether to shuffle the data at the beginning of every epoch
+    `activation` : FuncType, default=Activation.ReLU()
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss, default=CrossEntropy()
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `out_features` : int, default=1000
+        Number of output features
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.01
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
 
     References
     ----------
     1. Krizhevsky, Alex, Ilya Sutskever, and Geoffrey E. Hinton. "ImageNet
     Classification with Deep Convolutional Neural Networks." Advances in Neural
     Information Processing Systems, 2012.
 
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation = Activation.ReLU(),
+        activation: Activation.FuncType = Activation.ReLU(),
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         deep_verbose: bool = False,
     ) -> None:
         super().__init__(
             optimizer,
             activation,
             loss,
             initializer,
@@ -683,53 +771,65 @@
     ```
     Parameter Size:
     ```txt
     58,292,000 weights, 9,578 biases -> 58,301,578 params
     ```
     Parameters
     ----------
-    `activation` : Type of activation function (Default `ReLU`)
-    `optimizer` : Type of optimizer for weight update
-    `loss` : Type of loss function (Default `CrossEntropy`)
-    `initializer` : Type of weight initializer (Default None)
-    `out_features` : Number of output features (Default `1000`)
-    `batch_size` : Size of a single mini-batch
-    `n_epochs` : Number of epochs for training
-    `learning_rate` : Step size during optimization process
-    `valid_size` : Fractional size of validation set
-    `lambda_` : L2 regularization strength
-    `early_stopping` : Whether to early-stop the training when the valid
-    score stagnates
-    `patience` : Number of epochs to wait until early-stopping
-    `shuffle` : Whether to shuffle the data at the beginning of every epoch
+    `activation` : FuncType, default=Activation.ReLU()
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss, default=CrossEntropy()
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `out_features` : int, default=1000
+        Number of output features
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.01
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
 
     References
     ----------
     1. Zeiler, Matthew D., and Rob Fergus. "Visualizing and Understanding
     Convolutional Networks." European conference on computer vision, 2014.
 
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation = Activation.ReLU(),
+        activation: Activation.FuncType = Activation.ReLU(),
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         deep_verbose: bool = False,
     ) -> None:
         super().__init__(
             optimizer,
             activation,
             loss,
             initializer,
```

### Comparing `luma-ml-0.7.5/luma/neural/optimizer.py` & `luma-ml-0.8.0/luma/neural/optimizer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/neural/single.py` & `luma-ml-0.8.0/luma/neural/single.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,28 +21,32 @@
     classify training examples. It iteratively adjusts weights based on the
     difference between predicted and actual outcomes. The perceptron's
     simplicity makes it foundational in understanding more complex neural
     networks.
 
     Parameters
     ----------
-    `learning_rate` : Step size for updating weights
-    `max_iter` : Maximum iteration
-    `regularization` : Regularizing methods (e.g. `l1`, `l2`, `elastic-net`)
-    `alpha` : Regularization strength
-    `l1_ratio` : Ratio of `l1` (Only use when `elastic-net` regularization)
-    `random_state` : Seed for random shuffling during SGD
+    `learning_rate` : float, default=0.01
+        Step size for updating weights
+    `max_iter` : int, default=1000
+        Maximum iteration
+    `regularization` : {"l1", "l2", "elastic-net"}, optional, default=None
+        Regularizing methods
+    `alpha` : float, default=1e-4
+        Regularization strength
+    `l1_ratio` : float, default=0.5, range=[0,1]
+        Ratio of L1 regularization (Only used for elastic-net)
 
     """
 
     def __init__(
         self,
         learning_rate: float = 0.01,
         max_iter: int = 1000,
-        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        regularization: Literal["l1", "l2", "elastic-net"] | None = None,
         alpha: float = 0.0001,
         l1_ratio: float = 0.5,
         random_state: int = None,
         verbose: bool = False,
     ) -> None:
         self.learning_rate = learning_rate
         self.max_iter = max_iter
@@ -137,17 +141,24 @@
     weights. The Perceptron Regressor updates its weights during training to
     minimize the difference between predicted and actual continuous outcomes.
     This model provides a basic understanding of linear regression in the
     context of neural networks.
 
     Parameters
     ----------
-    `learning_rate` : Step size for updating weights
-    `max_iter` : Maximum iteration
-    `random_state` : Seed for random shuffling during SGD
+    `learning_rate` : float, default=0.01
+        Step size for updating weights
+    `max_iter` : int, default=1000
+        Maximum iteration
+    `regularization` : {"l1", "l2", "elastic-net"}, optional, default=None
+        Regularizing methods
+    `alpha` : float, default=1e-4
+        Regularization strength
+    `l1_ratio` : float, default=0.5, range=[0,1]
+        Ratio of L1 regularization (Only used for elastic-net)
 
     """
 
     def __init__(
         self,
         learning_rate: float = 0.01,
         max_iter: int = 1000,
```

### Comparing `luma-ml-0.7.5/luma/pipe/pipeline.py` & `luma-ml-0.8.0/luma/pipe/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,25 @@
     It includes data collection and preprocessing, model selection and training,
     evaluation, and deployment. This systematic approach ensures efficiency
     and accuracy in model development. Pipelines are often automated for
     scalability and reproducibility in real-world applications.
 
     Parameters
     ----------
-    `models` : List of models \n
-    You can assign labels to each model by encapsulating the label and the model
-    inside a tuple. \n
-    Otherwise, the name of the model is automatically assigned by default.
-
-    `param_dict` : Dictionary of parameters for each models \n
-    You must specify the name(or label) of the model and its parameter name
-    in the key of the dictionary. \n
-    e.g. `{'model_name__param_name': value}`
+    `models` : list of Tuple[str, Model] or list of Model
+        List of model; You can assign labels to each model by encapsulating the
+        label and the model inside a tuple.
+
+        Otherwise, the name of the model is automatically assigned by default.
+
+    `param_dict` : Dict[str, Any], default={}
+        Dictionary of parameters for each models
+
+        You must specify the name(or label) of the model and its parameter name
+        in the key of the dictionary. e.g. `{'model_name__param_name': value}`
 
     Examples
     --------
     >>> pipe = Pipeline(
             models=[
                 ('trans_1', Transformer()),
                 ('trans_2', Transformer()),
@@ -55,35 +57,32 @@
     Properties
     ----------
     Getting list of transformers:
         ```py
         @property
         def transformers(self) -> List[Transformer]
         ```
-
     Getting final estimator:
         ```py
         @property
         def estimator(self) -> Estimator
         ```
-
     Getting transformed data:
         ```py
         @property
         def transformed_data(self) -> Tuple[Matrix, Matrix]
         ```
-
     Notes
     -----
-    * To use `Pipeline` with visual methods of `luma.visual`, make sure to
-    transform data using `pipe.transform()` if the pipeline sequence contains
-    transformers
+    - To use `Pipeline` with visual methods of `luma.visual`, make sure to
+        transform data using `pipe.transform()` if the pipeline sequence contains
+        transformers
 
-    * More than one estimator might cause procedural failure
-    * Not all the models are compatible with `Pipeline`
+    - More than one estimator might cause procedural failure
+    - Not all the models are compatible with `Pipeline`
 
     """
 
     def __init__(
         self,
         models: List[Tuple[str, Model]] | List[Model],
         param_dict: Dict[str, Any] = dict(),
```

### Comparing `luma-ml-0.7.5/luma/preprocessing/encoder.py` & `luma-ml-0.8.0/luma/preprocessing/encoder.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/preprocessing/imputer.py` & `luma-ml-0.8.0/luma/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/preprocessing/outlier.py` & `luma-ml-0.8.0/luma/preprocessing/outlier.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,18 @@
     Points with significantly lower density than their neighbors are considered
     outliers. LOF scores greater than 1 indicate potential outliers. It is
     effective in datasets with varying densities and does not require a prior
     assumption about the data distribution.
 
     Parameters
     ----------
-    `n_neighbors` : Number of neighbors to estimate the local densities
-    `threshold` : Cutoff value deciding whether a point is considered an outlier
+    `n_neighbors` : int, default=10
+        Number of neighbors to estimate the local densities
+    `threshold` : float, default=1.5
+        Cutoff value deciding whether a point is considered an outlier
 
     Examples
     --------
     >>> lof = LocalOutlierFactor()
     >>> lof.fit(X)
 
     Getting LOF Scores
```

### Comparing `luma-ml-0.7.5/luma/preprocessing/scaler.py` & `luma-ml-0.8.0/luma/preprocessing/scaler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Self
 import numpy as np
 
-from luma.interface.typing import Matrix
+from luma.interface.typing import Matrix, Scalar
 from luma.core.super import Transformer
 from luma.interface.exception import NotFittedError
 
 
 __all__ = ("StandardScaler", "MinMaxScaler")
 
 
@@ -47,19 +47,20 @@
     MinMax scaling (also known as Min-Max normalization)
     to rescale features to a specific range, typically between 0 and 1.
     The purpose of MinMax scaling is to transform the features in a way
     that they fall within a specific interval.
 
     Parameters
     ----------
-    `feature_range` : Range to be scaled
+    `feature_range` : tuple[Scalar, Scalar], default=(0,1)
+        Range to be scaled
 
     """
 
-    def __init__(self, feature_range: tuple = (0, 1)) -> None:
+    def __init__(self, feature_range: tuple[Scalar, Scalar] = (0, 1)) -> None:
         self.feature_range = feature_range
         self.min = None
         self.max = None
         self._fitted = False
 
     def fit(self, X: Matrix) -> Self:
         self.min = np.min(X, axis=0)
```

### Comparing `luma-ml-0.7.5/luma/reduction/linear.py` & `luma-ml-0.8.0/luma/reduction/linear.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,19 +19,20 @@
     """
     PCA, or Principal Component Analysis, is a dimensionality
     reduction technique. It's primarily used to simplify complex
     data while retaining the most important information.
 
     Parameters
     ----------
-    `n_components` : Number of principal components
+    `n_components` : int, required optional, default=None
+        Number of principal components
 
     """
 
-    def __init__(self, n_components: int = None) -> None:
+    def __init__(self, n_components: int | None = None) -> None:
         self.n_components = n_components
         self._fitted = False
 
         self.set_param_ranges({"n_components": ("0<,+inf", int)})
         self.check_param_ranges()
 
     def fit(self, X: Matrix) -> Self:
@@ -71,26 +72,30 @@
     Principal Component Analysis (PCA) to capture complex, nonlinear
     relationships in data by using a kernel function to transform
     the data into a higher-dimensional space where nonlinear patterns
     can be better captured.
 
     Parameters
     ----------
-    `n_components` : Number of principal components
-    `deg` : Polynomial degree of `poly` kernel
-    `gamma` : Shape parameter of `rbf`, `sigmoid`, `laplacian`
-    `coef` : Additional coefficient of `poly`, `sigmoid`
-    `kernel` : Type of kernel functions
-    (e.g. `linear`, `poly`, `rbf`, `sigmoid`, `laplacian`)
+    `n_components` : int, required optional, default=None
+        Number of principal components
+    `deg` : int, default=3
+        Polynomial degree of polynomial kernel
+    `gamma` : float, default=1.0
+        Shape parameter of RBF, sigmoid, and laplacian kernels
+    `coef` : float, default=1.0
+        Additional coefficient of polynomial and sigmoid kernels
+    `kernel` : FuncType, default="rbf"
+        Type of kernel functions
 
     """
 
     def __init__(
         self,
-        n_components: int = None,
+        n_components: int | None = None,
         deg: int = 3,
         gamma: float = 1.0,
         coef: float = 1.0,
         kernel: KernelUtil.FuncType = "rbf",
     ) -> None:
         self.n_components = n_components
         self.deg = deg
@@ -188,24 +193,25 @@
     Linear Discriminant Analysis (LDA) is a dimensionality reduction
     and classification technique. It's primarily employed for dimensionality
     reduction and feature extraction while also considering class
     information for classification tasks.
 
     Parameters
     ----------
-    `n_components` : Number of linear discriminants
+    `n_components` : int, required optional, default=None
+        Number of linear discriminants
 
     Notes
     -----
     * To use LDA for classification, refer to
         `luma.classifier.discriminant.LDAClassifier`
 
     """
 
-    def __init__(self, n_components: int = None) -> None:
+    def __init__(self, n_components: int | None = None) -> None:
         self.n_components = n_components
         self._fitted = False
 
         self.set_param_ranges({"n_components": ("0<,+inf", int)})
         self.check_param_ranges()
 
     def fit(self, X: Matrix, y: Matrix) -> Self:
@@ -250,27 +256,28 @@
     def fit_transform(self, X: Matrix, y: Matrix) -> Matrix:
         self.fit(X, y)
         return self.transform(X)
 
 
 class TruncatedSVD(Transformer, Unsupervised):
     """
-    runcated Singular Value Decomposition (TruncatedSVD) is a linear dimensionality
+    Truncated Singular Value Decomposition (TruncatedSVD) is a linear dimensionality
     reduction method that simplifies large datasets by preserving the most relevant
     information. It achieves this by decomposing a matrix into three components
     using singular value decomposition (SVD) and retaining only a specified number
     of important components.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of low-space
+    `n_components` : int, required optional, default=None
+        Dimensionality of low-space
 
     """
 
-    def __init__(self, n_components: int = None) -> None:
+    def __init__(self, n_components: int | None = None) -> None:
         self.n_components = n_components
         self._fitted = False
 
         self.set_param_ranges({"n_components": ("0<,+inf", int)})
         self.check_param_ranges()
 
     def fit(self, X: Matrix) -> Self:
@@ -302,27 +309,31 @@
     influencing observed variables. It assumes that observed variables share
     common variance due to these unobservable factors, expressed through
     factor loadings. The technique helps simplify data interpretation by
     revealing the underlying structure of the dataset.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of low-space
-    `max_iter` : Number of iterations
-    `tol` : Threshold for convergence
-    `noise_variance` : Initial variances for noise of each features
+    `n_components` : int, required optional, default=None
+        Dimensionality of low-space
+    `max_iter` : int, default=1000
+        Number of iterations
+    `tol` : float, default=1e-5
+        Threshold for convergence
+    `noise_variance` : list or Matirx, optional, default=None
+        Initial variances for noise of each features
 
     """
 
     def __init__(
         self,
-        n_components: int = None,
+        n_components: int | None = None,
         max_iter: int = 1000,
         tol: float = 1e-5,
-        noise_variance: Matrix | list = None,
+        noise_variance: Matrix | list | None = None,
         verbose: bool = False,
     ) -> None:
         self.n_components = n_components
         self.max_iter = max_iter
         self.tol = tol
         self.noise_variance = noise_variance
         self.verbose = verbose
@@ -406,33 +417,38 @@
     are more separable by maximizing the ratio of between-class variance
     to within-class variance. KDA utilizes kernel functions to implicitly
     map input data to a high-dimensional space without explicitly computing
     the coordinates in that space.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of low-space
-    `deg` : Polynomial degree of `poly` kernel
-    `gamma` : Shape parameter of `rbf`, `sigmoid`, `laplacian`
-    `coef` : Additional coefficient of `poly`, `sigmoid`
-    `kernel` : Type of kernel functions
+    `n_components` : int, required optional, default=None
+        Dimensionality of low-space
+    `deg` : int, default=2
+        Polynomial degree of polynomial kernel
+    `gamma` : float, default=1.0
+        Shape parameter of RBF, sigmoid, laplacian
+    `coef` : float, default=0.0
+        Additional coefficient of polynomial, sigmoid
+    `kernel` : FuncType, default="rbf"
+        Type of kernel functions
 
     Notes
     -----
-    * To use KDA for classification, refer to
+    - To use KDA for classification, refer to
         `luma.classifier.discriminant.KDAClassifier`
 
     """
 
     def __init__(
         self,
-        n_components: int = None,
+        n_components: int | None = None,
         deg: int = 2,
         gamma: float = 1.0,
-        coef: int = 0.0,
+        coef: float = 0.0,
         kernel: KernelUtil.FuncType = "rbf",
     ) -> None:
         self.n_components = n_components
         self.deg = deg
         self.gamma = gamma
         self.coef = coef
         self.kernel = kernel
@@ -497,30 +513,31 @@
     between the two variable sets. CCA is an unsupervised technique, often
     used for exploring the relationships in complex data. The result is pairs
     of canonical variables (or components) that represent the maximal
     correlations between the sets.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of low-space
+    `n_components` : int, required optional, default=None
+        Dimensionality of low-space
 
     Notes
     -----
-    * `CCA` requires two distinct datasets `X` and `Y`,
+    - `CCA` requires two distinct datasets `X` and `Y`,
         in which `Y` is not a target variable
-    * Due to its uniqueness in its parameters,
+    - Due to its uniqueness in its parameters,
         `CCA` may not be compatible with several meta estimators
-    * `transform()` and `fit_transform()` returns a 2-tuple of `Matrix`
+    - `transform` and `fit_transform` returns a 2-tuple of `Matrix`
 
         ```py
         def transform(self, X: Matrix, Y: Matrix) -> Tuple[Matrix, Matrix]
         ```
     """
 
-    def __init__(self, n_components: int = None) -> None:
+    def __init__(self, n_components: int | None = None) -> None:
         self.n_components = n_components
         self.correlations_ = None
         self._fitted = False
 
         self.set_param_ranges({"n_components": ("0<,+inf", int)})
         self.check_param_ranges()
```

### Comparing `luma-ml-0.7.5/luma/reduction/manifold.py` & `luma-ml-0.8.0/luma/reduction/manifold.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,25 +34,28 @@
     """
     t-SNE, which stands for t-distributed Stochastic Neighbor Embedding,
     is a machine learning technique commonly used for data visualization
     and dimensionality reduction.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of lower spcae
-    `max_iter` : Number of iteration
-    `learning_rate` : Updating factor of embedding optimization
-    `perplexity` : Perplexity parameter of Gaussian kernel
-    `verbose` : Provided details of each iteration when set `True`
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
+    `max_iter` : int, default=1000
+        Number of iteration
+    `learning_rate` : float, default=300
+        Updating factor of embedding optimization
+    `perplexity` : int, default=30, preferred range=[5,50]
+        Perplexity parameter of Gaussian kernel
 
     """
 
     def __init__(
         self,
-        n_components: int = None,
+        n_components: int | None = None,
         max_iter: int = 1000,
         learning_rate: int = 300,
         perplexity: int = 30,
         verbose: bool = False,
     ) -> None:
         self.n_components = n_components
         self.max_iter = max_iter
@@ -189,19 +192,20 @@
     high-dimensional data in a lower-dimensional space while preserving the
     relationships between data points. It uses a distance matrix to find a
     lower-dimensional representation, making it easier to understand and
     explore data patterns.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of low-space
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
 
     """
 
-    def __init__(self, n_components: int = None) -> None:
+    def __init__(self, n_components: int | None = None) -> None:
         self.n_components = n_components
         self._fitted = False
 
         self.set_param_ranges({"n_components": ("0<,+inf", int)})
         self.check_param_ranges()
 
     def fit(self, X: Matrix) -> Self:
@@ -247,26 +251,29 @@
     Metric Multidimensional Scaling (MDS) is a data analysis method that focuses
     on accurately preserving the original pairwise distances or dissimilarities
     between objects in a high-dimensional space when projecting them onto a
     lower-dimensional space.
 
     Parameter
     ---------
-    `n_components` : Dimensionality of low-space
-    `metric` : Distance metric
-    (e.g. `euclidean`, `manhattan`, `chebyshev`, `minkowski`,
-    `cos_similarity`, `correation`, `mahalanobis`)
-    `p` : Power factor for `minkowski`
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
+    `metric` : {"euclidean", "manhattan", "chebyshev", "minkowski",
+                "cos_similarity", "correlation", "mahalanobis"},
+                default="euclidean"
+        Distance metric
+    `p` : int or float, optional, default=None
+        Power factor for `minkowski`
 
     """
 
     def __init__(
         self,
-        n_components: int = None,
-        p: float | int = None,
+        n_components: int | None = None,
+        p: float | int | None = None,
         metric: Literal[
             "euclidean",
             "manhattan",
             "chebyshev",
             "minkowski",
             "cos_similarity",
             "correlation",
@@ -351,24 +358,26 @@
     that selects a subset of "landmark" points to efficiently approximate the
     lower-dimensional representation of a dataset while preserving pairwise distances.
     It simplifies the computation by focusing on distances between data points and
     landmarks, making it suitable for large datasets.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of low-space
-    `n_landmarks` : Number of landmarks
-    `method` : Algorithm for landmark initialization
-    (e.g. `random`, `kmeans`, `kmeans++`, `kmedians`)
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
+    `n_landmarks` : int, default=10
+        Number of landmarks
+    `method` : {"random", "kmeans", "kmeans++", "kmedians"}, default="random"
+        Algorithm for landmark initialization
 
     """
 
     def __init__(
         self,
-        n_components: int = None,
+        n_components: int | None = None,
         n_landmarks: int = 10,
         method: Literal["random", "kmeans", "kmeans++", "kmedians"] = "random",
         verbose: bool = False,
     ) -> None:
         self.n_components = n_components
         self.n_landmarks = n_landmarks
         self.method = method
@@ -457,21 +466,26 @@
     to find a lower-dimensional representation of data while preserving the local
     relationships between data points. It works by approximating each data point
     as a linear combination of its nearest neighbors, revealing the underlying
     structure of the data in a lower-dimensional space.
 
     Parameters
     ----------
-    `n_neighbors` : Number of neighbors to be considered 'close'
-    `n_components` : Dimensionality of low-space
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
+    `n_neighbors` : int, default=5
+        Number of neighbors to be considered 'close'
 
     """
 
     def __init__(
-        self, n_components: int = None, n_neighbors: int = 5, verbose: bool = False
+        self,
+        n_components: int | None = None,
+        n_neighbors: int = 5,
+        verbose: bool = False,
     ) -> None:
         self.n_neighbors = n_neighbors
         self.n_components = n_components
         self.verbose = verbose
         self._fitted = False
 
         self.set_param_ranges(
@@ -524,24 +538,27 @@
     MLLE aims to find a lower-dimensional representation of data while preserving the
     local relationships between data points. It works by approximating each data
     point as a linear combination of its nearest neighbors, revealing the underlying
     structure of the data in a lower-dimensional space.
 
     Parameters
     ----------
-    `n_neighbors` : Number of neighbors to be considered 'close'
-    `n_components` : Dimensionality of the lower-dimensional space
-    `regularization` : Regularization parameter for stability
+    `n_neighbors` : int, default=5
+        Number of neighbors to be considered 'close'
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
+    `regularization` : float, default=1e-3
+        Regularization parameter for stability
 
     """
 
     def __init__(
         self,
         n_neighbors: int = 5,
-        n_components: int = None,
+        n_components: int | None = None,
         regularization: float = 1e-3,
         verbose: bool = False,
     ) -> None:
         self.n_neighbors = n_neighbors
         self.n_components = n_components
         self.regularization = regularization
         self.verbose = verbose
@@ -599,24 +616,27 @@
     Hessian Locally Linear Embedding (Hessian LLE) is a dimensionality reduction
     technique that extends Locally Linear Embedding (LLE). It aims to reduce the
     dimensionality of high-dimensional data while preserving local linear relationships
     and capturing the curvature of these relationships using the Hessian matrix.
 
     Parameters
     ----------
-    `n_neighbors` : Number of neighbors to be considered 'close'
-    `n_components` : Dimensionality of the lower-dimensional space
-    `regularization` : Regularization parameter for stability
+    `n_neighbors` : int, default=5
+        Number of neighbors to be considered 'close'
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
+    `regularization` : float, default=1e-5
+        Regularization parameter for stability
 
     """
 
     def __init__(
         self,
         n_neighbors: int = 5,
-        n_components: int = None,
+        n_components: int | None = None,
         regularization: float = 1e-5,
         verbose: bool = False,
     ) -> None:
         self.n_neighbors = n_neighbors
         self.n_components = n_components
         self.regularization = regularization
         self.verbose = verbose
@@ -712,25 +732,30 @@
     Sammon mapping is a dimensionality reduction algorithm designed to transform
     high-dimensional data into a lower-dimensional space. Sammon mapping focuses
     on preserving the pairwise distances or dissimilarities between data points,
     making it well-suited for capturing non-linear relationships in the data.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of low-space
-    `max_iter` : Number of iteration
-    `max_halves` : Number of halving of step-size
-    `tol` : Threshold for early-stopping
-    `initialize` : Methodology for embedding-space initialization
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
+    `max_iter` : int, default=100
+        Number of iteration
+    `max_halves` : int, default=20
+        Number of halving of step-size
+    `tol` : float, default=1e-5
+        Threshold for early-stopping
+    `initialize` : {"pca"}, optional, default="pca"
+        Methodology for embedding-space initialization
 
     """
 
     def __init__(
         self,
-        n_components: int = None,
+        n_components: int | None = None,
         max_iter: int = 100,
         max_halves: int = 20,
         tol: float = 1e-5,
         initialize: Literal["pca"] | None = "pca",
         verbose: bool = False,
     ) -> None:
         self.n_components = n_components
@@ -851,20 +876,22 @@
     preserving local relationships. It constructs a weighted graph based
     on pairwise similarities between data points, computes the Laplacian
     matrix from the graph, and performs eigenvalue decomposition to
     obtain eigenvectors.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of the lower-dimensional space
-    `sigma` : Width parameter for Gaussian kernel in affinity calculation
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
+    `sigma` : float, default=1.0
+        Width parameter for Gaussian kernel in affinity calculation
 
     """
 
-    def __init__(self, n_components: int = None, sigma: float = 1.0) -> None:
+    def __init__(self, n_components: int | None = None, sigma: float = 1.0) -> None:
         self.n_components = n_components
         self.sigma = sigma
         self.embedding = None
         self._fitted = False
 
         self.set_param_ranges(
             {"n_components": ("0<,+inf", int), "sigma": ("0<,+inf", None)}
@@ -911,26 +938,29 @@
     between data points in high-dimensional datasets. By constructing a neighborhood
     graph and calculating pairwise geodesic distances, Isomap transforms the data
     into a lower-dimensional space, offering insights into complex, nonlinear
     relationships within the dataset.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of low-space
-    `epsilon` : Boundary radius of the neighbor hypersphere
-    `algorithm` : Shortest path finding algorithm
-    (e.g. `dijkstra`, `floyd`)
-    `metric` : Distance metric
-    (e.g. `euclidean`, `cityblock`, `chebyshev`, `cosine`, `correlation`)
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
+    `epsilon` : float, default=5.0
+        Boundary radius of the neighbor hypersphere
+    `algorithm` : {"dijkstra", "floyd"}, default="dijkstra"
+        Shortest path finding algorithm
+    `metric` : {"euclidean", "cityblock", "chebyshev", "cosine", "correlation"},
+                default="euclidean"
+        Distance metric
 
     """
 
     def __init__(
         self,
-        n_components: int = None,
+        n_components: int | None = None,
         epsilon: float = 5.0,
         algorithm: Literal["dijkstra", "floyd"] = "dijkstra",
         metric: Literal[
             "euclidean", "cityblock", "chebyshev", "cosine", "correlation"
         ] = "euclidean",
     ) -> None:
         self.n_components = n_components
@@ -993,24 +1023,26 @@
     prioritizes preserving infinitesimal angles (conformality) by adjusting
     geodesic distances to reflect scale information. Unlike traditional Isomap,
     which focuses on preserving full isometry, C-Isomap is well-suited for
     datasets with varying local scales or non-uniform structures.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of low-space
-    `epsilon` : Boundary radius of the neighbor hypersphere
-    `algorithm` : Shortest path finding algorithm
-    (e.g. `dijkstra`, `floyd`)
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
+    `epsilon` : float, default=5.0
+        Boundary radius of the neighbor hypersphere
+    `algorithm` : {"dijkstra", "floyd"}, default="dijkstra"
+        Shortest path finding algorithm
 
     """
 
     def __init__(
         self,
-        n_components: int = None,
+        n_components: int | None = None,
         epsilon: float = 5.0,
         algorithm: Literal["dijkstra", "floyd"] = "dijkstra",
     ) -> None:
         self.n_components = n_components
         self.epsilon = epsilon
         self.algorithm = algorithm
         self._fitted = False
@@ -1076,20 +1108,26 @@
     It works by approximating the tangent space at each data point and aligning
     these local tangent spaces. This helps to capture the intrinsic structure
     of the data, particularly in cases where the global geometry might be
     complex or non-linear.
 
     Parameters
     ----------
-    `n_components` : Dimensionality of low-space
-    `n_neighbors` : Number of neighbors
+    `n_components` : int, required optional, default=None
+        Dimensionality of lower spcae
+    `n_neighbors` : int, default=10
+        Number of neighbors
 
     """
 
-    def __init__(self, n_components: int = None, n_neighbors: int = 10) -> None:
+    def __init__(
+        self,
+        n_components: int | None = None,
+        n_neighbors: int = 10,
+    ) -> None:
         self.n_components = n_components
         self.n_neighbors = n_neighbors
         self._fitted = False
 
         self.set_param_ranges(
             {"n_components": ("0<,+inf", int), "n_neighbors": ("0<,+inf", int)}
         )
```

### Comparing `luma-ml-0.7.5/luma/reduction/selection.py` & `luma-ml-0.8.0/luma/reduction/selection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import combinations
-from typing import Tuple
+from typing import Self, Tuple
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Transformer, Supervised
 from luma.interface.typing import Matrix, Vector
 from luma.interface.util import Clone
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 
@@ -22,53 +22,64 @@
     removes the least significant feature at each step_size. The goal is to
     reduce dimensionality while maintaining or improving model performance.
     The process continues until the desired number of features is reached
     or performance criteria are met.
 
     Parameters
     ----------
-    `estimator` : An estimator to fit and evaluate
-    `n_features` : Number of features to select (`0~1` value for proportion)
-    `metric` : Scoring metric for selecting features
-    `test_size` : Proportional size of the validation set
-    `cv` : K-fold size for cross validation (`0` to disable CV)
-    `shuffle` : Whether to shuffle the dataset
-    `stratify` : Whether to perform stratified split
-    `fold_type` : Fold type (Default `KFold`)
-    `random_state` : Seed for splitting the data
+    `estimator` : Estimator, optional, default=None
+        An estimator to fit and evaluate
+    `n_features` : int or float, default=1
+        Number of features to select (`0~1` value for proportion)
+    `metric` : Evaluator, optional, default=None
+        Scoring metric for selecting features
+    `test_size` : float, default=0.2
+        Proportional size of the validation set
+    `cv` : int, default=5
+        K-fold size for cross validation (`0` to disable CV)
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset
+    `stratify` : bool, default=False
+        Whether to perform stratified split
+    `fold_type` : FoldType, default=KFold
+        Fold type
+    `random_state` : int, optional, default=None
+        Seed for splitting the data
 
     Notes
     -----
-    * An instance of the estimator must be passed to `estimator`
-    * For `metric`, both class or instance are possible
+    - An instance of the estimator must be passed to `estimator`
+    - For `metric`, both class or instance are possible
 
     Examples
     --------
-    >>> sbs = SBS(estimator=AnyEstimator(),
-                  n_features=0.25,
-                  metric=AnyEvaluator,
-                  test_size=0.2,
-                  cv=5,
-                  random_state=None)
+    >>> sbs = SBS(
+            estimator=AnyEstimator(),
+            n_features=0.25,
+            metric=AnyEvaluator,
+            test_size=0.2,
+            cv=5,
+            random_state=None,
+        )
     >>> sbs.fit(X, y)
     >>> Z = sbs.transform(X)
 
     """
 
     def __init__(
         self,
-        estimator: Estimator = None,
+        estimator: Estimator | None = None,
         n_features: int | float = 1,
-        metric: Evaluator = None,
+        metric: Evaluator | None = None,
         test_size: float = 0.2,
         cv: int = 5,
         shuffle: bool = True,
         stratify: bool = False,
         fold_type: FoldType = KFold,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ) -> None:
         self.estimator = estimator
         self.n_features = n_features
         self.metric = metric
         self.test_size = test_size
         self.cv = cv
@@ -84,15 +95,15 @@
                 "n_features": ("0<,+inf", None),
                 "test_size": ("0,1", float),
                 "cv": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "SBS":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         _, n = X.shape
         self.estimator = Clone(self.estimator).get
 
         if 0 < self.n_features < 1:
             self.n_features = np.ceil(n * self.n_features).astype(int)
         elif self.n_features <= 0 or self.n_features > n:
             raise UnsupportedParameterError(self.n_features)
@@ -193,30 +204,39 @@
     adds the most significant feature at each step. The goal is to
     reduce dimensionality while maintaining or improving model performance.
     The process continues until the desired number of features is reached
     or performance criteria are met.
 
     Parameters
     ----------
-    `estimator` : An estimator to fit and evaluate
-    `n_features` : Number of features to select (`0~1` value for proportion)
-    `metric` : Scoring metric for selecting features
-    `test_size` : Proportional size of the validation set
-    `cv` : K-fold size for cross validation (`0` to disable CV)
-    `shuffle` : Whether to shuffle the dataset
-    `stratify` : Whether to perform stratified split
-    `fold_type` : Fold type (Default `KFold`)
-    `random_state` : Seed for splitting the data
+    `estimator` : Estimator, required optional, default=None
+        An estimator to fit and evaluate
+    `n_features` : int or float
+        Number of features to select (`0~1` value for proportion)
+    `metric` : Evaluator, optional, default=None
+        Scoring metric for selecting features
+    `test_size` : float, default=0.2
+        Proportional size of the validation set
+    `cv` : int, default=5
+        K-fold size for cross validation (`0` to disable CV)
+    `shuffle` : bool, defalut=True
+        Whether to shuffle the dataset
+    `stratify` : bool, default=False
+        Whether to perform stratified split
+    `fold_type` : FoldType, default=Kfold
+        Fold type
+    `random_state` : int, optional, default=None
+        Seed for splitting the data
 
     Notes
     -----
-    * An instance of the estimator must be passed to `estimator`
-    * Do not use the estimator for `SFS` if it is supposed to be the
+    - An instance of the estimator must be passed to `estimator`
+    - Do not use the estimator for `SFS` if it is supposed to be the
         main estimator for the model
-    * For `metric`, both class or instance are possible
+    - For `metric`, both class or instance are possible
 
     Examples
     --------
     >>> sfs = SFS(estimator=AnyEstimator(),
                   n_features=0.25,
                   metric=AnyEvaluator,
                   test_size=0.2,
@@ -225,23 +245,23 @@
     >>> sfs.fit(X, y)
     >>> Z = sbs.transform(X)
 
     """
 
     def __init__(
         self,
-        estimator: Estimator = None,
+        estimator: Estimator | None = None,
         n_features: int | float = 1,
-        metric: Evaluator = None,
+        metric: Evaluator | None = None,
         test_size: float = 0.2,
         cv: int = 5,
         shuffle: bool = True,
         stratify: bool = False,
         fold_type: FoldType = KFold,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ) -> None:
         self.estimator = estimator
         self.n_features = n_features
         self.metric = metric
         self.test_size = test_size
         self.cv = cv
@@ -257,15 +277,15 @@
                 "n_features": ("0<,+inf", None),
                 "test_size": ("0,1", float),
                 "cv": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "SFS":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         _, n = X.shape
         self.estimator = Clone(self.estimator).get
 
         if isinstance(self.n_features, float) and 0 < self.n_features < 1:
             self.n_features = np.ceil(n * self.n_features).astype(int)
         elif self.n_features <= 0 or self.n_features > n:
             raise UnsupportedParameterError(self.n_features)
@@ -358,22 +378,30 @@
     coefficients. RFE starts with all features and eliminates a specified
     number or fraction of features at each step. The process continues
     until the desired number of features is reached. This method helps in
     enhancing model performance and interpretability by reducing complexity.
 
     Parameters
     ----------
-    `estimator` : An estimator to fit and evaluate
-    `n_features` : Number of features to select (`0~1` value for proportion)
-    `metric` : Scoring metric for selecting features
-    `step_size` : Number of features to eliminate in each step
-    `cv` : K-fold size for cross validation (`0` to disable CV)
-    `shuffle` : Whether to shuffle the dataset
-    `fold_type` : Fold type (Default `KFold`)
-    `random_state` : Seed for splitting the data
+    `estimator` : Estimator, required optional, default=None
+        An estimator to fit and evaluate
+    `n_features` : int or float
+        Number of features to select (`0~1` value for proportion)
+    `metric` : Evaluator, optional, default=None
+        Scoring metric for selecting features
+    `step_size` : int, default=1
+        Number of features to eliminate in each step
+    `cv` : int, default=5
+        K-fold size for cross validation (`0` to disable CV)
+    `shuffle` : bool, defalut=True
+        Whether to shuffle the dataset
+    `fold_type` : FoldType, default=Kfold
+        Fold type
+    `random_state` : int, optional, default=None
+        Seed for splitting the data
 
     Notes
     -----
     * An instance of the estimator must be passed to `estimator`
     * Do not use the estimator for `RFE` if it is supposed to be the
         main estimator for the model
     * For `metric`, both class or instance are possible
@@ -419,15 +447,15 @@
                 "n_features": ("0<,+inf", None),
                 "step_size": ("0<,+inf", int),
                 "cv": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "RFE":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         _, n = X.shape
         self.estimator = Clone(self.estimator).get
 
         if 0 < self.n_features < 1:
             self.n_features = np.floor(n * self.n_features).astype(int)
         elif self.n_features <= 0 or self.n_features > n:
             raise UnsupportedParameterError(self.n_features)
```

### Comparing `luma-ml-0.7.5/luma/regressor/general.py` & `luma-ml-0.8.0/luma/regressor/general.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,29 +23,34 @@
     It models the relationship between features and counts, with a focus
     on count data that follows a Poisson distribution. The model uses
     the natural logarithm of expected counts as a link function and is
     trained to minimize the negative log-likelihood.
 
     Parameters
     ----------
-    `learning_rate` : Step size of the gradient descent update
-    `max_iter` : Number of iteration
-    `l1_ratio` : Balancing parameter of `elastic-net`
-    `alpha` : Regularization strength
-    `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
+    `learning_rate` : float, default=0.01
+        Step size of the gradient descent update
+    `max_iter` : int, default=100
+        Number of iteration
+    `l1_ratio` : float, default=0.5, range=[0,1]
+        Balancing parameter of `elastic-net`
+    `alpha` : float, default=0.01
+        Regularization strength
+    `regularization` : {"l1", "l2", "elastic-net"}, optional, default=None
+        Regularization type
 
     """
 
     def __init__(
         self,
         learning_rate: float = 0.01,
         max_iter: int = 100,
         l1_ratio: float = 0.5,
         alpha: float = 0.01,
-        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        regularization: Literal["l1", "l2", "elastic-net"] | None = None,
         verbose: bool = False,
     ) -> None:
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.regularization = regularization
         self.l1_ratio = l1_ratio
         self.alpha = alpha
@@ -121,20 +126,26 @@
     model count data, like the number of events or occurrences,
     when the data shows overdispersion (variance is greater than mean)
     compared to the Poisson distribution. It estimates how predictors
     influence the count while allowing for flexible variance modeling.
 
     Parameters
     ----------
-    `learning_rate` : Step size of the gradient descent update
-    `max_iter` : Number of iteration
-    `alpha` : Regularization strength
-    `l1_ratio` : Balancing parameter of `elastic-net`
-    `phi` : Dispersion parameter
-    `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
+    `learning_rate` : float, default=0.01
+        Step size of the gradient descent update
+    `max_iter` : int, default=100
+        Number of iteration
+    `l1_ratio` : float, default=0.5, range=[0,1]
+        Balancing parameter of `elastic-net`
+    `alpha` : float, default=0.01
+        Regularization strength
+    `regularization` : {"l1", "l2", "elastic-net"}, optional, default=None
+        Regularization type
+    `phi` : float, default=1.0
+        Dispersion parameter
 
     """
 
     def __init__(
         self,
         learning_rate: float = 0.01,
         max_iter: int = 100,
@@ -225,21 +236,26 @@
     the variance increases with the mean. It models the
     relationship between variables using the gamma distribution,
     making it suitable for situations where traditional
     linear regression doesn't apply.
 
     Parameters
     ----------
-    `alpha` : Shape parameter of gamma distribution
-    `beta` : Scale parameter of gamma distribution
-    `learning_rate` : Step size of the gradient descent update
-    `max_iter` : Number of iteration
-    `reg_strength` : Regularization strength
-    `l1_ratio` : Balancing parameter of `elastic-net`
-    `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
+    `alpha`, `beta` : float, default=1.0
+        Shape parameter of gamma distribution
+    `learning_rate` : float, default=0.01
+        Step size of the gradient descent update
+    `max_iter` : int, default=100
+        Number of iteration
+    `reg_strength` : float, default=0.01
+        Regularization strength
+    `l1_ratio` : float, default=0.5, range=[0,1]
+        Balancing parameter of `elastic-net`
+    `regularization` : {"l1", "l2", "elastic-net"}, optional, default=None
+        Regularization type
 
     """
 
     def __init__(
         self,
         alpha: float = 1.0,
         beta: float = 1.0,
@@ -337,20 +353,26 @@
     analyze and predict data that follows a bounded interval between
     0 and 1, such as proportions, probabilities, or percentages.
     It's particularly useful for modeling data with heteroscedasticity,
     where the spread of the data varies across different input values.
 
     Parameters
     ----------
-    `alpha`, `beta` : Shape parameters of beta function
-    `learning_rate` : Step size of the gradient descent update
-    `max_iter` : Number of iteration
-    `reg_strength` : Regularization strength
-    `l1_ratio` : Balacing parameter of `elastic-net`
-    `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
+    `alpha`, `beta` : float, default=1.0
+        Shape parameters of beta function
+    `learning_rate` : float, default=1.0
+        Step size of the gradient descent update
+    `max_iter` : int, default=100
+        Number of iteration
+    `reg_strength` : float, default=0.01
+        Regularization strength
+    `l1_ratio` : float, default=0.5, range=[0,1]
+        Balacing parameter of `elastic-net`
+    `regularization` : {"l1", "l2", "elastic-net"}, optional, default=None
+        Regularization type
 
     """
 
     def __init__(
         self,
         alpha: float = 1.0,
         beta: float = 1.0,
@@ -446,20 +468,26 @@
     Inverse Gaussian regression is a statistical technique applied in
     machine learning to model relationships between predictor variables
     and continuous response variables when the response data exhibits
     a skewed or non-normally distributed pattern.
 
     Parameters
     ----------
-    `learning_rate` : Step size of the gradient descent update
-    `max_iter` : Number of iteration
-    `phi` : Shape parameter of inverse Gaussian density
-    `l1_ratio` : Balacing parameter of `elastic-net`
-    `alpha` : Regularization strength
-    `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
+    `learning_rate` : float, default=0.01
+        Step size of the gradient descent update
+    `max_iter` : int, default=100
+        Number of iteration
+    `l1_ratio` : float, default=0.5, range=[0,1]
+        Balancing parameter of `elastic-net`
+    `alpha` : float, default=0.01
+        Regularization strength
+    `regularization` : {"l1", "l2", "elastic-net"}, optional, default=None
+        Regularization type
+    `phi` : float, default=1.0
+        Dispersion parameter
 
     """
 
     def __init__(
         self,
         learning_rate: float = 0.01,
         max_iter: int = 100,
```

### Comparing `luma-ml-0.7.5/luma/regressor/linear.py` & `luma-ml-0.8.0/luma/regressor/linear.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     prevent overfitting in predictive models.
     It adds a penalty term called "L2 regularization" to help
     reduce the complexity of the model and prevent it from
     fitting noise in the data.
 
     Parameters
     ----------
-    `alpha` : L2-regularization strength
+    `alpha` : float, default=1.0
+        L2-regularization strength
 
     """
 
     def __init__(self, alpha: float = 1.0) -> None:
         self.alpha = alpha
         self._fitted = False
 
@@ -67,17 +68,20 @@
     called "L1 regularization," to the standard linear regression
     objective function. Lasso encourages some of the model's
     coef_ to become exactly zero, effectively eliminating
     certain features from the model.
 
     Parameters
     ----------
-    `alpha` : L1-regularization strength
-    `max_iter` : Number of iteration
-    `learning_rate` : Step size of the gradient descent update
+    `alpha` : float, default=1.0
+        L1-regularization strength
+    `max_iter` : int, default=100
+        Number of iteration
+    `learning_rate` : float, default=0.01
+        Step size of the gradient descent update
 
     """
 
     def __init__(
         self,
         alpha: float = 1.0,
         max_iter: int = 100,
@@ -140,18 +144,22 @@
     Elastic-Net regression is a linear regression technique
     that combines both L1 (Lasso) and L2 (Ridge) regularization methods.
     It adds a combination of L1 and L2 penalty terms to the
     standard linear regression objective function.
 
     Parameters
     ----------
-    `alpha` : Regularization strength
-    `l1_ratio` : Balancing parameter between `l1` and `l2`
-    `max_iter` : Number of iteration
-    `learning_rate` : Step size of the gradient descent update
+    `alpha` : float, default=1.0
+        Regularization strength
+    `l1_ratio` : float, default=0.5, range=[0,1]
+        Balancing parameter between `l1` and `l2`
+    `max_iter` : int, default=100
+        Number of iteration
+    `learning_rate` : float, default=0.01
+        Step size of the gradient descent update
 
     """
 
     def __init__(
         self,
         alpha: float = 1.0,
         l1_ratio: float = 0.5,
@@ -256,19 +264,24 @@
     function, KRR maps input data into a higher-dimensional feature space. In this
     transformed space, it minimizes the regularized loss function to find linear
     relationships. KRR excels in capturing complex, non-linear patterns in data,
     making it versatile for various regression tasks.
 
     Parameters
     ----------
-    `alpha` : Regularization strength
-    `deg` : Degree for `poly` kernel
-    `gamma` : Scaling factor for `tanh`, `rbf`, and `laplacian` kernels
-    `coef` : Base coefficient for `linear` and `poly` kernels
-    `kernel` : Kernel functions
+    `alpha` : float, default=1.0
+        Regularization strength
+    `deg` : int, default=2
+        Degree for polynomial kernel
+    `gamma` : float, default=2
+        Scaling factor for Tanh, RBF, sigmoid kernels
+    `coef` : float, default=1.0
+        Base coefficient for linear and polynomial kernels
+    `kernel` : FuncType, default="rbf"
+        Kernel functions
 
     """
 
     def __init__(
         self,
         alpha: float = 1.0,
         deg: int = 2,
@@ -333,20 +346,26 @@
     estimating parameters with uncertainty. It automates regularization,
     balancing data fit and model simplicity. The approach provides both
     point estimates and confidence measures. It's effective for predictive
     modeling with inherent uncertainty.
 
     Parameters
     ----------
-    `alpha_init` : Initial value for the precision of the distribution of noise
-    `lambda_init` : Initial value for the precision of the distribution of weights
+    `alpha_init` : float, optional, default=None
+        Initial value for the precision of the distribution of noise
+    `lambda_init` : float, optional, default=None
+        Initial value for the precision of the distribution of weights
 
     """
 
-    def __init__(self, alpha_init: float = None, lambda_init: float = None) -> None:
+    def __init__(
+        self,
+        alpha_init: float | None = None,
+        lambda_init: float | None = None,
+    ) -> None:
         self.alpha_init = alpha_init
         self.lambda_init = lambda_init
         self._fitted = False
 
         self.set_param_ranges(
             {"alpha_init": ("0<,+inf", None), "lambda_init": ("0<,+inf", None)}
         )
```

### Comparing `luma-ml-0.7.5/luma/regressor/neighbors.py` & `luma-ml-0.8.0/luma/regressor/neighbors.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     Euclidean distance) between the new point and all points in the
     training set, determining the 'k' nearest neighbors, and then
     averaging the values of these neighbors to predict the continuous
     output.
 
     Parameters
     ----------
-    `n_neighbors` : Number of neighbors to be considered close
+    `n_neighbors` : int, default=5
+        Number of neighbors to be considered close
 
     """
 
     def __init__(self, n_neighbors: int = 5):
         self.n_neighbors = n_neighbors
         self._neighbors = None
         self._y = None
@@ -72,17 +73,20 @@
     new data point based on the average values of its neighbors, where the
     number of neighbors (k) is adaptively determined based on the local density
     of the training data. This method allows the algorithm to be more flexible
     and effective, particularly in datasets with varying densities.
 
     Parameters
     ----------
-    `n_density` : Number of nearest neighbors to estimate the local density
-    `min_neighbors` : Minimum number of neighbors to be considered for averaging
-    `max_neighbors` : Maximum number of neighbors to be considered
+    `n_density` : int, default=10
+        Number of nearest neighbors to estimate the local density
+    `min_neighbors` : int, default=5
+        Minimum number of neighbors to be considered for averaging
+    `max_neighbors` : int, default=20
+        Maximum number of neighbors to be considered
 
     """
 
     def __init__(
         self, n_density: int = 10, min_neighbors: int = 5, max_neighbors: int = 20
     ):
         self.n_density = n_density
@@ -146,15 +150,16 @@
     based on their distance from the query point. Closer neighbors exert greater
     influence due to higher weights, commonly calculated using inverse distance weighting.
     This method improves prediction precision, particularly in datasets with
     irregular distributions.
 
     Parameters
     ----------
-    `n_neighbors` : Number of neighbors to be considered close
+    `n_neighbors` : int, default=5
+        Number of neighbors to be considered close
 
     """
 
     def __init__(self, n_neighbors: int = 5):
         self.n_neighbors = n_neighbors
         self._X = None
         self._y = None
```

### Comparing `luma-ml-0.7.5/luma/regressor/poly.py` & `luma-ml-0.8.0/luma/regressor/poly.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,27 +14,31 @@
     """
     Polynomial regression is a type of regression analysis used
     in statistics and machine learning to model the relationship between
     a dependent variable and one or more independent variables.
 
     Parameters
     ----------
-    `deg` : Degree of a polynomial function
-    `alpha` : Regularization strength
-    `l1_ratio` : Balancing parameter between `l1` and `l2`
-    `regularization` : Regularization type (e.g. `l1`, `l2`, `elastic-net`)
+    `deg` : int, default=2
+        Degree of a polynomial function
+    `alpha` : float, default=0.01
+        Regularization strength
+    `l1_ratio` : float, default=0.5, range=[0,1]
+        Balancing parameter between L1 and L2 regularization
+    `regularization` : {"l1", "l2", "elastic-net"}, optional, default=None
+        Regularization type
 
     """
 
     def __init__(
         self,
         deg: int = 2,
         alpha: float = 0.01,
         l1_ratio: float = 0.5,
-        regularization: Literal["l1", "l2", "elastic-net"] = None,
+        regularization: Literal["l1", "l2", "elastic-net"] | None = None,
     ) -> None:
         self.deg = deg
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.regularization = regularization
         self._fitted = False
```

### Comparing `luma-ml-0.7.5/luma/regressor/robust.py` & `luma-ml-0.8.0/luma/regressor/robust.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,20 +20,26 @@
     classifying them as inliers or outliers based on a predefined threshold.
     This process is repeated multiple times, each time selecting a different
     subset. The best model is chosen based on the maximum number of inliers
     it includes.
 
     Parameters
     ----------
-    `estimator` : Regression estimator (Default `LinearRegressor()`)
-    `min_points` : Mininum sample size for each random sample
-    `max_iter` : Maximum iteration
-    `min_inliers` : Minimum number of inliers for a model to be considered valid
-    `threshold` : Maximum distance a point can have to be considered an inlier
-    `random_state` : Seed for random sampling the data
+    `estimator` : Estimator, default=LinearRegressor()
+        Regression estimator
+    `min_points` : int or float, default=2
+        Mininum sample size for each random sample
+    `max_iter` : int, default=1000
+        Maximum iteration
+    `min_inliers` : int or float, default=0.5
+        Minimum number of inliers for a model to be considered valid
+    `threshold` : float, optional, default=None
+        Maximum distance a point can have to be considered an inlier
+    `random_state` : int, optional, default=None
+        Seed for random sampling the data
 
     Properties
     ----------
     Get best estimator:
     ```py
         @property
         def best_estimator(self) -> Estimator
@@ -42,16 +48,16 @@
 
     def __init__(
         self,
         estimator: Estimator = LinearRegressor(),
         min_points: int | float = 2,
         max_iter: int = 1000,
         min_inliers: int | float = 0.5,
-        threshold: float = None,
-        random_state: int = None,
+        threshold: float | None = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ) -> None:
         self.estimator = estimator
         self.min_points = min_points
         self.max_iter = max_iter
         self.min_inliers = min_inliers
         self.threshold = threshold
@@ -158,20 +164,26 @@
     used for robust estimation of parameters from a set of data containing outliers.
     Unlike RANSAC which focuses on maximizing the number of inliers, MLESAC seeks
     to maximize the likelihood of the model given the data, considering both the
     number of inliers and the quality of the fit.
 
     Parameters
     ----------
-    `estimator` : Regression estimator (Default `LinearRegressor()`)
-    `min_points` : Minimum sample size for each random sample
-    `max_iter` : Maximum number of iterations
-    `min_inliers` : Minimum number of inliers for a model to be considered valid
-    `threshold` : Maximum distance a point can have to be considered an inlier
-    `random_state` : Seed for random sampling the data
+    `estimator` : Estimator, default=LinearRegressor()
+        Regression estimator
+    `min_points` : int or float, default=2
+        Minimum sample size for each random sample
+    `max_iter` : int, default=1000
+        Maximum number of iterations
+    `min_inliers` : int or float, default=0.5
+        Minimum number of inliers for a model to be considered valid
+    `threshold` : float, optional, default=None
+        Maximum distance a point can have to be considered an inlier
+    `random_state` : int, optional, default=None
+        Seed for random sampling the data
 
     Properties
     ----------
     Get best estimator:
     ```py
         @property
         def best_estimator(self) -> Estimator
@@ -185,16 +197,16 @@
 
     def __init__(
         self,
         estimator: Estimator = LinearRegressor(),
         min_points: int | float = 2,
         max_iter: int = 1000,
         min_inliers: int | float = 0.5,
-        threshold: float = None,
-        random_state: int = None,
+        threshold: float | None = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ) -> None:
         self.estimator = estimator
         self.min_points = min_points
         self.max_iter = max_iter
         self.min_inliers = min_inliers
         self.threshold = threshold
```

### Comparing `luma-ml-0.7.5/luma/regressor/svm.py` & `luma-ml-0.8.0/luma/regressor/svm.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,19 +16,24 @@
     Support Vector Regressor (SVR) is a supervised machine learning
     algorithm used for regression tasks. It operates by determining a
     hyperplane that best fits the input data, aiming to minimize the
     difference between the predicted and actual values.
 
     Parameters
     ----------
-    `C` : Regularization parameter
-    `epsilon` : Epsilon-tube in the training loss function
-    `batch_size` : Size of a single batch
-    `learning_rate` : Step-size of gradient descent update
-    `max_iter` : Number of iteration
+    `C` : float, default=1.0
+        Regularization parameter
+    `epsilon` : float, default=0.1
+        Epsilon-tube in the training loss function
+    `batch_size` : int, default=100
+        Size of a single batch
+    `learning_rate` : float, default=0.001
+        Step-size of gradient descent update
+    `max_iter` : int, default=1000
+        Number of iteration
 
     """
 
     def __init__(
         self,
         C: float = 1.0,
         epsilon: float = 0.1,
@@ -107,21 +112,28 @@
     Support Vector Regression (SVR) algorithm that enables regression on
     non-linearly related data by mapping it into a higher-dimensional space
     using a kernel function. The kernel function allows the algorithm to
     establish a flexible and non-linear regression model in the transformed space.
 
     Parameters
     ----------
-    `C` : Regularization parameter
-    `deg` : Polynomial Degree for `poly` kernel
-    `gamma` : Shape parameter of Gaussian curve for `rbf` kernel
-    `coef` : Coefficient for `poly`, `sigmoid` kernel
-    `learning_rate` : Step-size for gradient descent update
-    `max_iter` : Number of iteration
-    `kernel` : Type of kernel (e.g., `linear`, `poly`, `rbf`, `sigmoid`)
+    `C` : float, default=1.0
+        Regularization parameter
+    `deg` : int, default=3
+        Polynomial Degree for polynomial kernel
+    `gamma` : float, default=1.0
+        Shape parameter of Gaussian curve for RBF kernel
+    `coef` : float, default=1.0
+        Coefficient for polynomial, sigmoid kernel
+    `learning_rate` : float, default=0.001
+        Step-size for gradient descent update
+    `max_iter` : int, default=1000
+        Number of iteration
+    `kernel` : FuncType, default="rbf"
+        Type of kernel
 
     """
 
     def __init__(
         self,
         C: float = 1.0,
         deg: int = 3,
```

### Comparing `luma-ml-0.7.5/luma/regressor/tree.py` & `luma-ml-0.8.0/luma/regressor/tree.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,33 +19,40 @@
     The regressor works by splitting the data into distinct regions based
     on feature values. At each node of the tree, it chooses the split
     that minimizes the variance (or another specified criterion) of the
     target variable within the regions created by the split.
 
     Parameters
     ----------
-    `max_depth` : Maximum depth of the tree
-    `min_samples_split` : Minimum samples required to split a node
-    `min_samples_leaf` : Minimum samples required to be at a leaf node
-    `max_features` : Number of features to consider
-    `min_variance_decrease` : Minimum decrement of variance for a split
-    `max_leaf_nodes` : Maximum amount of leaf nodes
-    `random_state` : The randomness seed of the estimator
+    `max_depth` : int, default=10
+        Maximum depth of the tree
+    `min_samples_split` : int, default=2
+        Minimum samples required to split a node
+    `min_samples_leaf` : int, default=1
+        Minimum samples required to be at a leaf node
+    `max_features` : int, optional, default=None
+        Number of features to consider
+    `min_variance_decrease` : float, default=0.0
+        Minimum decrement of variance for a split
+    `max_leaf_nodes` : int, optional, default=None
+        Maximum amount of leaf nodes
+    `random_state` : int, optional, default=None
+        The randomness seed of the estimator
 
     """
 
     def __init__(
         self,
         max_depth: int = 10,
         min_samples_split: int = 2,
         min_samples_leaf: int = 1,
-        max_features: int = None,
+        max_features: int | None = None,
         min_variance_decrease: float = 0.0,
-        max_leaf_nodes: int = None,
-        random_state: int = None,
+        max_leaf_nodes: int | None = None,
+        random_state: int | None = None,
     ) -> None:
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.max_features = max_features
         self.min_variance_decrease = min_variance_decrease
         self.max_leaf_nodes = max_leaf_nodes
```

### Comparing `luma-ml-0.7.5/luma/visual/eda.py` & `luma-ml-0.8.0/luma/visual/eda.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.5/luma/visual/evaluation.py` & `luma-ml-0.8.0/luma/visual/evaluation.py`

 * *Files 5% similar despite different names*

```diff
@@ -425,41 +425,52 @@
     the model's error changes as it learns. A steep learning curve indicates rapid
     learning, while a plateau suggests no further learning. The ideal curve shows
     decreasing error on both training and validation datasets, converging to a
     low level.
 
     Parameters
     ----------
-    `estimator` : An estimator to evaluate
-    `X` : Feature data for training
-    `y`: Target data for training
-    `train_sizes` : List of fractional values for each dataset size
-    `test_size` : Proportional value for validation set size
-    `cv` : Number of times for cross-validation
-    `shuffle` : Whether to shuffle the dataset
-    `stratify` : Whether to perform stratified split
-    `fold_type` : Fold type (Default `KFold`)
-    `metric` : Evaluation metric for scoring
-    `random_state` : Seed for random sampling upon splitting samples
+    `estimator` : Estimator
+        An estimator to evaluate
+    `X` : Matrix
+        Feature data for training
+    `y`: Vector
+        Target data for training
+    `train_sizes` : Vector, optional, default=None
+        List of fractional values for each dataset size
+    `test_size` : float, default=0.3
+        Proportional value for validation set size
+    `cv` : int, default=5
+        Number of times for cross-validation
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset
+    `stratify` : bool, default=False
+        Whether to perform stratified split
+    `fold_type` : FoldType, default=KFold
+        Fold type
+    `metric` : Evaluator, default=Accuracy
+        Evaluation metric for scoring
+    `random_state` : int, optional, default=None
+        Seed for random sampling upon splitting samples
 
     """
 
     def __init__(
         self,
         estimator: Estimator,
         X: Matrix,
         y: Vector,
-        train_sizes: Vector = None,
+        train_sizes: Vector | None = None,
         test_size: float = 0.3,
         cv: int = 5,
         shuffle: bool = True,
         stratify: bool = False,
         fold_type: FoldType = KFold,
         metric: Evaluator = Accuracy,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ):
         self.estimator = estimator
         self.X = X
         self.y = y
         self.train_sizes = train_sizes
         self.test_size = test_size
@@ -590,39 +601,49 @@
     A validation curve in machine learning is a graph that compares the performance
     of a model on training and validation data over a range of values for a specific
     hyperparameter. It helps to diagnose the best hyperparameter setting by showing
     how the model's error changes as the value of the hyperparameter changes.
 
     Parameters
     ----------
-    `estimator` : An estimator to evaluate
-    `X` : Feature data for training
-    `y`: Target data for training
-    `param_name` : Name of the hyperparameter to be varied
-    `param_range` : Range of values for the hyperparameter
-    `cv` : Number of times for cross-validation
-    `shuffle` : Whether to shuffle the dataset
-    `fold_type` : Fold type (Default `KFold`)
-    `metric` : Evaluation metric for scoring
-    `random_state` : Seed for random sampling upon splitting samples
+    `estimator` : Estimator
+        An estimator to evaluate
+    `X` : Matrix
+        Feature data for training
+    `y`: Vector
+        Target data for training
+    `param_name` : str
+        Name of the hyperparameter to be varied
+    `param_range` : Vector
+        Range of values for the hyperparameter
+    `cv` : int, default=5
+        Number of times for cross-validation
+    `shuffle` : bool, default=True
+        Whether to shuffle the dataset
+    `fold_type` : FoldType, default=KfFold
+        Fold type
+    `metric` : Evaluator, default=Accuracy
+        Evaluation metric for scoring
+    `random_state` : int, optional, default=None
+        Seed for random sampling upon splitting samples
 
     """
 
     def __init__(
         self,
         estimator: Estimator,
         X: Matrix,
         y: Vector,
         param_name: str,
         param_range: Vector,
         cv: int = 5,
         shuffle: bool = True,
         fold_type: FoldType = KFold,
         metric: Evaluator = Accuracy,
-        random_state: int = None,
+        random_state: int | None = None,
         verbose: bool = False,
     ) -> None:
         self.estimator = estimator
         self.X = X
         self.y = y
         self.param_name = param_name
         self.param_range = param_range
@@ -731,16 +752,18 @@
     indicating better clustering. The plot aids in applying the elbow method for
     selecting a reasonable number of clusters in algorithms like K-means. The
     goal is to choose the number of clusters where inertia begins to decrease
     more slowly.
 
     Parameters
     ----------
-    `inertia_list` : List of inertia values for various cluster sizes
-    `n_clusters_list` : List of the number of clusters
+    `inertia_list` : list for float
+        List of inertia values for various cluster sizes
+    `n_clusters_list` : list of int
+        List of the number of clusters
 
     Examples
     --------
     ```py
     inertia_list = []
     for i in range(2, 10):
         km = KMeansClustering(n_clusters=i)
```

### Comparing `luma-ml-0.7.5/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.8.0/luma_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.5
+Version: 0.8.0
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.50k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.56k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.5</td>
+                    <td>0.8.0</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~21K</td>
+                    <td>~22K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.5 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.8.0 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.50k-red][GitHub code size in bytes][Code Style]
+5.56k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.5
-Lines of Code  ~21K
+Latest Version 0.8.0
+Lines of Code  ~22K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.5/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.8.0/luma_ml.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -71,9 +71,8 @@
 luma/visual/evaluation.py
 luma_ml.egg-info/PKG-INFO
 luma_ml.egg-info/SOURCES.txt
 luma_ml.egg-info/dependency_links.txt
 luma_ml.egg-info/requires.txt
 luma_ml.egg-info/top_level.txt
 test/__act.py
-test/__local__.py
 test/__test.py
```

### Comparing `luma-ml-0.7.5/setup.py` & `luma-ml-0.8.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.7.5",
+    version="0.8.0",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/luma",
     packages=setuptools.find_namespace_packages(),
```

### Comparing `luma-ml-0.7.5/test/__act.py` & `luma-ml-0.8.0/test/__act.py`

 * *Files identical despite different names*

