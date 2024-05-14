# Comparing `tmp/mlcvzoo_base-5.7.2.tar.gz` & `tmp/mlcvzoo_base-5.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_base-5.7.2.tar", max compression
+gzip compressed data, was "mlcvzoo_base-5.7.3.tar", last modified: Tue May 14 14:05:56 2024, max compression
```

## Comparing `mlcvzoo_base-5.7.2.tar` & `mlcvzoo_base-5.7.3.tar`

### file list

```diff
@@ -1,102 +1,385 @@
--rw-r--r--   0        0        0    11412 2024-03-04 08:38:20.164380 mlcvzoo_base-5.7.2/LICENSE
--rw-r--r--   0        0        0      547 2024-03-25 17:33:12.630680 mlcvzoo_base-5.7.2/README.md
--rw-r--r--   0        0        0      244 2024-04-05 08:00:50.573919 mlcvzoo_base-5.7.2/mlcvzoo_base/__init__.py
--rw-r--r--   0        0        0      196 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/__init__.py
--rw-r--r--   0        0        0     1021 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/configuration.py
--rw-r--r--   0        0        0      196 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/__init__.py
--rw-r--r--   0        0        0    11278 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation.py
--rw-r--r--   0        0        0      998 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_attributes.py
--rw-r--r--   0        0        0     2429 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_builder.py
--rw-r--r--   0        0        0    26718 2024-04-05 08:00:50.573919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_class_mapper.py
--rw-r--r--   0        0        0     1130 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_parser.py
--rw-r--r--   0        0        0      975 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_writer.py
--rw-r--r--   0        0        0     6558 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/bounding_box.py
--rw-r--r--   0        0        0    13370 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/box.py
--rw-r--r--   0        0        0     2734 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/class_identifier.py
--rw-r--r--   0        0        0     5309 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/classification.py
--rw-r--r--   0        0        0     3941 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/dataset_info.py
--rw-r--r--   0        0        0     3268 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/ocr_perception.py
--rw-r--r--   0        0        0    12107 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/segmentation.py
--rw-r--r--   0        0        0      457 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/types.py
--rw-r--r--   0        0        0      906 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/exceptions.py
--rw-r--r--   0        0        0     5029 2024-03-28 09:50:55.622541 mlcvzoo_base-5.7.2/mlcvzoo_base/api/interfaces.py
--rw-r--r--   0        0        0    13224 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/model.py
--rw-r--r--   0        0        0     2656 2024-03-27 06:44:37.840931 mlcvzoo_base-5.7.2/mlcvzoo_base/api/registry.py
--rw-r--r--   0        0        0      482 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/structs.py
--rw-r--r--   0        0        0      196 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/__init__.py
--rw-r--r--   0        0        0     8464 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/annotation_handler_config.py
--rw-r--r--   0        0        0     3942 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/class_mapping_config.py
--rw-r--r--   0        0        0      655 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/config_registry.py
--rw-r--r--   0        0        0      772 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/device_query.py
--rw-r--r--   0        0        0     1692 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/mlfow_config.py
--rw-r--r--   0        0        0     3093 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/model_config.py
--rw-r--r--   0        0        0     2589 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/reduction_mapping_config.py
--rw-r--r--   0        0        0     3889 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/replacement_config.py
--rw-r--r--   0        0        0     3939 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/structs.py
--rw-r--r--   0        0        0     7286 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/utils.py
--rw-r--r--   0        0        0      628 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/visualization_config.py
--rw-r--r--   0        0        0      196 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/__init__.py
--rw-r--r--   0        0        0      256 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/__init__.py
--rw-r--r--   0        0        0     9091 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py
--rw-r--r--   0        0        0     7138 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py
--rw-r--r--   0        0        0     2458 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py
--rw-r--r--   0        0        0     9143 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py
--rw-r--r--   0        0        0     8308 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py
--rw-r--r--   0        0        0    14648 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_handler.py
--rw-r--r--   0        0        0      196 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/__init__.py
--rw-r--r--   0        0        0     3409 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py
--rw-r--r--   0        0        0     8168 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py
--rw-r--r--   0        0        0    13949 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py
--rw-r--r--   0        0        0     7839 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py
--rw-r--r--   0        0        0    10838 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py
--rw-r--r--   0        0        0     9355 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py
--rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/__init__.py
--rw-r--r--   0        0        0    14717 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py
--rw-r--r--   0        0        0     9282 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py
--rw-r--r--   0        0        0     4097 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py
--rw-r--r--   0        0        0      501 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/structs.py
--rw-r--r--   0        0        0    11234 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/utils.py
--rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/__init__.py
--rw-r--r--   0        0        0      196 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/__init__.py
--rw-r--r--   0        0        0     2227 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/configuration.py
--rw-r--r--   0        0        0     6836 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/data_classes.py
--rw-r--r--   0        0        0    54147 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/metrics_computation.py
--rw-r--r--   0        0        0    15943 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/metrics_logging.py
--rw-r--r--   0        0        0     4134 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/model_evaluation.py
--rw-r--r--   0        0        0      633 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/structs.py
--rw-r--r--   0        0        0    15700 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/utils.py
--rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/__init__.py
--rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/mlflow/__init__.py
--rw-r--r--   0        0        0     7255 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/mlflow/mlflow_runner.py
--rw-r--r--   0        0        0     1676 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/mlflow/utils.py
--rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/models/__init__.py
--rw-r--r--   0        0        0      257 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/models/constants.py
--rw-r--r--   0        0        0    10705 2024-04-05 08:00:50.581919 mlcvzoo_base-5.7.2/mlcvzoo_base/models/model_registry.py
--rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/models/read_from_file/__init__.py
--rw-r--r--   0        0        0     1540 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/models/read_from_file/configuration.py
--rw-r--r--   0        0        0    10713 2024-04-05 08:00:50.581919 mlcvzoo_base-5.7.2/mlcvzoo_base/models/read_from_file/model.py
--rw-r--r--   0        0        0        0 2024-04-09 09:55:53.034324 mlcvzoo_base-5.7.2/mlcvzoo_base/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 09:55:53.034324 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/__init__.py
--rw-r--r--   0        0        0     1078 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE
--rw-r--r--   0        0        0      138 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/README.md
--rw-r--r--   0        0        0      249 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/__init__.py
--rw-r--r--   0        0        0     1774 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py
--rw-r--r--   0        0        0     1117 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/LICENSE.txt
--rw-r--r--   0        0        0      108 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/README.md
--rw-r--r--   0        0        0      296 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/__init__.py
--rw-r--r--   0        0        0     2794 2024-04-05 08:00:50.581919 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/perspective.py
--rw-r--r--   0        0        0     3744 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE
--rw-r--r--   0        0        0      127 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/README.md
--rw-r--r--   0        0        0      249 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/__init__.py
--rw-r--r--   0        0        0     1649 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py
--rw-r--r--   0        0        0      488 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/__init__.py
--rw-r--r--   0        0        0     4751 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/annotation_utils.py
--rw-r--r--   0        0        0     2353 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/common_utils.py
--rw-r--r--   0        0        0    11836 2024-04-05 08:00:50.581919 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/draw_utils.py
--rw-r--r--   0        0        0     5992 2024-04-05 08:00:50.581919 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/file_utils.py
--rw-r--r--   0        0        0     5852 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/gpu_util.py
--rw-r--r--   0        0        0     3009 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/implicit_path_replacements.py
--rw-r--r--   0        0        0     2435 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/versioning_utils.py
--rw-r--r--   0        0        0     3811 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/xml_utils.py
--rw-r--r--   0        0        0     4025 2024-04-09 09:55:34.725685 mlcvzoo_base-5.7.2/pyproject.toml
--rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 mlcvzoo_base-5.7.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.136516 mlcvzoo_base-5.7.3/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/.editorconfig
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.020512 mlcvzoo_base-5.7.3/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.036512 mlcvzoo_base-5.7.3/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      919 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/.gitlab/issue_templates/Bug.md
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/.gitlab/issue_templates/Implementation.md
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/.gitlab/issue_templates/Refactoring.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.036512 mlcvzoo_base-5.7.3/.gitlab/merge_request_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/.gitlab/merge_request_templates/Default.md
+-rw-rw-rw-   0 root         (0) root         (0)     1853 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     8535 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/CHANGELOG.md
+-rwxrwxrwx   0 root         (0) root         (0)     1528 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    11412 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-05-14 14:05:56.136516 mlcvzoo_base-5.7.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      547 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      276 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.020512 mlcvzoo_base-5.7.3/config/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.036512 mlcvzoo_base-5.7.3/config/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.036512 mlcvzoo_base-5.7.3/config/templates/data_preparation/
+-rw-rw-rw-   0 root         (0) root         (0)      784 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/config/templates/data_preparation/annotation-handler_coco-config-template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      799 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/config/templates/data_preparation/annotation-handler_cvat-config-template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/config/templates/data_preparation/annotation-handler_pascal-voc-config-template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/config/templates/data_preparation/class-mapping_config_template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.036512 mlcvzoo_base-5.7.3/config/templates/evaluation/
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/config/templates/evaluation/mlflow_runner_config_template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.040512 mlcvzoo_base-5.7.3/config/templates/models/
+-rw-rw-rw-   0 root         (0) root         (0)      641 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/config/templates/models/read-from-file.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/config/templates/replacement_config_template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.044512 mlcvzoo_base-5.7.3/documentation/
+-rw-rw-rw-   0 root         (0) root         (0)     6336 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/01_introduction_and_goals.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     3617 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/02_architecture_constraints.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/03_system_scope_and_context.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/04_solution_strategy.adoc
+-rw-rw-rw-   0 root         (0) root         (0)    23262 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/05_building_block_view.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/06_runtime_view.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     5492 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/08_concepts.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     3292 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/09_design_decisions.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/10_quality_scenarios.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     3825 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/11_technical_risks.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     7015 2024-05-14 13:24:42.000000 mlcvzoo_base-5.7.3/documentation/12_tutorial.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/about-arc42.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      547 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/glossary.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.052513 mlcvzoo_base-5.7.3/documentation/images/
+-rw-rw-rw-   0 root         (0) root         (0)   165132 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/01_ml_toolbox_big_picture.png
+-rw-rw-rw-   0 root         (0) root         (0)    59452 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/01_se_big_picture.png
+-rw-rw-rw-   0 root         (0) root         (0)   131875 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/04_se_reference_architecture.jpg
+-rw-rw-rw-   0 root         (0) root         (0)   123984 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/05_crisp-dm.png
+-rw-rw-rw-   0 root         (0) root         (0)     5661 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/05_mlcvzoo-base-package-structure-api.png
+-rw-rw-rw-   0 root         (0) root         (0)    13509 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/05_mlcvzoo-base-package-structure-data-prepartion.png
+-rw-rw-rw-   0 root         (0) root         (0)     6406 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/05_mlcvzoo-base-package-structure-models.png
+-rw-rw-rw-   0 root         (0) root         (0)    16992 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/05_mlcvzoo-base-package-structure.png
+-rw-rw-rw-   0 root         (0) root         (0)   173129 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/05_mlcvzoo-big-picture.jpg
+-rw-rw-rw-   0 root         (0) root         (0)   164928 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/05_mlcvzoo-uml-api-data.png
+-rw-rw-rw-   0 root         (0) root         (0)    32043 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/05_mlcvzoo-uml-api-interfaces.png
+-rw-rw-rw-   0 root         (0) root         (0)    80577 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/05_mlcvzoo-uml-api-model.png
+-rw-rw-rw-   0 root         (0) root         (0)    17381 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/images/05_mlcvzoo-uml-api-net.png
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/documentation/index.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.052513 mlcvzoo_base-5.7.3/mlcvzoo_base/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.052513 mlcvzoo_base-5.7.3/mlcvzoo_base/api/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.060513 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11278 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    26780 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation_class_mapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6558 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/bounding_box.py
+-rw-rw-rw-   0 root         (0) root         (0)    13370 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/box.py
+-rw-rw-rw-   0 root         (0) root         (0)     2734 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/class_identifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/dataset_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3268 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/ocr_perception.py
+-rw-rw-rw-   0 root         (0) root         (0)    12077 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/segmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5029 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    13224 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/api/structs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.060513 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8484 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/annotation_handler_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3942 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/class_mapping_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/config_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/device_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/mlfow_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3103 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/model_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/reduction_mapping_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3889 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/replacement_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/structs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/visualization_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.064513 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.068513 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9091 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     7138 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2458 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     9143 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8308 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    14648 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.068513 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3409 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     8168 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    13949 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     7839 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10859 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     9355 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.072513 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_writer/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_writer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14717 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     9282 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/structs.py
+-rw-rw-rw-   0 root         (0) root         (0)    11234 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.072513 mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.076514 mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6836 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/data_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    54149 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/metrics_computation.py
+-rw-rw-rw-   0 root         (0) root         (0)    15943 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/metrics_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     4134 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/model_evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/structs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15718 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.076514 mlcvzoo_base-5.7.3/mlcvzoo_base/metrics/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/metrics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.076514 mlcvzoo_base-5.7.3/mlcvzoo_base/metrics/mlflow/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/metrics/mlflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7255 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/metrics/mlflow/mlflow_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1676 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/metrics/mlflow/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.076514 mlcvzoo_base-5.7.3/mlcvzoo_base/models/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10707 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/models/model_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.076514 mlcvzoo_base-5.7.3/mlcvzoo_base/models/read_from_file/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/models/read_from_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/models/read_from_file/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    10947 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/models/read_from_file/model.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 14:05:50.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.024512 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.080514 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.080514 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/api/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7101 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/api/test_annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3236 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/api/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5322 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/api/test_bounding_box.py
+-rw-rw-rw-   0 root         (0) root         (0)    10544 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/api/test_box.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/api/test_class_identifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     3414 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/api/test_classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5447 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/api/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/api/test_ocr_perception.py
+-rw-rw-rw-   0 root         (0) root         (0)     6195 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/api/test_segmentation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.084514 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3158 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/configuration/test_model_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/configuration/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.084514 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.088514 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/annotation_parser/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/annotation_parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11720 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/annotation_parser/test_coco_annotation_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     8853 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/annotation_parser/test_cvat_annotation_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     3144 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/annotation_parser/test_label_studio_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    25796 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/annotation_parser/test_mot_annotation_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     9830 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/annotation_parser/test_pascal_voc_annotation_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.088514 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/annotation_writer/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/annotation_writer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6391 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/annotation_writer/test_cvat_annotation_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)    24303 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/test_AnnotationHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    33395 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/test_annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    20542 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/data_preparation/test_annotation_class_mapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.088514 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/evaluation/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.088514 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/evaluation/object_detection/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/evaluation/object_detection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29611 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/evaluation/object_detection/test_od_evaluation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.088514 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/metrics/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/metrics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7466 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/metrics/test_mlflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.092514 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9131 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/models/test_model_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/models/test_read_from_file_classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2050 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/models/test_read_from_file_common.py
+-rw-rw-rw-   0 root         (0) root         (0)    12709 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/models/test_read_from_file_object_detection.py
+-rw-rw-rw-   0 root         (0) root         (0)     6952 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/models/test_read_from_file_segmentation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.092514 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/templates/test_templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2056 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/tests/unit_tests/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.092514 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 14:05:50.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.092514 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/efficientdet_pytorch/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/efficientdet_pytorch/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/efficientdet_pytorch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.092514 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/imutils/
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/imutils/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/imutils/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/imutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2794 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/imutils/perspective.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.096514 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/py_faster_rcnn/
+-rw-rw-rw-   0 root         (0) root         (0)     3744 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/py_faster_rcnn/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/py_faster_rcnn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.096514 mlcvzoo_base-5.7.3/mlcvzoo_base/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4751 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/utils/annotation_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2353 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/utils/common_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12124 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/utils/draw_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5992 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/utils/file_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5852 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/utils/gpu_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3009 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/utils/implicit_path_replacements.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/utils/versioning_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3811 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/mlcvzoo_base/utils/xml_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.132516 mlcvzoo_base-5.7.3/mlcvzoo_base.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-05-14 14:05:55.000000 mlcvzoo_base-5.7.3/mlcvzoo_base.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17084 2024-05-14 14:05:56.000000 mlcvzoo_base-5.7.3/mlcvzoo_base.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 14:05:55.000000 mlcvzoo_base-5.7.3/mlcvzoo_base.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-14 14:05:55.000000 mlcvzoo_base-5.7.3/mlcvzoo_base.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-14 14:05:55.000000 mlcvzoo_base-5.7.3/mlcvzoo_base.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4510 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.100514 mlcvzoo_base-5.7.3/requirements_locked/
+-rw-rw-rw-   0 root         (0) root         (0)     4210 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/requirements_locked/requirements-lock-uv-py310-all.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3445 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/requirements_locked/requirements-lock-uv-py310-without-dev.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.100514 mlcvzoo_base-5.7.3/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)      413 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/scripts/lock-dependencies.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 14:05:56.136516 mlcvzoo_base-5.7.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.100514 mlcvzoo_base-5.7.3/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.100514 mlcvzoo_base-5.7.3/test_data/annotations/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.100514 mlcvzoo_base-5.7.3/test_data/annotations/coco/
+-rw-rw-rw-   0 root         (0) root         (0)     6726 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/test_data/annotations/coco/coco.json
+-rw-rw-rw-   0 root         (0) root         (0)     3828 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/coco/coco_all_attributes.json
+-rw-rw-rw-   0 root         (0) root         (0)     4197 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/coco/coco_alternate.json
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/coco/coco_evaluation.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.100514 mlcvzoo_base-5.7.3/test_data/annotations/csv_annotations/
+-rw-rw-rw-   0 root         (0) root         (0)      386 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/csv_annotations/test-evaluation.csv
+-rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/csv_annotations/test-task_eval.csv
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/csv_annotations/test-task_train.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.104514 mlcvzoo_base-5.7.3/test_data/annotations/cvat/
+-rw-rw-rw-   0 root         (0) root         (0)     5029 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/cvat/cvat-all-attributes.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2479 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/cvat/cvat-for-clean-annotations.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4322 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/cvat/cvat-for-images-annotations.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3568 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/cvat/cvat.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2479 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/cvat/test-cvat-write-annotations_expected.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3974 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/cvat/test-cvat-write-annotations_input.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.028512 mlcvzoo_base-5.7.3/test_data/annotations/label_studio_s3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.104514 mlcvzoo_base-5.7.3/test_data/annotations/label_studio_s3/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)     3082 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/label_studio_s3/dummy_task/cars
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/label_studio_s3/dummy_task/person
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/label_studio_s3/dummy_task/truck
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.108515 mlcvzoo_base-5.7.3/test_data/annotations/label_studio_s3/dummy_task_errors/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/label_studio_s3/dummy_task_errors/error_class_mapping_not_found
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/label_studio_s3/dummy_task_errors/error_forbidden_class
+-rw-rw-rw-   0 root         (0) root         (0)        8 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/label_studio_s3/dummy_task_errors/error_no_json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/label_studio_s3/dummy_task_errors/error_wrong_image_path
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/label_studio_s3/dummy_task_errors/error_wrong_label_studio_format
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.108515 mlcvzoo_base-5.7.3/test_data/annotations/mot/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/mot/custom_labels.txt
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/mot/mot_ground-truth_2015.txt
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/mot/mot_ground-truth_201617.txt
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/mot/mot_ground-truth_2020.txt
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/mot/mot_predictions_2020.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.028512 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.108515 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc/dummy_task/cars.xml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 14:05:50.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc/dummy_task/empty.xml
+-rw-rw-rw-   0 root         (0) root         (0)      716 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc/dummy_task/person.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc/dummy_task/truck.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.112515 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_all_attributes/
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_all_attributes/cars.xml
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_all_attributes/empty.xml
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_all_attributes/person.xml
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_all_attributes/truck.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.028512 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_clean_predictions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.112515 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_clean_predictions/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_clean_predictions/dummy_task/cars.xml
+-rw-rw-rw-   0 root         (0) root         (0)      519 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_clean_predictions/dummy_task/person.xml
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_clean_predictions/dummy_task/truck.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.028512 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_predictions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.112515 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_predictions/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_predictions/dummy_task/cars.xml
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_predictions/dummy_task/empty.xml
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_predictions/dummy_task/person.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_predictions/dummy_task/truck.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.028512 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_read_from_file/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.112515 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_read_from_file/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_read_from_file/dummy_task/3b09afbd59ed52a9b82a92856c0e2e82.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_read_from_file/dummy_task/636ae56768d7733bc65d1b1b543bfb4e.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/test_data/annotations/pascal_voc_read_from_file/dummy_task/6e443ec586208278605e6829dbdf94fd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.112515 mlcvzoo_base-5.7.3/test_data/annotations/test_inference_task/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/test_inference_task/test_object-detection_inference_image.xml
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/annotations/text_recognition_test_label.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.116515 mlcvzoo_base-5.7.3/test_data/checkpoints/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/checkpoints/model.pth
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/checkpoints/model_2.pth
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.028512 mlcvzoo_base-5.7.3/test_data/images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.028512 mlcvzoo_base-5.7.3/test_data/images/classification_test_dataset/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.116515 mlcvzoo_base-5.7.3/test_data/images/classification_test_dataset/class1/
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/images/classification_test_dataset/class1/black_image.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.116515 mlcvzoo_base-5.7.3/test_data/images/classification_test_dataset/class2/
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/images/classification_test_dataset/class2/black_image.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.116515 mlcvzoo_base-5.7.3/test_data/images/classification_test_dataset/class3/
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/images/classification_test_dataset/class3/black_image.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.116515 mlcvzoo_base-5.7.3/test_data/images/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)     3716 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/images/dummy_task/cars.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/images/dummy_task/empty.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/images/dummy_task/person.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/images/dummy_task/truck.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.120515 mlcvzoo_base-5.7.3/test_data/images/test_inference_task/
+-rw-rw-rw-   0 root         (0) root         (0)  2270306 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/images/test_inference_task/test_object-detection_inference_image.jpg
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/images/test_inference_task/test_text-recognition_inference_image.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.124515 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_all_sources_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_alternate_coco_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_coco_all_attributes_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_coco_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_coco_test_multiple_sources.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_cvat_all_attributes_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      333 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_cvat_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_cvat_write_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_generate-darknet_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_label-studio_errors_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_label-studio_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_mot-custom_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_mot-invalid-format_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_mot2015_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_mot201617_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_mot2020_ignore-class-names_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_mot2020_no-gt-data_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_mot2020_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_mot_missing-class_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      333 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_pascal-voc_all_attributes_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_pascal-voc_evaluation.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      614 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_pascal-voc_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-handler_pascal-voc_test_ignore_missing_images.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/annotation-transformer_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/instances_default.json
+-rw-rw-rw-   0 root         (0) root         (0)      808 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_AnnotationHandler/wanted_output_annotation.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.128515 mlcvzoo_base-5.7.3/test_data/test_ClassMapping/
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_ClassMapping/class-mapping_coco.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    61633 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_ClassMapping/class-mapping_imagenet.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      716 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_ClassMapping/class-mapping_mot.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_ClassMapping/class-mapping_test-default-lp.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      728 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_ClassMapping/class-mapping_test-default.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.128515 mlcvzoo_base-5.7.3/test_data/test_ReadFromFileObjectDetectionModel/
+-rw-rw-rw-   0 root         (0) root         (0)      355 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_coco_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_cvat_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_pascal-voc_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      456 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_pascal-voc_test_annotations_only.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.132516 mlcvzoo_base-5.7.3/test_data/test_annotation_class_mapper/
+-rw-rw-rw-   0 root         (0) root         (0)      681 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_annotation_class_mapper/test_annotation_class_not_in_model_classes_error__class-mapping.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_annotation_class_mapper/test_class_id_out_of_range_error__class-mapping.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      952 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_annotation_class_mapper/test_constructor__class-mapping.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_annotation_class_mapper/test_constructor__reduction-mapping.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_annotation_class_mapper/test_duplicate_model_class_id_error__class-mapping.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_annotation_class_mapper/test_duplicate_output_class_id_error__reduction-mapping.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_annotation_class_mapper/test_duplicate_output_class_name_error__reduction-mapping.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      449 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_annotation_class_mapper/test_model_class_id_not_in_model_classes_error__reduction-mapping.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      456 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_annotation_class_mapper/test_model_class_name_not_in_model_classes_error__reduction-mapping.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.132516 mlcvzoo_base-5.7.3/test_data/test_mlflow_runner/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_mlflow_runner/test_mlflow_file_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_mlflow_runner/test_mlflow_postgressql_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.132516 mlcvzoo_base-5.7.3/test_data/test_od_evaluation/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_od_evaluation/test_od_evaluation_model_based_annotation_handler.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      365 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_od_evaluation/test_od_evaluation_with_precomputed.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.132516 mlcvzoo_base-5.7.3/test_data/test_od_evaluation/wanted_metrics/
+-rw-rw-rw-   0 root         (0) root         (0)     2172 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/test_data/test_od_evaluation/wanted_metrics/wanted_metrics-dict_precomputed.json
+-rw-rw-rw-   0 root         (0) root         (0)     3038 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/test_data/test_od_evaluation/wanted_metrics/wanted_metrics-dict_read-from-file_pascal-voc_test.json
+-rw-rw-rw-   0 root         (0) root         (0)     3999 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/test_data/test_video.mp4
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:05:56.132516 mlcvzoo_base-5.7.3/third-party-licenses/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-13 06:25:02.000000 mlcvzoo_base-5.7.3/third-party-licenses/third-party-licenses-complementary.csv
+-rw-rw-rw-   0 root         (0) root         (0)     5468 2024-05-14 06:01:24.000000 mlcvzoo_base-5.7.3/third-party-licenses/third-party-licenses.csv
```

### Comparing `mlcvzoo_base-5.7.2/LICENSE` & `mlcvzoo_base-5.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/README.md` & `mlcvzoo_base-5.7.3/README.md`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/configuration.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_attributes.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation_attributes.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_builder.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_class_mapper.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation_class_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,51 +53,51 @@
         # EXAMPLE:
         # {
         #     0: "person",
         #     1: "truck",
         #     2: "car",
         #     3: "lion",
         # }
-        self.__annotation_class_id_to_model_class_name_map: Dict[
-            int, str
-        ] = self.__create_annotation_class_id_to_model_class_name_map(
-            class_mapping_config=class_mapping,
+        self.__annotation_class_id_to_model_class_name_map: Dict[int, str] = (
+            self.__create_annotation_class_id_to_model_class_name_map(
+                class_mapping_config=class_mapping,
+            )
         )
 
         # Dictionary that defines how a class names during the parsing of annotation files
         # are mapped to a model class IDs.
         #
         # EXAMPLE:
         # {
         #     "person": 0,
         #     "truck": 1,
         #     "car": 2,
         #     "lion": 3,
         # }
-        self.__annotation_class_name_to_model_class_id_map: Dict[
-            str, int
-        ] = self.__create_annotation_class_name_to_model_class_id_map(
-            annotation_class_id_to_model_class_name_map=self.__annotation_class_id_to_model_class_name_map
+        self.__annotation_class_name_to_model_class_id_map: Dict[str, int] = (
+            self.__create_annotation_class_name_to_model_class_id_map(
+                annotation_class_id_to_model_class_name_map=self.__annotation_class_id_to_model_class_name_map
+            )
         )
 
         # Dictionary for mapping annotation class names to model class names. This
         # can be used to fix typos or to aggregate classes to a single model class.
         # The
         #
         # EXAMPLE:
         # {
         #     "Person": "person",
         #     "LKW": "truck",
         #     "tuck": "truck",
         #     "PKW": "car",
         # }
-        self.__annotation_class_name_to_model_class_name_map: Dict[
-            str, str
-        ] = self.__create_annotation_class_name_to_model_class_name_map(
-            class_mapping_config=self.class_mapping_config
+        self.__annotation_class_name_to_model_class_name_map: Dict[str, str] = (
+            self.__create_annotation_class_name_to_model_class_name_map(
+                class_mapping_config=self.class_mapping_config
+            )
         )
 
         # Dictionary for mapping / reducing the model class IDs to an output class identifier.
         # The model class IDs 1 and 2 are reduced to class ID 1 and class name vehicle.
         # The model class ID is used to create multiple outputs.
         #
         # EXAMPLE:
@@ -106,20 +106,20 @@
         #     1: [ClassIdentifier(class_id=1, class_name="vehicle")],
         #     2: [ClassIdentifier(class_id=1, class_name="vehicle")],
         #     3: [
         #         ClassIdentifier(class_id=15, class_name="animal"),
         #         ClassIdentifier(class_id=16, class_name="cat"),
         #     ],
         # }
-        self.__model_class_id_to_class_identifier_map: Dict[
-            int, List[ClassIdentifier]
-        ] = self.__create_model_class_id_to_class_identifier_map(
-            annotation_class_id_to_model_class_name_map=self.__annotation_class_id_to_model_class_name_map,
-            annotation_class_name_to_model_class_id_map=self.__annotation_class_name_to_model_class_id_map,
-            reduction_mapping_config=reduction_mapping,
+        self.__model_class_id_to_class_identifier_map: Dict[int, List[ClassIdentifier]] = (
+            self.__create_model_class_id_to_class_identifier_map(
+                annotation_class_id_to_model_class_name_map=self.__annotation_class_id_to_model_class_name_map,
+                annotation_class_name_to_model_class_id_map=self.__annotation_class_name_to_model_class_id_map,
+                reduction_mapping_config=reduction_mapping,
+            )
         )
 
         # Dictionary for mapping / reducing the model class names to an output class identifier.
         # The model class names "banana" and "cherry" are reduced to class ID 10
         # and class name "fruit".
         #
         # EXAMPLE:
@@ -128,19 +128,19 @@
         #     "banana": [ClassIdentifier(class_id=10, class_name="fruit")],
         #     "cherry": [ClassIdentifier(class_id=10, class_name="fruit")],
         #     "lion": [
         #         ClassIdentifier(class_id=15, class_name="animal"),
         #         ClassIdentifier(class_id=16, class_name="cat"),
         #     ],
         # }
-        self.__model_class_name_to_class_identifier_map: Dict[
-            str, List[ClassIdentifier]
-        ] = self.__create_model_class_name_to_class_identifier_map(
-            annotation_class_id_to_model_class_name_map=self.__annotation_class_id_to_model_class_name_map,
-            model_class_id_to_class_identifier_map=self.__model_class_id_to_class_identifier_map,
+        self.__model_class_name_to_class_identifier_map: Dict[str, List[ClassIdentifier]] = (
+            self.__create_model_class_name_to_class_identifier_map(
+                annotation_class_id_to_model_class_name_map=self.__annotation_class_id_to_model_class_name_map,
+                model_class_id_to_class_identifier_map=self.__model_class_id_to_class_identifier_map,
+            )
         )
 
     @property
     def num_classes(self) -> int:
         """
         Returns the number of classes the AnnotationMapper 'knows'.
```

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_parser.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_writer.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/bounding_box.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/bounding_box.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/box.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/box.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/class_identifier.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/class_identifier.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/classification.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/classification.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/dataset_info.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/dataset_info.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/ocr_perception.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/ocr_perception.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/segmentation.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/data/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         The input format is nx2 =>  [(x, y), (x, y), ...].
         The output will be a numpy array out of 4 polygon-points => 4x2,
         which define the rect around the original polygon
         """
 
         min_area_rect = cv2.minAreaRect(np_polygon.astype(int))
         box = order_points(polygon=cv2.boxPoints(min_area_rect), sort_by_euclidean=False)
-        return np.intp(box).astype(np.float32)  # type: ignore[return-value]
+        return np.intp(box).astype(np.float32)
 
     def copy_segmentation(self, class_identifier: ClassIdentifier) -> Segmentation:
         return Segmentation(
             polygon=self.polygon,
             class_identifier=class_identifier,
             score=self.score,
             difficult=self.difficult,
```

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/exceptions.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/interfaces.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/model.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/api/registry.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/api/registry.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/annotation_handler_config.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/annotation_handler_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,20 +164,20 @@
 
     csv_annotation: Optional[AnnotationHandlerWriteOutputCSVAnnotationConfig] = related.ChildField(
         cls=AnnotationHandlerWriteOutputCSVAnnotationConfig,
         required=False,
         default=None,
     )
 
-    darknet_train_set: Optional[
-        AnnotationHandlerWriteOutputDarknetAnnotationConfig
-    ] = related.ChildField(
-        cls=AnnotationHandlerWriteOutputDarknetAnnotationConfig,
-        required=False,
-        default=None,
+    darknet_train_set: Optional[AnnotationHandlerWriteOutputDarknetAnnotationConfig] = (
+        related.ChildField(
+            cls=AnnotationHandlerWriteOutputDarknetAnnotationConfig,
+            required=False,
+            default=None,
+        )
     )
     darknet_annotation: AnnotationHandlerWriteOutputDarknetAnnotationConfig = related.ChildField(
         cls=AnnotationHandlerWriteOutputDarknetAnnotationConfig,
         required=False,
         default=None,
     )
     use_difficult: bool = related.BooleanField(default=True)
@@ -208,17 +208,17 @@
         AnnotationHandlerSingleFileInputDataConfig, default=[]
     )
 
     cvat_input_data: List[AnnotationHandlerSingleFileInputDataConfig] = related.SequenceField(
         AnnotationHandlerSingleFileInputDataConfig, default=[]
     )
 
-    label_studio_input_data: List[
-        AnnotationHandlerLabelStudioInputDataConfig
-    ] = related.SequenceField(AnnotationHandlerLabelStudioInputDataConfig, default=[])
+    label_studio_input_data: List[AnnotationHandlerLabelStudioInputDataConfig] = (
+        related.SequenceField(AnnotationHandlerLabelStudioInputDataConfig, default=[])
+    )
 
     write_output: Optional[AnnotationHandlerWriteOutputConfig] = related.ChildField(
         AnnotationHandlerWriteOutputConfig, required=False, default=None
     )
 
     reduction_class_mapping: Optional[ReductionMappingConfig] = related.ChildField(
         cls=ReductionMappingConfig, required=False, default=None
```

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/class_mapping_config.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/class_mapping_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/config_registry.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/config_registry.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/device_query.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/device_query.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/mlfow_config.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/mlfow_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/model_config.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/model_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 
 @define
 class ModelConfig(BaseConfigClass):
     __related_strict__ = True
 
     class_type: str = related.StringField()
-    constructor_parameters: Dict[
-        str, Union[int, bool, str, float, List[Any], Dict[str, Any]]
-    ] = related.ChildField(
-        cls=dict,
+    constructor_parameters: Dict[str, Union[int, bool, str, float, List[Any], Dict[str, Any]]] = (
+        related.ChildField(
+            cls=dict,
+        )
     )
 
     def update_class_type(self, args_dict: Dict[str, Optional[str]]) -> None:
         if "class_type" in args_dict and args_dict["class_type"] is not None:
             self.class_type = args_dict["class_type"]
 
     def update_constructor_parameters(
```

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/reduction_mapping_config.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/reduction_mapping_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/replacement_config.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/replacement_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/structs.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/structs.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/utils.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/visualization_config.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/configuration/visualization_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_handler.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_handler.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 image = cv2.imread(image_path)
                 if image is None:
                     logger.warning(
                         "Could not read image from path='%s', annotation will be skipped",
                         image_path,
                     )
                     continue
-                image_shape = image.shape
+                image_shape = (image.shape[0], image.shape[1])
 
                 replacement_string = AnnotationParser.csv_directory_replacement_string.format(
                     dataset_count
                 )
 
                 mot_builder = MOTAnnotationBuilder(
                     image_shape=image_shape,
```

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/utils.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/data_preparation/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/configuration.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/data_classes.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/metrics_computation.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/metrics_computation.py`

 * *Files 1% similar despite different names*

```diff
@@ -841,17 +841,17 @@
         try:
             f1 = 2 * (pr * rc) / (pr + rc)
         except ZeroDivisionError:
             f1 = DEFAULT_FLOAT_VALUE
 
         fn = num_annotations - tp
 
-        self.model_metrics.metrics_dict[iou_thresh][bbox_size_type][
-            str(class_identifier)
-        ] = ODMetrics(TP=tp, FP=fp, FN=fn, PR=pr, RC=rc, F1=f1, AP=ap, COUNT=num_annotations)
+        self.model_metrics.metrics_dict[iou_thresh][bbox_size_type][str(class_identifier)] = (
+            ODMetrics(TP=tp, FP=fp, FN=fn, PR=pr, RC=rc, F1=f1, AP=ap, COUNT=num_annotations)
+        )
 
     def __compute_metrics(self, class_identifier: ClassIdentifier) -> None:
         # TODO: Is this mAP computation? - separate from rest !
         for iou_thresh in self.iou_thresholds:
             for bbox_size_type in BBoxSizeTypes.get_values_as_list(class_type=BBoxSizeTypes):
                 num_annotations = self.computing_data.gt_counter_dict[bbox_size_type][
                     str(class_identifier)
```

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/metrics_logging.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/metrics_logging.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/model_evaluation.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/structs.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/structs.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/utils.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/evaluation/object_detection/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,15 +387,16 @@
                 2,
             )
 
     # Convert to RGB for tensorboard
     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
 
     # resize to the configured image size
-    height, width, _ = img.shape
+    height = img.shape[0]
+    width = img.shape[1]
     scale_factor = false_positive_image_size / width
     img = cv2.resize(
         img,
         (int(width * scale_factor), int(height * scale_factor)),
         interpolation=cv2.INTER_AREA,
     )
```

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/mlflow/mlflow_runner.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/metrics/mlflow/mlflow_runner.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/mlflow/utils.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/metrics/mlflow/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/models/model_registry.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/models/model_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,17 +241,17 @@
 
             if (
                 STRING_REPLACEMENT_MAP_KEY not in model_config.constructor_parameters
                 and STRING_REPLACEMENT_MAP_KEY in init_params
             ):
                 if string_replacement_map is None:
                     string_replacement_map = ReplacementConfig().to_dict()
-                model_config.constructor_parameters[
-                    STRING_REPLACEMENT_MAP_KEY
-                ] = string_replacement_map
+                model_config.constructor_parameters[STRING_REPLACEMENT_MAP_KEY] = (
+                    string_replacement_map
+                )
 
             try:
                 model = model_type(**model_config.constructor_parameters)  # type: ignore[arg-type]
             except TypeError as e:
                 logger.error(
                     "Please provide the parameters " "%s, as specified for %s",
                     init_params,
```

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/models/read_from_file/configuration.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/models/read_from_file/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/models/read_from_file/model.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/models/read_from_file/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,18 @@
     @staticmethod
     def create_image_hash(data_item: Union[str, ImageType]) -> str:
         if isinstance(data_item, str):
             image = cv2.imread(data_item)
         else:
             image = data_item
 
+        # The expected type is 'Buffer' which is comes with
+        # typing extensions >= 4.6.2. For now we don't want to
+        # limit other packages by requiring this version range.
+        # TODO: Add typing extensions >=4.6.2?
         return hashlib.md5(image).hexdigest()
 
     def initialize_annotations_dict(
         self, annotations: List[BaseAnnotation]
     ) -> Dict[str, BaseAnnotation]:
         """
         Create a hashed annotation dictionary from a given list of annotations
