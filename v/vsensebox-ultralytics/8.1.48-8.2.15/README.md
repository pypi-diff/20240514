# Comparing `tmp/vsensebox_ultralytics-8.1.48.tar.gz` & `tmp/vsensebox_ultralytics-8.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsensebox_ultralytics-8.1.48.tar", last modified: Thu May  2 12:37:35 2024, max compression
+gzip compressed data, was "vsensebox_ultralytics-8.2.15.tar", last modified: Tue May 14 14:11:06 2024, max compression
```

## Comparing `vsensebox_ultralytics-8.1.48.tar` & `vsensebox_ultralytics-8.2.15.tar`

### file list

```diff
@@ -1,258 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.703609 vsensebox_ultralytics-8.1.48/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-02 12:37:35.703609 vsensebox_ultralytics-8.1.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-02 12:37:35.703609 vsensebox_ultralytics-8.1.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.659608 vsensebox_ultralytics-8.1.48/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    22858 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.659608 vsensebox_ultralytics-8.1.48/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.659608 vsensebox_ultralytics-8.1.48/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.663608 vsensebox_ultralytics-8.1.48/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.667609 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/DOTAv1.5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/DOTAv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/african-wildlife.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/brain-tumor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/carparts-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/crack-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/dota8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/lvis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/open-images-v7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/package-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/tiger-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.655609 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.667609 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.667609 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.667609 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.667609 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.671609 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-obb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-world.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.671609 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v9/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v9/yolov9c-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v9/yolov9c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v9/yolov9e-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v9/yolov9e.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.671609 vsensebox_ultralytics-8.1.48/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.675608 vsensebox_ultralytics-8.1.48/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57741 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.675608 vsensebox_ultralytics-8.1.48/ultralytics/data/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.675608 vsensebox_ultralytics-8.1.48/ultralytics/data/explorer/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/explorer/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/explorer/gui/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/explorer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/split_dota.py
--rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.675608 vsensebox_ultralytics-8.1.48/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54476 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    40019 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    34933 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/engine/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14645 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.679609 vsensebox_ultralytics-8.1.48/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.679609 vsensebox_ultralytics-8.1.48/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.679609 vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.679609 vsensebox_ultralytics-8.1.48/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.679609 vsensebox_ultralytics-8.1.48/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.683609 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.683609 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.683609 vsensebox_ultralytics-8.1.48/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.683609 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.683609 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.683609 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.687609 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/obb/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/obb/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/obb/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.687609 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.687609 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.687609 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/world/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/world/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/world/train_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.687609 vsensebox_ultralytics-8.1.48/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30438 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.691609 vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.691609 vsensebox_ultralytics-8.1.48/ultralytics/solutions/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/solutions/ai_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/solutions/distance_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/solutions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/solutions/object_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/solutions/queue_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/solutions/speed_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.691609 vsensebox_ultralytics-8.1.48/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.691609 vsensebox_ultralytics-8.1.48/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.695609 vsensebox_ultralytics-8.1.48/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    39294 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18325 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.699609 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (127)    28284 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    47558 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (127)    25848 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-02 12:37:24.000000 vsensebox_ultralytics-8.1.48/ultralytics/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:37:35.699609 vsensebox_ultralytics-8.1.48/vsensebox_ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-02 12:37:35.000000 vsensebox_ultralytics-8.1.48/vsensebox_ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-05-02 12:37:35.000000 vsensebox_ultralytics-8.1.48/vsensebox_ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:37:35.000000 vsensebox_ultralytics-8.1.48/vsensebox_ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 12:37:35.000000 vsensebox_ultralytics-8.1.48/vsensebox_ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 12:37:35.000000 vsensebox_ultralytics-8.1.48/vsensebox_ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-02 12:37:35.000000 vsensebox_ultralytics-8.1.48/vsensebox_ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.328057 vsensebox_ultralytics-8.2.15/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-14 14:11:06.328057 vsensebox_ultralytics-8.2.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-14 14:11:06.328057 vsensebox_ultralytics-8.2.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.292057 vsensebox_ultralytics-8.2.15/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.296057 vsensebox_ultralytics-8.2.15/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.296057 vsensebox_ultralytics-8.2.15/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.296057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)    21358 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.300057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/DOTAv1.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/DOTAv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/african-wildlife.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/brain-tumor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/carparts-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/crack-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/dota8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/lvis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/open-images-v7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/package-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/tiger-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.288057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.300057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.300057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.300057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.300057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.304057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-obb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-world.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.304057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9c-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9e-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9e.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.304057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57665 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/gui/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/split_dota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31051 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58122 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40103 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30919 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35048 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/train_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.320057 vsensebox_ultralytics-8.2.15/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30866 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.320057 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22236 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.320057 vsensebox_ultralytics-8.2.15/ultralytics/solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/ai_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/distance_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/object_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/parking_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/queue_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/speed_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.320057 vsensebox_ultralytics-8.2.15/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.320057 vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.324057 vsensebox_ultralytics-8.2.15/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    39520 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23552 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.328057 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28375 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15654 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48466 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.328057 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/top_level.txt
```

### Comparing `vsensebox_ultralytics-8.1.48/LICENSE` & `vsensebox_ultralytics-8.2.15/LICENSE`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/PKG-INFO` & `vsensebox_ultralytics-8.2.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsensebox-ultralytics
-Version: 8.1.48
+Version: 8.2.15
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/rathaumons/ultralytics-for-vsensebox
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/rathaumons/ultralytics-for-vsensebox/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/rathaumons/ultralytics-for-vsensebox
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics
@@ -51,16 +51,16 @@
 Requires-Dist: duckdb<=0.9.2; extra == "explorer"
 Requires-Dist: streamlit; extra == "explorer"
 
 [![Test Build](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml) [![PyPI](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml)
 
 # Customized Ultralytics for VSenseBox
 
-* Updated: **May 2, 2024**
-* Synced with: v8.1.48 -> [[c54b013]](https://github.com/ultralytics/ultralytics/commit/c54b013188870dafdd5ce0d78b3f5f3fdee655fd)
+* Updated: **May 14, 2024**
+* Synced with: v8.2.15 -> [[590002f]](https://github.com/ultralytics/ultralytics/commit/590002ff6d3a936b0cb1aeb582ea2daa26fcdbb6)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
 * Customized for [`VSenseBox`](https://github.com/rathaumons/vsensebox):
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
```

### Comparing `vsensebox_ultralytics-8.1.48/README.md` & `vsensebox_ultralytics-8.2.15/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Test Build](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml) [![PyPI](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml)
 
 # Customized Ultralytics for VSenseBox
 
-* Updated: **May 2, 2024**
-* Synced with: v8.1.48 -> [[c54b013]](https://github.com/ultralytics/ultralytics/commit/c54b013188870dafdd5ce0d78b3f5f3fdee655fd)
+* Updated: **May 14, 2024**
+* Synced with: v8.2.15 -> [[590002f]](https://github.com/ultralytics/ultralytics/commit/590002ff6d3a936b0cb1aeb582ea2daa26fcdbb6)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
 * Customized for [`VSenseBox`](https://github.com/rathaumons/vsensebox):
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
```

### Comparing `vsensebox_ultralytics-8.1.48/requirements.txt` & `vsensebox_ultralytics-8.2.15/requirements.txt`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/setup.cfg` & `vsensebox_ultralytics-8.2.15/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/setup.py` & `vsensebox_ultralytics-8.2.15/setup.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/tests/conftest.py` & `vsensebox_ultralytics-8.2.15/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/tests/test_cli.py` & `vsensebox_ultralytics-8.2.15/tests/test_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import subprocess
 
 import pytest
 
+from ultralytics.cfg import TASK2DATA, TASK2MODEL, TASKS
 from ultralytics.utils import ASSETS, WEIGHTS_DIR, checks
 
-CUDA_IS_AVAILABLE = checks.cuda_is_available()
-CUDA_DEVICE_COUNT = checks.cuda_device_count()
-TASK_ARGS = [
-    ("detect", "yolov8n", "coco8.yaml"),
-    ("segment", "yolov8n-seg", "coco8-seg.yaml"),
-    ("classify", "yolov8n-cls", "imagenet10"),
-    ("pose", "yolov8n-pose", "coco8-pose.yaml"),
-    ("obb", "yolov8n-obb", "dota8.yaml"),
-]  # (task, model, data)
-EXPORT_ARGS = [
-    ("yolov8n", "torchscript"),
-    ("yolov8n-seg", "torchscript"),
-    ("yolov8n-cls", "torchscript"),
-    ("yolov8n-pose", "torchscript"),
-    ("yolov8n-obb", "torchscript"),
-]  # (model, format)
+from . import CUDA_DEVICE_COUNT, CUDA_IS_AVAILABLE
+
+# Constants
+TASK_MODEL_DATA = [(task, WEIGHTS_DIR / TASK2MODEL[task], TASK2DATA[task]) for task in TASKS]
+MODELS = [WEIGHTS_DIR / TASK2MODEL[task] for task in TASKS]
 
 
 def run(cmd):
     """Execute a shell command using subprocess."""
     subprocess.run(cmd.split(), check=True)
 
 
@@ -34,42 +24,42 @@
     run("yolo help")
     run("yolo checks")
     run("yolo version")
     run("yolo settings reset")
     run("yolo cfg")
 
 
-@pytest.mark.parametrize("task,model,data", TASK_ARGS)
+@pytest.mark.parametrize("task,model,data", TASK_MODEL_DATA)
 def test_train(task, model, data):
     """Test YOLO training for a given task, model, and data."""
-    run(f"yolo train {task} model={model}.yaml data={data} imgsz=32 epochs=1 cache=disk")
+    run(f"yolo train {task} model={model} data={data} imgsz=32 epochs=1 cache=disk")
 
 
-@pytest.mark.parametrize("task,model,data", TASK_ARGS)
+@pytest.mark.parametrize("task,model,data", TASK_MODEL_DATA)
 def test_val(task, model, data):
     """Test YOLO validation for a given task, model, and data."""
-    run(f"yolo val {task} model={WEIGHTS_DIR / model}.pt data={data} imgsz=32 save_txt save_json")
+    run(f"yolo val {task} model={model} data={data} imgsz=32 save_txt save_json")
 
 
-@pytest.mark.parametrize("task,model,data", TASK_ARGS)
+@pytest.mark.parametrize("task,model,data", TASK_MODEL_DATA)
 def test_predict(task, model, data):
     """Test YOLO prediction on sample assets for a given task and model."""
-    run(f"yolo predict model={WEIGHTS_DIR / model}.pt source={ASSETS} imgsz=32 save save_crop save_txt")
+    run(f"yolo predict model={model} source={ASSETS} imgsz=32 save save_crop save_txt")
 
 
-@pytest.mark.parametrize("model,format", EXPORT_ARGS)
-def test_export(model, format):
+@pytest.mark.parametrize("model", MODELS)
+def test_export(model):
     """Test exporting a YOLO model to different formats."""
-    run(f"yolo export model={WEIGHTS_DIR / model}.pt format={format} imgsz=32")
+    run(f"yolo export model={model} format=torchscript imgsz=32")
 
 
 def test_rtdetr(task="detect", model="yolov8n-rtdetr.yaml", data="coco8.yaml"):
     """Test the RTDETR functionality with the Ultralytics framework."""
-    # Warning: MUST use imgsz=640
-    run(f"yolo train {task} model={model} data={data} --imgsz= 160 epochs =1, cache = disk")  # add coma, spaces to args
+    # Warning: must use imgsz=640 (note also add coma, spaces, fraction=0.25 args to test single-image training)
+    run(f"yolo train {task} model={model} data={data} --imgsz= 160 epochs =1, cache = disk fraction=0.25")
     run(f"yolo predict {task} model={model} source={ASSETS / 'bus.jpg'} imgsz=160 save save_crop save_txt")
 
 
 @pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="MobileSAM with CLIP is not supported in Python 3.12")
 def test_fastsam(task="segment", model=WEIGHTS_DIR / "FastSAM-s.pt", data="coco8-seg.yaml"):
     """Test FastSAM segmentation functionality within Ultralytics."""
     source = ASSETS / "bus.jpg"
@@ -125,14 +115,14 @@
 
     # Predict all
     # model(source)
 
 
 # Slow Tests -----------------------------------------------------------------------------------------------------------
 @pytest.mark.slow
-@pytest.mark.parametrize("task,model,data", TASK_ARGS)
+@pytest.mark.parametrize("task,model,data", TASK_MODEL_DATA)
 @pytest.mark.skipif(not CUDA_IS_AVAILABLE, reason="CUDA is not available")
 @pytest.mark.skipif(CUDA_DEVICE_COUNT < 2, reason="DDP is not available")
 def test_train_gpu(task, model, data):
     """Test YOLO training on GPU(s) for various tasks and models."""
-    run(f"yolo train {task} model={model}.yaml data={data} imgsz=32 epochs=1 device=0")  # single GPU
-    run(f"yolo train {task} model={model}.pt data={data} imgsz=32 epochs=1 device=0,1")  # multi GPU
+    run(f"yolo train {task} model={model} data={data} imgsz=32 epochs=1 device=0")  # single GPU
+    run(f"yolo train {task} model={model} data={data} imgsz=32 epochs=1 device=0,1")  # multi GPU
```

### Comparing `vsensebox_ultralytics-8.1.48/tests/test_engine.py` & `vsensebox_ultralytics-8.2.15/tests/test_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,60 +5,57 @@
 
 from ultralytics import YOLO
 from ultralytics.cfg import get_cfg
 from ultralytics.engine.exporter import Exporter
 from ultralytics.models.yolo import classify, detect, segment
 from ultralytics.utils import ASSETS, DEFAULT_CFG, WEIGHTS_DIR
 
-CFG_DET = "yolov8n.yaml"
-CFG_SEG = "yolov8n-seg.yaml"
-CFG_CLS = "yolov8n-cls.yaml"  # or 'squeezenet1_0'
-CFG = get_cfg(DEFAULT_CFG)
-MODEL = WEIGHTS_DIR / "yolov8n"
+from . import MODEL
 
 
 def test_func(*args):  # noqa
     """Test function callback."""
     print("callback test passed")
 
 
 def test_export():
     """Test model exporting functionality."""
     exporter = Exporter()
     exporter.add_callback("on_export_start", test_func)
     assert test_func in exporter.callbacks["on_export_start"], "callback test failed"
-    f = exporter(model=YOLO(CFG_DET).model)
+    f = exporter(model=YOLO("yolov8n.yaml").model)
     YOLO(f)(ASSETS)  # exported model inference
 
 
 def test_detect():
     """Test object detection functionality."""
-    overrides = {"data": "coco8.yaml", "model": CFG_DET, "imgsz": 32, "epochs": 1, "save": False}
-    CFG.data = "coco8.yaml"
-    CFG.imgsz = 32
+    overrides = {"data": "coco8.yaml", "model": "yolov8n.yaml", "imgsz": 32, "epochs": 1, "save": False}
+    cfg = get_cfg(DEFAULT_CFG)
+    cfg.data = "coco8.yaml"
+    cfg.imgsz = 32
 
     # Trainer
     trainer = detect.DetectionTrainer(overrides=overrides)
     trainer.add_callback("on_train_start", test_func)
     assert test_func in trainer.callbacks["on_train_start"], "callback test failed"
     trainer.train()
 
     # Validator
-    val = detect.DetectionValidator(args=CFG)
+    val = detect.DetectionValidator(args=cfg)
     val.add_callback("on_val_start", test_func)
     assert test_func in val.callbacks["on_val_start"], "callback test failed"
     val(model=trainer.best)  # validate best.pt
 
     # Predictor
     pred = detect.DetectionPredictor(overrides={"imgsz": [64, 64]})
     pred.add_callback("on_predict_start", test_func)
     assert test_func in pred.callbacks["on_predict_start"], "callback test failed"
     # Confirm there is no issue with sys.argv being empty.
     with mock.patch.object(sys, "argv", []):
-        result = pred(source=ASSETS, model=f"{MODEL}.pt")
+        result = pred(source=ASSETS, model=MODEL)
         assert len(result), "predictor test failed"
 
     overrides["resume"] = trainer.last
     trainer = detect.DetectionTrainer(overrides=overrides)
     try:
         trainer.train()
     except Exception as e:
@@ -66,36 +63,37 @@
         return
 
     Exception("Resume test failed!")
 
 
 def test_segment():
     """Test image segmentation functionality."""
-    overrides = {"data": "coco8-seg.yaml", "model": CFG_SEG, "imgsz": 32, "epochs": 1, "save": False}
-    CFG.data = "coco8-seg.yaml"
-    CFG.imgsz = 32
+    overrides = {"data": "coco8-seg.yaml", "model": "yolov8n-seg.yaml", "imgsz": 32, "epochs": 1, "save": False}
+    cfg = get_cfg(DEFAULT_CFG)
+    cfg.data = "coco8-seg.yaml"
+    cfg.imgsz = 32
     # YOLO(CFG_SEG).train(**overrides)  # works
 
     # Trainer
     trainer = segment.SegmentationTrainer(overrides=overrides)
     trainer.add_callback("on_train_start", test_func)
     assert test_func in trainer.callbacks["on_train_start"], "callback test failed"
     trainer.train()
 
     # Validator
-    val = segment.SegmentationValidator(args=CFG)
+    val = segment.SegmentationValidator(args=cfg)
     val.add_callback("on_val_start", test_func)
     assert test_func in val.callbacks["on_val_start"], "callback test failed"
     val(model=trainer.best)  # validate best.pt
 
     # Predictor
     pred = segment.SegmentationPredictor(overrides={"imgsz": [64, 64]})
     pred.add_callback("on_predict_start", test_func)
     assert test_func in pred.callbacks["on_predict_start"], "callback test failed"
-    result = pred(source=ASSETS, model=f"{MODEL}-seg.pt")
+    result = pred(source=ASSETS, model=WEIGHTS_DIR / "yolov8n-seg.pt")
     assert len(result), "predictor test failed"
 
     # Test resume
     overrides["resume"] = trainer.last
     trainer = segment.SegmentationTrainer(overrides=overrides)
     try:
         trainer.train()
@@ -104,27 +102,28 @@
         return
 
     Exception("Resume test failed!")
 
 
 def test_classify():
     """Test image classification functionality."""
-    overrides = {"data": "imagenet10", "model": CFG_CLS, "imgsz": 32, "epochs": 1, "save": False}
-    CFG.data = "imagenet10"
-    CFG.imgsz = 32
+    overrides = {"data": "imagenet10", "model": "yolov8n-cls.yaml", "imgsz": 32, "epochs": 1, "save": False}
+    cfg = get_cfg(DEFAULT_CFG)
+    cfg.data = "imagenet10"
+    cfg.imgsz = 32
     # YOLO(CFG_SEG).train(**overrides)  # works
 
     # Trainer
     trainer = classify.ClassificationTrainer(overrides=overrides)
     trainer.add_callback("on_train_start", test_func)
     assert test_func in trainer.callbacks["on_train_start"], "callback test failed"
     trainer.train()
 
     # Validator
-    val = classify.ClassificationValidator(args=CFG)
+    val = classify.ClassificationValidator(args=cfg)
     val.add_callback("on_val_start", test_func)
     assert test_func in val.callbacks["on_val_start"], "callback test failed"
     val(model=trainer.best)
 
     # Predictor
     pred = classify.ClassificationPredictor(overrides={"imgsz": [64, 64]})
     pred.add_callback("on_predict_start", test_func)
```

### Comparing `vsensebox_ultralytics-8.1.48/tests/test_python.py` & `vsensebox_ultralytics-8.2.15/tests/test_python.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,38 +8,31 @@
 import numpy as np
 import pytest
 import torch
 import yaml
 from PIL import Image
 
 from ultralytics import RTDETR, YOLO
-from ultralytics.cfg import TASK2DATA
+from ultralytics.cfg import MODELS, TASKS, TASK2DATA
 from ultralytics.data.build import load_inference_source
 from ultralytics.utils import (
     ASSETS,
     DEFAULT_CFG,
     DEFAULT_CFG_PATH,
-    LINUX,
-    MACOS,
     ONLINE,
     ROOT,
     WEIGHTS_DIR,
     WINDOWS,
     Retry,
     checks,
-    is_dir_writeable,
 )
 from ultralytics.utils.downloads import download
-from ultralytics.utils.torch_utils import TORCH_1_9, TORCH_1_13
+from ultralytics.utils.torch_utils import TORCH_1_9
 
-MODEL = WEIGHTS_DIR / "path with spaces" / "yolov8n.pt"  # test spaces in path
-CFG = "yolov8n.yaml"
-SOURCE = ASSETS / "bus.jpg"
-TMP = (ROOT / "../tests/tmp").resolve()  # temp directory for test files
-IS_TMP_WRITEABLE = is_dir_writeable(TMP)
+from . import CFG, IS_TMP_WRITEABLE, MODEL, SOURCE, TMP
 
 
 def test_model_forward():
     """Test the forward pass of the YOLO model."""
     model = YOLO(CFG)
     model(source=None, imgsz=32, augment=True)  # also test no source and augment
 
@@ -79,50 +72,41 @@
     txt_file = TMP / "sources.txt"
     with open(txt_file, "w") as f:
         for x in [ASSETS / "bus.jpg", ASSETS, ASSETS / "*", ASSETS / "**/*.jpg"]:
             f.write(f"{x}\n")
     _ = YOLO(MODEL)(source=txt_file, imgsz=32)
 
 
-def test_predict_img():
+@pytest.mark.parametrize("model_name", MODELS)
+def test_predict_img(model_name):
     """Test YOLO prediction on various types of image sources."""
-    model = YOLO(MODEL)
-    seg_model = YOLO(WEIGHTS_DIR / "yolov8n-seg.pt")
-    cls_model = YOLO(WEIGHTS_DIR / "yolov8n-cls.pt")
-    pose_model = YOLO(WEIGHTS_DIR / "yolov8n-pose.pt")
-    obb_model = YOLO(WEIGHTS_DIR / "yolov8n-obb.pt")
-    im = cv2.imread(str(SOURCE))
+    model = YOLO(WEIGHTS_DIR / model_name)
+    im = cv2.imread(str(SOURCE))  # uint8 numpy array
     assert len(model(source=Image.open(SOURCE), save=True, verbose=True, imgsz=32)) == 1  # PIL
     assert len(model(source=im, save=True, save_txt=True, imgsz=32)) == 1  # ndarray
+    assert len(model(torch.rand((2, 3, 32, 32)), imgsz=32)) == 2  # batch-size 2 Tensor, FP32 0.0-1.0 RGB order
     assert len(model(source=[im, im], save=True, save_txt=True, imgsz=32)) == 2  # batch
     assert len(list(model(source=[im, im], save=True, stream=True, imgsz=32))) == 2  # stream
-    assert len(model(torch.zeros(320, 640, 3).numpy(), imgsz=32)) == 1  # tensor to numpy
+    assert len(model(torch.zeros(320, 640, 3).numpy().astype(np.uint8), imgsz=32)) == 1  # tensor to numpy
     batch = [
         str(SOURCE),  # filename
         Path(SOURCE),  # Path
         "https://ultralytics.com/images/zidane.jpg" if ONLINE else SOURCE,  # URI
         cv2.imread(str(SOURCE)),  # OpenCV
         Image.open(SOURCE),  # PIL
-        np.zeros((320, 640, 3)),
-    ]  # numpy
+        np.zeros((320, 640, 3), dtype=np.uint8),  # numpy
+    ]
     assert len(model(batch, imgsz=32)) == len(batch)  # multiple sources in a batch
 
-    # Test tensor inference
-    im = torch.rand((4, 3, 32, 32))  # batch-size 4, FP32 0.0-1.0 RGB order
-    results = model(im, imgsz=32)
-    assert len(results) == im.shape[0]
-    results = seg_model(im, imgsz=32)
-    assert len(results) == im.shape[0]
-    results = cls_model(im, imgsz=32)
-    assert len(results) == im.shape[0]
-    results = pose_model(im, imgsz=32)
-    assert len(results) == im.shape[0]
-    results = obb_model(im, imgsz=32)
-    assert len(results) == im.shape[0]
 
+@pytest.mark.parametrize("model", MODELS)
+def test_predict_visualize(model):
+    """Test model predict methods with 'visualize=True' arguments."""
+    YOLO(WEIGHTS_DIR / model)(SOURCE, imgsz=32, visualize=True)
+    
 
 def test_predict_grey_and_4ch():
     """Test YOLO prediction on SOURCE converted to greyscale and 4-channel images."""
     im = Image.open(SOURCE)
     directory = TMP / "im4"
     directory.mkdir(parents=True, exist_ok=True)
 
@@ -197,86 +181,14 @@
 def test_train_pretrained():
     """Test training the YOLO model from a pre-trained state."""
     model = YOLO(WEIGHTS_DIR / "yolov8n-seg.pt")
     model.train(data="coco8-seg.yaml", epochs=1, imgsz=32, cache="ram", copy_paste=0.5, mixup=0.5, name=0)
     model(SOURCE)
 
 
-def test_export_torchscript():
-    """Test exporting the YOLO model to TorchScript format."""
-    f = YOLO(MODEL).export(format="torchscript", optimize=False)
-    YOLO(f)(SOURCE)  # exported model inference
-
-
-def test_export_onnx():
-    """Test exporting the YOLO model to ONNX format."""
-    f = YOLO(MODEL).export(format="onnx", dynamic=True)
-    YOLO(f)(SOURCE)  # exported model inference
-
-
-@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="OpenVINO not supported in Python 3.12")
-@pytest.mark.skipif(not TORCH_1_13, reason="OpenVINO requires torch>=1.13")
-def test_export_openvino():
-    """Test exporting the YOLO model to OpenVINO format."""
-    f = YOLO(MODEL).export(format="openvino")
-    YOLO(f)(SOURCE)  # exported model inference
-
-
-@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="CoreML not supported in Python 3.12")
-def test_export_coreml():
-    """Test exporting the YOLO model to CoreML format."""
-    if not WINDOWS:  # RuntimeError: BlobWriter not loaded with coremltools 7.0 on windows
-        if MACOS:
-            f = YOLO(MODEL).export(format="coreml")
-            YOLO(f)(SOURCE)  # model prediction only supported on macOS for nms=False models
-        else:
-            YOLO(MODEL).export(format="coreml", nms=True)
-
-
-def test_export_tflite(enabled=False):
-    """
-    Test exporting the YOLO model to TFLite format.
-
-    Note TF suffers from install conflicts on Windows and macOS.
-    """
-    if enabled and LINUX:
-        model = YOLO(MODEL)
-        f = model.export(format="tflite")
-        YOLO(f)(SOURCE)
-
-
-def test_export_pb(enabled=False):
-    """
-    Test exporting the YOLO model to *.pb format.
-
-    Note TF suffers from install conflicts on Windows and macOS.
-    """
-    if enabled and LINUX:
-        model = YOLO(MODEL)
-        f = model.export(format="pb")
-        YOLO(f)(SOURCE)
-
-
-def test_export_paddle(enabled=False):
-    """
-    Test exporting the YOLO model to Paddle format.
-
-    Note Paddle protobuf requirements conflicting with onnx protobuf requirements.
-    """
-    if enabled:
-        YOLO(MODEL).export(format="paddle")
-
-
-@pytest.mark.slow
-def test_export_ncnn():
-    """Test exporting the YOLO model to NCNN format."""
-    f = YOLO(MODEL).export(format="ncnn")
-    YOLO(f)(SOURCE)  # exported model inference
-
-
 def test_all_model_yamls():
     """Test YOLO model creation for all available YAML configurations."""
     for m in (ROOT / "cfg" / "models").rglob("*.yaml"):
         if "rtdetr" in m.name:
             if TORCH_1_9:  # torch<=1.8 issue - TypeError: __init__() got an unexpected keyword argument 'batch_first'
                 _ = RTDETR(m.name)(SOURCE, imgsz=640)  # must be 640
         else:
