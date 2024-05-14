# Comparing `tmp/trainml-0.5.8.tar.gz` & `tmp/trainml-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainml-0.5.8.tar", last modified: Mon May  6 15:16:27 2024, max compression
+gzip compressed data, was "trainml-0.5.9.tar", last modified: Tue May 14 00:36:13 2024, max compression
```

## Comparing `trainml-0.5.8.tar` & `trainml-0.5.9.tar`

### file list

```diff
@@ -1,126 +1,148 @@
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.248930 trainml-0.5.8/
--rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.5.8/LICENSE
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-05-06 15:16:27.248795 trainml-0.5.8/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.5.8/README.md
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.225520 trainml-0.5.8/examples/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.5.8/examples/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2023-01-10 21:56:22.000000 trainml-0.5.8/examples/create_dataset_and_training_job.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2023-01-10 21:56:46.000000 trainml-0.5.8/examples/local_storage.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2023-01-22 22:47:55.000000 trainml-0.5.8/examples/training_inference_pipeline.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1037 2024-04-25 14:45:27.000000 trainml-0.5.8/pyproject.toml
--rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-05-06 15:16:27.248976 trainml-0.5.8/setup.cfg
--rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.5.8/setup.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.223562 trainml-0.5.8/tests/
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.227768 trainml-0.5.8/tests/integration/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.5.8/tests/integration/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.228102 trainml-0.5.8/tests/integration/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-19 19:22:07.000000 trainml-0.5.8/tests/integration/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2023-06-19 19:31:30.000000 trainml-0.5.8/tests/integration/cloudbender/test_providers_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.5.8/tests/integration/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-03-14 16:09:32.000000 trainml-0.5.8/tests/integration/test_checkpoints_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-03-19 18:31:45.000000 trainml-0.5.8/tests/integration/test_datasets_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2023-03-20 21:29:08.000000 trainml-0.5.8/tests/integration/test_environments_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2023-03-20 21:29:14.000000 trainml-0.5.8/tests/integration/test_gpu_types_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    25117 2024-04-17 17:22:21.000000 trainml-0.5.8/tests/integration/test_jobs_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-03-14 16:09:23.000000 trainml-0.5.8/tests/integration/test_models_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-02-29 23:09:06.000000 trainml-0.5.8/tests/integration/test_projects_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-02 13:07:27.000000 trainml-0.5.8/tests/integration/test_volumes_integration.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.231650 trainml-0.5.8/tests/unit/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.5.8/tests/unit/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.233985 trainml-0.5.8/tests/unit/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.5.8/tests/unit/cli/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.235355 trainml-0.5.8/tests/unit/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-21 01:22:34.000000 trainml-0.5.8/tests/unit/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2023-06-22 02:19:34.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2023-06-23 19:47:44.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_device_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2023-06-21 02:49:51.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_node_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      781 2023-06-21 01:49:51.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_provider_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2023-06-21 02:10:35.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_region_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-04-26 20:42:13.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_service_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.5.8/tests/unit/cli/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      702 2023-06-22 01:39:48.000000 trainml-0.5.8/tests/unit/cli/test_cli_checkpoint_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      653 2023-06-22 01:40:30.000000 trainml-0.5.8/tests/unit/cli/test_cli_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      683 2023-06-21 00:35:39.000000 trainml-0.5.8/tests/unit/cli/test_cli_environment_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      650 2023-06-21 00:36:29.000000 trainml-0.5.8/tests/unit/cli/test_cli_gpu_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      611 2023-06-22 01:49:26.000000 trainml-0.5.8/tests/unit/cli/test_cli_job_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      629 2023-06-22 01:42:02.000000 trainml-0.5.8/tests/unit/cli/test_cli_model_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-04-09 16:44:25.000000 trainml-0.5.8/tests/unit/cli/test_cli_project_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-03-12 15:29:44.000000 trainml-0.5.8/tests/unit/cli/test_cli_volume_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.237360 trainml-0.5.8/tests/unit/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-16 16:46:40.000000 trainml-0.5.8/tests/unit/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5783 2024-04-26 20:39:34.000000 trainml-0.5.8/tests/unit/cloudbender/test_data_connectors_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2023-06-23 16:49:35.000000 trainml-0.5.8/tests/unit/cloudbender/test_datastores_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2023-06-23 16:50:27.000000 trainml-0.5.8/tests/unit/cloudbender/test_device_configs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2023-06-23 19:46:10.000000 trainml-0.5.8/tests/unit/cloudbender/test_devices_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2023-06-23 16:51:45.000000 trainml-0.5.8/tests/unit/cloudbender/test_nodes_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2023-06-23 16:52:25.000000 trainml-0.5.8/tests/unit/cloudbender/test_providers_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2023-06-23 16:53:15.000000 trainml-0.5.8/tests/unit/cloudbender/test_regions_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5220 2024-04-26 20:39:32.000000 trainml-0.5.8/tests/unit/cloudbender/test_services_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    31129 2024-04-09 16:44:31.000000 trainml-0.5.8/tests/unit/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      858 2023-07-27 15:10:38.000000 trainml-0.5.8/tests/unit/test_auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2023-03-31 21:38:18.000000 trainml-0.5.8/tests/unit/test_checkpoints_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2023-01-10 22:45:55.000000 trainml-0.5.8/tests/unit/test_connections_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2023-03-31 21:39:46.000000 trainml-0.5.8/tests/unit/test_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2023-06-04 18:32:37.000000 trainml-0.5.8/tests/unit/test_environments_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.5.8/tests/unit/test_exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2023-06-21 20:53:31.000000 trainml-0.5.8/tests/unit/test_gpu_types_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2023-06-04 18:29:09.000000 trainml-0.5.8/tests/unit/test_jobs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2023-03-31 21:39:17.000000 trainml-0.5.8/tests/unit/test_models_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10743 2024-04-18 15:31:37.000000 trainml-0.5.8/tests/unit/test_projects_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.5.8/tests/unit/test_trainml.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-03-12 17:51:37.000000 trainml-0.5.8/tests/unit/test_volumes_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.240842 trainml-0.5.8/trainml/
--rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-05-06 15:15:01.000000 trainml-0.5.8/trainml/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.5.8/trainml/__main__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2023-09-08 15:42:01.000000 trainml-0.5.8/trainml/auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8667 2024-05-05 19:36:12.000000 trainml-0.5.8/trainml/checkpoints.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.243653 trainml-0.5.8/trainml/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-02-29 19:03:52.000000 trainml-0.5.8/trainml/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2023-06-19 19:34:08.000000 trainml-0.5.8/trainml/cli/checkpoint.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.245534 trainml-0.5.8/trainml/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)      592 2024-04-18 15:45:19.000000 trainml-0.5.8/trainml/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3606 2024-04-18 15:45:08.000000 trainml-0.5.8/trainml/cli/cloudbender/data_connector.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2023-06-22 02:11:56.000000 trainml-0.5.8/trainml/cli/cloudbender/datastore.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2023-06-25 18:44:34.000000 trainml-0.5.8/trainml/cli/cloudbender/device.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2023-06-22 02:09:01.000000 trainml-0.5.8/trainml/cli/cloudbender/node.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2023-06-22 02:09:04.000000 trainml-0.5.8/trainml/cli/cloudbender/provider.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2023-06-22 02:09:07.000000 trainml-0.5.8/trainml/cli/cloudbender/region.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3147 2024-04-26 20:42:25.000000 trainml-0.5.8/trainml/cli/cloudbender/service.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2023-06-19 19:34:11.000000 trainml-0.5.8/trainml/cli/connection.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-02-08 17:04:38.000000 trainml-0.5.8/trainml/cli/dataset.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2023-06-19 19:34:12.000000 trainml-0.5.8/trainml/cli/environment.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      883 2023-06-19 19:40:03.000000 trainml-0.5.8/trainml/cli/gpu.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.246001 trainml-0.5.8/trainml/cli/job/
--rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2023-06-19 19:34:17.000000 trainml-0.5.8/trainml/cli/job/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-02-14 15:58:34.000000 trainml-0.5.8/trainml/cli/job/create.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2023-09-08 19:00:58.000000 trainml-0.5.8/trainml/cli/model.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3314 2024-04-09 16:42:40.000000 trainml-0.5.8/trainml/cli/project.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-03-12 17:50:39.000000 trainml-0.5.8/trainml/cli/volume.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.248475 trainml-0.5.8/trainml/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)       64 2023-06-16 13:41:42.000000 trainml-0.5.8/trainml/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      717 2024-04-18 15:13:53.000000 trainml-0.5.8/trainml/cloudbender/cloudbender.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3297 2024-04-18 15:41:18.000000 trainml-0.5.8/trainml/cloudbender/data_connectors.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2023-06-23 16:22:15.000000 trainml-0.5.8/trainml/cloudbender/datastores.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2023-06-23 16:22:25.000000 trainml-0.5.8/trainml/cloudbender/device_configs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2023-06-23 16:28:32.000000 trainml-0.5.8/trainml/cloudbender/devices.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2023-06-23 16:25:10.000000 trainml-0.5.8/trainml/cloudbender/nodes.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2023-06-23 16:22:51.000000 trainml-0.5.8/trainml/cloudbender/providers.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2023-06-23 16:23:07.000000 trainml-0.5.8/trainml/cloudbender/regions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5126 2024-04-26 20:45:18.000000 trainml-0.5.8/trainml/cloudbender/services.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20029 2023-09-08 19:03:44.000000 trainml-0.5.8/trainml/connections.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8477 2024-05-05 19:36:10.000000 trainml-0.5.8/trainml/datasets.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2023-06-21 20:39:07.000000 trainml-0.5.8/trainml/environments.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-02-29 19:05:24.000000 trainml-0.5.8/trainml/exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2023-06-23 15:24:57.000000 trainml-0.5.8/trainml/gpu_types.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    18056 2024-04-17 17:23:52.000000 trainml-0.5.8/trainml/jobs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8161 2024-05-05 19:36:16.000000 trainml-0.5.8/trainml/models.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6585 2024-04-19 18:45:25.000000 trainml-0.5.8/trainml/projects.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-02-29 19:06:10.000000 trainml-0.5.8/trainml/trainml.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8312 2024-04-17 13:07:00.000000 trainml-0.5.8/trainml/volumes.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.241720 trainml-0.5.8/trainml.egg-info/
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     3619 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/SOURCES.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/dependency_links.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/entry_points.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/requires.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/top_level.txt
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.634658 trainml-0.5.9/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.5.9/LICENSE
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-05-14 00:36:13.634525 trainml-0.5.9/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.5.9/README.md
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.610853 trainml-0.5.9/examples/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.5.9/examples/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2023-01-10 21:56:22.000000 trainml-0.5.9/examples/create_dataset_and_training_job.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2023-01-10 21:56:46.000000 trainml-0.5.9/examples/local_storage.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2023-01-22 22:47:55.000000 trainml-0.5.9/examples/training_inference_pipeline.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1037 2024-04-25 14:45:27.000000 trainml-0.5.9/pyproject.toml
+-rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-05-14 00:36:13.634701 trainml-0.5.9/setup.cfg
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.5.9/setup.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.608664 trainml-0.5.9/tests/
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.612980 trainml-0.5.9/tests/integration/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.5.9/tests/integration/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.613321 trainml-0.5.9/tests/integration/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-19 19:22:07.000000 trainml-0.5.9/tests/integration/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2023-06-19 19:31:30.000000 trainml-0.5.9/tests/integration/cloudbender/test_providers_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.5.9/tests/integration/conftest.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.614246 trainml-0.5.9/tests/integration/projects/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-08 20:18:10.000000 trainml-0.5.9/tests/integration/projects/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      208 2024-05-08 20:44:17.000000 trainml-0.5.9/tests/integration/projects/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1241 2024-05-08 20:36:10.000000 trainml-0.5.9/tests/integration/projects/test_projects_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1423 2024-05-09 14:00:38.000000 trainml-0.5.9/tests/integration/projects/test_projects_keys_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1478 2024-05-09 15:12:32.000000 trainml-0.5.9/tests/integration/projects/test_projects_secrets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-03-14 16:09:32.000000 trainml-0.5.9/tests/integration/test_checkpoints_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-03-19 18:31:45.000000 trainml-0.5.9/tests/integration/test_datasets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2023-03-20 21:29:08.000000 trainml-0.5.9/tests/integration/test_environments_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2023-03-20 21:29:14.000000 trainml-0.5.9/tests/integration/test_gpu_types_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    25117 2024-04-17 17:22:21.000000 trainml-0.5.9/tests/integration/test_jobs_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-03-14 16:09:23.000000 trainml-0.5.9/tests/integration/test_models_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-02 13:07:27.000000 trainml-0.5.9/tests/integration/test_volumes_integration.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.617681 trainml-0.5.9/tests/unit/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.5.9/tests/unit/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.619748 trainml-0.5.9/tests/unit/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.5.9/tests/unit/cli/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.621104 trainml-0.5.9/tests/unit/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-21 01:22:34.000000 trainml-0.5.9/tests/unit/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2023-06-22 02:19:34.000000 trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2023-06-23 19:47:44.000000 trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_device_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2023-06-21 02:49:51.000000 trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_node_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      781 2023-06-21 01:49:51.000000 trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_provider_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2023-06-21 02:10:35.000000 trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_region_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-04-26 20:42:13.000000 trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_service_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.5.9/tests/unit/cli/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      702 2023-06-22 01:39:48.000000 trainml-0.5.9/tests/unit/cli/test_cli_checkpoint_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      653 2023-06-22 01:40:30.000000 trainml-0.5.9/tests/unit/cli/test_cli_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      683 2023-06-21 00:35:39.000000 trainml-0.5.9/tests/unit/cli/test_cli_environment_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      650 2023-06-21 00:36:29.000000 trainml-0.5.9/tests/unit/cli/test_cli_gpu_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      611 2023-06-22 01:49:26.000000 trainml-0.5.9/tests/unit/cli/test_cli_job_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      629 2023-06-22 01:42:02.000000 trainml-0.5.9/tests/unit/cli/test_cli_model_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-04-09 16:44:25.000000 trainml-0.5.9/tests/unit/cli/test_cli_project_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-03-12 15:29:44.000000 trainml-0.5.9/tests/unit/cli/test_cli_volume_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.623105 trainml-0.5.9/tests/unit/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-16 16:46:40.000000 trainml-0.5.9/tests/unit/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5783 2024-04-26 20:39:34.000000 trainml-0.5.9/tests/unit/cloudbender/test_data_connectors_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2023-06-23 16:49:35.000000 trainml-0.5.9/tests/unit/cloudbender/test_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2023-06-23 16:50:27.000000 trainml-0.5.9/tests/unit/cloudbender/test_device_configs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2023-06-23 19:46:10.000000 trainml-0.5.9/tests/unit/cloudbender/test_devices_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2023-06-23 16:51:45.000000 trainml-0.5.9/tests/unit/cloudbender/test_nodes_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2023-06-23 16:52:25.000000 trainml-0.5.9/tests/unit/cloudbender/test_providers_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2023-06-23 16:53:15.000000 trainml-0.5.9/tests/unit/cloudbender/test_regions_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5220 2024-04-26 20:39:32.000000 trainml-0.5.9/tests/unit/cloudbender/test_services_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    33174 2024-05-08 20:33:31.000000 trainml-0.5.9/tests/unit/conftest.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.624471 trainml-0.5.9/tests/unit/projects/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-08 19:50:46.000000 trainml-0.5.9/tests/unit/projects/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3385 2024-05-08 20:05:29.000000 trainml-0.5.9/tests/unit/projects/test_project_data_connectors_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3129 2024-05-08 20:05:23.000000 trainml-0.5.9/tests/unit/projects/test_project_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3161 2024-05-09 14:00:26.000000 trainml-0.5.9/tests/unit/projects/test_project_keys_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3276 2024-05-09 14:00:13.000000 trainml-0.5.9/tests/unit/projects/test_project_secrets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3331 2024-05-08 20:05:36.000000 trainml-0.5.9/tests/unit/projects/test_project_services_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3823 2024-05-08 20:02:49.000000 trainml-0.5.9/tests/unit/projects/test_projects_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      858 2023-07-27 15:10:38.000000 trainml-0.5.9/tests/unit/test_auth_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2023-03-31 21:38:18.000000 trainml-0.5.9/tests/unit/test_checkpoints_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2023-01-10 22:45:55.000000 trainml-0.5.9/tests/unit/test_connections_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2023-03-31 21:39:46.000000 trainml-0.5.9/tests/unit/test_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2023-06-04 18:32:37.000000 trainml-0.5.9/tests/unit/test_environments_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.5.9/tests/unit/test_exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2023-06-21 20:53:31.000000 trainml-0.5.9/tests/unit/test_gpu_types_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2023-06-04 18:29:09.000000 trainml-0.5.9/tests/unit/test_jobs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2023-03-31 21:39:17.000000 trainml-0.5.9/tests/unit/test_models_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.5.9/tests/unit/test_trainml_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-03-12 17:51:37.000000 trainml-0.5.9/tests/unit/test_volumes_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.626695 trainml-0.5.9/trainml/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-05-14 00:34:08.000000 trainml-0.5.9/trainml/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.5.9/trainml/__main__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2023-09-08 15:42:01.000000 trainml-0.5.9/trainml/auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8667 2024-05-05 19:36:12.000000 trainml-0.5.9/trainml/checkpoints.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.628448 trainml-0.5.9/trainml/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-05-09 12:53:06.000000 trainml-0.5.9/trainml/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2023-06-19 19:34:08.000000 trainml-0.5.9/trainml/cli/checkpoint.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.629463 trainml-0.5.9/trainml/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      592 2024-04-18 15:45:19.000000 trainml-0.5.9/trainml/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3606 2024-04-18 15:45:08.000000 trainml-0.5.9/trainml/cli/cloudbender/data_connector.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2023-06-22 02:11:56.000000 trainml-0.5.9/trainml/cli/cloudbender/datastore.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2023-06-25 18:44:34.000000 trainml-0.5.9/trainml/cli/cloudbender/device.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2023-06-22 02:09:01.000000 trainml-0.5.9/trainml/cli/cloudbender/node.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2023-06-22 02:09:04.000000 trainml-0.5.9/trainml/cli/cloudbender/provider.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2023-06-22 02:09:07.000000 trainml-0.5.9/trainml/cli/cloudbender/region.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3147 2024-04-26 20:42:25.000000 trainml-0.5.9/trainml/cli/cloudbender/service.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2023-06-19 19:34:11.000000 trainml-0.5.9/trainml/cli/connection.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-02-08 17:04:38.000000 trainml-0.5.9/trainml/cli/dataset.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2023-06-19 19:34:12.000000 trainml-0.5.9/trainml/cli/environment.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      883 2023-06-19 19:40:03.000000 trainml-0.5.9/trainml/cli/gpu.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.629730 trainml-0.5.9/trainml/cli/job/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2023-06-19 19:34:17.000000 trainml-0.5.9/trainml/cli/job/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-02-14 15:58:34.000000 trainml-0.5.9/trainml/cli/job/create.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2023-09-08 19:00:58.000000 trainml-0.5.9/trainml/cli/model.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.630492 trainml-0.5.9/trainml/cli/project/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3402 2024-05-09 14:01:25.000000 trainml-0.5.9/trainml/cli/project/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3203 2024-05-10 16:29:05.000000 trainml-0.5.9/trainml/cli/project/key.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1621 2024-05-13 13:07:52.000000 trainml-0.5.9/trainml/cli/project/secret.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-03-12 17:50:39.000000 trainml-0.5.9/trainml/cli/volume.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.633213 trainml-0.5.9/trainml/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       64 2023-06-16 13:41:42.000000 trainml-0.5.9/trainml/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      717 2024-04-18 15:13:53.000000 trainml-0.5.9/trainml/cloudbender/cloudbender.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3297 2024-04-18 15:41:18.000000 trainml-0.5.9/trainml/cloudbender/data_connectors.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2023-06-23 16:22:15.000000 trainml-0.5.9/trainml/cloudbender/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2023-06-23 16:22:25.000000 trainml-0.5.9/trainml/cloudbender/device_configs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2023-06-23 16:28:32.000000 trainml-0.5.9/trainml/cloudbender/devices.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2023-06-23 16:25:10.000000 trainml-0.5.9/trainml/cloudbender/nodes.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2023-06-23 16:22:51.000000 trainml-0.5.9/trainml/cloudbender/providers.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2023-06-23 16:23:07.000000 trainml-0.5.9/trainml/cloudbender/regions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5126 2024-04-26 20:45:18.000000 trainml-0.5.9/trainml/cloudbender/services.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20029 2023-09-08 19:03:44.000000 trainml-0.5.9/trainml/connections.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8477 2024-05-05 19:36:10.000000 trainml-0.5.9/trainml/datasets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2023-06-21 20:39:07.000000 trainml-0.5.9/trainml/environments.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-02-29 19:05:24.000000 trainml-0.5.9/trainml/exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2023-06-23 15:24:57.000000 trainml-0.5.9/trainml/gpu_types.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    18056 2024-04-17 17:23:52.000000 trainml-0.5.9/trainml/jobs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8161 2024-05-05 19:36:16.000000 trainml-0.5.9/trainml/models.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.634334 trainml-0.5.9/trainml/projects/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       75 2024-05-08 19:06:10.000000 trainml-0.5.9/trainml/projects/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1662 2024-05-08 20:10:53.000000 trainml-0.5.9/trainml/projects/data_connectors.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1560 2024-05-08 20:11:05.000000 trainml-0.5.9/trainml/projects/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2157 2024-05-12 15:42:35.000000 trainml-0.5.9/trainml/projects/keys.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2755 2024-05-08 20:44:41.000000 trainml-0.5.9/trainml/projects/projects.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2157 2024-05-09 13:59:28.000000 trainml-0.5.9/trainml/projects/secrets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1679 2024-05-08 20:51:01.000000 trainml-0.5.9/trainml/projects/services.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-05-13 13:25:44.000000 trainml-0.5.9/trainml/trainml.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8312 2024-04-17 13:07:00.000000 trainml-0.5.9/trainml/volumes.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:36:13.627449 trainml-0.5.9/trainml.egg-info/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-05-14 00:36:13.000000 trainml-0.5.9/trainml.egg-info/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4389 2024-05-14 00:36:13.000000 trainml-0.5.9/trainml.egg-info/SOURCES.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-05-14 00:36:13.000000 trainml-0.5.9/trainml.egg-info/dependency_links.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-05-14 00:36:13.000000 trainml-0.5.9/trainml.egg-info/entry_points.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-05-14 00:36:13.000000 trainml-0.5.9/trainml.egg-info/requires.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-05-14 00:36:13.000000 trainml-0.5.9/trainml.egg-info/top_level.txt
```

### Comparing `trainml-0.5.8/LICENSE` & `trainml-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/PKG-INFO` & `trainml-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.5.8
+Version: 0.5.9
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.5.8 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.5.9 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._t_r_a_i_n_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_t_r_a_i_n_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.5.8/README.md` & `trainml-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/examples/create_dataset_and_training_job.py` & `trainml-0.5.9/examples/create_dataset_and_training_job.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/examples/local_storage.py` & `trainml-0.5.9/examples/local_storage.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/examples/training_inference_pipeline.py` & `trainml-0.5.9/examples/training_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/pyproject.toml` & `trainml-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/setup.py` & `trainml-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/integration/cloudbender/test_providers_integration.py` & `trainml-0.5.9/tests/integration/cloudbender/test_providers_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/integration/conftest.py` & `trainml-0.5.9/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/integration/test_checkpoints_integration.py` & `trainml-0.5.9/tests/integration/test_checkpoints_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/integration/test_datasets_integration.py` & `trainml-0.5.9/tests/integration/test_datasets_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/integration/test_environments_integration.py` & `trainml-0.5.9/tests/integration/test_environments_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/integration/test_gpu_types_integration.py` & `trainml-0.5.9/tests/integration/test_gpu_types_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/integration/test_jobs_integration.py` & `trainml-0.5.9/tests/integration/test_jobs_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/integration/test_models_integration.py` & `trainml-0.5.9/tests/integration/test_models_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/integration/test_projects_integration.py` & `trainml-0.5.9/tests/integration/projects/test_projects_integration.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 
 pytestmark = [mark.sdk, mark.integration, mark.projects]
 
 
 @mark.create
 @mark.asyncio
 class GetProjectsTests:
