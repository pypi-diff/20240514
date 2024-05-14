# Comparing `tmp/thriftpy2-0.5.0.tar.gz` & `tmp/thriftpy2-0.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thriftpy2-0.5.0.tar", last modified: Tue May  7 11:57:01 2024, max compression
+gzip compressed data, was "thriftpy2-0.5.1rc1.tar", last modified: Tue May 14 13:17:04 2024, max compression
```

## Comparing `thriftpy2-0.5.0.tar` & `thriftpy2-0.5.1rc1.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.738722 thriftpy2-0.5.0/
--rw-r--r--   0 asaka      (501) staff       (20)    20403 2024-05-07 11:56:25.000000 thriftpy2-0.5.0/CHANGES.rst
--rw-r--r--   0 asaka      (501) staff       (20)     1081 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/LICENSE
--rw-r--r--   0 asaka      (501) staff       (20)      228 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/MANIFEST.in
--rw-r--r--   0 asaka      (501) staff       (20)     6909 2024-05-07 11:57:01.738327 thriftpy2-0.5.0/PKG-INFO
--rw-r--r--   0 asaka      (501) staff       (20)     5164 2024-02-29 11:36:31.000000 thriftpy2-0.5.0/README.rst
--rw-r--r--   0 asaka      (501) staff       (20)       62 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/pyproject.toml
--rw-r--r--   0 asaka      (501) staff       (20)      313 2024-05-07 11:57:01.739833 thriftpy2-0.5.0/setup.cfg
--rw-r--r--   0 asaka      (501) staff       (20)     3997 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/setup.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.547853 thriftpy2-0.5.0/tests/
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.585432 thriftpy2-0.5.0/tests/__pycache__/
--rw-r--r--   0 asaka      (501) staff       (20)     7417 2024-02-25 10:17:45.000000 thriftpy2-0.5.0/tests/__pycache__/addressbook.cpython-312.pyc
--rw-r--r--   0 asaka      (501) staff       (20)      459 2024-02-25 10:32:40.000000 thriftpy2-0.5.0/tests/__pycache__/conftest.cpython-312-pytest-6.2.5.pyc
--rw-r--r--   0 asaka      (501) staff       (20)      459 2024-02-25 10:34:10.000000 thriftpy2-0.5.0/tests/__pycache__/conftest.cpython-312-pytest-7.4.4.pyc
--rw-r--r--   0 asaka      (501) staff       (20)      459 2024-02-25 10:17:44.000000 thriftpy2-0.5.0/tests/__pycache__/conftest.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)      884 2024-02-25 10:17:45.000000 thriftpy2-0.5.0/tests/__pycache__/container.cpython-312.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    25692 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/storm.cpython-312.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    29360 2024-02-25 10:19:38.000000 thriftpy2-0.5.0/tests/__pycache__/test_aio.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     2127 2024-02-25 10:19:38.000000 thriftpy2-0.5.0/tests/__pycache__/test_aio_protocol_binary.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     1892 2024-02-25 10:19:38.000000 thriftpy2-0.5.0/tests/__pycache__/test_aio_protocol_compact.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    19687 2024-02-25 10:19:38.000000 thriftpy2-0.5.0/tests/__pycache__/test_all_protocols_binary_field.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    10464 2024-02-25 10:19:38.000000 thriftpy2-0.5.0/tests/__pycache__/test_apache_json.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    13313 2024-02-25 10:19:38.000000 thriftpy2-0.5.0/tests/__pycache__/test_base.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     6450 2024-02-25 10:19:38.000000 thriftpy2-0.5.0/tests/__pycache__/test_buffered_transport.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    10348 2024-02-25 10:19:38.000000 thriftpy2-0.5.0/tests/__pycache__/test_const.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     5366 2024-02-25 10:19:38.000000 thriftpy2-0.5.0/tests/__pycache__/test_container.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     8526 2024-02-25 10:19:38.000000 thriftpy2-0.5.0/tests/__pycache__/test_cytransport.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     9632 2024-02-25 10:19:38.000000 thriftpy2-0.5.0/tests/__pycache__/test_framed_transport.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     9361 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_hook.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    28293 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_http.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    11913 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_json_protocol.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    18427 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_loader.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     8608 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_memory_transport.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     5725 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_multiplexed.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     3727 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_oneway.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    94489 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_parser.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    39707 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_protocol_binary.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    48118 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_protocol_compact.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    62002 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_protocol_cybinary.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     3151 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_recursive_definition.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    31080 2024-02-25 10:32:40.000000 thriftpy2-0.5.0/tests/__pycache__/test_rpc.cpython-312-pytest-6.2.5.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    31575 2024-02-25 10:38:02.000000 thriftpy2-0.5.0/tests/__pycache__/test_rpc.cpython-312-pytest-7.4.4.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    31376 2024-02-25 10:17:44.000000 thriftpy2-0.5.0/tests/__pycache__/test_rpc.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    23616 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_socket.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     4816 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_sslsocket.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    16210 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_tornado.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    57520 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_tracking.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     1514 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_type.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     8815 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/__pycache__/test_type_mismatch.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     4231 2023-12-05 14:37:54.000000 thriftpy2-0.5.0/tests/addressbook.py
--rw-r--r--   0 asaka      (501) staff       (20)     1118 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/addressbook.thrift
--rw-r--r--   0 asaka      (501) staff       (20)     1122 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/apache_json_test.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      250 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/base.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      489 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/bin_test.thrift
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.586151 thriftpy2-0.5.0/tests/compatible/
--rw-r--r--   0 asaka      (501) staff       (20)        0 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/compatible/__init__.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.586575 thriftpy2-0.5.0/tests/compatible/__pycache__/
--rw-r--r--   0 asaka      (501) staff       (20)      154 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/compatible/__pycache__/__init__.cpython-312.pyc
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.588495 thriftpy2-0.5.0/tests/compatible/version_2/
--rw-r--r--   0 asaka      (501) staff       (20)        0 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/compatible/version_2/__init__.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.590212 thriftpy2-0.5.0/tests/compatible/version_2/__pycache__/
--rw-r--r--   0 asaka      (501) staff       (20)      164 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/compatible/version_2/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 asaka      (501) staff       (20)    15876 2024-02-25 10:19:39.000000 thriftpy2-0.5.0/tests/compatible/version_2/__pycache__/tracking.cpython-312.pyc
--rw-r--r--   0 asaka      (501) staff       (20)     8708 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/compatible/version_2/tracking.py
--rw-r--r--   0 asaka      (501) staff       (20)      307 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/compatible/version_2/tracking.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       30 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/conftest.py
--rw-r--r--   0 asaka      (501) staff       (20)      724 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/const.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      461 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/container.py
--rw-r--r--   0 asaka      (501) staff       (20)      889 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/container.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      103 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/multiplexed.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       53 2023-11-14 10:33:35.000000 thriftpy2-0.5.0/tests/oneway.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      255 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parent.thrift
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.625028 thriftpy2-0.5.0/tests/parser-cases/
--rw-r--r--   0 asaka      (501) staff       (20)     1694 2024-02-25 09:41:43.000000 thriftpy2-0.5.0/tests/parser-cases/annotations.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       82 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/comments.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      870 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/parser-cases/constants.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       30 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/cpp_include.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      228 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/parser-cases/doubles.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       34 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_dead_include_0.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       34 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_dead_include_1.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       34 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_dead_include_2.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       34 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_dead_include_3.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       81 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/parser-cases/e_duplicate_exception.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       55 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_duplicate_field_id.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       55 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_duplicate_field_name.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       74 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/parser-cases/e_duplicate_function.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       93 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/parser-cases/e_duplicate_service.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       74 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/parser-cases/e_duplicate_struct.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       47 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_grammer_error_at_eof.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       81 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_service_extends_0.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      263 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_structs_0.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      117 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_structs_1.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       23 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_type_error_0.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       65 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_type_error_1.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      104 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_type_error_2.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       20 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_use_thrift_reserved_keywords.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       21 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_value_ref_0.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       77 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_value_ref_1.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       75 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/e_value_ref_2.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      179 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/enums.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       74 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/include.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       22 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/included.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       33 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/parser-cases/issue_121.include.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       80 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/parser-cases/issue_121.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       97 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/issue_215.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      181 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/issue_252.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      156 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/parser-cases/nest_incomplete_type.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      213 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/recursive_union.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      395 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/service.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       97 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/service_extends.thrift
--rw-r--r--   0 asaka      (501) staff       (20)     1215 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/shared.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      482 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/parser-cases/structs.thrift
--rw-r--r--   0 asaka      (501) staff       (20)     4870 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/tutorial.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      224 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/type_ref.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      190 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/type_ref_shared.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      184 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/value_ref.thrift
--rw-r--r--   0 asaka      (501) staff       (20)       84 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/parser-cases/value_ref_shared.thrift
--rw-r--r--   0 asaka      (501) staff       (20)      228 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/recursive_definition.thrift
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.637308 thriftpy2-0.5.0/tests/ssl/
--rw-r--r--   0 asaka      (501) staff       (20)     8141 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/CA.pem
--rw-r--r--   0 asaka      (501) staff       (20)     3096 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/README.md
--rw-r--r--   0 asaka      (501) staff       (20)     1740 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/client.crt
--rw-r--r--   0 asaka      (501) staff       (20)     1679 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/client.key
--rw-r--r--   0 asaka      (501) staff       (20)     2845 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/client.p12
--rw-r--r--   0 asaka      (501) staff       (20)     4125 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/client.pem
--rw-r--r--   0 asaka      (501) staff       (20)     1870 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/client_v3.crt
--rw-r--r--   0 asaka      (501) staff       (20)     1679 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/client_v3.key
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.639331 thriftpy2-0.5.0/tests/ssl/keygen/
--rw-r--r--   0 asaka      (501) staff       (20)       42 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/keygen/.gitignore
--rw-r--r--   0 asaka      (501) staff       (20)     4080 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/keygen/make-serverkey.sh
--rw-r--r--   0 asaka      (501) staff       (20)     2390 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/server.crt
--rw-r--r--   0 asaka      (501) staff       (20)     3268 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/server.key
--rw-r--r--   0 asaka      (501) staff       (20)     4477 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/server.p12
--rw-r--r--   0 asaka      (501) staff       (20)     5658 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/tests/ssl/server.pem
--rw-r--r--   0 asaka      (501) staff       (20)    15265 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/storm.py
--rw-r--r--   0 asaka      (501) staff       (20)     8669 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/storm.thrift
--rw-r--r--   0 asaka      (501) staff       (20)    11872 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_aio.py
--rw-r--r--   0 asaka      (501) staff       (20)      900 2023-12-05 14:37:59.000000 thriftpy2-0.5.0/tests/test_aio_protocol_binary.py
--rw-r--r--   0 asaka      (501) staff       (20)      838 2023-12-05 14:37:59.000000 thriftpy2-0.5.0/tests/test_aio_protocol_compact.py
--rw-r--r--   0 asaka      (501) staff       (20)     9874 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_all_protocols_binary_field.py
--rw-r--r--   0 asaka      (501) staff       (20)     5988 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_apache_json.py
--rw-r--r--   0 asaka      (501) staff       (20)     1989 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/test_base.py
--rw-r--r--   0 asaka      (501) staff       (20)     3040 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_buffered_transport.py
--rw-r--r--   0 asaka      (501) staff       (20)      975 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/test_const.py
--rw-r--r--   0 asaka      (501) staff       (20)     1354 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/test_container.py
--rw-r--r--   0 asaka      (501) staff       (20)     1377 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_cytransport.py
--rw-r--r--   0 asaka      (501) staff       (20)     4291 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_framed_transport.py
--rw-r--r--   0 asaka      (501) staff       (20)     2219 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_hook.py
--rw-r--r--   0 asaka      (501) staff       (20)     7382 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_http.py
--rw-r--r--   0 asaka      (501) staff       (20)     2531 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_json_protocol.py
--rw-r--r--   0 asaka      (501) staff       (20)     2128 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/test_loader.py
--rw-r--r--   0 asaka      (501) staff       (20)     1648 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/test_memory_transport.py
--rw-r--r--   0 asaka      (501) staff       (20)     2722 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_multiplexed.py
--rw-r--r--   0 asaka      (501) staff       (20)      942 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_oneway.py
--rw-r--r--   0 asaka      (501) staff       (20)    11738 2023-09-15 12:04:17.000000 thriftpy2-0.5.0/tests/test_parser.py
--rw-r--r--   0 asaka      (501) staff       (20)     7044 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_protocol_binary.py
--rw-r--r--   0 asaka      (501) staff       (20)     7979 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_protocol_compact.py
--rw-r--r--   0 asaka      (501) staff       (20)    12803 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_protocol_cybinary.py
--rw-r--r--   0 asaka      (501) staff       (20)      444 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/test_recursive_definition.py
--rw-r--r--   0 asaka      (501) staff       (20)     8911 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_rpc.py
--rw-r--r--   0 asaka      (501) staff       (20)     6854 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_socket.py
--rw-r--r--   0 asaka      (501) staff       (20)     3179 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_sslsocket.py
--rw-r--r--   0 asaka      (501) staff       (20)     5812 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_tornado.py
--rw-r--r--   0 asaka      (501) staff       (20)    15877 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/tests/test_tracking.py
--rw-r--r--   0 asaka      (501) staff       (20)      212 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/test_type.py
--rw-r--r--   0 asaka      (501) staff       (20)     3441 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/test_type_mismatch.py
--rw-r--r--   0 asaka      (501) staff       (20)       49 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/tests/type.thrift
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.648470 thriftpy2-0.5.0/thriftpy2/
--rw-r--r--   0 asaka      (501) staff       (20)      296 2024-05-07 11:56:25.000000 thriftpy2-0.5.0/thriftpy2/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)      312 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/_compat.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.653060 thriftpy2-0.5.0/thriftpy2/contrib/
--rw-r--r--   0 asaka      (501) staff       (20)        0 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/thriftpy2/contrib/__init__.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.656670 thriftpy2-0.5.0/thriftpy2/contrib/aio/
--rw-r--r--   0 asaka      (501) staff       (20)        0 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)     3008 2024-03-05 12:23:36.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/client.py
--rw-r--r--   0 asaka      (501) staff       (20)     2415 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/processor.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.659613 thriftpy2-0.5.0/thriftpy2/contrib/aio/protocol/
--rw-r--r--   0 asaka      (501) staff       (20)      414 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/protocol/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)      682 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/protocol/base.py
--rw-r--r--   0 asaka      (501) staff       (20)     8706 2023-12-05 14:37:59.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/protocol/binary.py
--rw-r--r--   0 asaka      (501) staff       (20)     9678 2023-12-05 14:37:59.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/protocol/compact.py
--rw-r--r--   0 asaka      (501) staff       (20)     3405 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/rpc.py
--rw-r--r--   0 asaka      (501) staff       (20)     1477 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/server.py
--rw-r--r--   0 asaka      (501) staff       (20)    13095 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/socket.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.674446 thriftpy2-0.5.0/thriftpy2/contrib/aio/transport/
--rw-r--r--   0 asaka      (501) staff       (20)      429 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/transport/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)     1048 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/transport/base.py
--rw-r--r--   0 asaka      (501) staff       (20)     1557 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/transport/buffered.py
--rw-r--r--   0 asaka      (501) staff       (20)     2048 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/contrib/aio/transport/framed.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.679072 thriftpy2-0.5.0/thriftpy2/contrib/tracking/
--rw-r--r--   0 asaka      (501) staff       (20)     7723 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/contrib/tracking/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)     3877 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/thriftpy2/contrib/tracking/tracker.py
--rw-r--r--   0 asaka      (501) staff       (20)      404 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/thriftpy2/contrib/tracking/tracking.thrift
--rw-r--r--   0 asaka      (501) staff       (20)     1247 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/hook.py
--rw-r--r--   0 asaka      (501) staff       (20)    12042 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/http.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.692338 thriftpy2-0.5.0/thriftpy2/parser/
--rw-r--r--   0 asaka      (501) staff       (20)     7885 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/parser/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)      625 2023-09-15 12:01:14.000000 thriftpy2-0.5.0/thriftpy2/parser/exc.py
--rw-r--r--   0 asaka      (501) staff       (20)     4165 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/parser/lexer.py
--rw-r--r--   0 asaka      (501) staff       (20)    26511 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/parser/parser.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.699758 thriftpy2-0.5.0/thriftpy2/protocol/
--rw-r--r--   0 asaka      (501) staff       (20)     1271 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/protocol/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)    12209 2023-11-14 08:47:51.000000 thriftpy2-0.5.0/thriftpy2/protocol/apache_json.py
--rw-r--r--   0 asaka      (501) staff       (20)      696 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/protocol/base.py
--rw-r--r--   0 asaka      (501) staff       (20)    11803 2023-12-05 14:37:59.000000 thriftpy2-0.5.0/thriftpy2/protocol/binary.py
--rw-r--r--   0 asaka      (501) staff       (20)    16965 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/protocol/compact.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.703333 thriftpy2-0.5.0/thriftpy2/protocol/cybin/
--rw-r--r--   0 asaka      (501) staff       (20)   860411 2024-05-07 11:57:01.000000 thriftpy2-0.5.0/thriftpy2/protocol/cybin/cybin.c
--rw-r--r--   0 asaka      (501) staff       (20)    13965 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/protocol/cybin/cybin.pyx
--rw-r--r--   0 asaka      (501) staff       (20)     4154 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/protocol/cybin/endian_port.h
--rw-r--r--   0 asaka      (501) staff       (20)      939 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/protocol/exc.py
--rw-r--r--   0 asaka      (501) staff       (20)     6490 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/protocol/json.py
--rw-r--r--   0 asaka      (501) staff       (20)     1146 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/thriftpy2/protocol/multiplex.py
--rw-r--r--   0 asaka      (501) staff       (20)     5392 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/rpc.py
--rw-r--r--   0 asaka      (501) staff       (20)     3074 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/server.py
--rw-r--r--   0 asaka      (501) staff       (20)    13242 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/thrift.py
--rw-r--r--   0 asaka      (501) staff       (20)     9710 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/tornado.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.711884 thriftpy2-0.5.0/thriftpy2/transport/
--rw-r--r--   0 asaka      (501) staff       (20)     1958 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/transport/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)     2342 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/transport/_ssl.py
--rw-r--r--   0 asaka      (501) staff       (20)     2585 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/transport/base.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.717608 thriftpy2-0.5.0/thriftpy2/transport/buffered/
--rw-r--r--   0 asaka      (501) staff       (20)     1673 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/transport/buffered/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)   505401 2024-02-27 09:18:31.000000 thriftpy2-0.5.0/thriftpy2/transport/buffered/cybuffered.c
--rw-r--r--   0 asaka      (501) staff       (20)     2283 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/transport/buffered/cybuffered.pyx
--rw-r--r--   0 asaka      (501) staff       (20)   460367 2024-02-27 09:18:31.000000 thriftpy2-0.5.0/thriftpy2/transport/cybase.c
--rw-r--r--   0 asaka      (501) staff       (20)      562 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/thriftpy2/transport/cybase.pxd
--rw-r--r--   0 asaka      (501) staff       (20)     3539 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/transport/cybase.pyx
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.722720 thriftpy2-0.5.0/thriftpy2/transport/framed/
--rw-r--r--   0 asaka      (501) staff       (20)     2091 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/transport/framed/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)   522242 2024-02-27 09:18:32.000000 thriftpy2-0.5.0/thriftpy2/transport/framed/cyframed.c
--rw-r--r--   0 asaka      (501) staff       (20)     3553 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/thriftpy2/transport/framed/cyframed.pyx
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.729833 thriftpy2-0.5.0/thriftpy2/transport/memory/
--rw-r--r--   0 asaka      (501) staff       (20)     1264 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/transport/memory/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)   469985 2024-02-27 09:18:32.000000 thriftpy2-0.5.0/thriftpy2/transport/memory/cymemory.c
--rw-r--r--   0 asaka      (501) staff       (20)     2008 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/thriftpy2/transport/memory/cymemory.pyx
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.733666 thriftpy2-0.5.0/thriftpy2/transport/sasl/
--rw-r--r--   0 asaka      (501) staff       (20)     7576 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/transport/sasl/__init__.py
--rw-r--r--   0 asaka      (501) staff       (20)   643592 2024-05-07 11:56:59.000000 thriftpy2-0.5.0/thriftpy2/transport/sasl/cysasl.c
--rw-r--r--   0 asaka      (501) staff       (20)     7476 2024-05-07 07:42:55.000000 thriftpy2-0.5.0/thriftpy2/transport/sasl/cysasl.pyx
--rw-r--r--   0 asaka      (501) staff       (20)     7718 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/transport/socket.py
--rw-r--r--   0 asaka      (501) staff       (20)     4945 2023-08-07 06:50:06.000000 thriftpy2-0.5.0/thriftpy2/transport/sslsocket.py
--rw-r--r--   0 asaka      (501) staff       (20)     1059 2023-09-15 11:34:07.000000 thriftpy2-0.5.0/thriftpy2/utils.py
-drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-07 11:57:01.734507 thriftpy2-0.5.0/thriftpy2.egg-info/
--rw-r--r--   0 asaka      (501) staff       (20)     6909 2024-05-07 11:57:01.000000 thriftpy2-0.5.0/thriftpy2.egg-info/PKG-INFO
--rw-r--r--   0 asaka      (501) staff       (20)     8164 2024-05-07 11:57:01.000000 thriftpy2-0.5.0/thriftpy2.egg-info/SOURCES.txt
--rw-r--r--   0 asaka      (501) staff       (20)        1 2024-05-07 11:57:01.000000 thriftpy2-0.5.0/thriftpy2.egg-info/dependency_links.txt
--rw-r--r--   0 asaka      (501) staff       (20)        1 2024-02-25 10:15:24.000000 thriftpy2-0.5.0/thriftpy2.egg-info/not-zip-safe
--rw-r--r--   0 asaka      (501) staff       (20)      322 2024-05-07 11:57:01.000000 thriftpy2-0.5.0/thriftpy2.egg-info/requires.txt
--rw-r--r--   0 asaka      (501) staff       (20)       10 2024-05-07 11:57:01.000000 thriftpy2-0.5.0/thriftpy2.egg-info/top_level.txt
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:04.012588 thriftpy2-0.5.1rc1/
+-rw-r--r--   0 asaka      (501) staff       (20)    20507 2024-05-14 13:15:09.000000 thriftpy2-0.5.1rc1/CHANGES.rst
+-rw-r--r--   0 asaka      (501) staff       (20)     1081 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/LICENSE
+-rw-r--r--   0 asaka      (501) staff       (20)      228 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/MANIFEST.in
+-rw-r--r--   0 asaka      (501) staff       (20)     6912 2024-05-14 13:17:04.012356 thriftpy2-0.5.1rc1/PKG-INFO
+-rw-r--r--   0 asaka      (501) staff       (20)     5164 2024-02-29 11:36:31.000000 thriftpy2-0.5.1rc1/README.rst
+-rw-r--r--   0 asaka      (501) staff       (20)       62 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/pyproject.toml
+-rw-r--r--   0 asaka      (501) staff       (20)      313 2024-05-14 13:17:04.013458 thriftpy2-0.5.1rc1/setup.cfg
+-rw-r--r--   0 asaka      (501) staff       (20)     3997 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/setup.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.881269 thriftpy2-0.5.1rc1/tests/
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.909907 thriftpy2-0.5.1rc1/tests/__pycache__/
+-rw-r--r--   0 asaka      (501) staff       (20)     7417 2024-02-25 10:17:45.000000 thriftpy2-0.5.1rc1/tests/__pycache__/addressbook.cpython-312.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)      459 2024-02-25 10:32:40.000000 thriftpy2-0.5.1rc1/tests/__pycache__/conftest.cpython-312-pytest-6.2.5.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)      459 2024-02-25 10:34:10.000000 thriftpy2-0.5.1rc1/tests/__pycache__/conftest.cpython-312-pytest-7.4.4.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)      459 2024-02-25 10:17:44.000000 thriftpy2-0.5.1rc1/tests/__pycache__/conftest.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)      884 2024-02-25 10:17:45.000000 thriftpy2-0.5.1rc1/tests/__pycache__/container.cpython-312.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    25692 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/storm.cpython-312.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    29360 2024-02-25 10:19:38.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_aio.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     2127 2024-02-25 10:19:38.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_aio_protocol_binary.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     1892 2024-02-25 10:19:38.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_aio_protocol_compact.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    19687 2024-02-25 10:19:38.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_all_protocols_binary_field.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    10464 2024-02-25 10:19:38.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_apache_json.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    13313 2024-02-25 10:19:38.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_base.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     6450 2024-02-25 10:19:38.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_buffered_transport.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    10348 2024-02-25 10:19:38.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_const.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     5366 2024-02-25 10:19:38.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_container.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     8526 2024-02-25 10:19:38.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_cytransport.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     9632 2024-02-25 10:19:38.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_framed_transport.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     9361 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_hook.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    28293 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_http.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    11913 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_json_protocol.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    18427 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_loader.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     8608 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_memory_transport.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     5725 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_multiplexed.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     3727 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_oneway.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    94489 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_parser.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    39707 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_protocol_binary.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    48118 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_protocol_compact.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    62002 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_protocol_cybinary.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     3151 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_recursive_definition.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    31080 2024-02-25 10:32:40.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_rpc.cpython-312-pytest-6.2.5.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    31575 2024-02-25 10:38:02.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_rpc.cpython-312-pytest-7.4.4.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    31376 2024-02-25 10:17:44.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_rpc.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    23616 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_socket.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     4816 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_sslsocket.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    16210 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_tornado.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    57520 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_tracking.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     1514 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_type.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     8815 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/__pycache__/test_type_mismatch.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     4231 2023-12-05 14:37:54.000000 thriftpy2-0.5.1rc1/tests/addressbook.py
+-rw-r--r--   0 asaka      (501) staff       (20)     1118 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/addressbook.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)     1122 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/apache_json_test.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      250 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/base.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      489 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/bin_test.thrift
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.910551 thriftpy2-0.5.1rc1/tests/compatible/
+-rw-r--r--   0 asaka      (501) staff       (20)        0 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/compatible/__init__.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.910883 thriftpy2-0.5.1rc1/tests/compatible/__pycache__/
+-rw-r--r--   0 asaka      (501) staff       (20)      154 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/compatible/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.912566 thriftpy2-0.5.1rc1/tests/compatible/version_2/
+-rw-r--r--   0 asaka      (501) staff       (20)        0 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/compatible/version_2/__init__.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.913709 thriftpy2-0.5.1rc1/tests/compatible/version_2/__pycache__/
+-rw-r--r--   0 asaka      (501) staff       (20)      164 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/compatible/version_2/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)    15876 2024-02-25 10:19:39.000000 thriftpy2-0.5.1rc1/tests/compatible/version_2/__pycache__/tracking.cpython-312.pyc
+-rw-r--r--   0 asaka      (501) staff       (20)     8708 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/compatible/version_2/tracking.py
+-rw-r--r--   0 asaka      (501) staff       (20)      307 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/compatible/version_2/tracking.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       30 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/conftest.py
+-rw-r--r--   0 asaka      (501) staff       (20)      724 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/const.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      461 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/container.py
+-rw-r--r--   0 asaka      (501) staff       (20)      889 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/container.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      103 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/multiplexed.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       53 2023-11-14 10:33:35.000000 thriftpy2-0.5.1rc1/tests/oneway.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      255 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parent.thrift
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.938130 thriftpy2-0.5.1rc1/tests/parser-cases/
+-rw-r--r--   0 asaka      (501) staff       (20)     1694 2024-02-25 09:41:43.000000 thriftpy2-0.5.1rc1/tests/parser-cases/annotations.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       82 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/comments.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      870 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/parser-cases/constants.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       30 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/cpp_include.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      228 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/parser-cases/doubles.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       34 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_dead_include_0.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       34 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_dead_include_1.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       34 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_dead_include_2.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       34 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_dead_include_3.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       81 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_duplicate_exception.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       55 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_duplicate_field_id.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       55 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_duplicate_field_name.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       74 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_duplicate_function.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       93 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_duplicate_service.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       74 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_duplicate_struct.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       47 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_grammer_error_at_eof.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       81 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_service_extends_0.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      263 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_structs_0.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      117 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_structs_1.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       23 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_type_error_0.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       65 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_type_error_1.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      104 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_type_error_2.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       20 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_use_thrift_reserved_keywords.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       21 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_value_ref_0.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       77 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_value_ref_1.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       75 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/e_value_ref_2.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      179 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/enums.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       74 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/include.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       22 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/included.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       33 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/parser-cases/issue_121.include.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       80 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/parser-cases/issue_121.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       97 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/issue_215.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      181 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/issue_252.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      156 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/parser-cases/nest_incomplete_type.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      213 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/recursive_union.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      395 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/service.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       97 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/service_extends.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)     1215 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/shared.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      482 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/parser-cases/structs.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)     4870 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/tutorial.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      224 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/type_ref.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      190 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/type_ref_shared.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      184 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/value_ref.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)       84 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/parser-cases/value_ref_shared.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)      228 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/recursive_definition.thrift
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.945058 thriftpy2-0.5.1rc1/tests/ssl/
+-rw-r--r--   0 asaka      (501) staff       (20)     8141 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/CA.pem
+-rw-r--r--   0 asaka      (501) staff       (20)     3096 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/README.md
+-rw-r--r--   0 asaka      (501) staff       (20)     1740 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/client.crt
+-rw-r--r--   0 asaka      (501) staff       (20)     1679 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/client.key
+-rw-r--r--   0 asaka      (501) staff       (20)     2845 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/client.p12
+-rw-r--r--   0 asaka      (501) staff       (20)     4125 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/client.pem
+-rw-r--r--   0 asaka      (501) staff       (20)     1870 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/client_v3.crt
+-rw-r--r--   0 asaka      (501) staff       (20)     1679 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/client_v3.key
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.946395 thriftpy2-0.5.1rc1/tests/ssl/keygen/
+-rw-r--r--   0 asaka      (501) staff       (20)       42 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/keygen/.gitignore
+-rw-r--r--   0 asaka      (501) staff       (20)     4080 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/keygen/make-serverkey.sh
+-rw-r--r--   0 asaka      (501) staff       (20)     2390 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/server.crt
+-rw-r--r--   0 asaka      (501) staff       (20)     3268 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/server.key
+-rw-r--r--   0 asaka      (501) staff       (20)     4477 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/server.p12
+-rw-r--r--   0 asaka      (501) staff       (20)     5658 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/tests/ssl/server.pem
+-rw-r--r--   0 asaka      (501) staff       (20)    15265 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/storm.py
+-rw-r--r--   0 asaka      (501) staff       (20)     8669 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/storm.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)    11872 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_aio.py
+-rw-r--r--   0 asaka      (501) staff       (20)      900 2023-12-05 14:37:59.000000 thriftpy2-0.5.1rc1/tests/test_aio_protocol_binary.py
+-rw-r--r--   0 asaka      (501) staff       (20)      838 2023-12-05 14:37:59.000000 thriftpy2-0.5.1rc1/tests/test_aio_protocol_compact.py
+-rw-r--r--   0 asaka      (501) staff       (20)     9874 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_all_protocols_binary_field.py
+-rw-r--r--   0 asaka      (501) staff       (20)     5988 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_apache_json.py
+-rw-r--r--   0 asaka      (501) staff       (20)     1989 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/test_base.py
+-rw-r--r--   0 asaka      (501) staff       (20)     3040 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_buffered_transport.py
+-rw-r--r--   0 asaka      (501) staff       (20)      975 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/test_const.py
+-rw-r--r--   0 asaka      (501) staff       (20)     1354 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/test_container.py
+-rw-r--r--   0 asaka      (501) staff       (20)     1377 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_cytransport.py
+-rw-r--r--   0 asaka      (501) staff       (20)     4291 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_framed_transport.py
+-rw-r--r--   0 asaka      (501) staff       (20)     2219 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_hook.py
+-rw-r--r--   0 asaka      (501) staff       (20)     7382 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_http.py
+-rw-r--r--   0 asaka      (501) staff       (20)     2531 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_json_protocol.py
+-rw-r--r--   0 asaka      (501) staff       (20)     2128 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/test_loader.py
+-rw-r--r--   0 asaka      (501) staff       (20)     1648 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/test_memory_transport.py
+-rw-r--r--   0 asaka      (501) staff       (20)     2722 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_multiplexed.py
+-rw-r--r--   0 asaka      (501) staff       (20)      942 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_oneway.py
+-rw-r--r--   0 asaka      (501) staff       (20)    11738 2023-09-15 12:04:17.000000 thriftpy2-0.5.1rc1/tests/test_parser.py
+-rw-r--r--   0 asaka      (501) staff       (20)     7044 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_protocol_binary.py
+-rw-r--r--   0 asaka      (501) staff       (20)     7979 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_protocol_compact.py
+-rw-r--r--   0 asaka      (501) staff       (20)    12803 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_protocol_cybinary.py
+-rw-r--r--   0 asaka      (501) staff       (20)      444 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/test_recursive_definition.py
+-rw-r--r--   0 asaka      (501) staff       (20)     8911 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_rpc.py
+-rw-r--r--   0 asaka      (501) staff       (20)     6854 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_socket.py
+-rw-r--r--   0 asaka      (501) staff       (20)     3179 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_sslsocket.py
+-rw-r--r--   0 asaka      (501) staff       (20)     5812 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_tornado.py
+-rw-r--r--   0 asaka      (501) staff       (20)    15877 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/tests/test_tracking.py
+-rw-r--r--   0 asaka      (501) staff       (20)      212 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/test_type.py
+-rw-r--r--   0 asaka      (501) staff       (20)     3441 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/test_type_mismatch.py
+-rw-r--r--   0 asaka      (501) staff       (20)       49 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/tests/type.thrift
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.951341 thriftpy2-0.5.1rc1/thriftpy2/
+-rw-r--r--   0 asaka      (501) staff       (20)      299 2024-05-14 13:13:35.000000 thriftpy2-0.5.1rc1/thriftpy2/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)      312 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/_compat.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.955240 thriftpy2-0.5.1rc1/thriftpy2/contrib/
+-rw-r--r--   0 asaka      (501) staff       (20)        0 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/__init__.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.958674 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/
+-rw-r--r--   0 asaka      (501) staff       (20)        0 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)     3008 2024-03-05 12:23:36.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/client.py
+-rw-r--r--   0 asaka      (501) staff       (20)     2415 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/processor.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.961120 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/protocol/
+-rw-r--r--   0 asaka      (501) staff       (20)      414 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/protocol/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)      682 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/protocol/base.py
+-rw-r--r--   0 asaka      (501) staff       (20)     8706 2023-12-05 14:37:59.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/protocol/binary.py
+-rw-r--r--   0 asaka      (501) staff       (20)     9678 2023-12-05 14:37:59.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/protocol/compact.py
+-rw-r--r--   0 asaka      (501) staff       (20)     3405 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/rpc.py
+-rw-r--r--   0 asaka      (501) staff       (20)     1477 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/server.py
+-rw-r--r--   0 asaka      (501) staff       (20)    13095 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/socket.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.963584 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/transport/
+-rw-r--r--   0 asaka      (501) staff       (20)      429 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/transport/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)     1048 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/transport/base.py
+-rw-r--r--   0 asaka      (501) staff       (20)     1557 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/transport/buffered.py
+-rw-r--r--   0 asaka      (501) staff       (20)     2048 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/transport/framed.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.965185 thriftpy2-0.5.1rc1/thriftpy2/contrib/tracking/
+-rw-r--r--   0 asaka      (501) staff       (20)     7723 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/tracking/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)     3877 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/tracking/tracker.py
+-rw-r--r--   0 asaka      (501) staff       (20)      404 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/thriftpy2/contrib/tracking/tracking.thrift
+-rw-r--r--   0 asaka      (501) staff       (20)     1247 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/hook.py
+-rw-r--r--   0 asaka      (501) staff       (20)    12042 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/http.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.966894 thriftpy2-0.5.1rc1/thriftpy2/parser/
+-rw-r--r--   0 asaka      (501) staff       (20)     7885 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/parser/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)      625 2023-09-15 12:01:14.000000 thriftpy2-0.5.1rc1/thriftpy2/parser/exc.py
+-rw-r--r--   0 asaka      (501) staff       (20)     4165 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/parser/lexer.py
+-rw-r--r--   0 asaka      (501) staff       (20)    26724 2024-05-14 13:13:15.000000 thriftpy2-0.5.1rc1/thriftpy2/parser/parser.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.971719 thriftpy2-0.5.1rc1/thriftpy2/protocol/
+-rw-r--r--   0 asaka      (501) staff       (20)     1271 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/protocol/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)    12209 2023-11-14 08:47:51.000000 thriftpy2-0.5.1rc1/thriftpy2/protocol/apache_json.py
+-rw-r--r--   0 asaka      (501) staff       (20)      696 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/protocol/base.py
+-rw-r--r--   0 asaka      (501) staff       (20)    11803 2023-12-05 14:37:59.000000 thriftpy2-0.5.1rc1/thriftpy2/protocol/binary.py
+-rw-r--r--   0 asaka      (501) staff       (20)    16965 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/protocol/compact.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.979296 thriftpy2-0.5.1rc1/thriftpy2/protocol/cybin/
+-rw-r--r--   0 asaka      (501) staff       (20)   860411 2024-05-07 11:57:01.000000 thriftpy2-0.5.1rc1/thriftpy2/protocol/cybin/cybin.c
+-rw-r--r--   0 asaka      (501) staff       (20)    13965 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/protocol/cybin/cybin.pyx
+-rw-r--r--   0 asaka      (501) staff       (20)     4154 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/protocol/cybin/endian_port.h
+-rw-r--r--   0 asaka      (501) staff       (20)      939 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/protocol/exc.py
+-rw-r--r--   0 asaka      (501) staff       (20)     6490 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/protocol/json.py
+-rw-r--r--   0 asaka      (501) staff       (20)     1146 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/thriftpy2/protocol/multiplex.py
+-rw-r--r--   0 asaka      (501) staff       (20)     5392 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/rpc.py
+-rw-r--r--   0 asaka      (501) staff       (20)     3074 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/server.py
+-rw-r--r--   0 asaka      (501) staff       (20)    13242 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/thrift.py
+-rw-r--r--   0 asaka      (501) staff       (20)     9710 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/tornado.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.987072 thriftpy2-0.5.1rc1/thriftpy2/transport/
+-rw-r--r--   0 asaka      (501) staff       (20)     1958 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)     2342 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/_ssl.py
+-rw-r--r--   0 asaka      (501) staff       (20)     2585 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/base.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.991922 thriftpy2-0.5.1rc1/thriftpy2/transport/buffered/
+-rw-r--r--   0 asaka      (501) staff       (20)     1673 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/buffered/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)   505401 2024-02-27 09:18:31.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/buffered/cybuffered.c
+-rw-r--r--   0 asaka      (501) staff       (20)     2283 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/buffered/cybuffered.pyx
+-rw-r--r--   0 asaka      (501) staff       (20)   460367 2024-02-27 09:18:31.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/cybase.c
+-rw-r--r--   0 asaka      (501) staff       (20)      562 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/cybase.pxd
+-rw-r--r--   0 asaka      (501) staff       (20)     3539 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/cybase.pyx
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:03.997135 thriftpy2-0.5.1rc1/thriftpy2/transport/framed/
+-rw-r--r--   0 asaka      (501) staff       (20)     2091 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/framed/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)   522242 2024-02-27 09:18:32.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/framed/cyframed.c
+-rw-r--r--   0 asaka      (501) staff       (20)     3553 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/framed/cyframed.pyx
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:04.002047 thriftpy2-0.5.1rc1/thriftpy2/transport/memory/
+-rw-r--r--   0 asaka      (501) staff       (20)     1264 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/memory/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)   469985 2024-02-27 09:18:32.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/memory/cymemory.c
+-rw-r--r--   0 asaka      (501) staff       (20)     2008 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/memory/cymemory.pyx
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:04.007970 thriftpy2-0.5.1rc1/thriftpy2/transport/sasl/
+-rw-r--r--   0 asaka      (501) staff       (20)     7576 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/sasl/__init__.py
+-rw-r--r--   0 asaka      (501) staff       (20)   643592 2024-05-07 11:56:59.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/sasl/cysasl.c
+-rw-r--r--   0 asaka      (501) staff       (20)     7476 2024-05-07 07:42:55.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/sasl/cysasl.pyx
+-rw-r--r--   0 asaka      (501) staff       (20)     7718 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/socket.py
+-rw-r--r--   0 asaka      (501) staff       (20)     4945 2023-08-07 06:50:06.000000 thriftpy2-0.5.1rc1/thriftpy2/transport/sslsocket.py
+-rw-r--r--   0 asaka      (501) staff       (20)     1059 2023-09-15 11:34:07.000000 thriftpy2-0.5.1rc1/thriftpy2/utils.py
+drwxr-xr-x   0 asaka      (501) staff       (20)        0 2024-05-14 13:17:04.008756 thriftpy2-0.5.1rc1/thriftpy2.egg-info/
+-rw-r--r--   0 asaka      (501) staff       (20)     6912 2024-05-14 13:17:03.000000 thriftpy2-0.5.1rc1/thriftpy2.egg-info/PKG-INFO
+-rw-r--r--   0 asaka      (501) staff       (20)     8164 2024-05-14 13:17:03.000000 thriftpy2-0.5.1rc1/thriftpy2.egg-info/SOURCES.txt
+-rw-r--r--   0 asaka      (501) staff       (20)        1 2024-05-14 13:17:03.000000 thriftpy2-0.5.1rc1/thriftpy2.egg-info/dependency_links.txt
+-rw-r--r--   0 asaka      (501) staff       (20)        1 2024-02-25 10:15:24.000000 thriftpy2-0.5.1rc1/thriftpy2.egg-info/not-zip-safe
+-rw-r--r--   0 asaka      (501) staff       (20)      322 2024-05-14 13:17:03.000000 thriftpy2-0.5.1rc1/thriftpy2.egg-info/requires.txt
+-rw-r--r--   0 asaka      (501) staff       (20)       10 2024-05-14 13:17:03.000000 thriftpy2-0.5.1rc1/thriftpy2.egg-info/top_level.txt
```

### Comparing `thriftpy2-0.5.0/CHANGES.rst` & `thriftpy2-0.5.1rc1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+UNRELEASED
+~~~~~~~~~~
+
+- Fix an issue where loading a thrift file in a sub-thread will cause an error.
+
 0.5.0
 ~~~~~
 
 Version 0.5.0
 -------------
 
 Released on May 7, 2024.
