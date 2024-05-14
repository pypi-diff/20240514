# Comparing `tmp/najapy-1.3.1.tar.gz` & `tmp/najapy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "najapy-1.3.1.tar", last modified: Thu Jul  6 11:08:23 2023, max compression
+gzip compressed data, was "najapy-1.3.2.tar", last modified: Tue May 14 08:21:11 2024, max compression
```

## Comparing `najapy-1.3.1.tar` & `najapy-1.3.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.802632 najapy-1.3.1/
--rw-r--r--   0 lanqiao    (501) staff       (20)    11357 2022-07-06 03:22:18.000000 najapy-1.3.1/LICENSE
--rw-r--r--   0 lanqiao    (501) staff       (20)     2836 2023-07-06 11:08:23.801777 najapy-1.3.1/PKG-INFO
--rw-r--r--   0 lanqiao    (501) staff       (20)     2372 2023-06-29 07:51:40.000000 najapy-1.3.1/README.md
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.747203 najapy-1.3.1/najapy/
--rw-r--r--   0 lanqiao    (501) staff       (20)       48 2023-06-29 07:33:14.000000 najapy-1.3.1/najapy/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.750529 najapy-1.3.1/najapy/asyncio/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/asyncio/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3731 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/asyncio/future.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.752102 najapy-1.3.1/najapy/cache/
--rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/cache/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     4209 2023-05-24 08:53:21.000000 najapy-1.3.1/najapy/cache/base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    10506 2023-05-24 07:59:26.000000 najapy-1.3.1/najapy/cache/redis.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.758527 najapy-1.3.1/najapy/common/
--rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     8923 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/async_base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    23020 2023-06-30 05:47:17.000000 najapy-1.3.1/najapy/common/base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2827 2023-03-02 04:19:59.000000 najapy-1.3.1/najapy/common/buffer.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      564 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/error.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     6647 2022-10-14 09:29:48.000000 najapy-1.3.1/najapy/common/excel.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/interface.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/metaclass.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1691 2023-07-05 08:49:30.000000 najapy-1.3.1/najapy/common/pool.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1681 2023-03-17 09:08:13.000000 najapy-1.3.1/najapy/common/process.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     8528 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/struct.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2607 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/common/task.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.760176 najapy-1.3.1/najapy/database/
--rw-r--r--   0 lanqiao    (501) staff       (20)       49 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/database/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3750 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/database/mongo.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    15285 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/database/mysql.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.761336 najapy-1.3.1/najapy/enum/
--rw-r--r--   0 lanqiao    (501) staff       (20)       19 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/enum/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3141 2023-02-07 09:30:47.000000 najapy-1.3.1/najapy/enum/base_enum.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.763184 najapy-1.3.1/najapy/event/
--rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/event/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3443 2023-07-03 12:07:52.000000 najapy-1.3.1/najapy/event/async_event.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1210 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/event/event.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.764351 najapy-1.3.1/najapy/frame/
--rwxr-xr-x   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.767504 najapy-1.3.1/najapy/frame/fastapi/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/fastapi/__init__.py
--rwxr-xr-x   0 lanqiao    (501) staff       (20)     3263 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/fastapi/base.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3067 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/fastapi/form.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1042 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/fastapi/response.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1723 2023-03-02 04:30:39.000000 najapy-1.3.1/najapy/frame/fastapi/ws.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3334 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/frame/logging.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.768273 najapy-1.3.1/najapy/middleware/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-06-29 07:36:25.000000 najapy-1.3.1/najapy/middleware/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.770605 najapy-1.3.1/najapy/middleware/rabbitmq/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-06-29 07:36:39.000000 najapy-1.3.1/najapy/middleware/rabbitmq/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     5629 2023-07-06 06:07:51.000000 najapy-1.3.1/najapy/middleware/rabbitmq/consumer.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     7046 2023-07-05 08:41:39.000000 najapy-1.3.1/najapy/middleware/rabbitmq/producer.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2649 2023-07-05 08:58:21.000000 najapy-1.3.1/najapy/middleware/rabbitmq/producer_pool.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.771861 najapy-1.3.1/najapy/net/
--rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/net/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     8066 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/net/http.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.772416 najapy-1.3.1/najapy/scaffold/
--rw-r--r--   0 lanqiao    (501) staff       (20)       16 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.773312 najapy-1.3.1/najapy/scaffold/fastapi_example_project/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.775737 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.776284 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.777103 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)       75 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/base_model.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.778122 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/
--rw-r--r--   0 lanqiao    (501) staff       (20)        1 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3629 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.779253 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      842 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      315 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/activate.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.779907 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.782422 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/external_view.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/internal_view.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/model.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/schemas.py
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/service.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.786963 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/
--rw-r--r--   0 lanqiao    (501) staff       (20)     3486 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.dev.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.rel.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      107 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/gunicorn.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.dev.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.rel.conf
--rw-r--r--   0 lanqiao    (501) staff       (20)      983 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1276 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/main.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      582 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/router.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.787361 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/services/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/services/__init__.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.788215 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/utils/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/utils/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1655 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      161 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/scaffold/fastapi_example_project/manage.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.789340 najapy-1.3.1/najapy/static/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/static/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)   208075 2022-07-06 03:22:18.000000 najapy-1.3.1/najapy/static/cacert.pem
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.749703 najapy-1.3.1/najapy.egg-info/
--rw-r--r--   0 lanqiao    (501) staff       (20)     2836 2023-07-06 11:08:23.000000 najapy-1.3.1/najapy.egg-info/PKG-INFO
--rw-r--r--   0 lanqiao    (501) staff       (20)     4359 2023-07-06 11:08:23.000000 najapy-1.3.1/najapy.egg-info/SOURCES.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)        1 2023-07-06 11:08:23.000000 najapy-1.3.1/najapy.egg-info/dependency_links.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)      524 2023-07-06 11:08:23.000000 najapy-1.3.1/najapy.egg-info/requires.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)       13 2023-07-06 11:08:23.000000 najapy-1.3.1/najapy.egg-info/top_level.txt
--rw-r--r--   0 lanqiao    (501) staff       (20)       38 2023-07-06 11:08:23.802809 najapy-1.3.1/setup.cfg
--rw-r--r--   0 lanqiao    (501) staff       (20)     1951 2023-06-30 07:24:25.000000 najapy-1.3.1/setup.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.793568 najapy-1.3.1/tests/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-10-14 09:29:48.000000 najapy-1.3.1/tests/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      166 2022-10-14 09:29:48.000000 najapy-1.3.1/tests/main.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      863 2023-03-02 04:30:39.000000 najapy-1.3.1/tests/test_buffer.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3059 2023-01-12 02:07:34.000000 najapy-1.3.1/tests/test_func_cache.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1596 2023-07-04 09:54:43.000000 najapy-1.3.1/tests/test_obj_pool.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.795458 najapy-1.3.1/tests/test_rabbitmq/
--rw-r--r--   0 lanqiao    (501) staff       (20)       51 2023-07-05 02:21:37.000000 najapy-1.3.1/tests/test_rabbitmq/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1690 2023-07-06 10:37:21.000000 najapy-1.3.1/tests/test_rabbitmq/test_counsumer.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     3804 2023-07-06 10:59:25.000000 najapy-1.3.1/tests/test_rabbitmq/test_procuder_pool.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     4296 2023-07-05 09:02:09.000000 najapy-1.3.1/tests/test_rabbitmq/test_producer.py
-drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2023-07-06 11:08:23.800843 najapy-1.3.1/tests/test_redis/
--rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-03-15 01:19:41.000000 najapy-1.3.1/tests/test_redis/__init__.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     6863 2023-03-20 02:43:59.000000 najapy-1.3.1/tests/test_redis/conftest.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1337 2023-03-16 04:32:18.000000 najapy-1.3.1/tests/test_redis/mocks.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    26721 2023-03-29 02:50:21.000000 najapy-1.3.1/tests/test_redis/test_commands.py
--rw-r--r--   0 lanqiao    (501) staff       (20)    10554 2023-03-20 02:45:47.000000 najapy-1.3.1/tests/test_redis/test_connection_pool.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2889 2023-03-27 06:50:02.000000 najapy-1.3.1/tests/test_redis/test_distributed_event.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2079 2023-03-24 10:25:17.000000 najapy-1.3.1/tests/test_redis/test_lock.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     2587 2023-03-27 06:38:07.000000 najapy-1.3.1/tests/test_redis/test_pub_sub.py
--rw-r--r--   0 lanqiao    (501) staff       (20)      923 2023-03-30 08:02:33.000000 najapy-1.3.1/tests/test_redis/test_share_cache.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1319 2023-06-30 05:56:22.000000 najapy-1.3.1/tests/test_sync_utils.py
--rw-r--r--   0 lanqiao    (501) staff       (20)     1319 2023-06-30 03:14:48.000000 najapy-1.3.1/tests/test_utils.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.230854 najapy-1.3.2/
+-rw-r--r--   0 lanqiao    (501) staff       (20)    11357 2022-07-06 03:22:18.000000 najapy-1.3.2/LICENSE
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2836 2024-05-14 08:21:11.229579 najapy-1.3.2/PKG-INFO
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2372 2023-06-29 07:51:40.000000 najapy-1.3.2/README.md
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.126773 najapy-1.3.2/najapy/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       48 2024-05-14 05:53:57.000000 najapy-1.3.2/najapy/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.130813 najapy-1.3.2/najapy/asyncio/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/asyncio/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3731 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/asyncio/future.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.133856 najapy-1.3.2/najapy/cache/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/cache/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     4209 2023-08-17 08:22:06.000000 najapy-1.3.2/najapy/cache/base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    10506 2023-05-24 07:59:26.000000 najapy-1.3.2/najapy/cache/redis.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.144019 najapy-1.3.2/najapy/common/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/common/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     8923 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/common/async_base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    23020 2023-06-30 05:47:17.000000 najapy-1.3.2/najapy/common/base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2827 2023-03-02 04:19:59.000000 najapy-1.3.2/najapy/common/buffer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      564 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/common/error.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     6647 2022-10-14 09:29:48.000000 najapy-1.3.2/najapy/common/excel.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/common/interface.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      651 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/common/metaclass.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1691 2023-07-05 08:49:30.000000 najapy-1.3.2/najapy/common/pool.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1681 2023-03-17 09:08:13.000000 najapy-1.3.2/najapy/common/process.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     8528 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/common/struct.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2607 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/common/task.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.146565 najapy-1.3.2/najapy/database/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       49 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/database/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3750 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/database/mongo.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    15285 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/database/mysql.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.148889 najapy-1.3.2/najapy/enum/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       19 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/enum/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3141 2023-02-07 09:30:47.000000 najapy-1.3.2/najapy/enum/base_enum.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.153350 najapy-1.3.2/najapy/event/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       52 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/event/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3443 2023-07-03 12:07:52.000000 najapy-1.3.2/najapy/event/async_event.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1210 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/event/event.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.156399 najapy-1.3.2/najapy/frame/
+-rwxr-xr-x   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/frame/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.160194 najapy-1.3.2/najapy/frame/fastapi/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/frame/fastapi/__init__.py
+-rwxr-xr-x   0 lanqiao    (501) staff       (20)     3263 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/frame/fastapi/base.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     4622 2024-05-14 06:00:56.000000 najapy-1.3.2/najapy/frame/fastapi/form.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1042 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/frame/fastapi/response.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1723 2023-03-02 04:30:39.000000 najapy-1.3.2/najapy/frame/fastapi/ws.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3334 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/frame/logging.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.161291 najapy-1.3.2/najapy/middleware/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-06-29 07:36:25.000000 najapy-1.3.2/najapy/middleware/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.164986 najapy-1.3.2/najapy/middleware/rabbitmq/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-06-29 07:36:39.000000 najapy-1.3.2/najapy/middleware/rabbitmq/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     5629 2023-07-06 06:07:51.000000 najapy-1.3.2/najapy/middleware/rabbitmq/consumer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     7046 2023-07-05 08:41:39.000000 najapy-1.3.2/najapy/middleware/rabbitmq/producer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2649 2023-07-05 08:58:21.000000 najapy-1.3.2/najapy/middleware/rabbitmq/producer_pool.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.169462 najapy-1.3.2/najapy/net/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       46 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/net/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     8066 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/net/http.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.171438 najapy-1.3.2/najapy/scaffold/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       16 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.173817 najapy-1.3.2/najapy/scaffold/fastapi_example_project/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.177826 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.178697 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.179851 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)       75 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/model/base_model.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.181649 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        1 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3629 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.184394 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      842 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      315 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/activate.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.186006 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/apps/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/apps/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.189315 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/external_view.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/internal_view.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/model.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/schemas.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/apps/example_app/service.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.200286 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/conf/
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3486 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      362 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.dev.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/conf/dynamic.rel.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      107 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/conf/gunicorn.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      396 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.dev.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/conf/static.rel.conf
+-rw-r--r--   0 lanqiao    (501) staff       (20)      983 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1276 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/main.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      582 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/router.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.200769 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/services/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/services/__init__.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.201747 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/utils/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/utils/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1655 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      161 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/scaffold/fastapi_example_project/manage.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.203738 najapy-1.3.2/najapy/static/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/static/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)   208075 2022-07-06 03:22:18.000000 najapy-1.3.2/najapy/static/cacert.pem
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.129938 najapy-1.3.2/najapy.egg-info/
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2836 2024-05-14 08:21:10.000000 najapy-1.3.2/najapy.egg-info/PKG-INFO
+-rw-r--r--   0 lanqiao    (501) staff       (20)     4359 2024-05-14 08:21:11.000000 najapy-1.3.2/najapy.egg-info/SOURCES.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)        1 2024-05-14 08:21:10.000000 najapy-1.3.2/najapy.egg-info/dependency_links.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)      524 2024-05-14 08:21:10.000000 najapy-1.3.2/najapy.egg-info/requires.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)       13 2024-05-14 08:21:10.000000 najapy-1.3.2/najapy.egg-info/top_level.txt
+-rw-r--r--   0 lanqiao    (501) staff       (20)       38 2024-05-14 08:21:11.231274 najapy-1.3.2/setup.cfg
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1951 2024-05-14 05:52:57.000000 najapy-1.3.2/setup.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.212080 najapy-1.3.2/tests/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2022-10-14 09:29:48.000000 najapy-1.3.2/tests/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      166 2022-10-14 09:29:48.000000 najapy-1.3.2/tests/main.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      863 2023-03-02 04:30:39.000000 najapy-1.3.2/tests/test_buffer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3059 2023-08-17 08:22:06.000000 najapy-1.3.2/tests/test_func_cache.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1596 2023-07-04 09:54:43.000000 najapy-1.3.2/tests/test_obj_pool.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.216217 najapy-1.3.2/tests/test_rabbitmq/
+-rw-r--r--   0 lanqiao    (501) staff       (20)       51 2023-07-05 02:21:37.000000 najapy-1.3.2/tests/test_rabbitmq/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1690 2023-07-06 10:37:21.000000 najapy-1.3.2/tests/test_rabbitmq/test_counsumer.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     3804 2023-07-06 10:59:25.000000 najapy-1.3.2/tests/test_rabbitmq/test_procuder_pool.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     4296 2023-07-05 09:02:09.000000 najapy-1.3.2/tests/test_rabbitmq/test_producer.py
+drwxr-xr-x   0 lanqiao    (501) staff       (20)        0 2024-05-14 08:21:11.227774 najapy-1.3.2/tests/test_redis/
+-rw-r--r--   0 lanqiao    (501) staff       (20)        0 2023-03-15 01:19:41.000000 najapy-1.3.2/tests/test_redis/__init__.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     6863 2023-03-20 02:43:59.000000 najapy-1.3.2/tests/test_redis/conftest.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1337 2023-03-16 04:32:18.000000 najapy-1.3.2/tests/test_redis/mocks.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    26721 2023-03-29 02:50:21.000000 najapy-1.3.2/tests/test_redis/test_commands.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)    10554 2023-03-20 02:45:47.000000 najapy-1.3.2/tests/test_redis/test_connection_pool.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2889 2023-03-27 06:50:02.000000 najapy-1.3.2/tests/test_redis/test_distributed_event.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2079 2023-03-24 10:25:17.000000 najapy-1.3.2/tests/test_redis/test_lock.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     2587 2023-03-27 06:38:07.000000 najapy-1.3.2/tests/test_redis/test_pub_sub.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)      923 2023-03-30 08:02:33.000000 najapy-1.3.2/tests/test_redis/test_share_cache.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1319 2023-06-30 05:56:22.000000 najapy-1.3.2/tests/test_sync_utils.py
+-rw-r--r--   0 lanqiao    (501) staff       (20)     1319 2023-06-30 03:14:48.000000 najapy-1.3.2/tests/test_utils.py
```

### Comparing `najapy-1.3.1/LICENSE` & `najapy-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/PKG-INFO` & `najapy-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: najapy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Async Suite For Python
 Home-page: https://github.com/lanqiao-dev/najapy.git
 Author: lanqiao
 Author-email: 
 License: Apache License Version 2.0
 Platform: all
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `najapy-1.3.1/README.md` & `najapy-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/asyncio/future.py` & `najapy-1.3.2/najapy/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/cache/base.py` & `najapy-1.3.2/najapy/cache/base.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/cache/redis.py` & `najapy-1.3.2/najapy/cache/redis.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/common/async_base.py` & `najapy-1.3.2/najapy/common/async_base.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/common/base.py` & `najapy-1.3.2/najapy/common/base.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/common/buffer.py` & `najapy-1.3.2/najapy/common/buffer.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/common/error.py` & `najapy-1.3.2/najapy/common/error.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/common/excel.py` & `najapy-1.3.2/najapy/common/excel.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/common/interface.py` & `najapy-1.3.2/najapy/common/interface.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/common/metaclass.py` & `najapy-1.3.2/najapy/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/common/pool.py` & `najapy-1.3.2/najapy/common/pool.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/common/process.py` & `najapy-1.3.2/najapy/common/process.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/common/struct.py` & `najapy-1.3.2/najapy/common/struct.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/common/task.py` & `najapy-1.3.2/najapy/common/task.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/database/mongo.py` & `najapy-1.3.2/najapy/database/mongo.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/database/mysql.py` & `najapy-1.3.2/najapy/database/mysql.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/enum/base_enum.py` & `najapy-1.3.2/najapy/enum/base_enum.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/event/async_event.py` & `najapy-1.3.2/najapy/event/async_event.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/event/event.py` & `najapy-1.3.2/najapy/event/event.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/frame/fastapi/base.py` & `najapy-1.3.2/najapy/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/frame/fastapi/response.py` & `najapy-1.3.2/najapy/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/frame/fastapi/ws.py` & `najapy-1.3.2/najapy/frame/fastapi/ws.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/frame/logging.py` & `najapy-1.3.2/najapy/frame/logging.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/middleware/rabbitmq/consumer.py` & `najapy-1.3.2/najapy/middleware/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/middleware/rabbitmq/producer.py` & `najapy-1.3.2/najapy/middleware/rabbitmq/producer.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/middleware/rabbitmq/producer_pool.py` & `najapy-1.3.2/najapy/middleware/rabbitmq/producer_pool.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/net/http.py` & `najapy-1.3.2/najapy/net/http.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py` & `najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/service/base_service.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py` & `najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/abc_base/view/base_view.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py` & `najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py` & `najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/err_handler.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/main.py` & `najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/main.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/router.py` & `najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/router.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py` & `najapy-1.3.2/najapy/scaffold/fastapi_example_project/fastapi_example/utils/response.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy/static/cacert.pem` & `najapy-1.3.2/najapy/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy.egg-info/PKG-INFO` & `najapy-1.3.2/najapy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: najapy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Async Suite For Python
 Home-page: https://github.com/lanqiao-dev/najapy.git
 Author: lanqiao
 Author-email: 
 License: Apache License Version 2.0
 Platform: all
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `najapy-1.3.1/najapy.egg-info/SOURCES.txt` & `najapy-1.3.2/najapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/najapy.egg-info/requires.txt` & `najapy-1.3.2/najapy.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 WTForms==2.3.3
 aiohttp==3.8.3
 aiomysql==0.0.21
 redis==4.5.3
 async-timeout==4.0.2
 cachetools==4.2.1
 cryptography==3.4.6
