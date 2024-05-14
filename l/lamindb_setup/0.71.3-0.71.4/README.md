# Comparing `tmp/lamindb_setup-0.71.3.tar.gz` & `tmp/lamindb_setup-0.71.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.71.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.71.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.71.3.tar` & `lamindb_setup-0.71.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     8499 2024-05-06 20:56:01.582100 lamindb_setup-0.71.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.71.3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.71.3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.71.3/.gitignore
--rw-r--r--   0        0        0     1474 2024-04-25 16:11:02.471704 lamindb_setup-0.71.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.71.3/LICENSE
--rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.71.3/README.md
--rw-r--r--   0        0        0   100577 2024-05-06 21:23:12.374422 lamindb_setup-0.71.3/docs/changelog.md
--rw-r--r--   0        0        0     2574 2024-04-29 07:49:33.469384 lamindb_setup-0.71.3/docs/hub-cloud/01-init-local-instance.ipynb
--rw-r--r--   0        0        0     3948 2024-04-27 13:43:14.991516 lamindb_setup-0.71.3/docs/hub-cloud/02-connect-local-instance.ipynb
--rw-r--r--   0        0        0    10272 2024-05-06 20:56:01.583161 lamindb_setup-0.71.3/docs/hub-cloud/03-add-managed-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-04-25 13:58:37.156407 lamindb_setup-0.71.3/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     3191 2024-05-03 13:28:51.894897 lamindb_setup-0.71.3/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     3886 2024-05-03 13:28:51.895365 lamindb_setup-0.71.3/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     5454 2024-04-30 14:26:00.292361 lamindb_setup-0.71.3/docs/hub-cloud/07-keep-artifacts-local.ipynb
--rw-r--r--   0        0        0     3160 2024-04-25 13:58:37.156237 lamindb_setup-0.71.3/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472152 lamindb_setup-0.71.3/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-04-29 07:29:41.597110 lamindb_setup-0.71.3/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-04-25 13:58:37.175784 lamindb_setup-0.71.3/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-04-25 13:58:37.157085 lamindb_setup-0.71.3/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2712 2024-04-27 13:43:14.991856 lamindb_setup-0.71.3/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-04-25 13:58:37.174178 lamindb_setup-0.71.3/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-04-25 13:58:37.139783 lamindb_setup-0.71.3/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-04-25 13:58:37.137631 lamindb_setup-0.71.3/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6182 2024-04-27 13:43:14.992063 lamindb_setup-0.71.3/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472299 lamindb_setup-0.71.3/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.71.3/docs/index.md
--rw-r--r--   0        0        0      513 2024-04-30 14:26:00.292603 lamindb_setup-0.71.3/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.71.3/docs/reference.md
--rw-r--r--   0        0        0     1542 2024-05-06 21:22:59.437710 lamindb_setup-0.71.3/lamindb_setup/__init__.py
--rw-r--r--   0        0        0      846 2024-04-25 16:11:02.473229 lamindb_setup-0.71.3/lamindb_setup/_cache.py
--rw-r--r--   0        0        0      129 2024-04-25 16:11:02.473531 lamindb_setup-0.71.3/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2613 2024-04-25 16:11:02.473724 lamindb_setup-0.71.3/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1186 2024-04-25 16:11:02.473895 lamindb_setup-0.71.3/lamindb_setup/_close.py
--rw-r--r--   0        0        0    12600 2024-05-06 16:12:29.980099 lamindb_setup-0.71.3/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     7232 2024-05-03 15:45:13.866583 lamindb_setup-0.71.3/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1534 2024-04-25 16:11:02.474852 lamindb_setup-0.71.3/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2120 2024-04-25 16:11:02.475059 lamindb_setup-0.71.3/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1874 2024-04-25 16:11:02.475261 lamindb_setup-0.71.3/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11924 2024-05-06 10:09:29.480733 lamindb_setup-0.71.3/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     8815 2024-04-27 13:43:14.993255 lamindb_setup-0.71.3/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      940 2024-04-30 14:26:00.294512 lamindb_setup-0.71.3/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      679 2024-04-25 16:11:02.476265 lamindb_setup-0.71.3/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1268 2024-05-03 10:05:44.386575 lamindb_setup-0.71.3/lamindb_setup/_set_managed_storage.py
--rw-r--r--   0        0        0     3670 2024-04-25 16:11:02.476440 lamindb_setup-0.71.3/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1568 2024-04-25 16:11:02.476624 lamindb_setup-0.71.3/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      416 2024-04-30 14:26:00.294783 lamindb_setup-0.71.3/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     1799 2024-04-25 16:11:02.477005 lamindb_setup-0.71.3/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2520 2024-04-25 16:11:02.477187 lamindb_setup-0.71.3/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      276 2024-04-25 16:11:02.477423 lamindb_setup-0.71.3/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5504 2024-04-25 16:11:02.477677 lamindb_setup-0.71.3/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    15971 2024-05-06 14:14:11.656183 lamindb_setup-0.71.3/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4859 2024-05-03 10:05:44.387393 lamindb_setup-0.71.3/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1875 2024-04-25 16:11:02.478546 lamindb_setup-0.71.3/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3141 2024-04-30 14:26:00.295688 lamindb_setup-0.71.3/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    16588 2024-04-30 14:26:00.296030 lamindb_setup-0.71.3/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3922 2024-05-03 10:05:44.387683 lamindb_setup-0.71.3/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2704 2024-05-03 10:05:44.387946 lamindb_setup-0.71.3/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    12382 2024-05-03 10:05:44.388316 lamindb_setup-0.71.3/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     2084 2024-05-03 10:05:44.388614 lamindb_setup-0.71.3/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1344 2024-05-06 21:22:57.114573 lamindb_setup-0.71.3/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     3002 2024-04-25 16:11:02.481032 lamindb_setup-0.71.3/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6893 2024-04-27 13:43:14.995437 lamindb_setup-0.71.3/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     3542 2024-05-06 21:22:57.114756 lamindb_setup-0.71.3/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      305 2024-04-25 16:11:02.481611 lamindb_setup-0.71.3/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2218 2024-04-27 13:43:14.995719 lamindb_setup-0.71.3/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      532 2024-04-25 16:11:02.482026 lamindb_setup-0.71.3/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    28342 2024-05-06 11:31:20.317968 lamindb_setup-0.71.3/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     3325 2024-04-30 14:26:00.297371 lamindb_setup-0.71.3/noxfile.py
--rw-r--r--   0        0        0     4138 2024-04-30 14:26:00.297636 lamindb_setup-0.71.3/pyproject.toml
--rw-r--r--   0        0        0     5387 2024-05-06 20:56:01.584052 lamindb_setup-0.71.3/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      270 2024-05-03 10:05:44.388882 lamindb_setup-0.71.3/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     5716 2024-05-03 10:05:44.389145 lamindb_setup-0.71.3/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      538 2024-04-25 16:11:02.483601 lamindb_setup-0.71.3/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      504 2024-04-25 16:11:02.483785 lamindb_setup-0.71.3/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      482 2024-05-03 10:05:44.389367 lamindb_setup-0.71.3/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0      595 2024-05-06 20:56:01.584848 lamindb_setup-0.71.3/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11234 2024-05-06 20:56:01.585107 lamindb_setup-0.71.3/tests/hub-local/test_all.py
--rw-r--r--   0        0        0      734 2024-04-30 14:26:00.298827 lamindb_setup-0.71.3/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      401 2024-04-25 16:11:02.484790 lamindb_setup-0.71.3/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      193 2024-04-25 16:11:02.484963 lamindb_setup-0.71.3/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1469 2024-04-25 16:11:02.485160 lamindb_setup-0.71.3/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0     1109 2024-04-30 14:26:00.299030 lamindb_setup-0.71.3/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1642 2024-04-27 13:43:14.997388 lamindb_setup-0.71.3/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     2023 2024-04-27 13:43:14.997583 lamindb_setup-0.71.3/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      891 2024-05-03 15:45:13.867354 lamindb_setup-0.71.3/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      878 2024-04-25 16:11:02.486161 lamindb_setup-0.71.3/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1058 2024-04-25 16:11:02.486329 lamindb_setup-0.71.3/tests/storage/test_to_url.py
--rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.71.3/PKG-INFO
+-rw-r--r--   0        0        0     8499 2024-05-07 15:02:32.273843 lamindb_setup-0.71.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-02-29 12:04:01.937708 lamindb_setup-0.71.4/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-02-29 12:04:01.937784 lamindb_setup-0.71.4/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-02-29 12:04:01.937868 lamindb_setup-0.71.4/.gitignore
+-rw-r--r--   0        0        0     1474 2024-04-29 09:50:29.256493 lamindb_setup-0.71.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-02-29 12:04:01.938089 lamindb_setup-0.71.4/LICENSE
+-rw-r--r--   0        0        0      265 2024-02-29 12:04:01.938164 lamindb_setup-0.71.4/README.md
+-rw-r--r--   0        0        0   101357 2024-05-14 11:22:43.186340 lamindb_setup-0.71.4/docs/changelog.md
+-rw-r--r--   0        0        0     2574 2024-04-29 09:50:29.257640 lamindb_setup-0.71.4/docs/hub-cloud/01-init-local-instance.ipynb
+-rw-r--r--   0        0        0     3948 2024-04-29 09:50:29.257800 lamindb_setup-0.71.4/docs/hub-cloud/02-connect-local-instance.ipynb
+-rw-r--r--   0        0        0    10851 2024-05-13 09:56:45.668066 lamindb_setup-0.71.4/docs/hub-cloud/03-add-managed-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-03-07 19:17:51.102702 lamindb_setup-0.71.4/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3191 2024-05-03 13:46:52.497497 lamindb_setup-0.71.4/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3886 2024-05-03 13:46:52.498391 lamindb_setup-0.71.4/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     5454 2024-05-02 14:13:25.437615 lamindb_setup-0.71.4/docs/hub-cloud/07-keep-artifacts-local.ipynb
+-rw-r--r--   0        0        0     3160 2024-03-07 19:17:51.103066 lamindb_setup-0.71.4/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      177 2024-04-29 09:50:29.259621 lamindb_setup-0.71.4/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-03-07 19:17:51.103480 lamindb_setup-0.71.4/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-03-25 10:01:42.202871 lamindb_setup-0.71.4/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-03-19 12:58:36.468528 lamindb_setup-0.71.4/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2712 2024-04-29 09:50:29.259864 lamindb_setup-0.71.4/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-03-11 10:42:56.000471 lamindb_setup-0.71.4/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-03-07 19:17:51.104281 lamindb_setup-0.71.4/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-03-07 19:17:51.104386 lamindb_setup-0.71.4/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6182 2024-04-29 09:50:29.260752 lamindb_setup-0.71.4/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      177 2024-04-29 09:50:29.260962 lamindb_setup-0.71.4/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-02-29 12:04:01.938771 lamindb_setup-0.71.4/docs/index.md
+-rw-r--r--   0        0        0      513 2024-05-02 14:13:25.438254 lamindb_setup-0.71.4/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-02-29 12:04:01.940681 lamindb_setup-0.71.4/docs/reference.md
+-rw-r--r--   0        0        0     1542 2024-05-14 11:22:19.685276 lamindb_setup-0.71.4/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-29 09:50:29.261873 lamindb_setup-0.71.4/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0      129 2024-04-29 09:50:29.262000 lamindb_setup-0.71.4/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2613 2024-04-29 09:50:29.262479 lamindb_setup-0.71.4/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1186 2024-04-29 09:50:29.263120 lamindb_setup-0.71.4/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    12728 2024-05-09 13:59:53.552357 lamindb_setup-0.71.4/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     5498 2024-05-09 13:59:53.553371 lamindb_setup-0.71.4/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1534 2024-04-29 09:50:29.264420 lamindb_setup-0.71.4/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2120 2024-04-29 09:50:29.265153 lamindb_setup-0.71.4/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1874 2024-04-29 09:50:29.265389 lamindb_setup-0.71.4/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11897 2024-05-13 09:56:45.669008 lamindb_setup-0.71.4/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     8815 2024-04-29 09:50:29.266219 lamindb_setup-0.71.4/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      940 2024-05-02 14:13:25.440107 lamindb_setup-0.71.4/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      679 2024-04-29 09:50:29.266496 lamindb_setup-0.71.4/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1419 2024-05-13 09:56:45.669863 lamindb_setup-0.71.4/lamindb_setup/_set_managed_storage.py
+-rw-r--r--   0        0        0     3670 2024-04-29 09:50:29.266915 lamindb_setup-0.71.4/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1568 2024-04-29 09:50:29.267349 lamindb_setup-0.71.4/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      416 2024-05-02 14:13:25.440536 lamindb_setup-0.71.4/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     1799 2024-04-29 09:50:29.268812 lamindb_setup-0.71.4/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2520 2024-04-29 09:50:29.269069 lamindb_setup-0.71.4/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      276 2024-04-29 09:50:29.269197 lamindb_setup-0.71.4/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5504 2024-04-29 09:50:29.269650 lamindb_setup-0.71.4/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    16043 2024-05-09 13:59:53.554745 lamindb_setup-0.71.4/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4859 2024-05-03 10:21:42.522659 lamindb_setup-0.71.4/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1875 2024-04-29 09:50:29.270865 lamindb_setup-0.71.4/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3141 2024-05-02 14:13:25.441639 lamindb_setup-0.71.4/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    16191 2024-05-09 13:59:53.555705 lamindb_setup-0.71.4/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3922 2024-05-03 10:21:42.523183 lamindb_setup-0.71.4/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2704 2024-05-03 10:21:42.523417 lamindb_setup-0.71.4/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    12751 2024-05-13 09:56:45.670685 lamindb_setup-0.71.4/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     2084 2024-05-03 10:21:42.524061 lamindb_setup-0.71.4/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1344 2024-05-07 15:02:32.276034 lamindb_setup-0.71.4/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     3002 2024-04-29 09:50:29.273885 lamindb_setup-0.71.4/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6893 2024-04-29 09:50:29.274411 lamindb_setup-0.71.4/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     3542 2024-05-13 09:56:43.703710 lamindb_setup-0.71.4/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      305 2024-04-29 09:50:29.274891 lamindb_setup-0.71.4/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2269 2024-05-13 09:56:45.671582 lamindb_setup-0.71.4/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      532 2024-04-29 09:50:29.276245 lamindb_setup-0.71.4/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    28342 2024-05-06 16:40:35.041470 lamindb_setup-0.71.4/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     3325 2024-05-02 14:13:25.443812 lamindb_setup-0.71.4/noxfile.py
+-rw-r--r--   0        0        0     4138 2024-04-29 09:50:29.278441 lamindb_setup-0.71.4/pyproject.toml
+-rw-r--r--   0        0        0     5387 2024-05-07 15:02:32.277415 lamindb_setup-0.71.4/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      270 2024-05-03 10:21:42.524497 lamindb_setup-0.71.4/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     5716 2024-05-03 10:21:42.524786 lamindb_setup-0.71.4/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      538 2024-04-29 09:50:29.279431 lamindb_setup-0.71.4/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      504 2024-04-29 09:50:29.279656 lamindb_setup-0.71.4/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      482 2024-05-03 10:21:42.525026 lamindb_setup-0.71.4/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0      595 2024-05-07 15:02:32.277929 lamindb_setup-0.71.4/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11234 2024-05-07 15:02:32.278778 lamindb_setup-0.71.4/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0      772 2024-05-09 13:59:53.556852 lamindb_setup-0.71.4/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      401 2024-04-29 09:50:29.281008 lamindb_setup-0.71.4/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      193 2024-04-29 09:50:29.281261 lamindb_setup-0.71.4/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1469 2024-04-29 09:50:29.281514 lamindb_setup-0.71.4/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0     1109 2024-04-29 09:50:29.281652 lamindb_setup-0.71.4/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1642 2024-04-29 09:50:29.281814 lamindb_setup-0.71.4/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     2023 2024-04-29 09:50:29.281965 lamindb_setup-0.71.4/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      891 2024-05-05 15:00:22.453756 lamindb_setup-0.71.4/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      878 2024-04-29 09:50:29.283900 lamindb_setup-0.71.4/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1058 2024-04-29 09:50:29.283991 lamindb_setup-0.71.4/tests/storage/test_to_url.py
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.71.4/PKG-INFO
```

### Comparing `lamindb_setup-0.71.3/.github/workflows/build.yml` & `lamindb_setup-0.71.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/.github/workflows/latest-changes.yml` & `lamindb_setup-0.71.4/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/.gitignore` & `lamindb_setup-0.71.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/.pre-commit-config.yaml` & `lamindb_setup-0.71.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/LICENSE` & `lamindb_setup-0.71.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/changelog.md` & `lamindb_setup-0.71.4/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-♻️ Better treatment of current_user_id | [754](https://github.com/laminlabs/lamindb-setup/pull/754) | [falexwolf](https://github.com/falexwolf) | 2024-05-06 | 0.72.2
+⚡️ Speed-up file hash | [761](https://github.com/laminlabs/lamindb-setup/pull/761) | [Koncopd](https://github.com/Koncopd) | 2024-05-11 | 0.71.4
+♻️ Account for public storage locations | [758](https://github.com/laminlabs/lamindb-setup/pull/758) | [falexwolf](https://github.com/falexwolf) | 2024-05-10 |
+♻️ Make init_instance_hub idempotent | [757](https://github.com/laminlabs/lamindb-setup/pull/757) | [falexwolf](https://github.com/falexwolf) | 2024-05-09 |
+♻️ Refactor delete & connect | [756](https://github.com/laminlabs/lamindb-setup/pull/756) | [falexwolf](https://github.com/falexwolf) | 2024-05-09 |
+🔥 Remove laminapp-admin logic | [755](https://github.com/laminlabs/lamindb-setup/pull/755) | [falexwolf](https://github.com/falexwolf) | 2024-05-08 |
+♻️ Better treatment of current_user_id | [754](https://github.com/laminlabs/lamindb-setup/pull/754) | [falexwolf](https://github.com/falexwolf) | 2024-05-06 | 0.71.2
 💚 Fix tests | [753](https://github.com/laminlabs/lamindb-setup/pull/753) | [fredericenard](https://github.com/fredericenard) | 2024-05-06 |
 ♻️ Actually use local db | [751](https://github.com/laminlabs/lamindb-setup/pull/751) | [falexwolf](https://github.com/falexwolf) | 2024-05-06 | 0.71.2
 ✏️ Restore view_tree py3.9 compatibility | [750](https://github.com/laminlabs/lamindb-setup/pull/750) | [sunnyosun](https://github.com/sunnyosun) | 2024-05-06 |
 💚 Pin laminapp-ui | [749](https://github.com/laminlabs/lamindb-setup/pull/749) | [falexwolf](https://github.com/falexwolf) | 2024-05-06 |
 ♻️ Extend valid suffixes to composite suffixes | [746](https://github.com/laminlabs/lamindb-setup/pull/746) | [falexwolf](https://github.com/falexwolf) | 2024-05-03 | 0.71.1
 🐛 Fix test failures | [745](https://github.com/laminlabs/lamindb-setup/pull/745) | [Koncopd](https://github.com/Koncopd) | 2024-05-03 |
 ♻️ Persist keep-artifacts-local in settings.env | [743](https://github.com/laminlabs/lamindb-setup/pull/743) | [falexwolf](https://github.com/falexwolf) | 2024-05-03 |
```

### Comparing `lamindb_setup-0.71.3/docs/hub-cloud/01-init-local-instance.ipynb` & `lamindb_setup-0.71.4/docs/hub-cloud/01-init-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-cloud/02-connect-local-instance.ipynb` & `lamindb_setup-0.71.4/docs/hub-cloud/02-connect-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-cloud/03-add-managed-storage.ipynb` & `lamindb_setup-0.71.4/docs/hub-cloud/03-add-managed-storage.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9931587837837839%*

 * *Differences: {"'cells'": "{21: {'source': {insert: [(7, ')\\n'), (8, 'assert "*

 * *            "ln_setup.settings.storage._instance_id is not None')], delete: [7]}}, insert: [(25, "*

 * *            "OrderedDict([('cell_type', 'markdown'), ('id', '015b8f36'), ('metadata', "*

 * *            "OrderedDict()), ('source', ['Cloud storage with mere read access:'])])), (26, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', '4ef50cab'), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source' […]*

```diff
@@ -251,15 +251,16 @@
                 "assert ln_setup.settings.storage.type_is_cloud\n",
                 "assert ln_setup.settings.storage.root_as_str == \"s3://lamindb-ci/storage3\"\n",
                 "assert ln_setup.settings.storage.region == \"us-west-1\"\n",
                 "assert (ln_setup.settings.storage.root / \".lamindb/_is_initialized\").read_text() == ln_setup.settings.storage.uid\n",
                 "# root.fs contains the underlying fsspec filesystem\n",
                 "assert (\n",
                 "    ln_setup.settings.storage.root.fs.cache_regions  # set by lamindb to True for s3 by default\n",
-                ")"
+                ")\n",
+                "assert ln_setup.settings.storage._instance_id is not None"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ae953b6a",
             "metadata": {},
             "source": [
@@ -285,14 +286,34 @@
             "source": [
                 "# test cache_regions\n",
                 "assert not ln_setup.settings.storage.root.fs.cache_regions"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "015b8f36",
+            "metadata": {},
+            "source": [
+                "Cloud storage with mere read access:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "4ef50cab",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "with pytest.raises(ValueError) as error:\n",
+                "    set_managed_storage(\"gs://rxrx1-europe-west4/images/test/HEPG2-08\")\n",
+                "assert error.exconly().startswith(\"ValueError: Cannot manage storage without write access\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "83a2ee6b",
             "metadata": {},
             "source": [
                 "Add testuser2 as a collaborator to the instance:"
             ]
         },
         {
```

### Comparing `lamindb_setup-0.71.3/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.71.4/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.71.4/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.71.4/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-cloud/07-keep-artifacts-local.ipynb` & `lamindb_setup-0.71.4/docs/hub-cloud/07-keep-artifacts-local.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.71.4/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.71.4/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.71.4/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.71.4/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.71.4/docs/hub-prod/test-empty-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.71.4/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.71.4/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.71.4/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.71.4/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/docs/notebooks.md` & `lamindb_setup-0.71.4/docs/notebooks.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/__init__.py` & `lamindb_setup-0.71.4/lamindb_setup/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.71.3"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.71.4"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._check_setup import _check_instance_setup
 from ._close import close
```

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_cache.py` & `lamindb_setup-0.71.4/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_check_setup.py` & `lamindb_setup-0.71.4/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_close.py` & `lamindb_setup-0.71.4/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.71.4/lamindb_setup/_connect_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,18 @@
         and db_dsn_hub.host == db_dsn_local.host
         and db_dsn_hub.database == db_dsn_local.database
         and db_dsn_hub.port == db_dsn_local.port
     )
 
 
 def update_db_using_local(
-    hub_instance_result: dict[str, str], settings_file: Path, db: str | None = None
+    hub_instance_result: dict[str, str],
+    settings_file: Path,
+    db: str | None = None,
+    raise_permission_error=True,
 ) -> str | None:
     db_updated = None
     # check if postgres
     if hub_instance_result["db_scheme"] == "postgresql":
         db_dsn_hub = LaminDsnModel(db=hub_instance_result["db"])
         if db is not None:
             db_dsn_local = LaminDsnModel(db=db)
@@ -73,15 +76,19 @@
             elif settings_file.exists() and (
                 "read" in db_dsn_hub.db.user or db_dsn_hub.db.user is None
             ):
                 isettings = load_instance_settings(settings_file)
                 db_dsn_local = LaminDsnModel(db=isettings.db)
             else:
                 # just take the default hub result and ensure there is actually a user
-                if db_dsn_hub.db.user == "none" and db_dsn_hub.db.password == "none":
+                if (
+                    db_dsn_hub.db.user == "none"
+                    and db_dsn_hub.db.password == "none"
+                    and raise_permission_error
+                ):
                     raise PermissionError(
                         "No database access, please ask your admin to provide you with"
                         " a DB URL and pass it via --db <db_url>"
                     )
                 db_dsn_local = db_dsn_hub
         if not check_db_dsn_equal_up_to_credentials(db_dsn_hub.db, db_dsn_local.db):
             raise ValueError(
@@ -97,14 +104,73 @@
             host=db_dsn_hub.db.host,
             port=db_dsn_hub.db.port,
             database=db_dsn_hub.db.database,
         )
     return db_updated
 
 
+def _connect_instance(
+    owner: str,
+    name: str,
+    *,
+    db: str | None = None,
+    raise_permission_error: bool = True,
+) -> InstanceSettings:
+    settings_file = instance_settings_file(name, owner)
+    make_hub_request = True
+    if settings_file.exists():
+        isettings = load_instance_settings(settings_file)
+        # skip hub request for a purely local instance
+        make_hub_request = isettings.is_remote
+    if make_hub_request:
+        # the following will return a string if the instance does not exist
+        # on the hub
+        hub_result = load_instance_from_hub(owner=owner, name=name)
+        # if hub_result is not a string, it means it made a request
+        # that successfully returned metadata
+        if not isinstance(hub_result, str):
+            instance_result, storage_result = hub_result
+            db_updated = update_db_using_local(
+                instance_result,
+                settings_file,
+                db=db,
+                raise_permission_error=raise_permission_error,
+            )
+            ssettings = StorageSettings(
+                root=storage_result["root"],
+                region=storage_result["region"],
+                uid=storage_result["lnid"],
+                uuid=UUID(storage_result["id"]),
+                instance_id=UUID(instance_result["id"]),
+            )
+            isettings = InstanceSettings(
+                id=UUID(instance_result["id"]),
+                owner=owner,
+                name=name,
+                storage=ssettings,
+                db=db_updated,
+                schema=instance_result["schema_str"],
+                git_repo=instance_result["git_repo"],
+                keep_artifacts_local=bool(instance_result["keep_artifacts_local"]),
+                is_on_hub=True,
+            )
+            check_whether_migrations_in_sync(instance_result["lamindb_version"])
+        else:
+            message = INSTANCE_NOT_FOUND_MESSAGE.format(
+                owner=owner, name=name, hub_result=hub_result
+            )
+            if settings_file.exists():
+                isettings = load_instance_settings(settings_file)
+                if isettings.is_remote:
+                    raise InstanceNotFoundError(message)
+            else:
+                raise InstanceNotFoundError(message)
+    return isettings
+
+
 @unlock_cloud_sqlite_upon_exception(ignore_prev_locker=True)
 def connect(
     slug: str,
     *,
     db: str | None = None,
     storage: UPathStr | None = None,
     _raise_not_found_error: bool = True,
@@ -130,79 +196,30 @@
                 logger.info(f"connected lamindb: {settings.instance.slug}")
                 return None
             else:
                 raise RuntimeError(MESSAGE_NO_MULTIPLE_INSTANCE)
         elif settings._instance_exists and f"{owner}/{name}" != settings.instance.slug:
             close_instance(mute=True)
 
-        settings_file = instance_settings_file(name, owner)
-
-        make_hub_request = True
-        if settings_file.exists():
-            isettings = load_instance_settings(settings_file)
-            # mimic instance_result from hub
-            instance_result = {"id": isettings._id.hex}
-            # skip hub request for a purely local instance
-            make_hub_request = isettings.is_remote
-
-        if make_hub_request:
-            # the following will return a string if the instance does not exist
-            # on the hub
-            hub_result = load_instance_from_hub(owner=owner, name=name)
-            # if hub_result is not a string, it means it made a request
-            # that successfully returned metadata
-            if not isinstance(hub_result, str):
-                instance_result, storage_result = hub_result
-                db_updated = update_db_using_local(
-                    instance_result, settings_file, db=db
-                )
-                ssettings = StorageSettings(
-                    root=storage_result["root"],
-                    region=storage_result["region"],
-                    uid=storage_result["lnid"],
-                    uuid=UUID(storage_result["id"]),
-                    instance_id=UUID(instance_result["id"]),
-                )
-                isettings = InstanceSettings(
-                    id=UUID(instance_result["id"]),
-                    owner=owner,
-                    name=name,
-                    storage=ssettings,
-                    db=db_updated,
-                    schema=instance_result["schema_str"],
-                    git_repo=instance_result["git_repo"],
-                    keep_artifacts_local=bool(instance_result["keep_artifacts_local"]),
-                    is_on_hub=True,
-                )
-                check_whether_migrations_in_sync(instance_result["lamindb_version"])
+        try:
+            isettings = _connect_instance(owner, name, db=db)
+        except InstanceNotFoundError as e:
+            if _raise_not_found_error:
+                raise e
             else:
-                message = INSTANCE_NOT_FOUND_MESSAGE.format(
-                    owner=owner, name=name, hub_result=hub_result
-                )
-                if settings_file.exists():
-                    isettings = load_instance_settings(settings_file)
-                    if isettings.is_remote:
-                        if _raise_not_found_error:
-                            raise InstanceNotFoundError(message)
-                        return "instance-not-found"
-
-                else:
-                    if _raise_not_found_error:
-                        raise InstanceNotFoundError(message)
-                    return "instance-not-found"
-
+                return "instance-not-found"
+        if isinstance(isettings, str):
+            return isettings
         if storage is not None:
             update_isettings_with_storage(isettings, storage)
         isettings._persist()
         if _test:
             return None
         silence_loggers()
-        check, msg = isettings._load_db(
-            do_not_lock_for_laminapp_admin=True
-        )  # this also updates local SQLite
+        check, msg = isettings._load_db()
         if not check:
             local_db = (
                 isettings._is_cloud_sqlite and isettings._sqlite_file_local.exists()
             )
             if local_db:
                 logger.warning(
                     "SQLite file does not exist in the cloud, but exists locally:"
@@ -212,15 +229,15 @@
             elif _raise_not_found_error:
                 raise SystemExit(msg)
             else:
                 logger.warning(
                     f"instance exists with id {isettings._id.hex}, but database is not"
                     " loadable: re-initializing"
                 )
-                return "instance-corrupted-or-deleted", instance_result
+                return "instance-corrupted-or-deleted"
         # this is for testing purposes only
         if _TEST_FAILED_LOAD:
             raise RuntimeError("Technical testing error.")
 
         if storage is not None and isettings.dialect == "sqlite":
             update_root_field_in_default_storage(isettings)
         # below is for backfilling the instance_uid value
```

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_django.py` & `lamindb_setup-0.71.4/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_exportdb.py` & `lamindb_setup-0.71.4/lamindb_setup/_exportdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_importdb.py` & `lamindb_setup-0.71.4/lamindb_setup/_importdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_init_instance.py` & `lamindb_setup-0.71.4/lamindb_setup/_init_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,51 +40,52 @@
 
 def register_storage_in_instance(ssettings: StorageSettings):
     from lnschema_core.models import Storage
     from lnschema_core.users import current_user_id
 
     from .core.hashing import hash_and_encode_as_b62
 
-    assert ssettings._instance_id is not None
-
+    if ssettings._instance_id is not None:
+        instance_uid = hash_and_encode_as_b62(ssettings._instance_id.hex)[:12]
+    else:
+        instance_uid = None
     # how do we ensure that this function is only called passing
     # the managing instance?
     defaults = {
         "root": ssettings.root_as_str,
         "type": ssettings.type,
         "region": ssettings.region,
-        "instance_uid": hash_and_encode_as_b62(ssettings._instance_id.hex)[:12],
+        "instance_uid": instance_uid,
         "created_by_id": current_user_id(),
     }
     if ssettings._uid is not None:
         defaults["uid"] = ssettings._uid
     storage, _ = Storage.objects.update_or_create(
         root=ssettings.root_as_str,
         defaults=defaults,
     )
     return storage
 
 
 def register_user(usettings):
     from lnschema_core.models import User
 
-    if usettings.handle != "laminapp-admin":
-        try:
-            # need to have try except because of integer primary key migration
-            user, created = User.objects.update_or_create(
-                uid=usettings.uid,
-                defaults={
-                    "handle": usettings.handle,
-                    "name": usettings.name,
-                },
-            )
-        # for users with only read access, except via ProgrammingError
-        # ProgrammingError: permission denied for table lnschema_core_user
-        except (OperationalError, FieldError, ProgrammingError):
-            pass
+    try:
+        # need to have try except because of integer primary key migration
+        user, created = User.objects.update_or_create(
+            uid=usettings.uid,
+            defaults={
+                "handle": usettings.handle,
+                "name": usettings.name,
+            },
+        )
+    # for users with only read access, except via ProgrammingError
+    # ProgrammingError: permission denied for table lnschema_core_user
+    except (OperationalError, FieldError, ProgrammingError):
+        pass
 
 
 def register_user_and_storage_in_instance(isettings: InstanceSettings, usettings):
     """Register user & storage in DB."""
     from django.db.utils import OperationalError
 
     try:
```

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_migrate.py` & `lamindb_setup-0.71.4/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_register_instance.py` & `lamindb_setup-0.71.4/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_schema.py` & `lamindb_setup-0.71.4/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_set_managed_storage.py` & `lamindb_setup-0.71.4/lamindb_setup/_set_managed_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,11 +27,15 @@
     if not settings.instance.is_on_hub:
         raise ValueError(
             "Can't add additional managed storage locations for instances that aren't managed through the hub."
         )
     ssettings = init_storage(
         root=root, instance_id=settings.instance._id, register_hub=True
     )
+    if ssettings._instance_id is None:
+        raise ValueError(
+            f"Cannot manage storage without write access: {ssettings.root}"
+        )
     settings.instance._storage = ssettings
     settings.instance._persist()  # this also updates the settings object
     register_storage_in_instance(ssettings)
     settings.storage._set_fs_kwargs(**fs_kwargs)
```

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_setup_user.py` & `lamindb_setup-0.71.4/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.71.4/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_aws_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_hub_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,17 +280,19 @@
         fields.update(db_fields)
     # I'd like the following to be an upsert, but this seems to violate RLS
     # Similarly, if we don't specify `returning="minimal"`, we'll violate RLS
     # we could make this idempotent by catching an error, but this seems dangerous
     # as then init_instance is no longer idempotent
     try:
         client.table("instance").insert(fields, returning="minimal").execute()
-    except APIError as e:
-        logger.warning("instance likely already exists")
-        raise e
+    except APIError:
+        logger.warning(
+            f"instance already existed at: https://lamin.ai/{isettings.owner}/{isettings.name}"
+        )
+        return None
     client.table("storage").update(
         {"instance_id": isettings._id.hex, "is_default": True}
     ).eq("id", isettings.storage._uuid.hex).execute()  # type: ignore
     logger.important(f"go to: https://lamin.ai/{isettings.owner}/{isettings.name}")
 
 
 def connect_instance(
```

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_settings.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_settings_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         name: str,  # instance name
         storage: StorageSettings,  # storage location
         keep_artifacts_local: bool = False,  # default to local storage
         uid: str | None = None,  # instance uid/lnid
         db: str | None = None,  # DB URI
         schema: str | None = None,  # comma-separated string of schema names
         git_repo: str | None = None,  # a git repo URL
-        is_on_hub: bool = False,  # initialized from hub
+        is_on_hub: bool | None = None,  # initialized from hub
     ):
         from ._hub_utils import validate_db_arg
 
         self._id_: UUID = id
         self._owner: str = owner
         self._name: str = name
         self._uid: str | None = uid
@@ -402,38 +402,29 @@
         settings._instance_settings = self
 
     def _init_db(self):
         from .django import setup_django
 
         setup_django(self, init=True)
 
-    def _load_db(
-        self, do_not_lock_for_laminapp_admin: bool = False
-    ) -> tuple[bool, str]:
+    def _load_db(self) -> tuple[bool, str]:
         # Is the database available and initialized as LaminDB?
         # returns a tuple of status code and message
         if self.dialect == "sqlite" and not self._sqlite_file.exists():
             legacy_file = self.storage.key_to_filepath(f"{self.name}.lndb")
             if legacy_file.exists():
                 raise RuntimeError(
                     "The SQLite file has been renamed!\nPlease rename your SQLite file"
                     f" {legacy_file} to {self._sqlite_file}"
                 )
             return False, f"SQLite file {self._sqlite_file} does not exist"
         from lamindb_setup import settings  # to check user
 
         from .django import setup_django
 
-        # lock in all cases except if do_not_lock_for_laminapp_admin is True and
-        # user is `laminapp-admin`
-        # value doesn't matter if not a cloud sqlite instance
-        lock_cloud_sqlite = self._is_cloud_sqlite and (
-            not do_not_lock_for_laminapp_admin
-            or settings.user.handle != "laminapp-admin"
-        )
         # we need the local sqlite to setup django
-        self._update_local_sqlite_file(lock_cloud_sqlite=lock_cloud_sqlite)
+        self._update_local_sqlite_file(lock_cloud_sqlite=self._is_cloud_sqlite)
         # setting up django also performs a check for migrations & prints them
         # as warnings
         # this should fail, e.g., if the db is not reachable
         setup_django(self)
         return True, ""
```

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_settings_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,19 +109,28 @@
         uid=uid,
         root=root_str,
         region=region,
         instance_id=instance_id,
     )
     # the below might update the uid with one that's already taken on the hub
     if ssettings.type_is_cloud or register_hub:
+        from ._hub_core import delete_storage_record
         from ._hub_core import init_storage as init_storage_hub
 
         init_storage_hub(ssettings)
     # below comes last only if everything else was successful
-    mark_storage_root(ssettings.root, ssettings.uid)  # type: ignore
+    try:
+        mark_storage_root(ssettings.root, ssettings.uid)  # type: ignore
+    except Exception:
+        logger.important(
+            f"due to lack of write access, LaminDB won't manage storage location: {ssettings.root}"
+        )
+        if ssettings._uuid is not None:
+            delete_storage_record(ssettings._uuid)  # type: ignore
+        ssettings._instance_id = None
     return ssettings
 
 
 def _process_cache_path(cache_path: str | Path | UPath | None):
     if cache_path is None or cache_path == "null":
         return None
     cache_dir = UPath(cache_path)
```

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.71.4/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.71.4/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/django.py` & `lamindb_setup-0.71.4/lamindb_setup/core/django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/hashing.py` & `lamindb_setup-0.71.4/lamindb_setup/core/hashing.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,47 +36,50 @@
 # a lot to read about this: lamin-notes/2022/hashing
 def hash_set(s: set[str]) -> str:
     bstr = ":".join(sorted(s)).encode("utf-8")
     # as we're truncating at 20 b64, we choose md5 over sha512
     return to_b64_str(hashlib.md5(bstr).digest())[:20]
 
 
-def hash_md5s_from_dir(etags: list[str]) -> tuple[str, str]:
+def hash_md5s_from_dir(hashes: list[str]) -> tuple[str, str]:
     # need to sort below because we don't want the order of parsing the dir to
     # affect the hash
     digests = b"".join(
-        hashlib.md5(etag.encode("utf-8")).digest() for etag in sorted(etags)
+        hashlib.md5(hash.encode("utf-8")).digest() for hash in sorted(hashes)
     )
     digest = hashlib.md5(digests).digest()
     return to_b64_str(digest)[:22], "md5-d"
 
 
 def hash_code(file_path: UPathStr):
     with open(file_path, "rb") as fp:
         data = fp.read()
     data_size = len(data)
     header = f"blob {data_size}\0".encode()
     blob = header + data
     return hashlib.sha1(blob)
 
 
-def hash_file(file_path: Path, chunk_size=50 * 1024 * 1024) -> tuple[str, str]:
-    chunks = []
+def hash_file(
+    file_path: Path,
+    file_size: int | None = None,
+    chunk_size: int | None = 50 * 1024 * 1024,
+) -> tuple[str, str]:
     with open(file_path, "rb") as fp:
-        # read first chunk
-        chunks = [fp.read(chunk_size)]
-        # try reading the 2nd chunk
-        data = fp.read(chunk_size)
-        if data:
-            # go to end of file
+        if file_size is None:
+            fp.seek(0, 2)
+            file_size = fp.tell()
+            fp.seek(0, 0)
+        if chunk_size is None:
+            chunk_size = file_size
+        first_chunk = fp.read(chunk_size)
+        if file_size <= chunk_size:
+            digest = hashlib.md5(first_chunk).digest()
+            hash_type = "md5"
+        else:
             fp.seek(-chunk_size, 2)
-            # read last chunk
-            data = fp.read(chunk_size)
-            chunks.append(data)
-    if len(chunks) == 1:
-        digest = hashlib.md5(chunks[0]).digest()
-        hash_type = "md5"
-    else:
-        digests = b"".join(hashlib.sha1(chunk).digest() for chunk in chunks)
-        digest = hashlib.sha1(digests).digest()
-        hash_type = "sha1-fl"  # sha1 first last chunk
+            last_chunk = fp.read(chunk_size)
+            digest = hashlib.sha1(
+                hashlib.sha1(first_chunk).digest() + hashlib.sha1(last_chunk).digest()
+            ).digest()
+            hash_type = "sha1-fl"
     return to_b64_str(digest)[:22], hash_type
```

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/types.py` & `lamindb_setup-0.71.4/lamindb_setup/core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/lamindb_setup/core/upath.py` & `lamindb_setup-0.71.4/lamindb_setup/core/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/noxfile.py` & `lamindb_setup-0.71.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/pyproject.toml` & `lamindb_setup-0.71.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.71.4/tests/hub-cloud/test_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.71.4/tests/hub-cloud/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/hub-cloud/test_login.py` & `lamindb_setup-0.71.4/tests/hub-cloud/test_login.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/hub-local/conftest.py` & `lamindb_setup-0.71.4/tests/hub-local/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/hub-local/test_all.py` & `lamindb_setup-0.71.4/tests/hub-local/test_all.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/hub-prod/conftest.py` & `lamindb_setup-0.71.4/tests/hub-prod/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
-from typing import TYPE_CHECKING
 from uuid import UUID
 
 import lamindb_setup
 import pytest
 from lamin_utils import logger
 
 
 def pytest_sessionstart(session: pytest.Session):
     lamindb_instance_id = UUID("e1a2d3ab762e4592af5a1e53f288284e")
     os.environ["LAMINDB_INSTANCE_ID_INIT"] = lamindb_instance_id.hex
+    assert lamindb_setup.settings.user.handle == "testuser2"
     lamindb_setup.init(
         storage="./default_storage",
         schema="bionty",
         name="lamindb-setup-unit-tests",
     )
     assert lamindb_setup.settings.instance._id == lamindb_instance_id
     assert lamindb_setup.settings.instance.uid == "7cIQBFhUg8ok"
 
 
 def pytest_sessionfinish(session: pytest.Session):
     logger.set_verbosity(1)
-    lamindb_setup.delete("lamindb-setup-unit-tests", force=True)
+    lamindb_setup.delete("testuser2/lamindb-setup-unit-tests", force=True)
```

### Comparing `lamindb_setup-0.71.3/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.71.4/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/hub-prod/test_upath.py` & `lamindb_setup-0.71.4/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/storage/test_hashing.py` & `lamindb_setup-0.71.4/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/storage/test_storage_access.py` & `lamindb_setup-0.71.4/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/storage/test_storage_basis.py` & `lamindb_setup-0.71.4/tests/storage/test_storage_basis.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/storage/test_storage_stats.py` & `lamindb_setup-0.71.4/tests/storage/test_storage_stats.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/tests/storage/test_to_url.py` & `lamindb_setup-0.71.4/tests/storage/test_to_url.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.3/PKG-INFO` & `lamindb_setup-0.71.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.71.3
+Version: 0.71.4
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```