```

### Comparing `thriftpy2-0.5.0/LICENSE` & `thriftpy2-0.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/PKG-INFO` & `thriftpy2-0.5.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thriftpy2
-Version: 0.5.0
+Version: 0.5.1rc1
 Summary: Pure python implementation of Apache Thrift.
 Home-page: https://thriftpy2.readthedocs.io/
 Author: ThriftPy Organization
 Author-email: gotzehsing@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Thriftpy/thriftpy2
 Keywords: thrift python thriftpy thriftpy2
```

### Comparing `thriftpy2-0.5.0/README.rst` & `thriftpy2-0.5.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/setup.py` & `thriftpy2-0.5.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/addressbook.cpython-312.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/addressbook.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/container.cpython-312.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/container.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/storm.cpython-312.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/storm.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_aio.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_aio.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_aio_protocol_binary.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_aio_protocol_binary.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_aio_protocol_compact.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_aio_protocol_compact.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_all_protocols_binary_field.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_all_protocols_binary_field.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_apache_json.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_apache_json.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_base.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_base.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_buffered_transport.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_buffered_transport.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_const.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_const.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_container.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_container.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_cytransport.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_cytransport.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_framed_transport.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_framed_transport.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_hook.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_hook.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_http.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_http.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_json_protocol.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_json_protocol.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_loader.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_loader.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_memory_transport.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_memory_transport.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_multiplexed.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_multiplexed.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_oneway.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_oneway.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_parser.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_parser.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_protocol_binary.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_protocol_binary.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_protocol_compact.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_protocol_compact.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_protocol_cybinary.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_protocol_cybinary.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_recursive_definition.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_recursive_definition.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_rpc.cpython-312-pytest-6.2.5.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_rpc.cpython-312-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_rpc.cpython-312-pytest-7.4.4.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_rpc.cpython-312-pytest-7.4.4.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_rpc.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_rpc.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_socket.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_socket.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_sslsocket.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_sslsocket.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_tornado.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_tornado.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_tracking.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_tracking.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_type.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_type.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/__pycache__/test_type_mismatch.cpython-312-pytest-8.0.2.pyc` & `thriftpy2-0.5.1rc1/tests/__pycache__/test_type_mismatch.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/addressbook.py` & `thriftpy2-0.5.1rc1/tests/addressbook.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/addressbook.thrift` & `thriftpy2-0.5.1rc1/tests/addressbook.thrift`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/apache_json_test.thrift` & `thriftpy2-0.5.1rc1/tests/apache_json_test.thrift`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/compatible/version_2/__pycache__/tracking.cpython-312.pyc` & `thriftpy2-0.5.1rc1/tests/compatible/version_2/__pycache__/tracking.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/compatible/version_2/tracking.py` & `thriftpy2-0.5.1rc1/tests/compatible/version_2/tracking.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/const.thrift` & `thriftpy2-0.5.1rc1/tests/const.thrift`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/container.thrift` & `thriftpy2-0.5.1rc1/tests/container.thrift`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/parser-cases/annotations.thrift` & `thriftpy2-0.5.1rc1/tests/parser-cases/annotations.thrift`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/parser-cases/constants.thrift` & `thriftpy2-0.5.1rc1/tests/parser-cases/constants.thrift`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/parser-cases/shared.thrift` & `thriftpy2-0.5.1rc1/tests/parser-cases/shared.thrift`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/parser-cases/tutorial.thrift` & `thriftpy2-0.5.1rc1/tests/parser-cases/tutorial.thrift`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/CA.pem` & `thriftpy2-0.5.1rc1/tests/ssl/CA.pem`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/README.md` & `thriftpy2-0.5.1rc1/tests/ssl/README.md`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/client.crt` & `thriftpy2-0.5.1rc1/tests/ssl/client.crt`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/client.key` & `thriftpy2-0.5.1rc1/tests/ssl/client.key`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/client.p12` & `thriftpy2-0.5.1rc1/tests/ssl/client.p12`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/client.pem` & `thriftpy2-0.5.1rc1/tests/ssl/client.pem`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/client_v3.crt` & `thriftpy2-0.5.1rc1/tests/ssl/client_v3.crt`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/client_v3.key` & `thriftpy2-0.5.1rc1/tests/ssl/client_v3.key`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/keygen/make-serverkey.sh` & `thriftpy2-0.5.1rc1/tests/ssl/keygen/make-serverkey.sh`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/server.crt` & `thriftpy2-0.5.1rc1/tests/ssl/server.crt`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/server.key` & `thriftpy2-0.5.1rc1/tests/ssl/server.key`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/server.p12` & `thriftpy2-0.5.1rc1/tests/ssl/server.p12`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/ssl/server.pem` & `thriftpy2-0.5.1rc1/tests/ssl/server.pem`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/storm.py` & `thriftpy2-0.5.1rc1/tests/storm.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/storm.thrift` & `thriftpy2-0.5.1rc1/tests/storm.thrift`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_aio.py` & `thriftpy2-0.5.1rc1/tests/test_aio.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_aio_protocol_binary.py` & `thriftpy2-0.5.1rc1/tests/test_aio_protocol_binary.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_aio_protocol_compact.py` & `thriftpy2-0.5.1rc1/tests/test_aio_protocol_compact.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_all_protocols_binary_field.py` & `thriftpy2-0.5.1rc1/tests/test_all_protocols_binary_field.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_apache_json.py` & `thriftpy2-0.5.1rc1/tests/test_apache_json.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_base.py` & `thriftpy2-0.5.1rc1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_buffered_transport.py` & `thriftpy2-0.5.1rc1/tests/test_buffered_transport.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_const.py` & `thriftpy2-0.5.1rc1/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_container.py` & `thriftpy2-0.5.1rc1/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_cytransport.py` & `thriftpy2-0.5.1rc1/tests/test_cytransport.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_framed_transport.py` & `thriftpy2-0.5.1rc1/tests/test_framed_transport.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_hook.py` & `thriftpy2-0.5.1rc1/tests/test_hook.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_http.py` & `thriftpy2-0.5.1rc1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_json_protocol.py` & `thriftpy2-0.5.1rc1/tests/test_json_protocol.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_loader.py` & `thriftpy2-0.5.1rc1/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_memory_transport.py` & `thriftpy2-0.5.1rc1/tests/test_memory_transport.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_multiplexed.py` & `thriftpy2-0.5.1rc1/tests/test_multiplexed.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_oneway.py` & `thriftpy2-0.5.1rc1/tests/test_oneway.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_parser.py` & `thriftpy2-0.5.1rc1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_protocol_binary.py` & `thriftpy2-0.5.1rc1/tests/test_protocol_binary.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_protocol_compact.py` & `thriftpy2-0.5.1rc1/tests/test_protocol_compact.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_protocol_cybinary.py` & `thriftpy2-0.5.1rc1/tests/test_protocol_cybinary.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_rpc.py` & `thriftpy2-0.5.1rc1/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_socket.py` & `thriftpy2-0.5.1rc1/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_sslsocket.py` & `thriftpy2-0.5.1rc1/tests/test_sslsocket.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_tornado.py` & `thriftpy2-0.5.1rc1/tests/test_tornado.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_tracking.py` & `thriftpy2-0.5.1rc1/tests/test_tracking.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/tests/test_type_mismatch.py` & `thriftpy2-0.5.1rc1/tests/test_type_mismatch.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/aio/client.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/client.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/aio/processor.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/processor.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/aio/protocol/base.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/protocol/base.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/aio/protocol/binary.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/protocol/binary.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/aio/protocol/compact.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/protocol/compact.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/aio/rpc.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/rpc.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/aio/server.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/server.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/aio/socket.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/socket.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/aio/transport/base.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/transport/base.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/aio/transport/buffered.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/transport/buffered.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/aio/transport/framed.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/aio/transport/framed.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/tracking/__init__.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/contrib/tracking/tracker.py` & `thriftpy2-0.5.1rc1/thriftpy2/contrib/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/hook.py` & `thriftpy2-0.5.1rc1/thriftpy2/hook.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/http.py` & `thriftpy2-0.5.1rc1/thriftpy2/http.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/parser/__init__.py` & `thriftpy2-0.5.1rc1/thriftpy2/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/parser/exc.py` & `thriftpy2-0.5.1rc1/thriftpy2/parser/exc.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/parser/lexer.py` & `thriftpy2-0.5.1rc1/thriftpy2/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/parser/parser.py` & `thriftpy2-0.5.1rc1/thriftpy2/parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -386,17 +386,14 @@
 
     def set_info(self, info):
         self[self.index] = info
         self.index -= 1
         return self.index + 1
 
 