@@ -285,15 +197,15 @@
 
 def test_workflow():
     """Test the complete workflow including training, validation, prediction, and exporting."""
     model = YOLO(MODEL)
     model.train(data="coco8.yaml", epochs=1, imgsz=32, optimizer="SGD")
     model.val(imgsz=32)
     model.predict(SOURCE, imgsz=32)
-    model.export(format="onnx")  # export a model to ONNX format
+    model.export(format="torchscript")
 
 
 def test_predict_callback_and_setup():
     """Test callback functionality during YOLO prediction."""
 
     def on_predict_batch_end(predictor):
         """Callback function that handles operations at the end of a prediction batch."""
@@ -311,61 +223,61 @@
     for r, im0, bs in results:
         print("test_callback", im0.shape)
         print("test_callback", bs)
         boxes = r.boxes  # Boxes object for bbox outputs
         print(boxes)
 
 
-def test_results():
+@pytest.mark.parametrize("model", MODELS)
+def test_results(model):
     """Test various result formats for the YOLO model."""
-    for m in "yolov8n-pose.pt", "yolov8n-seg.pt", "yolov8n.pt", "yolov8n-cls.pt":
-        results = YOLO(WEIGHTS_DIR / m)([SOURCE, SOURCE], imgsz=160)
-        for r in results:
-            r = r.cpu().numpy()
-            r = r.to(device="cpu", dtype=torch.float32)
-            r.save_txt(txt_file=TMP / "runs/tests/label.txt", save_conf=True)
-            r.save_crop(save_dir=TMP / "runs/tests/crops/")
-            r.tojson(normalize=True)
-            r.plot(pil=True)
-            r.plot(conf=True, boxes=True)
-            print(r, len(r), r.path)
+    results = YOLO(WEIGHTS_DIR / model)([SOURCE, SOURCE], imgsz=160)
+    for r in results:
+        r = r.cpu().numpy()
+        r = r.to(device="cpu", dtype=torch.float32)
+        r.save_txt(txt_file=TMP / "runs/tests/label.txt", save_conf=True)
+        r.save_crop(save_dir=TMP / "runs/tests/crops/")
+        r.tojson(normalize=True)
+        r.plot(pil=True)
+        r.plot(conf=True, boxes=True)
+        print(r, len(r), r.path)
 
 
 def test_labels_and_crops():
     """Test output from prediction args for saving detection labels and crops."""
     imgs = [SOURCE, ASSETS / "zidane.jpg"]
     results = YOLO(WEIGHTS_DIR / "yolov8n.pt")(imgs, imgsz=160, save_txt=True, save_crop=True)
     save_path = Path(results[0].save_dir)
     for r in results:
         im_name = Path(r.path).stem
         cls_idxs = r.boxes.cls.int().tolist()
         # Check label path
         labels = save_path / f"labels/{im_name}.txt"
         assert labels.exists()
         # Check detections match label count
-        assert len(r.boxes.data) == len([l for l in labels.read_text().splitlines() if l])
+        assert len(r.boxes.data) == len([line for line in labels.read_text().splitlines() if line])
         # Check crops path and files
-        crop_dirs = [p for p in (save_path / "crops").iterdir()]
+        crop_dirs = list((save_path / "crops").iterdir())
         crop_files = [f for p in crop_dirs for f in p.glob("*")]
         # Crop directories match detections
-        assert all([r.names.get(c) in {d.name for d in crop_dirs} for c in cls_idxs])
+        assert all(r.names.get(c) in {d.name for d in crop_dirs} for c in cls_idxs)
         # Same number of crops as detections
         assert len([f for f in crop_files if im_name in f.name]) == len(r.boxes.data)
 
 
 @pytest.mark.skipif(not ONLINE, reason="environment is offline")
 def test_data_utils():
     """Test utility functions in ultralytics/data/utils.py."""
     from ultralytics.data.utils import HUBDatasetStats, autosplit
     from ultralytics.utils.downloads import zip_directory
 
     # from ultralytics.utils.files import WorkingDirectory
     # with WorkingDirectory(ROOT.parent / 'tests'):
 
-    for task in "detect", "segment", "pose", "classify":
+    for task in TASKS:
         file = Path(TASK2DATA[task]).with_suffix(".zip")  # i.e. coco8.zip
         download(f"https://github.com/ultralytics/hub/raw/main/example_datasets/{file}", unzip=False, dir=TMP)
         stats = HUBDatasetStats(TMP / file, task=task)
         stats.get_json(save=True)
         stats.process_images()
 
     autosplit(TMP / "coco8")
@@ -429,20 +341,20 @@
 
 def test_utils_checks():
     """Test various utility checks."""
     checks.check_yolov5u_filename("yolov5n.pt")
     checks.git_describe(ROOT)
     checks.check_requirements()  # check requirements.txt
     checks.check_imgsz([600, 600], max_dim=1)
-    checks.check_imshow()
+    checks.check_imshow(warn=True)
     checks.check_version("ultralytics", "8.0.0")
     checks.print_args()
-    # checks.check_imshow(warn=True)
 
 
+@pytest.mark.skipif(WINDOWS, reason="Windows profiling is extremely slow (cause unknown)")
 def test_utils_benchmarks():
     """Test model benchmarking."""
     from ultralytics.utils.benchmarks import ProfileModels
 
     ProfileModels(["yolov8n.yaml"], imgsz=32, min_time=1, num_timed_runs=3, num_warmup_runs=1).profile()
 
 
@@ -630,35 +542,35 @@
     for batch in [SOURCE], [SOURCE, SOURCE]:  # test batch size 1 and 2
         assert len(model_detect.embed(source=batch, imgsz=32)) == len(batch)
         assert len(model_segment.embed(source=batch, imgsz=32)) == len(batch)
 
 
 @pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="YOLOWorld with CLIP is not supported in Python 3.12")
 def test_yolo_world():
+    """Tests YOLO world models with different configurations, including classes, detection, and training scenarios."""
     model = YOLO("yolov8s-world.pt")  # no YOLOv8n-world model yet
     model.set_classes(["tree", "window"])
-    model(ASSETS / "bus.jpg", conf=0.01)
-
-    # Training from yaml
-    model = YOLO("yolov8s-worldv2.yaml")  # no YOLOv8n-world model yet
-    model.train(data="coco8.yaml", epochs=2, imgsz=32, cache="disk", batch=-1, close_mosaic=1, name="yolo-world")
+    model(SOURCE, conf=0.01)
 
     model = YOLO("yolov8s-worldv2.pt")  # no YOLOv8n-world model yet
