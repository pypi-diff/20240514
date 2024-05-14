# Comparing `tmp/superb-ai-label-0.21.2.tar.gz` & `tmp/superb-ai-label-0.21.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/superb-ai-label-0.21.2.tar", last modified: Tue Mar 26 08:39:37 2024, max compression
+gzip compressed data, was "dist/superb-ai-label-0.21.3.tar", last modified: Tue May 14 07:53:28 2024, max compression
```

## Comparing `superb-ai-label-0.21.2.tar` & `superb-ai-label-0.21.3.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/command/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/command/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/command/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/core/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/core/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/core/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/core/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/core/models/attrs/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/core/models/attrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/core/models/attrs/attributes_container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/core/models/types/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/core/models/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/core/models/types/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/core/models/types/type_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/core/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/core/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/datauri/
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/datauri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/datauri/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/exports/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/exports/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/exports/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/exports/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/exports/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/image_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/labels/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/labels/label.py
--rw-r--r--   0 runner    (1001) docker     (127)    16077 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/labels/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/labels/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/labels/serializer/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/labels/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/labels/serializer/label_info_build_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/labels/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/models/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/models/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/models/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/models/video_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/models/video_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/orm/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/orm/json_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/orm/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/orm/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/orm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/orm/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/orm/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/orm/type_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/orm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/pointcloud_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/projects/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/projects/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/projects/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/projects/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/projects/session.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32857 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/sdk_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13001 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/spb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12834 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/tasks/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/tasks/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/tasks/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/tasks/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/users/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/users/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/users/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/users/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/users/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/spb_label/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/utils/color_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/utils/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-03-26 08:39:18.000000 superb-ai-label-0.21.2/spb_label/video_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/superb_ai_label.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-03-26 08:39:36.000000 superb-ai-label-0.21.2/superb_ai_label.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-26 08:39:37.000000 superb-ai-label-0.21.2/superb_ai_label.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 08:39:36.000000 superb-ai-label-0.21.2/superb_ai_label.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 08:39:36.000000 superb-ai-label-0.21.2/superb_ai_label.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-26 08:39:36.000000 superb-ai-label-0.21.2/superb_ai_label.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 08:39:36.000000 superb-ai-label-0.21.2/superb_ai_label.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/command/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/command/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/core/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/core/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/core/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/core/models/attrs/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/core/models/attrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/core/models/attrs/attributes_container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/core/models/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/core/models/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/core/models/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/core/models/types/type_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/core/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/core/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/datauri/
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/datauri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/datauri/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/exports/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/exports/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/exports/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/exports/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/image_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/labels/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16077 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/labels/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/labels/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/labels/serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/labels/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/labels/serializer/label_info_build_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/labels/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/models/video_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/models/video_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/orm/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/orm/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/orm/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/orm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/orm/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/orm/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/orm/type_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/orm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/pointcloud_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/projects/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/projects/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/projects/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/projects/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32678 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/sdk_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13001 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/spb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12834 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/tasks/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/tasks/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/tasks/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/tasks/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/users/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/users/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/users/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/users/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/users/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/spb_label/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/utils/color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/utils/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-14 07:53:01.000000 superb-ai-label-0.21.3/spb_label/video_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/superb_ai_label.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/superb_ai_label.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/superb_ai_label.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/superb_ai_label.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/superb_ai_label.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/superb_ai_label.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 07:53:28.000000 superb-ai-label-0.21.3/superb_ai_label.egg-info/top_level.txt
```

### Comparing `superb-ai-label-0.21.2/PKG-INFO` & `superb-ai-label-0.21.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superb-ai-label
-Version: 0.21.2
+Version: 0.21.3
 Summary: Suite Standard Library
 Home-page: https://github.com/Superb-AI-Suite/superb-ai-label-python.git
 Author: Superb AI Dev Team
 Author-email: support@superb-ai.com
 License: MIT
 Description: <!-- <p align="center">
           <a href="http://suite-api.superb-ai.com/" target="blank"><img src="logo/cool-tree.png" width="200" height="200" alt="Cool-Tree Logo" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superb-ai-label Version: 0.21.2 Summary: Suite
