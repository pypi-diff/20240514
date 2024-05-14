# Comparing `tmp/libvirt_provider-0.0.0a3.tar.gz` & `tmp/libvirt_provider-0.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvirt_provider-0.0.0a3.tar", last modified: Fri Mar  8 14:55:26 2024, max compression
+gzip compressed data, was "libvirt_provider-0.0.0a6.tar", last modified: Tue May 14 13:12:21 2024, max compression
```

## Comparing `libvirt_provider-0.0.0a3.tar` & `libvirt_provider-0.0.0a6.tar`

### file list

```diff
@@ -1,60 +1,66 @@
-drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-03-08 14:55:26.535611 libvirt_provider-0.0.0a3/
--rw-r--r--   0 rasmunk    (501) staff       (20)     1137 2024-03-08 14:55:26.533575 libvirt_provider-0.0.0a3/PKG-INFO
--rw-r--r--   0 rasmunk    (501) staff       (20)       95 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a3/README.rst
-drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-03-08 14:55:26.509653 libvirt_provider-0.0.0a3/libvirt_provider/
--rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a3/libvirt_provider/__init__.py
-drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-03-08 14:55:26.514118 libvirt_provider-0.0.0a3/libvirt_provider/cli/
--rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/__init__.py
--rw-r--r--   0 rasmunk    (501) staff       (20)     4746 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/cli.py
--rw-r--r--   0 rasmunk    (501) staff       (20)     2963 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/helpers.py
-drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-03-08 14:55:26.515846 libvirt_provider-0.0.0a3/libvirt_provider/cli/input_groups/
--rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/input_groups/__init__.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      645 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/input_groups/container.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      118 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/input_groups/driver.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      815 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/input_groups/instance.py
-drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-03-08 14:55:26.518761 libvirt_provider-0.0.0a3/libvirt_provider/cli/parsers/
--rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/parsers/__init__.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      625 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/parsers/actions.py
--rw-r--r--   0 rasmunk    (501) staff       (20)     1040 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/parsers/container.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      418 2024-02-28 11:40:22.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/parsers/driver.py
--rw-r--r--   0 rasmunk    (501) staff       (20)     4295 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/cli/parsers/instance.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      575 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/client.py
--rw-r--r--   0 rasmunk    (501) staff       (20)     2955 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a3/libvirt_provider/cluster.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      112 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a3/libvirt_provider/config.py
--rw-r--r--   0 rasmunk    (501) staff       (20)     1556 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/defaults.py
--rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a3/libvirt_provider/helpers.py
-drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-03-08 14:55:26.524859 libvirt_provider-0.0.0a3/libvirt_provider/instance/
--rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a3/libvirt_provider/instance/__init__.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      317 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/instance/create.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      287 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/instance/get.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      326 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/instance/ls.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      266 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/instance/remove.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      290 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/instance/show.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      263 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/instance/start.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      300 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/instance/state.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      261 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/instance/stop.py
--rw-r--r--   0 rasmunk    (501) staff       (20)    11714 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/models.py
--rw-r--r--   0 rasmunk    (501) staff       (20)     2354 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/pool.py
--rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a3/libvirt_provider/types.py
-drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-03-08 14:55:26.527803 libvirt_provider-0.0.0a3/libvirt_provider/utils/
--rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a3/libvirt_provider/utils/__init__.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      195 2024-01-09 14:47:26.000000 libvirt_provider-0.0.0a3/libvirt_provider/utils/db.py
--rw-r--r--   0 rasmunk    (501) staff       (20)       86 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a3/libvirt_provider/utils/format.py
--rw-r--r--   0 rasmunk    (501) staff       (20)     4950 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/utils/io.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      434 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/libvirt_provider/utils/user.py
-drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-03-08 14:55:26.531621 libvirt_provider-0.0.0a3/libvirt_provider.egg-info/
--rw-r--r--   0 rasmunk    (501) staff       (20)     1137 2024-03-08 14:55:26.000000 libvirt_provider-0.0.0a3/libvirt_provider.egg-info/PKG-INFO
--rw-r--r--   0 rasmunk    (501) staff       (20)     1610 2024-03-08 14:55:26.000000 libvirt_provider-0.0.0a3/libvirt_provider.egg-info/SOURCES.txt
--rw-r--r--   0 rasmunk    (501) staff       (20)        1 2024-03-08 14:55:26.000000 libvirt_provider-0.0.0a3/libvirt_provider.egg-info/dependency_links.txt
--rw-r--r--   0 rasmunk    (501) staff       (20)      202 2024-03-08 14:55:26.000000 libvirt_provider-0.0.0a3/libvirt_provider.egg-info/entry_points.txt
--rw-r--r--   0 rasmunk    (501) staff       (20)      132 2024-03-08 14:55:26.000000 libvirt_provider-0.0.0a3/libvirt_provider.egg-info/requires.txt
--rw-r--r--   0 rasmunk    (501) staff       (20)       17 2024-03-08 14:55:26.000000 libvirt_provider-0.0.0a3/libvirt_provider.egg-info/top_level.txt
--rw-r--r--   0 rasmunk    (501) staff       (20)       38 2024-03-08 14:55:26.535784 libvirt_provider-0.0.0a3/setup.cfg
--rw-r--r--   0 rasmunk    (501) staff       (20)     1839 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a3/setup.py
-drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-03-08 14:55:26.530723 libvirt_provider-0.0.0a3/tests/
--rw-r--r--   0 rasmunk    (501) staff       (20)     3436 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/tests/test_dummy.py
--rw-r--r--   0 rasmunk    (501) staff       (20)     2995 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/tests/test_dummy_pool.py
--rw-r--r--   0 rasmunk    (501) staff       (20)    10999 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/tests/test_libvirt.py
--rw-r--r--   0 rasmunk    (501) staff       (20)      375 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/tests/test_libvirt_lxc.py
--rw-r--r--   0 rasmunk    (501) staff       (20)     4921 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/tests/test_libvirt_pool.py
--rw-r--r--   0 rasmunk    (501) staff       (20)     6087 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a3/tests/test_libvirt_remote_node.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.335917 libvirt_provider-0.0.0a6/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5925 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4884 2024-05-03 05:33:44.000000 libvirt_provider-0.0.0a6/README.rst
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.327916 libvirt_provider-0.0.0a6/libvirt_provider/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2023-11-27 15:36:25.000000 libvirt_provider-0.0.0a6/libvirt_provider/__init__.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.327916 libvirt_provider-0.0.0a6/libvirt_provider/cli/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-19 09:44:41.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4890 2024-05-03 05:33:44.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/cli.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2962 2024-03-12 08:00:51.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/helpers.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.327916 libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-19 10:27:45.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      821 2024-03-25 19:57:56.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/container.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      528 2024-05-03 05:33:44.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/driver.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      815 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/instance.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-19 09:44:41.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      625 2024-02-21 12:40:24.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/actions.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1271 2024-03-25 19:58:29.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/container.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1018 2024-05-03 05:33:44.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/driver.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4295 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/instance.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      575 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/client.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      112 2023-11-30 12:31:27.000000 libvirt_provider-0.0.0a6/libvirt_provider/config.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/libvirt_provider/container/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-04-25 12:21:54.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      323 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/create.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      293 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/get.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      333 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/ls.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      268 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/remove.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      263 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/stop.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1564 2024-03-12 08:00:51.000000 libvirt_provider-0.0.0a6/libvirt_provider/defaults.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2023-11-29 14:27:13.000000 libvirt_provider-0.0.0a6/libvirt_provider/helpers.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/libvirt_provider/instance/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-21 12:14:32.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      317 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/create.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      287 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/get.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      326 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/ls.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      283 2024-04-25 07:54:46.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/remove.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      290 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/show.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      263 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/start.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      300 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/state.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      261 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/stop.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    11797 2024-05-03 05:33:44.000000 libvirt_provider-0.0.0a6/libvirt_provider/models.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2304 2024-03-12 08:00:51.000000 libvirt_provider-0.0.0a6/libvirt_provider/pool.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2023-11-29 11:23:03.000000 libvirt_provider-0.0.0a6/libvirt_provider/types.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/libvirt_provider/utils/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2023-11-29 11:28:42.000000 libvirt_provider-0.0.0a6/libvirt_provider/utils/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      195 2024-01-09 15:39:48.000000 libvirt_provider-0.0.0a6/libvirt_provider/utils/db.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       86 2024-02-19 09:44:41.000000 libvirt_provider-0.0.0a6/libvirt_provider/utils/format.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5840 2024-05-06 12:44:20.000000 libvirt_provider-0.0.0a6/libvirt_provider/utils/io.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      759 2024-05-06 10:05:11.000000 libvirt_provider-0.0.0a6/libvirt_provider/utils/user.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5925 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1797 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        1 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      202 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/entry_points.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      131 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/requires.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       17 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/top_level.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       38 2024-05-14 13:12:21.335917 libvirt_provider-0.0.0a6/setup.cfg
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1839 2024-02-19 09:44:41.000000 libvirt_provider-0.0.0a6/setup.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/tests/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     3436 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/tests/test_dummy.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2995 2024-05-14 06:07:05.000000 libvirt_provider-0.0.0a6/tests/test_dummy_pool.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    11781 2024-05-06 16:30:51.000000 libvirt_provider-0.0.0a6/tests/test_libvirt.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      334 2024-04-25 07:54:46.000000 libvirt_provider-0.0.0a6/tests/test_libvirt_lxc.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5752 2024-05-06 16:32:24.000000 libvirt_provider-0.0.0a6/tests/test_libvirt_pool.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     7547 2024-05-14 11:49:50.000000 libvirt_provider-0.0.0a6/tests/test_libvirt_remote_node.py
```

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/cli/cli.py` & `libvirt_provider-0.0.0a6/libvirt_provider/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import datetime
 import json
 from libvirt_provider.utils.format import eprint
 from libvirt_provider.defaults import PACKAGE_NAME, LIBVIRT_CLI_STRUCTURE
-from libvirt_provider.cli.input_groups.driver import add_driver_group
+from libvirt_provider.cli.input_groups.driver import add_driver_group, has_driver_group
 from libvirt_provider.cli.helpers import cli_exec, import_from_module
 
 
 def to_str(o):
     if hasattr(o, "asdict"):
         return o.asdict()
     if isinstance(o, datetime.datetime):
@@ -77,35 +77,33 @@
                 module_name="{}".format(libvirt_cli_type),
                 func_name=operation,
                 provider_groups=provider_groups,
                 argument_groups=argument_groups,
             )
 
 
-def driver_cli(parser):
-    add_driver_group(parser)
-
-
-def functions_cli(commands):
+def libvirt_provider_cli(commands):
     for libvirt_cli_structure in LIBVIRT_CLI_STRUCTURE:
         for libvirt_cli_type, libvirt_cli_operations in libvirt_cli_structure.items():
             function_provider = commands.add_parser(libvirt_cli_type)
             function_parser = function_provider.add_subparsers(title="COMMAND")
+            if has_driver_group(libvirt_cli_type):
+                add_driver_group(function_provider, libvirt_cli_type)
             recursive_add_libvirt_operations(
                 libvirt_cli_type, libvirt_cli_operations, function_parser
             )
 
 
 def run():
-    parser = argparse.ArgumentParser(prog=PACKAGE_NAME)
+    parser = argparse.ArgumentParser(
+        prog=PACKAGE_NAME, formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
     commands = parser.add_subparsers(title="COMMAND")
-
-    driver_cli(parser)
     # Add libvirt functions to the CLI
-    functions_cli(commands)
+    libvirt_provider_cli(commands)
     args = parser.parse_args()
     # Convert to a dictionary
     arguments = vars(args)
     # Execute default function
     if "func" in arguments:
         func = arguments.pop("func")
         success, response = func(arguments)
```

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/cli/helpers.py` & `libvirt_provider-0.0.0a6/libvirt_provider/cli/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     else:
         argument_groups = []
 
     func = import_from_module(module_path, module_name, func_name)
     if not func:
         return False
 
