# Comparing `tmp/autotrain-advanced-0.7.92.tar.gz` & `tmp/autotrain-advanced-0.7.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.7.92.tar", last modified: Mon May 13 17:23:43 2024, max compression
+gzip compressed data, was "autotrain-advanced-0.7.93.tar", last modified: Tue May 14 10:44:54 2024, max compression
```

## Comparing `autotrain-advanced-0.7.92.tar` & `autotrain-advanced-0.7.93.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.520470 autotrain-advanced-0.7.92/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.92/LICENSE
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13452 2024-05-13 17:23:43.520470 autotrain-advanced-0.7.92/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2741 2024-05-04 09:15:32.000000 autotrain-advanced-0.7.92/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-13 17:23:43.520470 autotrain-advanced-0.7.92/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.92/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.500471 autotrain-advanced-0.7.92/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.500471 autotrain-advanced-0.7.92/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1450 2024-05-13 17:23:35.000000 autotrain-advanced-0.7.92/src/autotrain/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.500471 autotrain-advanced-0.7.92/src/autotrain/app/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.92/src/autotrain/app/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.92/src/autotrain/app/api_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-13 16:31:05.000000 autotrain-advanced-0.7.92/src/autotrain/app/app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.92/src/autotrain/app/db.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.92/src/autotrain/app/models.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.92/src/autotrain/app/oauth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    18596 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/app/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.500471 autotrain-advanced-0.7.92/src/autotrain/app/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.92/src/autotrain/app/static/logo.png
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.500471 autotrain-advanced-0.7.92/src/autotrain/app/templates/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.92/src/autotrain/app/templates/duplicate.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.92/src/autotrain/app/templates/error.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.92/src/autotrain/app/templates/index.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.92/src/autotrain/app/templates/login.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1594 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.92/src/autotrain/app/training_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17416 2024-05-13 16:38:01.000000 autotrain-advanced-0.7.92/src/autotrain/app/ui_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3220 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.92/src/autotrain/app/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.500471 autotrain-advanced-0.7.92/src/autotrain/backends/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.92/src/autotrain/backends/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/backends/base.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.92/src/autotrain/backends/endpoints.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.92/src/autotrain/backends/local.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.92/src/autotrain/backends/ngc.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.92/src/autotrain/backends/nvcf.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.92/src/autotrain/backends/spaces.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.504471 autotrain-advanced-0.7.92/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.92/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3668 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7711 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_object_detection.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9902 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_seq2seq.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_spacerunner.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7989 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7933 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_text_regression.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7910 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_token_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.92/src/autotrain/cli/run_tools.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/cli/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/commands.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.92/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.92/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.92/src/autotrain/logging.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6051 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.92/src/autotrain/parser.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.504471 autotrain-advanced-0.7.92/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.92/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.92/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.92/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.92/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.504471 autotrain-advanced-0.7.92/src/autotrain/tools/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.92/src/autotrain/tools/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.92/src/autotrain/tools/convert_to_kohya.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.92/src/autotrain/tools/merge_adapter.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.504471 autotrain-advanced-0.7.92/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.504471 autotrain-advanced-0.7.92/src/autotrain/trainers/clm/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/clm/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/clm/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/clm/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/clm/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/clm/train_clm_default.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/clm/train_clm_dpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/clm/train_clm_orpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/clm/train_clm_reward.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/clm/train_clm_sft.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20504 2024-05-09 12:46:57.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/clm/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8195 2024-05-06 12:50:40.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/common.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.504471 autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/train.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/train_xl.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.504471 autotrain-advanced-0.7.92/src/autotrain/trainers/generic/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/generic/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/generic/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/generic/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/generic/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.504471 autotrain-advanced-0.7.92/src/autotrain/trainers/image_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/image_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7406 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/image_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/image_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1824 2024-05-13 09:34:02.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/image_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/image_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.504471 autotrain-advanced-0.7.92/src/autotrain/trainers/object_detection/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/object_detection/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7094 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/object_detection/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/object_detection/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1982 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/object_detection/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7854 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/object_detection/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.504471 autotrain-advanced-0.7.92/src/autotrain/trainers/seq2seq/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/seq2seq/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8817 2024-04-29 09:01:25.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/seq2seq/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/seq2seq/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2424 2024-04-25 05:53:33.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/seq2seq/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/seq2seq/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.504471 autotrain-advanced-0.7.92/src/autotrain/trainers/tabular/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/tabular/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/tabular/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/tabular/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/tabular/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.508471 autotrain-advanced-0.7.92/src/autotrain/trainers/text_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/text_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7647 2024-04-25 05:44:56.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/text_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/text_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1876 2024-04-25 05:53:42.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/text_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/text_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.508471 autotrain-advanced-0.7.92/src/autotrain/trainers/text_regression/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/text_regression/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6928 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/text_regression/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/text_regression/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1875 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/text_regression/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2117 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/text_regression/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.508471 autotrain-advanced-0.7.92/src/autotrain/trainers/token_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/token_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7428 2024-04-25 05:44:07.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/token_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/token_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1877 2024-04-25 05:53:47.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/token_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1675 2024-04-25 05:15:09.000000 autotrain-advanced-0.7.92/src/autotrain/trainers/token_classification/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.92/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.508471 autotrain-advanced-0.7.92/src/autotrain_advanced.egg-info/
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13452 2024-05-13 17:23:43.000000 autotrain-advanced-0.7.92/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4885 2024-05-13 17:23:43.000000 autotrain-advanced-0.7.92/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-13 17:23:43.000000 autotrain-advanced-0.7.92/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-13 17:23:43.000000 autotrain-advanced-0.7.92/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3687 2024-05-13 17:23:43.000000 autotrain-advanced-0.7.92/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-13 17:23:43.000000 autotrain-advanced-0.7.92/src/autotrain_advanced.egg-info/top_level.txt
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 17:23:43.508471 autotrain-advanced-0.7.92/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.92/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.117190 autotrain-advanced-0.7.93/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.93/LICENSE
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13452 2024-05-14 10:44:54.117190 autotrain-advanced-0.7.93/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2741 2024-05-04 09:15:32.000000 autotrain-advanced-0.7.93/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-14 10:44:54.117190 autotrain-advanced-0.7.93/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.93/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.081191 autotrain-advanced-0.7.93/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.085191 autotrain-advanced-0.7.93/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1450 2024-05-14 10:44:37.000000 autotrain-advanced-0.7.93/src/autotrain/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.085191 autotrain-advanced-0.7.93/src/autotrain/app/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.93/src/autotrain/app/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.93/src/autotrain/app/api_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-13 16:31:05.000000 autotrain-advanced-0.7.93/src/autotrain/app/app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.93/src/autotrain/app/db.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.93/src/autotrain/app/models.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.93/src/autotrain/app/oauth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19092 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/app/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.085191 autotrain-advanced-0.7.93/src/autotrain/app/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.93/src/autotrain/app/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.085191 autotrain-advanced-0.7.93/src/autotrain/app/templates/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.93/src/autotrain/app/templates/duplicate.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.93/src/autotrain/app/templates/error.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.93/src/autotrain/app/templates/index.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.93/src/autotrain/app/templates/login.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1594 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.93/src/autotrain/app/training_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17416 2024-05-13 16:38:01.000000 autotrain-advanced-0.7.93/src/autotrain/app/ui_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3220 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.93/src/autotrain/app/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.085191 autotrain-advanced-0.7.93/src/autotrain/backends/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.93/src/autotrain/backends/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/backends/base.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.93/src/autotrain/backends/endpoints.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.93/src/autotrain/backends/local.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.93/src/autotrain/backends/ngc.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.93/src/autotrain/backends/nvcf.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.93/src/autotrain/backends/spaces.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.089191 autotrain-advanced-0.7.93/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.93/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3668 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8313 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_object_detection.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10504 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_seq2seq.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_spacerunner.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8591 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8535 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_text_regression.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8512 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_token_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.93/src/autotrain/cli/run_tools.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/cli/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/commands.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.93/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.93/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.93/src/autotrain/logging.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6407 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/parser.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.089191 autotrain-advanced-0.7.93/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.93/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.93/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.93/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.93/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.089191 autotrain-advanced-0.7.93/src/autotrain/tools/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.93/src/autotrain/tools/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.93/src/autotrain/tools/convert_to_kohya.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.93/src/autotrain/tools/merge_adapter.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.089191 autotrain-advanced-0.7.93/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.093191 autotrain-advanced-0.7.93/src/autotrain/trainers/clm/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/clm/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/clm/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/clm/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/clm/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/clm/train_clm_default.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/clm/train_clm_dpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/clm/train_clm_orpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/clm/train_clm_reward.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/clm/train_clm_sft.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20504 2024-05-09 12:46:57.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/clm/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8195 2024-05-06 12:50:40.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/common.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.093191 autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/train.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/train_xl.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.093191 autotrain-advanced-0.7.93/src/autotrain/trainers/generic/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/generic/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/generic/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/generic/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/generic/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.093191 autotrain-advanced-0.7.93/src/autotrain/trainers/image_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/image_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7497 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/image_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/image_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1985 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/image_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/image_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.093191 autotrain-advanced-0.7.93/src/autotrain/trainers/object_detection/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/object_detection/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7185 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/object_detection/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/object_detection/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2143 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/object_detection/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7854 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/object_detection/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.097190 autotrain-advanced-0.7.93/src/autotrain/trainers/seq2seq/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/seq2seq/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8908 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/seq2seq/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/seq2seq/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/seq2seq/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/seq2seq/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.097190 autotrain-advanced-0.7.93/src/autotrain/trainers/tabular/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/tabular/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/tabular/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/tabular/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/tabular/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.097190 autotrain-advanced-0.7.93/src/autotrain/trainers/text_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/text_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7738 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/text_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/text_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2037 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/text_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/text_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.097190 autotrain-advanced-0.7.93/src/autotrain/trainers/text_regression/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/text_regression/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7019 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/text_regression/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/text_regression/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2036 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/text_regression/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2117 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/text_regression/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.097190 autotrain-advanced-0.7.93/src/autotrain/trainers/token_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/token_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7519 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/token_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/token_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2038 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/token_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1675 2024-04-25 05:15:09.000000 autotrain-advanced-0.7.93/src/autotrain/trainers/token_classification/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.93/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.101190 autotrain-advanced-0.7.93/src/autotrain_advanced.egg-info/
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13452 2024-05-14 10:44:54.000000 autotrain-advanced-0.7.93/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4885 2024-05-14 10:44:54.000000 autotrain-advanced-0.7.93/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-14 10:44:54.000000 autotrain-advanced-0.7.93/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-14 10:44:54.000000 autotrain-advanced-0.7.93/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3687 2024-05-14 10:44:54.000000 autotrain-advanced-0.7.93/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-14 10:44:54.000000 autotrain-advanced-0.7.93/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 10:44:54.101190 autotrain-advanced-0.7.93/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.93/static/logo.png
```

### Comparing `autotrain-advanced-0.7.92/LICENSE` & `autotrain-advanced-0.7.93/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/PKG-INFO` & `autotrain-advanced-0.7.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.92
+Version: 0.7.93
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.7.92/README.md` & `autotrain-advanced-0.7.93/README.md`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/setup.py` & `autotrain-advanced-0.7.93/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/__init__.py` & `autotrain-advanced-0.7.93/src/autotrain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 warnings.filterwarnings("ignore", category=UserWarning, module="peft")
 warnings.filterwarnings("ignore", category=UserWarning, module="accelerate")
 warnings.filterwarnings("ignore", category=UserWarning, module="datasets")
 warnings.filterwarnings("ignore", category=FutureWarning, module="accelerate")
 
 
 logger = Logger().get_logger()
-__version__ = "0.7.92"
+__version__ = "0.7.93"
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/api_routes.py` & `autotrain-advanced-0.7.93/src/autotrain/app/api_routes.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/app.py` & `autotrain-advanced-0.7.93/src/autotrain/app/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/db.py` & `autotrain-advanced-0.7.93/src/autotrain/app/db.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/models.py` & `autotrain-advanced-0.7.93/src/autotrain/app/models.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/oauth.py` & `autotrain-advanced-0.7.93/src/autotrain/app/oauth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/params.py` & `autotrain-advanced-0.7.93/src/autotrain/app/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     "log",
     "image_column",
     "target_column",
     "id_column",
     "target_columns",
     "tokens_column",
     "tags_column",
+    "objects_column",
 ]
 
 
 PARAMS = {}
 PARAMS["llm"] = LLMTrainingParams(
     target_modules="all-linear",
     log="tensorboard",
@@ -405,50 +406,58 @@
             "weight_decay",
             "max_grad_norm",
             "seed",
             "logging_steps",
             "auto_find_batch_size",
             "save_total_limit",
             "evaluation_strategy",
+            "early_stopping_patience",
+            "early_stopping_threshold",
         ]
         task_params = {k: v for k, v in task_params.items() if k not in more_hidden_params}
     if task == "text-regression" and param_type == "basic":
         more_hidden_params = [
             "warmup_ratio",
             "weight_decay",
             "max_grad_norm",
             "seed",
             "logging_steps",
             "auto_find_batch_size",
             "save_total_limit",
             "evaluation_strategy",
+            "early_stopping_patience",
+            "early_stopping_threshold",
         ]
         task_params = {k: v for k, v in task_params.items() if k not in more_hidden_params}
     if task == "image-classification" and param_type == "basic":
         more_hidden_params = [
             "warmup_ratio",
             "weight_decay",
             "max_grad_norm",
             "seed",
             "logging_steps",
             "auto_find_batch_size",
             "save_total_limit",
             "evaluation_strategy",
+            "early_stopping_patience",
+            "early_stopping_threshold",
         ]
         task_params = {k: v for k, v in task_params.items() if k not in more_hidden_params}
     if task == "image-object-detection" and param_type == "basic":
         more_hidden_params = [
             "warmup_ratio",
             "weight_decay",
             "max_grad_norm",
             "seed",
             "logging_steps",
             "auto_find_batch_size",
             "save_total_limit",
             "evaluation_strategy",
+            "early_stopping_patience",
+            "early_stopping_threshold",
         ]
         task_params = {k: v for k, v in task_params.items() if k not in more_hidden_params}
     if task == "seq2seq" and param_type == "basic":
         more_hidden_params = [
             "warmup_ratio",
             "weight_decay",
             "max_grad_norm",
@@ -458,26 +467,30 @@
             "save_total_limit",
             "evaluation_strategy",
             "quantization",
             "lora_r",
             "lora_alpha",
             "lora_dropout",
             "target_modules",
+            "early_stopping_patience",
+            "early_stopping_threshold",
         ]
         task_params = {k: v for k, v in task_params.items() if k not in more_hidden_params}
     if task == "token-classification" and param_type == "basic":
         more_hidden_params = [
             "warmup_ratio",
             "weight_decay",
             "max_grad_norm",
             "seed",
             "logging_steps",
             "auto_find_batch_size",
             "save_total_limit",
             "evaluation_strategy",
+            "early_stopping_patience",
+            "early_stopping_threshold",
         ]
         task_params = {k: v for k, v in task_params.items() if k not in more_hidden_params}
     if task == "dreambooth":
         more_hidden_params = [
             "epochs",
             "logging",
             "bf16",
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/static/logo.png` & `autotrain-advanced-0.7.93/src/autotrain/app/static/logo.png`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/templates/duplicate.html` & `autotrain-advanced-0.7.93/src/autotrain/app/templates/duplicate.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/templates/error.html` & `autotrain-advanced-0.7.93/src/autotrain/app/templates/error.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/templates/index.html` & `autotrain-advanced-0.7.93/src/autotrain/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/templates/login.html` & `autotrain-advanced-0.7.93/src/autotrain/app/templates/login.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/training_api.py` & `autotrain-advanced-0.7.93/src/autotrain/app/training_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/ui_routes.py` & `autotrain-advanced-0.7.93/src/autotrain/app/ui_routes.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/app/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/app/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/backends/base.py` & `autotrain-advanced-0.7.93/src/autotrain/backends/base.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/backends/endpoints.py` & `autotrain-advanced-0.7.93/src/autotrain/backends/endpoints.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/backends/ngc.py` & `autotrain-advanced-0.7.93/src/autotrain/backends/ngc.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/backends/nvcf.py` & `autotrain-advanced-0.7.93/src/autotrain/backends/nvcf.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/backends/spaces.py` & `autotrain-advanced-0.7.93/src/autotrain/backends/spaces.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_api.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_image_classification.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_image_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,28 @@
                 "arg": "--mixed-precision",
                 "help": "Choose the precision mode for training to optimize performance and memory usage. Options are 'fp16', 'bf16', or None for default precision. Default is None.",
                 "required": False,
                 "type": str,
                 "default": None,
                 "choices": ["fp16", "bf16", None],
             },
