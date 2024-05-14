# Comparing `tmp/records-mover-1.6.3.tar.gz` & `tmp/records_mover-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "records-mover-1.6.3.tar", last modified: Tue Jan  2 21:52:19 2024, max compression
+gzip compressed data, was "records_mover-1.6.4.tar", last modified: Tue May 14 18:25:00 2024, max compression
```

## Comparing `records-mover-1.6.3.tar` & `records_mover-1.6.4.tar`

### file list

```diff
@@ -1,219 +1,831 @@
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.298880 records-mover-1.6.3/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    11357 2022-12-13 16:38:59.000000 records-mover-1.6.3/LICENSE
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    11068 2024-01-02 21:52:19.299022 records-mover-1.6.3/PKG-INFO
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7862 2023-12-18 21:29:31.000000 records-mover-1.6.3/README.md
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.261614 records-mover-1.6.3/records_mover/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1534 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/__init__.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.262452 records-mover-1.6.3/records_mover/airflow/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)       41 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/airflow/__init__.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.263233 records-mover-1.6.3/records_mover/airflow/hooks/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      145 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/airflow/hooks/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      886 2023-12-18 21:29:31.000000 records-mover-1.6.3/records_mover/airflow/hooks/google_cloud_credentials_hook.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4796 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/airflow/hooks/records_hook.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1048 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/airflow/hooks/sqlalchemy_db_hook.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2555 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/check_db_conn_engine.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.263528 records-mover-1.6.3/records_mover/cli/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/cli/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10464 2023-04-17 17:48:22.000000 records-mover-1.6.3/records_mover/cli/job_config_schema_as_args_parser.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.264746 records-mover-1.6.3/records_mover/creds/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/creds/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    12137 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/creds/base_creds.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2465 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/creds/creds_via_airflow.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2002 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/creds/creds_via_env.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1150 2024-01-01 21:14:40.000000 records-mover-1.6.3/records_mover/creds/creds_via_lastpass.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1452 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/creds/database.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.266433 records-mover-1.6.3/records_mover/db/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      194 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/__init__.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.267339 records-mover-1.6.3/records_mover/db/bigquery/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/bigquery/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7161 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/bigquery/bigquery_db_driver.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    15001 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/bigquery/load_job_config_options.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9492 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/bigquery/loader.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5460 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/bigquery/unloader.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5243 2024-01-01 21:14:40.000000 records-mover-1.6.3/records_mover/db/connect.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1067 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/db_conn_mixin.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      527 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/db_type.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10456 2023-12-18 21:29:31.000000 records-mover-1.6.3/records_mover/db/driver.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      445 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/errors.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1626 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/factory.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4545 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/loader.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.268372 records-mover-1.6.3/records_mover/db/mysql/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/mysql/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    19866 2023-12-18 21:29:31.000000 records-mover-1.6.3/records_mover/db/mysql/load_options.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5619 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/mysql/loader.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7837 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/mysql/mysql_db_driver.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.269459 records-mover-1.6.3/records_mover/db/postgres/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/postgres/__init__.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.270996 records-mover-1.6.3/records_mover/db/postgres/copy_options/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4471 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/db/postgres/copy_options/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2750 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/postgres/copy_options/common.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6487 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/postgres/copy_options/csv.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    14773 2023-06-07 16:25:30.000000 records-mover-1.6.3/records_mover/db/postgres/copy_options/date_input_style.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1663 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/postgres/copy_options/date_output_style.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)       87 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/postgres/copy_options/mode.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5283 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/postgres/copy_options/text.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4044 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/postgres/copy_options/types.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6618 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/postgres/loader.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4776 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/postgres/postgres_db_driver.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5453 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/db/postgres/sqlalchemy_postgres_copy.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6043 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/postgres/unloader.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2975 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/quoting.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.273119 records-mover-1.6.3/records_mover/db/redshift/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/redshift/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9546 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/redshift/loader.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    11595 2023-04-17 17:48:22.000000 records-mover-1.6.3/records_mover/db/redshift/records_copy.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6209 2023-03-28 18:26:22.000000 records-mover-1.6.3/records_mover/db/redshift/records_unload.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10362 2023-12-18 21:29:31.000000 records-mover-1.6.3/records_mover/db/redshift/redshift_db_driver.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2286 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/redshift/sql.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8355 2023-12-18 21:29:31.000000 records-mover-1.6.3/records_mover/db/redshift/unloader.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3228 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/unloader.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.275956 records-mover-1.6.3/records_mover/db/vertica/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/vertica/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1443 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/vertica/export_sql.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4023 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/vertica/import_sql.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      244 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/vertica/io_base_wrapper.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4568 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/vertica/loader.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2948 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/vertica/records_export_options.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4357 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/db/vertica/records_import_options.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7469 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/db/vertica/unloader.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5916 2023-12-18 21:29:31.000000 records-mover-1.6.3/records_mover/db/vertica/vertica_db_driver.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2787 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/logging.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1060 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/mover_types.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.276273 records-mover-1.6.3/records_mover/pandas/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1275 2023-06-07 16:25:30.000000 records-mover-1.6.3/records_mover/pandas/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/py.typed
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.280840 records-mover-1.6.3/records_mover/records/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      957 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      987 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/base_records_format.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5383 2023-03-17 16:09:02.000000 records-mover-1.6.3/records_mover/records/cli.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.283101 records-mover-1.6.3/records_mover/records/delimited/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1752 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/delimited/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      651 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/delimited/compression.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2294 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/delimited/conversions.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2798 2023-06-07 16:25:30.000000 records-mover-1.6.3/records_mover/records/delimited/csv_streamer.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4254 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/delimited/hint.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5611 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/delimited/hints.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    12383 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/delimited/sniff.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2590 2022-12-21 21:38:12.000000 records-mover-1.6.3/records_mover/records/delimited/types.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2165 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/delimited/utils.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1933 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/delimited/validated_records_hints.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      533 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/deprecated.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      297 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/errors.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1327 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/existing_table_handling.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.283764 records-mover-1.6.3/records_mover/records/job/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/job/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7822 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/job/config.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1720 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/job/mover.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3047 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/job/schema.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      389 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/load_plan.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9086 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/mover.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.284906 records-mover-1.6.3/records_mover/records/pandas/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      525 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/pandas/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5882 2023-12-18 21:29:31.000000 records-mover-1.6.3/records_mover/records/pandas/prep_for_csv.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    23611 2023-06-07 16:25:30.000000 records-mover-1.6.3/records_mover/records/pandas/read_csv_options.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4499 2023-06-07 16:25:30.000000 records-mover-1.6.3/records_mover/records/pandas/to_csv_options.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5405 2023-12-18 21:29:31.000000 records-mover-1.6.3/records_mover/records/prep.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2072 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/prep_and_load.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2929 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/processing_instructions.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3103 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/records.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9287 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/records_directory.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10672 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/records_format.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3400 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/records_format_file.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      701 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/records_schema_json_file.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      346 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/records_schema_sql_file.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1068 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/records_types.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      685 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/results.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.285337 records-mover-1.6.3/records_mover/records/schema/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      671 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/schema/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      496 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/schema/errors.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.287140 records-mover-1.6.3/records_mover/records/schema/field/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    14827 2023-04-04 17:39:28.000000 records-mover-1.6.3/records_mover/records/schema/field/__init__.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.288006 records-mover-1.6.3/records_mover/records/schema/field/constraints/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      368 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/schema/field/constraints/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9333 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/schema/field/constraints/constraints.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3115 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/schema/field/constraints/decimal.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1797 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/schema/field/constraints/integer.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2471 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/schema/field/constraints/string.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      434 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/schema/field/field_types.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1389 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/schema/field/numpy.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5427 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/schema/field/pandas.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8181 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/schema/field/representation.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9260 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/schema/field/sqlalchemy.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3093 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/schema/field/statistics.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2575 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/schema/field/string_length_generator.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.288766 records-mover-1.6.3/records_mover/records/schema/schema/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    11357 2023-06-07 16:25:24.000000 records-mover-1.6.3/records_mover/records/schema/schema/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4055 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/schema/schema/known_representation.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2391 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/schema/schema/pandas.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1973 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/schema/schema/sqlalchemy.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.290676 records-mover-1.6.3/records_mover/records/sources/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      289 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/sources/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6459 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/sources/base.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2551 2023-06-07 16:25:24.000000 records-mover-1.6.3/records_mover/records/sources/data_url.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8399 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/sources/dataframes.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2354 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/sources/directory.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    13519 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/sources/factory.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8507 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/sources/fileobjs.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4468 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/sources/google_sheets.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7010 2023-12-18 21:29:31.000000 records-mover-1.6.3/records_mover/records/sources/table.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2251 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/sources/uninferred_fileobjs.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1102 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/table.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.292302 records-mover-1.6.3/records_mover/records/targets/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)       71 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/targets/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7084 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/targets/base.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3850 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/targets/data_url.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1128 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/targets/directory_from_url.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10689 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/targets/factory.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3984 2023-04-17 17:48:22.000000 records-mover-1.6.3/records_mover/records/targets/fileobj.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5197 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/targets/google_sheets.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8029 2023-12-18 21:29:31.000000 records-mover-1.6.3/records_mover/records/targets/spectrum.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.294040 records-mover-1.6.3/records_mover/records/targets/table/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)       47 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/targets/table/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1345 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/records/targets/table/base.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5217 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/targets/table/move_from_dataframes_source.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3580 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/targets/table/move_from_fileobjs_source.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3628 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/targets/table/move_from_records_directory.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2991 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/targets/table/move_from_temp_loc_after_filling_it.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8858 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/records/targets/table/target.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      483 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/records/unload_plan.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    17448 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/session.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.295368 records-mover-1.6.3/records_mover/url/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)       95 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8203 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/base.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3823 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/filesystem.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.295831 records-mover-1.6.3/records_mover/url/gcs/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/gcs/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3296 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/gcs/gcs_directory_url.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2308 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/gcs/gcs_file_url.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      192 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/http.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5278 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/resolver.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.296758 records-mover-1.6.3/records_mover/url/s3/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/s3/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      673 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/s3/awscli.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3034 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/s3/s3_base_url.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2564 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/s3/s3_directory_url.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6147 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/s3/s3_file_url.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      556 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/s3/s3_url.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      287 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/url/urllib.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.298709 records-mover-1.6.3/records_mover/utils/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1707 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/utils/__init__.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1617 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/utils/concat_files.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      351 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/utils/json_parameter.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7845 2023-10-30 18:02:35.000000 records-mover-1.6.3/records_mover/utils/json_schema.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      722 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/utils/json_schema_array_document.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1033 2023-01-24 16:33:00.000000 records-mover-1.6.3/records_mover/utils/json_schema_document.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      574 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/utils/lazyprop.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1841 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/utils/limits.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2681 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/utils/retry.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      724 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/utils/rewound_fileobj.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)      967 2022-12-13 16:38:59.000000 records-mover-1.6.3/records_mover/utils/structures.py
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)       22 2024-01-01 21:27:07.000000 records-mover-1.6.3/records_mover/version.py
-drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-01-02 21:52:19.262337 records-mover-1.6.3/records_mover.egg-info/
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)    11068 2024-01-02 21:52:19.000000 records-mover-1.6.3/records_mover.egg-info/PKG-INFO
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7585 2024-01-02 21:52:19.000000 records-mover-1.6.3/records_mover.egg-info/SOURCES.txt
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)        1 2024-01-02 21:52:19.000000 records-mover-1.6.3/records_mover.egg-info/dependency_links.txt
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)       58 2024-01-02 21:52:19.000000 records-mover-1.6.3/records_mover.egg-info/entry_points.txt
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3083 2024-01-02 21:52:19.000000 records-mover-1.6.3/records_mover.egg-info/requires.txt
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)       14 2024-01-02 21:52:19.000000 records-mover-1.6.3/records_mover.egg-info/top_level.txt
--rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1500 2024-01-02 21:52:19.299499 records-mover-1.6.3/setup.cfg
--rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)    10875 2023-12-20 00:57:19.000000 records-mover-1.6.3/setup.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.501953 records_mover-1.6.4/
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.344769 records_mover-1.6.4/.circleci/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    27118 2024-05-09 22:32:16.000000 records_mover-1.6.4/.circleci/config.yml
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      905 2024-05-09 21:22:14.000000 records_mover-1.6.4/.dockerignore
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.324775 records_mover-1.6.4/.github/
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.345265 records_mover-1.6.4/.github/workflows/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1231 2024-05-09 22:32:16.000000 records_mover-1.6.4/.github/workflows/test.yml
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      905 2024-05-09 21:22:14.000000 records_mover-1.6.4/.gitignore
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1365 2022-12-13 16:38:59.000000 records_mover-1.6.4/.markdown.style.rb
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       53 2022-12-13 16:38:59.000000 records_mover-1.6.4/.mdlrc
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       56 2022-12-13 16:38:59.000000 records_mover-1.6.4/.pronto.yml
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       20 2023-01-12 20:44:33.000000 records_mover-1.6.4/.python-version
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      371 2024-05-09 21:22:14.000000 records_mover-1.6.4/.readthedocs.yml
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      574 2024-05-09 21:22:14.000000 records_mover-1.6.4/Dockerfile.dev
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    11357 2022-12-13 16:38:59.000000 records_mover-1.6.4/LICENSE
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2429 2024-05-13 17:53:02.000000 records_mover-1.6.4/Makefile
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    26324 2024-05-14 18:25:00.501772 records_mover-1.6.4/PKG-INFO
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8213 2024-05-09 21:22:14.000000 records_mover-1.6.4/README.md
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1526 2023-04-04 17:39:28.000000 records_mover-1.6.4/Rakefile.quality
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)      837 2022-12-13 16:38:59.000000 records_mover-1.6.4/deps.sh
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      468 2024-05-09 21:22:14.000000 records_mover-1.6.4/docker-compose.yaml
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.347860 records_mover-1.6.4/docs/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3355 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8395 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/CONFIG.md
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8410 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/DRIVERS.md
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3099 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/INSTALL.md
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8395 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/LOADING_SUPPORT.md
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3773 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/MAINT.md
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      815 2023-01-24 16:33:00.000000 records_mover-1.6.4/docs/Makefile
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    15275 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/RECORDS_SPEC.md
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4441 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/SECURITY.md
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    78388 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/records-mover-horizontal.png
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.348836 records_mover-1.6.4/docs/schema/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      107 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/schema/Makefile
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    12792 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/schema/SCHEMAv1.md
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8267 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/schema/pandas_example_1.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7670 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/schema/records_schema_v1_schema.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    17574 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/schema/redshift_example_1.json
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.350803 records_mover-1.6.4/docs/source/
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.351107 records_mover-1.6.4/docs/source/_static/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/source/_static/.gitkeep
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2624 2023-03-17 16:09:02.000000 records_mover-1.6.4/docs/source/conf.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      472 2022-12-21 20:47:49.000000 records_mover-1.6.4/docs/source/index.rst
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      480 2022-12-21 22:06:48.000000 records_mover-1.6.4/docs/source/records_mover.airflow.hooks.rst
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      149 2022-12-21 22:06:48.000000 records_mover-1.6.4/docs/source/records_mover.airflow.rst
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2608 2022-12-21 22:22:16.000000 records_mover-1.6.4/docs/source/records_mover.records.rst
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      212 2022-12-21 22:06:48.000000 records_mover-1.6.4/docs/source/records_mover.records.sources.rst
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      212 2022-12-21 22:06:48.000000 records_mover-1.6.4/docs/source/records_mover.records.targets.rst
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      630 2023-03-17 16:09:02.000000 records_mover-1.6.4/docs/source/records_mover.rst
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2446 2022-12-13 16:38:59.000000 records_mover-1.6.4/docs/terminalizer.yml
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.353828 records_mover-1.6.4/metrics/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/brakeman_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/bundle-audit_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/cane_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        8 2024-05-09 21:22:14.000000 records_mover-1.6.4/metrics/coverage_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2024-05-09 21:22:14.000000 records_mover-1.6.4/metrics/flake8_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/flay_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/flog_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/mdl_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        8 2024-05-09 21:22:14.000000 records_mover-1.6.4/metrics/mypy_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/punchlist_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/pycodestyle_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/rails_best_practices_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/reek_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/rubocop_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/scalastyle_high_water_mark
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/metrics/shellcheck_high_water_mark
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)      291 2022-12-13 16:38:59.000000 records_mover-1.6.4/publish.sh
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4328 2024-05-14 18:24:25.000000 records_mover-1.6.4/pyproject.toml
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      129 2024-05-09 21:22:14.000000 records_mover-1.6.4/pytest.ini
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.355226 records_mover-1.6.4/records_mover/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1534 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.356236 records_mover-1.6.4/records_mover/airflow/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       41 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/airflow/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.357115 records_mover-1.6.4/records_mover/airflow/hooks/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      145 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/airflow/hooks/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      886 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/airflow/hooks/google_cloud_credentials_hook.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4796 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/airflow/hooks/records_hook.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1048 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/airflow/hooks/sqlalchemy_db_hook.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2555 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/check_db_conn_engine.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.357623 records_mover-1.6.4/records_mover/cli/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/cli/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10464 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/cli/job_config_schema_as_args_parser.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.359258 records_mover-1.6.4/records_mover/creds/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/creds/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    12630 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/creds/base_creds.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2465 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/creds/creds_via_airflow.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2296 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/creds/creds_via_env.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1551 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/creds/creds_via_lastpass.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1451 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/creds/database.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.361448 records_mover-1.6.4/records_mover/db/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      194 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.362729 records_mover-1.6.4/records_mover/db/bigquery/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/bigquery/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7161 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/bigquery/bigquery_db_driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    15001 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/bigquery/load_job_config_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9492 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/bigquery/loader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5460 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/bigquery/unloader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5243 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/connect.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1067 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/db_conn_mixin.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      527 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/db_type.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10456 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      445 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/errors.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1626 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/factory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4545 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/loader.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.363786 records_mover-1.6.4/records_mover/db/mysql/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/mysql/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    19866 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/mysql/load_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5619 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/mysql/loader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7837 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/mysql/mysql_db_driver.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.365062 records_mover-1.6.4/records_mover/db/postgres/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/postgres/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.368130 records_mover-1.6.4/records_mover/db/postgres/copy_options/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4471 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/db/postgres/copy_options/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2750 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/postgres/copy_options/common.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6487 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/postgres/copy_options/csv.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    14773 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/postgres/copy_options/date_input_style.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1663 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/postgres/copy_options/date_output_style.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       87 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/postgres/copy_options/mode.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5283 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/postgres/copy_options/text.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4044 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/postgres/copy_options/types.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6618 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/postgres/loader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4776 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/postgres/postgres_db_driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5453 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/db/postgres/sqlalchemy_postgres_copy.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      551 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/postgres/sqlalchemy_postgres_copy.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6043 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/postgres/unloader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2975 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/quoting.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.370226 records_mover-1.6.4/records_mover/db/redshift/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/redshift/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9546 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/redshift/loader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    11595 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/redshift/records_copy.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6209 2023-03-28 18:26:22.000000 records_mover-1.6.4/records_mover/db/redshift/records_unload.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10362 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/redshift/redshift_db_driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2286 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/redshift/sql.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8355 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/redshift/unloader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3228 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/unloader.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.372268 records_mover-1.6.4/records_mover/db/vertica/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/vertica/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1443 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/vertica/export_sql.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4023 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/vertica/import_sql.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      244 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/vertica/io_base_wrapper.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4568 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/vertica/loader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2948 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/vertica/records_export_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4357 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/db/vertica/records_import_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7469 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/vertica/unloader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5916 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/db/vertica/vertica_db_driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2787 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/logging.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1060 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/mover_types.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.372505 records_mover-1.6.4/records_mover/pandas/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1275 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/pandas/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/py.typed
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.377793 records_mover-1.6.4/records_mover/records/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      957 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.378065 records_mover-1.6.4/records_mover/records/airbyte/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1715 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/airbyte/airbyte.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      987 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/base_records_format.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6010 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/cli.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.380493 records_mover-1.6.4/records_mover/records/delimited/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1752 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/delimited/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      651 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/delimited/compression.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2294 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/delimited/conversions.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2798 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/delimited/csv_streamer.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4254 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/delimited/hint.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5611 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/delimited/hints.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    12383 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/delimited/sniff.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2590 2022-12-21 21:38:12.000000 records_mover-1.6.4/records_mover/records/delimited/types.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2165 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/delimited/utils.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1933 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/delimited/validated_records_hints.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      533 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/deprecated.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      297 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/errors.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1327 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/existing_table_handling.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.381373 records_mover-1.6.4/records_mover/records/job/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/job/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7822 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/job/config.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1720 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/job/mover.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3047 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/job/schema.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      389 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/load_plan.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9086 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/mover.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.382456 records_mover-1.6.4/records_mover/records/pandas/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      525 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/pandas/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5882 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/pandas/prep_for_csv.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    23611 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/pandas/read_csv_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4499 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/pandas/to_csv_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5405 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/prep.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2072 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/prep_and_load.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2929 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/processing_instructions.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3103 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/records.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9287 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/records_directory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10672 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/records_format.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3400 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/records_format_file.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      701 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/records_schema_json_file.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      346 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/records_schema_sql_file.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1068 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/records_types.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      685 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/results.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.382994 records_mover-1.6.4/records_mover/records/schema/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      671 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/schema/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      496 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/schema/errors.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.385219 records_mover-1.6.4/records_mover/records/schema/field/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    14827 2023-04-04 17:39:28.000000 records_mover-1.6.4/records_mover/records/schema/field/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.386206 records_mover-1.6.4/records_mover/records/schema/field/constraints/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      368 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/schema/field/constraints/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9333 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/schema/field/constraints/constraints.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3115 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/schema/field/constraints/decimal.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1797 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/schema/field/constraints/integer.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2471 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/schema/field/constraints/string.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      434 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/schema/field/field_types.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1389 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/schema/field/numpy.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5427 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/schema/field/pandas.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8181 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/schema/field/representation.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9260 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/schema/field/sqlalchemy.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3093 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/schema/field/statistics.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2575 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/schema/field/string_length_generator.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.387204 records_mover-1.6.4/records_mover/records/schema/schema/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    11357 2024-05-09 21:11:05.000000 records_mover-1.6.4/records_mover/records/schema/schema/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4055 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/schema/schema/known_representation.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2391 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/schema/schema/pandas.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1973 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/schema/schema/sqlalchemy.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.390440 records_mover-1.6.4/records_mover/records/sources/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      289 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/sources/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6459 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/sources/base.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2551 2023-06-07 16:25:24.000000 records_mover-1.6.4/records_mover/records/sources/data_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8399 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/sources/dataframes.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2354 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/sources/directory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    13519 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/sources/factory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8507 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/sources/fileobjs.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4468 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/sources/google_sheets.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7010 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/sources/table.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2251 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/sources/uninferred_fileobjs.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1102 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/table.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.392417 records_mover-1.6.4/records_mover/records/targets/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       71 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/targets/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7084 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/targets/base.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3850 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/targets/data_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1128 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/targets/directory_from_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10689 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/targets/factory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3984 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/targets/fileobj.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5197 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/targets/google_sheets.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8029 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/targets/spectrum.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.394951 records_mover-1.6.4/records_mover/records/targets/table/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       47 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/targets/table/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1345 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/records/targets/table/base.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5217 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/targets/table/move_from_dataframes_source.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3580 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/targets/table/move_from_fileobjs_source.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3628 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/targets/table/move_from_records_directory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2991 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/targets/table/move_from_temp_loc_after_filling_it.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8858 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/records/targets/table/target.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      483 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/records/unload_plan.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    17450 2024-05-09 22:32:16.000000 records_mover-1.6.4/records_mover/session.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.396573 records_mover-1.6.4/records_mover/url/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       95 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8203 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/base.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3823 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/filesystem.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.397234 records_mover-1.6.4/records_mover/url/gcs/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/gcs/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3296 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/gcs/gcs_directory_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2395 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/url/gcs/gcs_file_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      192 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/http.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5482 2024-05-09 22:32:16.000000 records_mover-1.6.4/records_mover/url/resolver.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.398504 records_mover-1.6.4/records_mover/url/s3/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/s3/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      673 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/s3/awscli.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3034 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/s3/s3_base_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2564 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/s3/s3_directory_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6147 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/s3/s3_file_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      556 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/s3/s3_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      287 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/url/urllib.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.401048 records_mover-1.6.4/records_mover/utils/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1707 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/utils/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1617 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/utils/concat_files.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      351 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/utils/json_parameter.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7845 2024-05-09 21:22:14.000000 records_mover-1.6.4/records_mover/utils/json_schema.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      722 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/utils/json_schema_array_document.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1033 2023-01-24 16:33:00.000000 records_mover-1.6.4/records_mover/utils/json_schema_document.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      574 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/utils/lazyprop.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1841 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/utils/limits.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2681 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/utils/retry.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      724 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/utils/rewound_fileobj.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      967 2022-12-13 16:38:59.000000 records_mover-1.6.4/records_mover/utils/structures.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       22 2024-05-09 22:32:16.000000 records_mover-1.6.4/records_mover/version.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.497414 records_mover-1.6.4/records_mover.egg-info/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    26324 2024-05-14 18:25:00.000000 records_mover-1.6.4/records_mover.egg-info/PKG-INFO
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    29951 2024-05-14 18:25:00.000000 records_mover-1.6.4/records_mover.egg-info/SOURCES.txt
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        1 2024-05-14 18:25:00.000000 records_mover-1.6.4/records_mover.egg-info/dependency_links.txt
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       57 2024-05-14 18:25:00.000000 records_mover-1.6.4/records_mover.egg-info/entry_points.txt
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1671 2024-05-14 18:25:00.000000 records_mover-1.6.4/records_mover.egg-info/requires.txt
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       79 2024-05-14 18:25:00.000000 records_mover-1.6.4/records_mover.egg-info/top_level.txt
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      145 2024-05-13 17:53:02.000000 records_mover-1.6.4/requirements.txt
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1500 2024-05-14 18:25:00.502615 records_mover-1.6.4/setup.cfg
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)     3798 2024-05-09 21:22:14.000000 records_mover-1.6.4/setup.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.401236 records_mover-1.6.4/tests/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3328 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/README.md
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.401552 records_mover-1.6.4/tests/component/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.401884 records_mover-1.6.4/tests/component/airbyte/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1614 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/airbyte/test_airbyte_healthcheck.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.402290 records_mover-1.6.4/tests/component/cli/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/cli/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8287 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/cli/test_job_config_schema_as_args_parser.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.402604 records_mover-1.6.4/tests/component/db/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.403464 records_mover-1.6.4/tests/component/db/bigquery/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/bigquery/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10002 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/bigquery/test_load_config_options_custom.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6228 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/bigquery/test_load_config_options_datetime.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1416 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/bigquery/test_load_config_options_other.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5839 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/bigquery/test_load_config_options_variants.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.404730 records_mover-1.6.4/tests/component/db/mysql/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/mysql/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9862 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/mysql/test_load_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8470 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/db/mysql/test_load_options_class.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6078 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/db/mysql/test_mysql_db_driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1148 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/db/mysql/test_mysql_load_options_known.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.406970 records_mover-1.6.4/tests/component/db/postgres/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/postgres/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3115 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/postgres/test_copy_options_csv_unload.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10120 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/postgres/test_copy_options_date_output_style.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7350 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/postgres/test_date_order_style.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4936 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/postgres/test_postgres_copy_from_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3737 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/db/postgres/test_postgres_copy_from_options_load_known.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      826 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/db/postgres/test_postgres_copy_from_options_unload_known.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3536 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/db/postgres/test_postgres_db_driver.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.407859 records_mover-1.6.4/tests/component/db/redshift/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/redshift/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7634 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/redshift/test_records_copy.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4883 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/redshift/test_records_unload.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.408616 records_mover-1.6.4/tests/component/db/vertica/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/vertica/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6071 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/vertica/test_records_export_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6310 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/vertica/test_records_import_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5856 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/db/vertica/test_vertica_import_options.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.411319 records_mover-1.6.4/tests/component/records/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1288 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/datetime_cases.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1236 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/format_hints.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.412123 records_mover-1.6.4/tests/component/records/pandas/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/pandas/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    13550 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/pandas/test_prep_for_csv.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    11230 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/records/pandas/test_read_csv_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6867 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/pandas/test_to_csv_options.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.413094 records_mover-1.6.4/tests/component/records/schema/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/schema/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.413908 records_mover-1.6.4/tests/component/records/schema/field/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/schema/field/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4365 2023-02-13 18:27:28.000000 records_mover-1.6.4/tests/component/records/schema/field/test_dtype.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      729 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/schema/field/test_numpy.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5542 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/schema/field/test_pandas.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    45125 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/schema/future_incompatible_redshift_example_1.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8064 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/schema/pandas_example_1.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    45125 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/schema/redshift_example_1.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1620 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/schema/test_json_roundtrip.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.414238 records_mover-1.6.4/tests/component/records/sources/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/sources/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      473 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/sources/test_uninferred_fileobjs.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.414523 records_mover-1.6.4/tests/component/records/targets/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/targets/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1864 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/targets/test_data_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5106 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/test_delimited_records_format.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8853 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/test_hints.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6749 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/records/test_pandas_read_csv_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1713 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/records/test_pandas_to_csv_options_bluelabs.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1641 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/records/test_pandas_to_csv_options_csv.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5216 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/records/test_pandas_to_csv_options_dateformats.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1569 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/component/records/test_pandas_to_csv_options_vertica.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      625 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/test_parquet_records_format.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      830 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/test_records_format.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      475 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/records/test_validated_records_hints.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.329431 records_mover-1.6.4/tests/component/resources/
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.417355 records_mover-1.6.4/tests/component/resources/hint_sniffing/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1070 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-bluelabs-no-header-pandas-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      183 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-bluelabs-no-header-pandas-utc.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      281 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-csv-with-header-dos-newlines.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      220 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-csv-with-header-dos-newlines.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      278 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-csv-with-header-mac-newlines.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      218 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-csv-with-header-mac-newlines.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      278 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-csv-with-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      218 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-csv-with-header.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        4 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-one-column.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      284 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-one-column.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      275 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-tsv-with-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      216 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-tsv-with-header.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      209 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-vertica-no-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      510 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-vertica-no-header.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-zero-bytes.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      180 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/resources/hint_sniffing/delimited-zero-bytes.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      520 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/test_secrets_redacting_log_stream.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.418329 records_mover-1.6.4/tests/component/url/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/url/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      390 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/url/test_base.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      924 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/url/test_base_directory_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1460 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/url/test_resolver_misconfigured.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2233 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/url/test_resolver_no_creds.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      533 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/url/test_url_defaults.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.418781 records_mover-1.6.4/tests/component/utils/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/utils/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1855 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/utils/test_concat_files.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4727 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/component/utils/test_json_schema.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.421316 records_mover-1.6.4/tests/integration/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1458 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/Dockerfile
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3618 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/TORTURE.md
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.423096 records_mover-1.6.4/tests/integration/bin/
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)       44 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/bin/bluelabs-email
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)     1241 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/bin/db
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)     1099 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/bin/db-bigquery
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)      487 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/bin/db-connect
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)      308 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/bin/db-mysql
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)     1749 2022-12-19 15:42:08.000000 records_mover-1.6.4/tests/integration/bin/db-psql
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)     1068 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/bin/db-vsql
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)      101 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/bin/ensure-lpass-active
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)       28 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/bin/first-initial-then-last-name
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)     1218 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/bin/with-db
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1259 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/circleci-dbfacts.yml
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.425966 records_mover-1.6.4/tests/integration/cli/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       60 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/.gitignore
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)     5031 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/cli-tests.sh
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        4 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/data.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/empty.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        2 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/expected_target_recordsdir.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        4 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/expected_target_recordsdir_with_header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        4 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/expected_target_table.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4097 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/individual_tests.sh
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.427008 records_mover-1.6.4/tests/integration/cli/source_rdir/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      392 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/source_rdir/_format_delimited
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       51 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/source_rdir/_schema
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      480 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/source_rdir/_schema.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       40 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/cli/source_rdir/data.csv.gz
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1482 2023-01-11 17:27:41.000000 records_mover-1.6.4/tests/integration/docker-compose.yml
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.427220 records_mover-1.6.4/tests/integration/etc/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       31 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/etc/bigqueryrc
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1043 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/inside-docker-dbfacts.yml
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)    16775 2023-03-16 20:53:39.000000 records_mover-1.6.4/tests/integration/itest
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)      199 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/itest-dc
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.432126 records_mover-1.6.4/tests/integration/records/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/records/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1288 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/records/datetime_cases.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6652 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/records/directory_validator.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7945 2023-02-24 15:47:52.000000 records_mover-1.6.4/tests/integration/records/expected_column_types.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5553 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/mover_test_case.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.432847 records_mover-1.6.4/tests/integration/records/multi_db/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/records/multi_db/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1988 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/multi_db/test_dataframe_schema_sql_creation.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5384 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/multi_db/test_records_table2table.py
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)     3584 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/records/purge_old_test_sheets.py
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)     1855 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/purge_old_test_tables.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5628 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/records_database_fixture.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9590 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/records_datetime_fixture.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5860 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/records_numeric_database_fixture.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2452 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/integration/records/records_schema_v1_schema.json
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.435572 records_mover-1.6.4/tests/integration/records/single_db/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/records/single_db/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5132 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/single_db/base_records_test.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5715 2024-05-09 22:32:16.000000 records_mover-1.6.4/tests/integration/records/single_db/numeric_expectations.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      129 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/single_db/pytest.ini
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8690 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/records/single_db/test_records_load.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8039 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/single_db/test_records_load_datetime.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2287 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/records/single_db/test_records_load_df.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5689 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/single_db/test_records_numeric.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3564 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/records/single_db/test_records_save_df.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4170 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/single_db/test_records_unload.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    15582 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/single_db/test_records_unload_datetime.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10353 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/table_timezone_validator.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    12649 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/table_validator.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      626 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/integration/records/timezone.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.447697 records_mover-1.6.4/tests/integration/resources/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3045 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/README.md
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1145 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/_schema.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      217 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bigquery-no-header-pandas-notz.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      217 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bigquery-no-header-pandas-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      217 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bigquery-no-header-pandas.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      220 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bigquery-no-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      201 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bigquery-no-header.csv.gz
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      309 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bigquery-with-header-pandas-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      309 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bigquery-with-header-pandas.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      309 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bigquery-with-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      248 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bigquery-with-header.csv.gz
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      209 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-no-header-pandas-notz.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      214 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-no-header-pandas-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      214 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-no-header-pandas.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      212 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-no-header-postgres-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      212 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-no-header-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      171 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-no-header-utc.csv.gz
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      212 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-no-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      234 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-no-header.csv-broken
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      170 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-no-header.csv.gz
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      301 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-with-header-pandas-notz.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      306 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-with-header-pandas-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      306 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-with-header-pandas.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      304 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-with-header-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      304 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-with-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      218 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-bluelabs-with-header.csv.gz
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      191 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-csv-no-header-pandas-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      191 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-csv-no-header-pandas.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      185 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-csv-no-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      283 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-csv-with-header-pandas-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      283 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-csv-with-header-pandas.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      278 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-csv-with-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      233 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-csv-with-header.csv.gz
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      212 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-redshift-no-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      204 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-redshift-no-header.csv.gz
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      304 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-redshift-with-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      255 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-redshift-with-header.csv.gz
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      206 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-vertica-no-header-pandas-notz.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      211 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-vertica-no-header-pandas-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      211 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-vertica-no-header-pandas.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      209 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-vertica-no-header-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      209 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-vertica-no-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      201 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-vertica-no-header.csv.gz
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      298 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-vertica-with-header-pandas-notz.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      303 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-vertica-with-header-pandas-utc.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      303 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-vertica-with-header-pandas.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      301 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-vertica-with-header.csv
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      252 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/delimited-vertica-with-header.csv.gz
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3084 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/example_numeric_records_schema.json
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      282 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/schema-bigquery.sql
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      592 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/schema-redshift.sql
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      319 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/resources/schema-vertica.sql
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)      784 2023-03-16 20:52:09.000000 records_mover-1.6.4/tests/integration/test_docs_build.sh
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)      130 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/wait-for-mysql.sh
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)      136 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/wait-for-postgres.sh
+-rwxr-xr-x   0 brunocastrokarney   (502) staff       (20)      134 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/integration/wait-for-vertica.sh
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.451475 records_mover-1.6.4/tests/unit/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.452187 records_mover-1.6.4/tests/unit/airflow/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/airflow/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.452616 records_mover-1.6.4/tests/unit/airflow/hooks/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/airflow/hooks/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2139 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/unit/airflow/hooks/test_records_hook.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      667 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/airflow/test_google_cloud_credentials_hook.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1040 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/unit/airflow/test_records_hook.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.453760 records_mover-1.6.4/tests/unit/creds/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/creds/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    12581 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/creds/test_base_creds.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2791 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/unit/creds/test_creds_via_airflow.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1884 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/creds/test_creds_via_env.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.455964 records_mover-1.6.4/tests/unit/db/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.457191 records_mover-1.6.4/tests/unit/db/bigquery/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/bigquery/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5924 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/bigquery/test_bigquery_db_driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    18680 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/bigquery/test_bigquery_loader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7996 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/bigquery/test_bigquery_loader_can_load_this_format.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6341 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/bigquery/test_bigquery_unloader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      716 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/fake_results.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       75 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/fakes.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.457575 records_mover-1.6.4/tests/unit/db/mysql/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/mysql/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3662 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/mysql/test_loader.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.458575 records_mover-1.6.4/tests/unit/db/postgres/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/postgres/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10435 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/postgres/test_loader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3287 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/postgres/test_postgres_copy_to_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7371 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/postgres/test_unloader.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.461703 records_mover-1.6.4/tests/unit/db/redshift/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/redshift/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3133 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/redshift/base_test_redshift_db_driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8007 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/redshift/test_loader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      706 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/redshift/test_loader_temporary_bucket.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4830 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/redshift/test_redshift_db_driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2227 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/redshift/test_redshift_db_driver_format_negotiation.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1462 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/redshift/test_redshift_db_driver_import_bluelabs.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1422 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/redshift/test_redshift_db_driver_import_csv.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      336 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/redshift/test_redshift_db_driver_import_vertica.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3805 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/redshift/test_redshift_db_driver_unload.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1429 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/redshift/test_sql.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6625 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/redshift/test_unloader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3553 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/test_connect.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1519 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/test_db_conn_mixin.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6720 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/test_db_driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1680 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/test_factory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2224 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/test_quoting.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3486 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/test_sqlalchemy_driver_picking.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.464289 records_mover-1.6.4/tests/unit/db/vertica/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/vertica/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2728 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/vertica/base_test_vertica_db_driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1836 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/vertica/test_export_options.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2131 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/vertica/test_import_sql.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      341 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/vertica/test_io_base_wrapper.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1973 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/vertica/test_loader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2371 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/vertica/test_unloader.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3833 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/vertica/test_unloader_no_aws_creds.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2150 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/vertica/test_unloader_no_s3.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4989 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/vertica/test_vertica_db_driver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3879 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/db/vertica/test_vertica_db_driver_load.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       75 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/db/vertica/vertica_sql_expectations.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.464583 records_mover-1.6.4/tests/unit/pandas/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/pandas/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      648 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/pandas/test_pandas.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.468369 records_mover-1.6.4/tests/unit/records/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1283 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/base_test_records.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.468685 records_mover-1.6.4/tests/unit/records/delimited/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/delimited/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1452 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/delimited/test_sniff.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1361 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/fake_s3_object.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1236 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/format_hints.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.469538 records_mover-1.6.4/tests/unit/records/schema/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.471493 records_mover-1.6.4/tests/unit/records/schema/field/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.472312 records_mover-1.6.4/tests/unit/records/schema/field/sqlalchemy/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/sqlalchemy/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2268 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/schema/field/sqlalchemy/base_test_field_from_sqlalchemy_column.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1854 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/sqlalchemy/test_field_from_sqlalchemy_column_numeric.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8137 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/sqlalchemy/test_field_from_sqlalchemy_column_other.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7833 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/sqlalchemy/test_field_to_sqlalchemy_type.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3087 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/test_contraints.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3440 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/test_decimal_constraints.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7705 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/test_field.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2131 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/test_field_representation.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1999 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/test_field_string_constraints.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1475 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/test_integer_constraints.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3290 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/test_pandas.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1175 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/test_statistics.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5175 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/field/test_string_length_generator.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1636 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/unit/records/schema/test_known_representation.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6585 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/unit/records/schema/test_pandas.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    11192 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/schema/test_records_schema.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.473977 records_mover-1.6.4/tests/unit/records/sources/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/sources/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1336 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/sources/test_data_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9857 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/unit/records/sources/test_dataframes.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2467 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/sources/test_directory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5857 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/sources/test_factory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    12025 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/unit/records/sources/test_fileobjs.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     8710 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/sources/test_google_sheets.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    11054 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/sources/test_table.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1449 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/sources/test_table_edge_cases.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.476677 records_mover-1.6.4/tests/unit/records/targets/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/targets/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.478381 records_mover-1.6.4/tests/unit/records/targets/table/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/targets/table/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5459 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/targets/table/test_move_from_dataframes_source.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7570 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/targets/table/test_move_from_fileobjs_source.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6658 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/targets/table/test_move_from_records_directory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2467 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/targets/table/test_move_from_temp_loc_after_filling_it.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3969 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/targets/table/test_target.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      226 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/targets/test_base.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7205 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/targets/test_data_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2537 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/targets/test_directory_from_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4811 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/targets/test_factory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    20706 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/targets/test_fileobj.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6038 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/unit/records/targets/test_google_sheets.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     5358 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/targets/test_spectrum.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4772 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/targets/test_table_delegation.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2039 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/targets/test_table_file_objects.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1722 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/targets/test_table_format_negotiation.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1633 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/test_cli.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3874 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/test_csv_streamer.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1854 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/test_hints.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4620 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/test_jobs.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4073 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/test_jobs_hints_and_parquet_records_format.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9639 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/test_jobs_hints_and_records_format.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6980 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/test_mover.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     9327 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/records/test_prep.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    12251 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/unit/records/test_records_directory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3256 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/unit/records/test_records_directory_schema.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1132 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/test_records_format.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3742 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/test_records_format_file.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1112 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/test_records_infer.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1126 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/records/test_records_schema_json_file.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4150 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/test_check_db_conn_engine.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1485 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/test_cli_session.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1688 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/test_cli_session_records.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1427 2023-01-24 16:33:00.000000 records_mover-1.6.4/tests/unit/test_database.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      288 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/test_public_interface.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1250 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/test_records_hook.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2553 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/test_s3_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    17412 2024-05-09 21:22:14.000000 records_mover-1.6.4/tests/unit/test_session.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10673 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/test_session_choices.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1142 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/test_top_level.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.480459 records_mover-1.6.4/tests/unit/url/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/url/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.481012 records_mover-1.6.4/tests/unit/url/gcs/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/url/gcs/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2779 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/url/gcs/test_gcs_directory_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2228 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/url/gcs/test_gcs_file_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1027 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/url/test_awscli.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1323 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/url/test_base_file_url.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)    10428 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/url/test_filesystem.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      885 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/url/test_http_file.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3010 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/url/test_resolver.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     4117 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/url/test_s3_directory.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6654 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/url/test_s3_file.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.481494 records_mover-1.6.4/tests/unit/utils/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/utils/__init__.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      658 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/utils/test_beta.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      596 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/utils/test_deprecated.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       20 2022-12-13 16:38:59.000000 records_mover-1.6.4/tests/unit/workproduct.txt
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.332415 records_mover-1.6.4/types/
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.481864 records_mover-1.6.4/types/stubs/
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.482043 records_mover-1.6.4/types/stubs/airbyte/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2024-05-09 21:22:14.000000 records_mover-1.6.4/types/stubs/airbyte/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.482170 records_mover-1.6.4/types/stubs/airflow/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/airflow/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.482292 records_mover-1.6.4/types/stubs/airflow/contrib/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/airflow/contrib/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.482415 records_mover-1.6.4/types/stubs/airflow/contrib/hooks/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/airflow/contrib/hooks/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.482538 records_mover-1.6.4/types/stubs/airflow/contrib/hooks/aws_hook/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      344 2023-01-24 16:33:00.000000 records_mover-1.6.4/types/stubs/airflow/contrib/hooks/aws_hook/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.482859 records_mover-1.6.4/types/stubs/airflow/contrib/hooks/gcp_api_base_hook/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      412 2023-01-24 16:33:00.000000 records_mover-1.6.4/types/stubs/airflow/contrib/hooks/gcp_api_base_hook/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.483102 records_mover-1.6.4/types/stubs/airflow/exceptions/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      115 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/airflow/exceptions/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.483269 records_mover-1.6.4/types/stubs/airflow/hooks/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      189 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/airflow/hooks/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.483429 records_mover-1.6.4/types/stubs/airflow/models/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      242 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/airflow/models/__init__.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      405 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/argparse_types.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.483603 records_mover-1.6.4/types/stubs/awscli/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/awscli/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.483830 records_mover-1.6.4/types/stubs/awscli/clidriver/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      274 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/awscli/clidriver/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.484104 records_mover-1.6.4/types/stubs/boto3/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      271 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/boto3/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.484304 records_mover-1.6.4/types/stubs/boto3/session/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6001 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/boto3/session/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.484500 records_mover-1.6.4/types/stubs/botocore/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/botocore/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.484634 records_mover-1.6.4/types/stubs/botocore/credentials/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      503 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/botocore/credentials/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.484838 records_mover-1.6.4/types/stubs/chardet/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      434 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/chardet/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.485565 records_mover-1.6.4/types/stubs/config_resolver/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      137 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/config_resolver/__init__.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1809 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/config_resolver/core.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       41 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/config_resolver/exc.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.486450 records_mover-1.6.4/types/stubs/config_resolver/handler/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/config_resolver/handler/__init__.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      563 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/config_resolver/handler/base.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      596 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/config_resolver/handler/ini.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      594 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/config_resolver/handler/json.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      261 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/config_resolver/util.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.486645 records_mover-1.6.4/types/stubs/distutils/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/distutils/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.486818 records_mover-1.6.4/types/stubs/docstring_parser/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      804 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/docstring_parser/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.487125 records_mover-1.6.4/types/stubs/google/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.487269 records_mover-1.6.4/types/stubs/google/api_core/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/api_core/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.487403 records_mover-1.6.4/types/stubs/google/api_core/exceptions/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       35 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/api_core/exceptions/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.487658 records_mover-1.6.4/types/stubs/google/api_core/retry/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       21 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/api_core/retry/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.487852 records_mover-1.6.4/types/stubs/google/auth/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      156 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/auth/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.488067 records_mover-1.6.4/types/stubs/google/auth/credentials/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       28 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/auth/credentials/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.488253 records_mover-1.6.4/types/stubs/google/auth/exceptions/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       50 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/auth/exceptions/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.488452 records_mover-1.6.4/types/stubs/google/auth/service_account/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       97 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/auth/service_account/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.488628 records_mover-1.6.4/types/stubs/google/cloud/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.488748 records_mover-1.6.4/types/stubs/google/cloud/bigquery/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      218 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/bigquery/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.488929 records_mover-1.6.4/types/stubs/google/cloud/bigquery/client/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3364 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/bigquery/client/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.489132 records_mover-1.6.4/types/stubs/google/cloud/bigquery/dataset/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      295 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/bigquery/dataset/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.489331 records_mover-1.6.4/types/stubs/google/cloud/bigquery/dbapi/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/bigquery/dbapi/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.489466 records_mover-1.6.4/types/stubs/google/cloud/bigquery/dbapi/connection/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       88 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/bigquery/dbapi/connection/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.489655 records_mover-1.6.4/types/stubs/google/cloud/bigquery/encryption_configuration/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       39 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/bigquery/encryption_configuration/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.489900 records_mover-1.6.4/types/stubs/google/cloud/bigquery/external_config/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       39 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/bigquery/external_config/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.490158 records_mover-1.6.4/types/stubs/google/cloud/bigquery/job/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2804 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/bigquery/job/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.490343 records_mover-1.6.4/types/stubs/google/cloud/bigquery/retry/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       63 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/bigquery/retry/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.490522 records_mover-1.6.4/types/stubs/google/cloud/bigquery/schema/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       27 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/bigquery/schema/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.490699 records_mover-1.6.4/types/stubs/google/cloud/bigquery/table/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      181 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/bigquery/table/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.490877 records_mover-1.6.4/types/stubs/google/cloud/exceptions/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       35 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/exceptions/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.491061 records_mover-1.6.4/types/stubs/google/cloud/storage/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      678 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/storage/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.491283 records_mover-1.6.4/types/stubs/google/cloud/storage/blob/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      126 2024-05-09 21:22:14.000000 records_mover-1.6.4/types/stubs/google/cloud/storage/blob/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.491470 records_mover-1.6.4/types/stubs/google/cloud/storage/bucket/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      222 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/cloud/storage/bucket/__init__.py
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.491636 records_mover-1.6.4/types/stubs/google/oauth2/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/oauth2/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.491807 records_mover-1.6.4/types/stubs/google/oauth2/service_account/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      396 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/google/oauth2/service_account/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.492020 records_mover-1.6.4/types/stubs/googleapiclient/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/googleapiclient/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.492210 records_mover-1.6.4/types/stubs/googleapiclient/discovery/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      515 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/googleapiclient/discovery/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.492454 records_mover-1.6.4/types/stubs/googleapiclient/errors/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       40 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/googleapiclient/errors/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.492635 records_mover-1.6.4/types/stubs/httplib2/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       20 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/httplib2/__init__.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7092 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/inspect.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.492816 records_mover-1.6.4/types/stubs/jsonschema/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      253 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/jsonschema/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.493025 records_mover-1.6.4/types/stubs/jsonschema/exceptions/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       57 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/jsonschema/exceptions/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.494294 records_mover-1.6.4/types/stubs/logging/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6594 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/logging/__init__.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     2255 2023-01-24 16:33:00.000000 records_mover-1.6.4/types/stubs/logging/config.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      242 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/logging/filterer.py
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     7256 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/logging/handlers.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      841 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/logging/log_record.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     1732 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/logging/logger.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.494496 records_mover-1.6.4/types/stubs/requests/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       45 2024-05-09 21:22:14.000000 records_mover-1.6.4/types/stubs/requests/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.494675 records_mover-1.6.4/types/stubs/s3_concat/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      362 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/s3_concat/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.494863 records_mover-1.6.4/types/stubs/setuptools/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      352 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/setuptools/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.495132 records_mover-1.6.4/types/stubs/setuptools/command/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/setuptools/command/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.495270 records_mover-1.6.4/types/stubs/setuptools/command/install/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       80 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/setuptools/command/install/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.495493 records_mover-1.6.4/types/stubs/smart_open/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       17 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/smart_open/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.495691 records_mover-1.6.4/types/stubs/smart_open/gcs/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      535 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/smart_open/gcs/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.495895 records_mover-1.6.4/types/stubs/smart_open/s3/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)      649 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/smart_open/s3/__init__.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.496880 records_mover-1.6.4/types/stubs/sqlalchemy_redshift/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/sqlalchemy_redshift/__init__.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     6153 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/sqlalchemy_redshift/commands.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)       52 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/sqlalchemy_redshift/compat.pyi
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)     3400 2024-05-09 21:22:14.000000 records_mover-1.6.4/types/stubs/sqlalchemy_redshift/dialect.pyi
+drwxr-xr-x   0 brunocastrokarney   (502) staff       (20)        0 2024-05-14 18:25:00.497089 records_mover-1.6.4/types/stubs/tenacity/
+-rw-r--r--   0 brunocastrokarney   (502) staff       (20)        0 2022-12-13 16:38:59.000000 records_mover-1.6.4/types/stubs/tenacity/__init__.pyi
```

### Comparing `records-mover-1.6.3/LICENSE` & `records_mover-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/PKG-INFO` & `records_mover-1.6.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,269 +1,238 @@
-Metadata-Version: 2.1
-Name: records-mover
-Version: 1.6.3
-Summary: Library and CLI to move relational data from one place to another - DBs/CSV/gsheets/dataframes/...
-Home-page: UNKNOWN
-Author: Vince Broz
-Author-email: opensource@bluelabs.com
-License: Apache Software License
-Download-URL: https://github.com/bluelabsio/records-mover/tarball/1.6.3
-Description: <img
-         src="https://raw.githubusercontent.com/bluelabsio/records-mover/master/docs/records-mover-horizontal.png"
-         alt="Records Mover">
-        
-        [![Documentation Status](https://readthedocs.org/projects/records-mover/badge/?version=latest)](https://records-mover.readthedocs.io/en/latest/?badge=latest)
-        
-        [![CircleCI](https://dl.circleci.com/status-badge/img/gh/bluelabsio/records-mover/tree/main.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/bluelabsio/records-mover/tree/main)
-        
-        Records mover is a command-line tool and Python library you can
-        use to move relational data from one place to another.
-        
-        Relational data here means anything roughly "rectangular" - with
-        columns and rows.  For example, it supports reading and writing from:
-        
-        * Databases, including using native high-speed methods of
-          import/export of bulk data.  Redshift, Vertica and PostgreSQL are
-          well-supported, with some support for BigQuery and MySQL.
-        * CSV files
-        * Parquet files (initial support)
-        * Google Sheets
-        * Pandas DataFrames
-        * Records directories - a structured directory of CSV/Parquet/etc
-          files containing some JSON metadata about their format and origins.
-          Records directories are especially helpful for the ever-ambiguous
-          CSV format, where they solve the problem of 'hey, this may be a
-          CSV - but what's the schema?  What's the format of the CSV itself?
-          How is it escaped?'
-        
-        Records mover can be exended expand to handle additional databases
-        and data file types.  Databases are supported by building on top of
-        their [SQLAlchemy](https://www.sqlalchemy.org/) drivers.  Records
-        mover is able to auto-negotiate the most efficient way of moving data
-        from one to the other.
-        
-        ## CLI use example
-        
-        Installing:
-        
-        ```sh
-        pip3 install 'records_mover[cli,postgres-binary,redshift-binary]'
-        ```
-        
-        Loading a CSV into a database:
-        
-        ```sh
-        mvrec file2table foo.csv redshiftdb1 myschema1 mytable1
-        ```
-        
-        Copying a table from a PostgreSQL to a Redshift database:
-        
-        ```sh
-        mvrec --help
-        mvrec table2table postgresdb1 myschema1 mytable1 redshiftdb2 myschema2 mytable2
-        ```
-        
-        Note records mover will automatically build an appropriate `CREATE
-        TABLE` statement on the target end if the table doesn't already exist.
-        
-        Note that the connection details for the database names here must be
-        configured using
-        [db-facts](https://github.com/bluelabsio/db-facts/blob/master/CONFIGURATION.md).
-        
-        For more installation notes, see [INSTALL.md](./docs/INSTALL.md).  To
-        understand the security model here, see [SECURITY.md](./docs/SECURITY.md).
-        
-        ## CLI use demo (table creation and loading)
-        
-        <img src="https://i.imgur.com/PvmMhft.gif">
-        
-        ## Python library use example
-        
-        First, install records_mover.  We'll also use Pandas, so we'll install
-        that, too, as well as a driver for Postgres.
-        
-        ```sh
-        pip3 install records_mover[pandas,postgres-source]
-        ```
-        
-        Now we can run this code:
-        
-        ```python
-        #!/usr/bin/env python3
-        
-        # Pull in the records-mover library - be sure to run the pip install above first!
-        from records_mover import sources, targets, move
-        from pandas import DataFrame
-        import sqlalchemy
-        import os
-        
-        sqlalchemy_url = f"postgresql+psycopg2://username:{os.environ['DB_PASSWORD']}@hostname/database_name"
-        db_engine = sqlalchemy.create_engine(sqlalchemy_url)
-        
-        df = DataFrame.from_dict([{'a': 1}])  # or make your own!
-        
-        source = sources.dataframe(df=df)
-        target = targets.table(schema_name='myschema',
+<img
+ src="https://raw.githubusercontent.com/bluelabsio/records-mover/master/docs/records-mover-horizontal.png"
+ alt="Records Mover">
+
+[![Documentation Status](https://readthedocs.org/projects/records-mover/badge/?version=latest)](https://records-mover.readthedocs.io/en/latest/?badge=latest)
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/bluelabsio/records-mover/tree/main.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/bluelabsio/records-mover/tree/main)
+
+Records mover is a command-line tool and Python library you can
+use to move relational data from one place to another.
+
+Relational data here means anything roughly "rectangular" - with
+columns and rows.  For example, it supports reading and writing from:
+
+* Databases, including using native high-speed methods of
+  import/export of bulk data.  Redshift, Vertica and PostgreSQL are
+  well-supported, with some support for BigQuery and MySQL.
+* CSV files
+* Parquet files (initial support)
+* Google Sheets
+* Pandas DataFrames
+* Records directories - a structured directory of CSV/Parquet/etc
+  files containing some JSON metadata about their format and origins.
+  Records directories are especially helpful for the ever-ambiguous
+  CSV format, where they solve the problem of 'hey, this may be a
+  CSV - but what's the schema?  What's the format of the CSV itself?
+  How is it escaped?'
+
+Records mover can be exended expand to handle additional databases
+and data file types.  Databases are supported by building on top of
+their [SQLAlchemy](https://www.sqlalchemy.org/) drivers.  Records
+mover is able to auto-negotiate the most efficient way of moving data
+from one to the other.
+
+## CLI use example
+
+Installing:
+
+```sh
+pip3 install 'records_mover[cli,postgres-binary,redshift-binary]'
+```
+
+Loading a CSV into a database:
+
+```sh
+mvrec file2table foo.csv redshiftdb1 myschema1 mytable1
+```
+
+Copying a table from a PostgreSQL to a Redshift database:
+
+```sh
+mvrec --help
+mvrec table2table postgresdb1 myschema1 mytable1 redshiftdb2 myschema2 mytable2
+```
+
+Note records mover will automatically build an appropriate `CREATE
+TABLE` statement on the target end if the table doesn't already exist.
+
+Note that the connection details for the database names here must be
+configured using
+[db-facts](https://github.com/bluelabsio/db-facts/blob/master/CONFIGURATION.md).
+
+For more installation notes, see [INSTALL.md](./docs/INSTALL.md).  To
+understand the security model here, see [SECURITY.md](./docs/SECURITY.md).
+
+## CLI use demo (table creation and loading)
+
+<img src="https://i.imgur.com/PvmMhft.gif">
+
+## Python library use example
+
+First, install records_mover.  We'll also use Pandas, so we'll install
+that, too, as well as a driver for Postgres.
+
+```sh
+pip3 install records_mover[pandas,postgres-source]
+```
+
+Now we can run this code:
+
+```python
+#!/usr/bin/env python3
+
+# Pull in the records-mover library - be sure to run the pip install above first!
+from records_mover import sources, targets, move
+from pandas import DataFrame
+import sqlalchemy
+import os
+
+sqlalchemy_url = f"postgresql+psycopg2://username:{os.environ['DB_PASSWORD']}@hostname/database_name"
+db_engine = sqlalchemy.create_engine(sqlalchemy_url)
+
+df = DataFrame.from_dict([{'a': 1}])  # or make your own!
+
+source = sources.dataframe(df=df)
+target = targets.table(schema_name='myschema',
+                       table_name='mytable',
+                       db_engine=db_engine)
+results = move(source, target)
+```
+
+When moving data, the sources supported can be found
+[here](https://records-mover.readthedocs.io/en/latest/records_mover.records.sources.html),
+and the targets supported can be found
+[here](https://records-mover.readthedocs.io/en/latest/records_mover.records.targets.html).
+
+## Advanced Python library use example
+
+Here's another example, using some additional features:
+
+* Loading from an existing dataframe.
+* Secrets management using
+  [db-facts](https://github.com/bluelabsio/db-facts), which is a way
+  to configure credentials in YAML files or even fetch them
+  dynamically from your secrets store.
+* Logging configuration to show the internal processing steps (helpful
+  in optimizing performance or debugging issues)
+
+you can use this:
+
+```python
+#!/usr/bin/env python3
+
+# Pull in the records-mover library - be sure to run the pip install above first!
+from records_mover import Session
+from pandas import DataFrame
+
+session = Session()
+session.set_stream_logging()
+records = session.records
+
+db_engine = session.get_default_db_engine()
+
+df = DataFrame.from_dict([{'a': 1}])  # or make your own!
+
+source = records.sources.dataframe(df=df)
+target = records.targets.table(schema_name='myschema',
                                table_name='mytable',
                                db_engine=db_engine)
-        results = move(source, target)
-        ```
-        
-        When moving data, the sources supported can be found
-        [here](https://records-mover.readthedocs.io/en/latest/records_mover.records.sources.html),
-        and the targets supported can be found
-        [here](https://records-mover.readthedocs.io/en/latest/records_mover.records.targets.html).
-        
-        ## Advanced Python library use example
-        
-        Here's another example, using some additional features:
-        
-        * Loading from an existing dataframe.
-        * Secrets management using
-          [db-facts](https://github.com/bluelabsio/db-facts), which is a way
-          to configure credentials in YAML files or even fetch them
-          dynamically from your secrets store.
-        * Logging configuration to show the internal processing steps (helpful
-          in optimizing performance or debugging issues)
-        
-        you can use this:
-        
-        ```python
-        #!/usr/bin/env python3
-        
-        # Pull in the records-mover library - be sure to run the pip install above first!
-        from records_mover import Session
-        from pandas import DataFrame
-        
-        session = Session()
-        session.set_stream_logging()
-        records = session.records
-        
-        db_engine = session.get_default_db_engine()
-        
-        df = DataFrame.from_dict([{'a': 1}])  # or make your own!
-        
-        source = records.sources.dataframe(df=df)
-        target = records.targets.table(schema_name='myschema',
-                                       table_name='mytable',
-                                       db_engine=db_engine)
-        results = records.move(source, target)
-        ```
-        
-        ## Python library API documentation
-        
-        You can can find more API documentation
-        [here](https://records-mover.readthedocs.io/en/latest/index.html).
-        In particular, note:
-        
-        * [Session() constructor](https://records-mover.readthedocs.io/en/latest/records_mover.html#records_mover.Session.__init__)
-        * [sources factory methods](https://records-mover.readthedocs.io/en/latest/records_mover.records.sources.html)
-        * [targets factory methods](https://records-mover.readthedocs.io/en/latest/records_mover.records.targets.html)
-        * [move() method](https://records-mover.readthedocs.io/en/latest/records_mover.records.html#records_mover.records.move)
-        * [BaseRecordsFormat](https://records-mover.readthedocs.io/en/latest/records_mover.records.html#records_mover.records.base_records_format.BaseRecordsFormat)
-        
-        ## Local Development
-        
-        The included Dockerfile can be used to build a docker image that is
-        suitable for local development.
-        
-        ```bash
-        docker build Dockerfile.dev -t records-mover:latest .
-        ```
-        
-        Or, using docker compose,
-        ```bash
-        docker compose build
-        ```
-        
-        The following commands assume the records-mover container has been
-        named `records-mover`.
-        
-        Mount the directory containing your local copy of the repository to
-        have it override what's in the container.
-        
-        ```bash
-        docker run -it --mount src="$(pwd)/records_mover",target=/records-mover/records_mover,type=bind records-mover
-        ```
-        This will mount your local src overtop of the same directory in the
-        container. Mount any additional directories you are working on with
-        additional --mount entries
-        
-        Alternatively, you can launch the container using docker-compose.
-        This will start the container with pre-defined mounts.
-        ```
-        docker-compose up -d
-        ```
-        This will build the container image as necessary, launch it, and
-        mount the most relevant volumes for local dev.
-        The container is hosting a bash shell and will run until you
-        manually shut it down.
-        
-        Note, if you have to add a dependency to requirements.txt and want
-        to test it locally, add the line `COPY requirements.txt .` after
-        `RUN git clone ...` in the Dockerfile and rebuild the container.
-        
-        ### Working within the container
-        
-        The container presumes you're still working with python
-        virtual environments when working with it. This could possibly
-        be considered a "hat on a hat" situation.
-        The practical consequence of this is that if you do open a shell
-        in the container, ensure you activate the `venv` virtual
-        environment. Otherwise, you will not have all the dependencies
-        you'll need.
-        
-        After you've started a shell with the `docker run...` command above,
-        you can activate the virtual environment with:
-        ```
-        source venv/bin/activate
-        ```
-        
-        ### Running unit and type tests
-        
-        Unit and type tests can be run within the container by running:
-        ```
-        make citest
-        make cicoverage
-        make typecheck
-        make citypecoverage
-        ```
-        
-        The tests can be run from outside the container using docker-compose.
-        ```bash
-        docker compose run test
-        ```
-        It's theoretically possible to build sufficient additional
-        containers to support running integration tests locally but
-        that has not been planned yet.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Database :: Front-Ends
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: airflow
-Provides-Extra: db
-Provides-Extra: gsheets
-Provides-Extra: cli
-Provides-Extra: bigquery
-Provides-Extra: aws
-Provides-Extra: mysql
-Provides-Extra: redshift-binary
-Provides-Extra: redshift-source
-Provides-Extra: postgres-binary
-Provides-Extra: postgres-source
-Provides-Extra: vertica
-Provides-Extra: pandas
-Provides-Extra: literally_every_single_database_binary
-Provides-Extra: itest
-Provides-Extra: unittest
-Provides-Extra: typecheck
-Provides-Extra: gcs
-Provides-Extra: parquet
-Provides-Extra: docs
+results = records.move(source, target)
+```
+
+## Python library API documentation
+
+You can can find more API documentation
+[here](https://records-mover.readthedocs.io/en/latest/index.html).
+In particular, note:
+
+* [Session() constructor](https://records-mover.readthedocs.io/en/latest/records_mover.html#records_mover.Session.__init__)
+* [sources factory methods](https://records-mover.readthedocs.io/en/latest/records_mover.records.sources.html)
+* [targets factory methods](https://records-mover.readthedocs.io/en/latest/records_mover.records.targets.html)
+* [move() method](https://records-mover.readthedocs.io/en/latest/records_mover.records.html#records_mover.records.move)
+* [BaseRecordsFormat](https://records-mover.readthedocs.io/en/latest/records_mover.records.html#records_mover.records.base_records_format.BaseRecordsFormat)
+
+## Local Development
+
+The included Dockerfile can be used to build a docker image that is
+suitable for local development.
+
+```bash
+docker build Dockerfile.dev -t records-mover:latest .
+```
+
+Or, using docker compose,
+```bash
+docker compose build
+```
+
+The following commands assume the records-mover container has been
+named `records-mover`.
+
+Mount the directory containing your local copy of the repository to
+have it override what's in the container.
+
+```bash
+docker run -it --mount src="$(pwd)/records_mover",target=/records-mover/records_mover,type=bind records-mover
+```
+This will mount your local src overtop of the same directory in the
+container. Mount any additional directories you are working on with
+additional --mount entries
+
+Alternatively, you can launch the container using docker-compose.
+This will start the container with pre-defined mounts.
+```
+docker-compose up -d
+```
+This will build the container image as necessary, launch it, and
+mount the most relevant volumes for local dev.
+The container is hosting a bash shell and will run until you
+manually shut it down.
+
+Note, if you have to add a dependency to requirements.txt and want
+to test it locally, add the line `COPY requirements.txt .` after
+`RUN git clone ...` in the Dockerfile and rebuild the container.
+
+### Working within the container
+
+The container presumes you're still working with python
+virtual environments when working with it. This could possibly
+be considered a "hat on a hat" situation.
+The practical consequence of this is that if you do open a shell
+in the container, ensure you activate the `venv` virtual
+environment. Otherwise, you will not have all the dependencies
+you'll need.
+
+After you've started a shell with the `docker run...` command above,
+you can activate the virtual environment with:
+```
+source venv/bin/activate
+```
+
+### Running unit and type tests
+
+Unit and type tests can be run within the container by running:
+```
+make citest
+make cicoverage
+make typecheck
+make citypecoverage
+```
+
+The tests can be run from outside the container using docker-compose.
+```bash
+docker compose run test
+```
+It's theoretically possible to build sufficient additional
+containers to support running integration tests locally but
+that has not been planned yet.
+
+### In-progress airbyte integration
+
+Currently in progress integration airbyte as an alternative engine for executing
+source <-> destination transfers. This functionality is currently behind a
+feature flag. To enable all airbyte features in your environment, set the
+following environment variable:
+```bash
+export RECORDS_MOVER_AIRBYTE_ENABLED=1
+```
```

### Comparing `records-mover-1.6.3/records_mover/__init__.py` & `records_mover-1.6.4/records_mover/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/airflow/hooks/google_cloud_credentials_hook.py` & `records_mover-1.6.4/records_mover/airflow/hooks/google_cloud_credentials_hook.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/airflow/hooks/records_hook.py` & `records_mover-1.6.4/records_mover/airflow/hooks/records_hook.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/airflow/hooks/sqlalchemy_db_hook.py` & `records_mover-1.6.4/records_mover/airflow/hooks/sqlalchemy_db_hook.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/check_db_conn_engine.py` & `records_mover-1.6.4/records_mover/check_db_conn_engine.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/cli/job_config_schema_as_args_parser.py` & `records_mover-1.6.4/records_mover/cli/job_config_schema_as_args_parser.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/creds/base_creds.py` & `records_mover-1.6.4/records_mover/creds/base_creds.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from .database import db_facts_from_env
 from typing import TYPE_CHECKING, Iterable, Union, Optional, Dict, Any
 from records_mover.mover_types import PleaseInfer
 from config_resolver import get_config
 import os
 import logging
 if TYPE_CHECKING:
-    # see the 'gsheets' extras_require option in setup.py - needed for this!
     import google.auth.credentials  # noqa
     import boto3  # noqa
 
 
 logger = logging.getLogger(__name__)
 
 _GSHEETS_SCOPES = ('https://www.googleapis.com/auth/spreadsheets',)
@@ -50,27 +49,32 @@
                                            'google.cloud.storage.Client',
                                            None] = PleaseInfer.token,
                  scratch_s3_url: Union[PleaseInfer,
                                        str,
                                        None] = PleaseInfer.token,
                  scratch_gcs_url: Union[PleaseInfer,
                                         str,
-                                        None] = PleaseInfer.token) -> None:
+                                        None] = PleaseInfer.token,
+                 default_airbyte_creds: Union[PleaseInfer,
+                                              Dict[str, Any],
+                                              None] = PleaseInfer.token) -> None:
         self._default_db_creds_name = default_db_creds_name
         self._default_aws_creds_name = default_aws_creds_name
         self._default_gcp_creds_name = default_gcp_creds_name
 
         self.__default_db_facts = default_db_facts
         self.__default_gcs_creds = default_gcp_creds
         self.__default_gcs_client = default_gcs_client
         self.__default_boto3_session = default_boto3_session
 
         self._scratch_s3_url = scratch_s3_url
         self._scratch_gcs_url = scratch_gcs_url
 
+        self._default_airbyte_creds = default_airbyte_creds
+
     def google_sheets(self, gcp_creds_name: str) -> 'google.auth.credentials.Credentials':
         scopes = _GSHEETS_SCOPES
         return self._gcp_creds(gcp_creds_name, scopes)
 
     def gcs(self, gcp_creds_name: str) -> 'google.auth.credentials.Credentials':
         scopes = _GCS_SCOPES
         return self._gcp_creds(gcp_creds_name, scopes)
@@ -262,7 +266,15 @@
             logger.debug('No config ini file found')
             return None
 
     def default_scratch_gcs_url(self) -> Optional[str]:
         if self._scratch_gcs_url is PleaseInfer.token:
             self._scratch_gcs_url = self._infer_scratch_gcs_url()
         return self._scratch_gcs_url
+
+    def _infer_airbyte_creds(self) -> Dict[str, Any]:
+        raise NotImplementedError
+
+    def airbyte(self) -> Optional[Dict[str, Any]]:
+        if self._default_airbyte_creds is PleaseInfer.token:
+            self._default_airbyte_creds = self._infer_airbyte_creds()
+        return self._default_airbyte_creds
```

### Comparing `records-mover-1.6.3/records_mover/creds/creds_via_airflow.py` & `records_mover-1.6.4/records_mover/creds/creds_via_airflow.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/creds/creds_via_env.py` & `records_mover-1.6.4/records_mover/creds/creds_via_env.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 from db_facts import db
 import os
 import base64
 import json
-from typing import Iterable, Optional
+from typing import Iterable, Optional, Any, Dict
 from .base_creds import BaseCreds
 from typing import TYPE_CHECKING
 from db_facts.db_facts_types import DBFacts
 if TYPE_CHECKING:
     # see the 'gsheets' extras_require option in setup.py - needed for this!
     import google.auth.credentials  # noqa
     import boto3  # noqa
 
 
 class CredsViaEnv(BaseCreds):
-    def _gcp_creds_from_env(self,
-                            scopes: Iterable[str]) ->\
-            Optional['google.auth.credentials.Credentials']:
+    def _infer_airbyte_creds(self) -> Dict[str, Any]:
+        if 'AIRBYTE_CONNECTION' not in os.environ:
+            return {}
+        return {
+            'user': 'username',
+            'host': 'host',
+            'port': 0,
+            'endpoint': 'endpoint',
+            'password': 'password',
+        }
+
+    def _gcp_creds_from_env(self, scopes: Iterable[str]) \
+            -> Optional['google.auth.credentials.Credentials']:
         if 'GCP_SERVICE_ACCOUNT_JSON_BASE64' not in os.environ:
             return None
         import google.oauth2.service_account
         json_base64 = os.environ['GCP_SERVICE_ACCOUNT_JSON_BASE64']
         json_str = base64.b64decode(json_base64.encode('utf-8'))
         cred_details = json.loads(json_str)
```

### Comparing `records-mover-1.6.3/records_mover/creds/creds_via_lastpass.py` & `records_mover-1.6.4/records_mover/creds/creds_via_lastpass.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,30 @@
 from db_facts.lpass import lpass_field
 from db_facts.db_facts_types import DBFacts
 import json
 from typing import Iterable
 from .base_creds import BaseCreds
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    # see the 'gsheets' extras_require option in setup.py - needed for this!
     import google.auth.credentials  # noqa
     import boto3  # noqa
 
 
 class CredsViaLastPass(BaseCreds):
+    def _infer_airbyte_creds(self) -> dict:
+        # Magic string! Huzzah. Assumes you have this entry in your local password manager
+        cred_name = 'airbyte'
+        return {
+            'user': lpass_field(cred_name, 'username'),
+            'host': lpass_field(cred_name, 'host'),
+            'port': int(lpass_field(cred_name, 'port')),
+            'endpoint': lpass_field(cred_name, 'endpoint'),
+            'password': lpass_field(cred_name, 'password'),
+        }
+
     def _gcp_creds(self, gcp_creds_name: str,
                    scopes: Iterable[str]) -> 'google.auth.credentials.Credentials':
         import google.oauth2.service_account
         notes_json = lpass_field(gcp_creds_name, 'notes')
         cred_details = json.loads(notes_json)
 
         return google.oauth2.service_account.Credentials.\
```

### Comparing `records-mover-1.6.3/records_mover/creds/database.py` & `records_mover-1.6.4/records_mover/creds/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,11 +27,10 @@
         redshift_base_url_values = {
             name.lower(): value
             for name, value in os.environ.items()
             if name.startswith('REDSHIFT_SPECTRUM_BASE_URL_')
         }
 
         db_facts.update(redshift_base_url_values)
-
         if None in db_facts.values():
             raise NotImplementedError("Please run with with-db or set DB_* environment variables")
     return db_facts  # type: ignore
```

### Comparing `records-mover-1.6.3/records_mover/db/bigquery/bigquery_db_driver.py` & `records_mover-1.6.4/records_mover/db/bigquery/bigquery_db_driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/bigquery/load_job_config_options.py` & `records_mover-1.6.4/records_mover/db/bigquery/load_job_config_options.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/bigquery/loader.py` & `records_mover-1.6.4/records_mover/db/bigquery/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/bigquery/unloader.py` & `records_mover-1.6.4/records_mover/db/bigquery/unloader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/connect.py` & `records_mover-1.6.4/records_mover/db/connect.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/db_conn_mixin.py` & `records_mover-1.6.4/records_mover/db/db_conn_mixin.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/db_type.py` & `records_mover-1.6.4/records_mover/db/db_type.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/driver.py` & `records_mover-1.6.4/records_mover/db/driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/factory.py` & `records_mover-1.6.4/records_mover/db/factory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/loader.py` & `records_mover-1.6.4/records_mover/db/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/mysql/load_options.py` & `records_mover-1.6.4/records_mover/db/mysql/load_options.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/mysql/loader.py` & `records_mover-1.6.4/records_mover/db/mysql/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/mysql/mysql_db_driver.py` & `records_mover-1.6.4/records_mover/db/mysql/mysql_db_driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/postgres/copy_options/__init__.py` & `records_mover-1.6.4/records_mover/db/postgres/copy_options/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/postgres/copy_options/common.py` & `records_mover-1.6.4/records_mover/db/postgres/copy_options/common.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/postgres/copy_options/csv.py` & `records_mover-1.6.4/records_mover/db/postgres/copy_options/csv.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/postgres/copy_options/date_input_style.py` & `records_mover-1.6.4/records_mover/db/postgres/copy_options/date_input_style.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/postgres/copy_options/date_output_style.py` & `records_mover-1.6.4/records_mover/db/postgres/copy_options/date_output_style.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/postgres/copy_options/text.py` & `records_mover-1.6.4/records_mover/db/postgres/copy_options/text.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/postgres/copy_options/types.py` & `records_mover-1.6.4/records_mover/db/postgres/copy_options/types.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/postgres/loader.py` & `records_mover-1.6.4/records_mover/db/postgres/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/postgres/postgres_db_driver.py` & `records_mover-1.6.4/records_mover/db/postgres/postgres_db_driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/postgres/sqlalchemy_postgres_copy.py` & `records_mover-1.6.4/records_mover/db/postgres/sqlalchemy_postgres_copy.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/postgres/unloader.py` & `records_mover-1.6.4/records_mover/db/postgres/unloader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/quoting.py` & `records_mover-1.6.4/records_mover/db/quoting.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/redshift/loader.py` & `records_mover-1.6.4/records_mover/db/redshift/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/redshift/records_copy.py` & `records_mover-1.6.4/records_mover/db/redshift/records_copy.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/redshift/records_unload.py` & `records_mover-1.6.4/records_mover/db/redshift/records_unload.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/redshift/redshift_db_driver.py` & `records_mover-1.6.4/records_mover/db/redshift/redshift_db_driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/redshift/sql.py` & `records_mover-1.6.4/records_mover/db/redshift/sql.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/redshift/unloader.py` & `records_mover-1.6.4/records_mover/db/redshift/unloader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/unloader.py` & `records_mover-1.6.4/records_mover/db/unloader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/vertica/export_sql.py` & `records_mover-1.6.4/records_mover/db/vertica/export_sql.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/vertica/import_sql.py` & `records_mover-1.6.4/records_mover/db/vertica/import_sql.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/vertica/loader.py` & `records_mover-1.6.4/records_mover/db/vertica/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/vertica/records_export_options.py` & `records_mover-1.6.4/records_mover/db/vertica/records_export_options.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/vertica/records_import_options.py` & `records_mover-1.6.4/records_mover/db/vertica/records_import_options.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/vertica/unloader.py` & `records_mover-1.6.4/records_mover/db/vertica/unloader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/db/vertica/vertica_db_driver.py` & `records_mover-1.6.4/records_mover/db/vertica/vertica_db_driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/logging.py` & `records_mover-1.6.4/records_mover/logging.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/mover_types.py` & `records_mover-1.6.4/records_mover/mover_types.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/pandas/__init__.py` & `records_mover-1.6.4/records_mover/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/__init__.py` & `records_mover-1.6.4/records_mover/records/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/base_records_format.py` & `records_mover-1.6.4/records_mover/records/base_records_format.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/cli.py` & `records_mover-1.6.4/records_mover/records/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """CLI to move records from place to place"""
 import argparse
 from odictliteral import odict
+from .airbyte.airbyte import AirbyteEngine
 from .job.schema import method_to_json_schema
 from .job.mover import run_records_mover_job
 from ..utils.json_schema import method_signature_to_json_schema
 from .processing_instructions import ProcessingInstructions
-from records_mover.cli.job_config_schema_as_args_parser import (JobConfigSchemaAsArgsParser,
-                                                                arguments_output_to_config)
+from records_mover.cli.job_config_schema_as_args_parser import (
+    JobConfigSchemaAsArgsParser, arguments_output_to_config
+)
 from records_mover.logging import set_stream_logging
 from ..mover_types import JsonSchema, JobConfig
 from ..version import __version__
 import sys
+import os
 from typing import Callable, Dict, Any, TYPE_CHECKING
 if TYPE_CHECKING:
     from records_mover import Session
 
 
 def populate_subparser(bootstrap_session: 'Session',
                        sub_parser: argparse.ArgumentParser,
@@ -78,18 +81,23 @@
                                         special_handling={},
                                         parameters_to_ignore=['self'])
     JobConfigSchemaAsArgsParser(config_json_schema=pi_config_schema,
                                 argument_parser=parser).configure_arg_parser()
 
     # https://stackoverflow.com/questions/15405636/pythons-argparse-to-show-programs-version-with-prog-and-version-string-formatt
     parser.add_argument('-V', '--version', action='version', version="%(prog)s ("+__version__+")")
+
+    airbyte_feature_flag = os.getenv('RECORDS_MOVER_AIRBYTE_ENABLED')
+    if airbyte_feature_flag is not None:
+        parser.add_argument('-hc', '--healthcheck', action='store_true', required=False,
+                            help='Returns health of the configured airbyte instance')
+
     subparsers = parser.add_subparsers(help='subcommand_help')
     from records_mover import Session
     bootstrap_session = Session()
-
     for source in sources:
         for target in targets:
             name = f"{source}2{target}"
             sub_parser = subparsers.add_parser(name, help=f"Copy from {source} to {target}")
             source_method_name = source_method_name_by_cli_name[source]
             target_method_name = target_method_name_by_cli_name[target]
             job_config_schema = \
@@ -110,15 +118,25 @@
     warnings.filterwarnings("ignore",
                             "Your application has authenticated using end user credentials")
 
     parser = build_parser()
     args = parser.parse_args()
     raw_config = vars(args)
     func = getattr(args, 'func', None)
-    if func is None:
+    healthcheck = getattr(args, 'healthcheck', False)
+    if healthcheck:
+        from records_mover import Session
+        session = Session()
+        engine = AirbyteEngine(session)
+        result = engine.healthcheck()
+        if result:
+            print("Airbyte Status: OK!")
+        else:
+            print("Airbyte Status: Unhealthy")
+    elif func is None:
         parser.print_help()
     else:
         set_stream_logging()
         try:
             func(raw_config)
         except Exception:
             # This is logged above using a redacting logger
```

### Comparing `records-mover-1.6.3/records_mover/records/delimited/__init__.py` & `records_mover-1.6.4/records_mover/records/delimited/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/delimited/compression.py` & `records_mover-1.6.4/records_mover/records/delimited/compression.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/delimited/conversions.py` & `records_mover-1.6.4/records_mover/records/delimited/conversions.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/delimited/csv_streamer.py` & `records_mover-1.6.4/records_mover/records/delimited/csv_streamer.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/delimited/hint.py` & `records_mover-1.6.4/records_mover/records/delimited/hint.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/delimited/hints.py` & `records_mover-1.6.4/records_mover/records/delimited/hints.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/delimited/sniff.py` & `records_mover-1.6.4/records_mover/records/delimited/sniff.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/delimited/types.py` & `records_mover-1.6.4/records_mover/records/delimited/types.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/delimited/utils.py` & `records_mover-1.6.4/records_mover/records/delimited/utils.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/delimited/validated_records_hints.py` & `records_mover-1.6.4/records_mover/records/delimited/validated_records_hints.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/deprecated.py` & `records_mover-1.6.4/records_mover/records/deprecated.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/existing_table_handling.py` & `records_mover-1.6.4/records_mover/records/existing_table_handling.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/job/config.py` & `records_mover-1.6.4/records_mover/records/job/config.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/job/mover.py` & `records_mover-1.6.4/records_mover/records/job/mover.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/job/schema.py` & `records_mover-1.6.4/records_mover/records/job/schema.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/mover.py` & `records_mover-1.6.4/records_mover/records/mover.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/pandas/__init__.py` & `records_mover-1.6.4/records_mover/records/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/pandas/prep_for_csv.py` & `records_mover-1.6.4/records_mover/records/pandas/prep_for_csv.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/pandas/read_csv_options.py` & `records_mover-1.6.4/records_mover/records/pandas/read_csv_options.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/pandas/to_csv_options.py` & `records_mover-1.6.4/records_mover/records/pandas/to_csv_options.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/prep.py` & `records_mover-1.6.4/records_mover/records/prep.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/prep_and_load.py` & `records_mover-1.6.4/records_mover/records/prep_and_load.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/processing_instructions.py` & `records_mover-1.6.4/records_mover/records/processing_instructions.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/records.py` & `records_mover-1.6.4/records_mover/records/records.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/records_directory.py` & `records_mover-1.6.4/records_mover/records/records_directory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/records_format.py` & `records_mover-1.6.4/records_mover/records/records_format.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/records_format_file.py` & `records_mover-1.6.4/records_mover/records/records_format_file.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/records_schema_json_file.py` & `records_mover-1.6.4/records_mover/records/records_schema_json_file.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/records_types.py` & `records_mover-1.6.4/records_mover/records/records_types.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/results.py` & `records_mover-1.6.4/records_mover/records/results.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/__init__.py` & `records_mover-1.6.4/records_mover/records/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/field/__init__.py` & `records_mover-1.6.4/records_mover/records/schema/field/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/field/constraints/constraints.py` & `records_mover-1.6.4/records_mover/records/schema/field/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/field/constraints/decimal.py` & `records_mover-1.6.4/records_mover/records/schema/field/constraints/decimal.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/field/constraints/integer.py` & `records_mover-1.6.4/records_mover/records/schema/field/constraints/integer.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/field/constraints/string.py` & `records_mover-1.6.4/records_mover/records/schema/field/constraints/string.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/field/numpy.py` & `records_mover-1.6.4/records_mover/records/schema/field/numpy.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/field/pandas.py` & `records_mover-1.6.4/records_mover/records/schema/field/pandas.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/field/representation.py` & `records_mover-1.6.4/records_mover/records/schema/field/representation.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/field/sqlalchemy.py` & `records_mover-1.6.4/records_mover/records/schema/field/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/field/statistics.py` & `records_mover-1.6.4/records_mover/records/schema/field/statistics.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/field/string_length_generator.py` & `records_mover-1.6.4/records_mover/records/schema/field/string_length_generator.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/schema/__init__.py` & `records_mover-1.6.4/records_mover/records/schema/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/schema/known_representation.py` & `records_mover-1.6.4/records_mover/records/schema/schema/known_representation.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/schema/pandas.py` & `records_mover-1.6.4/records_mover/records/schema/schema/pandas.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/schema/schema/sqlalchemy.py` & `records_mover-1.6.4/records_mover/records/schema/schema/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/sources/base.py` & `records_mover-1.6.4/records_mover/records/sources/base.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/sources/data_url.py` & `records_mover-1.6.4/records_mover/records/sources/data_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/sources/dataframes.py` & `records_mover-1.6.4/records_mover/records/sources/dataframes.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/sources/directory.py` & `records_mover-1.6.4/records_mover/records/sources/directory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/sources/factory.py` & `records_mover-1.6.4/records_mover/records/sources/factory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/sources/fileobjs.py` & `records_mover-1.6.4/records_mover/records/sources/fileobjs.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/sources/google_sheets.py` & `records_mover-1.6.4/records_mover/records/sources/google_sheets.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/sources/table.py` & `records_mover-1.6.4/records_mover/records/sources/table.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/sources/uninferred_fileobjs.py` & `records_mover-1.6.4/records_mover/records/sources/uninferred_fileobjs.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/table.py` & `records_mover-1.6.4/records_mover/records/table.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/base.py` & `records_mover-1.6.4/records_mover/records/targets/base.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/data_url.py` & `records_mover-1.6.4/records_mover/records/targets/data_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/directory_from_url.py` & `records_mover-1.6.4/records_mover/records/targets/directory_from_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/factory.py` & `records_mover-1.6.4/records_mover/records/targets/factory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/fileobj.py` & `records_mover-1.6.4/records_mover/records/targets/fileobj.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/google_sheets.py` & `records_mover-1.6.4/records_mover/records/targets/google_sheets.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/spectrum.py` & `records_mover-1.6.4/records_mover/records/targets/spectrum.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/table/base.py` & `records_mover-1.6.4/records_mover/records/targets/table/base.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/table/move_from_dataframes_source.py` & `records_mover-1.6.4/records_mover/records/targets/table/move_from_dataframes_source.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/table/move_from_fileobjs_source.py` & `records_mover-1.6.4/records_mover/records/targets/table/move_from_fileobjs_source.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/table/move_from_records_directory.py` & `records_mover-1.6.4/records_mover/records/targets/table/move_from_records_directory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/table/move_from_temp_loc_after_filling_it.py` & `records_mover-1.6.4/records_mover/records/targets/table/move_from_temp_loc_after_filling_it.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/records/targets/table/target.py` & `records_mover-1.6.4/records_mover/records/targets/table/target.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/session.py` & `records_mover-1.6.4/records_mover/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,23 +270,23 @@
         kwargs = {}
         scratch_s3_url = self.creds.default_scratch_s3_url()
         if scratch_s3_url is not None:
             try:
                 s3_temp_base_loc = self.directory_url(scratch_s3_url)
                 kwargs['s3_temp_base_loc'] = s3_temp_base_loc
             except NotImplementedError:
-                logger.debug('boto3 not installed', exc_info=True)
+                logger.debug('boto3 not installed', exc_info=False)
 
         scratch_gcs_url = self.creds.default_scratch_gcs_url()
         if scratch_gcs_url is not None:
             try:
                 gcs_temp_base_loc = self.directory_url(scratch_gcs_url)
                 kwargs['gcs_temp_base_loc'] = gcs_temp_base_loc
             except NotImplementedError:
-                logger.debug('google.cloud.storage not installed', exc_info=True)
+                logger.debug('google.cloud.storage not installed', exc_info=False)
 
         return db_driver(db=db,
                          db_conn=db_conn,
                          db_engine=db_engine,
                          url_resolver=self.url_resolver,
                          **kwargs)
```

### Comparing `records-mover-1.6.3/records_mover/url/base.py` & `records_mover-1.6.4/records_mover/url/base.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/url/filesystem.py` & `records_mover-1.6.4/records_mover/url/filesystem.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/url/gcs/gcs_directory_url.py` & `records_mover-1.6.4/records_mover/url/gcs/gcs_directory_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/url/gcs/gcs_file_url.py` & `records_mover-1.6.4/records_mover/url/gcs/gcs_file_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         parsed = urlparse(url)
         self.blob = unquote(parsed.path[1:])
         self.bucket = parsed.netloc
         self.client = gcs_client
         self.credentials = gcp_credentials
         self.bucket_obj = self.client.bucket(self.bucket)
 
+    def exists(self) -> bool:
+        return self.bucket_obj.blob(self.blob).exists()
+
     def open(self, mode: str = "rb") -> IO[bytes]:
         try:
             return gs_open(bucket_id=self.bucket,
                            blob_id=self.blob,
                            mode=mode,
                            client=self.client)
         except google.api_core.exceptions.NotFound:
```

### Comparing `records-mover-1.6.3/records_mover/url/resolver.py` & `records_mover-1.6.4/records_mover/url/resolver.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,35 +18,39 @@
 file_url_ctors: Dict[str, Union[Type[BaseFileUrl], CreatesUrls]] = {}
 
 
 def init_urls() -> None:
     try:
         from .s3.s3_url import S3Url
     except ModuleNotFoundError:
-        logger.debug('No S3 support', exc_info=True)
+        logger.debug('No S3 support', exc_info=False)
         S3Url = None  # type: ignore
     try:
         from .gcs.gcs_file_url import GCSFileUrl
         from .gcs.gcs_directory_url import GCSDirectoryUrl
     except ModuleNotFoundError:
-        logger.debug('No Google Cloud Storage support', exc_info=True)
+        logger.debug('No Google Cloud Storage support', exc_info=False)
         GCSFileUrl = None  # type: ignore
         GCSDirectoryUrl = None  # type: ignore
     from .filesystem import FilesystemDirectoryUrl, FilesystemFileUrl
     from .http import HttpFileUrl
     if len(directory_url_ctors) == 0:
         if S3Url is not None:
+            logger.debug('Resolved using S3 URL')
             directory_url_ctors['s3'] = S3Url
         if GCSDirectoryUrl is not None:
+            logger.debug('Resolved using GCS URL')
             directory_url_ctors['gs'] = GCSDirectoryUrl
         directory_url_ctors['file'] = FilesystemDirectoryUrl
     if len(file_url_ctors) == 0:
         if S3Url is not None:
+            logger.debug('Resolved using S3 URL')
             file_url_ctors['s3'] = S3Url
         if GCSFileUrl is not None:
+            logger.debug('Resolved using GCS URL')
             file_url_ctors['gs'] = GCSFileUrl
         file_url_ctors['file'] = FilesystemFileUrl
 
         file_url_ctors['http'] = HttpFileUrl
         file_url_ctors['https'] = HttpFileUrl
```

### Comparing `records-mover-1.6.3/records_mover/url/s3/awscli.py` & `records_mover-1.6.4/records_mover/url/s3/awscli.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/url/s3/s3_base_url.py` & `records_mover-1.6.4/records_mover/url/s3/s3_base_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/url/s3/s3_directory_url.py` & `records_mover-1.6.4/records_mover/url/s3/s3_directory_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/url/s3/s3_file_url.py` & `records_mover-1.6.4/records_mover/url/s3/s3_file_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/url/s3/s3_url.py` & `records_mover-1.6.4/records_mover/url/s3/s3_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/utils/__init__.py` & `records_mover-1.6.4/records_mover/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/utils/concat_files.py` & `records_mover-1.6.4/records_mover/utils/concat_files.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/utils/json_schema.py` & `records_mover-1.6.4/records_mover/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/utils/json_schema_array_document.py` & `records_mover-1.6.4/records_mover/utils/json_schema_array_document.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/utils/json_schema_document.py` & `records_mover-1.6.4/records_mover/utils/json_schema_document.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/utils/lazyprop.py` & `records_mover-1.6.4/records_mover/utils/lazyprop.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/utils/limits.py` & `records_mover-1.6.4/records_mover/utils/limits.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/utils/retry.py` & `records_mover-1.6.4/records_mover/utils/retry.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/utils/rewound_fileobj.py` & `records_mover-1.6.4/records_mover/utils/rewound_fileobj.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/records_mover/utils/structures.py` & `records_mover-1.6.4/records_mover/utils/structures.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.6.3/setup.cfg` & `records_mover-1.6.4/setup.cfg`

 * *Files identical despite different names*

