# Comparing `tmp/smartredis-0.5.2.tar.gz` & `tmp/smartredis-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartredis-0.5.2.tar", last modified: Fri Feb 16 04:39:13 2024, max compression
+gzip compressed data, was "smartredis-0.5.3.tar", last modified: Tue May 14 21:47:37 2024, max compression
```

## Comparing `smartredis-0.5.2.tar` & `smartredis-0.5.3.tar`

### file list

```diff
@@ -1,178 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.042146 smartredis-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-02-16 04:38:49.000000 smartredis-0.5.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-16 04:38:49.000000 smartredis-0.5.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-16 04:38:49.000000 smartredis-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23058 2024-02-16 04:38:49.000000 smartredis-0.5.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-02-16 04:39:13.042146 smartredis-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-02-16 04:38:49.000000 smartredis-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.030146 smartredis-0.5.2/include/
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/address.h
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/addressallcommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/addressanycommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/addressatcommand.h
--rw-r--r--   0 runner    (1001) docker     (127)    82235 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/c_client.h
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/c_configoptions.h
--rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/c_dataset.h
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/c_logcontext.h
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/c_logger.h
--rw-r--r--   0 runner    (1001) docker     (127)    87124 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/client.h
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/clusterinfocommand.h
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/command.h
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/command.tcc
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/commandlist.h
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/commandlist.tcc
--rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/commandreply.h
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/compoundcommand.h
--rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/configoptions.h
--rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/dataset.h
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/dbinfocommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/dbnode.h
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/enum_fortran.inc
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/gettensorcommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/keyedcommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/logcontext.h
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/logger.h
--rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/metadata.h
--rw-r--r--   0 runner    (1001) docker     (127)    13075 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/metadatabuffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/metadatafield.h
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/multikeycommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/nonkeyedcommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/pipelinereply.h
--rw-r--r--   0 runner    (1001) docker     (127)    48169 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/pyclient.h
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/pyconfigoptions.h
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/pydataset.h
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/pylogcontext.h
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/pysrobject.h
--rw-r--r--   0 runner    (1001) docker     (127)    26463 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/redis.h
--rw-r--r--   0 runner    (1001) docker     (127)    35412 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/rediscluster.h
--rw-r--r--   0 runner    (1001) docker     (127)    32159 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/redisserver.h
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/scalarfield.h
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/scalarfield.tcc
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/sharedmemorylist.h
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/sharedmemorylist.tcc
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/singlekeycommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/sr_enums.h
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/srassert.h
--rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/srexception.h
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/srobject.h
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/stringfield.h
--rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/tensor.h
--rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/tensor.tcc
--rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/tensorbase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/tensorpack.h
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/threadpool.h
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-02-16 04:38:49.000000 smartredis-0.5.2/include/utility.h
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-16 04:38:49.000000 smartredis-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-16 04:38:49.000000 smartredis-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-16 04:39:13.042146 smartredis-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-02-16 04:38:49.000000 smartredis-0.5.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-02-16 04:38:49.000000 smartredis-0.5.2/smartredis_defs.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.018146 smartredis-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.030146 smartredis-0.5.2/src/c/
--rw-r--r--   0 runner    (1001) docker     (127)    47145 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/c/c_client.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/c/c_configoptions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/c/c_dataset.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/c/c_error.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/c/c_logcontext.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/c/c_logger.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.034146 smartredis-0.5.2/src/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/address.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/addressallcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/addressanycommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/addressatcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    82131 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/client.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/clusterinfocommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/command.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/commandlist.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/commandreply.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/compoundcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/configoptions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/dataset.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/dbinfocommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/dbnode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/gettensorcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/keyedcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/logger.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23104 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/metadata.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/metadatafield.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/multikeycommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/nonkeyedcommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/pipelinereply.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    30675 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/redis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    54439 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/rediscluster.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/redisserver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/singlekeycommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/srobject.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/stringfield.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/tensorbase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/tensorpack.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/threadpool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/cpp/utility.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.034146 smartredis-0.5.2/src/fortran/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.038146 smartredis-0.5.2/src/fortran/client/
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client/aggregation_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client/client_dataset_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client/client_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client/ensemble_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client/misc_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)    21582 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client/model_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client/put_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client/put_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (127)    13313 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client/script_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client/unpack_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client/unpack_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (127)    95415 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/client.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.038146 smartredis-0.5.2/src/fortran/configoptions/
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/configoptions/configoptions_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/configoptions.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.038146 smartredis-0.5.2/src/fortran/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/dataset/add_meta_scalar_common.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/dataset/add_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/dataset/dataset_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/dataset/get_meta_scalars_common.inc
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/dataset/metadata_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/dataset/tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc
--rw-r--r--   0 runner    (1001) docker     (127)    26722 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/dataset.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.038146 smartredis-0.5.2/src/fortran/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/errors/errors_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/errors.F90
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/fortran_c_interop.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.038146 smartredis-0.5.2/src/fortran/logcontext/
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/logcontext/logcontext_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/logcontext.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.038146 smartredis-0.5.2/src/fortran/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/logger/logger_interfaces.inc
--rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/fortran/logger.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.018146 smartredis-0.5.2/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.038146 smartredis-0.5.2/src/python/bindings/
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/bindings/bind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.018146 smartredis-0.5.2/src/python/module/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.042146 smartredis-0.5.2/src/python/module/smartredis/
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/module/smartredis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    78110 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/module/smartredis/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/module/smartredis/configoptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/module/smartredis/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/module/smartredis/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/module/smartredis/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/module/smartredis/logcontext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/module/smartredis/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/module/smartredis/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/module/smartredis/srobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/module/smartredis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.042146 smartredis-0.5.2/src/python/module/smartredis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-02-16 04:39:12.000000 smartredis-0.5.2/src/python/module/smartredis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-02-16 04:39:13.000000 smartredis-0.5.2/src/python/module/smartredis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 04:39:12.000000 smartredis-0.5.2/src/python/module/smartredis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 04:39:12.000000 smartredis-0.5.2/src/python/module/smartredis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-16 04:39:12.000000 smartredis-0.5.2/src/python/module/smartredis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-16 04:39:12.000000 smartredis-0.5.2/src/python/module/smartredis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.042146 smartredis-0.5.2/src/python/src/
--rw-r--r--   0 runner    (1001) docker     (127)    23330 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/src/pyclient.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/src/pyconfigoptions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/src/pydataset.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/src/pylogcontext.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-02-16 04:38:49.000000 smartredis-0.5.2/src/python/src/pysrobject.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:39:13.042146 smartredis-0.5.2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-02-16 04:38:49.000000 smartredis-0.5.2/utils/launch_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.360324 smartredis-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-05-14 21:47:05.000000 smartredis-0.5.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-14 21:47:05.000000 smartredis-0.5.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 21:47:05.000000 smartredis-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23002 2024-05-14 21:47:05.000000 smartredis-0.5.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-14 21:47:37.360324 smartredis-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-14 21:47:05.000000 smartredis-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.348324 smartredis-0.5.3/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/address.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/addressallcommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/addressanycommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/addressatcommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)    82235 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/c_client.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/c_configoptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/c_dataset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/c_logcontext.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/c_logger.h
+-rw-r--r--   0 runner    (1001) docker     (127)    87504 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/client.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/clusterinfocommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/command.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/command.tcc
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/commandlist.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/commandlist.tcc
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/commandreply.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/compoundcommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/configoptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21594 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/dataset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/dbinfocommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/dbnode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/enum_fortran.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/gettensorcommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/keyedcommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/logcontext.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/logger.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/metadata.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/metadatabuffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/metadatafield.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/multikeycommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/nonkeyedcommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/pipelinereply.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48169 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/pyclient.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/pyconfigoptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/pydataset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/pylogcontext.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/pysrobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26463 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/redis.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/rediscluster.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32457 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/redisserver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/scalarfield.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/scalarfield.tcc
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/sharedmemorylist.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/sharedmemorylist.tcc
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/singlekeycommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/sr_enums.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/srassert.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/srexception.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/srobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/stringfield.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15170 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/tensor.tcc
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/tensorbase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/tensorpack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/threadpool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-14 21:47:05.000000 smartredis-0.5.3/include/utility.h
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-14 21:47:05.000000 smartredis-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-14 21:47:37.360324 smartredis-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-14 21:47:05.000000 smartredis-0.5.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-14 21:47:05.000000 smartredis-0.5.3/smartredis_defs.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.336324 smartredis-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.348324 smartredis-0.5.3/src/c/
+-rw-r--r--   0 runner    (1001) docker     (127)    47145 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/c/c_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/c/c_configoptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/c/c_dataset.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/c/c_error.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/c/c_logcontext.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/c/c_logger.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.352324 smartredis-0.5.3/src/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/address.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/addressallcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/addressanycommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/addressatcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    81908 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/client.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/clusterinfocommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/command.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/commandlist.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/commandreply.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/compoundcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/configoptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/dataset.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/dbinfocommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/dbnode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/gettensorcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/keyedcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/logger.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23104 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/metadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/metadatafield.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/multikeycommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/nonkeyedcommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/pipelinereply.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/redis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    54450 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/rediscluster.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/redisserver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/singlekeycommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/srobject.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/stringfield.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/tensorbase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/tensorpack.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/threadpool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/cpp/utility.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.352324 smartredis-0.5.3/src/fortran/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.356324 smartredis-0.5.3/src/fortran/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client/aggregation_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client/client_dataset_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client/client_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client/ensemble_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client/misc_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    21582 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client/model_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client/put_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client/put_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    13313 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client/script_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client/unpack_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client/unpack_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    95415 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/client.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.356324 smartredis-0.5.3/src/fortran/configoptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/configoptions/configoptions_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/configoptions.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.356324 smartredis-0.5.3/src/fortran/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/dataset/add_meta_scalar_common.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/dataset/add_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/dataset/dataset_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/dataset/get_meta_scalars_common.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/dataset/metadata_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/dataset/tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    26722 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/dataset.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.356324 smartredis-0.5.3/src/fortran/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/errors/errors_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/errors.F90
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/fortran_c_interop.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.356324 smartredis-0.5.3/src/fortran/logcontext/
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/logcontext/logcontext_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/logcontext.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.356324 smartredis-0.5.3/src/fortran/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/logger/logger_interfaces.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/fortran/logger.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.336324 smartredis-0.5.3/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.356324 smartredis-0.5.3/src/python/bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/bindings/bind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.336324 smartredis-0.5.3/src/python/module/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.360324 smartredis-0.5.3/src/python/module/smartredis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/module/smartredis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78110 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/module/smartredis/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/module/smartredis/configoptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/module/smartredis/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/module/smartredis/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/module/smartredis/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/module/smartredis/logcontext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/module/smartredis/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/module/smartredis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/module/smartredis/srobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/module/smartredis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.360324 smartredis-0.5.3/src/python/module/smartredis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-14 21:47:37.000000 smartredis-0.5.3/src/python/module/smartredis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-14 21:47:37.000000 smartredis-0.5.3/src/python/module/smartredis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:47:37.000000 smartredis-0.5.3/src/python/module/smartredis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:47:37.000000 smartredis-0.5.3/src/python/module/smartredis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 21:47:37.000000 smartredis-0.5.3/src/python/module/smartredis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 21:47:37.000000 smartredis-0.5.3/src/python/module/smartredis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.360324 smartredis-0.5.3/src/python/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    23330 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/src/pyclient.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/src/pyconfigoptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/src/pydataset.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/src/pylogcontext.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-14 21:47:05.000000 smartredis-0.5.3/src/python/src/pysrobject.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:47:37.360324 smartredis-0.5.3/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-14 21:47:05.000000 smartredis-0.5.3/utils/launch_redis.py
```

### Comparing `smartredis-0.5.2/CMakeLists.txt` & `smartredis-0.5.3/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Enable setting version in the project statement
 if (POLICY CMP0048)
     cmake_policy(SET CMP0048 NEW)
 endif (POLICY CMP0048)
 
 # Project definition for the SmartRedis project
 cmake_minimum_required(VERSION 3.13)