-fastapi==0.66.1
+fastapi==0.96.0
 gunicorn==20.1.0
 hiredis==1.1.0
 httptools==0.2.0
 loguru==0.5.3
 motor==2.3.1
 ujson==4.0.2
 pytz==2021.1
```

### Comparing `najapy-1.3.1/setup.py` & `najapy-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
           r'WTForms==2.3.3',
           r'aiohttp==3.8.3',
           r'aiomysql==0.0.21',
           r'redis==4.5.3',
           r'async-timeout==4.0.2',
           r'cachetools==4.2.1',
           r'cryptography==3.4.6',
-          r'fastapi==0.66.1',
+          r'fastapi==0.96.0',
           r'gunicorn==20.1.0',
           r'hiredis==1.1.0',
           r'httptools==0.2.0',
           r'loguru==0.5.3',
           r'motor==2.3.1',
           r'ujson==4.0.2',
           r'pytz==2021.1',
```

### Comparing `najapy-1.3.1/tests/test_buffer.py` & `najapy-1.3.2/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_func_cache.py` & `najapy-1.3.2/tests/test_func_cache.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_obj_pool.py` & `najapy-1.3.2/tests/test_obj_pool.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_rabbitmq/test_counsumer.py` & `najapy-1.3.2/tests/test_rabbitmq/test_counsumer.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_rabbitmq/test_procuder_pool.py` & `najapy-1.3.2/tests/test_rabbitmq/test_procuder_pool.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_rabbitmq/test_producer.py` & `najapy-1.3.2/tests/test_rabbitmq/test_producer.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_redis/conftest.py` & `najapy-1.3.2/tests/test_redis/conftest.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_redis/mocks.py` & `najapy-1.3.2/tests/test_redis/mocks.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_redis/test_commands.py` & `najapy-1.3.2/tests/test_redis/test_commands.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_redis/test_connection_pool.py` & `najapy-1.3.2/tests/test_redis/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_redis/test_distributed_event.py` & `najapy-1.3.2/tests/test_redis/test_distributed_event.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_redis/test_lock.py` & `najapy-1.3.2/tests/test_redis/test_lock.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_redis/test_pub_sub.py` & `najapy-1.3.2/tests/test_redis/test_pub_sub.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_redis/test_share_cache.py` & `najapy-1.3.2/tests/test_redis/test_share_cache.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_sync_utils.py` & `najapy-1.3.2/tests/test_sync_utils.py`

 * *Files identical despite different names*

### Comparing `najapy-1.3.1/tests/test_utils.py` & `najapy-1.3.2/tests/test_utils.py`

 * *Files identical despite different names*

