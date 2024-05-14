# Comparing `tmp/psij-python-0.9.7.tar.gz` & `tmp/psij-python-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psij-python-0.9.7.tar", last modified: Wed May  1 04:39:00 2024, max compression
+gzip compressed data, was "psij-python-0.9.8.tar", last modified: Tue May 14 20:46:04 2024, max compression
```

## Comparing `psij-python-0.9.7.tar` & `psij-python-0.9.8.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.137713 psij-python-0.9.7/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1065 2024-05-01 04:36:19.000000 psij-python-0.9.7/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)       25 2024-05-01 04:36:19.000000 psij-python-0.9.7/MANIFEST.in
--rw-rw-r--   0 mike      (1000) mike      (1000)      414 2024-05-01 04:39:00.137713 psij-python-0.9.7/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      904 2024-05-01 04:36:19.000000 psij-python-0.9.7/README.md
--rw-rw-r--   0 mike      (1000) mike      (1000)       87 2024-05-01 04:36:19.000000 psij-python-0.9.7/requirements.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-05-01 04:39:00.137713 psij-python-0.9.7/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     1213 2024-05-01 04:36:19.000000 psij-python-0.9.7/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.129711 psij-python-0.9.7/src/
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/
--rw-rw-r--   0 mike      (1000) mike      (1000)     3577 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      243 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/__main__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4766 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/_plugins.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4875 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3003 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/exceptions.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/
--rw-rw-r--   0 mike      (1000) mike      (1000)      341 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/__init__.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/batch/
--rw-rw-r--   0 mike      (1000) mike      (1000)       86 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    31379 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/batch_scheduler_executor.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/batch/cobalt/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1759 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/cobalt/cobalt.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     5704 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/cobalt.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      807 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/escape_functions.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/batch/lsf/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1814 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/lsf/lsf.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     6177 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/lsf.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/batch/pbs/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1586 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/pbs/pbs_classic.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     1675 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/pbs/pbspro.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)      988 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/pbs.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7118 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/pbs_base.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1138 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/pbs_classic.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3248 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/script_generator.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/batch/slurm/
--rw-rw-r--   0 mike      (1000) mike      (1000)     3225 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/slurm/slurm.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     9839 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/slurm.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2343 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/template_function_library.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7359 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/flux.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    15054 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/local.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6220 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/rp.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    10706 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7127 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_attributes.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    14194 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_executor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2721 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_executor_config.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4624 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_launcher.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    12790 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_spec.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4985 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_state.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1995 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_status.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4280 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launcher.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/launchers/
--rw-rw-r--   0 mike      (1000) mike      (1000)      623 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      557 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/aprun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      554 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/jsrun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      692 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/mpirun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1718 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/multiple.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     8023 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/script_based_launcher.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/launchers/scripts/
--rw-rw-r--   0 mike      (1000) mike      (1000)       69 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      300 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/aprun_launch.sh
--rwxrwxr-x   0 mike      (1000) mike      (1000)      307 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/jsrun_launch.sh
--rwxrwxr-x   0 mike      (1000) mike      (1000)      812 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/launcher_lib.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      546 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/mpi_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      594 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/multi_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      236 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/single_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      274 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/srun_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      643 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/single.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      660 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/srun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/py.typed
--rw-rw-r--   0 mike      (1000) mike      (1000)     9052 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/resource_spec.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    10549 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/serialize.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1881 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/utils.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      168 2024-05-01 04:38:57.000000 psij-python-0.9.7/src/psij/version.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij-descriptors/
--rw-rw-r--   0 mike      (1000) mike      (1000)      217 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/aprun_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      262 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/cobalt_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      616 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/core_descriptors.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      248 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/flux_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      216 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/jsrun_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      250 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/lsf_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      564 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/pbs_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      285 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/rp_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      258 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/slurm_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      214 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/srun_descriptor.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.137713 psij-python-0.9.7/src/psij_python.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      414 2024-05-01 04:39:00.000000 psij-python-0.9.7/src/psij_python.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     2850 2024-05-01 04:39:00.000000 psij-python-0.9.7/src/psij_python.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-05-01 04:39:00.000000 psij-python-0.9.7/src/psij_python.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       88 2024-05-01 04:39:00.000000 psij-python-0.9.7/src/psij_python.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       22 2024-05-01 04:39:00.000000 psij-python-0.9.7/src/psij_python.egg-info/top_level.txt
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.137713 psij-python-0.9.7/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)     2192 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_callbacks.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4938 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_doc_examples.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7981 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_executor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      994 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_executor_loading.py
--rwxrwxr-x   0 mike      (1000) mike      (1000)      316 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_executor_versions.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      610 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_infrastructure.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_issue_387_1.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_issue_387_2.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_issue_387_3.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      589 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_issue_435.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1606 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_job_spec.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2159 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_mpi.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1209 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_nodefile.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3289 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_resources.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      836 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_serialization.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      911 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_wait.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.408270 psij-python-0.9.8/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1065 2024-05-14 20:45:39.000000 psij-python-0.9.8/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)       25 2024-05-14 20:45:39.000000 psij-python-0.9.8/MANIFEST.in
+-rw-rw-r--   0 mike      (1000) mike      (1000)      414 2024-05-14 20:46:04.408270 psij-python-0.9.8/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      904 2024-05-14 20:45:39.000000 psij-python-0.9.8/README.md
+-rw-rw-r--   0 mike      (1000) mike      (1000)       75 2024-05-14 20:45:39.000000 psij-python-0.9.8/requirements.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-05-14 20:46:04.408270 psij-python-0.9.8/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1213 2024-05-14 20:45:39.000000 psij-python-0.9.8/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.400270 psij-python-0.9.8/src/
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.404270 psij-python-0.9.8/src/psij/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3577 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      243 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/__main__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4766 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/_plugins.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4875 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3003 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/exceptions.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.404270 psij-python-0.9.8/src/psij/executors/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      341 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/__init__.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.404270 psij-python-0.9.8/src/psij/executors/batch/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       86 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    31379 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/batch_scheduler_executor.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.404270 psij-python-0.9.8/src/psij/executors/batch/cobalt/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1759 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/cobalt/cobalt.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5704 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/cobalt.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      807 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/escape_functions.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.404270 psij-python-0.9.8/src/psij/executors/batch/lsf/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1814 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/lsf/lsf.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6177 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/lsf.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.404270 psij-python-0.9.8/src/psij/executors/batch/pbs/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1586 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/pbs/pbs_classic.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1675 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/pbs/pbspro.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)      988 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/pbs.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7118 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/pbs_base.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1138 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/pbs_classic.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3248 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/script_generator.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.404270 psij-python-0.9.8/src/psij/executors/batch/slurm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3225 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/slurm/slurm.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     9839 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/slurm.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2343 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/batch/template_function_library.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7359 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/flux.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    15054 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/local.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6220 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/executors/rp.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    10706 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/job.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7141 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/job_attributes.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    14194 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/job_executor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2721 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/job_executor_config.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4624 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/job_launcher.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    12759 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/job_spec.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4985 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/job_state.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1995 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/job_status.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4280 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launcher.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.404270 psij-python-0.9.8/src/psij/launchers/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      623 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      557 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/aprun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      554 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/jsrun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      692 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/mpirun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1718 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/multiple.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     8023 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/script_based_launcher.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.408270 psij-python-0.9.8/src/psij/launchers/scripts/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       69 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/scripts/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      300 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/scripts/aprun_launch.sh
+-rwxrwxr-x   0 mike      (1000) mike      (1000)      307 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/scripts/jsrun_launch.sh
+-rwxrwxr-x   0 mike      (1000) mike      (1000)      812 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/scripts/launcher_lib.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      546 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/scripts/mpi_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      594 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/scripts/multi_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      236 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/scripts/single_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      274 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/scripts/srun_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      643 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/single.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      660 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/launchers/srun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/py.typed
+-rw-rw-r--   0 mike      (1000) mike      (1000)     9017 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/resource_spec.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    10549 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/serialize.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1881 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij/utils.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      168 2024-05-14 20:46:00.000000 psij-python-0.9.8/src/psij/version.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.404270 psij-python-0.9.8/src/psij-descriptors/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      217 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij-descriptors/aprun_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      262 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij-descriptors/cobalt_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      616 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij-descriptors/core_descriptors.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      248 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij-descriptors/flux_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      216 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij-descriptors/jsrun_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      250 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij-descriptors/lsf_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      564 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij-descriptors/pbs_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      285 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij-descriptors/rp_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      258 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij-descriptors/slurm_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      214 2024-05-14 20:45:39.000000 psij-python-0.9.8/src/psij-descriptors/srun_descriptor.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.408270 psij-python-0.9.8/src/psij_python.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      414 2024-05-14 20:46:04.000000 psij-python-0.9.8/src/psij_python.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2850 2024-05-14 20:46:04.000000 psij-python-0.9.8/src/psij_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-05-14 20:46:04.000000 psij-python-0.9.8/src/psij_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       75 2024-05-14 20:46:04.000000 psij-python-0.9.8/src/psij_python.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       22 2024-05-14 20:46:04.000000 psij-python-0.9.8/src/psij_python.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-14 20:46:04.408270 psij-python-0.9.8/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2192 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_callbacks.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4938 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_doc_examples.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7981 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_executor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      994 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_executor_loading.py
+-rwxrwxr-x   0 mike      (1000) mike      (1000)      316 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_executor_versions.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      610 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_infrastructure.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_issue_387_1.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_issue_387_2.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_issue_387_3.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      589 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_issue_435.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1691 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_job_spec.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2159 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_mpi.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1209 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_nodefile.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3289 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_resources.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      836 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_serialization.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      911 2024-05-14 20:45:39.000000 psij-python-0.9.8/tests/test_wait.py
```

### Comparing `psij-python-0.9.7/LICENSE` & `psij-python-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/README.md` & `psij-python-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/setup.py` & `psij-python-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/__init__.py` & `psij-python-0.9.8/src/psij/__init__.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/_plugins.py` & `psij-python-0.9.8/src/psij/_plugins.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/descriptor.py` & `psij-python-0.9.8/src/psij/descriptor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/exceptions.py` & `psij-python-0.9.8/src/psij/exceptions.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/batch_scheduler_executor.py` & `psij-python-0.9.8/src/psij/executors/batch/batch_scheduler_executor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/cobalt/cobalt.mustache` & `psij-python-0.9.8/src/psij/executors/batch/cobalt/cobalt.mustache`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/cobalt.py` & `psij-python-0.9.8/src/psij/executors/batch/cobalt.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/escape_functions.py` & `psij-python-0.9.8/src/psij/executors/batch/escape_functions.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/lsf/lsf.mustache` & `psij-python-0.9.8/src/psij/executors/batch/lsf/lsf.mustache`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/lsf.py` & `psij-python-0.9.8/src/psij/executors/batch/lsf.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/pbs/pbs_classic.mustache` & `psij-python-0.9.8/src/psij/executors/batch/pbs/pbs_classic.mustache`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/pbs/pbspro.mustache` & `psij-python-0.9.8/src/psij/executors/batch/pbs/pbspro.mustache`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/pbs.py` & `psij-python-0.9.8/src/psij/executors/batch/pbs.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/pbs_base.py` & `psij-python-0.9.8/src/psij/executors/batch/pbs_base.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/pbs_classic.py` & `psij-python-0.9.8/src/psij/executors/batch/pbs_classic.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/script_generator.py` & `psij-python-0.9.8/src/psij/executors/batch/script_generator.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/slurm/slurm.mustache` & `psij-python-0.9.8/src/psij/executors/batch/slurm/slurm.mustache`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/slurm.py` & `psij-python-0.9.8/src/psij/executors/batch/slurm.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/batch/template_function_library.py` & `psij-python-0.9.8/src/psij/executors/batch/template_function_library.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/flux.py` & `psij-python-0.9.8/src/psij/executors/flux.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/local.py` & `psij-python-0.9.8/src/psij/executors/local.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/executors/rp.py` & `psij-python-0.9.8/src/psij/executors/rp.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/job.py` & `psij-python-0.9.8/src/psij/job.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/job_attributes.py` & `psij-python-0.9.8/src/psij/job_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import logging
 import re
 from datetime import timedelta
 from typing import Optional, Dict
 
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 
 logger = logging.getLogger(__name__)
 
 
 _WALLTIME_FMT_ERROR = 'Unknown walltime format: %s. Accepted formats are hh:mm:ss, ' \
                       'hh:mm, mm, or n\\s*[h|m|s].'
 
 
 class JobAttributes(object):
     """A class containing ancillary job information that describes how a job is to be run."""
 
+    @typechecked
     def __init__(self, duration: timedelta = timedelta(minutes=10),
                  queue_name: Optional[str] = None, account: Optional[str] = None,
                  reservation_id: Optional[str] = None,
                  custom_attributes: Optional[Dict[str, object]] = None,
                  project_name: Optional[str] = None) -> None:
         """
         :param duration: Specifies the duration (walltime) of the job. A job whose execution
@@ -45,16 +46,14 @@
             `pbs.c`, `lsf.core_isolation`) and translate them into the corresponding batch
             scheduler directives (e.g., `#SLURM --constraint=...`, `#PBS -c ...`,
             `#BSUB -core_isolation ...`).
         :param project_name: Deprecated. Please use the `account` attribute.
 
         All constructor parameters are accessible as properties.
         """
-        assert check_argument_types()
-
         self.account = account
         self.duration = duration
         self.queue_name = queue_name
         self.project_name = project_name
         self.reservation_id = reservation_id
         self._custom_attributes = custom_attributes
 
@@ -162,10 +161,11 @@
     @property
     def project_name(self) -> Optional[str]:
         """Deprecated. Please use the `account` attribute."""
         return self.account
 
     @project_name.setter
     def project_name(self, project_name: Optional[str]) -> None:
-        logger.warning('The "project_name" attribute is deprecated. Please use the "account" '
-                       'attribute instead.')
+        if project_name is not None:
+            logger.warning('The "project_name" attribute is deprecated. Please use the "account" '
+                           'attribute instead.')
         self.account = project_name
```

### Comparing `psij-python-0.9.7/src/psij/job_executor.py` & `psij-python-0.9.8/src/psij/job_executor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/job_executor_config.py` & `psij-python-0.9.8/src/psij/job_executor_config.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/job_launcher.py` & `psij-python-0.9.8/src/psij/job_launcher.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/job_spec.py` & `psij-python-0.9.8/src/psij/job_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 # for some reason, Sphinx cannot find Path if imported directly
 # from pathlib import Path
 import pathlib
 from typing import Dict, List, Optional, Union
 
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 import psij.resource_spec
 import psij.job_attributes
 
 
 def _to_path(arg: Union[str, pathlib.Path, None]) -> Optional[pathlib.Path]:
     if isinstance(arg, pathlib.Path):
@@ -32,14 +32,15 @@
             ret[k] = v
     return ret
 
 
 class JobSpec(object):
     """A class that describes the details of a job."""
 
+    @typechecked
     def __init__(self, executable: Optional[str] = None, arguments: Optional[List[str]] = None,
                  # For some odd reason, and only in the constructor, if Path is used directly,
                  # sphinx fails to find the class. Using Path in the getters and setters does not
                  # appear to trigger a problem.
                  directory: Union[str, pathlib.Path, None] = None, name: Optional[str] = None,
                  inherit_environment: bool = True,
                  environment: Optional[Dict[str, Union[str, int]]] = None,
@@ -125,16 +126,14 @@
             to `/tmp/bar.txt`.
 
             Relative paths are useful when there is a need to refer to the job directory that the
             scheduler chooses for the job, which is not generally known until the job is started by
             the scheduler. In such a case, one must leave the `spec.directory` attribute empty and
             refer to files inside the job directory using relative paths.
         """