```

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE` & `mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/LICENSE.txt` & `mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/imutils/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/perspective.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/imutils/perspective.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE` & `mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/annotation_utils.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/utils/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/common_utils.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/draw_utils.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/utils/draw_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # For details on the licensing terms, see the LICENSE file.
 # SPDX-License-Identifier: OLFL-1.3
 
 """Module for different utility operations regarding drawing on images"""
 
 import colorsys
 import copy
-from typing import List, Optional, Tuple, Union
+from typing import Any, List, Optional, Tuple, Union
 
 import cv2
 import numpy as np
 from PIL import Image, ImageDraw, ImageFont
 
 from mlcvzoo_base.api.data.bounding_box import BoundingBox
 from mlcvzoo_base.api.data.box import Box
@@ -148,15 +148,15 @@
         thickness = (frame.shape[0] + frame.shape[1]) // 450
 
     # TODO: add box.to_tuple(...) ?
     if flip_image:
         # TODO: what to do when image is flipped?
         pass
     else:
-        pts = np.array(polygon, np.int32)
+        pts = np.array(polygon, np.int32)  # type:ignore[var-annotated]
         pts = pts.reshape((-1, 1, 2))
 
         frame = cv2.polylines(
             img=frame, pts=[pts], isClosed=True, color=color, thickness=thickness
         )
 
     # TODO: add caption
@@ -294,27 +294,31 @@
     Returns:
         Numpy array, the given image decorated with annotations
     """
 
     white_color = (255, 255, 255, 15)
 
     if type(image) is np.ndarray:
-        image = Image.fromarray(image)
+        image = Image.fromarray(image)  # type: ignore[no-untyped-call]
 
     assert isinstance(image, Image.Image)
 
-    font = ImageFont.truetype(
+    font = ImageFont.truetype(  # type: ignore[no-untyped-call]
         font=font_path, size=np.floor(0.042 * image.size[1] + 0.1).astype("int32")
     )
 
     draw = ImageDraw.Draw(image)
 
     for bounding_box in bounding_boxes:
         label = "{} {:.2f}".format(bounding_box.class_name, bounding_box.score)
-        label_size = draw.textsize(label, font)
+
+        # the anchor xy can be zero because we are only interested in the necessary
+        # text width and height
+        label_box = draw.textbbox(xy=(0, 0), text=label, font=font)
+        label_size = (label_box[2], label_box[3])
 
         if is_ground_truth:
             text_origin = (
                 float(bounding_box.box.xmin),
                 float(bounding_box.box.ymax - label_size[1]),
             )
         else:
```

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/file_utils.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/gpu_util.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/utils/gpu_util.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/implicit_path_replacements.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/utils/implicit_path_replacements.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/versioning_utils.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/utils/versioning_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/xml_utils.py` & `mlcvzoo_base-5.7.3/mlcvzoo_base/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.2/pyproject.toml` & `mlcvzoo_base-5.7.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,90 @@
-[tool.poetry]
+[project]
 name = "mlcvzoo_base"
 description = "MLCVZoo Base Package"