+            {
+                "arg": "--early-stopping-patience",
+                "help": "Specify the number of epochs with no improvement after which training will stop. Default is 5.",
+                "required": False,
+                "type": int,
+                "default": 5,
+            },
+            {
+                "arg": "--early-stopping-threshold",
+                "help": "Define the minimum change in the monitored metric to qualify as an improvement. Default is 0.01.",
+                "required": False,
+                "type": float,
+                "default": 0.01,
+            },
         ]
         arg_list = common_args() + arg_list
         run_image_classification_parser = parser.add_parser(
             "image-classification", description="✨ Run AutoTrain Image Classification"
         )
         for arg in arg_list:
             if "action" in arg:
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_object_detection.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_object_detection.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_seq2seq.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_seq2seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,28 @@
             {
                 "arg": "--target-modules",
                 "help": "List the modules within the model architecture that should be targeted for specific techniques such as LoRA adaptations. Useful for fine-tuning particular components of large models. By default all linear layers are targeted.",
                 "required": False,
                 "type": str,
                 "default": "all-linear",
             },
+            {
+                "arg": "--early-stopping-patience",
+                "help": "Specify the number of epochs with no improvement after which training will stop. Default is 5.",
+                "required": False,
+                "type": int,
+                "default": 5,
+            },
+            {
+                "arg": "--early-stopping-threshold",
+                "help": "Define the minimum change in the monitored metric to qualify as an improvement. Default is 0.01.",
+                "required": False,
+                "type": float,
+                "default": 0.01,
+            },
         ]
         arg_list = common_args() + arg_list
         run_seq2seq_parser = parser.add_parser("seq2seq", description="✨ Run AutoTrain Seq2Seq")
         for arg in arg_list:
             if "action" in arg:
                 run_seq2seq_parser.add_argument(
                     arg["arg"],
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_spacerunner.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_spacerunner.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_tabular.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_text_classification.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_text_classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,14 +104,28 @@
                 "arg": "--mixed-precision",
                 "help": "Choose the precision mode for training to optimize performance and memory usage. Options are 'fp16', 'bf16', or None for default precision. Default is None.",
                 "required": False,
                 "type": str,
                 "default": None,
                 "choices": ["fp16", "bf16", None],
             },
