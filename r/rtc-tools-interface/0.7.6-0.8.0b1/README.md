# Comparing `tmp/rtc-tools-interface-0.7.6.tar.gz` & `tmp/rtc-tools-interface-0.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-interface-0.7.6.tar", last modified: Tue May  7 15:05:50 2024, max compression
+gzip compressed data, was "rtc-tools-interface-0.8.0b1.tar", last modified: Tue May 14 13:15:55 2024, max compression
```

## Comparing `rtc-tools-interface-0.7.6.tar` & `rtc-tools-interface-0.8.0b1.tar`

### file list

```diff
@@ -1,60 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.599009 rtc-tools-interface-0.7.6/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)      268 2024-05-07 15:05:50.599009 rtc-tools-interface-0.7.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12413 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.593009 rtc-tools-interface-0.7.6/rtc_tools_interface.egg-info/
--rw-r--r--   0 root         (0) root         (0)      268 2024-05-07 15:05:50.000000 rtc-tools-interface-0.7.6/rtc_tools_interface.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1882 2024-05-07 15:05:50.000000 rtc-tools-interface-0.7.6/rtc_tools_interface.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 15:05:50.000000 rtc-tools-interface-0.7.6/rtc_tools_interface.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-05-07 15:05:50.000000 rtc-tools-interface-0.7.6/rtc_tools_interface.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-07 15:05:50.000000 rtc-tools-interface-0.7.6/rtc_tools_interface.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.600009 rtc-tools-interface-0.7.6/rtctools_interface/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-05-07 15:05:50.600009 rtc-tools-interface-0.7.6/rtctools_interface/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.595009 rtc-tools-interface-0.7.6/rtctools_interface/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10183 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/optimization/base_goal.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/optimization/base_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     4068 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/optimization/goal_generator_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     5055 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/optimization/goal_performance_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3613 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/optimization/goal_table_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.595009 rtc-tools-interface-0.7.6/rtctools_interface/optimization/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/optimization/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3032 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/optimization/helpers/statistics_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/optimization/plot_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/optimization/plot_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3292 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/optimization/read_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.596009 rtc-tools-interface-0.7.6/rtctools_interface/plotting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11023 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/plotting/plot_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    12382 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/plotting/subplot_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.596009 rtc-tools-interface-0.7.6/rtctools_interface/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/simulation/base_simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/simulation/plot_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.597009 rtc-tools-interface-0.7.6/rtctools_interface/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/utils/plot_table_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/utils/read_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2094 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/utils/read_plot_table.py
--rw-rw-rw-   0 root         (0) root         (0)     7748 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/utils/results_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/utils/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     1722 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/rtctools_interface/utils/type_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-05-07 15:05:50.600009 rtc-tools-interface-0.7.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.597009 rtc-tools-interface-0.7.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.598009 rtc-tools-interface-0.7.6/tests/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/tests/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/tests/optimization/test_base_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     1265 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/tests/optimization/test_passing_goals_directly.py
--rw-rw-rw-   0 root         (0) root         (0)     2076 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/tests/optimization/test_plot_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/tests/optimization/test_read_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.599009 rtc-tools-interface-0.7.6/tests/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/tests/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/tests/simulation/test_base_simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     1892 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/tests/simulation/test_plot_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 15:05:50.599009 rtc-tools-interface-0.7.6/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/tests/utils/get_test.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2024-05-07 15:05:49.000000 rtc-tools-interface-0.7.6/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.449740 rtc-tools-interface-0.8.0b1/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-14 13:15:55.449740 rtc-tools-interface-0.8.0b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14497 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.440740 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-14 13:15:55.000000 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-05-14 13:15:55.000000 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:15:55.000000 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-14 13:15:55.000000 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-14 13:15:55.000000 rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.450740 rtc-tools-interface-0.8.0b1/rtctools_interface/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-14 13:15:55.450740 rtc-tools-interface-0.8.0b1/rtctools_interface/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.442740 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/closed_loop_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4893 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/results_construction.py
+-rw-rw-rw-   0 root         (0) root         (0)     7597 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)    18717 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/closed_loop/time_series_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.444740 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10183 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/base_goal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/base_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     4068 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_generator_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     5147 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_performance_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3613 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_table_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.444740 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/helpers/statistics_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/plot_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/plot_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3292 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/read_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.445740 rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11023 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/plot_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    12382 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/subplot_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.445740 rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/base_simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/plot_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.447740 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/plot_table_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/read_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/read_plot_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     7748 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/results_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/rtctools_interface/utils/type_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-05-14 13:15:55.450740 rtc-tools-interface-0.8.0b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.447740 rtc-tools-interface-0.8.0b1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.447740 rtc-tools-interface-0.8.0b1/tests/closed_loop/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/tests/closed_loop/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/closed_loop/test_read_xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     4872 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/closed_loop/test_run_optization_problem_closed_loop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.448740 rtc-tools-interface-0.8.0b1/tests/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/tests/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/optimization/test_base_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1265 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/optimization/test_passing_goals_directly.py
+-rw-rw-rw-   0 root         (0) root         (0)     2076 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/optimization/test_plot_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/optimization/test_read_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.449740 rtc-tools-interface-0.8.0b1/tests/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/tests/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/simulation/test_base_simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1892 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/simulation/test_plot_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:15:55.449740 rtc-tools-interface-0.8.0b1/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:15:54.000000 rtc-tools-interface-0.8.0b1/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/tests/utils/get_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2024-05-14 13:15:53.000000 rtc-tools-interface-0.8.0b1/versioneer.py
```

### Comparing `rtc-tools-interface-0.7.6/COPYING.LESSER` & `rtc-tools-interface-0.8.0b1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/README.md` & `rtc-tools-interface-0.8.0b1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 ## Install
 
 ```bash
 pip install rtc-tools-interface
 ```
 