-    # val
-    model.val(data="coco8.yaml", imgsz=32, save_txt=True, save_json=True)
-    # Training from pretrain
-    model.train(data="coco8.yaml", epochs=2, imgsz=32, cache="disk", batch=-1, close_mosaic=1, name="yolo-world")
+    # Training from a pretrained model. Eval is included at the final stage of training.
+    # Use dota8.yaml which has fewer categories to reduce the inference time of CLIP model
+    model.train(
+        data="dota8.yaml",
+        epochs=1,
+        imgsz=32,
+        cache="disk",
+        close_mosaic=1,
+    )
 
     # test WorWorldTrainerFromScratch
     from ultralytics.models.yolo.world.train_world import WorldTrainerFromScratch
 
     model = YOLO("yolov8s-worldv2.yaml")  # no YOLOv8n-world model yet
     model.train(
-        data={"train": {"yolo_data": ["coco8.yaml"]}, "val": {"yolo_data": ["coco8.yaml"]}},
-        epochs=2,
+        data={"train": {"yolo_data": ["dota8.yaml"]}, "val": {"yolo_data": ["dota8.yaml"]}},
+        epochs=1,
         imgsz=32,
         cache="disk",
-        batch=-1,
         close_mosaic=1,
-        name="yolo-world",
         trainer=WorldTrainerFromScratch,
     )
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/__init__.py` & `vsensebox_ultralytics-8.2.15/ultralytics/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = "8.1.48"
+__version__ = "8.2.15"
 
 from ultralytics.data.explorer.explorer import Explorer
 from ultralytics.models import RTDETR, SAM, YOLO, YOLOWorld
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import ASSETS, SETTINGS
 from ultralytics.utils.checks import check_yolo as checks
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/assets/bus.jpg` & `vsensebox_ultralytics-8.2.15/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/assets/zidane.jpg` & `vsensebox_ultralytics-8.2.15/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/__init__.py` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,34 +49,35 @@
 TASK2METRIC = {
     "detect": "metrics/mAP50-95(B)",
     "segment": "metrics/mAP50-95(M)",
     "classify": "metrics/accuracy_top1",
     "pose": "metrics/mAP50-95(P)",
     "obb": "metrics/mAP50-95(B)",
 }
+MODELS = {TASK2MODEL[task] for task in TASKS}
 
 ARGV = sys.argv or ["", ""]  # sometimes sys.argv = []
 CLI_HELP_MSG = f"""
     Arguments received: {str(['yolo'] + ARGV[1:])}. Ultralytics 'yolo' commands use the following syntax:
 
         yolo TASK MODE ARGS
 
         Where   TASK (optional) is one of {TASKS}
                 MODE (required) is one of {MODES}
                 ARGS (optional) are any number of custom 'arg=value' pairs like 'imgsz=320' that override defaults.
                     See all ARGS at https://docs.ultralytics.com/usage/cfg or with 'yolo cfg'
 
     1. Train a detection model for 10 epochs with an initial learning_rate of 0.01
-        yolo train data=coco128.yaml model=yolov8n.pt epochs=10 lr0=0.01
+        yolo train data=coco8.yaml model=yolov8n.pt epochs=10 lr0=0.01
 
     2. Predict a YouTube video using a pretrained segmentation model at image size 320:
         yolo predict model=yolov8n-seg.pt source='https://youtu.be/LNwODJXcvt4' imgsz=320
 
     3. Val a pretrained detection model at batch-size 1 and image size 640:
-        yolo val model=yolov8n.pt data=coco128.yaml batch=1 imgsz=640
+        yolo val model=yolov8n.pt data=coco8.yaml batch=1 imgsz=640
 
     4. Export a YOLOv8n classification model to ONNX format at image size 224 by 128 (no TASK required)
         yolo export model=yolov8n-cls.pt format=onnx imgsz=224,128
 
     6. Explore your datasets using semantic search and SQL with a simple GUI powered by Ultralytics Explorer API
         yolo explorer
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/Argoverse.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/DOTAv1.5.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/DOTAv1.5.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/DOTAv1.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/DOTAv1.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/ImageNet.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/Objects365.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/SKU-110K.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/VOC.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/VisDrone.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/african-wildlife.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/african-wildlife.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/brain-tumor.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/brain-tumor.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/carparts-seg.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/carparts-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco-pose.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco128-seg.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco128.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco8-pose.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco8-seg.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/coco8.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/crack-seg.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/crack-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/dota8.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/dota8.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/lvis.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/lvis.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/open-images-v7.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/open-images-v7.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/package-seg.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/package-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/tiger-pose.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/tiger-pose.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/datasets/xView.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/default.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/default.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Default training settings and hyperparameters for medium-augmentation COCO training
 
 task: detect # (str) YOLO task, i.e. detect, segment, classify, pose
 mode: train # (str) YOLO mode, i.e. train, val, predict, export, track, benchmark
 
 # Train settings -------------------------------------------------------------------------------------------------------
 model: # (str, optional) path to model file, i.e. yolov8n.pt, yolov8n.yaml
-data: # (str, optional) path to data file, i.e. coco128.yaml
+data: # (str, optional) path to data file, i.e. coco8.yaml
 epochs: 100 # (int) number of epochs to train for
 time: # (float, optional) number of hours to train for, overrides epochs if supplied
 patience: 100 # (int) epochs to wait for no observable improvement for early stopping of training
 batch: 16 # (int) number of images per batch (-1 for AutoBatch)
 imgsz: 640 # (int | list) input images size as int for train and val modes, or list[w,h] for predict and export modes
 save: True # (bool) save train checkpoints and predict results
 save_period: -1 # (int) Save checkpoint every x epochs (disabled if < 1)
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v3/yolov3.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v5/yolov5.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v6/yolov6.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-ghost.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-obb.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-obb.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-world.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-world.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8-worldv2.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-worldv2.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v8/yolov8.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v9/yolov9c-seg.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9c-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v9/yolov9c.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9c.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v9/yolov9e-seg.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9e-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/models/v9/yolov9e.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9e.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/trackers/botsort.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/cfg/trackers/bytetrack.yaml` & `vsensebox_ultralytics-8.2.15/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/__init__.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/__init__.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/annotator.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/augment.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/augment.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 from typing import Tuple, Union
 
 import cv2
 import numpy as np
 import torch
 from PIL import Image
 
+from ultralytics.data.utils import polygons2masks, polygons2masks_overlap
 from ultralytics.utils import LOGGER, colorstr
 from ultralytics.utils.checks import check_version
 from ultralytics.utils.instance import Instances
 from ultralytics.utils.metrics import bbox_ioa
 from ultralytics.utils.ops import segment2box, xyxyxyxy2xywhr
 from ultralytics.utils.torch_utils import TORCHVISION_0_10, TORCHVISION_0_11, TORCHVISION_0_13
 
-from .utils import polygons2masks, polygons2masks_overlap
-
 DEFAULT_MEAN = (0.0, 0.0, 0.0)
 DEFAULT_STD = (1.0, 1.0, 1.0)
 DEFAULT_CROP_FRACTION = 1.0
 
 
 # TODO: we might need a BaseTransform to make all these augments be compatible with both classification and semantic
 class BaseTransform:
@@ -913,15 +912,14 @@
                     labels["img"] = new["image"]
                     labels["cls"] = np.array(new["class_labels"])
                     bboxes = np.array(new["bboxes"], dtype=np.float32)
             labels["instances"].update(bboxes=bboxes)
         return labels
 
 
-# TODO: technically this is not an augmentation, maybe we should put this to another files
 class Format:
     """
     Formats image annotations for object detection, instance segmentation, and pose estimation tasks. The class
     standardizes the image and instance annotations to be used by the `collate_fn` in PyTorch DataLoader.
 
     Attributes:
         bbox_format (str): Format for bounding boxes. Default is 'xywh'.
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/base.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 from typing import Optional
 
 import cv2
 import numpy as np
 import psutil
 from torch.utils.data import Dataset
 
+from ultralytics.data.utils import FORMATS_HELP_MSG, HELP_URL, IMG_FORMATS
 from ultralytics.utils import DEFAULT_CFG, LOCAL_RANK, LOGGER, NUM_THREADS, TQDM
 
-from .utils import FORMATS_HELP_MSG, HELP_URL, IMG_FORMATS
-
 
 class BaseDataset(Dataset):
     """
     Base dataset class for loading and processing image data.
 
     Args:
         img_path (str): Path to the folder containing images.
@@ -167,15 +166,15 @@
             elif not (h0 == w0 == self.imgsz):  # resize by stretching image to square imgsz
                 im = cv2.resize(im, (self.imgsz, self.imgsz), interpolation=cv2.INTER_LINEAR)
 
             # Add to buffer if training with augmentations
             if self.augment:
                 self.ims[i], self.im_hw0[i], self.im_hw[i] = im, (h0, w0), im.shape[:2]  # im, hw_original, hw_resized
                 self.buffer.append(i)
-                if len(self.buffer) >= self.max_buffer_length:
+                if 1 < len(self.buffer) >= self.max_buffer_length:  # prevent empty buffer
                     j = self.buffer.pop(0)
                     if self.cache != "ram":
                         self.ims[j], self.im_hw0[j], self.im_hw[j] = None, None, None
 
             return im, (h0, w0), im.shape[:2]
 
         return self.ims[i], self.im_hw0[i], self.im_hw[i]
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/build.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,31 +5,29 @@
 from pathlib import Path
 
 import numpy as np
 import torch
 from PIL import Image
 from torch.utils.data import dataloader, distributed
 
+from ultralytics.data.dataset import GroundingDataset, YOLODataset, YOLOMultiModalDataset
 from ultralytics.data.loaders import (
     LOADERS,
     LoadImagesAndVideos,
     LoadPilAndNumpy,
     LoadScreenshots,
     LoadStreams,
     LoadTensor,
     SourceTypes,
     autocast_list,
 )
-from ultralytics.data.utils import IMG_FORMATS, VID_FORMATS
-from ultralytics.utils import RANK, colorstr
+from ultralytics.data.utils import IMG_FORMATS, PIN_MEMORY, VID_FORMATS
+from ultralytics.utils import LINUX, RANK, colorstr
 from ultralytics.utils.checks import check_file
 
-from .dataset import GroundingDataset, YOLODataset, YOLOMultiModalDataset
-from .utils import PIN_MEMORY
-
 
 class InfiniteDataLoader(dataloader.DataLoader):
     """
     Dataloader that reuses workers.
 
     Uses same syntax as vanilla DataLoader.
     """
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/converter.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/dataset.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/explorer/explorer.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/explorer/gui/dash.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/gui/dash.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/explorer/utils.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/loaders.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/loaders.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/split_dota.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/split_dota.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/data/utils.py` & `vsensebox_ultralytics-8.2.15/ultralytics/data/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,14 +437,15 @@
             i.e. https://github.com/ultralytics/hub/raw/main/example_datasets/coco8.zip for coco8.zip.
         ```python
         from ultralytics.data.utils import HUBDatasetStats
 
         stats = HUBDatasetStats('path/to/coco8.zip', task='detect')  # detect dataset
         stats = HUBDatasetStats('path/to/coco8-seg.zip', task='segment')  # segment dataset
         stats = HUBDatasetStats('path/to/coco8-pose.zip', task='pose')  # pose dataset