-    ## Extract the arguments provided
+    # Extract the arguments provided
     driver_kwargs, remaining_driver_kwargs = extract_arguments(
         arguments, provider_groups
     )
     driver_kwargs = strip_argument_group_prefix(driver_kwargs, provider_groups)
     driver_provider = driver_kwargs.pop("name", LIBVIRT)
     client = new_client(driver_provider, **driver_kwargs)
```

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/cli/input_groups/container.py` & `libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from libvirt_provider.defaults import DRIVER, CONTAINER
 from libvirt_provider.cli.parsers.container import (
     create_group,
     remove_group,
+    show_group,
     ls_group,
 )
 
 
 def create_groups(parser):
     create_group(parser)
 
@@ -18,13 +19,21 @@
     remove_group(parser)
 
     provider_groups = [DRIVER]
     argument_groups = [CONTAINER]
     return provider_groups, argument_groups
 
 
+def show_groups(parser):
+    show_group(parser)
+
+    provider_groups = [DRIVER]
+    argument_groups = [CONTAINER]
+    return provider_groups, argument_groups
+
+
 def ls_groups(parser):
     ls_group(parser)
 
     provider_groups = [DRIVER]
     argument_groups = [CONTAINER]
     return provider_groups, argument_groups
```

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/cli/input_groups/instance.py` & `libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/instance.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/cli/parsers/actions.py` & `libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/actions.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/cli/parsers/container.py` & `libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/container.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,9 +31,16 @@
 def remove_group(parser):
     container_group = parser.add_argument_group(title="Container remove arguments")
     container_group.add_argument(
         "name", action=PositionalArgumentsAction, help="The name of the container"
     )
 
 