+## Table of Contents
+1. [Goal generator](#goal-generator)
+2. [Goal performance metrics](#goal-performance-metrics)
+3. [Automatic plotting of results](#automatic-plotting-of-results)
+4. [Closed loop runner](#closed-loop-runner)
+
 ## Goal generator
 The `goal generator` can be used to automatically add goals based on a csv file. Currently, the following goal types are supported:
 - range (default order is 2)
 - minimization_path (default order is 1)
 - maximization_path (default order is 1)
 - range_rate_of_change (default order is 1)
 
@@ -160,7 +166,36 @@
 |---------|-----------------|------------------|------------------|------------------|------------------|------------------|
 | goal_1  | Volume (\$m^3\$)  |      "PowerPlant1.QOut.Q"            |                  | | | goal_generator
 | goal_2  | Volume (\$m^3\$)  |      "PowerPlant1.QOut.Q, PowerPlant2.QOut.Q"            |   | |               | goal_generator
 |  | Volume (\$m^3\$)  |                |                  | electricity_cost | "Goal for minimizing electricity cost, at priority 10" | python
 
 
 After running the model, in your output folder the folder `figures` containing the figures is created.
+
+## Closed loop runner
+To run a closed loop experiment one can use the `run_optimization_problem_closed_loop` function from `run_closed_loop`.
+This function is a drop-in replacement for the `run_optimization_problem` of rtc-tools. The user only needs to specify the `closed_loop_dates.csv` in the input folder of the optimization problem.
+
+### Setup
+Import `run_optimization_problem_closed_loop` with:
+```python
+from rtctools_interface import run_optimization_problem_closed_loop
+```
+Add a table named `closed_loop_dates.csv` to the input folder of your optimization problem. The table should contain two columns: `start_date` and `end_date`.
+Each row of the table corresponds to one modelling period. 
+
+Example table `closed_loop_dates.csv`:
+```
+start_date, end_date
+2024-05-19, 2024-05-23
+2024-05-23, 2024-05-25
+```
+With this table rtc-tools will run two optimization problems (modelling periods): one with the data from 2024-05-19 upto and including 2024-05-23 and one from 2024-05-23 upto and including 2024-05-25. 
+The `run_optimization_problem_closed_loop` will automatically set the final results from the previous as initial conditions of the next run. Note that this happens for:
+- All variables available at the first time step in original timeseries_import, but not available at any timestep in the modelling period.
+- All variables in the `initial_state.csv` (if the csv_mixin is used).
+
+### Notes
+- The first start_date in your `closed_loop_dates.csv` should be equal to the start_date of your timeseries_import.
+- The different horizons should overlap with at least one day (to allow retrieving and setting initial values). An overlap of more days is allowed.
+- Currently only a single timestep is copied as an initial value.
+- The closed_loop runner only works in combination with the CSVMixin or the PIMixin. The CDFMixin is not supported.
```

### Comparing `rtc-tools-interface-0.7.6/rtc_tools_interface.egg-info/SOURCES.txt` & `rtc-tools-interface-0.8.0b1/rtc_tools_interface.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 rtc_tools_interface.egg-info/PKG-INFO
 rtc_tools_interface.egg-info/SOURCES.txt
 rtc_tools_interface.egg-info/dependency_links.txt
 rtc_tools_interface.egg-info/requires.txt
 rtc_tools_interface.egg-info/top_level.txt
 rtctools_interface/__init__.py
 rtctools_interface/_version.py
+rtctools_interface/closed_loop/__init__.py
+rtctools_interface/closed_loop/closed_loop_dates.py
+rtctools_interface/closed_loop/results_construction.py
+rtctools_interface/closed_loop/runner.py
+rtctools_interface/closed_loop/time_series_handler.py
 rtctools_interface/optimization/__init__.py
 rtctools_interface/optimization/base_goal.py
 rtctools_interface/optimization/base_optimization_problem.py
 rtctools_interface/optimization/goal_generator_mixin.py
 rtctools_interface/optimization/goal_performance_metrics.py
 rtctools_interface/optimization/goal_table_schema.py
 rtctools_interface/optimization/plot_goals_mixin.py
@@ -31,14 +36,17 @@
 rtctools_interface/utils/plot_table_schema.py
 rtctools_interface/utils/read_goals_mixin.py
 rtctools_interface/utils/read_plot_table.py
 rtctools_interface/utils/results_collection.py
 rtctools_interface/utils/serialization.py
 rtctools_interface/utils/type_definitions.py
 tests/__init__.py
+tests/closed_loop/__init__.py
+tests/closed_loop/test_read_xml.py
+tests/closed_loop/test_run_optization_problem_closed_loop.py
 tests/optimization/__init__.py
 tests/optimization/test_base_optimization_problem.py
 tests/optimization/test_passing_goals_directly.py
 tests/optimization/test_plot_goals_mixin.py
 tests/optimization/test_read_goals.py
 tests/simulation/__init__.py
 tests/simulation/test_base_simulation_problem.py
```

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/optimization/base_goal.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/base_goal.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/optimization/base_optimization_problem.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/base_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/optimization/goal_generator_mixin.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_generator_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/optimization/goal_performance_metrics.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_performance_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,24 @@
 
 
 def get_mean_absolute_percentual_difference(timeseries: np.ndarray) -> float:
     """Calculate the mean absolute percentual difference, ignoring entries where timeseries = 0."""
     nonzero_indices = np.nonzero(timeseries)
     timeseries = timeseries[nonzero_indices]
     differences = np.diff(timeseries)
+    if len(timeseries) <= 1:
+        return 0
     mapd = np.mean(np.abs(differences / timeseries[:-1]))
     return mapd
 
 
 def get_absolute_sum_difference(timeseries: np.ndarray) -> float:
     """Calculate the mean of absolute first-order difference."""
+    if len(timeseries) <= 1:
+        return 0
     mad = np.mean(np.abs(np.diff(timeseries)))
     return mad
 
 
 def get_max_difference(timeseries: np.ndarray) -> float:
     """Get maximum one step difference"""
     return max(np.diff(timeseries))
```

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/optimization/goal_table_schema.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/goal_table_schema.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/optimization/helpers/statistics_mixin.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/helpers/statistics_mixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,20 +49,25 @@
                 target_min = goal.target_min
             try:
                 target_max = goal.target_max.values
             except AttributeError:
                 target_max = goal.target_max
             return target_min, target_max
 
-        if goal.goal_type in ["range", "range_rate_of_change"]:
+        supported_goal_types = ["range", "range_rate_of_change"]
+        if goal.goal_type in supported_goal_types:
             if goal.target_data_type == "parameter":
                 target_min, target_max = get_parameter_ranges(goal)
             elif goal.target_data_type == "value":
                 target_min, target_max = get_value_ranges(goal)
             elif goal.target_data_type == "timeseries":
                 target_min, target_max = get_timeseries_ranges(goal)
             else:
                 message = "Target type {} not known for goal {}.".format(goal.target_data_type, goal.goal_id)
                 logger.error(message)
                 raise ValueError(message)
-            target_dict: TargetDict = {"target_min": target_min, "target_max": target_max}
+        else:
+            message = "Goal type {} not supported for target collection.".format(goal.goal_type)
+            logger.error(message)
+            raise ValueError(message)
+        target_dict: TargetDict = {"target_min": target_min, "target_max": target_max}
         return target_dict
```

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/optimization/plot_mixin.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/plot_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/optimization/read_goals.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/optimization/read_goals.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/plotting/plot_tools.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/plot_tools.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/plotting/subplot_classes.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/plotting/subplot_classes.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/simulation/base_simulation_problem.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/base_simulation_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/simulation/plot_mixin.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/simulation/plot_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/utils/plot_table_schema.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/plot_table_schema.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/utils/read_goals_mixin.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/read_goals_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/utils/read_plot_table.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/read_plot_table.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/utils/results_collection.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/results_collection.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/utils/serialization.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/rtctools_interface/utils/type_definitions.py` & `rtc-tools-interface-0.8.0b1/rtctools_interface/utils/type_definitions.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/tests/optimization/test_base_optimization_problem.py` & `rtc-tools-interface-0.8.0b1/tests/optimization/test_base_optimization_problem.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Tests for the base optimization problem class."""
 import unittest
 
 from rtctools_interface.optimization.base_optimization_problem import BaseOptimizationProblem
 from tests.utils.get_test import get_test_data
 
 
-
 class TestBaseOptimizationProblem(unittest.TestCase):
     """Test for the base optimization problem class."""
+
     def run_test(self, test):
         """Solve an optimization problem."""
         test_data = get_test_data(test, optimization=True)
         problem = BaseOptimizationProblem(
             goal_table_file=test_data["goals_file"],
             model_folder=test_data["model_folder"],
             model_name=test_data["model_name"],
```

### Comparing `rtc-tools-interface-0.7.6/tests/optimization/test_passing_goals_directly.py` & `rtc-tools-interface-0.8.0b1/tests/optimization/test_passing_goals_directly.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/tests/optimization/test_plot_goals_mixin.py` & `rtc-tools-interface-0.8.0b1/tests/optimization/test_plot_goals_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/tests/simulation/test_base_simulation_problem.py` & `rtc-tools-interface-0.8.0b1/tests/simulation/test_base_simulation_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/tests/simulation/test_plot_mixin.py` & `rtc-tools-interface-0.8.0b1/tests/simulation/test_plot_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/tests/utils/get_test.py` & `rtc-tools-interface-0.8.0b1/tests/utils/get_test.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.6/versioneer.py` & `rtc-tools-interface-0.8.0b1/versioneer.py`

 * *Files identical despite different names*