+        stats = HUBDatasetStats('path/to/dota8.zip', task='obb')  # OBB dataset
         stats = HUBDatasetStats('path/to/imagenet10.zip', task='classify')  # classification dataset
 
         stats.get_json(save=True)
         stats.process_images()
         ```
     """
 
@@ -493,21 +494,21 @@
     def get_json(self, save=False, verbose=False):
         """Return dataset JSON for Ultralytics HUB."""
 
         def _round(labels):
             """Update labels to integer class and 4 decimal place floats."""
             if self.task == "detect":
                 coordinates = labels["bboxes"]
-            elif self.task == "segment":
+            elif self.task in {"segment", "obb"}:  # Segment and OBB use segments. OBB segments are normalized xyxyxyxy
                 coordinates = [x.flatten() for x in labels["segments"]]
             elif self.task == "pose":
-                n = labels["keypoints"].shape[0]
-                coordinates = np.concatenate((labels["bboxes"], labels["keypoints"].reshape(n, -1)), 1)
+                n, nk, nd = labels["keypoints"].shape
+                coordinates = np.concatenate((labels["bboxes"], labels["keypoints"].reshape(n, nk * nd)), 1)
             else:
-                raise ValueError("Undefined dataset task.")
+                raise ValueError(f"Undefined dataset task={self.task}.")
             zipped = zip(labels["cls"], coordinates)
             return [[int(c[0]), *(round(float(x), 4) for x in points)] for c, points in zipped]
 
         for split in "train", "val", "test":
             self.stats[split] = None  # predefine
             path = self.data.get(split)
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/engine/exporter.py` & `vsensebox_ultralytics-8.2.15/ultralytics/engine/exporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,50 +46,53 @@
 TensorFlow.js:
     $ cd .. && git clone https://github.com/zldrobit/tfjs-yolov5-example.git && cd tfjs-yolov5-example
     $ npm install
     $ ln -s ../../yolov5/yolov8n_web_model public/yolov8n_web_model
     $ npm start
 """
 
+import gc
 import json
 import os
 import shutil
 import subprocess
 import time
 import warnings
 from copy import deepcopy
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import torch
 
-from ultralytics.cfg import get_cfg
+from ultralytics.cfg import TASK2DATA, get_cfg
+from ultralytics.data import build_dataloader
 from ultralytics.data.dataset import YOLODataset
-from ultralytics.data.utils import check_det_dataset
+from ultralytics.data.utils import check_cls_dataset, check_det_dataset
 from ultralytics.nn.autobackend import check_class_names, default_class_names
 from ultralytics.nn.modules import C2f, Detect, RTDETRDecoder
 from ultralytics.nn.tasks import DetectionModel, SegmentationModel, WorldModel
 from ultralytics.utils import (
     ARM64,
     DEFAULT_CFG,
+    IS_JETSON,
     LINUX,
     LOGGER,
     MACOS,
     PYTHON_VERSION,
     ROOT,
     WINDOWS,
     __version__,
     callbacks,
     colorstr,
     get_default_args,
     yaml_save,
 )
 from ultralytics.utils.checks import check_imgsz, check_is_path_safe, check_requirements, check_version
-from ultralytics.utils.downloads import attempt_download_asset, get_github_assets
+from ultralytics.utils.downloads import attempt_download_asset, get_github_assets, safe_download
 from ultralytics.utils.files import file_size, spaces_in_path
 from ultralytics.utils.ops import Profile
 from ultralytics.utils.torch_utils import TORCH_1_13, get_latest_opset, select_device, smart_inference_mode
 
 
 def export_formats():
     """YOLOv8 export formats."""
@@ -163,15 +166,15 @@
         if self.args.format.lower() in {"coreml", "mlmodel"}:  # fix attempt for protobuf<3.20.x errors
             os.environ["PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION"] = "python"  # must run before TensorBoard callback
 
         self.callbacks = _callbacks or callbacks.get_default_callbacks()
         callbacks.add_integration_callbacks(self)
 
     @smart_inference_mode()
-    def __call__(self, model=None):
+    def __call__(self, model=None) -> str:
         """Returns list of exported files/dirs after running callbacks."""
         self.run_callbacks("on_export_start")
         t = time.time()
         fmt = self.args.format.lower()  # to lowercase
         if fmt in {"tensorrt", "trt"}:  # 'engine' aliases
             fmt = "engine"
         if fmt in {"mlmodel", "mlpackage", "mlprogram", "apple", "ios", "coreml"}:  # 'coreml' aliases
@@ -193,27 +196,34 @@
             model.names = default_class_names()
         model.names = check_class_names(model.names)
         if self.args.half and onnx and self.device.type == "cpu":
             LOGGER.warning("WARNING ⚠️ half=True only compatible with GPU export, i.e. use device=0")
             self.args.half = False
             assert not self.args.dynamic, "half=True not compatible with dynamic=True, i.e. use only one."
         self.imgsz = check_imgsz(self.args.imgsz, stride=model.stride, min_dim=2)  # check image size
+        if self.args.int8 and (engine or xml):
+            self.args.dynamic = True  # enforce dynamic to export TensorRT INT8; ensures ONNX is dynamic
         if self.args.optimize:
             assert not ncnn, "optimize=True not compatible with format='ncnn', i.e. use optimize=False"
             assert self.device.type == "cpu", "optimize=True not compatible with cuda devices, i.e. use device='cpu'"
         if edgetpu and not LINUX:
             raise SystemError("Edge TPU export only supported on Linux. See https://coral.ai/docs/edgetpu/compiler/")
         if isinstance(model, WorldModel):
             LOGGER.warning(
                 "WARNING ⚠️ YOLOWorld (original version) export is not supported to any format.\n"
                 "WARNING ⚠️ YOLOWorldv2 models (i.e. 'yolov8s-worldv2.pt') only support export to "
                 "(torchscript, onnx, openvino, engine, coreml) formats. "
                 "See https://docs.ultralytics.com/models/yolo-world for details."
             )
-
+        if self.args.int8 and not self.args.data:
+            self.args.data = DEFAULT_CFG.data or TASK2DATA[getattr(model, "task", "detect")]  # assign default data
+            LOGGER.warning(
+                "WARNING ⚠️ INT8 export requires a missing 'data' arg for calibration. "
+                f"Using default 'data={self.args.data}'."
+            )
         # Input
         im = torch.zeros(self.args.batch, 3, *self.imgsz).to(self.device)
         file = Path(
             getattr(model, "pt_path", None) or getattr(model, "yaml_file", None) or model.yaml.get("yaml_file", "")
         )
         if file.suffix in {".yaml", ".yml"}:
             file = Path(file.name)
@@ -327,14 +337,31 @@
                 f'\nValidate:        yolo val task={model.task} model={f} imgsz={imgsz} data={data} {q} {s}'
                 f'\nVisualize:       https://netron.app'
             )
 
         self.run_callbacks("on_export_end")
         return f  # return list of exported files/dirs
 
+    def get_int8_calibration_dataloader(self, prefix=""):
+        """Build and return a dataloader suitable for calibration of INT8 models."""
+        LOGGER.info(f"{prefix} collecting INT8 calibration images from 'data={self.args.data}'")
+        data = (check_cls_dataset if self.model.task == "classify" else check_det_dataset)(self.args.data)
+        dataset = YOLODataset(
+            data[self.args.split or "val"],
+            data=data,
+            task=self.model.task,
+            imgsz=self.imgsz[0],
+            augment=False,
+            batch_size=self.args.batch * 2,  # NOTE TensorRT INT8 calibration should use 2x batch size
+        )
+        n = len(dataset)
+        if n < 300:
+            LOGGER.warning(f"{prefix} WARNING ⚠️ >300 images recommended for INT8 calibration, found {n} images.")
+        return build_dataloader(dataset, batch=self.args.batch * 2, workers=0)  # required for batch loading
+
     @try_export
     def export_torchscript(self, prefix=colorstr("TorchScript:")):
         """YOLOv8 TorchScript model export."""
         LOGGER.info(f"\n{prefix} starting export with torch {torch.__version__}...")
         f = self.file.with_suffix(".torchscript")
 
         ts = torch.jit.trace(self.model, self.im, strict=False)
@@ -408,15 +435,15 @@
 
         onnx.save(model_onnx, f)
         return f, model_onnx
 
     @try_export
     def export_openvino(self, prefix=colorstr("OpenVINO:")):
         """YOLOv8 OpenVINO export."""
-        check_requirements("openvino>=2024.0.0")  # requires openvino: https://pypi.org/project/openvino/
+        check_requirements(f'openvino{"<=2024.0.0" if ARM64 else ">=2024.0.0"}')  # fix OpenVINO issue on ARM64
         import openvino as ov
 
         LOGGER.info(f"\n{prefix} starting export with openvino {ov.__version__}...")
         assert TORCH_1_13, f"OpenVINO export requires torch>=1.13.0 but torch=={torch.__version__} is installed"
         ov_model = ov.convert_model(
             self.model.cpu(),
             input=None if self.args.dynamic else [self.im.shape],
@@ -436,58 +463,45 @@
 
             ov.runtime.save_model(ov_model, file, compress_to_fp16=self.args.half)
             yaml_save(Path(file).parent / "metadata.yaml", self.metadata)  # add metadata.yaml
 
         if self.args.int8:
             fq = str(self.file).replace(self.file.suffix, f"_int8_openvino_model{os.sep}")
             fq_ov = str(Path(fq) / self.file.with_suffix(".xml").name)
-            if not self.args.data:
-                self.args.data = DEFAULT_CFG.data or "coco128.yaml"
-                LOGGER.warning(
-                    f"{prefix} WARNING ⚠️ INT8 export requires a missing 'data' arg for calibration. "
-                    f"Using default 'data={self.args.data}'."
-                )
             check_requirements("nncf>=2.8.0")
             import nncf
 
-            def transform_fn(data_item):
+            def transform_fn(data_item) -> np.ndarray:
                 """Quantization transform function."""
-                assert (
-                    data_item["img"].dtype == torch.uint8
-                ), "Input image must be uint8 for the quantization preprocessing"
-                im = data_item["img"].numpy().astype(np.float32) / 255.0  # uint8 to fp16/32 and 0 - 255 to 0.0 - 1.0
+                data_item: torch.Tensor = data_item["img"] if isinstance(data_item, dict) else data_item
+                assert data_item.dtype == torch.uint8, "Input image must be uint8 for the quantization preprocessing"
+                im = data_item.numpy().astype(np.float32) / 255.0  # uint8 to fp16/32 and 0 - 255 to 0.0 - 1.0
                 return np.expand_dims(im, 0) if im.ndim == 3 else im
 
             # Generate calibration data for integer quantization
-            LOGGER.info(f"{prefix} collecting INT8 calibration images from 'data={self.args.data}'")
-            data = check_det_dataset(self.args.data)
-            dataset = YOLODataset(data["val"], data=data, task=self.model.task, imgsz=self.imgsz[0], augment=False)
-            n = len(dataset)
-            if n < 300:
-                LOGGER.warning(f"{prefix} WARNING ⚠️ >300 images recommended for INT8 calibration, found {n} images.")
-            quantization_dataset = nncf.Dataset(dataset, transform_fn)
-
             ignored_scope = None
             if isinstance(self.model.model[-1], Detect):
                 # Includes all Detect subclasses like Segment, Pose, OBB, WorldDetect
                 head_module_name = ".".join(list(self.model.named_modules())[-1][0].split(".")[:2])
-
                 ignored_scope = nncf.IgnoredScope(  # ignore operations
                     patterns=[
                         f".*{head_module_name}/.*/Add",
                         f".*{head_module_name}/.*/Sub*",
                         f".*{head_module_name}/.*/Mul*",
                         f".*{head_module_name}/.*/Div*",
                         f".*{head_module_name}\\.dfl.*",
                     ],
                     types=["Sigmoid"],
                 )
 
             quantized_ov_model = nncf.quantize(
-                ov_model, quantization_dataset, preset=nncf.QuantizationPreset.MIXED, ignored_scope=ignored_scope
+                model=ov_model,
+                calibration_dataset=nncf.Dataset(self.get_int8_calibration_dataloader(prefix), transform_fn),
+                preset=nncf.QuantizationPreset.MIXED,
+                ignored_scope=ignored_scope,
             )
             serialize(quantized_ov_model, fq_ov)
             return fq, None
 
         f = str(self.file).replace(self.file.suffix, f"_openvino_model{os.sep}")
         f_ov = str(Path(f) / self.file.with_suffix(".xml").name)
 
@@ -517,36 +531,36 @@
         import ncnn  # noqa
 
         LOGGER.info(f"\n{prefix} starting export with NCNN {ncnn.__version__}...")
         f = Path(str(self.file).replace(self.file.suffix, f"_ncnn_model{os.sep}"))
         f_ts = self.file.with_suffix(".torchscript")
 
         name = Path("pnnx.exe" if WINDOWS else "pnnx")  # PNNX filename
-        pnnx = name if name.is_file() else ROOT / name
+        pnnx = name if name.is_file() else (ROOT / name)
         if not pnnx.is_file():
             LOGGER.warning(
                 f"{prefix} WARNING ⚠️ PNNX not found. Attempting to download binary file from "
                 "https://github.com/pnnx/pnnx/.\nNote PNNX Binary file must be placed in current working directory "
                 f"or in {ROOT}. See PNNX repo for full installation instructions."
             )
             system = "macos" if MACOS else "windows" if WINDOWS else "linux-aarch64" if ARM64 else "linux"
             try:
-                _, assets = get_github_assets(repo="pnnx/pnnx")
-                url = [x for x in assets if f"{system}.zip" in x][0]
-                assert url, "Unable to retrieve PNNX repo assets"
+                release, assets = get_github_assets(repo="pnnx/pnnx")
+                asset = [x for x in assets if f"{system}.zip" in x][0]
+                assert isinstance(asset, str), "Unable to retrieve PNNX repo assets"  # i.e. pnnx-20240410-macos.zip
+                LOGGER.info(f"{prefix} successfully found latest PNNX asset file {asset}")
             except Exception as e:
-                url = f"https://github.com/pnnx/pnnx/releases/download/20240410/pnnx-20240410-{system}.zip"
-                LOGGER.warning(f"{prefix} WARNING ⚠️ PNNX GitHub assets not found: {e}, using default {url}")
-            asset = attempt_download_asset(url, repo="pnnx/pnnx", release="latest")
-            if check_is_path_safe(Path.cwd(), asset):  # avoid path traversal security vulnerability
-                unzip_dir = Path(asset).with_suffix("")
+                release = "20240410"
+                asset = f"pnnx-{release}-{system}.zip"
+                LOGGER.warning(f"{prefix} WARNING ⚠️ PNNX GitHub assets not found: {e}, using default {asset}")
+            unzip_dir = safe_download(f"https://github.com/pnnx/pnnx/releases/download/{release}/{asset}", delete=True)
+            if check_is_path_safe(Path.cwd(), unzip_dir):  # avoid path traversal security vulnerability
                 (unzip_dir / name).rename(pnnx)  # move binary to ROOT
-                shutil.rmtree(unzip_dir)  # delete unzip dir
-                Path(asset).unlink()  # delete zip
                 pnnx.chmod(0o777)  # set read, write, and execute permissions for everyone
+                shutil.rmtree(unzip_dir)  # delete unzip dir
 
         ncnn_args = [
             f'ncnnparam={f / "model.ncnn.param"}',
             f'ncnnbin={f / "model.ncnn.bin"}',
             f'ncnnpy={f / "model_ncnn.py"}',
         ]
 
@@ -583,14 +597,15 @@
         """YOLOv8 CoreML export."""
         mlmodel = self.args.format.lower() == "mlmodel"  # legacy *.mlmodel export format requested
         check_requirements("coremltools>=6.0,<=6.2" if mlmodel else "coremltools>=7.0")
         import coremltools as ct  # noqa
 
         LOGGER.info(f"\n{prefix} starting export with coremltools {ct.__version__}...")
         assert not WINDOWS, "CoreML export is not supported on Windows, please run on macOS or Linux."
+        assert self.args.batch == 1, "CoreML batch sizes > 1 are not supported. Please retry at 'batch=1'."
         f = self.file.with_suffix(".mlmodel" if mlmodel else ".mlpackage")
         if f.is_dir():
             shutil.rmtree(f)
 
         bias = [0.0, 0.0, 0.0]
         scale = 1 / 255
         classifier_config = None
@@ -662,61 +677,120 @@
             import tensorrt as trt  # noqa
         except ImportError:
             if LINUX:
                 check_requirements("nvidia-tensorrt", cmds="-U --index-url https://pypi.ngc.nvidia.com")
             import tensorrt as trt  # noqa
         check_version(trt.__version__, "7.0.0", hard=True)  # require tensorrt>=7.0.0
 
+        # Setup and checks
         LOGGER.info(f"\n{prefix} starting export with TensorRT {trt.__version__}...")
         is_trt10 = int(trt.__version__.split(".")[0]) >= 10  # is TensorRT >= 10
         assert Path(f_onnx).exists(), f"failed to export ONNX file: {f_onnx}"
         f = self.file.with_suffix(".engine")  # TensorRT engine file
         logger = trt.Logger(trt.Logger.INFO)
         if self.args.verbose:
             logger.min_severity = trt.Logger.Severity.VERBOSE
 
+        # Engine builder
         builder = trt.Builder(logger)
         config = builder.create_builder_config()
         workspace = int(self.args.workspace * (1 << 30))
         if is_trt10:
             config.set_memory_pool_limit(trt.MemoryPoolType.WORKSPACE, workspace)
         else:  # TensorRT versions 7, 8
             config.max_workspace_size = workspace
         flag = 1 << int(trt.NetworkDefinitionCreationFlag.EXPLICIT_BATCH)
         network = builder.create_network(flag)
+        half = builder.platform_has_fast_fp16 and self.args.half
+        int8 = builder.platform_has_fast_int8 and self.args.int8
+        # Read ONNX file
         parser = trt.OnnxParser(network, logger)
         if not parser.parse_from_file(f_onnx):
             raise RuntimeError(f"failed to load ONNX file: {f_onnx}")
 
+        # Network inputs
         inputs = [network.get_input(i) for i in range(network.num_inputs)]
         outputs = [network.get_output(i) for i in range(network.num_outputs)]
         for inp in inputs:
             LOGGER.info(f'{prefix} input "{inp.name}" with shape{inp.shape} {inp.dtype}')
         for out in outputs:
             LOGGER.info(f'{prefix} output "{out.name}" with shape{out.shape} {out.dtype}')
 
         if self.args.dynamic:
             shape = self.im.shape
             if shape[0] <= 1:
                 LOGGER.warning(f"{prefix} WARNING ⚠️ 'dynamic=True' model requires max batch size, i.e. 'batch=16'")
             profile = builder.create_optimization_profile()
             min_shape = (1, shape[1], 32, 32)  # minimum input shape
-            opt_shape = (max(1, shape[0] // 2), *shape[1:])  # optimal input shape
             max_shape = (*shape[:2], *(max(1, self.args.workspace) * d for d in shape[2:]))  # max input shape
             for inp in inputs:
-                profile.set_shape(inp.name, min_shape, opt_shape, max_shape)
+                profile.set_shape(inp.name, min=min_shape, opt=shape, max=max_shape)
             config.add_optimization_profile(profile)
 
-        half = builder.platform_has_fast_fp16 and self.args.half
-        LOGGER.info(f"{prefix} building FP{16 if half else 32} engine as {f}")
-        if half:
+        LOGGER.info(f"{prefix} building {'INT8' if int8 else 'FP' + ('16' if half else '32')} engine as {f}")
+        if int8:
+            config.set_flag(trt.BuilderFlag.INT8)
+            config.set_calibration_profile(profile)
+            config.profiling_verbosity = trt.ProfilingVerbosity.DETAILED
+
+            class EngineCalibrator(trt.IInt8Calibrator):
+                def __init__(
+                    self,
+                    dataset,  # ultralytics.data.build.InfiniteDataLoader
+                    batch: int,
+                    cache: str = "",
+                ) -> None:
+                    trt.IInt8Calibrator.__init__(self)
+                    self.dataset = dataset
+                    self.data_iter = iter(dataset)
+                    self.algo = trt.CalibrationAlgoType.ENTROPY_CALIBRATION_2
+                    self.batch = batch
+                    self.cache = Path(cache)
+
+                def get_algorithm(self) -> trt.CalibrationAlgoType:
+                    """Get the calibration algorithm to use."""
+                    return self.algo
+
+                def get_batch_size(self) -> int:
+                    """Get the batch size to use for calibration."""
+                    return self.batch or 1
+
+                def get_batch(self, names) -> list:
+                    """Get the next batch to use for calibration, as a list of device memory pointers."""
+                    try:
+                        im0s = next(self.data_iter)["img"] / 255.0
+                        im0s = im0s.to("cuda") if im0s.device.type == "cpu" else im0s
+                        return [int(im0s.data_ptr())]
+                    except StopIteration:
+                        # Return [] or None, signal to TensorRT there is no calibration data remaining
+                        return None
+
+                def read_calibration_cache(self) -> bytes:
+                    """Use existing cache instead of calibrating again, otherwise, implicitly return None."""
+                    if self.cache.exists() and self.cache.suffix == ".cache":
+                        return self.cache.read_bytes()
+
+                def write_calibration_cache(self, cache) -> None:
+                    """Write calibration cache to disk."""
+                    _ = self.cache.write_bytes(cache)
+
+            # Load dataset w/ builder (for batching) and calibrate
+            dataset = self.get_int8_calibration_dataloader(prefix)
+            config.int8_calibrator = EngineCalibrator(
+                dataset=dataset,
+                batch=2 * self.args.batch,
+                cache=self.file.with_suffix(".cache"),
+            )
+
+        elif half:
             config.set_flag(trt.BuilderFlag.FP16)
 
         # Free CUDA memory
         del self.model
+        gc.collect()
         torch.cuda.empty_cache()
 
         # Write file
         build = builder.build_serialized_network if is_trt10 else builder.build_engine
         with build(network, config) as engine, open(f, "wb") as t:
             # Metadata
             meta = json.dumps(self.metadata)
@@ -743,15 +817,15 @@
         check_requirements(
             (
                 "onnx>=1.12.0",
                 "onnx2tf>=1.15.4,<=1.17.5",
                 "sng4onnx>=1.0.1",
                 "onnxsim>=0.4.33",
                 "onnx_graphsurgeon>=0.3.26",
-                "tflite_support",
+                "tflite_support<=0.4.3" if IS_JETSON else "tflite_support",  # fix ImportError 'GLIBCXX_3.4.29'
                 "flatbuffers>=23.5.26,<100",  # update old 'flatbuffers' included inside tensorflow package
                 "onnxruntime-gpu" if cuda else "onnxruntime",
             ),
             cmds="--extra-index-url https://pypi.ngc.nvidia.com",
         )  # onnx_graphsurgeon only on NVIDIA
 
         LOGGER.info(f"\n{prefix} starting export with tensorflow {tf.__version__}...")
@@ -780,19 +854,17 @@
         # Export to TF
         tmp_file = f / "tmp_tflite_int8_calibration_images.npy"  # int8 calibration images file
         np_data = None
         if self.args.int8:
             verbosity = "info"
             if self.args.data:
                 # Generate calibration data for integer quantization
-                LOGGER.info(f"{prefix} collecting INT8 calibration images from 'data={self.args.data}'")
-                data = check_det_dataset(self.args.data)
-                dataset = YOLODataset(data["val"], data=data, imgsz=self.imgsz[0], augment=False)
+                dataloader = self.get_int8_calibration_dataloader(prefix)
                 images = []
-                for i, batch in enumerate(dataset):
+                for i, batch in enumerate(dataloader):
                     if i >= 100:  # maximum number of calibration images
                         break
                     im = batch["img"].permute(1, 2, 0)[None]  # list to nparray, CHW to BHWC
                     images.append(im)
                 f.mkdir()
                 images = torch.cat(images, 0).float()
                 # mean = images.view(-1, 3).mean(0)  # imagenet mean [123.675, 116.28, 103.53]
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/engine/model.py` & `vsensebox_ultralytics-8.2.15/ultralytics/engine/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import inspect
 from pathlib import Path
-from typing import Union
+from typing import List, Union
 
 import numpy as np
 import torch
 
 from ultralytics.cfg import TASK2DATA, get_cfg, get_save_dir
+from ultralytics.engine.results import Results
 from ultralytics.hub.utils import HUB_WEB_ROOT
 from ultralytics.nn.tasks import attempt_load_one_weight, guess_model_task, nn, yaml_model_load
 from ultralytics.utils import (
     ARGV,
     ASSETS,
     DEFAULT_CFG_DICT,
     LOGGER,
@@ -395,15 +396,15 @@
 
     def predict(
         self,
         source: Union[str, Path, int, list, tuple, np.ndarray, torch.Tensor] = None,
         stream: bool = False,
         predictor=None,
         **kwargs,
-    ) -> list:
+    ) -> List[Results]:
         """
         Performs predictions on the given image source using the YOLO model.
 
         This method facilitates the prediction process, allowing various configurations through keyword arguments.
         It supports predictions with custom predictors or the default predictor method. The method handles different
         types of image sources and can operate in a streaming mode. It also provides support for SAM-type models
         through 'prompts'.
@@ -453,15 +454,15 @@
 
     def track(
         self,
         source: Union[str, Path, int, list, tuple, np.ndarray, torch.Tensor] = None,
         stream: bool = False,
         persist: bool = False,
         **kwargs,
-    ) -> list:
+    ) -> List[Results]:
         """
         Conducts object tracking on the specified input source using the registered trackers.
 
         This method performs object tracking using the model's predictors and optionally registered trackers. It is
         capable of handling different types of input sources such as file paths or video streams. The method supports
         customization of the tracking process through various keyword arguments. It registers trackers if they are not
         already present and optionally persists them based on the 'persist' flag.
@@ -568,15 +569,15 @@
             device=args["device"],
             verbose=kwargs.get("verbose"),
         )
 
     def export(
         self,
         **kwargs,
-    ):
+    ) -> str:
         """
         Exports the model to a different format suitable for deployment.
 
         This method facilitates the export of the model to various formats (e.g., ONNX, TorchScript) for deployment
         purposes. It uses the 'Exporter' class for the export process, combining model-specific overrides, method
         defaults, and any additional arguments provided. The combined arguments are used to configure export settings.
 
@@ -584,15 +585,15 @@
         possible arguments, refer to the 'configuration' section in the documentation.
 
         Args:
             **kwargs (any): Arbitrary keyword arguments to customize the export process. These are combined with the
                 model's overrides and method defaults.
 
         Returns:
-            (object): The exported model in the specified format, or an object related to the export process.
+            (str): The exported model filename in the specified format, or an object related to the export process.
 
         Raises:
             AssertionError: If the model is not a PyTorch model.
         """
         self._check_is_pytorch_model()
         from .exporter import Exporter
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/engine/predictor.py` & `vsensebox_ultralytics-8.2.15/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/engine/results.py` & `vsensebox_ultralytics-8.2.15/ultralytics/engine/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,34 +383,40 @@
                 self.orig_img.copy(),
                 file=Path(save_dir) / self.names[int(d.cls)] / f"{Path(file_name)}.jpg",
                 BGR=True,
             )
 
     def summary(self, normalize=False, decimals=5):
         """Convert the results to a summarized format."""
-        if self.probs is not None:
-            LOGGER.warning("Warning: Classify results do not support the `summary()` method yet.")
-            return
-
         # Create list of detection dictionaries
         results = []
-        data = self.boxes.data.cpu().tolist()
+        if self.probs is not None:
+            class_id = self.probs.top1
+            results.append(
+                {
+                    "name": self.names[class_id],
+                    "class": class_id,
+                    "confidence": round(self.probs.top1conf.item(), decimals),
+                }
+            )
+            return results
+
+        data = self.boxes or self.obb
+        is_obb = self.obb is not None
         h, w = self.orig_shape if normalize else (1, 1)
         for i, row in enumerate(data):  # xyxy, track_id if tracking, conf, class_id
-            box = {
-                "x1": round(row[0] / w, decimals),
-                "y1": round(row[1] / h, decimals),
-                "x2": round(row[2] / w, decimals),
-                "y2": round(row[3] / h, decimals),
-            }
-            conf = round(row[-2], decimals)
-            class_id = int(row[-1])
-            result = {"name": self.names[class_id], "class": class_id, "confidence": conf, "box": box}
-            if self.boxes.is_track:
-                result["track_id"] = int(row[-3])  # track ID
+            class_id, conf = int(row.cls), round(row.conf.item(), decimals)
+            box = (row.xyxyxyxy if is_obb else row.xyxy).squeeze().reshape(-1, 2).tolist()
+            xy = {}
+            for j, b in enumerate(box):
+                xy[f"x{j + 1}"] = round(b[0] / w, decimals)
+                xy[f"y{j + 1}"] = round(b[1] / h, decimals)
+            result = {"name": self.names[class_id], "class": class_id, "confidence": conf, "box": xy}
+            if data.is_track:
+                result["track_id"] = int(row.id.item())  # track ID
             if self.masks:
                 result["segments"] = {
                     "x": (self.masks.xy[i][:, 0] / w).round(decimals).tolist(),
                     "y": (self.masks.xy[i][:, 1] / h).round(decimals).tolist(),
                 }
             if self.keypoints is not None:
                 x, y, visible = self.keypoints[i].data[0].cpu().unbind(dim=1)  # torch Tensor
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/engine/trainer.py` & `vsensebox_ultralytics-8.2.15/ultralytics/engine/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 """
 Train a model on a dataset.
 
 Usage:
-    $ yolo mode=train model=yolov8n.pt data=coco128.yaml imgsz=640 epochs=100 batch=16
+    $ yolo mode=train model=yolov8n.pt data=coco8.yaml imgsz=640 epochs=100 batch=16
 """
 
+import gc
 import math
 import os
 import subprocess
 import time
 import warnings
 from copy import deepcopy
 from datetime import datetime, timedelta
@@ -324,14 +325,15 @@
             f"Logging results to {colorstr('bold', self.save_dir)}\n"
             f'Starting training for ' + (f"{self.args.time} hours..." if self.args.time else f"{self.epochs} epochs...")
         )
         if self.args.close_mosaic:
             base_idx = (self.epochs - self.args.close_mosaic) * nb
             self.plot_idx.extend([base_idx, base_idx + 1, base_idx + 2])
         epoch = self.start_epoch
+        self.optimizer.zero_grad()  # zero any resumed gradients to ensure stability on train start
         while True:
             self.epoch = epoch
             self.run_callbacks("on_train_epoch_start")
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")  # suppress 'Detected lr_scheduler.step() before optimizer.step()'
                 self.scheduler.step()
 
@@ -344,15 +346,14 @@
                 self._close_dataloader_mosaic()
                 self.train_loader.reset()
 
             if RANK in {-1, 0}:
                 LOGGER.info(self.progress_string())
                 pbar = TQDM(enumerate(self.train_loader), total=nb)
             self.tloss = None
-            self.optimizer.zero_grad()
             for i, batch in pbar:
                 self.run_callbacks("on_train_batch_start")
                 # Warmup
                 ni = i + nb * epoch
                 if ni <= nw:
                     xi = [0, nw]  # x interp
                     self.accumulate = max(1, int(np.interp(ni, xi, [1, self.args.nbs / self.batch_size]).round()))
@@ -433,14 +434,15 @@
             if self.args.time:
                 mean_epoch_time = (t - self.train_time_start) / (epoch - self.start_epoch + 1)
                 self.epochs = self.args.epochs = math.ceil(self.args.time * 3600 / mean_epoch_time)
                 self._setup_scheduler()
                 self.scheduler.last_epoch = self.epoch  # do not move
                 self.stop |= epoch >= self.epochs  # stop if exceeded epochs
             self.run_callbacks("on_fit_epoch_end")
+            gc.collect()
             torch.cuda.empty_cache()  # clear GPU memory at end of epoch, may help reduce CUDA out of memory errors
 
             # Early Stopping
             if RANK != -1:  # if DDP training
                 broadcast_list = [self.stop if RANK == 0 else None]
                 dist.broadcast_object_list(broadcast_list, 0)  # broadcast 'stop' to all ranks
                 self.stop = broadcast_list[0]
@@ -454,14 +456,15 @@
                 f"\n{epoch - self.start_epoch + 1} epochs completed in "
                 f"{(time.time() - self.train_time_start) / 3600:.3f} hours."
             )
             self.final_eval()
             if self.args.plots:
                 self.plot_metrics()
             self.run_callbacks("on_train_end")
+        gc.collect()
         torch.cuda.empty_cache()
         self.run_callbacks("teardown")
 
     def save_model(self):
         """Save model training checkpoints with additional metadata."""
         import io
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/engine/tuner.py` & `vsensebox_ultralytics-8.2.15/ultralytics/engine/tuner.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/engine/validator.py` & `vsensebox_ultralytics-8.2.15/ultralytics/engine/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 """
 Check a model's accuracy on a test or val split of a dataset.
 
 Usage:
-    $ yolo mode=val model=yolov8n.pt data=coco128.yaml imgsz=640
+    $ yolo mode=val model=yolov8n.pt data=coco8.yaml imgsz=640
 
 Usage - formats:
     $ yolo mode=val model=yolov8n.pt                 # PyTorch
                           yolov8n.torchscript        # TorchScript
                           yolov8n.onnx               # ONNX Runtime or OpenCV DNN with dnn=True
                           yolov8n_openvino_model     # OpenVINO
                           yolov8n.engine             # TensorRT
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/hub/__init__.py` & `vsensebox_ultralytics-8.2.15/ultralytics/hub/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -102,27 +102,31 @@
         json={"apiKey": Auth().api_key, "modelId": model_id, "format": format},
         headers={"x-api-key": Auth().api_key},
     )
     assert r.status_code == 200, f"{PREFIX}{format} get_export failure {r.status_code} {r.reason}"
     return r.json()
 
 
-def check_dataset(path="", task="detect"):
+def check_dataset(path: str, task: str) -> None:
     """
     Function for error-checking HUB dataset Zip file before upload. It checks a dataset for errors before it is uploaded
     to the HUB. Usage examples are given below.
 
     Args:
-        path (str, optional): Path to data.zip (with data.yaml inside data.zip). Defaults to ''.
-        task (str, optional): Dataset task. Options are 'detect', 'segment', 'pose', 'classify'. Defaults to 'detect'.
+        path (str): Path to data.zip (with data.yaml inside data.zip).
+        task (str): Dataset task. Options are 'detect', 'segment', 'pose', 'classify', 'obb'.
 
     Example:
+        Download *.zip files from https://github.com/ultralytics/hub/tree/main/example_datasets
+            i.e. https://github.com/ultralytics/hub/raw/main/example_datasets/coco8.zip for coco8.zip.
         ```python
         from ultralytics.hub import check_dataset
 
         check_dataset('path/to/coco8.zip', task='detect')  # detect dataset
         check_dataset('path/to/coco8-seg.zip', task='segment')  # segment dataset
         check_dataset('path/to/coco8-pose.zip', task='pose')  # pose dataset