+def show_group(parser):
+    container_group = parser.add_argument_group(title="Container show arguments")
+    container_group.add_argument(
+        "name", action=PositionalArgumentsAction, help="The name of the container"
+    )
+
+
 def ls_group(parser):
     _ = parser.add_argument_group(title="Container list arguments")
```

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/cli/parsers/instance.py` & `libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/instance.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/client.py` & `libvirt_provider-0.0.0a6/libvirt_provider/client.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/defaults.py` & `libvirt_provider-0.0.0a6/libvirt_provider/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 DUMMY = "dummy"
 INSTANCE = "instance"
 CONTAINER = "container"
 
 INSTANCE_OPERATIONS = ["create", "remove", "show", "ls"]
 INSTANCE_CLI = {INSTANCE: INSTANCE_OPERATIONS}
 
-CONTAINER_OPERATIONS = ["create", "remove", "ls"]
+CONTAINER_OPERATIONS = ["create", "remove", "show", "ls"]
 CONTAINER_CLI = {CONTAINER: CONTAINER_OPERATIONS}
 
 LIBVIRT_CLI_STRUCTURE = [INSTANCE_CLI, CONTAINER_CLI]
 
 default_driver_config = {
     "uri": "test:///default",
     "key": None,
```

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/models.py` & `libvirt_provider-0.0.0a6/libvirt_provider/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,25 @@
             libvirt.VIR_CRED_REALM,
             libvirt.VIR_CRED_PASSPHRASE,
             libvirt.VIR_CRED_NOECHOPROMPT,
             libvirt.VIR_CRED_EXTERNAL,
         ]
         flags = 0
         auth_list = [valid_auth_options, auth_callback, None]