-        assert check_argument_types()
-
         self._name = name
         self.executable = executable
         self.arguments = arguments
         # I would do self.directory = directory, because that goes through the setter, which takes
         # care of the conversion, but mypy gets confused
         self._directory = _to_path(directory)
         self.inherit_environment = inherit_environment
```

### Comparing `psij-python-0.9.7/src/psij/job_state.py` & `psij-python-0.9.8/src/psij/job_state.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/job_status.py` & `psij-python-0.9.8/src/psij/job_status.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launcher.py` & `psij-python-0.9.8/src/psij/launcher.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launchers/__init__.py` & `psij-python-0.9.8/src/psij/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launchers/aprun.py` & `psij-python-0.9.8/src/psij/launchers/aprun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launchers/jsrun.py` & `psij-python-0.9.8/src/psij/launchers/jsrun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launchers/mpirun.py` & `psij-python-0.9.8/src/psij/launchers/mpirun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launchers/multiple.py` & `psij-python-0.9.8/src/psij/launchers/multiple.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launchers/script_based_launcher.py` & `psij-python-0.9.8/src/psij/launchers/script_based_launcher.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launchers/scripts/launcher_lib.sh` & `psij-python-0.9.8/src/psij/launchers/scripts/launcher_lib.sh`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launchers/scripts/mpi_launch.sh` & `psij-python-0.9.8/src/psij/launchers/scripts/mpi_launch.sh`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launchers/scripts/multi_launch.sh` & `psij-python-0.9.8/src/psij/launchers/scripts/multi_launch.sh`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launchers/single.py` & `psij-python-0.9.8/src/psij/launchers/single.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/launchers/srun.py` & `psij-python-0.9.8/src/psij/launchers/srun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/resource_spec.py` & `psij-python-0.9.8/src/psij/resource_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import Optional, List
 
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 from psij.exceptions import InvalidJobException
 
 
 def _nulls(objs: List[object]) -> int:
     s = 0
     for e in objs:
@@ -41,14 +41,15 @@
         """
         if version == 1:
             return ResourceSpecV1()
         else:
             raise ValueError()
 
 
+@typechecked
 class ResourceSpecV1(ResourceSpec):
     """This class implements V1 of the PSI/J resource specification."""
 
     def __init__(self, node_count: Optional[int] = None,
                  process_count: Optional[int] = None,
                  processes_per_node: Optional[int] = None,
                  cpu_cores_per_process: Optional[int] = None,
@@ -77,16 +78,14 @@
             is requesting fewer cores than the total number of cores on a node. With this parameter
             set to `False`, which is the default, the LRM is free to co-schedule multiple jobs
             on a given node if the number of cores requested by those jobs total less than the
             amount available on the node.
 
         All constructor parameters are accessible as properties.
         """
-        assert check_argument_types()
-
         self.node_count = node_count
         self.process_count = process_count
         self.processes_per_node = processes_per_node
         self.cpu_cores_per_process = cpu_cores_per_process
         self.gpu_cores_per_process = gpu_cores_per_process
         self.exclusive_node_use = exclusive_node_use
         self._check_constraints()
```