-project(SmartRedis VERSION "0.5.2")
+project(SmartRedis VERSION "0.5.3")
 
 # Configure options for the SmartRedis project
 option(SR_PYTHON  "Build the python module" OFF)
 option(SR_FORTRAN "Build the fortran client library" OFF)
 option(SR_PEDANTIC "Build with pickiest compiler settings" OFF)
 
 set(CMAKE_CXX_STANDARD 17)
@@ -49,19 +49,31 @@
 if (SR_FORTRAN)
     enable_language(Fortran)
 endif()
 
 # For now, we only support Pedantic on the main library build.
 # If/when we fine-tune the examples and test cases, move this block
 # to smartredis_defs.cmake
+# Note: -Wextra can be added after unused parameters are addressed
 if (SR_PEDANTIC)
-    if((CMAKE_CXX_COMPILER_ID STREQUAL "GNU") AND (CMAKE_C_COMPILER_ID STREQUAL "GNU"))
-        add_compile_options(-Wall -Werror)
+    if(
+        (CMAKE_CXX_COMPILER_ID STREQUAL "GNU") OR
+        (CMAKE_CXX_COMPILER_ID STREQUAL "NVHPC")
+    )
+	set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Werror -pedantic -Wextra")
+	set(CMAKE_Fortran_FLAGS "${CMAKE_Fortran_FLAGS} -Wall -Werror -Wextra")
+    elseif(
+        (CMAKE_CXX_COMPILER_ID STREQUAL "Intel") OR
+        (CMAKE_CXX_COMPILER_ID STREQUAL "IntelLLVM")
+    )
+        set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Werror -pedantic")
+        set(CMAKE_Fortran_FLAGS "${CMAKE_Fortran_FLAGS} -warn all -warn error")
     else()
-        message(WARNING "SR_PEDANTIC was specified, but the CMAKE compiler is not GCC")
+        message(WARNING "SR_PEDANTIC not supported for ${CMAKE_CXX_COMPILER_ID}")
+        message(WARNING ${CMAKE_CXX_COMPILER_ID})
     endif()
     if(CMAKE_Fortran_COMPILER_ID STREQUAL "GNU")
         set(CMAKE_Fortran_FLAGS "${CMAKE_Fortran_FLAGS} -Wno-maybe-uninitialized")
     endif()
 endif()
 
 # Bring in third-party libaries needed for the SmartRedis library
```

### Comparing `smartredis-0.5.2/LICENSE.md` & `smartredis-0.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/Makefile` & `smartredis-0.5.3/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 HIREDIS_URL := https://github.com/redis/hiredis.git
 HIREDIS_VER := v1.2.0
 RPP_URL := https://github.com/sewenew/redis-plus-plus.git
 RPP_VER := 1.3.10
 PYBIND_URL := https://github.com/pybind/pybind11.git
 PYBIND_VER := v2.11.1
 REDIS_URL := https://github.com/redis/redis.git
-REDIS_VER := 7.0.5
+REDIS_VER := 7.2.4
 REDISAI_URL := https://github.com/RedisAI/RedisAI.git
 # REDISAI_VER is controlled instead by SR_TEST_REDISAI_VER below
 CATCH2_URL := https://github.com/catchorg/Catch2.git
 CATCH2_VER := v2.13.6
 LCOV_URL := https://github.com/linux-test-project/lcov.git
 LCOV_VER := v2.0
 DEP_CC := gcc
@@ -133,20 +133,20 @@
 # help: lib-with-fortran               - Build SmartRedis C/C++/Python and Fortran clients into a dynamic library
 .PHONY: lib-with-fortran
 lib-with-fortran: SR_FORTRAN=ON
 lib-with-fortran: lib
 
 # help: test-lib                       - Build SmartRedis clients into a dynamic library with least permissive compiler settings
 .PHONY: test-lib
-test-lib: SR_PEDANTIC=OFF #TODO: fix warnings in C++
+test-lib: SR_PEDANTIC=ON
 test-lib: lib
 
 # help: test-lib-with-fortran          - Build SmartRedis clients into a dynamic library with least permissive compiler settings
 .PHONY: test-lib-with-fortran
-test-lib-with-fortran: SR_PEDANTIC=OFF #TODO: fix warnings in C++
+test-lib-with-fortran: SR_PEDANTIC=ON
 test-lib-with-fortran: lib-with-fortran
 
 # help: test-deps                      - Make SmartRedis testing dependencies
 .PHONY: test-deps
 test-deps: redis
 test-deps: redisAI
 test-deps: catch2
```

### Comparing `smartredis-0.5.2/README.md` & `smartredis-0.5.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 SmartRedis is a collection of Redis clients that support
 RedisAI capabilities and include additional
 features for high performance computing (HPC) applications.
 SmartRedis provides clients in the following languages:
 
 | Language   | Version/Standard                               |
 |------------|:----------------------------------------------:|
-| Python     |   3.8, 3.9, 3.10, 3.11                         |
+| Python     |   3.9, 3.10, 3.11                              |
 | C++        |   C++17                                        |
 | C          |   C99                                          |
 | Fortran    |   Fortran 2018 (GNU/Intel), 2003 (PGI/Nvidia)  |
 
 SmartRedis is used in the [SmartSim library](https://github.com/CrayLabs/SmartSim).
 SmartSim makes it easier to use common Machine Learning (ML) libraries like
 PyTorch and TensorFlow in numerical simulations at scale.  SmartRedis connects
```

#### html2text {}

```diff
@@ -14,19 +14,19 @@
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![codecov](https://codecov.io/gh/CrayLabs/SmartRedis/
 branch/develop/graph/badge.svg?token=XSS8CCJ2KR)](https://codecov.io/gh/
 CrayLabs/SmartRedis) ---------- # SmartRedis SmartRedis is a collection of
 Redis clients that support RedisAI capabilities and include additional features
 for high performance computing (HPC) applications. SmartRedis provides clients
 in the following languages: | Language | Version/Standard | |------------|:----