-    @fixture(scope="class")
-    async def project(self, trainml):
-        project = await trainml.projects.create(name="New Project", copy_keys=False)
-        yield project
-        await project.remove()
-
     async def test_get_projects(self, trainml):
         projects = await trainml.projects.list()
         assert len(projects) > 0
 
     async def test_get_project(self, trainml, project):
         response = await trainml.projects.get(project.id)
         assert response.id == project.id
```

### Comparing `trainml-0.5.8/tests/integration/test_volumes_integration.py` & `trainml-0.5.9/tests/integration/test_volumes_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_datastore_unit.py` & `trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_datastore_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_device_unit.py` & `trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_device_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_node_unit.py` & `trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_node_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_provider_unit.py` & `trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_provider_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_region_unit.py` & `trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_region_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_service_unit.py` & `trainml-0.5.9/tests/unit/cli/cloudbender/test_cli_service_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/test_cli_checkpoint_unit.py` & `trainml-0.5.9/tests/unit/cli/test_cli_checkpoint_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/test_cli_datasets_unit.py` & `trainml-0.5.9/tests/unit/cli/test_cli_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/test_cli_environment_unit.py` & `trainml-0.5.9/tests/unit/cli/test_cli_environment_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/test_cli_gpu_unit.py` & `trainml-0.5.9/tests/unit/cli/test_cli_gpu_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/test_cli_job_unit.py` & `trainml-0.5.9/tests/unit/cli/test_cli_job_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/test_cli_model_unit.py` & `trainml-0.5.9/tests/unit/cli/test_cli_model_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/test_cli_project_unit.py` & `trainml-0.5.9/tests/unit/cli/test_cli_project_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cli/test_cli_volume_unit.py` & `trainml-0.5.9/tests/unit/cli/test_cli_volume_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cloudbender/test_data_connectors_unit.py` & `trainml-0.5.9/tests/unit/cloudbender/test_data_connectors_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cloudbender/test_datastores_unit.py` & `trainml-0.5.9/tests/unit/cloudbender/test_datastores_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cloudbender/test_device_configs_unit.py` & `trainml-0.5.9/tests/unit/cloudbender/test_device_configs_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cloudbender/test_devices_unit.py` & `trainml-0.5.9/tests/unit/cloudbender/test_devices_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cloudbender/test_nodes_unit.py` & `trainml-0.5.9/tests/unit/cloudbender/test_nodes_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cloudbender/test_providers_unit.py` & `trainml-0.5.9/tests/unit/cloudbender/test_providers_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cloudbender/test_regions_unit.py` & `trainml-0.5.9/tests/unit/cloudbender/test_regions_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/cloudbender/test_services_unit.py` & `trainml-0.5.9/tests/unit/cloudbender/test_services_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/conftest.py` & `trainml-0.5.9/tests/unit/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,27 @@
 from trainml.gpu_types import GpuType, GpuTypes
 from trainml.environments import Environment, Environments
 from trainml.jobs import Job, Jobs
 from trainml.connections import Connections
 from trainml.projects import (
     Projects,
     Project,
-    ProjectDatastore,
-    ProjectService,
 )