+Metadata-Version: 2.1 Name: superb-ai-label Version: 0.21.3 Summary: Suite
 Standard Library Home-page: https://github.com/Superb-AI-Suite/superb-ai-label-
 python.git Author: Superb AI Dev Team Author-email: support@superb-ai.com
 License: MIT Description: # Superb AI Suite Software Development Kit ![Build]
 (https://github.com/Superb-AI-Suite/spb-cli/workflows/Build/badge.svg) !
 [Version](https://img.shields.io/pypi/v/spb-cli) [![License: MIT](https://
 img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/
 MIT) Official Superb AI Suite Software Development Kit for managing data and
```

### Comparing `superb-ai-label-0.21.2/README.md` & `superb-ai-label-0.21.3/README.md`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/setup.py` & `superb-ai-label-0.21.3/setup.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/__init__.py` & `superb-ai-label-0.21.3/spb_label/__init__.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/command/__init__.py` & `superb-ai-label-0.21.3/spb_label/command/__init__.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/command/builder.py` & `superb-ai-label-0.21.3/spb_label/command/builder.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/command/commands.py` & `superb-ai-label-0.21.3/spb_label/command/commands.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/core/manager.py` & `superb-ai-label-0.21.3/spb_label/core/manager.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/core/model.py` & `superb-ai-label-0.21.3/spb_label/core/model.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/core/models/attrs/attributes_container.py` & `superb-ai-label-0.21.3/spb_label/core/models/attrs/attributes_container.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/core/models/types/type.py` & `superb-ai-label-0.21.3/spb_label/core/models/types/type.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/core/models/types/type_base.py` & `superb-ai-label-0.21.3/spb_label/core/models/types/type_base.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/core/query.py` & `superb-ai-label-0.21.3/spb_label/core/query.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/core/session.py` & `superb-ai-label-0.21.3/spb_label/core/session.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/datauri/__init__.py` & `superb-ai-label-0.21.3/spb_label/datauri/__init__.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/exceptions/__init__.py` & `superb-ai-label-0.21.3/spb_label/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/exports/export.py` & `superb-ai-label-0.21.3/spb_label/exports/export.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/exports/manager.py` & `superb-ai-label-0.21.3/spb_label/exports/manager.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/exports/session.py` & `superb-ai-label-0.21.3/spb_label/exports/session.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/image_sdk.py` & `superb-ai-label-0.21.3/spb_label/image_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,27 +110,28 @@
         except:
             return None
 
     ##############################
     # Simple SDK functions
     ##############################
 
-    def download_image(self, download_to="./"):
+    def download_image(self, download_to="./", print_log=False):
         self._describe_data_detail()
         if self._is_expired_url():
             return None, None
 
         if download_to is None:
             download_to = self._data.data_key
         path = self._data.data_key.lstrip("/")
         full_path = os.path.join(
             download_to,
             path,
         )
-        print("[INFO] Downloaded to {}".format(full_path))
+        if print_log:
+            print("[INFO] Downloaded to {}".format(full_path))
         return retrieve_file(
             url=self._data.data_url,
             file_path=full_path
         )
 
     def get_image(self):
         self._describe_data_detail()
```

### Comparing `superb-ai-label-0.21.2/spb_label/labels/label.py` & `superb-ai-label-0.21.3/spb_label/labels/label.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/labels/manager.py` & `superb-ai-label-0.21.3/spb_label/labels/manager.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/labels/query.py` & `superb-ai-label-0.21.3/spb_label/labels/query.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/labels/serializer/label_info_build_params.py` & `superb-ai-label-0.21.3/spb_label/labels/serializer/label_info_build_params.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/labels/session.py` & `superb-ai-label-0.21.3/spb_label/labels/session.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/models/data.py` & `superb-ai-label-0.21.3/spb_label/models/data.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/models/label.py` & `superb-ai-label-0.21.3/spb_label/models/label.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/models/project.py` & `superb-ai-label-0.21.3/spb_label/models/project.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/models/video_data.py` & `superb-ai-label-0.21.3/spb_label/models/video_data.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/models/video_label.py` & `superb-ai-label-0.21.3/spb_label/models/video_label.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/orm/__init__.py` & `superb-ai-label-0.21.3/spb_label/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/orm/json_type.py` & `superb-ai-label-0.21.3/spb_label/orm/json_type.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/orm/loading.py` & `superb-ai-label-0.21.3/spb_label/orm/loading.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/orm/manager.py` & `superb-ai-label-0.21.3/spb_label/orm/manager.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/orm/model.py` & `superb-ai-label-0.21.3/spb_label/orm/model.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/orm/query.py` & `superb-ai-label-0.21.3/spb_label/orm/query.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/orm/type.py` & `superb-ai-label-0.21.3/spb_label/orm/type.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/orm/type_base.py` & `superb-ai-label-0.21.3/spb_label/orm/type_base.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/orm/utils.py` & `superb-ai-label-0.21.3/spb_label/orm/utils.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/pointcloud_sdk.py` & `superb-ai-label-0.21.3/spb_label/pointcloud_sdk.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/projects/manager.py` & `superb-ai-label-0.21.3/spb_label/projects/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,22 @@
 
     def create_project(
         self,
         name: str,
         label_interface: dict,
         description: str = "",
         is_public: bool = False,
-        allow_advanced_qa: bool = False,
     ) -> Optional[Project]:
         query_id = "createProject"
         self.query.query_id = query_id
         project_info = {
             "name": name,
             "description": description,
             "label_interface": label_interface,
             "is_public": is_public,
-            "settings": {
-                "allow_advanced_qa": allow_advanced_qa,
-            },
         }
         if "workapp" not in project_info:
             project_info["workapp"] = label_interface["type"]
 
         project = Project()
         response_attrs = "\n".join(project.get_property_names())
         query = f"mutation ($projectInfo:JSONObject!) {{{query_id}(projectInfo: $projectInfo) {{{response_attrs}}}}}"
@@ -74,15 +70,14 @@
     def update_project(
         self,
         id: uuid.UUID,
         new_name: str = None,
         label_interface: dict = None,
         description: str = None,
         is_public: bool = None,
-        allow_advanced_qa: bool = None,
     ):
         existing_project = self.get_project_by_id(id=id)
 
         query_id = "updateProject"
         self.query.query_id = query_id
         project_info = dict()
         if new_name is not None:
@@ -96,22 +91,14 @@
                 != label_interface["type"]
             ):
                 raise PreConditionException(
                     "[ERROR] Workapp type cannot be changed"
                 )
         if is_public is not None:
             project_info.update({"is_public": is_public})