-------------------------------------------:| | Python | 3.8, 3.9, 3.10, 3.11 |
-| C++ | C++17 | | C | C99 | | Fortran | Fortran 2018 (GNU/Intel), 2003 (PGI/
-Nvidia) | SmartRedis is used in the [SmartSim library](https://github.com/
-CrayLabs/SmartSim). SmartSim makes it easier to use common Machine Learning
-(ML) libraries like PyTorch and TensorFlow in numerical simulations at scale.
+------------------------------------------:| | Python | 3.9, 3.10, 3.11 | | C++
+| C++17 | | C | C99 | | Fortran | Fortran 2018 (GNU/Intel), 2003 (PGI/Nvidia) |
+SmartRedis is used in the [SmartSim library](https://github.com/CrayLabs/
+SmartSim). SmartSim makes it easier to use common Machine Learning (ML)
+libraries like PyTorch and TensorFlow in numerical simulations at scale.
 SmartRedis connects these simulations to a Redis database or Redis database
 cluster for data storage, script execution, and model evaluation. While
 SmartRedis contains features for simulation workflows on supercomputers,
 SmartRedis is fully functional as a RedisAI client library and can be used
 without SmartSim in any Python, C++, C, or Fortran project. ## Using SmartRedis
 SmartRedis installation instructions are currently hosted as part of the
 [SmartSim library installation instructions](https://www.craylabs.org/docs/
```

### Comparing `smartredis-0.5.2/include/address.h` & `smartredis-0.5.3/include/address.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/addressallcommand.h` & `smartredis-0.5.3/include/addressallcommand.h`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -73,8 +73,8 @@
         */
         int key_index;
 
 };
 
 } // namespace SmartRedis
 
-#endif // SMARTREDIS_ADDRRESSALLCOMMAND_H
+#endif // SMARTREDIS_ADDRRESSALLCOMMAND_H
```

### Comparing `smartredis-0.5.2/include/addressanycommand.h` & `smartredis-0.5.3/include/addressanycommand.h`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,8 @@
         *            type.
         */
         virtual Command* clone();
 };
 
 } // namespace SmartRedis
 
-#endif // SMARTREDIS_ADDRESSANYCOMMAND_H
+#endif // SMARTREDIS_ADDRESSANYCOMMAND_H
```

### Comparing `smartredis-0.5.2/include/addressatcommand.h` & `smartredis-0.5.3/include/addressatcommand.h`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -132,8 +132,8 @@
             return port;
         }
 
 };
 
 } // namespace SmartRedis
 
-#endif // SMARTREDIS_ADDRESSATCOMMAND_H
+#endif // SMARTREDIS_ADDRESSATCOMMAND_H
```

### Comparing `smartredis-0.5.2/include/c_client.h` & `smartredis-0.5.3/include/c_client.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/c_configoptions.h` & `smartredis-0.5.3/include/c_configoptions.h`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,16 @@
 *                          excluding null terminating character
 *   \param cfg_result Receives true IFF the option was defined or has been
 *                     overridden; false otherwise
 *   \returns Returns SRNoError on success or an error code on failure
 */
 SRError is_configured(
     void* c_cfgopts,
-    const char* key,
-    size_t key_len,
+    const char* option_name,
+    size_t option_name_len,
     bool* cfg_result);
 
 /////////////////////////////////////////////////////////////
 // Option overrides
 
 /*!
 *   \brief Override the value of a numeric configuration option
```

### Comparing `smartredis-0.5.2/include/c_dataset.h` & `smartredis-0.5.3/include/c_dataset.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/c_logcontext.h` & `smartredis-0.5.3/include/c_logcontext.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/c_logger.h` & `smartredis-0.5.3/include/c_logger.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/client.h` & `smartredis-0.5.3/include/client.h`

 * *Files 0% similar despite different names*

```diff
@@ -1747,14 +1747,21 @@
 
         /*!
         *   \brief Initialize a connection to the back-end database
         *   \throw SmartRedis::Exception if the connection fails
         */
        void _establish_server_connection();
 
+       /*!
+        *   \brief Augment exceptions with underlying connection errors
+        *   \param reply The CommandReply to inspect for errors
+        *   \param error_message The base error message to raise
+        *   \throw SmartRedis::Exception if poll list length command fails
+        */
+       void _report_reply_errors(CommandReply &reply, std::string error_message);
 };
 
 /*!
 *   \brief Serialize a client
 *   \param stream The stream onto which to serialize the client
 *   \param client The client to serialize
 *   \returns The output stream, for chaining
```

### Comparing `smartredis-0.5.2/include/clusterinfocommand.h` & `smartredis-0.5.3/include/clusterinfocommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/command.h` & `smartredis-0.5.3/include/command.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/command.tcc` & `smartredis-0.5.3/include/command.tcc`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 void Command::add_keys(const std::vector<T>& keyfields)
 {
     for (size_t i = 0; i < keyfields.size(); i++) {
         this->add_field(std::to_string(keyfields[i]), true);
     }
 }
 
-#endif // SMARTREDIS_COMMAND_TCC
+#endif // SMARTREDIS_COMMAND_TCC
```

### Comparing `smartredis-0.5.2/include/commandlist.h` & `smartredis-0.5.3/include/commandlist.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/commandlist.tcc` & `smartredis-0.5.3/include/commandlist.tcc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/commandreply.h` & `smartredis-0.5.3/include/commandreply.h`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_COMMANDREPLY_H
 #define SMARTREDIS_COMMANDREPLY_H
 
-#include "stdlib.h"
+#include <stdlib.h>
 #include <sw/redis++/redis++.h>
 #include <iostream>
 #include <vector>
 #include <queue>
 
 ///@file
```

### Comparing `smartredis-0.5.2/include/compoundcommand.h` & `smartredis-0.5.3/include/compoundcommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/configoptions.h` & `smartredis-0.5.3/include/configoptions.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/dataset.h` & `smartredis-0.5.3/include/dataset.h`

 * *Files 4% similar despite different names*

```diff
@@ -472,14 +472,23 @@
         /*!
         *   \brief Throw an exception if a tensor does not exist
         *   \throw RuntimeException if the tensor is not in the DataSet
         */
         inline void _enforce_tensor_exists(const std::string& name) const;
 
         /*!
+        *   \brief Throw an exception if the provided tensor type does not match
+        *          the internal tensor type
+        *   \throw RuntimeException if the provided tensor type does not match
+        *          the internal tensor type
+        */
+        inline void _enforce_tensor_type(const std::string& tensorname,
+                                         const SRTensorType& type) const;
+
+        /*!
         *   \brief SharedMemoryList to manage memory associated
         *          with tensor dimensions from tensor retrieval
         */
         mutable SharedMemoryList<size_t> _dim_queries;
 
         /*!
         *  \brief The _tensor_pack memory is not for querying
```

### Comparing `smartredis-0.5.2/include/dbinfocommand.h` & `smartredis-0.5.3/include/dbinfocommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/dbnode.h` & `smartredis-0.5.3/include/dbnode.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/enum_fortran.inc` & `smartredis-0.5.3/include/enum_fortran.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/gettensorcommand.h` & `smartredis-0.5.3/include/gettensorcommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/keyedcommand.h` & `smartredis-0.5.3/include/keyedcommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/logcontext.h` & `smartredis-0.5.3/include/logcontext.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/logger.h` & `smartredis-0.5.3/include/logger.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/metadata.h` & `smartredis-0.5.3/include/metadata.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/metadatabuffer.h` & `smartredis-0.5.3/include/metadatabuffer.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 #ifndef SMARTREDIS_METADATABUFFER_H
 #define SMARTREDIS_METADATABUFFER_H
 
 #include <iostream>
 #include <vector>
 #include <string>
 #include <cstring>
+#include <cstdint>
 #include "srexception.h"
 
 using namespace SmartRedis;
 
 namespace MetadataBuffer {
 
 /*!
```

### Comparing `smartredis-0.5.2/include/metadatafield.h` & `smartredis-0.5.3/include/metadatafield.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/multikeycommand.h` & `smartredis-0.5.3/include/multikeycommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/nonkeyedcommand.h` & `smartredis-0.5.3/include/nonkeyedcommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/pipelinereply.h` & `smartredis-0.5.3/include/pipelinereply.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/pyclient.h` & `smartredis-0.5.3/include/pyclient.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/pyconfigoptions.h` & `smartredis-0.5.3/include/pyconfigoptions.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/pydataset.h` & `smartredis-0.5.3/include/pydataset.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/pylogcontext.h` & `smartredis-0.5.3/include/pylogcontext.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/pysrobject.h` & `smartredis-0.5.3/include/pysrobject.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/redis.h` & `smartredis-0.5.3/include/redis.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/rediscluster.h` & `smartredis-0.5.3/include/rediscluster.h`

 * *Files 0% similar despite different names*

```diff
@@ -734,24 +734,25 @@
         *   \throw SmartRedis::Exception execution fails
         */
         void __run_model_dagrun(const std::string& key,
                                 std::vector<std::string> inputs,
                                 std::vector<std::string> outputs);
 
         /*!
-        *   \brief  Retrieve the optimum model prefix for
-        *           the set of inputs
-        *   \param name The name of the model
+        *   \brief  Retrieve the db node in the cluster that contains
+        *           the most input and output tensors.  If multiple
+        *           db nodes contain the same amount of input and
+        *           output tensors, the first db node in the internal
+        *           data structure is returned.
         *   \param inputs The keys of inputs tensors to use
         *                 in the model
         *   \param outputs The keys of output tensors that
         *                 will be used to save model results
         */
