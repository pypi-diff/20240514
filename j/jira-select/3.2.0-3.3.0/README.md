# Comparing `tmp/jira-select-3.2.0.tar.gz` & `tmp/jira-select-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira-select-3.2.0.tar", last modified: Wed Aug 16 00:57:00 2023, max compression
+gzip compressed data, was "jira-select-3.3.0.tar", last modified: Tue May 14 15:37:23 2024, max compression
```

## Comparing `jira-select-3.2.0.tar` & `jira-select-3.3.0.tar`

### file list

```diff
@@ -1,145 +1,122 @@
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.931919 jira-select-3.2.0/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      574 2023-08-16 00:56:50.000000 jira-select-3.2.0/.bumpversion.cfg
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1097 2023-03-04 07:50:34.000000 jira-select-3.2.0/.pre-commit-config.yaml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-26 21:00:29.000000 jira-select-3.2.0/MANIFEST.in
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3982 2023-08-16 00:57:00.931919 jira-select-3.2.0/PKG-INFO
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.911919 jira-select-3.2.0/docs/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      580 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/Makefile
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.903919 jira-select-3.2.0/docs/_build/
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.903919 jira-select-3.2.0/docs/_build/html/
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.915919 jira-select-3.2.0/docs/_build/html/_sources/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      104 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/api_documentation.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      116 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/appendix.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     7463 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/commands.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6018 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/examples.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3550 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/extending.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    16413 2023-03-04 03:10:17.000000 jira-select-3.2.0/docs/_build/html/_sources/functions.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4095 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/how_to.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1741 2023-03-04 06:42:17.000000 jira-select-3.2.0/docs/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      829 2023-03-04 07:50:34.000000 jira-select-3.2.0/docs/_build/html/_sources/parameters.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10703 2023-03-04 06:39:28.000000 jira-select-3.2.0/docs/_build/html/_sources/query.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1110 2023-03-05 04:20:36.000000 jira-select-3.2.0/docs/_build/html/_sources/query_lifecycle.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      956 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/quickstart.rst.txt
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.919919 jira-select-3.2.0/docs/_build/html/_sources/source/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1658 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/source/jira_select.commands.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      903 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/source/jira_select.formatters.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1192 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/source/jira_select.functions.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1343 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/source/jira_select.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       88 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/source/modules.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      103 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/source/setup.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      559 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/source/tests.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4099 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/_build/html/_sources/troubleshooting.rst.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      104 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/api_documentation.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       99 2023-04-12 19:20:42.000000 jira-select-3.2.0/docs/appendix.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     7463 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/commands.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5463 2023-08-16 00:56:50.000000 jira-select-3.2.0/docs/conf.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1028 2023-04-13 02:48:26.000000 jira-select-3.2.0/docs/evaluation_location.csv
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6051 2023-04-11 04:23:44.000000 jira-select-3.2.0/docs/examples.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3550 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/extending.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    22460 2023-08-16 00:55:28.000000 jira-select-3.2.0/docs/functions.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4124 2023-04-11 04:23:39.000000 jira-select-3.2.0/docs/how_to.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1758 2023-04-12 19:20:56.000000 jira-select-3.2.0/docs/index.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      787 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/make.bat
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      840 2023-04-11 04:20:52.000000 jira-select-3.2.0/docs/parameters.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    12629 2023-04-11 05:08:47.000000 jira-select-3.2.0/docs/query.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1171 2023-04-11 05:01:21.000000 jira-select-3.2.0/docs/query_lifecycle.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      956 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/quickstart.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       53 2023-03-05 04:28:37.000000 jira-select-3.2.0/docs/requirements.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      131 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/run.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.919919 jira-select-3.2.0/docs/source/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1658 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/source/jira_select.commands.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1240 2023-04-09 01:20:37.000000 jira-select-3.2.0/docs/source/jira_select.formatters.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1192 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/source/jira_select.functions.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1343 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/source/jira_select.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       88 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/source/modules.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      103 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/source/setup.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      559 2022-05-20 02:53:24.000000 jira-select-3.2.0/docs/source/tests.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4136 2023-04-12 04:16:44.000000 jira-select-3.2.0/docs/troubleshooting.rst
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.923919 jira-select-3.2.0/jira_select/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       22 2023-08-16 00:56:50.000000 jira-select-3.2.0/jira_select/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       98 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/__main__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4180 2023-03-04 07:50:34.000000 jira-select-3.2.0/jira_select/cache.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4595 2023-04-10 16:55:25.000000 jira-select-3.2.0/jira_select/cmdline.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.923919 jira-select-3.2.0/jira_select/commands/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/commands/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1815 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/commands/build_query.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3473 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/commands/configure.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4371 2023-04-09 01:41:06.000000 jira-select-3.2.0/jira_select/commands/functions.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2971 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/commands/install_user_script.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      411 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/commands/remove_instance.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4181 2023-04-10 03:27:31.000000 jira-select-3.2.0/jira_select/commands/run.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      899 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/commands/run_script.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4031 2023-04-09 01:41:06.000000 jira-select-3.2.0/jira_select/commands/schema.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2706 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/commands/setup_instance.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6891 2023-04-09 01:20:37.000000 jira-select-3.2.0/jira_select/commands/shell.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1687 2023-04-09 01:41:06.000000 jira-select-3.2.0/jira_select/commands/show_instances.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      759 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/commands/store_password.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      442 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/constants.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      343 2023-03-04 07:50:34.000000 jira-select-3.2.0/jira_select/exceptions.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.927919 jira-select-3.2.0/jira_select/formatters/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/formatters/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      974 2023-04-09 01:20:37.000000 jira-select-3.2.0/jira_select/formatters/csv.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1895 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/formatters/html.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      706 2023-04-09 01:40:24.000000 jira-select-3.2.0/jira_select/formatters/json.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      386 2023-04-12 03:52:31.000000 jira-select-3.2.0/jira_select/formatters/raw.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1061 2023-01-26 02:12:26.000000 jira-select-3.2.0/jira_select/formatters/table.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      176 2023-04-09 01:20:37.000000 jira-select-3.2.0/jira_select/formatters/tsv.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.927919 jira-select-3.2.0/jira_select/functions/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/functions/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      944 2023-03-24 16:42:35.000000 jira-select-3.2.0/jira_select/functions/estimate_to_days.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1010 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/functions/extract.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1085 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/functions/field_by_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1833 2023-04-09 01:20:37.000000 jira-select-3.2.0/jira_select/functions/flatten_changelog.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      261 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/functions/flatten_list.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      427 2023-04-11 05:23:23.000000 jira-select-3.2.0/jira_select/functions/get_issue.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3339 2023-04-12 02:18:27.000000 jira-select-3.2.0/jira_select/functions/get_issue_snapshot_on_date.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      998 2023-08-16 00:56:32.000000 jira-select-3.2.0/jira_select/functions/get_linked_issue_keys.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      788 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/functions/get_sprint_by_id.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3371 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/functions/get_sprint_by_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2010 2023-04-11 05:15:10.000000 jira-select-3.2.0/jira_select/functions/interval_business_hours.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      859 2023-04-12 01:44:30.000000 jira-select-3.2.0/jira_select/functions/interval_matching.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      578 2023-04-10 23:51:45.000000 jira-select-3.2.0/jira_select/functions/interval_size.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      366 2023-04-09 01:37:57.000000 jira-select-3.2.0/jira_select/functions/json_dumps.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      408 2023-06-02 01:43:27.000000 jira-select-3.2.0/jira_select/functions/now.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      628 2023-03-04 07:50:34.000000 jira-select-3.2.0/jira_select/functions/parse_date.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      776 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/functions/parse_datetime.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      718 2023-04-09 01:20:37.000000 jira-select-3.2.0/jira_select/functions/simple_filter.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      592 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/functions/simple_filter_any.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2834 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/functions/sprint_details.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      473 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/functions/sprint_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1574 2023-04-12 03:38:13.000000 jira-select-3.2.0/jira_select/functions/subquery.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-10 04:56:24.000000 jira-select-3.2.0/jira_select/functions/union.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3454 2023-04-10 15:58:21.000000 jira-select-3.2.0/jira_select/functions/workdays_in_state.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10204 2023-06-02 01:42:06.000000 jira-select-3.2.0/jira_select/plugin.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    23290 2023-04-13 02:51:26.000000 jira-select-3.2.0/jira_select/query.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.931919 jira-select-3.2.0/jira_select/sources/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.2.0/jira_select/sources/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2300 2023-03-04 07:50:34.000000 jira-select-3.2.0/jira_select/sources/boards.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3983 2023-04-12 03:22:28.000000 jira-select-3.2.0/jira_select/sources/issues.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3576 2023-03-04 07:50:34.000000 jira-select-3.2.0/jira_select/sources/sprints.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2254 2023-04-12 02:50:17.000000 jira-select-3.2.0/jira_select/types.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10705 2023-05-14 23:28:09.000000 jira-select-3.2.0/jira_select/utils.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.923919 jira-select-3.2.0/jira_select.egg-info/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3982 2023-08-16 00:57:00.000000 jira-select-3.2.0/jira_select.egg-info/PKG-INFO
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4124 2023-08-16 00:57:00.000000 jira-select-3.2.0/jira_select.egg-info/SOURCES.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2023-08-16 00:57:00.000000 jira-select-3.2.0/jira_select.egg-info/dependency_links.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2712 2023-08-16 00:57:00.000000 jira-select-3.2.0/jira_select.egg-info/entry_points.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2022-09-19 22:12:27.000000 jira-select-3.2.0/jira_select.egg-info/not-zip-safe
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2023-08-16 00:57:00.000000 jira-select-3.2.0/jira_select.egg-info/requires.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       18 2023-08-16 00:57:00.000000 jira-select-3.2.0/jira_select.egg-info/top_level.txt
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.931919 jira-select-3.2.0/pyinstaller/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      829 2022-05-20 02:53:24.000000 jira-select-3.2.0/pyinstaller/Makefile
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2965 2022-05-20 02:53:24.000000 jira-select-3.2.0/pyinstaller/jira_select.exe.spec
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3160 2022-05-20 02:53:24.000000 jira-select-3.2.0/pyinstaller/jira_select.spec
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      163 2022-05-20 02:53:24.000000 jira-select-3.2.0/pyinstaller/requirements.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2843 2023-04-11 04:15:47.000000 jira-select-3.2.0/readme.md
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2023-08-15 17:47:38.000000 jira-select-3.2.0/requirements.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      775 2023-08-16 00:57:00.931919 jira-select-3.2.0/setup.cfg
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5863 2023-08-16 00:56:50.000000 jira-select-3.2.0/setup.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-08-16 00:57:00.931919 jira-select-3.2.0/tests/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.2.0/tests/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      892 2022-05-20 02:53:24.000000 jira-select-3.2.0/tests/base.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2022-05-20 02:53:24.000000 jira-select-3.2.0/tests/conftest.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10342 2023-04-11 05:12:36.000000 jira-select-3.2.0/tests/test_functions.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    13320 2023-04-11 05:12:47.000000 jira-select-3.2.0/tests/test_query.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6901 2023-04-11 05:12:28.000000 jira-select-3.2.0/tests/test_utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:37:23.307830 jira-select-3.3.0/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      574 2024-05-14 15:36:56.000000 jira-select-3.3.0/.bumpversion.cfg
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1097 2024-05-14 15:29:54.000000 jira-select-3.3.0/.pre-commit-config.yaml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2024-05-14 15:29:54.000000 jira-select-3.3.0/MANIFEST.in
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4002 2024-05-14 15:37:23.307830 jira-select-3.3.0/PKG-INFO
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:37:23.299830 jira-select-3.3.0/docs/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      580 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/Makefile
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      104 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/api_documentation.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       99 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/appendix.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     7463 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/commands.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5463 2024-05-14 15:36:56.000000 jira-select-3.3.0/docs/conf.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1028 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/evaluation_location.csv
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6051 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/examples.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3550 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/extending.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    22460 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/functions.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4124 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/how_to.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1758 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/index.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      787 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/make.bat
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      840 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/parameters.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    12629 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/query.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1171 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/query_lifecycle.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      956 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/quickstart.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       53 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/requirements.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      131 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/run.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:37:23.299830 jira-select-3.3.0/docs/source/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1658 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/source/jira_select.commands.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1240 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/source/jira_select.formatters.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1192 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/source/jira_select.functions.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1343 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/source/jira_select.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       88 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/source/modules.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      103 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/source/setup.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      559 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/source/tests.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4136 2024-05-14 15:29:54.000000 jira-select-3.3.0/docs/troubleshooting.rst
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:37:23.299830 jira-select-3.3.0/jira_select/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       22 2024-05-14 15:36:56.000000 jira-select-3.3.0/jira_select/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       98 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/__main__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4180 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/cache.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4595 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/cmdline.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:37:23.303830 jira-select-3.3.0/jira_select/commands/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4210 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/batch.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1815 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/build_query.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3473 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/configure.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4371 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/functions.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2971 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/install_user_script.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      411 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/remove_instance.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4181 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/run.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      899 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/run_script.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4031 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/schema.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2706 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/setup_instance.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6891 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/shell.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1687 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/show_instances.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      759 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/commands/store_password.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      442 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/constants.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      343 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/exceptions.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:37:23.303830 jira-select-3.3.0/jira_select/formatters/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/formatters/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      974 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/formatters/csv.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1895 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/formatters/html.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      706 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/formatters/json.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      386 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/formatters/raw.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1061 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/formatters/table.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      176 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/formatters/tsv.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:37:23.307830 jira-select-3.3.0/jira_select/functions/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      944 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/estimate_to_days.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1010 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/extract.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1085 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/field_by_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1833 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/flatten_changelog.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      261 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/flatten_list.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      427 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/get_issue.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3339 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/get_issue_snapshot_on_date.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      998 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/get_linked_issue_keys.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      788 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/get_sprint_by_id.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3371 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/get_sprint_by_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2010 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/interval_business_hours.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      859 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/interval_matching.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      578 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/interval_size.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      366 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/json_dumps.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      408 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/now.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      628 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/parse_date.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      776 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/parse_datetime.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      718 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/simple_filter.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      592 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/simple_filter_any.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2834 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/sprint_details.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      473 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/sprint_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1574 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/subquery.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/union.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3454 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/functions/workdays_in_state.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10184 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/plugin.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    23331 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/query.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:37:23.307830 jira-select-3.3.0/jira_select/sources/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/sources/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2300 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/sources/boards.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3983 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/sources/issues.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3576 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/sources/sprints.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2254 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/types.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10767 2024-05-14 15:29:54.000000 jira-select-3.3.0/jira_select/utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:37:23.303830 jira-select-3.3.0/jira_select.egg-info/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4002 2024-05-14 15:37:23.000000 jira-select-3.3.0/jira_select.egg-info/PKG-INFO
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3189 2024-05-14 15:37:23.000000 jira-select-3.3.0/jira_select.egg-info/SOURCES.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2024-05-14 15:37:23.000000 jira-select-3.3.0/jira_select.egg-info/dependency_links.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2756 2024-05-14 15:37:23.000000 jira-select-3.3.0/jira_select.egg-info/entry_points.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2024-05-14 15:37:23.000000 jira-select-3.3.0/jira_select.egg-info/not-zip-safe
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2024-05-14 15:37:23.000000 jira-select-3.3.0/jira_select.egg-info/requires.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       18 2024-05-14 15:37:23.000000 jira-select-3.3.0/jira_select.egg-info/top_level.txt
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:37:23.307830 jira-select-3.3.0/pyinstaller/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      829 2024-05-14 15:29:54.000000 jira-select-3.3.0/pyinstaller/Makefile
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2965 2024-05-14 15:29:54.000000 jira-select-3.3.0/pyinstaller/jira_select.exe.spec
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3160 2024-05-14 15:29:54.000000 jira-select-3.3.0/pyinstaller/jira_select.spec
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      163 2024-05-14 15:29:54.000000 jira-select-3.3.0/pyinstaller/requirements.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2843 2024-05-14 15:29:54.000000 jira-select-3.3.0/readme.md
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2024-05-14 15:29:54.000000 jira-select-3.3.0/requirements.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      782 2024-05-14 15:37:23.311830 jira-select-3.3.0/setup.cfg
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5921 2024-05-14 15:36:56.000000 jira-select-3.3.0/setup.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:37:23.307830 jira-select-3.3.0/tests/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2024-05-14 15:29:54.000000 jira-select-3.3.0/tests/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      892 2024-05-14 15:29:54.000000 jira-select-3.3.0/tests/base.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2024-05-14 15:29:54.000000 jira-select-3.3.0/tests/conftest.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10342 2024-05-14 15:29:54.000000 jira-select-3.3.0/tests/test_functions.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    13320 2024-05-14 15:29:54.000000 jira-select-3.3.0/tests/test_query.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6901 2024-05-14 15:29:54.000000 jira-select-3.3.0/tests/test_utils.py
```

### Comparing `jira-select-3.2.0/.bumpversion.cfg` & `jira-select-3.3.0/.bumpversion.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.2.0
+current_version = 3.3.0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>.*))?
 serialize = 
 	{major}.{minor}.{patch}.{release}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
