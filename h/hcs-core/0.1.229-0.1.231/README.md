# Comparing `tmp/hcs_core-0.1.229.tar.gz` & `tmp/hcs_core-0.1.231.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs_core-0.1.229.tar", last modified: Fri May 10 16:39:25 2024, max compression
+gzip compressed data, was "hcs_core-0.1.231.tar", last modified: Tue May 14 18:53:59 2024, max compression
```

## Comparing `hcs_core-0.1.229.tar` & `hcs_core-0.1.231.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-10 16:39:25.636412 hcs_core-0.1.229/
--rw-r--r--   0 nanw       (501) staff       (20)     1405 2024-05-10 16:39:25.635749 hcs_core-0.1.229/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)       25 2024-04-09 21:58:38.000000 hcs_core-0.1.229/README.md
--rw-r--r--   0 nanw       (501) staff       (20)        7 2024-05-10 16:39:21.000000 hcs_core-0.1.229/VERSION
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-10 16:39:25.577325 hcs_core-0.1.229/hcs_core/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-10 16:39:25.593653 hcs_core-0.1.229/hcs_core/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)      790 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-10 16:39:25.596461 hcs_core-0.1.229/hcs_core/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3086 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/built_in_cmds/_ut.py
--rw-r--r--   0 nanw       (501) staff       (20)     2387 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     4034 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     2274 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     5791 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1160 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    14088 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/data_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2856 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     1623 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/extension.py
--rw-r--r--   0 nanw       (501) staff       (20)     6801 2024-05-09 16:11:42.000000 hcs_core-0.1.229/hcs_core/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     4666 2024-05-09 16:11:42.000000 hcs_core-0.1.229/hcs_core/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     6346 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/logger.py
--rw-r--r--   0 nanw       (501) staff       (20)     6518 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1767 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/recent.py
--rw-r--r--   0 nanw       (501) staff       (20)     1619 2024-05-09 16:11:42.000000 hcs_core-0.1.229/hcs_core/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     7933 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3245 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/ctxp/var_template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-10 16:39:25.604176 hcs_core-0.1.229/hcs_core/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      203 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      125 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/actions.py
--rw-r--r--   0 nanw       (501) staff       (20)     1298 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/base_provider.py
--rw-r--r--   0 nanw       (501) staff       (20)      116 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    20914 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)    12918 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     7784 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     5363 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/kop.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-10 16:39:25.604943 hcs_core-0.1.229/hcs_core/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-10 16:39:25.607901 hcs_core-0.1.229/hcs_core/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       30 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       34 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1994 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/provider/dev/dummy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1104 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/plan/provider/dev/fibonacci.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-10 16:39:25.617802 hcs_core-0.1.229/hcs_core/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     5194 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1790 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/sglib/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     8378 2024-04-11 21:31:53.000000 hcs_core-0.1.229/hcs_core/sglib/client_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     8043 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     5167 2024-04-20 00:00:21.000000 hcs_core-0.1.229/hcs_core/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      901 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)    10128 2024-05-09 16:11:42.000000 hcs_core-0.1.229/hcs_core/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)      684 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/sglib/payload_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-10 16:39:25.634088 hcs_core-0.1.229/hcs_core/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     3482 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)      838 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/util/exit.py
--rw-r--r--   0 nanw       (501) staff       (20)     1755 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/util/hcs_constants.py
--rw-r--r--   0 nanw       (501) staff       (20)     8438 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/util/job_view.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1946 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2958 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/util/scheduler.py
--rw-r--r--   0 nanw       (501) staff       (20)     1239 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/util/ssl_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1727 2024-04-09 21:58:38.000000 hcs_core-0.1.229/hcs_core/util/versions.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-05-10 16:39:25.634897 hcs_core-0.1.229/hcs_core.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     1405 2024-05-10 16:39:25.000000 hcs_core-0.1.229/hcs_core.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1810 2024-05-10 16:39:25.000000 hcs_core-0.1.229/hcs_core.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2024-05-10 16:39:25.000000 hcs_core-0.1.229/hcs_core.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)      284 2024-05-10 16:39:25.000000 hcs_core-0.1.229/hcs_core.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)        9 2024-05-10 16:39:25.000000 hcs_core-0.1.229/hcs_core.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)     1250 2024-04-09 21:58:38.000000 hcs_core-0.1.229/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      284 2024-05-09 16:11:42.000000 hcs_core-0.1.229/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2024-05-10 16:39:25.636520 hcs_core-0.1.229/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      808 2024-04-09 21:58:38.000000 hcs_core-0.1.229/setup.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-14 18:53:59.374966 hcs_core-0.1.231/
+-rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-14 18:53:59.374514 hcs_core-0.1.231/PKG-INFO
+-rw-r--r--   0 nanw       (503) staff       (20)       25 2024-05-14 18:28:08.000000 hcs_core-0.1.231/README.md
+-rw-r--r--   0 nanw       (503) staff       (20)        7 2024-05-14 18:53:57.000000 hcs_core-0.1.231/VERSION
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-14 18:53:59.342772 hcs_core-0.1.231/hcs_core/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/__init__.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-14 18:53:59.355584 hcs_core-0.1.231/hcs_core/ctxp/
+-rw-r--r--   0 nanw       (503) staff       (20)      790 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1155 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/_init.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-14 18:53:59.358039 hcs_core-0.1.231/hcs_core/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3086 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/built_in_cmds/_ut.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2387 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)     4034 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2274 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/cli_options.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5791 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (503) staff       (20)      936 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/config.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1160 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)    14088 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/data_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2856 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/duration.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1623 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/extension.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6801 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/fstore.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1200 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/init.py
+-rw-r--r--   0 nanw       (503) staff       (20)     4666 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6346 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/logger.py
+-rw-r--r--   0 nanw       (503) staff       (20)     6586 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/profile.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1565 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1767 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/recent.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1619 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/state.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8036 2024-05-14 18:37:03.000000 hcs_core-0.1.231/hcs_core/ctxp/util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3245 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/ctxp/var_template.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-14 18:53:59.361042 hcs_core-0.1.231/hcs_core/plan/
+-rw-r--r--   0 nanw       (503) staff       (20)      203 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)      125 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/actions.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1298 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/base_provider.py
+-rw-r--r--   0 nanw       (503) staff       (20)      116 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/context.py
+-rw-r--r--   0 nanw       (503) staff       (20)    20914 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/core.py
+-rw-r--r--   0 nanw       (503) staff       (20)    12918 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/dag.py
+-rw-r--r--   0 nanw       (503) staff       (20)     7784 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/helper.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5363 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/kop.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-14 18:53:59.361610 hcs_core-0.1.231/hcs_core/plan/provider/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-14 18:53:59.363046 hcs_core-0.1.231/hcs_core/plan/provider/dev/
+-rw-r--r--   0 nanw       (503) staff       (20)       30 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)       34 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1994 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/provider/dev/dummy.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1104 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/plan/provider/dev/fibonacci.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-14 18:53:59.368080 hcs_core-0.1.231/hcs_core/sglib/
+-rw-r--r--   0 nanw       (503) staff       (20)      654 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/sglib/__init__.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5194 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/sglib/auth.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1790 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/sglib/cli_options.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8378 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/sglib/client_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8043 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/sglib/csp.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5167 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/sglib/ez_client.py
+-rw-r--r--   0 nanw       (503) staff       (20)      901 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (503) staff       (20)    10128 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/sglib/login_support.py
+-rw-r--r--   0 nanw       (503) staff       (20)      684 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/sglib/payload_util.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-14 18:53:59.373300 hcs_core-0.1.231/hcs_core/util/
+-rw-r--r--   0 nanw       (503) staff       (20)        0 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/util/__init__.py
+-rwxr-xr-x   0 nanw       (503) staff       (20)     2535 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/util/check_license.py
+-rw-r--r--   0 nanw       (503) staff       (20)     3482 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/util/duration.py
+-rw-r--r--   0 nanw       (503) staff       (20)      838 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/util/exit.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1755 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/util/hcs_constants.py
+-rw-r--r--   0 nanw       (503) staff       (20)     8438 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/util/job_view.py
+-rw-r--r--   0 nanw       (503) staff       (20)     5288 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/util/pki_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1946 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/util/query_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     2958 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/util/scheduler.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1239 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/util/ssl_util.py
+-rw-r--r--   0 nanw       (503) staff       (20)     1727 2024-05-14 18:28:08.000000 hcs_core-0.1.231/hcs_core/util/versions.py
+drwxr-xr-x   0 nanw       (503) staff       (20)        0 2024-05-14 18:53:59.373875 hcs_core-0.1.231/hcs_core.egg-info/
+-rw-r--r--   0 nanw       (503) staff       (20)     1405 2024-05-14 18:53:59.000000 hcs_core-0.1.231/hcs_core.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (503) staff       (20)     1810 2024-05-14 18:53:59.000000 hcs_core-0.1.231/hcs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (503) staff       (20)        1 2024-05-14 18:53:59.000000 hcs_core-0.1.231/hcs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-14 18:53:59.000000 hcs_core-0.1.231/hcs_core.egg-info/requires.txt
+-rw-r--r--   0 nanw       (503) staff       (20)        9 2024-05-14 18:53:59.000000 hcs_core-0.1.231/hcs_core.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (503) staff       (20)     1250 2024-05-14 18:28:08.000000 hcs_core-0.1.231/pyproject.toml
+-rw-r--r--   0 nanw       (503) staff       (20)      284 2024-05-14 18:28:08.000000 hcs_core-0.1.231/requirements.txt
+-rw-r--r--   0 nanw       (503) staff       (20)       38 2024-05-14 18:53:59.375023 hcs_core-0.1.231/setup.cfg
+-rw-r--r--   0 nanw       (503) staff       (20)      808 2024-05-14 18:28:08.000000 hcs_core-0.1.231/setup.py
```

### Comparing `hcs_core-0.1.229/PKG-INFO` & `hcs_core-0.1.231/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.229
+Version: 0.1.231
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/__init__.py` & `hcs_core-0.1.231/hcs_core/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/_init.py` & `hcs_core-0.1.231/hcs_core/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/built_in_cmds/_ut.py` & `hcs_core-0.1.231/hcs_core/ctxp/built_in_cmds/_ut.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/built_in_cmds/context.py` & `hcs_core-0.1.231/hcs_core/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/built_in_cmds/profile.py` & `hcs_core-0.1.231/hcs_core/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/cli_options.py` & `hcs_core-0.1.231/hcs_core/ctxp/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/cli_processor.py` & `hcs_core-0.1.231/hcs_core/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/config.py` & `hcs_core-0.1.231/hcs_core/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/context.py` & `hcs_core-0.1.231/hcs_core/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/data_util.py` & `hcs_core-0.1.231/hcs_core/ctxp/data_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/duration.py` & `hcs_core-0.1.231/hcs_core/ctxp/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/extension.py` & `hcs_core-0.1.231/hcs_core/ctxp/extension.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/fstore.py` & `hcs_core-0.1.231/hcs_core/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/init.py` & `hcs_core-0.1.231/hcs_core/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/jsondot.py` & `hcs_core-0.1.231/hcs_core/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/logger.py` & `hcs_core-0.1.231/hcs_core/ctxp/logger.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/profile.py` & `hcs_core-0.1.231/hcs_core/ctxp/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,17 @@
 
 def file(profile_name: str) -> str:
     """Get the file path of a profile"""
     return os.path.join(_repo_path, profile_name, "profile.yml")
 
 
 def exists(profile_name: str) -> bool:
-    return profile_name in names()
+    if profile_name not in names():
+        return False
+    return os.path.isfile(file(profile_name))
 
 
 class auth:
     @staticmethod
     def _file_name() -> str:
         return os.path.join(_repo_path, name(), ".auth")
```

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/profile_store.py` & `hcs_core-0.1.231/hcs_core/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/recent.py` & `hcs_core-0.1.231/hcs_core/ctxp/recent.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/state.py` & `hcs_core-0.1.231/hcs_core/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/util.py` & `hcs_core-0.1.231/hcs_core/ctxp/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,17 +157,23 @@
     else:
         text = str(reason)
     print(text, file=sys.stderr, flush=True)
     os._exit(code)
 
 
 def launch_text_editor(file_name: str, default_editor: str = None):
-    if not default_editor:
-        default_editor = "vi"
-    cmd = os.environ.get("EDITOR", default_editor) + " " + file_name
+    editor = os.environ.get("EDITOR", default_editor)
+    if not editor:
+        if os.name == "nt":
+            os.system(file_name)
+            return
+        else:
+            editor = "vi"
+
+    cmd = editor + " " + file_name
     subprocess.call(cmd, shell=True)
 
 
 def choose(prompt: str, items: list, fn_get_text: Callable = None, selected=None, select_by_default=True):
     if len(items) == 0:
         panic(prompt + " ERROR: no item available.")
```