-threadlocal.incomplete_type = CurrentIncompleteType()
-
-
 def p_ref_type(p):
     '''ref_type : IDENTIFIER'''
     ref_type = threadlocal.thrift_stack[-1]
 
     for attr in dir(ref_type):
         if attr in {'__doc__', '__loader__', '__name__', '__package__',
                     '__spec__', '__thrift_file__', '__thrift_meta__'}:
@@ -511,19 +508,14 @@
                        | IDENTIFIER '''
     if len(p) == 4:
         p[0] = p[1], p[3]
     else:
         p[0] = p[1], None  # Without Value
 
 
-threadlocal.thrift_stack = []
-threadlocal.include_dirs_ = ['.']
-threadlocal.thrift_cache = {}
-
-
 def parse(path, module_name=None, include_dirs=None, include_dir=None,
           lexer=None, parser=None, enable_cache=True, encoding='utf-8'):
     """Parse a single thrift file to module object, e.g.::
 
         >>> from thriftpy2.parser.parser import parse
         >>> note_thrift = parse("path/to/note.thrift")
         <module 'note_thrift' (built-in)>
@@ -539,14 +531,23 @@
                         it will be appended to `include_dirs`.
     :param lexer: ply lexer to use, if not provided, `parse` will new one.
     :param parser: ply parser to use, if not provided, `parse` will new one.
     :param enable_cache: if this is set to be `True`, parsed module will be
                          cached, this is enabled by default. If `module_name`
                          is provided, use it as cache key, else use the `path`.
     """
+    # threadlocal should be initialized in every threads
+    initialized = getattr(threadlocal, 'initialized', None)
+    if initialized is None:
+        threadlocal.thrift_stack = []
+        threadlocal.include_dirs_ = ['.']
+        threadlocal.thrift_cache = {}
+        threadlocal.incomplete_type = CurrentIncompleteType()
+        threadlocal.initialized = True
+
     # dead include checking on current stack
     for thrift in threadlocal.thrift_stack:
         if thrift.__thrift_file__ is not None and \
                 os.path.samefile(path, thrift.__thrift_file__):
             raise ThriftParserError('Dead including on %s' % path)
 
     cache_key = module_name or os.path.normpath(path)
```

### Comparing `thriftpy2-0.5.0/thriftpy2/protocol/__init__.py` & `thriftpy2-0.5.1rc1/thriftpy2/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/protocol/apache_json.py` & `thriftpy2-0.5.1rc1/thriftpy2/protocol/apache_json.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/protocol/base.py` & `thriftpy2-0.5.1rc1/thriftpy2/protocol/base.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/protocol/binary.py` & `thriftpy2-0.5.1rc1/thriftpy2/protocol/binary.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/protocol/compact.py` & `thriftpy2-0.5.1rc1/thriftpy2/protocol/compact.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/protocol/cybin/cybin.c` & `thriftpy2-0.5.1rc1/thriftpy2/protocol/cybin/cybin.c`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/protocol/cybin/cybin.pyx` & `thriftpy2-0.5.1rc1/thriftpy2/protocol/cybin/cybin.pyx`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/protocol/cybin/endian_port.h` & `thriftpy2-0.5.1rc1/thriftpy2/protocol/cybin/endian_port.h`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/protocol/exc.py` & `thriftpy2-0.5.1rc1/thriftpy2/protocol/exc.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/protocol/json.py` & `thriftpy2-0.5.1rc1/thriftpy2/protocol/json.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/protocol/multiplex.py` & `thriftpy2-0.5.1rc1/thriftpy2/protocol/multiplex.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/rpc.py` & `thriftpy2-0.5.1rc1/thriftpy2/rpc.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/server.py` & `thriftpy2-0.5.1rc1/thriftpy2/server.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/thrift.py` & `thriftpy2-0.5.1rc1/thriftpy2/thrift.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/tornado.py` & `thriftpy2-0.5.1rc1/thriftpy2/tornado.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/__init__.py` & `thriftpy2-0.5.1rc1/thriftpy2/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/_ssl.py` & `thriftpy2-0.5.1rc1/thriftpy2/transport/_ssl.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/base.py` & `thriftpy2-0.5.1rc1/thriftpy2/transport/base.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/buffered/__init__.py` & `thriftpy2-0.5.1rc1/thriftpy2/transport/buffered/__init__.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/buffered/cybuffered.c` & `thriftpy2-0.5.1rc1/thriftpy2/transport/buffered/cybuffered.c`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/buffered/cybuffered.pyx` & `thriftpy2-0.5.1rc1/thriftpy2/transport/buffered/cybuffered.pyx`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/cybase.c` & `thriftpy2-0.5.1rc1/thriftpy2/transport/cybase.c`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/cybase.pxd` & `thriftpy2-0.5.1rc1/thriftpy2/transport/cybase.pxd`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/cybase.pyx` & `thriftpy2-0.5.1rc1/thriftpy2/transport/cybase.pyx`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/framed/__init__.py` & `thriftpy2-0.5.1rc1/thriftpy2/transport/framed/__init__.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/framed/cyframed.c` & `thriftpy2-0.5.1rc1/thriftpy2/transport/framed/cyframed.c`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/framed/cyframed.pyx` & `thriftpy2-0.5.1rc1/thriftpy2/transport/framed/cyframed.pyx`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/memory/__init__.py` & `thriftpy2-0.5.1rc1/thriftpy2/transport/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/memory/cymemory.c` & `thriftpy2-0.5.1rc1/thriftpy2/transport/memory/cymemory.c`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/memory/cymemory.pyx` & `thriftpy2-0.5.1rc1/thriftpy2/transport/memory/cymemory.pyx`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/sasl/__init__.py` & `thriftpy2-0.5.1rc1/thriftpy2/transport/sasl/__init__.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/sasl/cysasl.c` & `thriftpy2-0.5.1rc1/thriftpy2/transport/sasl/cysasl.c`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/sasl/cysasl.pyx` & `thriftpy2-0.5.1rc1/thriftpy2/transport/sasl/cysasl.pyx`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/socket.py` & `thriftpy2-0.5.1rc1/thriftpy2/transport/socket.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/transport/sslsocket.py` & `thriftpy2-0.5.1rc1/thriftpy2/transport/sslsocket.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2/utils.py` & `thriftpy2-0.5.1rc1/thriftpy2/utils.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-0.5.0/thriftpy2.egg-info/PKG-INFO` & `thriftpy2-0.5.1rc1/thriftpy2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thriftpy2
-Version: 0.5.0
+Version: 0.5.1rc1
 Summary: Pure python implementation of Apache Thrift.
 Home-page: https://thriftpy2.readthedocs.io/
 Author: ThriftPy Organization
 Author-email: gotzehsing@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Thriftpy/thriftpy2
 Keywords: thrift python thriftpy thriftpy2
```

### Comparing `thriftpy2-0.5.0/thriftpy2.egg-info/SOURCES.txt` & `thriftpy2-0.5.1rc1/thriftpy2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