-        self._conn = libvirt.openAuth(self._open_uri, auth_list, flags)
+        try:
+            self._conn = libvirt.openAuth(self._open_uri, auth_list, flags)
+        except libvirt.libvirtError as err:
+            print(
+                "Could not connect to the libvirt socket: {} - {}".format(
+                    self._open_uri, err
+                )
+            )
+            print("Are you sure that the libvirt daemon is running?")
+            self._conn = None
+            raise Exception("Failed to connect to the libvirt daemon socket")
 
     def close(self):
         self._conn.close()
 
     def get(self, node_id):
         domain = self._get(node_id)
         if not domain:
@@ -350,22 +360,7 @@
         if not template_path:
             created_id = self._create(name=name, **kwargs)
         else:
             created_id = self._create_from_template(name, template_path, **kwargs)
         if not created_id:
             return False
         return self.get(created_id)
-
-    def get(self, container_id):
-        raise NotImplementedError
-
-    def start(self, container):
-        raise NotImplementedError
-
-    def stop(self, container):
-        raise NotImplementedError
-
-    def remove(self, container):
-        raise NotImplementedError
-
-    def ls(self):
-        raise NotImplementedError
```

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/pool.py` & `libvirt_provider-0.0.0a6/libvirt_provider/pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,42 +7,42 @@
         # The name of the pool is equal to the
         # database name
         self.name = name
         self._database_path = "{}.db".format(self.name)
         self._lock_path = "{}.lock".format(self.name)
 
     async def items(self):
-        with shelve.open(self._database_path) as db:
+        with shelve.open(self.name) as db:
             return [item for item in db.values()]
 
     async def add(self, item):
         if not hasattr(item, "id"):
             raise AttributeError(
                 "add item must have an 'id' attribute to be added to the pool"
             )
 
         lock = acquire_lock(self._lock_path)
         if not lock:
             return False
         try:
-            with shelve.open(self._database_path) as db:
+            with shelve.open(self.name) as db:
                 db[item.id] = item
         except Exception as err:
             print(err)
             return False
         finally:
             release_lock(lock)
         return True
 
     async def remove(self, item_id):
         lock = acquire_lock(self._lock_path)
         if not lock:
             return False
         try:
-            with shelve.open(self._database_path) as db:
+            with shelve.open(self.name) as db:
                 db.pop(item_id)
         except Exception as err:
             print(err)
             return False
         finally:
             release_lock(lock)
         return True
@@ -60,24 +60,24 @@
             print(err)
             return False
         finally:
             release_lock(lock)
         return True
 
     async def get(self, item_id):
-        with shelve.open(self._database_path) as db:
+        with shelve.open(self.name) as db:
             return db.get(item_id)
 
     async def flush(self):
         lock = acquire_lock(self._lock_path)
         if not lock:
             return False
 
         try:
-            with shelve.open(self._database_path) as db:
+            with shelve.open(self.name) as db:
                 [db.pop(item_id) for item_id in db.keys()]
         except Exception as err:
             print(err)
             return False
         finally:
             release_lock(lock)
         return True
```

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider/utils/io.py` & `libvirt_provider-0.0.0a6/libvirt_provider/utils/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -140,14 +140,54 @@
         os.chown(path, uid, gid)
     except Exception as err:
         print("Failed to set owner: {} on: {} - {}".format(uid, path, err))
         return False
     return True
 
 