+from trainml.projects.datastores import ProjectDatastore
+from trainml.projects.services import ProjectService
+from trainml.projects.data_connectors import ProjectDataConnector
+
 from trainml.cloudbender import Cloudbender
 from trainml.cloudbender.providers import Provider, Providers
 from trainml.cloudbender.regions import Region, Regions
 from trainml.cloudbender.nodes import Node, Nodes
 from trainml.cloudbender.devices import Device, Devices
 from trainml.cloudbender.datastores import Datastore, Datastores
 from trainml.cloudbender.services import Service, Services
+from trainml.cloudbender.data_connectors import DataConnector, DataConnectors
 from trainml.cloudbender.device_configs import DeviceConfig, DeviceConfigs
 
 
 pytestmark = mark.unit
 
 
 @fixture(scope="session")
@@ -945,14 +948,76 @@
                 "hostname": "service-b.local",
             },
         ),
     ]
 
 
 @fixture(scope="session")
+def mock_data_connectors():
+    trainml = Mock()
+    yield [
+        DataConnector(
+            trainml,
+            **{
+                "provider_uuid": "prov-id-1",
+                "region_uuid": "reg-id-1",
+                "connector_id": "con-id-1",
+                "type": "custom",
+                "name": "On-Prem Connection A",
+                "protocol": "TCP",
+                "port_range": "8000-8099",
+                "cidr": "10.0.3.0/24",
+            },
+        ),
+        DataConnector(
+            trainml,
+            **{
+                "provider_uuid": "prov-id-2",
+                "region_uuid": "reg-id-2",
+                "connector_id": "con-id-2",
+                "type": "custom",
+                "name": "Cloud Connection B",
+                "protocol": "UDP",
+                "port_range": "5000",
+                "cidr": "10.0.2.0/24",
+            },
+        ),
+    ]
+
+
+@fixture(
+    scope="session",
+)
+def mock_project_data_connectors():
+    trainml = Mock()
+    yield [
+        ProjectDataConnector(
+            trainml,
+            **{
+                "project_uuid": "proj-id-1",
+                "region_uuid": "reg-id-1",
+                "id": "con-id-1",
+                "type": "custom",
+                "name": "On-Prem Connection A",
+            },
+        ),
+        ProjectDataConnector(
+            trainml,
+            **{
+                "project_uuid": "proj-id-1",
+                "region_uuid": "reg-id-2",
+                "id": "con-id-2",
+                "type": "custom",
+                "name": "Cloud Connection B",
+            },
+        ),
+    ]
+
+
+@fixture(scope="session")
 def mock_device_configs():
     trainml = Mock()
     yield [
         DeviceConfig(
             trainml,
             **{
                 "provider_uuid": "prov-id-1",
@@ -987,14 +1052,15 @@
     mock_projects,
     mock_providers,
     mock_regions,
     mock_nodes,
     mock_devices,
     mock_datastores,
     mock_services,
+    mock_data_connectors,
     mock_device_configs,
 ):
     trainml = create_autospec(TrainML)
     trainml.active_project = "proj-id-1"
     trainml.project = "proj-id-1"
     trainml.datasets = create_autospec(Datasets)
     trainml.checkpoints = create_autospec(Checkpoints)
@@ -1026,12 +1092,16 @@
     trainml.cloudbender.nodes.list = AsyncMock(return_value=mock_nodes)
     trainml.cloudbender.devices = create_autospec(Nodes)
     trainml.cloudbender.devices.list = AsyncMock(return_value=mock_devices)
     trainml.cloudbender.datastores = create_autospec(Datastores)
     trainml.cloudbender.datastores.list = AsyncMock(return_value=mock_datastores)
     trainml.cloudbender.services = create_autospec(Services)
     trainml.cloudbender.services.list = AsyncMock(return_value=mock_services)
+    trainml.cloudbender.data_connectors = create_autospec(DataConnectors)
+    trainml.cloudbender.data_connectors.list = AsyncMock(
+        return_value=mock_data_connectors
+    )
     trainml.cloudbender.device_configs = create_autospec(DeviceConfigs)
     trainml.cloudbender.device_configs.list = AsyncMock(
         return_value=mock_device_configs
     )
     yield trainml
```

### Comparing `trainml-0.5.8/tests/unit/test_auth.py` & `trainml-0.5.9/tests/unit/test_auth_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/test_checkpoints_unit.py` & `trainml-0.5.9/tests/unit/test_checkpoints_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/test_connections_unit.py` & `trainml-0.5.9/tests/unit/test_connections_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/test_datasets_unit.py` & `trainml-0.5.9/tests/unit/test_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/test_environments_unit.py` & `trainml-0.5.9/tests/unit/test_environments_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/test_exceptions.py` & `trainml-0.5.9/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/test_gpu_types_unit.py` & `trainml-0.5.9/tests/unit/test_gpu_types_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/test_jobs_unit.py` & `trainml-0.5.9/tests/unit/test_jobs_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/test_models_unit.py` & `trainml-0.5.9/tests/unit/test_models_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/test_trainml.py` & `trainml-0.5.9/tests/unit/test_trainml_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/tests/unit/test_volumes_unit.py` & `trainml-0.5.9/tests/unit/test_volumes_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/auth.py` & `trainml-0.5.9/trainml/auth.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/checkpoints.py` & `trainml-0.5.9/trainml/checkpoints.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/__init__.py` & `trainml-0.5.9/trainml/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/checkpoint.py` & `trainml-0.5.9/trainml/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/cloudbender/__init__.py` & `trainml-0.5.9/trainml/cli/cloudbender/__init__.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/cloudbender/data_connector.py` & `trainml-0.5.9/trainml/cli/cloudbender/data_connector.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/cloudbender/datastore.py` & `trainml-0.5.9/trainml/cli/cloudbender/datastore.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/cloudbender/device.py` & `trainml-0.5.9/trainml/cli/cloudbender/device.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/cloudbender/node.py` & `trainml-0.5.9/trainml/cli/cloudbender/node.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/cloudbender/provider.py` & `trainml-0.5.9/trainml/cli/cloudbender/provider.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/cloudbender/region.py` & `trainml-0.5.9/trainml/cli/cloudbender/region.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/cloudbender/service.py` & `trainml-0.5.9/trainml/cli/cloudbender/service.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/connection.py` & `trainml-0.5.9/trainml/cli/connection.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/dataset.py` & `trainml-0.5.9/trainml/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/environment.py` & `trainml-0.5.9/trainml/cli/environment.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/gpu.py` & `trainml-0.5.9/trainml/cli/gpu.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/job/__init__.py` & `trainml-0.5.9/trainml/cli/job/__init__.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/job/create.py` & `trainml-0.5.9/trainml/cli/job/create.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/model.py` & `trainml-0.5.9/trainml/cli/model.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cli/project.py` & `trainml-0.5.9/trainml/cli/project/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,7 +143,11 @@
         )
 
     for row in data:
         click.echo(
             "{: >38.36} {: >30.28} {: >30.28} {: >38.36}" "".format(*row),
             file=config.stdout,
         )
+
+
+from trainml.cli.project.secret import secret
+from trainml.cli.project.key import key
```

### Comparing `trainml-0.5.8/trainml/cli/volume.py` & `trainml-0.5.9/trainml/cli/volume.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cloudbender/cloudbender.py` & `trainml-0.5.9/trainml/cloudbender/cloudbender.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cloudbender/data_connectors.py` & `trainml-0.5.9/trainml/cloudbender/data_connectors.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cloudbender/datastores.py` & `trainml-0.5.9/trainml/cloudbender/datastores.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cloudbender/device_configs.py` & `trainml-0.5.9/trainml/cloudbender/device_configs.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cloudbender/devices.py` & `trainml-0.5.9/trainml/cloudbender/devices.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cloudbender/nodes.py` & `trainml-0.5.9/trainml/cloudbender/nodes.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cloudbender/providers.py` & `trainml-0.5.9/trainml/cloudbender/providers.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cloudbender/regions.py` & `trainml-0.5.9/trainml/cloudbender/regions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/cloudbender/services.py` & `trainml-0.5.9/trainml/cloudbender/services.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/connections.py` & `trainml-0.5.9/trainml/connections.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/datasets.py` & `trainml-0.5.9/trainml/datasets.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/environments.py` & `trainml-0.5.9/trainml/environments.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/exceptions.py` & `trainml-0.5.9/trainml/exceptions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/gpu_types.py` & `trainml-0.5.9/trainml/gpu_types.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/jobs.py` & `trainml-0.5.9/trainml/jobs.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/models.py` & `trainml-0.5.9/trainml/models.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/trainml.py` & `trainml-0.5.9/trainml/trainml.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml/volumes.py` & `trainml-0.5.9/trainml/volumes.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.8/trainml.egg-info/PKG-INFO` & `trainml-0.5.9/trainml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.5.8
+Version: 0.5.9
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.5.8 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.5.9 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._t_r_a_i_n_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_t_r_a_i_n_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.5.8/trainml.egg-info/SOURCES.txt` & `trainml-0.5.9/trainml.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,31 +10,34 @@
 tests/integration/conftest.py
 tests/integration/test_checkpoints_integration.py
 tests/integration/test_datasets_integration.py
 tests/integration/test_environments_integration.py
 tests/integration/test_gpu_types_integration.py
 tests/integration/test_jobs_integration.py
 tests/integration/test_models_integration.py
-tests/integration/test_projects_integration.py
 tests/integration/test_volumes_integration.py
 tests/integration/cloudbender/__init__.py
 tests/integration/cloudbender/test_providers_integration.py
+tests/integration/projects/__init__.py
+tests/integration/projects/conftest.py
+tests/integration/projects/test_projects_integration.py
+tests/integration/projects/test_projects_keys_integration.py
+tests/integration/projects/test_projects_secrets_integration.py
 tests/unit/__init__.py
 tests/unit/conftest.py
-tests/unit/test_auth.py
+tests/unit/test_auth_unit.py
 tests/unit/test_checkpoints_unit.py
 tests/unit/test_connections_unit.py
 tests/unit/test_datasets_unit.py
 tests/unit/test_environments_unit.py
 tests/unit/test_exceptions.py
 tests/unit/test_gpu_types_unit.py
 tests/unit/test_jobs_unit.py
 tests/unit/test_models_unit.py
-tests/unit/test_projects_unit.py
-tests/unit/test_trainml.py
+tests/unit/test_trainml_unit.py
 tests/unit/test_volumes_unit.py
 tests/unit/cli/__init__.py
 tests/unit/cli/conftest.py
 tests/unit/cli/test_cli_checkpoint_unit.py
 tests/unit/cli/test_cli_datasets_unit.py
 tests/unit/cli/test_cli_environment_unit.py
 tests/unit/cli/test_cli_gpu_unit.py
@@ -54,26 +57,32 @@
 tests/unit/cloudbender/test_datastores_unit.py
 tests/unit/cloudbender/test_device_configs_unit.py
 tests/unit/cloudbender/test_devices_unit.py
 tests/unit/cloudbender/test_nodes_unit.py
 tests/unit/cloudbender/test_providers_unit.py
 tests/unit/cloudbender/test_regions_unit.py
 tests/unit/cloudbender/test_services_unit.py
+tests/unit/projects/__init__.py
+tests/unit/projects/test_project_data_connectors_unit.py
+tests/unit/projects/test_project_datastores_unit.py
+tests/unit/projects/test_project_keys_unit.py
+tests/unit/projects/test_project_secrets_unit.py
+tests/unit/projects/test_project_services_unit.py
+tests/unit/projects/test_projects_unit.py
 trainml/__init__.py
 trainml/__main__.py
 trainml/auth.py
 trainml/checkpoints.py
 trainml/connections.py
 trainml/datasets.py
 trainml/environments.py
 trainml/exceptions.py
 trainml/gpu_types.py
 trainml/jobs.py
 trainml/models.py
-trainml/projects.py
 trainml/trainml.py
 trainml/volumes.py
 trainml.egg-info/PKG-INFO
 trainml.egg-info/SOURCES.txt
 trainml.egg-info/dependency_links.txt
 trainml.egg-info/entry_points.txt
 trainml.egg-info/requires.txt
@@ -81,29 +90,38 @@
 trainml/cli/__init__.py
 trainml/cli/checkpoint.py
 trainml/cli/connection.py
 trainml/cli/dataset.py
 trainml/cli/environment.py
 trainml/cli/gpu.py
 trainml/cli/model.py
-trainml/cli/project.py
 trainml/cli/volume.py
 trainml/cli/cloudbender/__init__.py
 trainml/cli/cloudbender/data_connector.py
 trainml/cli/cloudbender/datastore.py
 trainml/cli/cloudbender/device.py
 trainml/cli/cloudbender/node.py
 trainml/cli/cloudbender/provider.py
 trainml/cli/cloudbender/region.py
 trainml/cli/cloudbender/service.py
 trainml/cli/job/__init__.py
 trainml/cli/job/create.py
+trainml/cli/project/__init__.py
+trainml/cli/project/key.py
+trainml/cli/project/secret.py
 trainml/cloudbender/__init__.py
 trainml/cloudbender/cloudbender.py
 trainml/cloudbender/data_connectors.py
 trainml/cloudbender/datastores.py
 trainml/cloudbender/device_configs.py
 trainml/cloudbender/devices.py
 trainml/cloudbender/nodes.py
 trainml/cloudbender/providers.py
 trainml/cloudbender/regions.py
-trainml/cloudbender/services.py
+trainml/cloudbender/services.py
+trainml/projects/__init__.py
+trainml/projects/data_connectors.py
+trainml/projects/datastores.py
+trainml/projects/keys.py
+trainml/projects/projects.py
+trainml/projects/secrets.py
+trainml/projects/services.py
```