+        check_dataset('path/to/dota8.zip', task='obb')  # OBB dataset
+        check_dataset('path/to/imagenet10.zip', task='classify')  # classification dataset
         ```
     """
     HUBDatasetStats(path=path, task=task).get_json()
     LOGGER.info(f"Checks completed correctly ✅. Upload this dataset to {HUB_WEB_ROOT}/datasets/.")
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/hub/auth.py` & `vsensebox_ultralytics-8.2.15/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/hub/session.py` & `vsensebox_ultralytics-8.2.15/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/hub/utils.py` & `vsensebox_ultralytics-8.2.15/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/model.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/model.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/predict.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/prompt.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/utils.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/fastsam/val.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/nas/model.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/nas/model.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/nas/predict.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/nas/val.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/rtdetr/model.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/rtdetr/predict.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/rtdetr/train.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/rtdetr/val.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/sam/amg.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/sam/build.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/sam/model.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/model.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/decoders.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/encoders.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/sam.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/tiny_encoder.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/sam/modules/transformer.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/sam/predict.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/utils/loss.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/utils/ops.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/classify/predict.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/classify/train.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/classify/val.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/val.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         batch["img"] = batch["img"].half() if self.args.half else batch["img"].float()
         batch["cls"] = batch["cls"].to(self.device)
         return batch
 
     def update_metrics(self, preds, batch):
         """Updates running metrics with model predictions and batch targets."""
         n5 = min(len(self.names), 5)
-        self.pred.append(preds.argsort(1, descending=True)[:, :n5])
-        self.targets.append(batch["cls"])
+        self.pred.append(preds.argsort(1, descending=True)[:, :n5].type(torch.int32).cpu())
+        self.targets.append(batch["cls"].type(torch.int32).cpu())
 
     def finalize_metrics(self, *args, **kwargs):
         """Finalizes metrics of the model such as confusion_matrix and speed."""
         self.confusion_matrix.process_cls_preds(self.pred, self.targets)
         if self.args.plots:
             for normalize in True, False:
                 self.confusion_matrix.plot(
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/detect/predict.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/detect/train.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/detect/val.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/model.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class YOLO(Model):
     """YOLO (You Only Look Once) object detection model."""
 
     def __init__(self, model="yolov8n.pt", task=None, verbose=False):
         """Initialize YOLO model, switching to YOLOWorld if model filename contains '-world'."""
         path = Path(model)
         if "-world" in path.stem and path.suffix in {".pt", ".yaml", ".yml"}:  # if YOLOWorld PyTorch model
-            new_instance = YOLOWorld(path)
+            new_instance = YOLOWorld(path, verbose=verbose)
             self.__class__ = type(new_instance)
             self.__dict__ = new_instance.__dict__
         else:
             # Continue with default YOLO initialization
             super().__init__(model=model, task=task, verbose=verbose)
 
     @property
@@ -58,22 +58,22 @@
             },
         }
 
 
 class YOLOWorld(Model):
     """YOLO-World object detection model."""
 
-    def __init__(self, model="yolov8s-world.pt") -> None:
+    def __init__(self, model="yolov8s-world.pt", verbose=False) -> None:
         """
         Initializes the YOLOv8-World model with the given pre-trained model file. Supports *.pt and *.yaml formats.
 
         Args:
             model (str | Path): Path to the pre-trained model. Defaults to 'yolov8s-world.pt'.
         """
-        super().__init__(model=model, task="detect")
+        super().__init__(model=model, task="detect", verbose=verbose)
 
         # Assign default COCO class names when there are no custom names
         if not hasattr(self.model, "names"):
             self.model.names = yaml_load(ROOT / "cfg/datasets/coco8.yaml").get("names")
 
     @property
     def task_map(self):
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/obb/predict.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/obb/train.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/obb/val.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/pose/predict.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/pose/train.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/pose/val.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/segment/predict.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/segment/train.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/segment/val.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/world/train.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/models/yolo/world/train_world.py` & `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/train_world.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/nn/__init__.py` & `vsensebox_ultralytics-8.2.15/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/nn/autobackend.py` & `vsensebox_ultralytics-8.2.15/ultralytics/nn/autobackend.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import cv2
 import numpy as np
 import torch
 import torch.nn as nn
 from PIL import Image
 
-from ultralytics.utils import ARM64, LINUX, LOGGER, ROOT, yaml_load
+from ultralytics.utils import ARM64, IS_JETSON, IS_RASPBERRYPI, LINUX, LOGGER, ROOT, yaml_load
 from ultralytics.utils.checks import check_requirements, check_suffix, check_version, check_yaml
 from ultralytics.utils.downloads import attempt_download_asset, is_url
 
 
 def check_class_names(names):
     """
     Check class names.
@@ -179,14 +179,17 @@
             # check_requirements("opencv-python>=4.5.4")
             net = cv2.dnn.readNetFromONNX(w)
 
         # ONNX Runtime
         elif onnx:
             LOGGER.info(f"Loading {w} for ONNX Runtime inference...")
             check_requirements(("onnx", "onnxruntime-gpu" if cuda else "onnxruntime"))
+            if IS_RASPBERRYPI or IS_JETSON:
+                # Fix error: module 'numpy.linalg._umath_linalg' has no attribute '_ilp64' when exporting to Tensorflow SavedModel on RPi and Jetson
+                check_requirements("numpy==1.23.5")
             import onnxruntime
 
             providers = ["CUDAExecutionProvider", "CPUExecutionProvider"] if cuda else ["CPUExecutionProvider"]
             session = onnxruntime.InferenceSession(w, providers=providers)
             output_names = [x.name for x in session.get_outputs()]
             metadata = session.get_modelmeta().custom_metadata_map
 
@@ -227,16 +230,19 @@
             check_version(trt.__version__, "7.0.0", hard=True)  # require tensorrt>=7.0.0
             if device.type == "cpu":
                 device = torch.device("cuda:0")
             Binding = namedtuple("Binding", ("name", "dtype", "shape", "data", "ptr"))
             logger = trt.Logger(trt.Logger.INFO)
             # Read file
             with open(w, "rb") as f, trt.Runtime(logger) as runtime:
-                meta_len = int.from_bytes(f.read(4), byteorder="little")  # read metadata length
-                metadata = json.loads(f.read(meta_len).decode("utf-8"))  # read metadata
+                try:
+                    meta_len = int.from_bytes(f.read(4), byteorder="little")  # read metadata length
+                    metadata = json.loads(f.read(meta_len).decode("utf-8"))  # read metadata
+                except UnicodeDecodeError:
+                    f.seek(0)  # engine file may lack embedded Ultralytics metadata
                 model = runtime.deserialize_cuda_engine(f.read())  # read engine
 
             # Model context
             try:
                 context = model.create_execution_context()
             except Exception as e:  # model is None
                 LOGGER.error(f"ERROR: TensorRT model exported with a different version than {trt.__version__}\n")
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/__init__.py` & `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/block.py` & `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/conv.py` & `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/head.py` & `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/head.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,53 +94,51 @@
 
     def __init__(self, nc=80, nm=32, npr=256, ch=()):
         """Initialize the YOLO model attributes such as the number of masks, prototypes, and the convolution layers."""
         super().__init__(nc, ch)
         self.nm = nm  # number of masks
         self.npr = npr  # number of protos
         self.proto = Proto(ch[0], self.npr, self.nm)  # protos
-        self.detect = Detect.forward
 
         c4 = max(ch[0] // 4, self.nm)
         self.cv4 = nn.ModuleList(nn.Sequential(Conv(x, c4, 3), Conv(c4, c4, 3), nn.Conv2d(c4, self.nm, 1)) for x in ch)
 
     def forward(self, x):
         """Return model outputs and mask coefficients if training, otherwise return outputs and mask coefficients."""
         p = self.proto(x[0])  # mask protos
         bs = p.shape[0]  # batch size
 
         mc = torch.cat([self.cv4[i](x[i]).view(bs, self.nm, -1) for i in range(self.nl)], 2)  # mask coefficients
-        x = self.detect(self, x)
+        x = Detect.forward(self, x)
         if self.training:
             return x, mc, p
         return (torch.cat([x, mc], 1), p) if self.export else (torch.cat([x[0], mc], 1), (x[1], mc, p))
 
 
 class OBB(Detect):
     """YOLOv8 OBB detection head for detection with rotation models."""
 
     def __init__(self, nc=80, ne=1, ch=()):
         """Initialize OBB with number of classes `nc` and layer channels `ch`."""
         super().__init__(nc, ch)
         self.ne = ne  # number of extra parameters
-        self.detect = Detect.forward
 
         c4 = max(ch[0] // 4, self.ne)
         self.cv4 = nn.ModuleList(nn.Sequential(Conv(x, c4, 3), Conv(c4, c4, 3), nn.Conv2d(c4, self.ne, 1)) for x in ch)
 
     def forward(self, x):
         """Concatenates and returns predicted bounding boxes and class probabilities."""
         bs = x[0].shape[0]  # batch size
         angle = torch.cat([self.cv4[i](x[i]).view(bs, self.ne, -1) for i in range(self.nl)], 2)  # OBB theta logits
         # NOTE: set `angle` as an attribute so that `decode_bboxes` could use it.
         angle = (angle.sigmoid() - 0.25) * math.pi  # [-pi/4, 3pi/4]
         # angle = angle.sigmoid() * math.pi / 2  # [0, pi/2]
         if not self.training:
             self.angle = angle
-        x = self.detect(self, x)
+        x = Detect.forward(self, x)
         if self.training:
             return x, angle
         return torch.cat([x, angle], 1) if self.export else (torch.cat([x[0], angle], 1), (x[1], angle))
 
     def decode_bboxes(self, bboxes, anchors):
         """Decode rotated bounding boxes."""
         return dist2rbox(bboxes, self.angle, anchors, dim=1)
@@ -150,24 +148,23 @@
     """YOLOv8 Pose head for keypoints models."""
 
     def __init__(self, nc=80, kpt_shape=(17, 3), ch=()):
         """Initialize YOLO network with default parameters and Convolutional Layers."""
         super().__init__(nc, ch)
         self.kpt_shape = kpt_shape  # number of keypoints, number of dims (2 for x,y or 3 for x,y,visible)
         self.nk = kpt_shape[0] * kpt_shape[1]  # number of keypoints total
-        self.detect = Detect.forward
 
         c4 = max(ch[0] // 4, self.nk)
         self.cv4 = nn.ModuleList(nn.Sequential(Conv(x, c4, 3), Conv(c4, c4, 3), nn.Conv2d(c4, self.nk, 1)) for x in ch)
 
     def forward(self, x):
         """Perform forward pass through YOLO model and return predictions."""
         bs = x[0].shape[0]  # batch size
         kpt = torch.cat([self.cv4[i](x[i]).view(bs, self.nk, -1) for i in range(self.nl)], -1)  # (bs, 17*3, h*w)
-        x = self.detect(self, x)
+        x = Detect.forward(self, x)
         if self.training:
             return x, kpt
         pred_kpt = self.kpts_decode(bs, kpt)
         return torch.cat([x, pred_kpt], 1) if self.export else (torch.cat([x[0], pred_kpt], 1), (x[1], kpt))
 
     def kpts_decode(self, bs, kpts):
         """Decodes keypoints."""
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/transformer.py` & `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/nn/modules/utils.py` & `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/nn/tasks.py` & `vsensebox_ultralytics-8.2.15/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/solutions/ai_gym.py` & `vsensebox_ultralytics-8.2.15/ultralytics/solutions/ai_gym.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/solutions/distance_calculation.py` & `vsensebox_ultralytics-8.2.15/ultralytics/solutions/distance_calculation.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/solutions/heatmap.py` & `vsensebox_ultralytics-8.2.15/ultralytics/solutions/heatmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,17 +186,15 @@
                 self.annotator.draw_region(
                     reg_pts=self.count_reg_pts, color=self.region_color, thickness=self.region_thickness
                 )
 
             for box, cls, track_id in zip(self.boxes, self.clss, self.track_ids):
                 # Store class info
                 if self.names[cls] not in self.class_wise_count:
-                    if len(self.names[cls]) > 5:
-                        self.names[cls] = self.names[cls][:5]
-                    self.class_wise_count[self.names[cls]] = {"in": 0, "out": 0}
+                    self.class_wise_count[self.names[cls]] = {"IN": 0, "OUT": 0}
 
                 if self.shape == "circle":
                     center = (int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2))
                     radius = min(int(box[2]) - int(box[0]), int(box[3]) - int(box[1])) // 2
 
                     y, x = np.ogrid[0 : self.heatmap.shape[0], 0 : self.heatmap.shape[1]]
                     mask = (x - center[0]) ** 2 + (y - center[1]) ** 2 <= radius**2
@@ -221,32 +219,32 @@
                     is_inside = self.counting_region.contains(Point(track_line[-1]))
 
                     if prev_position is not None and is_inside and track_id not in self.count_ids:
                         self.count_ids.append(track_id)
 
                         if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                             self.in_counts += 1
-                            self.class_wise_count[self.names[cls]]["in"] += 1
+                            self.class_wise_count[self.names[cls]]["IN"] += 1
                         else:
                             self.out_counts += 1
-                            self.class_wise_count[self.names[cls]]["out"] += 1
+                            self.class_wise_count[self.names[cls]]["OUT"] += 1
 
                 # Count objects using line
                 elif len(self.count_reg_pts) == 2:
                     if prev_position is not None and track_id not in self.count_ids:
                         distance = Point(track_line[-1]).distance(self.counting_region)
                         if distance < self.line_dist_thresh and track_id not in self.count_ids:
                             self.count_ids.append(track_id)
 
                             if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                                 self.in_counts += 1
-                                self.class_wise_count[self.names[cls]]["in"] += 1
+                                self.class_wise_count[self.names[cls]]["IN"] += 1
                             else:
                                 self.out_counts += 1
-                                self.class_wise_count[self.names[cls]]["out"] += 1
+                                self.class_wise_count[self.names[cls]]["OUT"] += 1
 
         else:
             for box, cls in zip(self.boxes, self.clss):
                 if self.shape == "circle":
                     center = (int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2))
                     radius = min(int(box[2]) - int(box[0]), int(box[3]) - int(box[1])) // 2
 
@@ -260,36 +258,29 @@
                 else:
                     self.heatmap[int(box[1]) : int(box[3]), int(box[0]) : int(box[2])] += 2
 
         # Normalize, apply colormap to heatmap and combine with original image
         heatmap_normalized = cv2.normalize(self.heatmap, None, 0, 255, cv2.NORM_MINMAX)
         heatmap_colored = cv2.applyColorMap(heatmap_normalized.astype(np.uint8), self.colormap)
 
-        label = "Ultralytics Analytics \t"
+        labels_dict = {}
 
         for key, value in self.class_wise_count.items():
-            if value["in"] != 0 or value["out"] != 0:
+            if value["IN"] != 0 or value["OUT"] != 0:
                 if not self.view_in_counts and not self.view_out_counts:
-                    label = None
+                    continue
                 elif not self.view_in_counts:
-                    label += f"{str.capitalize(key)}: IN {value['in']} \t"
+                    labels_dict[str.capitalize(key)] = f"OUT {value['OUT']}"
                 elif not self.view_out_counts:
-                    label += f"{str.capitalize(key)}: OUT {value['out']} \t"
+                    labels_dict[str.capitalize(key)] = f"IN {value['IN']}"
                 else:
-                    label += f"{str.capitalize(key)}: IN {value['in']} OUT {value['out']} \t"
+                    labels_dict[str.capitalize(key)] = f"IN {value['IN']} OUT {value['OUT']}"
 
-        label = label.rstrip()
-        label = label.split("\t")
-
-        if self.count_reg_pts is not None and label is not None:
-            self.annotator.display_counts(
-                counts=label,
-                count_txt_color=self.count_txt_color,
-                count_bg_color=self.count_bg_color,
-            )
+        if labels_dict is not None:
+            self.annotator.display_analytics(self.im0, labels_dict, self.count_txt_color, self.count_bg_color, 10)
 
         self.im0 = cv2.addWeighted(self.im0, 1 - self.heatmap_alpha, heatmap_colored, self.heatmap_alpha, 0)
 
         if self.env_check and self.view_img:
             self.display_frames()
 
         return self.im0
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/solutions/object_counter.py` & `vsensebox_ultralytics-8.2.15/ultralytics/solutions/object_counter.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,17 +177,15 @@
             # Extract tracks
             for box, track_id, cls in zip(boxes, track_ids, clss):
                 # Draw bounding box
                 self.annotator.box_label(box, label=f"{self.names[cls]}#{track_id}", color=colors(int(track_id), True))
 
                 # Store class info
                 if self.names[cls] not in self.class_wise_count:
-                    if len(self.names[cls]) > 5:
-                        self.names[cls] = self.names[cls][:5]
-                    self.class_wise_count[self.names[cls]] = {"in": 0, "out": 0}
+                    self.class_wise_count[self.names[cls]] = {"IN": 0, "OUT": 0}
 
                 # Draw Tracks
                 track_line = self.track_history[track_id]
                 track_line.append((float((box[0] + box[2]) / 2), float((box[1] + box[3]) / 2)))
                 if len(track_line) > 30:
                     track_line.pop(0)
 
@@ -206,55 +204,48 @@
                     is_inside = self.counting_region.contains(Point(track_line[-1]))
 
                     if prev_position is not None and is_inside and track_id not in self.count_ids:
                         self.count_ids.append(track_id)
 
                         if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                             self.in_counts += 1
-                            self.class_wise_count[self.names[cls]]["in"] += 1
+                            self.class_wise_count[self.names[cls]]["IN"] += 1
                         else:
                             self.out_counts += 1
-                            self.class_wise_count[self.names[cls]]["out"] += 1
+                            self.class_wise_count[self.names[cls]]["OUT"] += 1
 
                 # Count objects using line
                 elif len(self.reg_pts) == 2:
                     if prev_position is not None and track_id not in self.count_ids:
                         distance = Point(track_line[-1]).distance(self.counting_region)
                         if distance < self.line_dist_thresh and track_id not in self.count_ids:
                             self.count_ids.append(track_id)
 
                             if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                                 self.in_counts += 1
-                                self.class_wise_count[self.names[cls]]["in"] += 1
+                                self.class_wise_count[self.names[cls]]["IN"] += 1
                             else:
                                 self.out_counts += 1
-                                self.class_wise_count[self.names[cls]]["out"] += 1
+                                self.class_wise_count[self.names[cls]]["OUT"] += 1
 
-        label = "Ultralytics Analytics \t"
+        labels_dict = {}
 
         for key, value in self.class_wise_count.items():
-            if value["in"] != 0 or value["out"] != 0:
+            if value["IN"] != 0 or value["OUT"] != 0:
                 if not self.view_in_counts and not self.view_out_counts:
-                    label = None
+                    continue
                 elif not self.view_in_counts:
-                    label += f"{str.capitalize(key)}: IN {value['in']} \t"
+                    labels_dict[str.capitalize(key)] = f"OUT {value['OUT']}"
                 elif not self.view_out_counts:
-                    label += f"{str.capitalize(key)}: OUT {value['out']} \t"
+                    labels_dict[str.capitalize(key)] = f"IN {value['IN']}"
                 else:
-                    label += f"{str.capitalize(key)}: IN {value['in']} OUT {value['out']} \t"
+                    labels_dict[str.capitalize(key)] = f"IN {value['IN']} OUT {value['OUT']}"
 
-        label = label.rstrip()
-        label = label.split("\t")
-
-        if label is not None:
-            self.annotator.display_counts(
-                counts=label,
-                count_txt_color=self.count_txt_color,
-                count_bg_color=self.count_bg_color,
-            )
+        if labels_dict is not None:
+            self.annotator.display_analytics(self.im0, labels_dict, self.count_txt_color, self.count_bg_color, 10)
 
     def display_frames(self):
         """Display frame."""
         if self.env_check:
             cv2.namedWindow(self.window_name)
             if len(self.reg_pts) == 4:  # only add mouse event If user drawn region
                 cv2.setMouseCallback(self.window_name, self.mouse_event_for_region, {"region_points": self.reg_pts})
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/solutions/queue_management.py` & `vsensebox_ultralytics-8.2.15/ultralytics/solutions/queue_management.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/solutions/speed_estimation.py` & `vsensebox_ultralytics-8.2.15/ultralytics/solutions/speed_estimation.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/trackers/basetrack.py` & `vsensebox_ultralytics-8.2.15/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/trackers/bot_sort.py` & `vsensebox_ultralytics-8.2.15/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/trackers/byte_tracker.py` & `vsensebox_ultralytics-8.2.15/ultralytics/trackers/byte_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,19 +260,19 @@
 
         scores = results.conf
         bboxes = results.xywhr if hasattr(results, "xywhr") else results.xywh
         # Add index
         bboxes = np.concatenate([bboxes, np.arange(len(bboxes)).reshape(-1, 1)], axis=-1)
         cls = results.cls
 
-        remain_inds = scores > self.args.track_high_thresh
+        remain_inds = scores >= self.args.track_high_thresh
         inds_low = scores > self.args.track_low_thresh
         inds_high = scores < self.args.track_high_thresh
 
-        inds_second = np.logical_and(inds_low, inds_high)
+        inds_second = inds_low & inds_high
         dets_second = bboxes[inds_second]
         dets = bboxes[remain_inds]
         scores_keep = scores[remain_inds]
         scores_second = scores[inds_second]
         cls_keep = cls[remain_inds]
         cls_second = cls[inds_second]
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/trackers/track.py` & `vsensebox_ultralytics-8.2.15/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/trackers/utils/gmc.py` & `vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/trackers/utils/kalman_filter.py` & `vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/trackers/utils/matching.py` & `vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 try:
     import lap  # for linear_assignment
 
     assert lap.__version__  # verify package is not directory
 except (ImportError, AssertionError, AttributeError):
     from ultralytics.utils.checks import check_requirements
 
-    check_requirements("lapx>=0.5.8")  # update to lap package from https://github.com/rathaROG/lapx
+    check_requirements("lapx>=0.5.9")  # update to lap package from https://github.com/rathaROG/lapx
     import lap
 
 
 def linear_assignment(cost_matrix: np.ndarray, thresh: float, use_lap: bool = True) -> tuple:
     """
     Perform linear assignment using scipy or lap.lapjv.
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/__init__.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 # Other Constants
 ARGV = sys.argv or ["", ""]  # sometimes sys.argv = []
 FILE = Path(__file__).resolve()
 ROOT = FILE.parents[1]  # YOLO
 ASSETS = ROOT / "assets"  # default images
 DEFAULT_CFG_PATH = ROOT / "cfg/default.yaml"
-NUM_THREADS = min(8, max(1, os.cpu_count() - 1))  # number of YOLOv5 multiprocessing threads
+NUM_THREADS = min(8, max(1, os.cpu_count() - 1))  # number of YOLO multiprocessing threads
 AUTOINSTALL = str(os.getenv("YOLO_AUTOINSTALL", True)).lower() == "true"  # global auto-install mode
 VERBOSE = str(os.getenv("YOLO_VERBOSE", True)).lower() == "true"  # global verbose mode
 TQDM_BAR_FORMAT = "{l_bar}{bar:10}{r_bar}" if VERBOSE else None  # tqdm bar format
 LOGGING_NAME = "ultralytics"
 MACOS, LINUX, WINDOWS = (platform.system() == x for x in ["Darwin", "Linux", "Windows"])  # environment booleans
 ARM64 = platform.machine() in {"arm64", "aarch64"}  # ARM64 booleans
 PYTHON_VERSION = platform.python_version()
@@ -57,15 +57,15 @@
         from ultralytics import YOLO
 
         # Load a model
         model = YOLO('yolov8n.yaml')  # build a new model from scratch
         model = YOLO("yolov8n.pt")  # load a pretrained model (recommended for training)
 
         # Use the model
-        results = model.train(data="coco128.yaml", epochs=3)  # train the model
+        results = model.train(data="coco8.yaml", epochs=3)  # train the model
         results = model.val()  # evaluate model performance on the validation set
         results = model('https://ultralytics.com/images/bus.jpg')  # predict on an image
         success = model.export(format='onnx')  # export the model to ONNX format
 
     3. Use the command line interface (CLI):
 
         YOLOv8 'yolo' CLI commands use the following syntax:
@@ -74,21 +74,21 @@
 
             Where   TASK (optional) is one of [detect, segment, classify]
                     MODE (required) is one of [train, val, predict, export]
                     ARGS (optional) are any number of custom 'arg=value' pairs like 'imgsz=320' that override defaults.
                         See all ARGS at https://docs.ultralytics.com/usage/cfg or with 'yolo cfg'
 
         - Train a detection model for 10 epochs with an initial learning_rate of 0.01
-            yolo detect train data=coco128.yaml model=yolov8n.pt epochs=10 lr0=0.01
+            yolo detect train data=coco8.yaml model=yolov8n.pt epochs=10 lr0=0.01
 
         - Predict a YouTube video using a pretrained segmentation model at image size 320:
             yolo segment predict model=yolov8n-seg.pt source='https://youtu.be/LNwODJXcvt4' imgsz=320
 
         - Val a pretrained detection model at batch-size 1 and image size 640:
-            yolo detect val model=yolov8n.pt data=coco128.yaml batch=1 imgsz=640
+            yolo detect val model=yolov8n.pt data=coco8.yaml batch=1 imgsz=640
 
         - Export a YOLOv8n classification model to ONNX format at image size 224 by 128 (no TASK required)
             yolo export model=yolov8n-cls.pt format=onnx imgsz=224,128
 
         - Run special commands:
             yolo help
             yolo checks
@@ -98,21 +98,23 @@
             yolo cfg
 
     Docs: https://docs.ultralytics.com
     Community: https://community.ultralytics.com
     GitHub: https://github.com/ultralytics/ultralytics
     """
 
-# Settings
+# Settings and Environment Variables
 torch.set_printoptions(linewidth=320, precision=4, profile="default")
 np.set_printoptions(linewidth=320, formatter={"float_kind": "{:11.5g}".format})  # format short g, %precision=5
 # cv2.setNumThreads(0)  # prevent OpenCV from multithreading (incompatible with PyTorch DataLoader)
 os.environ["NUMEXPR_MAX_THREADS"] = str(NUM_THREADS)  # NumExpr max threads
 os.environ["CUBLAS_WORKSPACE_CONFIG"] = ":4096:8"  # for deterministic training
-os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"  # suppress verbose TF compiler warnings in Colab
+os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"  # suppress verbose TF compiler warnings in Colab
+os.environ["TORCH_CPP_LOG_LEVEL"] = "ERROR"  # suppress "NNPACK.cpp could not initialize NNPACK" warnings
+os.environ["KINETO_LOG_LEVEL"] = "5"  # suppress verbose PyTorch profiler output when computing FLOPs
 
 
 class TQDM(tqdm_original):
     """
     Custom Ultralytics tqdm class with different default arguments.
 
     Args:
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/autobatch.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/benchmarks.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/benchmarks.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,26 +21,31 @@
 TensorFlow Edge TPU     | `edgetpu`                 | yolov8n_edgetpu.tflite
 TensorFlow.js           | `tfjs`                    | yolov8n_web_model/
 PaddlePaddle            | `paddle`                  | yolov8n_paddle_model/
 NCNN                    | `ncnn`                    | yolov8n_ncnn_model/
 """
 
 import glob
+import os
 import platform
+import re
+import shutil
 import time
 from pathlib import Path
 
 import numpy as np
 import torch.cuda
+import yaml
 
 from ultralytics import YOLO, YOLOWorld
 from ultralytics.cfg import TASK2DATA, TASK2METRIC
 from ultralytics.engine.exporter import export_formats
-from ultralytics.utils import ASSETS, LINUX, LOGGER, MACOS, TQDM, WEIGHTS_DIR
+from ultralytics.utils import ARM64, ASSETS, IS_JETSON, IS_RASPBERRYPI, LINUX, LOGGER, MACOS, TQDM, WEIGHTS_DIR
 from ultralytics.utils.checks import IS_PYTHON_3_12, check_requirements, check_yolo
+from ultralytics.utils.downloads import safe_download
 from ultralytics.utils.files import file_size
 from ultralytics.utils.torch_utils import select_device
 
 
 def benchmark(
     model=WEIGHTS_DIR / "yolov8n.pt", data=None, imgsz=160, half=False, int8=False, device="cpu", verbose=False
 ):
@@ -79,16 +84,18 @@
 
     y = []
     t0 = time.time()
     for i, (name, format, suffix, cpu, gpu) in export_formats().iterrows():  # index, (name, format, suffix, CPU, GPU)
         emoji, filename = "❌", None  # export defaults
         try:
             # Checks
+            if i == 5:  # CoreML
+                assert not (IS_RASPBERRYPI or IS_JETSON), "CoreML export not supported on Raspberry Pi or NVIDIA Jetson"
             if i == 9:  # Edge TPU
-                assert LINUX, "Edge TPU export only supported on Linux"
+                assert LINUX and not ARM64, "Edge TPU export only supported on non-aarch64 Linux"
             elif i == 7:  # TF GraphDef
                 assert model.task != "obb", "TensorFlow GraphDef not supported for OBB task"
             elif i in {5, 10}:  # CoreML and TF.js
                 assert MACOS or LINUX, "export only supported on macOS and Linux"
             if i in {3, 5}:  # CoreML and OpenVINO
                 assert not IS_PYTHON_3_12, "CoreML and OpenVINO not supported on Python 3.12"
             if i in {6, 7, 8, 9, 10}:  # All TF formats
@@ -121,24 +128,25 @@
             # Validate
             data = data or TASK2DATA[model.task]  # task to dataset, i.e. coco8.yaml for task=detect
             key = TASK2METRIC[model.task]  # task to metric, i.e. metrics/mAP50-95(B) for task=detect
             results = exported_model.val(
                 data=data, batch=1, imgsz=imgsz, plots=False, device=device, half=half, int8=int8, verbose=False
             )
             metric, speed = results.results_dict[key], results.speed["inference"]
-            y.append([name, "✅", round(file_size(filename), 1), round(metric, 4), round(speed, 2)])
+            fps = round((1000 / speed), 2)  # frames per second
+            y.append([name, "✅", round(file_size(filename), 1), round(metric, 4), round(speed, 2), fps])
         except Exception as e:
             if verbose:
                 assert type(e) is AssertionError, f"Benchmark failure for {name}: {e}"
             LOGGER.warning(f"ERROR ❌️ Benchmark failure for {name}: {e}")
-            y.append([name, emoji, round(file_size(filename), 1), None, None])  # mAP, t_inference
+            y.append([name, emoji, round(file_size(filename), 1), None, None, None])  # mAP, t_inference
 
     # Print results
     check_yolo(device=device)  # print system info
-    df = pd.DataFrame(y, columns=["Format", "Status❔", "Size (MB)", key, "Inference time (ms/im)"])
+    df = pd.DataFrame(y, columns=["Format", "Status❔", "Size (MB)", key, "Inference time (ms/im)", "FPS"])
 
     name = Path(model.ckpt_path).name
     s = f"\nBenchmarks complete for {name} on {data} at imgsz={imgsz} ({time.time() - t0:.2f}s)\n{df}\n"
     LOGGER.info(s)
     with open("benchmarks.log", "a", errors="ignore", encoding="utf-8") as f:
         f.write(s)
 
@@ -146,14 +154,141 @@
         metrics = df[key].array  # values to compare to floor
         floor = verbose  # minimum metric floor to pass, i.e. = 0.29 mAP for YOLOv5n
         assert all(x > floor for x in metrics if pd.notna(x)), f"Benchmark failure: metric(s) < floor {floor}"
 
     return df
 
 
+class RF100Benchmark:
+    def __init__(self):
+        """Function for initialization of RF100Benchmark."""
+        self.ds_names = []
+        self.ds_cfg_list = []
+        self.rf = None
+        self.val_metrics = ["class", "images", "targets", "precision", "recall", "map50", "map95"]
+
+    def set_key(self, api_key):
+        """
+        Set Roboflow API key for processing.
+
+        Args:
+            api_key (str): The API key.
+        """
+
+        check_requirements("roboflow")
+        from roboflow import Roboflow
+
+        self.rf = Roboflow(api_key=api_key)
+
+    def parse_dataset(self, ds_link_txt="datasets_links.txt"):
+        """
+        Parse dataset links and downloads datasets.
+
+        Args:
+            ds_link_txt (str): Path to dataset_links file.
+        """
+
+        (shutil.rmtree("rf-100"), os.mkdir("rf-100")) if os.path.exists("rf-100") else os.mkdir("rf-100")
+        os.chdir("rf-100")
+        os.mkdir("ultralytics-benchmarks")
+        safe_download("https://ultralytics.com/assets/datasets_links.txt")
+
+        with open(ds_link_txt, "r") as file:
+            for line in file:
+                try:
+                    _, url, workspace, project, version = re.split("/+", line.strip())
+                    self.ds_names.append(project)
+                    proj_version = f"{project}-{version}"
+                    if not Path(proj_version).exists():
+                        self.rf.workspace(workspace).project(project).version(version).download("yolov8")
+                    else:
+                        print("Dataset already downloaded.")
+                    self.ds_cfg_list.append(Path.cwd() / proj_version / "data.yaml")
+                except Exception:
+                    continue
+
+        return self.ds_names, self.ds_cfg_list
+
+    def fix_yaml(self, path):
+        """
+        Function to fix yaml train and val path.
+
+        Args:
+            path (str): YAML file path.
+        """
+
+        with open(path, "r") as file:
+            yaml_data = yaml.safe_load(file)
+        yaml_data["train"] = "train/images"
+        yaml_data["val"] = "valid/images"
+        with open(path, "w") as file:
+            yaml.safe_dump(yaml_data, file)
+
+    def evaluate(self, yaml_path, val_log_file, eval_log_file, list_ind):
+        """
+        Model evaluation on validation results.
+
+        Args:
+            yaml_path (str): YAML file path.
+            val_log_file (str): val_log_file path.
+            eval_log_file (str): eval_log_file path.
+            list_ind (int): Index for current dataset.
+        """
+        skip_symbols = ["🚀", "⚠️", "💡", "❌"]
+        with open(yaml_path) as stream:
+            class_names = yaml.safe_load(stream)["names"]
+        with open(val_log_file, "r", encoding="utf-8") as f:
+            lines = f.readlines()
+            eval_lines = []
+            for line in lines:
+                if any(symbol in line for symbol in skip_symbols):
+                    continue
+                entries = line.split(" ")
+                entries = list(filter(lambda val: val != "", entries))
+                entries = [e.strip("\n") for e in entries]
+                start_class = False
+                for e in entries:
+                    if e == "all":
+                        if "(AP)" not in entries:
+                            if "(AR)" not in entries:
+                                # parse all
+                                eval = {}
+                                eval["class"] = entries[0]
+                                eval["images"] = entries[1]
+                                eval["targets"] = entries[2]
+                                eval["precision"] = entries[3]
+                                eval["recall"] = entries[4]
+                                eval["map50"] = entries[5]
+                                eval["map95"] = entries[6]
+                                eval_lines.append(eval)
+
+                    if e in class_names:
+                        eval = {}
+                        eval["class"] = entries[0]
+                        eval["images"] = entries[1]
+                        eval["targets"] = entries[2]
+                        eval["precision"] = entries[3]
+                        eval["recall"] = entries[4]
+                        eval["map50"] = entries[5]
+                        eval["map95"] = entries[6]
+                        eval_lines.append(eval)
+        map_val = 0.0
+        if len(eval_lines) > 1:
+            print("There's more dicts")
+            for lst in eval_lines:
+                if lst["class"] == "all":
+                    map_val = lst["map50"]
+        else:
+            print("There's only one dict res")
+            map_val = [res["map50"] for res in eval_lines][0]
+
+        with open(eval_log_file, "a") as f:
+            f.write(f"{self.ds_names[list_ind]}: {map_val}\n")
+
+
 class ProfileModels:
     """
     ProfileModels class for profiling different models on ONNX and TensorRT.
 
     This class profiles the performance of different models, returning results such as model speed and FLOPs.
 
     Attributes:
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/base.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/clearml.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/comet.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/dvc.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/hub.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/mlflow.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/neptune.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/raytune.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/tensorboard.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/callbacks/wb.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/checks.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,34 +249,34 @@
         if hard:
             raise ModuleNotFoundError(emojis(warning))  # assert version requirements met
         if verbose:
             LOGGER.warning(warning)
     return result
 
 
-def check_latest_pypi_version(package_name="vsensebox-ultralytics"):
+def check_latest_pypi_version(package_name="pyppbox-ultralytics"):
     """
     Returns the latest version of a PyPI package without downloading or installing it.
 
     Parameters:
         package_name (str): The name of the package to find the latest version for.
 
     Returns:
         (str): The latest version of the package.
     """
-    if package_name == 'vsensebox-ultralytics':
+    if package_name == 'pyppbox-ultralytics':
         with contextlib.suppress(Exception):
             requests.packages.urllib3.disable_warnings()  # Disable the InsecureRequestWarning
             response = requests.get(f'https://pypi.org/pypi/{package_name}/json', timeout=3)
             if response.status_code == 200:
                 return response.json()['info']['version']
     else:
         LOGGER.info(
-        f'This is custom vsensebox-ultralytics for VsenseBox 😃 '
-        f"🌐 Check for the update here: https://github.com/rathaumons/ultralytics-for-vsensebox")
+        f'This is custom pyppbox-ultralytics for pyppbox 😃 '
+        f"🌐 Check for the update here: https://github.com/rathaumons/ultralytics-for-pyppbox")
     return None
 
 
 def check_pip_update_available():
     """
     Checks if a new version of the ultralytics package is available on PyPI.
 
@@ -286,16 +286,16 @@
     if ONLINE and IS_PIP_PACKAGE:
         with contextlib.suppress(Exception):
             from ultralytics import __version__
 
             latest = check_latest_pypi_version()
             if check_version(__version__, f"<{latest}"):  # check if current version is < latest version
                 LOGGER.info(
-                    f"New https://pypi.org/project/vsensebox-ultralytics/{latest} available 😃 "
-                    f"Update with 'pip install -U vsensebox-ultralytics'"
+                    f"New https://pypi.org/project/pyppbox-ultralytics/{latest} available 😃 "
+                    f"Update with 'pip install -U pyppbox-ultralytics'"
                 )
                 return True
     return False
 
 
 @ThreadingLocked()
 def check_font(font="Arial.ttf"):
@@ -421,15 +421,22 @@
     https://github.com/pytorch/vision#installation.
 
     The compatibility table is a dictionary where the keys are PyTorch versions and the values are lists of compatible
     Torchvision versions.
     """
 
     # Compatibility table
-    compatibility_table = {"2.0": ["0.15"], "1.13": ["0.14"], "1.12": ["0.13"]}
+    compatibility_table = {
+        "2.3": ["0.18"],
+        "2.2": ["0.17"],
+        "2.1": ["0.16"],
+        "2.0": ["0.15"],
+        "1.13": ["0.14"],
+        "1.12": ["0.13"],
+    }
 
     # Extract only the major and minor versions
     v_torch = ".".join(torch.__version__.split("+")[0].split(".")[:2])
     v_torchvision = ".".join(TORCHVISION_VERSION.split("+")[0].split(".")[:2])
 
     if v_torch in compatibility_table:
         compatible_versions = compatibility_table[v_torch]
@@ -523,15 +530,15 @@
 
     Returns:
         (bool): True if the path is safe, False otherwise.
     """
     base_dir_resolved = Path(basedir).resolve()
     path_resolved = Path(path).resolve()
 
-    return path_resolved.is_file() and path_resolved.parts[: len(base_dir_resolved.parts)] == base_dir_resolved.parts
+    return path_resolved.exists() and path_resolved.parts[: len(base_dir_resolved.parts)] == base_dir_resolved.parts
 
 
 def check_imshow(warn=False):
     """Check if environment supports image displays."""
     try:
         if LINUX:
             assert "DISPLAY" in os.environ and not IS_DOCKER and not IS_COLAB and not IS_KAGGLE
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/dist.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/downloads.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/downloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,31 +398,31 @@
     if r.status_code != 200:
         LOGGER.warning(f"⚠️ GitHub assets check failure for {url}: {r.status_code} {r.reason}")
         return "", []
     data = r.json()
     return data["tag_name"], [x["name"] for x in data["assets"]]  # tag, assets i.e. ['yolov8n.pt', 'yolov8s.pt', ...]
 
 
-def attempt_download_asset(file, repo="ultralytics/assets", release="v8.1.0", **kwargs):
+def attempt_download_asset(file, repo="ultralytics/assets", release="v8.2.0", **kwargs):
     """
     Attempt to download a file from GitHub release assets if it is not found locally. The function checks for the file
     locally first, then tries to download it from the specified GitHub repository release.
 
     Args:
         file (str | Path): The filename or file path to be downloaded.
         repo (str, optional): The GitHub repository in the format 'owner/repo'. Defaults to 'ultralytics/assets'.
-        release (str, optional): The specific release version to be downloaded. Defaults to 'v8.1.0'.
+        release (str, optional): The specific release version to be downloaded. Defaults to 'v8.2.0'.
         **kwargs (any): Additional keyword arguments for the download process.
 
     Returns:
         (str): The path to the downloaded file.
 
     Example:
         ```python