-        if allow_advanced_qa is not None:
-            project_info.update(
-                {
-                    "settings": {
-                        "allow_advanced_qa": allow_advanced_qa,
-                    }
-                }
-            )
 
         project = Project(id=id)
         id = project.to_json()["id"]
         response_attr = "\n".join(project.get_property_names())
         query = f"mutation ($id: String!, $projectInfo: JSONObject!) {{{query_id}(id: $id, projectInfo: $projectInfo) {{{response_attr}}}}}"
         values = {"id": id, "projectInfo": project_info}
         response = self.session.execute(query, values)
```

### Comparing `superb-ai-label-0.21.2/spb_label/projects/project.py` & `superb-ai-label-0.21.3/spb_label/projects/project.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/projects/query.py` & `superb-ai-label-0.21.3/spb_label/projects/query.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/projects/session.py` & `superb-ai-label-0.21.3/spb_label/projects/session.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/sdk.py` & `superb-ai-label-0.21.3/spb_label/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,53 +116,49 @@
 
     def create_project(
         self,
         name: str,
         label_interface: dict,
         description: str = "",
         is_public: bool = False,
-        allow_advanced_qa: bool = False,
     ):
         manager = ProjectManager(
             self.credential["team_name"], self.credential["access_key"]
         )
         project = manager.create_project(
             name=name,
             label_interface=label_interface,
             description=description,
             is_public=is_public,
-            allow_advanced_qa=allow_advanced_qa,
         )
         if project:
             self._project = project
             print(f"[INFO] create project success: {self._project.name}.")
 
     def update_project(
         self,
         id: uuid.UUID,
         new_name: str = None,
         label_interface: dict = None,
         description: str = None,
         is_public: bool = None,
-        allow_advanced_qa: bool = None,
     ):
         manager = ProjectManager(
             self.credential["team_name"], self.credential["access_key"]
         )
         if not (id or new_name or label_interface or description or is_public):
             raise ParameterException(
                 "[ERROR] More than one paramter should be described."
             )
         project = manager.update_project(
             id=id,
             new_name=new_name,
             label_interface=label_interface,
             description=description,
             is_public=is_public,
-            allow_advanced_qa=allow_advanced_qa,
         )
 
         if project:
             self._project = project
             print(f"[INFO] Update project success: {self._project.name}.")
 
     def get_project(self, name: str = None, id: uuid.UUID = None):