-version = "5.7.2"
-license = "Open Logistics Foundation License v1.3"
+dynamic = ["version"]
+license = { text = "Open Logistics Foundation License 1.3" }
 readme = "README.md"
-homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
-repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
-documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
 ]
 authors = [
-    "Maximilian Otten <maximilian.otten@iml.fraunhofer.de>",
-    "Christian Hoppe <christian.hoppe@iml.fraunhofer.de>",
-    "Oliver Bredtmann <oliver.bredtmann@dbschenker.com>",
-    "Thilo Bauer <thilo.bauer@dbschenker.com>",
-    "Oliver Urbann <oliver.urbann@iml.fraunhofer.de>",
-    "Jan Basrawi <jan.basrawi@dbschenker.com>",
-    "Luise Weickhmann <luise.weickhmann@iml.fraunhofer.de>",
-    "Luca Kotulla <luca.kotulla@iml.fraunhofer.de>",
+    {name = "Maximilian Otten, email =  <maximilian.otten@iml.fraunhofer.de>"},
+    {name = "Christian Hoppe, email =  <christian.hoppe@iml.fraunhofer.de>"},
+    {name = "Oliver Bredtmann, email =  <oliver.bredtmann@dbschenker.com>"},
+    {name = "Thilo Bauer, email =  <thilo.bauer@dbschenker.com>"},
+    {name = "Oliver Urbann, email =  <oliver.urbann@iml.fraunhofer.de>"},
+    {name = "Jan Basrawi, email =  <jan.basrawi@dbschenker.com>"},
+    {name = "Luise Weickhmann, email =  <luise.weickhmann@iml.fraunhofer.de>"},
+    {name = "Luca Kotulla, email =  <luca.kotulla@iml.fraunhofer.de>"},
 ]
 