+            {
+                "arg": "--early-stopping-patience",
+                "help": "Specify the number of epochs with no improvement after which training will stop. Default is 5.",
+                "required": False,
+                "type": int,
+                "default": 5,
+            },
+            {
+                "arg": "--early-stopping-threshold",
+                "help": "Define the minimum change in the monitored metric to qualify as an improvement. Default is 0.01.",
+                "required": False,
+                "type": float,
+                "default": 0.01,
+            },
         ]
         arg_list = common_args() + arg_list
         arg_list = [arg for arg in arg_list if arg["arg"] != "--disable-gradient-checkpointing"]
         run_text_classification_parser = parser.add_parser(
             "text-classification", description="✨ Run AutoTrain Text Classification"
         )
         for arg in arg_list:
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_text_regression.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_text_regression.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,14 +104,28 @@
                 "arg": "--mixed-precision",
                 "help": "Choose the precision mode for training to optimize performance and memory usage. Options are 'fp16', 'bf16', or None for default precision. Default is None.",
                 "required": False,
                 "type": str,
                 "default": None,
                 "choices": ["fp16", "bf16", None],
             },
+            {
+                "arg": "--early-stopping-patience",
+                "help": "Specify the number of epochs with no improvement after which training will stop. Default is 5.",
+                "required": False,
+                "type": int,
+                "default": 5,
+            },
+            {
+                "arg": "--early-stopping-threshold",
+                "help": "Define the minimum change in the monitored metric to qualify as an improvement. Default is 0.01.",
+                "required": False,
+                "type": float,
+                "default": 0.01,
+            },
         ]
         arg_list = common_args() + arg_list
         arg_list = [arg for arg in arg_list if arg["arg"] != "--disable-gradient-checkpointing"]
         run_text_regression_parser = parser.add_parser(
             "text-regression", description="✨ Run AutoTrain Text Regression"
         )
         for arg in arg_list:
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_token_classification.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_token_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,28 @@
                 "arg": "--mixed-precision",
                 "help": "Choose the precision mode for training to optimize performance and memory usage. Options are 'fp16', 'bf16', or None for default precision. Default is None.",
                 "required": False,
                 "type": str,
                 "default": None,
                 "choices": ["fp16", "bf16", None],
             },