-        DBNode* _get_model_script_db(const std::string& name,
-                                     std::vector<std::string>& inputs,
+        DBNode* _get_model_script_db(std::vector<std::string>& inputs,
                                      std::vector<std::string>& outputs);
 
         /*!
         *   \brief Reconfigure the chunking size that Redis uses for model
         *          serialization, replication, and the model_get command.
         *   \details This method triggers the AI.CONFIG method in the Redis
         *            database to change the model chunking size.
```

### Comparing `smartredis-0.5.2/include/redisserver.h` & `smartredis-0.5.3/include/redisserver.h`

 * *Files 0% similar despite different names*

```diff
@@ -577,14 +577,19 @@
 
         /*!
         *   \brief Timeout (in seconds) of command attempt(s).
         */
         int _command_timeout;
 
         /*!
+        *   \brief Timeout (in milliseconds) for socket reply.
+        */
+        int _socket_timeout;
+
+        /*!
         *   \brief Interval (in milliseconds) between connection attempts.
         */
         int _connection_interval;
 
         /*!
         *   \brief Interval (in milliseconds) between command execution attempts.
         */
@@ -711,14 +716,20 @@
         /*!
         *   \brief Environment variable for model execution timeout
         */
         inline static const std::string _MODEL_TIMEOUT_ENV_VAR =
             "SR_MODEL_TIMEOUT";
 
         /*!
+        *   \brief Environment variable for socket timeout
+        */
+        inline static const std::string _SOCKET_TIMEOUT_ENV_VAR =
+            "SR_SOCKET_TIMEOUT";
+
+        /*!
         *   \brief Environment variable for thread count in thread pool
         */
         inline static const std::string _TP_THREAD_COUNT =
             "SR_THREAD_COUNT";
 
         /*!
         *   \brief Retrieve a single address, randomly
```

### Comparing `smartredis-0.5.2/include/scalarfield.h` & `smartredis-0.5.3/include/scalarfield.h`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -155,8 +155,8 @@
 
 };
 
 #include "scalarfield.tcc"
 
 } // namespace SmartRedis
 
-#endif // SMARTREDIS_SCALARFIELD_H
+#endif // SMARTREDIS_SCALARFIELD_H
```

### Comparing `smartredis-0.5.2/include/scalarfield.tcc` & `smartredis-0.5.3/include/scalarfield.tcc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/sharedmemorylist.h` & `smartredis-0.5.3/include/sharedmemorylist.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/sharedmemorylist.tcc` & `smartredis-0.5.3/include/sharedmemorylist.tcc`

 * *Files 7% similar despite different names*

```diff
@@ -25,19 +25,29 @@
  * OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
  * OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef SMARTREDIS_SHAREDMEMORYLIST_TCC
 #define SMARTREDIS_SHAREDMEMORYLIST_TCC
 
+// Define memory deletion operator (delete[]) to
+// match the memory allocation operator (new[])
+class PointerDeletion {
+    public:
+        template<class T>
+        void operator()(T* ptr) const {
+            delete[] ptr;
+        }
+};
+
 // Record a memory allocation
 template <class T>
 void SharedMemoryList<T>::add_allocation(size_t bytes, T* ptr)
 {
-    std::shared_ptr<T> s_ptr(ptr);
+    std::shared_ptr<T> s_ptr(ptr, PointerDeletion());
     _inventory.push_front(s_ptr);
 }
 
 // Allocate memory and record the allocation
 template <class T>
 T* SharedMemoryList<T>::allocate_bytes(size_t bytes)
 {
```

### Comparing `smartredis-0.5.2/include/singlekeycommand.h` & `smartredis-0.5.3/include/singlekeycommand.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/sr_enums.h` & `smartredis-0.5.3/include/sr_enums.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/srassert.h` & `smartredis-0.5.3/include/srassert.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/srexception.h` & `smartredis-0.5.3/include/srexception.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/srobject.h` & `smartredis-0.5.3/include/srobject.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/stringfield.h` & `smartredis-0.5.3/include/stringfield.h`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -146,8 +146,8 @@
         */
         std::vector<std::string> _vals;
 
 };
 
 } // namespace SmartRedis
 
-#endif // SMARTREDIS_STRINGFIELD_H
+#endif // SMARTREDIS_STRINGFIELD_H
```

### Comparing `smartredis-0.5.2/include/tensor.h` & `smartredis-0.5.3/include/tensor.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/tensor.tcc` & `smartredis-0.5.3/include/tensor.tcc`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 // Tensor constructor
 template <class T>
 Tensor<T>::Tensor(const std::string& name,
                   const void* data,
                   const std::vector<size_t>& dims,
                   const SRTensorType type,
                   const SRMemoryLayout mem_layout) :
-                  TensorBase(name, data, dims, type, mem_layout)
+                  TensorBase(name, data, dims, type)
 {
     _set_tensor_data(data, dims, mem_layout);
 }
 
 // Tensor copy constructor
 template <class T>
 Tensor<T>::Tensor(const Tensor<T>& tensor) : TensorBase(tensor)
```

### Comparing `smartredis-0.5.2/include/tensorbase.h` & `smartredis-0.5.3/include/tensorbase.h`

 * *Files 0% similar despite different names*

```diff
@@ -93,16 +93,15 @@
         *   \param dims The dimensions of the tensor
         *   \param type The data type of the tensor
         *   \param mem_layout The memory layout of the source data
         */
         TensorBase(const std::string& name,
                    const void* data,
                    const std::vector<size_t>& dims,
-                   const SRTensorType type,
-                   const SRMemoryLayout mem_layout);
+                   const SRTensorType type);
 
         /*!
         *   \brief TensorBase copy constructor
         *   \param tb The TensorBase to copy for construction
         */
         TensorBase(const TensorBase& tb);
```