-        file_path = attempt_download_asset('yolov5s.pt', repo='ultralytics/assets', release='latest')
+        file_path = attempt_download_asset('yolov8n.pt', repo='ultralytics/assets', release='latest')
         ```
     """
     from ultralytics.utils import SETTINGS  # scoped for circular import
 
     # YOLOv3/5u updates
     file = str(file)
     file = checks.check_yolov5u_filename(file)
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/errors.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/errors.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/files.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/files.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/instance.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,19 @@
         else:
             func = ltwh2xyxy if format == "xyxy" else ltwh2xywh
         self.bboxes = func(self.bboxes)
         self.format = format
 
     def areas(self):
         """Return box areas."""
-        self.convert("xyxy")
-        return (self.bboxes[:, 2] - self.bboxes[:, 0]) * (self.bboxes[:, 3] - self.bboxes[:, 1])
+        return (
+            (self.bboxes[:, 2] - self.bboxes[:, 0]) * (self.bboxes[:, 3] - self.bboxes[:, 1])  # format xyxy
+            if self.format == "xyxy"
+            else self.bboxes[:, 3] * self.bboxes[:, 2]  # format xywh or ltwh
+        )
 
     # def denormalize(self, w, h):
     #    if not self.normalized:
     #         return
     #     assert (self.bboxes <= 1.0).all()
     #     self.bboxes[:, 0::2] *= w
     #     self.bboxes[:, 1::2] *= h
@@ -336,19 +339,15 @@
         self.segments[..., 0] = self.segments[..., 0].clip(0, w)
         self.segments[..., 1] = self.segments[..., 1].clip(0, h)
         if self.keypoints is not None:
             self.keypoints[..., 0] = self.keypoints[..., 0].clip(0, w)
             self.keypoints[..., 1] = self.keypoints[..., 1].clip(0, h)
 
     def remove_zero_area_boxes(self):
-        """
-        Remove zero-area boxes, i.e. after clipping some boxes may have zero width or height.
-
-        This removes them.
-        """
+        """Remove zero-area boxes, i.e. after clipping some boxes may have zero width or height."""
         good = self.bbox_areas > 0
         if not all(good):
             self._bboxes = self._bboxes[good]
             if len(self.segments):
                 self.segments = self.segments[good]
             if self.keypoints is not None:
                 self.keypoints = self.keypoints[good]
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/loss.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/metrics.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/ops.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/ops.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/patches.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/plotting.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -415,64 +415,71 @@
             0,
             fontScale=fontsize,
             color=txt_color,
             thickness=self.tf,
             lineType=cv2.LINE_AA,
         )
 
-    def display_counts(self, counts=None, count_bg_color=(0, 0, 0), count_txt_color=(255, 255, 255)):
+    ### Parking management utils
+    def display_objects_labels(self, im0, text, txt_color, bg_color, x_center, y_center, margin):
         """
-        Display counts on im0 with text background and border.
+        Display the bounding boxes labels in parking management app.
 
         Args:
-            counts (str): objects count data
-            count_bg_color (RGB Color): counts highlighter color
-            count_txt_color (RGB Color): counts display color
-        """
-
-        tl = self.tf or round(0.002 * (self.im.shape[0] + self.im.shape[1]) / 2) + 1
-        tf = max(tl - 1, 1)
-
-        t_sizes = [cv2.getTextSize(str(count), 0, fontScale=self.sf, thickness=self.tf)[0] for count in counts]
-
-        max_text_width = max([size[0] for size in t_sizes])
-        max_text_height = max([size[1] for size in t_sizes])
-
-        text_x = self.im.shape[1] - int(self.im.shape[1] * 0.025 + max_text_width)
-        text_y = int(self.im.shape[0] * 0.025)
-
-        # Calculate dynamic gap between each count value based on the width of the image
-        dynamic_gap = max(1, self.im.shape[1] // 100) * tf
+            im0 (ndarray): inference image
+            text (str): object/class name
+            txt_color (bgr color): display color for text foreground
+            bg_color (bgr color): display color for text background
+            x_center (float): x position center point for bounding box
+            y_center (float): y position center point for bounding box
+            margin (int): gap between text and rectangle for better display
+        """
+
+        text_size = cv2.getTextSize(text, 0, fontScale=self.sf, thickness=self.tf)[0]
+        text_x = x_center - text_size[0] // 2
+        text_y = y_center + text_size[1] // 2
+
+        rect_x1 = text_x - margin
+        rect_y1 = text_y - text_size[1] - margin
+        rect_x2 = text_x + text_size[0] + margin
+        rect_y2 = text_y + margin
+        cv2.rectangle(im0, (rect_x1, rect_y1), (rect_x2, rect_y2), bg_color, -1)
+        cv2.putText(im0, text, (text_x, text_y), 0, self.sf, txt_color, self.tf, lineType=cv2.LINE_AA)
 
-        for i, count in enumerate(counts):
-            text_x_pos = text_x
-            text_y_pos = text_y + i * dynamic_gap  # Adjust vertical position with dynamic gap
-
-            # Draw the border
-            cv2.rectangle(
-                self.im,
-                (text_x_pos - (10 * tf), text_y_pos - (10 * tf)),
-                (text_x_pos + max_text_width + (10 * tf), text_y_pos + max_text_height + (10 * tf)),
-                count_bg_color,
-                -1,
-            )
-
-            # Draw the count text
+    # Parking lot and object counting app
+    def display_analytics(self, im0, text, txt_color, bg_color, margin):
+        """
+        Display the overall statistics for parking lots
+        Args:
+            im0 (ndarray): inference image
+            text (dict): labels dictionary
+            txt_color (bgr color): display color for text foreground
+            bg_color (bgr color): display color for text background
+            margin (int): gap between text and rectangle for better display
+        """
+
+        horizontal_gap = int(im0.shape[1] * 0.02)
+        vertical_gap = int(im0.shape[0] * 0.01)
+
+        text_y_offset = 0
+
+        for label, value in text.items():
+            txt = f"{label}: {value}"
+            text_size = cv2.getTextSize(txt, 0, int(self.sf * 1.5), int(self.tf * 1.5))[0]
+            text_x = im0.shape[1] - text_size[0] - margin * 2 - horizontal_gap
+            text_y = text_y_offset + text_size[1] + margin * 2 + vertical_gap
+            rect_x1 = text_x - margin * 2
+            rect_y1 = text_y - text_size[1] - margin * 2
+            rect_x2 = text_x + text_size[0] + margin * 2
+            rect_y2 = text_y + margin * 2
+            cv2.rectangle(im0, (rect_x1, rect_y1), (rect_x2, rect_y2), bg_color, -1)
             cv2.putText(
-                self.im,
-                str(count),
-                (text_x_pos, text_y_pos + max_text_height),
-                0,
-                fontScale=self.sf,
-                color=count_txt_color,
-                thickness=self.tf,
-                lineType=cv2.LINE_AA,
+                im0, txt, (text_x, text_y), 0, int(self.sf * 1.5), txt_color, int(self.tf * 1.5), lineType=cv2.LINE_AA
             )
-
-            text_y_pos += tf * max_text_height
+            text_y_offset = rect_y2
 
     @staticmethod
     def estimate_pose_angle(a, b, c):
         """
         Calculate the pose angle for object.
 
         Args:
@@ -1094,27 +1101,28 @@
     Args:
         x (torch.Tensor): Features to be visualized.
         module_type (str): Module type.
         stage (int): Module stage within the model.
         n (int, optional): Maximum number of feature maps to plot. Defaults to 32.
         save_dir (Path, optional): Directory to save results. Defaults to Path('runs/detect/exp').
     """
-    for m in ["Detect", "Pose", "Segment"]:
+    for m in {"Detect", "Segment", "Pose", "Classify", "OBB", "RTDETRDecoder"}:  # all model heads
         if m in module_type:
             return
-    _, channels, height, width = x.shape  # batch, channels, height, width
-    if height > 1 and width > 1:
-        f = save_dir / f"stage{stage}_{module_type.split('.')[-1]}_features.png"  # filename
-
-        blocks = torch.chunk(x[0].cpu(), channels, dim=0)  # select batch index 0, block by channels
-        n = min(n, channels)  # number of plots
-        _, ax = plt.subplots(math.ceil(n / 8), 8, tight_layout=True)  # 8 rows x n/8 cols
-        ax = ax.ravel()
-        plt.subplots_adjust(wspace=0.05, hspace=0.05)
-        for i in range(n):
-            ax[i].imshow(blocks[i].squeeze())  # cmap='gray'
-            ax[i].axis("off")
-
-        LOGGER.info(f"Saving {f}... ({n}/{channels})")
-        plt.savefig(f, dpi=300, bbox_inches="tight")
-        plt.close()
-        np.save(str(f.with_suffix(".npy")), x[0].cpu().numpy())  # npy save
+    if isinstance(x, torch.Tensor):
+        _, channels, height, width = x.shape  # batch, channels, height, width
+        if height > 1 and width > 1:
+            f = save_dir / f"stage{stage}_{module_type.split('.')[-1]}_features.png"  # filename
+
+            blocks = torch.chunk(x[0].cpu(), channels, dim=0)  # select batch index 0, block by channels
+            n = min(n, channels)  # number of plots
+            _, ax = plt.subplots(math.ceil(n / 8), 8, tight_layout=True)  # 8 rows x n/8 cols
+            ax = ax.ravel()
+            plt.subplots_adjust(wspace=0.05, hspace=0.05)
+            for i in range(n):
+                ax[i].imshow(blocks[i].squeeze())  # cmap='gray'
+                ax[i].axis("off")
+
+            LOGGER.info(f"Saving {f}... ({n}/{channels})")
+            plt.savefig(f, dpi=300, bbox_inches="tight")
+            plt.close()
+            np.save(str(f.with_suffix(".npy")), x[0].cpu().numpy())  # npy save
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/tal.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/tal.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/torch_utils.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/torch_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
+import gc
 import math
 import os
 import random
 import time
 from contextlib import contextmanager
 from copy import deepcopy
 from pathlib import Path
@@ -326,27 +327,36 @@
             im = torch.empty((1, p.shape[1], *imgsz), device=p.device)  # input image in BCHW format
             return thop.profile(deepcopy(model), inputs=[im], verbose=False)[0] / 1e9 * 2  # imgsz GFLOPs
     except Exception:
         return 0.0
 
 
 def get_flops_with_torch_profiler(model, imgsz=640):
-    """Compute model FLOPs (thop alternative)."""
-    if TORCH_2_0:
-        model = de_parallel(model)
-        p = next(model.parameters())
+    """Compute model FLOPs (thop package alternative, but 2-10x slower unfortunately)."""
+    if not TORCH_2_0:  # torch profiler implemented in torch>=2.0
+        return 0.0
+    model = de_parallel(model)
+    p = next(model.parameters())
+    if not isinstance(imgsz, list):
+        imgsz = [imgsz, imgsz]  # expand if int/float
+    try:
+        # Use stride size for input tensor
         stride = (max(int(model.stride.max()), 32) if hasattr(model, "stride") else 32) * 2  # max stride
-        im = torch.zeros((1, p.shape[1], stride, stride), device=p.device)  # input image in BCHW format
+        im = torch.empty((1, p.shape[1], stride, stride), device=p.device)  # input image in BCHW format
         with torch.profiler.profile(with_flops=True) as prof:
             model(im)
         flops = sum(x.flops for x in prof.key_averages()) / 1e9
-        imgsz = imgsz if isinstance(imgsz, list) else [imgsz, imgsz]  # expand if int/float
         flops = flops * imgsz[0] / stride * imgsz[1] / stride  # 640x640 GFLOPs
-        return flops
-    return 0
+    except Exception:
+        # Use actual image size for input tensor (i.e. required for RTDETR models)
+        im = torch.empty((1, p.shape[1], *imgsz), device=p.device)  # input image in BCHW format
+        with torch.profiler.profile(with_flops=True) as prof:
+            model(im)
+        flops = sum(x.flops for x in prof.key_averages()) / 1e9
+    return flops
 
 
 def initialize_weights(model):
     """Initialize model weights to random values."""
     for m in model.modules():
         t = type(m)
         if t is nn.Conv2d:
@@ -385,16 +395,21 @@
         if (len(include) and k not in include) or k.startswith("_") or k in exclude:
             continue
         else:
             setattr(a, k, v)
 
 
 def get_latest_opset():
-    """Return second-most (for maturity) recently supported ONNX opset by this version of torch."""
-    return max(int(k[14:]) for k in vars(torch.onnx) if "symbolic_opset" in k) - 1  # opset
+    """Return the second-most recent ONNX opset version supported by this version of PyTorch, adjusted for maturity."""
+    if TORCH_1_13:
+        # If the PyTorch>=1.13, dynamically compute the latest opset minus one using 'symbolic_opset'
+        return max(int(k[14:]) for k in vars(torch.onnx) if "symbolic_opset" in k) - 1
+    # Otherwise for PyTorch<=1.12 return the corresponding predefined opset
+    version = torch.onnx.producer_version.rsplit(".", 1)[0]  # i.e. '2.3'
+    return {"1.12": 15, "1.11": 14, "1.10": 13, "1.9": 12, "1.8": 12}.get(version, 12)
 
 
 def intersect_dicts(da, db, exclude=()):
     """Returns a dictionary of intersecting keys with matching shapes, excluding 'exclude' keys, using da values."""
     return {k: v for k, v in da.items() if k in db and all(x not in k for x in exclude) and v.shape == db[k].shape}
 
 
@@ -577,14 +592,15 @@
                 s_in, s_out = (tuple(x.shape) if isinstance(x, torch.Tensor) else "list" for x in (x, y))  # shapes
                 p = sum(x.numel() for x in m.parameters()) if isinstance(m, nn.Module) else 0  # parameters
                 LOGGER.info(f"{p:12}{flops:12.4g}{mem:>14.3f}{tf:14.4g}{tb:14.4g}{str(s_in):>24s}{str(s_out):>24s}")
                 results.append([p, flops, mem, tf, tb, s_in, s_out])
             except Exception as e:
                 LOGGER.info(e)
                 results.append(None)
+            gc.collect()  # attempt to free unused memory
             torch.cuda.empty_cache()
     return results
 
 
 class EarlyStopping:
     """Early stopping class that stops training when a specified number of epochs have passed without improvement."""
```

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/triton.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/triton.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.1.48/ultralytics/utils/tuner.py` & `vsensebox_ultralytics-8.2.15/ultralytics/utils/tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     try:
         import wandb
 
         assert hasattr(wandb, "__version__")
     except (ImportError, AssertionError):
         wandb = False
 