+            {
+                "arg": "--early-stopping-patience",
+                "help": "Specify the number of epochs with no improvement after which training will stop. Default is 5.",
+                "required": False,
+                "type": int,
+                "default": 5,
+            },
+            {
+                "arg": "--early-stopping-threshold",
+                "help": "Define the minimum change in the monitored metric to qualify as an improvement. Default is 0.01.",
+                "required": False,
+                "type": float,
+                "default": 0.01,
+            },
         ]
         arg_list = common_args() + arg_list
         arg_list = [arg for arg in arg_list if arg["arg"] != "--disable-gradient-checkpointing"]
         run_token_classification_parser = parser.add_parser(
             "token-classification", description="✨ Run AutoTrain Token Classification"
         )
         for arg in arg_list:
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/run_tools.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/run_tools.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/cli/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/cli/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/commands.py` & `autotrain-advanced-0.7.93/src/autotrain/commands.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/dataset.py` & `autotrain-advanced-0.7.93/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/help.py` & `autotrain-advanced-0.7.93/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/logging.py` & `autotrain-advanced-0.7.93/src/autotrain/logging.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/parser.py` & `autotrain-advanced-0.7.93/src/autotrain/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 import requests
 import yaml
 
 from autotrain import logger
 from autotrain.cli.utils import (
     dreambooth_munge_data,
     img_clf_munge_data,
+    img_obj_detect_munge_data,
     llm_munge_data,
     seq2seq_munge_data,
     tabular_munge_data,
     text_clf_munge_data,
     text_reg_munge_data,
     token_clf_munge_data,
 )
 from autotrain.project import AutoTrainProject
 from autotrain.tasks import TASKS
 from autotrain.trainers.clm.params import LLMTrainingParams
 from autotrain.trainers.dreambooth.params import DreamBoothTrainingParams
 from autotrain.trainers.image_classification.params import ImageClassificationParams