### Comparing `smartredis-0.5.2/include/tensorpack.h` & `smartredis-0.5.3/include/tensorpack.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/threadpool.h` & `smartredis-0.5.3/include/threadpool.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/include/utility.h` & `smartredis-0.5.3/include/utility.h`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/pyproject.toml` & `smartredis-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools>=42",
             "wheel",
             "cmake>=3.13"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 88
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py39', 'py310', 'py311']
 exclude = '''
 (
   | \.egg
   | \.git
   | \.hg
   | \.mypy_cache
   | \.nox
```

### Comparing `smartredis-0.5.2/setup.cfg` & `smartredis-0.5.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [metadata]
 name = smartredis
-version = 0.5.2
+version = 0.5.3
 description = RedisAI clients for SmartSim
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrayLabs/SmartRedis
 project_urls = 
 	Source = https://github.com/CrayLabs/SmartRedis
 	Documentation = https://www.craylabs.org
 author = CrayLabs, a Hewlett Packard Enterprise OSS Organization
 author_email = craylabs@hpe.com
 contact = CrayLabs, a Hewlett Packard Enterprise OSS Organization
 contact_email = craylabs@hpe.com
 license = BSD 2-Clause License
 keywords = redis, clients, hpc, ai, deep learning
 classifiers = 
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: BSD License
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
 
@@ -28,23 +27,23 @@
 	=src/python/module
 packages = find:
 setup_requires = 
 	setuptools>=42
 include_package_data = True
 install_requires = 
 	numpy>=1.18.2
-python_requires = >=3.8,<3.12
+python_requires = >=3.9,<3.12
 
 [options.extras_require]
 dev = 
 	pytest>=6.0.0
 	pytest-cov==2.10.1
 	black==23.3.0
 	isort==5.6.4
-	pylint>=2.10.0
+	pylint>=2.10.0,<3.2.0
 	torch<=2.0.1
 	mypy>=1.4.0
 	typing_extensions
 	jinja2==3.0.3
 doc = 
 	sphinx==3.1.1
 	sphinx-fortran==1.1.1
```

### Comparing `smartredis-0.5.2/setup.py` & `smartredis-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/smartredis_defs.cmake` & `smartredis-0.5.3/smartredis_defs.cmake`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/c/c_client.cpp` & `smartredis-0.5.3/src/c/c_client.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/c/c_configoptions.cpp` & `smartredis-0.5.3/src/c/c_configoptions.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/c/c_dataset.cpp` & `smartredis-0.5.3/src/c/c_dataset.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/c/c_error.cpp` & `smartredis-0.5.3/src/c/c_error.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/c/c_logcontext.cpp` & `smartredis-0.5.3/src/c/c_logcontext.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/c/c_logger.cpp` & `smartredis-0.5.3/src/c/c_logger.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/address.cpp` & `smartredis-0.5.3/src/cpp/address.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/addressallcommand.cpp` & `smartredis-0.5.3/src/cpp/addressallcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/addressanycommand.cpp` & `smartredis-0.5.3/src/cpp/addressanycommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/addressatcommand.cpp` & `smartredis-0.5.3/src/cpp/addressatcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/client.cpp` & `smartredis-0.5.3/src/cpp/client.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -281,18 +281,16 @@
     std::vector<std::string> tensor_keys =
         _build_dataset_tensor_keys(dataset.get_name(), tensor_names, true);
     cmd.add_keys(tensor_keys);
 
     // Run the command
     reply = _run(cmd);
 
-    if (reply.has_error()) {
-        throw SRRuntimeException("An error was encountered when executing "\
-                                 "DataSet " + name + " deletion.");
-    }
+    _report_reply_errors(reply, "An error was encountered when executing "\
+                                "DataSet " + name + " deletion.");
 }
 
 // Put a tensor into the database
 void Client::put_tensor(const std::string& name,
                         const void* data,
                         const std::vector<size_t>& dims,
                         const SRTensorType type,
@@ -340,16 +338,15 @@
 
     // Send the tensor
     CommandReply reply = _redis_server->put_tensor(*tensor);
 
     // Cleanup
     delete tensor;
     tensor = NULL;
-    if (reply.has_error())
-        throw SRRuntimeException("put_tensor failed");
+    _report_reply_errors(reply, "put_tensor failed");
 }
 
 // Get the tensor data, dimensions, and type for the provided tensor name.
 // This function will allocate and retain management of the memory for the
 // tensor data.
 void Client::get_tensor(const std::string& name,
                         void*& data,
@@ -532,42 +529,39 @@
 {
     // Track calls to this API function
     LOG_API_FUNCTION();
 
     std::string old_key = _build_tensor_key(old_name, true);
     std::string new_key = _build_tensor_key(new_name, false);
     CommandReply reply = _redis_server->rename_tensor(old_key, new_key);
-    if (reply.has_error())
-        throw SRRuntimeException("rename_tensor failed");
+    _report_reply_errors(reply, "rename_tensor failed");
 }
 
 // Delete a tensor from the database
 void Client::delete_tensor(const std::string& name)
 {
     // Track calls to this API function
     LOG_API_FUNCTION();
 
     std::string key = _build_tensor_key(name, true);
     CommandReply reply = _redis_server->delete_tensor(key);
-    if (reply.has_error())
-        throw SRRuntimeException("delete_tensor failed");
+    _report_reply_errors(reply, "delete_tensor failed");
 }
 
 // Copy the tensor from the source name to the destination name
 void Client::copy_tensor(const std::string& src_name,
                          const std::string& dest_name)
 {
     // Track calls to this API function
     LOG_API_FUNCTION();
 
     std::string src_key = _build_tensor_key(src_name, true);
     std::string dest_key = _build_tensor_key(dest_name, false);
     CommandReply reply = _redis_server->copy_tensor(src_key, dest_key);
-    if (reply.has_error())
-        throw SRRuntimeException("copy_tensor failed");
+    _report_reply_errors(reply, "copy_tensor failed");
 }
 
 // Set a model from file in the database for future execution
 void Client::set_model_from_file(const std::string& name,
                                  const std::string& model_file,
                                  const std::string& backend,
                                  const std::string& device,
@@ -815,16 +809,15 @@
 {
     // Track calls to this API function
     LOG_API_FUNCTION();
 
     // Get the model from the server
     std::string get_key = _build_model_key(name, true);
     CommandReply reply = _redis_server->get_model(get_key);
-    if (reply.has_error())
-        throw SRRuntimeException("failed to get model from server");
+    _report_reply_errors(reply, "failed to get model from server");
 
     // In most cases, the reply will be a single string
     // consisting of the serialized model
     if (!reply.is_array()) {
         char* model = _model_queries.allocate(reply.str_len());
         if (model == NULL)
             throw SRBadAllocException("model query");
@@ -1045,16 +1038,15 @@
 {
     // Track calls to this API function
     LOG_API_FUNCTION();
 
     std::string key = _build_model_key(name, true);
     CommandReply reply = _redis_server->delete_model(key);
 
-    if (reply.has_error())
-        throw SRRuntimeException("AI.MODELDEL command failed on server");
+    _report_reply_errors(reply, "AI.MODELDEL command failed on server");
 }
 
 // Delete a multiGPU model from the database
 void Client::delete_model_multigpu(
     const std::string& name, int first_gpu, int num_gpus)
 {
     // Track calls to this API function
@@ -1076,16 +1068,15 @@
 {
     // Track calls to this API function
     LOG_API_FUNCTION();
 
     std::string key = _build_model_key(name, true);
     CommandReply reply = _redis_server->delete_script(key);
 
-    if (reply.has_error())
-        throw SRRuntimeException("AI.SCRIPTDEL command failed on server");
+    _report_reply_errors(reply, "AI.SCRIPTDEL command failed on server");
 }
 
 // Delete a multiGPU script from the database
 void Client::delete_script_multigpu(
     const std::string& name, int first_gpu, int num_gpus)
 {
     // Track calls to this API function
@@ -1313,17 +1304,15 @@
 
     // Run an INFO EVERYTHING command to get node info
     DBInfoCommand cmd;
     SRAddress db_address(address);
     cmd.set_exec_address(db_address);
     cmd << "INFO" << "EVERYTHING";
     CommandReply reply = _run(cmd);
-    if (reply.has_error())
-        throw SRRuntimeException("INFO EVERYTHING command failed on server");
-
+    _report_reply_errors(reply, "INFO EVERYTHING command failed on server");
     // Parse the results
     std::string db_node_info(reply.str(), reply.str_len());
     return DBInfoCommand::parse_db_node_info(db_node_info);
 }
 
 // Returns the CLUSTER INFO command reply addressed to a single cluster node.
 parsed_reply_map Client::get_db_cluster_info(const std::string address)
@@ -1336,16 +1325,15 @@
 
     // Run the CLUSTER INFO command
     ClusterInfoCommand cmd;
     SRAddress db_address(address);
     cmd.set_exec_address(db_address);
     cmd << "CLUSTER" << "INFO";
     CommandReply reply = _run(cmd);
-    if (reply.has_error())
-        throw SRRuntimeException("CLUSTER INFO command failed on server");
+    _report_reply_errors(reply, "CLUSTER INFO command failed on server");
 
     // Parse the results
     std::string db_cluster_info(reply.str(), reply.str_len());
     return ClusterInfoCommand::parse_db_cluster_info(db_cluster_info);
 }
 
 // Returns the AI.INFO command reply
@@ -1356,16 +1344,15 @@
     // Track calls to this API function
     LOG_API_FUNCTION();
 
     // Run the command
     CommandReply reply =
         _redis_server->get_model_script_ai_info(address, key, reset_stat);
 
-    if (reply.has_error())
-        throw SRRuntimeException("AI.INFO command failed on server");
+    _report_reply_errors(reply, "AI.INFO command failed on server");
 
     if (reply.n_elements() % 2 != 0)
         throw SRInternalException("The AI.INFO reply structure has an "\
                                   "unexpected format");
 
     // Parse reply
     parsed_reply_map reply_map;
@@ -1403,16 +1390,15 @@
 
     AddressAtCommand cmd;
     SRAddress db_address(address);
     cmd.set_exec_address(db_address);
     cmd << "FLUSHDB";
 
     CommandReply reply = _run(cmd);
-    if (reply.has_error() > 0)
-        throw SRRuntimeException("FLUSHDB command failed");
+    _report_reply_errors(reply, "FLUSHDB command failed");
 }
 
 // Read the configuration parameters of a running server
 std::unordered_map<std::string,std::string>
 Client::config_get(
     const std::string expression,
     const std::string address)
@@ -1422,16 +1408,15 @@
 
     AddressAtCommand cmd;
     SRAddress db_address(address);
     cmd.set_exec_address(db_address);
     cmd << "CONFIG" << "GET" << expression;
 
     CommandReply reply = _run(cmd);
-    if (reply.has_error() > 0)
-        throw SRRuntimeException("CONFIG GET command failed");
+    _report_reply_errors(reply, "CONFIG GET command failed");
 
     // parse reply
     size_t n_dims = reply.n_elements();
     std::unordered_map<std::string,std::string> reply_map;
     for(size_t i = 0; i < n_dims; i += 2){
         reply_map[reply[i].str()] = reply[i+1].str();
     }
@@ -1450,31 +1435,29 @@
 
     AddressAtCommand cmd;
     SRAddress db_address(address);
     cmd.set_exec_address(db_address);
     cmd << "CONFIG" << "SET" << config_param << value;
 
     CommandReply reply = _run(cmd);
-    if (reply.has_error() > 0)
-        throw SRRuntimeException("CONFIG SET command failed");
+    _report_reply_errors(reply, "CONFIG SET command failed");
 }
 
 void Client::save(const std::string address)
 {
     // Track calls to this API function
     LOG_API_FUNCTION();
 
     AddressAtCommand cmd;
     SRAddress db_address(address);
     cmd.set_exec_address(db_address);
     cmd << "SAVE";
 
     CommandReply reply = _run(cmd);
-    if (reply.has_error() > 0)
-        throw SRRuntimeException("SAVE command failed");
+    _report_reply_errors(reply, "SAVE command failed");
 }
 
 // Append dataset to aggregation list
 void Client::append_to_list(const std::string& list_name,
                             const DataSet& dataset)
 {
     // Track calls to this API function
@@ -1488,17 +1471,16 @@
 
     // Build the command
     SingleKeyCommand cmd;
     cmd << "RPUSH" << Keyfield(list_key) << dataset_key;
 
     // Run the command
     CommandReply reply = _run(cmd);
-    if (reply.has_error() > 0)
-        throw SRRuntimeException("RPUSH command failed. DataSet could not "\
-                                 "be added to the aggregation list.");
+    _report_reply_errors(reply, "RPUSH command failed. DataSet could not "\
+                                "be added to the aggregation list.");
 }
 
 // Delete an aggregation list
 void Client::delete_list(const std::string& list_name)
 {
     // Track calls to this API function
     LOG_API_FUNCTION();
@@ -1508,16 +1490,15 @@
 
     // Build the command
     SingleKeyCommand cmd;
     cmd << "DEL" << Keyfield(list_key);
 
     // Run the command
     CommandReply reply = _run(cmd);
-    if (reply.has_error() > 0)
-        throw SRRuntimeException("DEL command failed.");
+    _report_reply_errors(reply, "DEL command failed.");
 }
 
 // Copy aggregation list
 void Client::copy_list(const std::string& src_name,
                        const std::string& dest_name)
 {
     // Track calls to this API function
@@ -1549,17 +1530,16 @@
     cmd << std::to_string(0);
     cmd << std::to_string(-1);
 
     // Run the command to retrive the list contents
     CommandReply reply = _run(cmd);
 
     // Check for reply errors and correct type
-    if (reply.has_error() > 0)
-        throw SRRuntimeException("GET command failed. The aggregation "\
-                                 "list could not be retrieved.");
+    _report_reply_errors(reply, "GET command failed. The aggregation "\
+                                "list could not be retrieved.");
 
     if (reply.redis_reply_type() != "REDIS_REPLY_ARRAY")
         throw SRRuntimeException("An unexpected type was returned for "
                                  "for the aggregation list.");
 
     if (reply.n_elements() == 0)
         throw SRRuntimeException("The source aggregation list does "\
@@ -1597,17 +1577,16 @@
         }
 
         copy_cmd.add_field_ptr(reply[i].str(), reply[i].str_len());
     }
 
     CommandReply copy_reply = _run(copy_cmd);
 
-    if (reply.has_error() > 0)
-        throw SRRuntimeException("Dataset aggregation list copy "
-                                 "operation failed.");
+    _report_reply_errors(reply, "Dataset aggregation list copy "
+                                "operation failed.");
 }
 
 // Rename an aggregation list
 void Client::rename_list(const std::string& src_name,
                          const std::string& dest_name)
 {
     // Track calls to this API function
@@ -1644,17 +1623,16 @@
     SingleKeyCommand cmd;
     cmd << "LLEN" << Keyfield(list_key);
 
     // Run the command
     CommandReply reply = _run(cmd);
 
     // Check for errors and return value
-    if (reply.has_error() > 0)
-        throw SRRuntimeException("LLEN command failed. The list "\
-                                 "length could not be retrieved.");
+    _report_reply_errors(reply, "LLEN command failed. The list "\
+                                "length could not be retrieved.");
 
     if (reply.redis_reply_type() != "REDIS_REPLY_INTEGER")
         throw SRRuntimeException("An unexpected type was returned for "
                                  "for list length.");
 
     int list_length = reply.integer();
 
@@ -1858,17 +1836,16 @@
     cmd << std::to_string(start_index);
     cmd << std::to_string(end_index);
 
     // Run the command to retrive the list
     CommandReply reply = _run(cmd);
 
     // Check for reply errors and correct type
-    if (reply.has_error() > 0)
-        throw SRRuntimeException("GET command failed. The aggregation "\
-                                 "list could not be retrieved.");
+    _report_reply_errors(reply, "GET command failed. The aggregation "\
+                                "list could not be retrieved.");
 
     if (reply.redis_reply_type() != "REDIS_REPLY_ARRAY")
         throw SRRuntimeException("An unexpected type was returned for "
                                  "for the aggregation list.");
 
     // Create CommandList for retrieving all metadata values in pipeline
     CommandList metadata_cmd_list;
@@ -1911,18 +1888,16 @@
 
     for (size_t i = 0; i < metadata_replies.size(); i++) {
 
         // Shallow copy of the underlying PipelineReply entry
         CommandReply metadata_reply = metadata_replies[i];
 
         // Check if metadata_reply has any errors
-        if (metadata_reply.has_error() > 0) {
-            throw SRRuntimeException("An error was encountered in "\
-                                        "metdata retrieval.");
-        }
+        _report_reply_errors(metadata_reply, "An error was encountered in "\
+                                             "metdata retrieval.");
 
         std::string dataset_key =
             std::string(reply[i].str(), reply[i].str_len());
         std::string dataset_name =
             _get_dataset_name_from_list_entry(dataset_key);
 
         // Unpack the dataset to get tensor names
@@ -2154,16 +2129,15 @@
 // TensorBase object has been dynamically allocated, but not yet tracked
 // for memory management in any object.
 TensorBase* Client::_get_tensorbase_obj(const std::string& name)
 {
     // Fetch the tensor
     std::string get_key = _build_tensor_key(name, true);
     CommandReply reply = _redis_server->get_tensor(get_key);
-    if (reply.has_error())
-        throw SRRuntimeException("tensor retrieval failed");
+    _report_reply_errors(reply, "tensor retrieval failed");
 
     std::vector<size_t> dims = GetTensorCommand::get_dims(reply);
     if (dims.size() <= 0)
         throw SRRuntimeException("The number of dimensions of the "\
                                  "fetched tensor are invalid: " +
                                  std::to_string(dims.size()));
 
@@ -2289,16 +2263,15 @@
     // Build the command
     AddressAnyCommand cmd;
     cmd << "AI.CONFIG" << "MODEL_CHUNK_SIZE" << std::to_string(chunk_size);
     std::cout << cmd.to_string() << std::endl;
 
     // Run it
     CommandReply reply = _run(cmd);
-    if (reply.has_error() > 0)
-        throw SRRuntimeException("AI.CONFIG MODEL_CHUNK_SIZE command failed");
+    _report_reply_errors(reply, "AI.CONFIG MODEL_CHUNK_SIZE command failed");
 
     // Remember the new chunk size
     _redis_server->store_model_chunk_size(chunk_size);
 }
 
 // Create a string representation of the client
 std::string Client::to_string() const
@@ -2307,7 +2280,24 @@
     LOG_API_FUNCTION();
 
     std::string result;
     result = "Client (" + _lname + "):\n";
     result += _redis_server->to_string();
     return result;
 }
+
+// Raise an exception containing available error messages
+void Client::_report_reply_errors(CommandReply &reply, std::string error_message)
+{
+    if (!reply.has_error())
+        return;
+
+    std::vector<std::string> errors = reply.get_reply_errors();
+    std::string combined_error = error_message + " ";
+    for (size_t i = 0; i < errors.size(); i++)
+    {
+        combined_error += errors.at(i);
+        if (i < errors.size() - 1)
+            combined_error += ":";
+    }
+    throw SRRuntimeException(combined_error);
+}
```

### Comparing `smartredis-0.5.2/src/cpp/clusterinfocommand.cpp` & `smartredis-0.5.3/src/cpp/clusterinfocommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/command.cpp` & `smartredis-0.5.3/src/cpp/command.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/commandlist.cpp` & `smartredis-0.5.3/src/cpp/commandlist.cpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -113,8 +113,8 @@
     return _commands.cend();
 }
 
 // Returns the number of elements
 size_t CommandList::size()
 {
     return _commands.size();
-}
+}
```

### Comparing `smartredis-0.5.2/src/cpp/commandreply.cpp` & `smartredis-0.5.3/src/cpp/commandreply.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/compoundcommand.cpp` & `smartredis-0.5.3/src/cpp/compoundcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/configoptions.cpp` & `smartredis-0.5.3/src/cpp/configoptions.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/dataset.cpp` & `smartredis-0.5.3/src/cpp/dataset.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
                             const SRTensorType type,
                             SRMemoryLayout mem_layout)
 {
     // Track calls to this API function
     LOG_API_FUNCTION();
 
     _enforce_tensor_exists(name);
+    _enforce_tensor_type(name, type);
     _tensorpack.get_tensor(name)->fill_mem_space(data, dims, mem_layout);
 }
 
 // Get the metadata scalar field values from the DataSet. The data pointer
 // reference will be pointed to newly allocated memory that will contain all
 // values in the metadata field. The length variable will be set to the number
 // of entries in the allocated memory space to allow for iteration over the values.
@@ -374,14 +375,30 @@
     if (!_tensorpack.tensor_exists(tensorname)) {
         throw SRKeyException("The tensor \"" + std::string(tensorname) +
                              "\" does not exist in dataset \"" +
                              _dsname + "\".");
     }
 }
 
+// Check that the provided tensor type matches the internal tensor type
+inline void DataSet::_enforce_tensor_type(const std::string& tensorname,
+                                          const SRTensorType& type) const
+{
+    _enforce_tensor_exists(tensorname);
+
+    SRTensorType known_type = _tensorpack.get_tensor(tensorname)->type();
+
+    if (known_type != type) {
+        throw SRRuntimeException("The tensor \"" + std::string(tensorname) +
+                                 "\" has type \"" + TENSOR_STR_MAP.at(known_type) +
+                                 "\" in dataset \"" + _dsname + "\" but the provided " +
+                                 "type is " "\"" + TENSOR_STR_MAP.at(type) + "\".");
+    }
+}
+
 // Retrieve the tensor from the DataSet and return a TensorBase object that
 // can be used to return tensor information to the user. The returned TensorBase
 // object has been dynamically allocated, but not yet tracked for memory
 // management in any object.
 TensorBase* DataSet::_get_tensorbase_obj(const std::string& name) const
 {
     _enforce_tensor_exists(name);
```

### Comparing `smartredis-0.5.2/src/cpp/dbinfocommand.cpp` & `smartredis-0.5.3/src/cpp/dbinfocommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/dbnode.cpp` & `smartredis-0.5.3/src/cpp/dbnode.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/gettensorcommand.cpp` & `smartredis-0.5.3/src/cpp/gettensorcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/keyedcommand.cpp` & `smartredis-0.5.3/src/cpp/keyedcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/logger.cpp` & `smartredis-0.5.3/src/cpp/logger.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/metadata.cpp` & `smartredis-0.5.3/src/cpp/metadata.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/metadatafield.cpp` & `smartredis-0.5.3/src/cpp/metadatafield.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/multikeycommand.cpp` & `smartredis-0.5.3/src/cpp/multikeycommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/nonkeyedcommand.cpp` & `smartredis-0.5.3/src/cpp/nonkeyedcommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/pipelinereply.cpp` & `smartredis-0.5.3/src/cpp/pipelinereply.cpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -106,8 +106,8 @@
     _queued_replies.push_back(std::forward<QueuedReplies>(reply));
 
     // Add redisReply contained in the QueuedReplies into the inventory
     size_t n_replies = _queued_replies.back().size();
     for (size_t i = 0; i < n_replies; i++) {
         _all_replies.push_back(&(_queued_replies.back().get(i)));
     }
-}
+}
```

### Comparing `smartredis-0.5.2/src/cpp/redis.cpp` & `smartredis-0.5.3/src/cpp/redis.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -732,15 +732,15 @@
         connectOpts.type = sw::redis::ConnectionType::TCP;
     }
     else {
         connectOpts.path = db_address._uds_file;
         connectOpts.type = sw::redis::ConnectionType::UNIX;
     }
     connectOpts.socket_timeout = std::chrono::milliseconds(
-        _DEFAULT_SOCKET_TIMEOUT);
+        _socket_timeout);
 
     // Connect
     for (int i = 1; i <= _connection_attempts; i++) {
         try {
             // Try to create the sw::redis::Redis object
             _redis = new sw::redis::Redis(connectOpts);
```

### Comparing `smartredis-0.5.2/src/cpp/rediscluster.cpp` & `smartredis-0.5.3/src/cpp/rediscluster.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,19 @@
     // Keep track of CommandList index order of execution (ooe)
     std::vector<size_t> cmd_list_index_ooe;
     cmd_list_index_ooe.reserve(cmd_list.size());
 
     volatile size_t pipeline_completion_count = 0;
     size_t num_shards = shard_cmd_index_list.size();
     Exception error_response = Exception("no error");
-    bool success_status[num_shards];
+
+    bool* success_status = new bool[num_shards];
+    for (size_t s = 0; s < num_shards; s++) {
+        success_status[s] = false;
+    }
     std::mutex results_mutex;
 
     // Loop over all shards and execute pipelines
     for (size_t s = 0; s < num_shards; s++) {
         // Get shard prefix
         std::string shard_prefix = _db_nodes[s].prefix;
 
@@ -306,14 +310,15 @@
         }
     }
 
     // Reorder the command replies in all_replies to align
     // with order of execution
     all_replies.reorder(cmd_list_index_ooe);
 
+    delete[] success_status;
     return all_replies;
 }
 
 // Check if a model or script key exists in the database
 bool RedisCluster::model_key_exists(const std::string& key)
 {
     // Add model prefix to the key
@@ -1085,15 +1090,15 @@
         connectOpts.type = sw::redis::ConnectionType::TCP;
     }
     else {
         throw SRInternalException(
             "RedisCluster encountered a UDS request in _connect()");
     }
     connectOpts.socket_timeout = std::chrono::milliseconds(
-        _DEFAULT_SOCKET_TIMEOUT);
+        _socket_timeout);
 
     // Connect
     std::string msg;
     for (int i = 1; i <= _connection_attempts; i++) {
         msg = "Connection attempt " + std::to_string(i) + " of " +
             std::to_string(_connection_attempts);
         _cfgopts->_get_log_context()->log_data(LLDeveloper, msg);
@@ -1406,22 +1411,21 @@
     cmd << "DEL";
     cmd.add_keys(keys);
 
     // Run it, ignoring failure
     (void)run(cmd);
 }
 
-// Retrieve the optimum model prefix for the set of inputs
-DBNode* RedisCluster::_get_model_script_db(const std::string& name,
-                                           std::vector<std::string>& inputs,
+// Retrieve the optimum db node for model and script execution
+DBNode* RedisCluster::_get_model_script_db(std::vector<std::string>& inputs,
                                            std::vector<std::string>& outputs)
 {
-    /* This function calculates the optimal model name to use
-    to run the provided inputs.  If a cluster is not being used,
-    the model name is returned, else a prefixed model name is returned.
+    /* This function determines which db node in the cluster
+    contains the most input and output tensors and
+    returns a pointer to that db node.
     */
 
     // TODO we should randomly choose the max if there are multiple maxes
 
     std::vector<int> hash_slot_tally(_db_nodes.size(), 0);
 
     for (size_t i = 0; i < inputs.size(); i++) {
@@ -1548,7 +1552,9 @@
 // Create a string representation of the Redis connection
 std::string RedisCluster::to_string() const
 {
     std::string result("Clustered Redis connection:\n");
     result += RedisServer::to_string();
     return result;
 }
+
+
```

### Comparing `smartredis-0.5.2/src/cpp/redisserver.cpp` & `smartredis-0.5.3/src/cpp/redisserver.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 {
     _connection_timeout = _cfgopts->_resolve_integer_option(
         _CONN_TIMEOUT_ENV_VAR, _DEFAULT_CONN_TIMEOUT);
     _connection_interval = _cfgopts->_resolve_integer_option(
         _CONN_INTERVAL_ENV_VAR, _DEFAULT_CONN_INTERVAL);
     _command_timeout = _cfgopts->_resolve_integer_option(
         _CMD_TIMEOUT_ENV_VAR, _DEFAULT_CMD_TIMEOUT);
+    _socket_timeout = _cfgopts->_resolve_integer_option(
+        _SOCKET_TIMEOUT_ENV_VAR, _DEFAULT_SOCKET_TIMEOUT);
     _command_interval = _cfgopts->_resolve_integer_option(
         _CMD_INTERVAL_ENV_VAR, _DEFAULT_CMD_INTERVAL);
     _thread_count = _cfgopts->_resolve_integer_option(
         _TP_THREAD_COUNT, _DEFAULT_THREAD_COUNT);
 
     _check_runtime_variables();
 
@@ -163,14 +165,19 @@
 
     if (_command_timeout > (INT_MAX / 1000)) {
         throw SRParameterException(_CMD_TIMEOUT_ENV_VAR + " " +
                                    std::to_string(_command_timeout) +
                                    " must be less than "
                                    + std::to_string(INT_MAX / 1000));
     }
+
+    if (_socket_timeout <= 0) {
+        throw SRParameterException(_SOCKET_TIMEOUT_ENV_VAR +
+                                   " must be greater than 0.");
+    }
 }
 
 // Create a string representation of the Redis connection
 std::string RedisServer::to_string() const
 {
     std::string result;
 
@@ -197,13 +204,15 @@
     result += "  Connection parameters:\n";
     result += "    Retry attempts: "
            + std::to_string(_connection_attempts) + "\n";
     result += "    Retry interval (ms): "
            + std::to_string(_connection_interval) + "\n";
     result += "    Attempt timeout (ms): "
            + std::to_string(_connection_timeout) + "\n";
+    result += "    Socket timeout (ms): "
+           + std::to_string(_socket_timeout) + "\n";
 
     // Threadpool
     result += "  Threadpool: " + std::to_string(_thread_count) + " threads\n";
 
     return result;
 }
```

### Comparing `smartredis-0.5.2/src/cpp/singlekeycommand.cpp` & `smartredis-0.5.3/src/cpp/singlekeycommand.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/srobject.cpp` & `smartredis-0.5.3/src/cpp/srobject.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/stringfield.cpp` & `smartredis-0.5.3/src/cpp/stringfield.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/tensorbase.cpp` & `smartredis-0.5.3/src/cpp/tensorbase.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 
 using namespace SmartRedis;
 
 // TensorBase constructor
 TensorBase::TensorBase(const std::string& name,
                        const void* data,
                        const std::vector<size_t>& dims,
-                       const SRTensorType type,
-                       const SRMemoryLayout mem_layout)
+                       const SRTensorType type)
 {
     /* The TensorBase constructor makes a copy of the
     name, type, and dims associated with the tensor.
     The provided data is copied into a memory space
     owned by the tensor.
     */
```

### Comparing `smartredis-0.5.2/src/cpp/tensorpack.cpp` & `smartredis-0.5.3/src/cpp/tensorpack.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/cpp/threadpool.cpp` & `smartredis-0.5.3/src/cpp/threadpool.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     : _context(context)
 {
     // Flags that we're initializing and not shutting down
     initialization_complete = false;
     shutting_down = false;
 
     // By default, we'll make one thread for each hardware context
-    if (num_threads == 0)
-        num_threads = std::thread::hardware_concurrency();
+    if (num_threads == 0) num_threads = std::thread::hardware_concurrency();
 
     // Create worker threads
 	if (num_threads < 1) num_threads = 1; // Force a minimum of 1 thread
     for (unsigned int i = 0; i < num_threads; i++) {
         _context->log_data(
             LLDeveloper, "Kicking off thread " + std::to_string(i));
         threads.push_back(std::thread(&ThreadPool::perform_jobs, this, i));
```

### Comparing `smartredis-0.5.2/src/cpp/utility.cpp` & `smartredis-0.5.3/src/cpp/utility.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client/aggregation_interfaces.inc` & `smartredis-0.5.3/src/fortran/client/aggregation_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client/client_dataset_interfaces.inc` & `smartredis-0.5.3/src/fortran/client/client_dataset_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client/client_interfaces.inc` & `smartredis-0.5.3/src/fortran/client/client_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client/ensemble_interfaces.inc` & `smartredis-0.5.3/src/fortran/client/ensemble_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client/misc_tensor_interfaces.inc` & `smartredis-0.5.3/src/fortran/client/misc_tensor_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client/model_interfaces.inc` & `smartredis-0.5.3/src/fortran/client/model_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client/put_tensor_interfaces.inc` & `smartredis-0.5.3/src/fortran/client/put_tensor_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client/put_tensor_methods_common.inc` & `smartredis-0.5.3/src/fortran/client/put_tensor_methods_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client/script_interfaces.inc` & `smartredis-0.5.3/src/fortran/client/script_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client/unpack_tensor_interfaces.inc` & `smartredis-0.5.3/src/fortran/client/unpack_tensor_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client/unpack_tensor_methods_common.inc` & `smartredis-0.5.3/src/fortran/client/unpack_tensor_methods_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/client.F90` & `smartredis-0.5.3/src/fortran/client.F90`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/configoptions/configoptions_interfaces.inc` & `smartredis-0.5.3/src/fortran/configoptions/configoptions_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/configoptions.F90` & `smartredis-0.5.3/src/fortran/configoptions.F90`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/dataset/add_meta_scalar_common.inc` & `smartredis-0.5.3/src/fortran/dataset/add_meta_scalar_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/dataset/add_tensor_methods_common.inc` & `smartredis-0.5.3/src/fortran/dataset/add_tensor_methods_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/dataset/dataset_interfaces.inc` & `smartredis-0.5.3/src/fortran/dataset/dataset_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/dataset/get_meta_scalars_common.inc` & `smartredis-0.5.3/src/fortran/dataset/get_meta_scalars_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/dataset/metadata_interfaces.inc` & `smartredis-0.5.3/src/fortran/dataset/metadata_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/dataset/tensor_interfaces.inc` & `smartredis-0.5.3/src/fortran/dataset/tensor_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc` & `smartredis-0.5.3/src/fortran/dataset/unpack_dataset_tensor_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc` & `smartredis-0.5.3/src/fortran/dataset/unpack_dataset_tensor_methods_common.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/dataset.F90` & `smartredis-0.5.3/src/fortran/dataset.F90`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/errors/errors_interfaces.inc` & `smartredis-0.5.3/src/fortran/errors/errors_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/errors.F90` & `smartredis-0.5.3/src/fortran/errors.F90`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/fortran_c_interop.F90` & `smartredis-0.5.3/src/fortran/fortran_c_interop.F90`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/logcontext/logcontext_interfaces.inc` & `smartredis-0.5.3/src/fortran/logcontext/logcontext_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/logcontext.F90` & `smartredis-0.5.3/src/fortran/logcontext.F90`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/logger/logger_interfaces.inc` & `smartredis-0.5.3/src/fortran/logger/logger_interfaces.inc`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/fortran/logger.F90` & `smartredis-0.5.3/src/fortran/logger.F90`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/bindings/bind.cpp` & `smartredis-0.5.3/src/python/bindings/bind.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/module/smartredis/__init__.py` & `smartredis-0.5.3/src/python/module/smartredis/__init__.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/module/smartredis/client.py` & `smartredis-0.5.3/src/python/module/smartredis/client.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/module/smartredis/configoptions.py` & `smartredis-0.5.3/src/python/module/smartredis/configoptions.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/module/smartredis/dataset.py` & `smartredis-0.5.3/src/python/module/smartredis/dataset.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/module/smartredis/dataset_utils.py` & `smartredis-0.5.3/src/python/module/smartredis/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/module/smartredis/error.py` & `smartredis-0.5.3/src/python/module/smartredis/error.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/module/smartredis/logcontext.py` & `smartredis-0.5.3/src/python/module/smartredis/logcontext.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/module/smartredis/logger.py` & `smartredis-0.5.3/src/python/module/smartredis/logger.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/module/smartredis/srobject.py` & `smartredis-0.5.3/src/python/module/smartredis/srobject.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/module/smartredis/util.py` & `smartredis-0.5.3/src/python/module/smartredis/util.py`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/module/smartredis.egg-info/SOURCES.txt` & `smartredis-0.5.3/src/python/module/smartredis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 CMakeLists.txt
 LICENSE.md
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
-requirements.txt
 setup.cfg
 setup.py
 smartredis_defs.cmake
 include/address.h
 include/addressallcommand.h
 include/addressanycommand.h
 include/addressatcommand.h
```

### Comparing `smartredis-0.5.2/src/python/src/pyclient.cpp` & `smartredis-0.5.3/src/python/src/pyclient.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/src/pyconfigoptions.cpp` & `smartredis-0.5.3/src/python/src/pyconfigoptions.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/src/pydataset.cpp` & `smartredis-0.5.3/src/python/src/pydataset.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/src/pylogcontext.cpp` & `smartredis-0.5.3/src/python/src/pylogcontext.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/src/python/src/pysrobject.cpp` & `smartredis-0.5.3/src/python/src/pysrobject.cpp`

 * *Files identical despite different names*

### Comparing `smartredis-0.5.2/utils/launch_redis.py` & `smartredis-0.5.3/utils/launch_redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,16 @@
                 command_succeeded = True
                 break
             except Exception:
                 # That try failed, so just retry
                 sleep(5)
         if not command_succeeded:
             raise RuntimeError(f"Failed to validate availability for connection {connection}")
+    # add a small sleep after completing availability test to let cluster complete setup
+    sleep(1)
 
 def stop_db(n_nodes, port, udsport):
     """Stop a redis cluster and clear the files
     associated with it
     """
     is_uds = udsport is not None
     if is_uds:
@@ -201,18 +203,19 @@
         _ = proc.communicate(timeout=15)
         if proc.returncode != 0:
             raise RuntimeError("Failed to launch Redis server!")
 
     # Create cluster for clustered Redis request
     if n_nodes > 1:
         cluster_str = " ".join(f"127.0.0.1:{port + i}" for i in range(n_nodes))
-        cmd = f"{rediscli} --cluster create {cluster_str} --cluster-replicas 0"
+        cmd = f"{rediscli} --cluster create {cluster_str} --cluster-replicas 0 --cluster-yes"
         print(cmd)
-        proc = run(cmd.split(), input="yes", encoding="utf-8", shell=False)
+        proc = run(cmd.split(), encoding="utf-8", shell=False)
         if proc.returncode != 0:
+            print(f'{rediscli} returncode: {proc.returncode}')
             raise SubprocessError("Cluster could not be created!")
         sleep(2)
         print("Cluster has been setup!")
     else:
         print("Server has been setup!")
     check_availability(n_nodes, port, udsport)
```