+def get_uid(path):
+    try:
+        return stat(path).st_uid
+    except Exception as err:
+        print("Failed to get file uid: {} - {}".format(path, err))
+    return False
+
+
+def get_gid(path):
+    try:
+        return stat(path).st_gid
+    except Exception as err:
+        print("Failed to get file gid: {} - {}".format(path, err))
+    return False
+
+
+def get_mode(path):
+    try:
+        return oct(stat(path).st_mode)
+    except Exception as err:
+        print("Failed to get file mode: {} - {}".format(path, err))
+    return False
+
+
+def access(path, mode):
+    try:
+        return os.access(path, mode)
+    except Exception as err:
+        print("Failed to access file: {} - {}".format(path, err))
+    return False
+
+
+def stat(path):
+    try:
+        return os.stat(path)
+    except Exception as err:
+        print("Failed to get file stat: {} - {}".format(path, err))
+    return False
+
+
 def parse_yaml(data):
     try:
         parsed = yaml.safe_load(data)
         return parsed
     except yaml.reader.ReaderError as err:
         print("Failed to parse yaml: {}".format(err))
     return False
```

### Comparing `libvirt_provider-0.0.0a3/libvirt_provider.egg-info/SOURCES.txt` & `libvirt_provider-0.0.0a6/libvirt_provider.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 README.rst
 setup.py
 libvirt_provider/__init__.py
 libvirt_provider/client.py
-libvirt_provider/cluster.py
 libvirt_provider/config.py
 libvirt_provider/defaults.py
 libvirt_provider/helpers.py
 libvirt_provider/models.py
 libvirt_provider/pool.py
 libvirt_provider/types.py
 libvirt_provider.egg-info/PKG-INFO
@@ -23,14 +22,20 @@
 libvirt_provider/cli/input_groups/driver.py
 libvirt_provider/cli/input_groups/instance.py
 libvirt_provider/cli/parsers/__init__.py
 libvirt_provider/cli/parsers/actions.py
 libvirt_provider/cli/parsers/container.py
 libvirt_provider/cli/parsers/driver.py
 libvirt_provider/cli/parsers/instance.py