+from autotrain.trainers.object_detection.params import ObjectDetectionParams
 from autotrain.trainers.seq2seq.params import Seq2SeqParams
 from autotrain.trainers.tabular.params import TabularParams
 from autotrain.trainers.text_classification.params import TextClassificationParams
 from autotrain.trainers.text_regression.params import TextRegressionParams
 from autotrain.trainers.token_classification.params import TokenClassificationParams
 
 
@@ -43,27 +45,29 @@
                 self.config = yaml.safe_load(f)
 
         self.task_param_map = {
             "lm_training": LLMTrainingParams,
             "dreambooth": DreamBoothTrainingParams,
             "image_binary_classification": ImageClassificationParams,
             "image_multi_class_classification": ImageClassificationParams,
+            "image_object_detection": ObjectDetectionParams,
             "seq2seq": Seq2SeqParams,
             "tabular": TabularParams,
             "text_binary_classification": TextClassificationParams,
             "text_multi_class_classification": TextClassificationParams,
             "text_single_column_regression": TextRegressionParams,
             "text_token_classification": TokenClassificationParams,
         }
         self.munge_data_map = {
             "lm_training": llm_munge_data,
             "dreambooth": dreambooth_munge_data,
             "tabular": tabular_munge_data,
             "seq2seq": seq2seq_munge_data,
             "image_multi_class_classification": img_clf_munge_data,
+            "image_object_detection": img_obj_detect_munge_data,
             "text_multi_class_classification": text_clf_munge_data,
             "text_token_classification": token_clf_munge_data,
             "text_single_column_regression": text_reg_munge_data,
         }
         self.task_aliases = {
             "llm": "lm_training",
             "llm_training": "lm_training",
@@ -74,14 +78,16 @@
             "seq2seq": "seq2seq",
             "tabular": "tabular",
             "text_binary_classification": "text_multi_class_classification",
             "text_classification": "text_multi_class_classification",
             "text_single_column_regression": "text_single_column_regression",
             "text_regression": "text_single_column_regression",
             "token_classification": "text_token_classification",
+            "image_object_detection": "image_object_detection",
+            "object_detection": "image_object_detection",
         }
         task = self.config.get("task")
         self.task = self.task_aliases.get(task, task)
         if self.task is None:
             raise ValueError("Task is required in the configuration file")
         if self.task not in TASKS:
             raise ValueError(f"Task `{self.task}` is not supported")
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.7.93/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.7.93/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.7.93/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.7.93/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/project.py` & `autotrain-advanced-0.7.93/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/tasks.py` & `autotrain-advanced-0.7.93/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/tools/convert_to_kohya.py` & `autotrain-advanced-0.7.93/src/autotrain/tools/convert_to_kohya.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/tools/merge_adapter.py` & `autotrain-advanced-0.7.93/src/autotrain/tools/merge_adapter.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/clm/__main__.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/clm/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/clm/callbacks.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/clm/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/clm/params.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/clm/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/clm/train_clm_default.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/clm/train_clm_default.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/clm/train_clm_dpo.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/clm/train_clm_dpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/clm/train_clm_orpo.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/clm/train_clm_orpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/clm/train_clm_reward.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/clm/train_clm_reward.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/clm/train_clm_sft.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/clm/train_clm_sft.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/clm/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/clm/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/common.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/common.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/__main__.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/train.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/train.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/train_xl.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/train_xl.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/dreambooth/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/generic/__main__.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/generic/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/generic/params.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/generic/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/generic/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/generic/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/image_classification/__main__.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/image_classification/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,18 @@
 
     if config.mixed_precision == "fp16":
         training_args["fp16"] = True
     if config.mixed_precision == "bf16":
         training_args["bf16"] = True
 
     if config.valid_split is not None:
-        early_stop = EarlyStoppingCallback(early_stopping_patience=3, early_stopping_threshold=0.01)
+        early_stop = EarlyStoppingCallback(
+            early_stopping_patience=config.early_stopping_patience,
+            early_stopping_threshold=config.early_stopping_threshold,
+        )
         callbacks_to_use = [early_stop]
     else:
         callbacks_to_use = []
 
     callbacks_to_use.extend([UploadLogs(config=config), LossLoggingCallback(), TrainStartCallback()])
 
     args = TrainingArguments(**training_args)
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/image_classification/dataset.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/image_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/image_classification/params.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/token_classification/params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from typing import Optional
 
 from pydantic import Field
 
 from autotrain.trainers.common import AutoTrainParams
 
 
-class ImageClassificationParams(AutoTrainParams):
+class TokenClassificationParams(AutoTrainParams):
     data_path: str = Field(None, title="Data path")
-    model: str = Field("google/vit-base-patch16-224", title="Model name")
-    username: Optional[str] = Field(None, title="Hugging Face Username")
+    model: str = Field("bert-base-uncased", title="Model name")
     lr: float = Field(5e-5, title="Learning rate")
     epochs: int = Field(3, title="Number of training epochs")
+    max_seq_length: int = Field(128, title="Max sequence length")
     batch_size: int = Field(8, title="Training batch size")
     warmup_ratio: float = Field(0.1, title="Warmup proportion")
     gradient_accumulation: int = Field(1, title="Gradient accumulation steps")
     optimizer: str = Field("adamw_torch", title="Optimizer")
     scheduler: str = Field("linear", title="Scheduler")
     weight_decay: float = Field(0.0, title="Weight decay")
     max_grad_norm: float = Field(1.0, title="Max gradient norm")
     seed: int = Field(42, title="Seed")
     train_split: str = Field("train", title="Train split")
     valid_split: Optional[str] = Field(None, title="Validation split")
+    tokens_column: str = Field("tokens", title="Tokens column")
+    tags_column: str = Field("tags", title="Tags column")
     logging_steps: int = Field(-1, title="Logging steps")
     project_name: str = Field("project-name", title="Output directory")
     auto_find_batch_size: bool = Field(False, title="Auto find batch size")
     mixed_precision: Optional[str] = Field(None, title="fp16, bf16, or None")
     save_total_limit: int = Field(1, title="Save total limit")
     token: Optional[str] = Field(None, title="Hub Token")
     push_to_hub: bool = Field(False, title="Push to hub")
     evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
-    image_column: str = Field("image", title="Image column")
-    target_column: str = Field("target", title="Target column")
+    username: Optional[str] = Field(None, title="Hugging Face Username")
     log: str = Field("none", title="Logging using experiment tracking")
+    early_stopping_patience: int = Field(5, title="Early stopping patience")
+    early_stopping_threshold: float = Field(0.01, title="Early stopping threshold")
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/image_classification/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/image_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/object_detection/__main__.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/object_detection/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,15 +144,18 @@
     if config.mixed_precision == "fp16":
         training_args["fp16"] = True
     if config.mixed_precision == "bf16":
         training_args["bf16"] = True
 
     if config.valid_split is not None:
         training_args["eval_do_concat_batches"] = False