```

### Comparing `superb-ai-label-0.21.2/spb_label/session.py` & `superb-ai-label-0.21.3/spb_label/session.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/spb_logger.py` & `superb-ai-label-0.21.3/spb_label/spb_logger.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/tasks/manager.py` & `superb-ai-label-0.21.3/spb_label/tasks/manager.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/tasks/query.py` & `superb-ai-label-0.21.3/spb_label/tasks/query.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/tasks/session.py` & `superb-ai-label-0.21.3/spb_label/tasks/session.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/tasks/task.py` & `superb-ai-label-0.21.3/spb_label/tasks/task.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/users/manager.py` & `superb-ai-label-0.21.3/spb_label/users/manager.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/users/query.py` & `superb-ai-label-0.21.3/spb_label/users/query.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/users/session.py` & `superb-ai-label-0.21.3/spb_label/users/session.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/utils/deprecated.py` & `superb-ai-label-0.21.3/spb_label/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/utils/file_utils.py` & `superb-ai-label-0.21.3/spb_label/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/utils/search_filter.py` & `superb-ai-label-0.21.3/spb_label/utils/search_filter.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/utils/utils.py` & `superb-ai-label-0.21.3/spb_label/utils/utils.py`

 * *Files identical despite different names*

### Comparing `superb-ai-label-0.21.2/spb_label/video_sdk.py` & `superb-ai-label-0.21.3/spb_label/video_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,34 +58,35 @@
     def get_frame(self, idx):
         return self.get_frame_url(idx)
 
     ##############################
     # Simple SDK functions
     ##############################
 
-    def download_image(self, download_to=None):
+    def download_image(self, download_to=None, print_log=False):
         raise NotSupportedException(
             "Does not support download label image."
         )
 
     def get_image(self):
         raise NotSupportedException(
             "Does not support describe label image."
         )
 
-    def download_video(self, download_to=None):
+    def download_video(self, download_to=None, print_log=False):
         self._describe_data_detail()
         if self._is_expired_url():
             return None
         if self._data.data_url is None:
             return None
 
         if download_to is None:
             download_to = self._data.data_key
-            print("[INFO] Downloaded to {}".format(download_to))
+            if print_log:
+                print("[INFO] Downloaded to {}".format(download_to))
 
         data_url = json.loads(self._data.data_url)
         for frame_idx, file_info in enumerate(data_url["file_infos"]):
             url = self.get_frame_url(frame_idx, data_url)
             retrieve_file(
                 url=url,
                 file_path=os.path.join(download_to, file_info["file_name"])
```

### Comparing `superb-ai-label-0.21.2/superb_ai_label.egg-info/PKG-INFO` & `superb-ai-label-0.21.3/superb_ai_label.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superb-ai-label
-Version: 0.21.2
+Version: 0.21.3
 Summary: Suite Standard Library
 Home-page: https://github.com/Superb-AI-Suite/superb-ai-label-python.git
 Author: Superb AI Dev Team
 Author-email: support@superb-ai.com
 License: MIT
 Description: <!-- <p align="center">
           <a href="http://suite-api.superb-ai.com/" target="blank"><img src="logo/cool-tree.png" width="200" height="200" alt="Cool-Tree Logo" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superb-ai-label Version: 0.21.2 Summary: Suite
+Metadata-Version: 2.1 Name: superb-ai-label Version: 0.21.3 Summary: Suite
 Standard Library Home-page: https://github.com/Superb-AI-Suite/superb-ai-label-
 python.git Author: Superb AI Dev Team Author-email: support@superb-ai.com
 License: MIT Description: # Superb AI Suite Software Development Kit ![Build]
 (https://github.com/Superb-AI-Suite/spb-cli/workflows/Build/badge.svg) !
 [Version](https://img.shields.io/pypi/v/spb-cli) [![License: MIT](https://
 img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/
 MIT) Official Superb AI Suite Software Development Kit for managing data and
```

### Comparing `superb-ai-label-0.21.2/superb_ai_label.egg-info/SOURCES.txt` & `superb-ai-label-0.21.3/superb_ai_label.egg-info/SOURCES.txt`

 * *Files identical despite different names*