+libvirt_provider/container/__init__.py
+libvirt_provider/container/create.py
+libvirt_provider/container/get.py
+libvirt_provider/container/ls.py
+libvirt_provider/container/remove.py
+libvirt_provider/container/stop.py
 libvirt_provider/instance/__init__.py
 libvirt_provider/instance/create.py
 libvirt_provider/instance/get.py
 libvirt_provider/instance/ls.py
 libvirt_provider/instance/remove.py
 libvirt_provider/instance/show.py
 libvirt_provider/instance/start.py
```

### Comparing `libvirt_provider-0.0.0a3/setup.py` & `libvirt_provider-0.0.0a6/setup.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a3/tests/test_dummy.py` & `libvirt_provider-0.0.0a6/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a3/tests/test_dummy_pool.py` & `libvirt_provider-0.0.0a6/tests/test_dummy_pool.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a3/tests/test_libvirt.py` & `libvirt_provider-0.0.0a6/tests/test_libvirt.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,43 @@
     copy,
     join,
     exists,
     makedirs,
     load_json,
     chown,
     chmod,
+    get_uid,
+    get_gid,
+    access,
+)
+from libvirt_provider.utils.user import (
+    lookup_uid,
+    lookup_gid,
+    find_user_with_username,
+    find_group_with_groupname,
 )
-from libvirt_provider.utils.user import lookup_uid, lookup_gid
 from libvirt_provider.defaults import LIBVIRT
 from libvirt_provider.models import Node
 from libvirt_provider.client import new_client
 from libvirt_provider.instance.create import create
 from libvirt_provider.instance.remove import remove
 from libvirt_provider.instance.stop import stop
 from libvirt_provider.instance.get import get
 from libvirt_provider.instance.ls import ls
 from libvirt_provider.instance.state import state
 
 
 class TestLibvirt(unittest.IsolatedAsyncioTestCase):
     async def asyncSetUp(self):
-        self.user = "qemu"
+        user_base = "qemu"
+        self.user = find_user_with_username(user_base)
+        self.assertIsNot(self.user, False)
+        self.group = find_group_with_groupname(user_base)
+        self.assertIsNot(self.group, False)
+
         self.architecture = "x86_64"
         self.name = f"libvirt-{self.architecture}"
         # Note, a properly SELinux labelled directory is required when SELinux is enabled
         # self.images_dir = join(
         #    os.sep, "var", "lib", "libvirt", "images", self.architecture
         # )
         self.images_dir = join("tests", "images", self.architecture)
@@ -44,25 +57,34 @@
                 print(f"Downloading image: {url} for testing")
                 wget.download(url, self.image)
             except Exception as err:
                 print(f"Failed to download image: {url} - {err}")
                 self.assertFalse(True)
         self.assertTrue(exists(self.image))
 
-        qemu_uid, qemu_gid = lookup_uid(self.user), lookup_gid(self.user)
+        qemu_uid, qemu_gid = lookup_uid(self.user), lookup_gid(self.group)
+        self.assertIsNot(qemu_uid, False)
+        self.assertIsNot(qemu_gid, False)
+
         open_uri = "qemu:///session"
         self.client = new_client(LIBVIRT, open_uri=open_uri)
         for i in range(6):
             test_image = join(self.images_dir, f"{self.name}-Rocky-9-{i}.qcow2")
             if not exists(test_image):
                 self.assertTrue(copy(self.image, test_image))
             self.assertTrue(exists(test_image))
             # Ensure correct ownership on image file
-            self.assertTrue(chown(test_image, qemu_uid, qemu_gid))
-            self.assertTrue(chmod(test_image, 0o755))
+            existing_uid, existing_gid = get_uid(test_image), get_gid(test_image)
+            self.assertIsNot(existing_uid, False)
+            self.assertIsNot(existing_gid, False)
+            if existing_uid != qemu_uid or existing_gid != qemu_gid:
+                self.assertTrue(chown(test_image, qemu_uid, qemu_gid))
+            if not access(test_image, os.R_OK | os.X_OK):
+                self.assertTrue(chmod(test_image, 0o755))
+            self.assertTrue(access(test_image, os.R_OK | os.X_OK))
 
     async def asyncTearDown(self):
         for i in range(6):
             test_image = join(self.images_dir, f"{self.name}-Rocky-9-{i}.qcow2")
             self.assertTrue(remove_file(test_image))
             self.assertFalse(exists(test_image))
         self.client.close()