-        early_stop = EarlyStoppingCallback(early_stopping_patience=3, early_stopping_threshold=0.01)
+        early_stop = EarlyStoppingCallback(
+            early_stopping_patience=config.early_stopping_patience,
+            early_stopping_threshold=config.early_stopping_threshold,
+        )
         callbacks_to_use = [early_stop]
     else:
         callbacks_to_use = []
 
     callbacks_to_use.extend([UploadLogs(config=config), LossLoggingCallback(), TrainStartCallback()])
 
     _compute_metrics_fn = partial(
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/object_detection/dataset.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/object_detection/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/object_detection/params.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/object_detection/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,7 +31,9 @@
     evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
     image_column: str = Field("image", title="Image column")
     objects_column: str = Field("objects", title="Target column")
     log: str = Field("none", title="Logging using experiment tracking")
     image_square_size: Optional[int] = Field(
         600, title="Image longest size will be resized to this value, then image will be padded to square."
     )
+    early_stopping_patience: int = Field(5, title="Early stopping patience")
+    early_stopping_threshold: float = Field(0.01, title="Early stopping threshold")
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/object_detection/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/seq2seq/__main__.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/seq2seq/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,18 @@
 
     if config.mixed_precision == "fp16":
         training_args["fp16"] = True
     if config.mixed_precision == "bf16":
         training_args["bf16"] = True
 
     if config.valid_split is not None:
-        early_stop = EarlyStoppingCallback(early_stopping_patience=3, early_stopping_threshold=0.01)
+        early_stop = EarlyStoppingCallback(
+            early_stopping_patience=config.early_stopping_patience,
+            early_stopping_threshold=config.early_stopping_threshold,
+        )
         callbacks_to_use = [early_stop]
     else:
         callbacks_to_use = []
 
     callbacks_to_use.extend([UploadLogs(config=config), LossLoggingCallback(), TrainStartCallback()])
 
     args = Seq2SeqTrainingArguments(**training_args)
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/seq2seq/dataset.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/seq2seq/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/seq2seq/params.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/image_classification/params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 from typing import Optional
 
 from pydantic import Field
 
 from autotrain.trainers.common import AutoTrainParams
 
 
-class Seq2SeqParams(AutoTrainParams):
+class ImageClassificationParams(AutoTrainParams):
     data_path: str = Field(None, title="Data path")
-    model: str = Field("google/flan-t5-base", title="Model name")
+    model: str = Field("google/vit-base-patch16-224", title="Model name")
     username: Optional[str] = Field(None, title="Hugging Face Username")
-    seed: int = Field(42, title="Seed")
-    train_split: str = Field("train", title="Train split")
-    valid_split: Optional[str] = Field(None, title="Validation split")
-    project_name: str = Field("project-name", title="Output directory")
-    token: Optional[str] = Field(None, title="Hub Token")
-    push_to_hub: bool = Field(False, title="Push to hub")
-    text_column: str = Field("text", title="Text column")
-    target_column: str = Field("target", title="Target text column")
     lr: float = Field(5e-5, title="Learning rate")
     epochs: int = Field(3, title="Number of training epochs")
-    max_seq_length: int = Field(128, title="Max sequence length")
-    max_target_length: int = Field(128, title="Max target sequence length")
-    batch_size: int = Field(2, title="Training batch size")
+    batch_size: int = Field(8, title="Training batch size")
     warmup_ratio: float = Field(0.1, title="Warmup proportion")
     gradient_accumulation: int = Field(1, title="Gradient accumulation steps")
     optimizer: str = Field("adamw_torch", title="Optimizer")
     scheduler: str = Field("linear", title="Scheduler")
     weight_decay: float = Field(0.0, title="Weight decay")
     max_grad_norm: float = Field(1.0, title="Max gradient norm")
+    seed: int = Field(42, title="Seed")
+    train_split: str = Field("train", title="Train split")
+    valid_split: Optional[str] = Field(None, title="Validation split")
     logging_steps: int = Field(-1, title="Logging steps")
-    evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
+    project_name: str = Field("project-name", title="Output directory")
     auto_find_batch_size: bool = Field(False, title="Auto find batch size")
     mixed_precision: Optional[str] = Field(None, title="fp16, bf16, or None")
     save_total_limit: int = Field(1, title="Save total limit")
     token: Optional[str] = Field(None, title="Hub Token")
     push_to_hub: bool = Field(False, title="Push to hub")
-    peft: bool = Field(False, title="Use PEFT")
-    quantization: Optional[str] = Field("int4", title="int4, int8, or None")
-    lora_r: int = Field(16, title="LoRA-R")
-    lora_alpha: int = Field(32, title="LoRA-Alpha")
-    lora_dropout: float = Field(0.05, title="LoRA-Dropout")
-    target_modules: str = Field("all-linear", title="Target modules for PEFT")
+    evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
+    image_column: str = Field("image", title="Image column")
+    target_column: str = Field("target", title="Target column")
     log: str = Field("none", title="Logging using experiment tracking")
+    early_stopping_patience: int = Field(5, title="Early stopping patience")
+    early_stopping_threshold: float = Field(0.01, title="Early stopping threshold")
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/seq2seq/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/seq2seq/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/tabular/__main__.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/tabular/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/tabular/params.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/tabular/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/tabular/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/text_classification/__main__.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/text_classification/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,15 +149,18 @@
 
     if config.mixed_precision == "fp16":
         training_args["fp16"] = True
     if config.mixed_precision == "bf16":
         training_args["bf16"] = True
 
     if config.valid_split is not None:
-        early_stop = EarlyStoppingCallback(early_stopping_patience=3, early_stopping_threshold=0.01)
+        early_stop = EarlyStoppingCallback(
+            early_stopping_patience=config.early_stopping_patience,
+            early_stopping_threshold=config.early_stopping_threshold,
+        )
         callbacks_to_use = [early_stop]
     else:
         callbacks_to_use = []
 
     callbacks_to_use.extend([UploadLogs(config=config), LossLoggingCallback(), TrainStartCallback()])
 
     args = TrainingArguments(**training_args)
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/text_classification/dataset.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/text_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/text_classification/params.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/text_classification/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,7 +29,9 @@
     mixed_precision: Optional[str] = Field(None, title="fp16, bf16, or None")
     save_total_limit: int = Field(1, title="Save total limit")
     token: Optional[str] = Field(None, title="Hub Token")
     push_to_hub: bool = Field(False, title="Push to hub")
     evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
     username: Optional[str] = Field(None, title="Hugging Face Username")
     log: str = Field("none", title="Logging using experiment tracking")
+    early_stopping_patience: int = Field(5, title="Early stopping patience")
+    early_stopping_threshold: float = Field(0.01, title="Early stopping threshold")
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/text_classification/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/text_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/text_regression/__main__.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/text_regression/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,18 @@
 
     if config.mixed_precision == "fp16":
         training_args["fp16"] = True
     if config.mixed_precision == "bf16":
         training_args["bf16"] = True
 
     if config.valid_split is not None:
-        early_stop = EarlyStoppingCallback(early_stopping_patience=3, early_stopping_threshold=0.01)
+        early_stop = EarlyStoppingCallback(
+            early_stopping_patience=config.early_stopping_patience,
+            early_stopping_threshold=config.early_stopping_threshold,
+        )
         callbacks_to_use = [early_stop]
     else:
         callbacks_to_use = []
 
     callbacks_to_use.extend([UploadLogs(config=config), LossLoggingCallback(), TrainStartCallback()])
 
     args = TrainingArguments(**training_args)
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/text_regression/dataset.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/text_regression/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/text_regression/params.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/text_regression/params.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,7 +29,9 @@
     mixed_precision: Optional[str] = Field(None, title="fp16, bf16, or None")
     save_total_limit: int = Field(1, title="Save total limit")
     token: Optional[str] = Field(None, title="Hub Token")
     push_to_hub: bool = Field(False, title="Push to hub")
     evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
     username: Optional[str] = Field(None, title="Hugging Face Username")
     log: str = Field("none", title="Logging using experiment tracking")
+    early_stopping_patience: int = Field(5, title="Early stopping patience")
+    early_stopping_threshold: float = Field(0.01, title="Early stopping threshold")
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/text_regression/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/text_regression/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/token_classification/__main__.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/token_classification/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,18 @@
 
     if config.mixed_precision == "fp16":
         training_args["fp16"] = True
     if config.mixed_precision == "bf16":
         training_args["bf16"] = True
 
     if config.valid_split is not None:
-        early_stop = EarlyStoppingCallback(early_stopping_patience=3, early_stopping_threshold=0.01)
+        early_stop = EarlyStoppingCallback(
+            early_stopping_patience=config.early_stopping_patience,
+            early_stopping_threshold=config.early_stopping_threshold,
+        )
         callbacks_to_use = [early_stop]
     else:
         callbacks_to_use = []
 
     callbacks_to_use.extend([UploadLogs(config=config), LossLoggingCallback(), TrainStartCallback()])
 
     args = TrainingArguments(**training_args)
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/token_classification/dataset.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/token_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/token_classification/params.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/seq2seq/params.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 from typing import Optional
 
 from pydantic import Field
 
 from autotrain.trainers.common import AutoTrainParams
 
 
-class TokenClassificationParams(AutoTrainParams):
+class Seq2SeqParams(AutoTrainParams):
     data_path: str = Field(None, title="Data path")
-    model: str = Field("bert-base-uncased", title="Model name")
+    model: str = Field("google/flan-t5-base", title="Model name")
+    username: Optional[str] = Field(None, title="Hugging Face Username")
+    seed: int = Field(42, title="Seed")
+    train_split: str = Field("train", title="Train split")
+    valid_split: Optional[str] = Field(None, title="Validation split")
+    project_name: str = Field("project-name", title="Output directory")
+    token: Optional[str] = Field(None, title="Hub Token")
+    push_to_hub: bool = Field(False, title="Push to hub")
+    text_column: str = Field("text", title="Text column")
+    target_column: str = Field("target", title="Target text column")
     lr: float = Field(5e-5, title="Learning rate")
     epochs: int = Field(3, title="Number of training epochs")
     max_seq_length: int = Field(128, title="Max sequence length")
-    batch_size: int = Field(8, title="Training batch size")
+    max_target_length: int = Field(128, title="Max target sequence length")
+    batch_size: int = Field(2, title="Training batch size")
     warmup_ratio: float = Field(0.1, title="Warmup proportion")
     gradient_accumulation: int = Field(1, title="Gradient accumulation steps")
     optimizer: str = Field("adamw_torch", title="Optimizer")
     scheduler: str = Field("linear", title="Scheduler")
     weight_decay: float = Field(0.0, title="Weight decay")
     max_grad_norm: float = Field(1.0, title="Max gradient norm")
-    seed: int = Field(42, title="Seed")
-    train_split: str = Field("train", title="Train split")
-    valid_split: Optional[str] = Field(None, title="Validation split")
-    tokens_column: str = Field("tokens", title="Tokens column")
-    tags_column: str = Field("tags", title="Tags column")
     logging_steps: int = Field(-1, title="Logging steps")
-    project_name: str = Field("project-name", title="Output directory")
+    evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
     auto_find_batch_size: bool = Field(False, title="Auto find batch size")
     mixed_precision: Optional[str] = Field(None, title="fp16, bf16, or None")
     save_total_limit: int = Field(1, title="Save total limit")
     token: Optional[str] = Field(None, title="Hub Token")
     push_to_hub: bool = Field(False, title="Push to hub")
-    evaluation_strategy: str = Field("epoch", title="Evaluation strategy")
-    username: Optional[str] = Field(None, title="Hugging Face Username")
+    peft: bool = Field(False, title="Use PEFT")
+    quantization: Optional[str] = Field("int4", title="int4, int8, or None")
+    lora_r: int = Field(16, title="LoRA-R")
+    lora_alpha: int = Field(32, title="LoRA-Alpha")
+    lora_dropout: float = Field(0.05, title="LoRA-Dropout")
+    target_modules: str = Field("all-linear", title="Target modules for PEFT")
     log: str = Field("none", title="Logging using experiment tracking")
+    early_stopping_patience: int = Field(5, title="Early stopping patience")
+    early_stopping_threshold: float = Field(0.01, title="Early stopping threshold")
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain/trainers/token_classification/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/trainers/token_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain/utils.py` & `autotrain-advanced-0.7.93/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.7.93/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.92
+Version: 0.7.93
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.7.92/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.7.93/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.7.93/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.92/static/logo.png` & `autotrain-advanced-0.7.93/static/logo.png`

 * *Files identical despite different names*