```

### Comparing `jira-select-3.2.0/.pre-commit-config.yaml` & `jira-select-3.3.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,23 @@
       - id: debug-statements
   - repo: https://github.com/timothycrosley/isort
     rev: 5.12.0
     hooks:
       - id: isort
         args: ["--profile", "black", "--filter-files"]
   - repo: https://github.com/ambv/black
-    rev: 22.8.0
+    rev: 24.1.1
     hooks:
       - id: black
   - repo: https://gitlab.com/pycqa/flake8
     rev: 3.9.2
     hooks:
       - id: flake8
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.910
+    rev: v1.9.0
     hooks:
       - id: mypy
         args:
           - --pretty
           - --show-error-codes
           - --show-error-context
           - --ignore-missing-imports
```

### Comparing `jira-select-3.2.0/PKG-INFO` & `jira-select-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: jira-select
-Version: 3.2.0
+Version: 3.3.0
 Summary: Easily run complex SQL-like queries far beyond what Jira's standard JQL query language can provide.
 Home-page: https://github.com/coddingtonbear/jira-select
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
 Project-URL: Issue Tracker, https://github.com/coddingtonbear/jira-select/issues
 Keywords: jira,csv,sql
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
@@ -110,7 +111,9 @@
 your query, press `Esc` followed by `Enter` and after a short wait (watch the progressbars), you'll be shown your results. Press `q` to exit your results.
 
 ---
 
 - Documentation for Jira-select is available on [ReadTheDocs](http://jira-select.readthedocs.org/).
 - Please post issues on [Github](http://github.com/coddingtonbear/jira-select/issues).
 - Questions? Ask them on [Gitter](https://gitter.im/coddingtonbear/jira-select).
+
+
```

### Comparing `jira-select-3.2.0/docs/Makefile` & `jira-select-3.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/commands.rst.txt` & `jira-select-3.3.0/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/examples.rst.txt` & `jira-select-3.3.0/docs/examples.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 ========
 
 Finding all issues assigned to a particular user
 ------------------------------------------------
 
 .. code-block:: yaml
 
-   select:
-   - "*"
+   select: "*"
    from: issues
    where:
    - assignee = "some-user@some-company.com"
 
 
 Summing the number of story points assigned in a particular sprint
 ------------------------------------------------------------------
 
 .. code-block:: yaml
 
    select:
-   - sum({Story Points}) as "Total Story Points"
+     Total Story Points: sum({Story Points})
    from: issues
    where:
    - project = "MYPROJECT"
    group_by:
    - True
    having:
    - '"My Sprint Name" in sprint_name({Sprint}[-1])'
@@ -58,16 +57,16 @@
 
 Summing the total estimated size of issues per-person for a given sprint
 ------------------------------------------------------------------------
 
 .. code-block:: yaml
 
    select:
-   - assignee
-   - sum(map(estimate_to_days, timeestimate.originalEstimate))
+     Assignee: assignee
+     Total Size: sum(map(estimate_to_days, timeestimate.originalEstimate))
    from: issues
    where:
    - project = "MYPROJECT"
    group_by:
    - assignee
    having:
    - '"My Sprint Name" in sprint_name({Sprint}[-1])'
@@ -99,16 +98,16 @@
 
 Summing story points of issues resolved during a particular sprint
 ------------------------------------------------------------------
 
 .. code-block:: yaml
 
    select:
-   - assignee
-   - sum({Story Points})
+     Assignee: assignee
+     Story Points: sum({Story Points})
    from: issues
    where:
    - project = 'My Project'
    filter:
    - simple_filter(
        flatten_changelog(changelog),
        created__gt=parse_datetime(get_sprint_by_name("Board Name", "Sprint Name").startDate),
@@ -137,15 +136,15 @@
 
 Summing worklog entries
 -----------------------
 
 .. code-block:: yaml
 
    select:
-   - sum(extract(flatten_list(worklogs.worklogs), "timespentSeconds")) as "total seconds"
+     Total Seconds: sum(extract(flatten_list(worklogs.worklogs), "timespentSeconds"))
    from: issues
    group_by:
    - True
 
 Worklog entries on issues are shaped like this for every row
 (unnecessary fields omitted)::
```

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/extending.rst.txt` & `jira-select-3.3.0/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/functions.rst.txt` & `jira-select-3.3.0/docs/functions.rst`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,55 @@
 
 Jira-select provides a long list of functions out-of-the-box, and you can
 add your own if these are not enough.
 
 Jira
 ----
 
+.. py:function:: get_issue(ticket_number: str) -> jira.resources.Issue
+
+   Fetch a Jira issue by its issue key (e.g. ``MYPROJECT-1045``).
+
+   This will return a ``jira.resources.Issue`` object; you can access
+   most fields via its ``fields`` property, eg::
+
+      get_issue(field_holding_issue_key).fields.summary
+
+.. py:function:: get_issue_snapshot_on_date(issue: jira.resources.Issue) -> jira_select.types.IssueSnapshot:
+
+   Reconstruct the state of an issue at a particular point in time
+   using the issue's ``changelog``.
+
+   You will want to pass the literal value ``issue`` as the first parameter of this function.
+   Jira-select provides the ``jira.resources.Issue`` object itself under that name,
+   and this function will use both that object and the changes recorded in the ``changelog`` field
+   for getting an understanding of what the issue looked liked at a particular point in time.
+
+   This function requires that you set the query ``expand`` option
+   such that it includes ``changelog`` for this to work correctly --
+   if you do not do that, this function will fail.
+
+   .. code-block:: yaml
+
+      select:
+        snapshot: get_issue_snapshot_on_date(issue, parse_datetime('2022-01-01'))
+      from: issues
+      expand:
+      - changelog
+
+   The returned snapshot is *not* a ``jira.resources.Issue`` object,
+   but instead a ``jira_select.types.IssueSnapshot`` object
+   due to limitations around what kinds of data can be gathered
+   from the snapshot information.
+   The most important difference between a ``jira_select.types.IssueSnapshot`` and a ``jira.resources.Issue`` object is
+   that the ``jira_select.types.IssueSnapshot`` object is
+   a simple ``dict[str,str]`` object in which
+   the value of the ``dict`` entries is always the ``str``-ified
+   field value.
+
 .. py:function:: sprint_name(sprint_blob: str) -> Optional[str]
 
    Shortcut for returning the name of a sprint via its ID.  Equivalent
    to calling ``sprint_details(sprint_blob).name``.
 
 .. py:function:: sprint_details(sprint_blob: str) -> Optional[jira_select.functions.sprint_details.SprintInfo]
 
@@ -56,34 +97,34 @@
       the value of a field by its human-readable name--
       just place the human-readable name in between
       curly braces in your query expression; eg:
 
       .. code-block::
 
          select
-           - {Story Points} as "Story Points"
+           Story Points: "{Story Points}"
          from: issues
 
    .. note::
 
-      You will almost certainly want to provide the parameter named ``_``
-      (an underscore) as the first argument to this function.
+      You will almost certainly want to provide the parameter named
+      ``issue`` as the first argument to this function.
       Jira-select provides the raw row data to functions under this variable name.
 
    In Jira, custom fields are usually named something like ``customfield_10024``
    which is, for most people, somewhat difficult to remember.  You can use
    this function to get the field value for a field by its display name instead
    of its ID.
 
    Example:
 
    .. code-block:: yaml
 
       select
-        - field_by_name(_, "Story Points") as "Story Points"
+        - field_by_name(issue, "Story Points") as "Story Points"
       from: issues
 
 .. py:function:: estimate_to_days(estimate_string: str, day_hour_count=8) -> Optional[float]
 
    Converts a string estimation (typically stored in ``timetracking.originalEstimate``)
    into an integer count of days.
 
@@ -100,15 +141,15 @@
 
       You must use the ``expand`` option of ``changelog`` for Jira to
       return to you changelog information in your query; eg:
 
       .. code-block:: yaml
 
          select:
-         - flatten_changelog(changelog)
+           changelog: flatten_changelog(changelog)
          from: issues
          expand:
          - changelog
 
       If you do not provide the necessary ``expand`` option, this
       function will raise an error.
 
@@ -128,98 +169,172 @@
    * ``toString`` (Optional[str]): The final value of the field as a
      string.
 
    This returned list of records can be filtered with ``simple_filter``
    to either find particular entries or filter out rows that do not
    have an entry having particular characteristics.
 
+.. py:function:: get_linked_issue_keys(issue: jira.resources.Issue, link_type: str | None = None) -> list[str]:
+
+   Return a list of issue keys that are related to the relevant issue via the specified relation type (e.g. ``causes``, ``is associated with``, etc.).
+
+   You will want to pass the literal value ``issuelinks`` as the first parameter of this function.  This will provide this function with the list of issuelinks your issue has.
+
+   If ``link_type`` is unspecified, all related issue keys will be returned.
+
+   For example, to find the keys for all issues that were caused by a particular issue, you could run the following query:
+
+   .. code-block:: yaml
+
+      select:
+        caused_bugs: get_linked_issue_keys(issuelinks, 'causes')
+      from: issues
+      where:
+      - type = 'Bug'
+
+Subquery
+--------
+
+.. py:function:: subquery(subquery_name, **params) -> Any:
+
+   Runs a subquery by name with the provided parameters.
+
+   For example: you can get the time intervals during which an issue
+   and its associated subtasks were in the "In Progress" status with
+   a query like so:
+
+   .. code-block:: yaml
+
+      select:
+        self_and_child_intervals_in_progress: interval_matching(issue, status="In Progress") | union(subquery("children", key=issue.key))
+      from: issues
+      subqueries:
+         children:
+            select:
+              in_progress_intervals: interval_matching(issue, status='In Progress')
+            from: issues
+            where:
+            - parent = "{params.key}"
+            expand:
+            - changelog
+      expand:
+      - changelog
+
+   Your specified ``**params`` will become available to the subquery via ``{params.*}``;
+   in the above example, ``{params.key}`` will be set to the value of the outer query's
+   ``issue.key``.
+
+   Unless specifically specified,
+   a subquery will use the same cache settings as the parent query.
+
+   .. warning::
+
+      If you would like your subquery's cache to be effective,
+      only pass simple values in ``**params``.
+
+      The string representation of an object is used for calculating cache
+      keys, and many objects include information in their default
+      string representations that vary between instantiations.
+      If things like, for example, the memory address of an object appears in
+      its string representation, the cache key will never match,
+      and the cached value will not be used.
+
+      A common way that this problem might occur is if you were to pass the
+      entire ``issue`` object to the subquery.
+      Instead of passing the entire ``issue`` object to the subquery,
+      pass simple values from it as shown in the example above.
 
 Time Analysis
 -------------
 
-.. py:function:: workdays_in_state(changelog, state: str, start_hour: int = 9, end_hour: int = 17, timezone_name: str | None \ None, work_days: list[int] = [1, 2, 3, 4, 5], min_date: datetime.date = datetime.date(1, 1, 1), max_date: datetime.date = datetime.date(9999, 1, 1)) -> float
+.. py:function:: interval_matching(issue, **query_params: dict[str, Any]) -> portion.Interval
 
-   Calculates how many "work days" your returned Jira issue was in a given state
-   during the time period specified.
+   See `simple_filter function` for information about how to specify ``query_params``.
 
-   As we all know, it's very difficult to get an actual understanding of how much
-   time a given assignee has spent working on a given issue without asking them to
-   track it directly, but this function intends to get us at least a reasonably
-   good understanding of that by making some imperfect generalizations.
+   Will return an interval covering segments in which the provided issue
+   matches the conditions specified by ``query_params``.
 
    .. note::
 
-      A naive implementation of this function might use actual clock time, but
-      consider the following two situations:
+      Contrary to what you might guess,
+      a single `portion.Interval` object
+      can represnt multiple ranges of time.
+
+   Note that `portion.Interval` objects can be used with logical operations like `|`, `&`, and `-`.
+
+.. py:function:: interval_size(interval: portion.Interval) -> datetime.timedelta
+
+   For a provided interval, return the total amount of time that the interval's
+   segments span.
+
+.. py:function:: interval_business_hours(min_date: datetime.date | None = None, max_date: datetime.date | None = None, start_hour: int = 9, end_hour: int = 17, timezone_name: str | None = None, work_days: Iterable[int] = (1, 2, 3, 4, 5)) -> portion.Interval:
+
+   Returns an interval having segments that correspond with the "business hours"
+   specified by your paramters.
+
+   This is particularly useful when used in conjunction with `interval_matching`
+   and `interval_size` above for determining the amount of time an issue was
+   actively in a particular state, for example:
+
+   .. code-block:: yaml
+
+      select:
+        total_time_in_progress: interval_size(interval_matching(issue, status="In Progress") & interval_business_hours(parse_date(created)))
+      from: issues
+
+   This will find all segments of time during which the relevant issue was
+   in the "In Progress" status during business hours, then return the
+   amount of time that those segments spanned.
+
+   .. note::
+
+      A naive implementation of this sort of time analysis might use actual,
+      raw clock time, but consider the following two situations:
 
       - MYPROJECT-01 moves from "To Do" into "In Progress" at 4:55PM, just
         five minutes before the end of the day, then the next day moves
         from "In Progress" into "Done" at 9:05AM, five minutes after the
         beginning of the next day.
       - MYPROJECT-02 moves from "To Do" into "In Progress" at 10:00AM and
         in the same day from "In Progress" into "Done" at 4:00PM.
 
       Clearly, MYPROJECT-02 was being "worked on" for more time than
       MYPROJECT-01, but let's see how various algorithms might measure
       that time.
 
-      If we use clock time:
+      If we use raw clock time:
 
       - MYPROJECT-01: 16.2h (81 times more than the actual working time)
       - MYPROJECT-02: 6h
 
       If we only measure time happening between 9A and 5P:
 
       - MYPROJECT-01: 0.2h (the actual working time)
       - MYPROJECT-02: 6h (the actual working time)
 
-      Of course, this does introduce one inaccuracy that may, depending on
-      how predicable your team's working hours are: time spent working on
-      an issue outside of business hours isn't counted.
-
-      If you would like to instead use clock time even knowing the
-      distortions using that may create, you can do so by specifying
-      a ``start_hour`` and ``end_hour`` of ``None``.
-
-   .. note::
-
-      You must use the ``expand`` option of ``changelog`` for Jira to
-      return to you changelog information in your query; eg:
-
-      .. code-block:: yaml
-
-         select:
-         - flatten_changelog(changelog)
-         from: issues
-         expand:
-         - changelog
-
-      If you do not provide the necessary ``expand`` option, this
-      function will raise an error.
-
-   Parameters:
-
-   - ``state``: The name of the state you would like to count time for
-     (e.g. "In Progress")
+      Of course, this does introduce one inaccuracy that may,
+      depending on how predicable your team's working hours are,
+      make this behavior undesirable:
+      time spent working on an issue outside of business hours isn't counted.
+      Typically, though,
+      the amount of time an issue might be worked on outside those hours
+      will be much smaller
+      than the amount of excess time
+      using raw clock time directly would count.
+
+   - ``min_date``: The minimum date to add the business hours of to your interval.
+     By default, 365 days before now.
+   - ``max_date``: The (exclusive) maximum date to add the business hours of to
+     your interval.  By default: tomorrow.
    - ``start_hour``: The work day starting hour.  Defaults to 9 (i.e. 9 AM)
    - ``end_hour``: The work day ending hour.  Defaults to 17 (i.e 5 PM)
    - ``timezone_name``: The timezone to interpret ``start_hour`` and
      ``end_hour`` in.
    - ``work_days``: The days of the week to count as work days; 0 = Sunday,
       1 = Monday... 6 = Saturday.
-   - ``min_date``: The minmimum date to use when processing changelog entries.
-     If an issue is in the relevant state at ``min_date`` at ``start_hour``,
-     ``min_date`` and ``start_hour`` will be used for calculating the time range
-     during which the issue was in the relevant state instead of using issue's
-     actual time range in that state.
-   - ``max_date``: The maximuim date to use when processing changelog entries.
-     If an issue is in the relevant state at ``max_date`` at ``end_hour``,
-     ``max_date`` and ``end_hour`` will be used for calculating the time range
-     during which the issue was in the relevant state instead of using issue's
-     actual time range in that state.
 
 Data Traversal
 --------------
 
 .. _extract function:
 
 .. py:function:: extract(field: Iterable[Any], dotpath: str) -> Iterable[Any]
@@ -253,28 +368,69 @@
    into a single list of the shape::
 
       [1, 2, 3, 4, 5, 6]
 
 Dates
 -----
 
+.. py:function:: now(**replacements) -> datetime.datetime
+
+   Return "now" as a timezone-aware ``datetime.datetime`` object.
+
+   Additional parameters can be passed via keyword arguments;
+   these values will be applied
+   to the ``datetime.datetime`` object
+   via its ``replace`` method.
+   See `Python's documentation <https://docs.python.org/3/library/datetime.html#datetime.datetime.replace>`_ for for more information .
+
+   If you would like to obtain a timezone-unaware datetime object,
+   pass ``tzinfo=None`` as a keyword argument.
+
+.. py:function:: timedelta(days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0) -> datetime.timedelta
+
+   Returns a ``datetime.timedelta`` object.
+
+   This object can be used in math
+   with existing ``datetime.datetime``objects.
+
+.. py:function:: datetime(year, month, day, hour=0, minute=0, second=0, microsecond=0, tzinfo=None, *, fold=0) -> datetime.datetime
+
+   Returns a ``datetime.datetime`` object.
+
+   To obtain a ``date`` object, call ``.date()`` on the return value
+   of this function.
+
 .. py:function:: parse_datetime(datetime_string: str, *args, **kwargs) -> datetime.datetime
 
    Parse a date string into a datetime object.
 
    This relies on `python-dateutil`; there are many additional options available
    that you can find documented `here <https://dateutil.readthedocs.io/en/stable/parser.html#dateutil.parser.parse>`_.
 
 .. py:function:: parse_date(date_string: str, *args, **kwargs) -> datetime.date
 
    Parse a date string into a date object.
 
    This relies on `python-dateutil`; there are many additional options available
    that you can find documented `here <https://dateutil.readthedocs.io/en/stable/parser.html#dateutil.parser.parse>`_.
 
+
+Intervals
+---------
+
+.. py:function:: empty_interval() -> portion.Interval
+
+.. py:function:: closed_interval() -> portion.Interval
+
+.. py:function:: open_interval() -> portion.Interval
+
+.. py:function:: openclosed_interval() -> portion.Interval
+
+.. py:function:: closedopen_interval() -> portion.Interval
+
 Json
 ----
 
 .. py:function:: json_loads(json: str) -> Union[Dict, List]
 
    Parse a JSON string.
 
@@ -360,14 +516,19 @@
 
 .. py:function:: hex(value: int) -> str
 
 .. py:function:: oct(value: int) -> str
 
 .. py:function:: ord(value: str) -> int
 
+List Operations
+---------------
+
+.. py:function:: union(iterable: Iterable[X]) -> X
+
 Types
 -----
 
 See more in information in `Python's Documentation <https://docs.python.org/3/library/functions.html>`_.
 
 .. py:function:: bool(value: Any) -> bool
 
@@ -390,14 +551,16 @@
 .. py:function:: reversed(iterable: List[Any]) -> Iterable[List[Any]]
 
 .. py:function:: sorted(iterable: List[Any]) -> Iterable[List[Any]]
 
 Filtering & Mapping
 -------------------
 
+.. _simple_filter function:
+
 .. py:function:: simple_filter(iterable: Iterable[Any], **query_params: Dict[str, Any]) -> Iterable[Any]
 .. py:function:: simple_filter_any(iterable: Iterable[Any], **query_params: Dict[str, Any]) -> Iterable[Any]
 
    These functions provide you with a simple way of filtering lists using
    a syntax reminiscent of Django's ORM query filter parameters.
 
    * ``simple_filter``: All provided ``query_params`` must match for the row
@@ -406,16 +569,15 @@
      must match for the row to be returned.
 
    For example; to find issues having become resolved between two dates,
    you could run a query like the following:
 
    .. code-block:: yaml
 
-      select:
-      - "*"
+      select: "*"
       from: issues
       filter:
       - simple_filter(
             flatten_changelog(changelog),
             field__eq="resolution",
             toValue__ne=None,
             created__lt=parse_datetime("2020-02-02"),
```

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/how_to.rst.txt` & `jira-select-3.3.0/docs/how_to.rst`

 * *Files 12% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 Format data using functions
 ---------------------------
 
 .. code-block:: yaml
 
    select:
-     - status
-     - summary
-     - customfield_10069 as "Story Points"
-     - len(customfield_10010) as "Sprint Count"
-     - sprint_name(customfield_10010[-1]) as "Sprint Name"
+     Status: status
+     Summary: summary
+     Story Points: "{Story Points}"
+     Spring Count: len(customfield_10010)
+     Sprint Name: sprint_name(customfield_10010[-1])
    from: issues
 
 In the above example, two of the displayed columns are processed with
 a function:
 
 - `Sprint Count`: Will render the number of array elements in the field
   containing the list of sprints in which this issue was present.
@@ -35,17 +35,17 @@
 
 Filter results using functions
 ------------------------------
 
 .. code-block:: yaml
 
    select:
-     - status as "Status"
-     - summary as "Summary"
-     - customfield_10069 as "Story Points"
+     Status: status
+     Summary: summary
+     Story Points: "{Story Points}"
    from: issues
    having:
      # The quoting below is required only because the first character of line
      # being a double-quote causes YAML parsers to parse the line differently
      - '"Sprint #19" in sprint_name(customfield_10010[-1])'
 
 In the above example, the issues returned from Jira will be compared against
@@ -65,16 +65,16 @@
 ------------------------------------
 
 You can group and/or aggregate your returned rows by using ``group_by``:
 
 .. code-block:: yaml
 
    select:
-     - status
-     - count(key)
+     Status: status
+     Count: count(key)
    from: issues
    group_by:
      - status
 
 You'll receive just a single result row for each status, and a count
 of how many records shared that status in the second column.
 
@@ -82,16 +82,16 @@
 ----------------------------
 
 You can order your entries using any expression, too:
 
 .. code-block:: yaml
 
    select:
-     - status
-     - count(key)
+     Status: status
+     Count: count(key)
    from: issues
    group_by:
      - status
    sort_by:
      - count(key) desc
 
 This will sort all returned tickets, grouped by status, in descending order
@@ -108,17 +108,17 @@
 ------------------------------------
 
 You can limit the number of results returned by adding a ``limit`` to your query:
 
 .. code-block:: yaml
 
    select:
-     - key
-     - status
-     - summary
+     Key: key
+     Status: status
+     Summary: summary
    from: issues
    where:
      - assignee = "me@adamcoddington.net"
    limit: 10
 
 Be aware that this limit is handled by Jira;
 so only the first N records will be available for downstream steps
@@ -128,16 +128,16 @@
 ------------------------
 
 You can ask Jira to expand issue fields by adding an ``expand`` element to your query:
 
 .. code-block:: yaml
 
    select:
-     - key
-     - status
-     - summary
+     Key: key
+     Status: status
+     Summary: summary
    from: issues
    expand:
      - transitions
 
 The meaning of these expansions is defined by Jira; you can find more information
 in `Jira's documentation <https://developer.atlassian.com/cloud/jira/platform/rest/v3/intro/#expansion>`_.
```

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/index.rst.txt` & `jira-select-3.3.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,18 @@
 
 .. toctree::
    :maxdepth: 3
    :caption: Contents:
 
    quickstart.rst
    query.rst
-   how_to.rst
    query_lifecycle.rst
+   functions.rst
    parameters.rst
+   how_to.rst
    examples.rst
    commands.rst
    extending.rst
    troubleshooting.rst
    appendix.rst
```

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/parameters.rst.txt` & `jira-select-3.3.0/docs/parameters.rst`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 the below query will require that you specify
 a query parameter ``project`` that will
 be used when interpreting the query.
 
 .. code-block:: yaml
 
    select:
-   - key
+     Issue Key: key
    from: issues
    where:
    - project = "{params.project}"
    - updated > "2023-01-01"
 
 .. note::
```

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/query.rst.txt` & `jira-select-3.3.0/docs/query.rst`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 but using section names inspired by SQL.
 
 Here's a simple example that will return all Jira issues assigned to you:
 
 .. code-block:: yaml
 
    select:
-   - key
-   - summary
+   - Issue Key: key
+   - Issue Summary: summary
    from: issues
    where:
    - assignee = "your-email@your-company.net"
 
-Here's a query that uses _all_ of the possible sections,
+Here's a query that uses many more of the possible sections,
 but know that in real life, you're very unlikely to use them all at once:
 
 .. code-block:: yaml
 
    select:
-   - assignee
-   - len(key)
+     My Assignee: assignee
+     Key Length: len(key)
    from: issues
    expand:
    - changelog
    where:
    - project = "MYPROJECT"
    order_by:
    - created
@@ -88,29 +88,69 @@
 Ubiquitous
 ----------
 
 ``select``
 ~~~~~~~~~~
 
 This section defines what data you would like to include in your report.
-It should be a list of fields you would like to include in your document,
-and *can* use custom functions (see :ref:`Query Functions` for options).
+It should be a dictionary mapping the column name with the expression
+you would like to display in that column.
+This section *can* use custom functions (see :ref:`Query Functions` for options).
 
-By default, the column will be named to match your field definition,
-but you can overide that by providing a name using the format ``EXPRESSION as "NAME"``::
+For example:
 
-    somefunction(my_field) as "My Field Name"
+.. code-block:: yaml
 
-If you would like to return *all* fields values,
-use the expression ``*`` in your search statement:
+   select:
+     My Field Name: somefunction(my_field)
+
+.. note::
+
+   This section supports a handful of formats
+   in addition to the one discussed here
+   that you may find in some documentation
+   or in other examples including:
+
+   You can specify columns as a list:
+
+   .. code-block:: yaml
+
+      select:
+      - somefunction(my_field) as "My Field Name"
+
+   You can specify a single column as a string:
+
+   .. code-block:: yaml
+
+      select: somefunction(my_field) as "My Field Name"
+
+   The above formats will be supported for the foreseeable future,
+   but the dictionary-based format discussed outside this box is the
+   preferred format for writing queries.
+
+As a shorthand, if you do not provide a value for your dictionary entry,
+the dictionary entry's name will be used as the expression for your column:
 
 .. code-block:: yaml
 
    select:
-   - "*"
+     issuetype:
+     key:
+     summary:
+   from: issues
+
+In the above example, the fields ``issuetype``, ``key``, and ``summary``
+will be displayed in columns matching their field name.
+
+If you would like to return *all* fields values,
+use the expression ``*`` as a stirng value to your `select` statement:
+
+.. code-block:: yaml
+
+   select: "*"
    from: issues
 
 .. important::
 
    Due to yaml parsing rules, the ``*`` expression must be quoted.
 
 ``from``
@@ -214,16 +254,16 @@
 
 For example; to count the number of issues by type that are assigned to you
 you could run the following query:
 
 .. code-block:: yaml
 
    select:
-   - issuetype
-   - len(key)
+     Issue Type: issuetype
+     Key Length: len(key)
    from: issues
    where:
    - assignee = "your-email@your-company.net"
    group_by:
    - issuetype
 
 .. Note::
@@ -242,15 +282,15 @@
 you can provide ``True`` in your ``group_by`` statement.
 This works because, for every row, ``True`` will evaluate to the same result
 causing all rows to be grouped together:
 
 .. code-block:: yaml
 
    select:
-   - len(key)
+     Key Length: len(key)
    from: issues
    where:
    - assignee = "your-email@your-company.net"
    group_by:
    - True
 
 You **can** use custom functions in this section.
@@ -259,14 +299,39 @@
 ~~~~~~~~~~
 
 This section is where you can provide filtering instructions that Jql cannot handle
 because they either require local functions or operate on grouped data.
 
 You **can** use custom functions in this section.
 
+``calculate``
+~~~~~~~~~~~~~
+
+Perhaps you have an expression you'd like to calculate once
+and use multiple times across your query
+(e.g. multiple times across ``select`` columns,
+or in both ``select`` and ``filter`` at the same time).
+You can use the ``calculate`` section for performing those calculations
+once and then referencing their result in other expressions; for example:
+
+.. code-block:: yaml
+
+   select:
+     Hours in Progress: round(in_progress_seconds / 3600)
+   calculate:
+     in_progress_seconds: interval_size(interval_matching(issue, status="In Progress") & interval_business_hours(parse_date(created))).total_seconds() / 28800
+   from: issues
+   filter:
+   - in_progress_seconds > 60
+   expand:
+   - changelog
+
+The above example will calculate the total amount of time issues were in progress
+in hours while excluding results where they were in progress for fewer than sixty seconds.
+
 ``sort_by``
 ~~~~~~~~~~~
 
 This section is where you can provide sorting instructions that Jql cannot handle
 because they either require local functions or operate on grouped data.
 
 You **can** use custom functions in this section.
```

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/query_lifecycle.rst.txt` & `jira-select-3.3.0/docs/query_lifecycle.rst`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,16 @@
      subgraph Cacheable
        subgraph Remote
            where-->order_by
            order_by-->limit
        end
      end
      subgraph Local
-       limit-->filt[filter]
+       limit-->calculate
+       calculate-->filt[filter]
        filt[filter]-->group_by
        group_by-->having
        having-->sort_by
        sort_by-->cap
        cap-->select
      end
      result([Display])
@@ -27,14 +28,15 @@
 
 * Remote
 
   * JQL Query (``where``, ``order_by``, and ``limit``)
 
 * Local
 
+  * Calculating (``calculate``)
   * Filtering (``filter``)
   * Grouping (``group_by``)
   * Filtering (``having``)
   * Sorting (``sort_by``)
   * Capping count of results (``cap``)
   * Rendering results (``select``)
```

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/quickstart.rst.txt` & `jira-select-3.3.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/source/jira_select.commands.rst.txt` & `jira-select-3.3.0/docs/source/jira_select.commands.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/source/jira_select.formatters.rst.txt` & `jira-select-3.3.0/docs/source/jira_select.formatters.rst`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 ----------------------------------
 
 .. automodule:: jira_select.formatters.csv
    :members:
    :undoc-members:
    :show-inheritance:
 
+jira\_select.formatters.tsv module
+----------------------------------
+
+.. automodule:: jira_select.formatters.tsv
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 jira\_select.formatters.html module
 -----------------------------------
 
 .. automodule:: jira_select.formatters.html
    :members:
    :undoc-members:
    :show-inheritance:
@@ -32,14 +40,21 @@
 ------------------------------------
 
 .. automodule:: jira_select.formatters.table
    :members:
    :undoc-members:
    :show-inheritance:
 
+jira\_select.formatters.raw module
+----------------------------------
+
+.. automodule:: jira_select.formatters.raw
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 Module contents
 ---------------
 
 .. automodule:: jira_select.formatters
    :members:
    :undoc-members:
```

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/source/jira_select.functions.rst.txt` & `jira-select-3.3.0/docs/source/jira_select.functions.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/source/jira_select.rst.txt` & `jira-select-3.3.0/docs/source/jira_select.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/source/tests.rst.txt` & `jira-select-3.3.0/docs/source/tests.rst`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/docs/_build/html/_sources/troubleshooting.rst.txt` & `jira-select-3.3.0/docs/troubleshooting.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 -------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 The viewer you see being used on in the demo gif is called `Visidata <https://www.visidata.org/>`_, and unfortunately it isn't available on all platforms.  You do have a few options, though:
 
 1. You could use the ``--format=table`` command-line argument to tell jira-select to print your output to the screen in a fancy table mode.
 2. You could ask jira-select to open the query results in your system's defualt viewer using the ``--launch-default-viewer`` command-line argument.  On Windows, you will also need to specify an output path explicitly to make this work by using ``--output=/some/path/to/write/output/to.csv``.
 3. If you're running on Windows, you could install this under "Windows Subsystem for Linux" so that you can use the default viewer (visidata). See more information here: `Windows Subsystem for Linux Installation Guide for Windows 10 <https://docs.microsoft.com/en-us/windows/wsl/install-win10>`_.
-4. You could use the ``run`` subcommand instead of ``shell`.  This particular subcommand is a lot less fancy than ``shell``, though.
+4. You could use the ``run-query`` subcommand instead of ``shell``.  This particular subcommand is a lot less fancy than ``shell``, though.
 
 Sometimes filtering using ``having`` (or sorting using ``sort_by``) on a value I see in the output doesn't work; why not?
 -------------------------------------------------------------------------------------------------------------------------
 
 Oftentimes the data returned from Jira for a particular field
 is not a simple string or number
 and is instead a complex object full of other information.
@@ -34,15 +34,15 @@
 -- for example: for ``issuetype`` --
 you can access the raw Jira object via the ``raw`` property
 of the field; e.g.
 
 .. code-block:: yaml
 
    select:
-   - issuetype.raw
+     Raw Issue Data: issuetype.raw
    from: issues
 
 I can't connect because my Jira instance uses a self-signed certificate
 -----------------------------------------------------------------------
 
 Don't worry,
 there are two command-line arguments you can use
@@ -76,9 +76,9 @@
 In cases like those,
 you should just wrap your whole query expression in quotes;
 for example:
 
 .. code-block:: yaml
 
    select:
-   - '{Story Points}'
+     Story Points: '{Story Points}'
    from: issues
```

### Comparing `jira-select-3.2.0/docs/conf.py` & `jira-select-3.3.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 project = "Jira-Select"
 copyright = "2022, Adam Coddington"
 author = "Adam Coddington"
 
 # The short X.Y version
 version = ""
 # The full version, including alpha/beta/rc tags
-release = "3.2.0"
+release = "3.3.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `jira-select-3.2.0/docs/evaluation_location.csv` & `jira-select-3.3.0/docs/evaluation_location.csv`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/docs/make.bat` & `jira-select-3.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/cache.py` & `jira-select-3.3.0/jira_select/cache.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/cmdline.py` & `jira-select-3.3.0/jira_select/cmdline.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/commands/build_query.py` & `jira-select-3.3.0/jira_select/commands/build_query.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/commands/configure.py` & `jira-select-3.3.0/jira_select/commands/configure.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/commands/functions.py` & `jira-select-3.3.0/jira_select/commands/functions.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/commands/install_user_script.py` & `jira-select-3.3.0/jira_select/commands/install_user_script.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/commands/run.py` & `jira-select-3.3.0/jira_select/commands/run.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/commands/run_script.py` & `jira-select-3.3.0/jira_select/commands/run_script.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/commands/schema.py` & `jira-select-3.3.0/jira_select/commands/schema.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/commands/setup_instance.py` & `jira-select-3.3.0/jira_select/commands/setup_instance.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/commands/shell.py` & `jira-select-3.3.0/jira_select/commands/shell.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/commands/show_instances.py` & `jira-select-3.3.0/jira_select/commands/show_instances.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/commands/store_password.py` & `jira-select-3.3.0/jira_select/commands/store_password.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/formatters/csv.py` & `jira-select-3.3.0/jira_select/formatters/csv.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/formatters/html.py` & `jira-select-3.3.0/jira_select/formatters/html.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/formatters/json.py` & `jira-select-3.3.0/jira_select/formatters/json.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/formatters/table.py` & `jira-select-3.3.0/jira_select/formatters/table.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/estimate_to_days.py` & `jira-select-3.3.0/jira_select/functions/estimate_to_days.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/extract.py` & `jira-select-3.3.0/jira_select/functions/extract.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/field_by_name.py` & `jira-select-3.3.0/jira_select/functions/field_by_name.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/flatten_changelog.py` & `jira-select-3.3.0/jira_select/functions/flatten_changelog.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/get_issue_snapshot_on_date.py` & `jira-select-3.3.0/jira_select/functions/get_issue_snapshot_on_date.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/get_linked_issue_keys.py` & `jira-select-3.3.0/jira_select/functions/get_linked_issue_keys.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/get_sprint_by_id.py` & `jira-select-3.3.0/jira_select/functions/get_sprint_by_id.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/get_sprint_by_name.py` & `jira-select-3.3.0/jira_select/functions/get_sprint_by_name.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/interval_business_hours.py` & `jira-select-3.3.0/jira_select/functions/interval_business_hours.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/interval_matching.py` & `jira-select-3.3.0/jira_select/functions/interval_matching.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/interval_size.py` & `jira-select-3.3.0/jira_select/functions/interval_size.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/parse_date.py` & `jira-select-3.3.0/jira_select/functions/parse_date.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/parse_datetime.py` & `jira-select-3.3.0/jira_select/functions/parse_datetime.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/simple_filter.py` & `jira-select-3.3.0/jira_select/functions/simple_filter.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/simple_filter_any.py` & `jira-select-3.3.0/jira_select/functions/simple_filter_any.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/sprint_details.py` & `jira-select-3.3.0/jira_select/functions/sprint_details.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/subquery.py` & `jira-select-3.3.0/jira_select/functions/subquery.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/functions/workdays_in_state.py` & `jira-select-3.3.0/jira_select/functions/workdays_in_state.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/plugin.py` & `jira-select-3.3.0/jira_select/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,16 +196,15 @@
 class BaseFormatter(metaclass=ABCMeta):
     def __init__(self, executor: Executor, stream: IO[bytes]):
         self._executor = proxy(executor)
         self._stream = stream
 
     @classmethod
     @abstractmethod
-    def get_file_extension(cls) -> str:
-        ...
+    def get_file_extension(cls) -> str: ...
 
     @property
     def executor(self):
         return self._executor
 
     @property
     def stream(self):
@@ -222,25 +221,24 @@
     def open(self):
         return
 
     def close(self):
         return
 
     @abstractmethod
-    def writerow(self, row: Dict[str, Any]):
-        ...
+    def writerow(self, row: Dict[str, Any]): ...
 
 
 def register_function(fn: Callable):
     """Register a callable to be a function available in queries."""
     REGISTERED_FUNCTIONS[fn.__name__] = fn
 
 
 def get_installed_functions(
-    jira: JIRA = None, executor: Executor = None
+    jira: Optional[JIRA] = None, executor: Optional[Executor] = None
 ) -> Dict[str, Callable]:
     possible_commands: Dict[str, Callable] = copy.copy(BUILTIN_FUNCTIONS)
 
     # Import any modules in the custom functions directory; as a
     # side-effect of this, the functions will become listed within
     # REGISTERED_FUNCTIONS
     function_dir = get_custom_function_dir()
@@ -293,16 +291,15 @@
     @property
     def jira(self):
         assert self._jira
 
         return self._jira
 
     @abstractmethod
-    def __call__(self, *args, **kwargs) -> Optional[Any]:
-        ...
+    def __call__(self, *args, **kwargs) -> Optional[Any]: ...
 
 
 def get_installed_sources() -> Dict[str, Type[BaseSource]]:
     return get_entrypoints(SOURCE_ENTRYPOINT, BaseSource)
 
 
 class BaseSource(metaclass=ABCMeta):
@@ -347,13 +344,11 @@
         return self._executor.query
 
     @property
     def jira(self) -> JIRA:
         return self._executor.jira
 
     @abstractmethod
-    def rehydrate(self, value: Any) -> Any:
-        ...
+    def rehydrate(self, value: Any) -> Any: ...
 
     @abstractmethod
-    def __iter__(self) -> Iterator[Any]:
-        ...
+    def __iter__(self) -> Iterator[Any]: ...
```

### Comparing `jira-select-3.2.0/jira_select/query.py` & `jira-select-3.3.0/jira_select/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,32 +75,30 @@
             return False
 
     def __str__(self):
         return str(self._value)
 
 
 class Result(metaclass=ABCMeta):
-    def __init__(self):
+    def __init__(self) -> None:
         self._overlay: dict[str, Any] = {}
 
-    def __getattr__(self, name):
+    def __getattr__(self, name) -> Any:
         result = self.as_dict()
 
         if name not in result:
             raise AttributeError(name)
 
         return result[name]
 
     @abstractmethod
-    def as_dict(self) -> Dict[str, Any]:
-        ...
+    def as_dict(self) -> Dict[str, Any]: ...
 
     @abstractmethod
-    def single(self) -> SingleResult:
-        ...
+    def single(self) -> SingleResult: ...
 
     def evaluate_expression(
         self,
         expression: Expression,
         group_by: Optional[ExpressionList] = None,
         field_name_map: Optional[Dict[str, Any]] = None,
         functions: Optional[Dict[str, Callable]] = None,
@@ -162,15 +160,15 @@
 
         return results
 
 
 class GroupedResult(Result):
     def __init__(
         self,
-        rows: List[SingleResult] = None,
+        rows: Optional[List[SingleResult]] = None,
     ):
         super().__init__()
         self._rows: List[SingleResult] = rows if rows is not None else []
 
     @property
     def rows(self):
         return self._rows
@@ -352,24 +350,24 @@
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         pass
 
 
 class CounterChannel:
-    def __init__(self):
+    def __init__(self) -> None:
         self._counter: int = 2**32
 
-    def zero(self):
+    def zero(self) -> None:
         self._counter = 0
 
-    def increment(self):
+    def increment(self) -> None:
         self._counter += 1
 
-    def set(self, value: int):
+    def set(self, value: int) -> None:
         self._counter = value
 
     def get(self) -> int:
         return self._counter
 
 
 class FieldNameMap(dict):
```

### Comparing `jira-select-3.2.0/jira_select/sources/boards.py` & `jira-select-3.3.0/jira_select/sources/boards.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/sources/issues.py` & `jira-select-3.3.0/jira_select/sources/issues.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/sources/sprints.py` & `jira-select-3.3.0/jira_select/sources/sprints.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/types.py` & `jira-select-3.3.0/jira_select/types.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/jira_select/utils.py` & `jira-select-3.3.0/jira_select/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,19 @@
         from .functions.flatten_changelog import ChangelogEntry
 
         if isinstance(obj, datetime.datetime):
             return UTC.normalize(obj).strftime(ISO_FORMAT)
         elif isinstance(obj, ChangelogEntry):
             return {
                 "author": obj.author,
-                "created": UTC.normalize(obj.created).strftime(ISO_FORMAT)
-                if obj.created
-                else None,
+                "created": (
+                    UTC.normalize(obj.created).strftime(ISO_FORMAT)
+                    if obj.created
+                    else None
+                ),
                 "field": obj.field,
                 "fieldtype": obj.fieldtype,
                 "fromValue": obj.fromValue,
                 "fromString": obj.fromString,
                 "toValue": obj.toValue,
                 "toString": obj.toString,
             }
@@ -116,26 +118,26 @@
     root_path = get_config_dir()
     return os.path.join(
         root_path,
         "config.yaml",
     )
 
 
-def get_config(path: str = None) -> ConfigDict:
+def get_config(path: str | None = None) -> ConfigDict:
     if path is None:
         path = get_default_config_path()
 
     if not os.path.isfile(path):
         return ConfigDict()
 
     with open(path, "r") as inf:
         return ConfigDict.parse_obj(safe_load(inf))
 
 
-def save_config(data: ConfigDict, path: str = None) -> None:
+def save_config(data: ConfigDict, path: str | None = None) -> None:
     if path is None:
         path = get_default_config_path()
 
     with open(path, "w") as outf:
         safe_dump(data.dict(), outf)
```

### Comparing `jira-select-3.2.0/jira_select.egg-info/PKG-INFO` & `jira-select-3.3.0/jira_select.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: jira-select
-Version: 3.2.0
+Version: 3.3.0
 Summary: Easily run complex SQL-like queries far beyond what Jira's standard JQL query language can provide.
 Home-page: https://github.com/coddingtonbear/jira-select
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
 Project-URL: Issue Tracker, https://github.com/coddingtonbear/jira-select/issues
 Keywords: jira,csv,sql
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
@@ -110,7 +111,9 @@
 your query, press `Esc` followed by `Enter` and after a short wait (watch the progressbars), you'll be shown your results. Press `q` to exit your results.
 
 ---
 
 - Documentation for Jira-select is available on [ReadTheDocs](http://jira-select.readthedocs.org/).
 - Please post issues on [Github](http://github.com/coddingtonbear/jira-select/issues).
 - Questions? Ask them on [Gitter](https://gitter.im/coddingtonbear/jira-select).
+
+
```

### Comparing `jira-select-3.2.0/jira_select.egg-info/entry_points.txt` & `jira-select-3.3.0/jira_select.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [console_scripts]
 jira-select = jira_select.cmdline:main
 
 [jira_select.commands]
+batch = jira_select.commands.batch:Command
 build-query = jira_select.commands.build_query:Command
 configure = jira_select.commands.configure:Command
 functions = jira_select.commands.functions:Command
 install-user-script = jira_select.commands.install_user_script:Command
 remove-instance = jira_select.commands.remove_instance:Command
 run-query = jira_select.commands.run:Command
 run-script = jira_select.commands.run_script:Command
@@ -49,7 +50,8 @@
 union = jira_select.functions.union:Function
 workdays_in_state = jira_select.functions.workdays_in_state:Function
 
 [jira_select.sources]
 boards = jira_select.sources.boards:Source
 issues = jira_select.sources.issues:Source
 sprints = jira_select.sources.sprints:Source
+
```

### Comparing `jira-select-3.2.0/pyinstaller/Makefile` & `jira-select-3.3.0/pyinstaller/Makefile`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/pyinstaller/jira_select.exe.spec` & `jira-select-3.3.0/pyinstaller/jira_select.exe.spec`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/pyinstaller/jira_select.spec` & `jira-select-3.3.0/pyinstaller/jira_select.spec`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/readme.md` & `jira-select-3.3.0/readme.md`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/setup.cfg` & `jira-select-3.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 max-line-length = 88
 ignore = 
 	E203,
 	E231,
 	E501,
 	W503,
 	A003,
+	E704,
 exclude = 
 	migrations,
 
 [pep8]
 max-line-length = 88
 ignore = 
 	E701,
```

### Comparing `jira-select-3.2.0/setup.py` & `jira-select-3.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="jira-select",
-    version="3.2.0",
+    version="3.3.0",
     license="MIT",
     description=(
         "Easily run complex SQL-like queries far beyond what "
         "Jira's standard JQL query language can provide."
     ),
     long_description_content_type="text/markdown",
     long_description=read("readme.md"),
@@ -88,14 +88,15 @@
             "functions = jira_select.commands.functions:Command",
             "shell = jira_select.commands.shell:Command",
             "run-script = jira_select.commands.run_script:Command",
             "show-instances = jira_select.commands.show_instances:Command",
             "setup-instance = jira_select.commands.setup_instance:Command",
             "remove-instance = jira_select.commands.remove_instance:Command",
             "install-user-script = jira_select.commands.install_user_script:Command",
+            "batch = jira_select.commands.batch:Command",
         ],
         "jira_select.formatters": [
             "csv = jira_select.formatters.csv:Formatter",
             "tsv = jira_select.formatters.tsv:Formatter",
             "html = jira_select.formatters.html:Formatter",
             "json = jira_select.formatters.json:Formatter",
             "table = jira_select.formatters.table:Formatter",
```

### Comparing `jira-select-3.2.0/tests/base.py` & `jira-select-3.3.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/tests/test_functions.py` & `jira-select-3.3.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/tests/test_query.py` & `jira-select-3.3.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.2.0/tests/test_utils.py` & `jira-select-3.3.0/tests/test_utils.py`

 * *Files identical despite different names*