### Comparing `psij-python-0.9.7/src/psij/serialize.py` & `psij-python-0.9.8/src/psij/serialize.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij/utils.py` & `psij-python-0.9.8/src/psij/utils.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij-descriptors/core_descriptors.py` & `psij-python-0.9.8/src/psij-descriptors/core_descriptors.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij-descriptors/pbs_descriptor.py` & `psij-python-0.9.8/src/psij-descriptors/pbs_descriptor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/src/psij_python.egg-info/SOURCES.txt` & `psij-python-0.9.8/src/psij_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/tests/test_callbacks.py` & `psij-python-0.9.8/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/tests/test_doc_examples.py` & `psij-python-0.9.8/tests/test_doc_examples.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/tests/test_executor.py` & `psij-python-0.9.8/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/tests/test_executor_loading.py` & `psij-python-0.9.8/tests/test_executor_loading.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/tests/test_infrastructure.py` & `psij-python-0.9.8/tests/test_infrastructure.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/tests/test_issue_435.py` & `psij-python-0.9.8/tests/test_issue_435.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/tests/test_job_spec.py` & `psij-python-0.9.8/tests/test_job_spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import os
 from pathlib import Path
 
+from typeguard import suppress_type_checks
+
 import pytest
 
 from psij import Job, JobExecutor, JobSpec
 
 
 def _test_spec(spec: JobSpec) -> None:
     ex = JobExecutor.get_instance('local')
     ex.submit(Job(spec))
 
 
 def test_environment_types() -> None:
 
-    with pytest.raises(TypeError):
-        _test_spec(JobSpec(executable='true', environment={1: 'foo'}))  # type: ignore
+    with suppress_type_checks():
+        with pytest.raises(TypeError):
+            _test_spec(JobSpec(executable='true', environment={1: 'foo'}))  # type: ignore
 
     with pytest.raises(TypeError):
         spec = JobSpec(executable='true')
         spec.environment = {'foo': 'bar'}
         spec.environment['buz'] = [2]  # type: ignore
         _test_spec(spec)
```

### Comparing `psij-python-0.9.7/tests/test_mpi.py` & `psij-python-0.9.8/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/tests/test_nodefile.py` & `psij-python-0.9.8/tests/test_nodefile.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/tests/test_resources.py` & `psij-python-0.9.8/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/tests/test_serialization.py` & `psij-python-0.9.8/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.7/tests/test_wait.py` & `psij-python-0.9.8/tests/test_wait.py`

 * *Files identical despite different names*