-    checks.check_version(ray.__version__, "<=2.9.3", "ray")
+    checks.check_version(ray.__version__, ">=2.0.0", "ray")
     default_space = {
         # 'optimizer': tune.choice(['SGD', 'Adam', 'AdamW', 'NAdam', 'RAdam', 'RMSProp']),
         "lr0": tune.uniform(1e-5, 1e-1),
         "lrf": tune.uniform(0.01, 1.0),  # final OneCycleLR learning rate (lr0 * lrf)
         "momentum": tune.uniform(0.6, 0.98),  # SGD momentum/Adam beta1
         "weight_decay": tune.uniform(0.0, 0.001),  # optimizer weight decay 5e-4
         "warmup_epochs": tune.uniform(0.0, 5.0),  # warmup epochs (fractions ok)
```

### Comparing `vsensebox_ultralytics-8.1.48/vsensebox_ultralytics.egg-info/PKG-INFO` & `vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsensebox-ultralytics
-Version: 8.1.48
+Version: 8.2.15
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/rathaumons/ultralytics-for-vsensebox
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/rathaumons/ultralytics-for-vsensebox/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/rathaumons/ultralytics-for-vsensebox
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics
@@ -51,16 +51,16 @@
 Requires-Dist: duckdb<=0.9.2; extra == "explorer"
 Requires-Dist: streamlit; extra == "explorer"
 
 [![Test Build](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml) [![PyPI](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml)
 
 # Customized Ultralytics for VSenseBox
 
-* Updated: **May 2, 2024**
-* Synced with: v8.1.48 -> [[c54b013]](https://github.com/ultralytics/ultralytics/commit/c54b013188870dafdd5ce0d78b3f5f3fdee655fd)
+* Updated: **May 14, 2024**
+* Synced with: v8.2.15 -> [[590002f]](https://github.com/ultralytics/ultralytics/commit/590002ff6d3a936b0cb1aeb582ea2daa26fcdbb6)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
 * Customized for [`VSenseBox`](https://github.com/rathaumons/vsensebox):
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
```

### Comparing `vsensebox_ultralytics-8.1.48/vsensebox_ultralytics.egg-info/SOURCES.txt` & `vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
+tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
+tests/test_cuda.py
 tests/test_engine.py
+tests/test_explorer.py
+tests/test_exports.py
+tests/test_integrations.py
 tests/test_python.py
 ultralytics/__init__.py
 ultralytics/assets/bus.jpg
 ultralytics/assets/zidane.jpg
 ultralytics/cfg/__init__.py
 ultralytics/cfg/default.yaml
 ultralytics/cfg/datasets/Argoverse.yaml
@@ -164,14 +169,15 @@
 ultralytics/nn/modules/transformer.py
 ultralytics/nn/modules/utils.py
 ultralytics/solutions/__init__.py
 ultralytics/solutions/ai_gym.py
 ultralytics/solutions/distance_calculation.py
 ultralytics/solutions/heatmap.py
 ultralytics/solutions/object_counter.py
+ultralytics/solutions/parking_management.py
 ultralytics/solutions/queue_management.py
 ultralytics/solutions/speed_estimation.py
 ultralytics/trackers/__init__.py
 ultralytics/trackers/basetrack.py
 ultralytics/trackers/bot_sort.py
 ultralytics/trackers/byte_tracker.py
 ultralytics/trackers/track.py
```

### Comparing `vsensebox_ultralytics-8.1.48/vsensebox_ultralytics.egg-info/top_level.txt` & `vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/top_level.txt`

 * *Files identical despite different names*