```

### Comparing `libvirt_provider-0.0.0a3/tests/test_libvirt_pool.py` & `libvirt_provider-0.0.0a6/tests/test_libvirt_pool.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,27 +6,40 @@
     copy,
     exists,
     join,
     makedirs,
     load_json,
     chown,
     chmod,
+    get_uid,
+    get_gid,
+    access,
+)
+from libvirt_provider.utils.user import (
+    lookup_uid,
+    lookup_gid,
+    find_user_with_username,
+    find_group_with_groupname,
 )
-from libvirt_provider.utils.user import lookup_uid, lookup_gid
 from libvirt_provider.defaults import LIBVIRT
 from libvirt_provider.client import new_client
 from libvirt_provider.pool import Pool
 from libvirt_provider.models import Node
 from libvirt_provider.instance.create import create
 from libvirt_provider.instance.remove import remove
 
 
 class TestLibvirtPool(unittest.IsolatedAsyncioTestCase):
     async def asyncSetUp(self):
-        self.user = "qemu"
+        user_base = "qemu"
+        self.user = find_user_with_username(user_base)
+        self.assertIsNot(self.user, False)
+        self.group = find_group_with_groupname(user_base)
+        self.assertIsNot(self.group, False)
+
         self.architecture = "x86_64"
         self.name = f"libvirt-pool-{self.architecture}"
         # Note, a properly SELinux labelled directory is required when SELinux is enabled
         # self.images_dir = join(
         #    os.sep, "var", "lib", "libvirt", "images", self.architecture
         # )
         self.images_dir = join("tests", "images", self.architecture)
@@ -41,25 +54,34 @@
                 print(f"Downloading image: {url} for testing")
                 wget.download(url, self.image)
             except Exception as err:
                 print(f"Failed to download image: {url} - {err}")
                 self.assertFalse(True)
         self.assertTrue(exists(self.image))
 
-        qemu_uid, qemu_gid = lookup_uid(self.user), lookup_gid(self.user)
+        qemu_uid, qemu_gid = lookup_uid(self.user), lookup_gid(self.group)
+        self.assertIsNot(qemu_uid, False)
+        self.assertIsNot(qemu_gid, False)
+
         open_uri = "qemu:///session"
         self.client = new_client(LIBVIRT, open_uri=open_uri)
         for i in range(2):
             test_image = join(self.images_dir, f"{self.name}-Rocky-9-{i}.qcow2")
             if not exists(test_image):
                 self.assertTrue(copy(self.image, test_image))
             self.assertTrue(exists(test_image))
             # Ensure correct ownership on image file
-            self.assertTrue(chown(test_image, qemu_uid, qemu_gid))
-            self.assertTrue(chmod(test_image, 0o755))
+            existing_uid, existing_gid = get_uid(test_image), get_gid(test_image)
+            self.assertIsNot(existing_uid, False)
+            self.assertIsNot(existing_gid, False)
+            if existing_uid != qemu_uid or existing_gid != qemu_gid:
+                self.assertTrue(chown(test_image, qemu_uid, qemu_gid))
+            if not access(test_image, os.R_OK | os.X_OK):
+                self.assertTrue(chmod(test_image, 0o755))
+            self.assertTrue(access(test_image, os.R_OK | os.X_OK))
 
     async def asyncTearDown(self):
         # Ensure that any pool is destroyed
         pool = Pool(self.name)
         for node in await pool.items():
             removed, response = await remove(self.client, node.id)
             self.assertTrue(removed)
@@ -116,7 +138,11 @@
 
             self.assertTrue(await pool.remove(node.id))
             self.assertFalse(await pool.get(node.id))
             self.assertEqual(len(await pool.items()), 0)
 
             removed, remove_response = await remove(self.client, node.id)
             self.assertTrue(removed)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