-exclude = ["mlcvzoo_base/tests/**/*"]
+requires-python = ">=3.8,<4.0"
+
+dependencies = [
+    "yaml-config-builder>=8, <9",
+    "related-mltoolbox>=1.0, <2.0",
+    "attrs>=20",
+    # numpy 1.19.2 is oldest available on aarch64 but 1.19.5 leads
+    # to unbuildable pytorch there, all is well on amd64
+    "numpy>=1.19.2,!=1.19.5",
+    # above 4.9.0 the signature of some opencv functions change which are incompatible to our code
+    # we restrict both opencv dependencies to keep them on the same version
+    "opencv-python>=4.5,!=4.5.5.64,<4.9.0.0",
+    "opencv-contrib-python>=4.5,!=4.5.5.64,<4.9.0.0",
+    "dataclasses-json>=0.5",
+    "tqdm>=4.61",
+    "imageio>=2.9",
+    "pillow>=8.2",
+    "mlflow>=1.22",
+    "terminaltables>=3.1",
+    "tensorboardX>=2.5",
+    "gitpython>=3"
+]
 
-packages = [
-    { include = "mlcvzoo_base" },
+[project.optional-dependencies]
+dev = [
+    "mock>=4.0",
+    "pytest>=7.0",
+    "pytest-cov>=3.0.0",
+    "black>=22",
+    "mypy>=0.961",
+    "pylint>=2.9.6",
+  # Isort guarantees formatting results for 5.X
+    "isort>=5.0, <6.0",
+    "pytest-mock>=3.7"
 ]
 
+[project.urls]
+homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
+repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
+documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base/-/blob/main/documentation/index.adoc"
 
-[tool.poetry.dependencies]
-python = "^3.8"
+[tool.setuptools.dynamic]
+version = {attr = "mlcvzoo_base.__version__"}
 
-yaml-config-builder = { version = "^8" }
-related-mltoolbox = { version = "^1.0" }
-attrs = { version = ">=20" }
-# numpy 1.19.2 is oldest available on aarch64 but 1.19.5 leads
-# to unbuildable pytorch there, all is well on amd64
-numpy = { version = ">=1.19.2,!=1.19.5" }
-opencv-python = { version = ">=4.5,!=4.5.5.64"}
-opencv-contrib-python = { version = ">=4.5,!=4.5.5.64" }
-dataclasses-json = { version = ">=0.5" }
-tqdm = { version = ">=4.61" }
-imageio = { version = ">=2.9" }
-pillow = { version =  ">=8.2" }
-# TODO: Newer mlflow pulls in llvmlite which is not _just_
-#       installable currently so defer upgrading this for now
-mlflow = { version = ">=1.22" }
-terminaltables = { version = ">=3.1" }
-tensorboardX = { version = ">=2.5" }
-gitpython = { version = ">=3" }
-
-[tool.poetry.dev-dependencies]
-mock = { version = ">=4.0" }
-pytest = { version = ">=7.0" }
-pytest-cov = { version = ">=3.0.0" }
-black = { version = ">=22" }
-mypy = { version = ">=0.961" }
-pylint = { version = ">=2.9.6" }
-# Isort guarantees formatting results for 5.X
-isort = { version = "^5.0" }
-pytest-mock = { version = ">=3.7" }
+[tool.setuptools]
+include-package-data = false
+
+[tool.setuptools.packages.find]
+where = ["."]  # list of folders that contain the packages (["."] by default)
+include = ["mlcvzoo_base*"]  # package names should match these glob patterns (["*"] by default)
+exclude = ["mlcvzoo_base.tests*"]  # exclude packages matching these glob patterns (empty by default)
+namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
-requires = ["setuptools", "poetry_core>=1.0"]
-build-backend = "poetry.core.masonry.api"
+requires = [
+    "setuptools>=42",
+    "wheel",
+    "setuptools_scm[toml]>=3.4"
+]
+build-backend = "setuptools.build_meta"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 line-length = 99
```