### Comparing `hcs_core-0.1.229/hcs_core/ctxp/var_template.py` & `hcs_core-0.1.231/hcs_core/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/plan/base_provider.py` & `hcs_core-0.1.231/hcs_core/plan/base_provider.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/plan/core.py` & `hcs_core-0.1.231/hcs_core/plan/core.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/plan/dag.py` & `hcs_core-0.1.231/hcs_core/plan/dag.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/plan/helper.py` & `hcs_core-0.1.231/hcs_core/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/plan/kop.py` & `hcs_core-0.1.231/hcs_core/plan/kop.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/plan/provider/dev/dummy.py` & `hcs_core-0.1.231/hcs_core/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/plan/provider/dev/fibonacci.py` & `hcs_core-0.1.231/hcs_core/plan/provider/dev/fibonacci.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/sglib/__init__.py` & `hcs_core-0.1.231/hcs_core/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/sglib/auth.py` & `hcs_core-0.1.231/hcs_core/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/sglib/cli_options.py` & `hcs_core-0.1.231/hcs_core/sglib/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/sglib/client_util.py` & `hcs_core-0.1.231/hcs_core/sglib/client_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/sglib/csp.py` & `hcs_core-0.1.231/hcs_core/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/sglib/ez_client.py` & `hcs_core-0.1.231/hcs_core/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/sglib/hcs_client.py` & `hcs_core-0.1.231/hcs_core/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/sglib/login_support.py` & `hcs_core-0.1.231/hcs_core/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/sglib/payload_util.py` & `hcs_core-0.1.231/hcs_core/sglib/payload_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/util/check_license.py` & `hcs_core-0.1.231/hcs_core/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/util/duration.py` & `hcs_core-0.1.231/hcs_core/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/util/exit.py` & `hcs_core-0.1.231/hcs_core/util/exit.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/util/hcs_constants.py` & `hcs_core-0.1.231/hcs_core/util/hcs_constants.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/util/job_view.py` & `hcs_core-0.1.231/hcs_core/util/job_view.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/util/pki_util.py` & `hcs_core-0.1.231/hcs_core/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/util/query_util.py` & `hcs_core-0.1.231/hcs_core/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/util/scheduler.py` & `hcs_core-0.1.231/hcs_core/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/util/ssl_util.py` & `hcs_core-0.1.231/hcs_core/util/ssl_util.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core/util/versions.py` & `hcs_core-0.1.231/hcs_core/util/versions.py`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/hcs_core.egg-info/PKG-INFO` & `hcs_core-0.1.231/hcs_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.229
+Version: 0.1.231
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs_core-0.1.229/hcs_core.egg-info/SOURCES.txt` & `hcs_core-0.1.231/hcs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/pyproject.toml` & `hcs_core-0.1.231/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs_core-0.1.229/setup.py` & `hcs_core-0.1.231/setup.py`

 * *Files identical despite different names*
