# Comparing `tmp/BL_Python.database-0.1.0.tar.gz` & `tmp/bl_python_database-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BL_Python.database-0.1.0.tar", last modified: Wed Feb  7 18:58:32 2024, max compression
+gzip compressed data, was "bl_python_database-0.2.0.tar", last modified: Tue May 14 21:43:13 2024, max compression
```

## Comparing `BL_Python.database-0.1.0.tar` & `bl_python_database-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:32.695716 BL_Python.database-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:32.691716 BL_Python.database-0.1.0/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:32.695716 BL_Python.database-0.1.0/BL_Python/database/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/BL_Python/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/BL_Python/database/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/BL_Python/database/dependency_injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:32.695716 BL_Python.database-0.1.0/BL_Python/database/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/BL_Python/database/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/BL_Python/database/engine/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:32.695716 BL_Python.database-0.1.0/BL_Python/database/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/BL_Python/database/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/BL_Python/database/migrations/alembic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:32.695716 BL_Python.database-0.1.0/BL_Python.database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-07 18:58:32.000000 BL_Python.database-0.1.0/BL_Python.database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-07 18:58:32.000000 BL_Python.database-0.1.0/BL_Python.database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 18:58:32.000000 BL_Python.database-0.1.0/BL_Python.database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-07 18:58:32.000000 BL_Python.database-0.1.0/BL_Python.database.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-07 18:58:32.000000 BL_Python.database-0.1.0/BL_Python.database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-07 18:58:32.695716 BL_Python.database-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 18:58:32.695716 BL_Python.database-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:32.691716 BL_Python.database-0.1.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:32.695716 BL_Python.database-0.1.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-02-07 18:58:24.000000 BL_Python.database-0.1.0/test/unit/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.887207 bl_python_database-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.871207 bl_python_database-0.2.0/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.875207 bl_python_database-0.2.0/BL_Python/database/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/dependency_injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.875207 bl_python_database-0.2.0/BL_Python/database/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/engine/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/engine/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.875207 bl_python_database-0.2.0/BL_Python/database/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.875207 bl_python_database-0.2.0/BL_Python/database/migrations/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/alembic/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/alembic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/alembic/_replacement_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/alembic/_replacement_env_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/alembic/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/alembic/bl_alembic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/alembic/env_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/alembic/script.py.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/migrations/alembic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.879207 bl_python_database-0.2.0/BL_Python/database/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/schema/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/schema/metabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/schema/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/schema/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.879207 bl_python_database-0.2.0/BL_Python/database/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/BL_Python/database/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.887207 bl_python_database-0.2.0/BL_Python.database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-14 21:43:13.000000 bl_python_database-0.2.0/BL_Python.database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-14 21:43:13.000000 bl_python_database-0.2.0/BL_Python.database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:43:13.000000 bl_python_database-0.2.0/BL_Python.database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 21:43:13.000000 bl_python_database-0.2.0/BL_Python.database.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 21:43:13.000000 bl_python_database-0.2.0/BL_Python.database.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 21:43:13.000000 bl_python_database-0.2.0/BL_Python.database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-14 21:43:13.887207 bl_python_database-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:43:13.887207 bl_python_database-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.871207 bl_python_database-0.2.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.879207 bl_python_database-0.2.0/test/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.871207 bl_python_database-0.2.0/test/unit/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.879207 bl_python_database-0.2.0/test/unit/migrations/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/test/unit/migrations/alembic/test_bl_alembic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/test/unit/migrations/alembic/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.879207 bl_python_database-0.2.0/test/unit/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/test/unit/schema/test_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/test/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/test/unit/test_dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/test/unit/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/test/unit/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.871207 bl_python_database-0.2.0/typings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.879207 bl_python_database-0.2.0/typings/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/__main__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.879207 bl_python_database-0.2.0/typings/alembic/autogenerate/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/autogenerate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/autogenerate/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/autogenerate/compare.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/autogenerate/render.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/autogenerate/rewriter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29823 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/context.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.883206 bl_python_database-0.2.0/typings/alembic/ddl/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/ddl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/ddl/_autogen.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/ddl/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/ddl/impl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/ddl/mssql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/ddl/mysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/ddl/oracle.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/ddl/postgresql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/ddl/sqlite.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/migration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    48244 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/op.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.883206 bl_python_database-0.2.0/typings/alembic/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/operations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    64920 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/operations/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/operations/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    62676 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/operations/ops.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/operations/schemaobj.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/operations/toimpl.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.883206 bl_python_database-0.2.0/typings/alembic/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    35932 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/runtime/environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19478 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/runtime/migration.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.887207 bl_python_database-0.2.0/typings/alembic/script/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/script/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/script/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/script/revision.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/script/write_hooks.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.887207 bl_python_database-0.2.0/typings/alembic/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/testing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/testing/assertions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/testing/env.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/testing/fixtures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/testing/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:43:13.887207 bl_python_database-0.2.0/typings/alembic/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/util/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/util/editor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/util/exc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/util/langhelpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/util/messaging.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/util/pyfiles.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-14 21:43:09.000000 bl_python_database-0.2.0/typings/alembic/util/sqla_compat.pyi
```

### Comparing `BL_Python.database-0.1.0/BL_Python/database/dependency_injection.py` & `bl_python_database-0.2.0/BL_Python/database/dependency_injection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from BL_Python.database.config import Config, DatabaseConfig
 from BL_Python.database.engine import DatabaseEngine
-from injector import Binder, CallableProvider, Module, inject, singleton
+from BL_Python.database.types import MetaBase
+from BL_Python.programming.dependency_injection import ConfigModule
+from injector import Binder, CallableProvider, Injector, Module, inject, singleton
 from sqlalchemy.orm.scoping import ScopedSession
 from sqlalchemy.orm.session import Session
 from typing_extensions import override
 
 from .config import DatabaseConfig
 
 
 class ScopedSessionModule(Module):
     """
     Configure SQLAlchemy Session depedencies for Injector.
     """
 
+    _bases: list[MetaBase | type[MetaBase]] | None = None
+
     @override
-    def configure(
-        self, binder: Binder, database_config: DatabaseConfig | None = None
-    ) -> None:
+    def configure(self, binder: Binder) -> None:
         # Any ScopedSession dependency should be the same for the lifetime of the application.
         # ScopeSession is a factory that creates a Session per thread.
         # The Session returned is the same for the lifetime of the thread.
         binder.bind(
             ScopedSession,
             to=CallableProvider(self._get_scoped_session),
             scope=singleton,
@@ -28,30 +31,48 @@
         # Injecting a Session means calling the ScopedSession factory.
         # This is largely a convenience dependency, because the same
         # instance can be obtained by executing the factory that is
         # ScopedSession. ScopedSession handles all thread local concerns.
         # It is safe for this method to be called multiple times.
         binder.bind(Session, to=CallableProvider(self._get_session))
 
-        # it is possible for DatabaseConfig to have been registered
-        # in another module for the IoC container.
-        if database_config:
-            binder.bind(DatabaseConfig, database_config)
+    def __init__(self, bases: list[MetaBase | type[MetaBase]] | None = None) -> None:
+        super().__init__()
+        self._bases = bases
 
     @inject
     def _get_scoped_session(self, database_config: DatabaseConfig) -> ScopedSession:
         """
         Returns a ScopedSession instance configured with
         the correct engine and connection string.
         Defaults to using the `sessionmaker` Session factory.
         """
         return DatabaseEngine.get_session_from_connection_string(
-            database_config.connection_string, database_config.sqlalchemy_echo
+            database_config.connection_string,
+            database_config.sqlalchemy_echo,
+            {},
+            database_config.connect_args,
+            bases=self._bases,
         )
 
     @inject
     def _get_session(self, session_factory: ScopedSession) -> Session:
         """
         Returns a Session instance from the injected ScopedSession instance.
         """
         session: Session = session_factory()
         return session
+
+
+def get_database_config_container(config: Config):
+    config_module = ConfigModule(config, Config)
+    database_config_module = ConfigModule(config.database, DatabaseConfig)
+
+    return Injector([config_module, database_config_module])
+
+
+def get_database_ioc_container(
+    config: Config, bases: list[MetaBase | type[MetaBase]] | None = None
+):
+    container = get_database_config_container(config)
+    container.binder.install(ScopedSessionModule(bases=bases))
+    return container
```

### Comparing `BL_Python.database-0.1.0/BL_Python/database/engine/sqlite.py` & `bl_python_database-0.2.0/BL_Python/database/engine/postgresql.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,78 @@
-from typing import Any, Callable
+from importlib.util import find_spec
+from typing import Any, Callable, Union
 
-from sqlalchemy import create_engine, event
+from BL_Python.database.config import DatabaseConnectArgsConfig
+from BL_Python.database.types import IScopedSessionFactory, MetaBase
+from sqlalchemy import create_engine
+from sqlalchemy.engine import Engine
 from sqlalchemy.orm.scoping import ScopedSession
 from sqlalchemy.orm.session import sessionmaker
-from sqlalchemy.pool import Pool, StaticPool
+from typing_extensions import override
 
 
-class SQLiteScopedSession(ScopedSession):
+class PostgreSQLScopedSession(
+    ScopedSession, IScopedSessionFactory["PostgreSQLScopedSession"]
+):
+    @override
     @staticmethod
     def create(
         connection_string: str,
         echo: bool = False,
         execution_options: dict[str, Any] | None = None,
-    ):
-        """
-        Create a new session factory for SQLite.
-        """
-        poolclass: type[Pool] | None = None
-        # if the connection string is an SQLite in-memory database
-        # then make SQLAlchemy maintain a static pool of "connections"
-        # so that the in-memory database is not deallocated. Otherwise,
-        # the database would disappear when a thread is done with it.
-        # Note: SQLite will reject usage from other threads unless
-        # the connection string also contains `?check_same_thread=False`,
-        # e.g. `sqlite:///:memory:?check_same_thread=False`
-        if ":memory:" in connection_string:
-            poolclass = StaticPool
+        connect_args: DatabaseConnectArgsConfig | None = None,
+        bases: list[MetaBase | type[MetaBase]] | None = None,
+    ) -> "PostgreSQLScopedSession":
+        if find_spec("psycopg2") is None:
+            raise ModuleNotFoundError(
+                "No module named 'psycopg2'. Install PostgreSQL support through `BL_Python.database[postgres]` or `BL_Python.database[postgres-binary]`."
+            )
 
         engine = create_engine(
             connection_string,
             echo=echo,
             execution_options=execution_options or {},
-            poolclass=poolclass,
+            connect_args=connect_args.model_dump() if connect_args is not None else {},
         )
 
-        return SQLiteScopedSession(
+        if bases:
+            PostgreSQLScopedSession._alter_base_schemas(engine, bases)
+
+        return PostgreSQLScopedSession(
             sessionmaker(autocommit=False, autoflush=False, bind=engine)
         )
 
+    @staticmethod
+    def _alter_base_schemas(engine: Engine, bases: list[MetaBase | type[MetaBase]]):
+        # This renames all tables to undo any renaming that previously happened
+        # from, e.g., our SQLite engine.
+        for metadata_base in bases:
+            metadata_base.metadata.reflect(bind=engine)
+            for table_subclass in type(metadata_base).__subclasses__(metadata_base):
+                schema: str | None = None
+                if hasattr(metadata_base, "__table_args__") and isinstance(
+                    metadata_base.__table_args__, dict
+                ):
+                    schema = metadata_base.__table_args__.get("schema")
+
+                if schema:
+                    table_name: list[str] = table_subclass.__tablename__.split(".")
+                    # Trim all prepended schema names
+                    while table_name[0] == schema:
+                        table_name = table_name[1:]
+
+                    table_subclass.__tablename__ = table_name[0]
+
+                    for table in metadata_base.metadata.sorted_tables:
+                        table_name = table.name.split(".")
+                        while table_name[0] == table.schema:
+                            table_name = table_name[1:]
+
+                        table.name = ".".join(table_name)
+                        table.fullname = f"{table.schema}.{table.name}"
+
     def __init__(
         self,
-        session_factory: Callable[..., Any] | "sessionmaker[Any]",
+        session_factory: Union[Callable[..., Any], "sessionmaker[Any]"],
         scopefunc: Any = None,
     ) -> None:
         super().__init__(session_factory, scopefunc)
-        """
-        This callback is used to subscribe to the "connect" core SQLAlchemy event.
-        When a session is instantiated from sessionmaker, and immediately after a connection
-        is made to the database, this will issue the `pragma foreign_key=ON` query. This
-        query ensures SQLite respects foreign key constraints.
-        This will be removed at a later date.
-        """
-
-        def _fk_pragma_on_connect(dbapi_con: Any, con_record: Any):
-            """
-            Called immediately after a connection is established.
-            """
-            dbapi_con.execute("pragma foreign_keys=ON")
-
-        event.listen(self.bind, "connect", _fk_pragma_on_connect)
```

### Comparing `BL_Python.database-0.1.0/BL_Python/database/migrations/alembic.py` & `bl_python_database-0.2.0/BL_Python/database/migrations/alembic.py`

 * *Files identical despite different names*

### Comparing `BL_Python.database-0.1.0/BL_Python.database.egg-info/PKG-INFO` & `bl_python_database-0.2.0/BL_Python.database.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.database
-Version: 0.1.0
+Version: 0.2.0
 Summary: Libraries for working with databases in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
@@ -30,7 +30,15 @@
 Requires-Dist: psycopg2~=2.9; extra == "postgres"
 Provides-Extra: postgres-binary
 Requires-Dist: psycopg2-binary~=2.9; extra == "postgres-binary"
 
 # `BL_Python.database`
 
 Libraries for working with databases in Boutros Lab.
+
+# SQLite Support
+
+SQLite support is built into `BL_Python.database`.
+
+# PostgreSQL Support
+
+Install `BL_Python.database[postgres]` for production use or `BL_Python.database[postgres-binary]` if your machine cannot compile [psycopg2](https://pypi.org/project/psycopg2/).
```

### Comparing `BL_Python.database-0.1.0/LICENSE.md` & `bl_python_database-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `BL_Python.database-0.1.0/PKG-INFO` & `bl_python_database-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.database
-Version: 0.1.0
+Version: 0.2.0
 Summary: Libraries for working with databases in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
@@ -30,7 +30,15 @@
 Requires-Dist: psycopg2~=2.9; extra == "postgres"
 Provides-Extra: postgres-binary
 Requires-Dist: psycopg2-binary~=2.9; extra == "postgres-binary"
 
 # `BL_Python.database`
 
 Libraries for working with databases in Boutros Lab.
+
+# SQLite Support
+
+SQLite support is built into `BL_Python.database`.
+
+# PostgreSQL Support
+
+Install `BL_Python.database[postgres]` for production use or `BL_Python.database[postgres-binary]` if your machine cannot compile [psycopg2](https://pypi.org/project/psycopg2/).
```

### Comparing `BL_Python.database-0.1.0/pyproject.toml` & `bl_python_database-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 
 [tool.setuptools.packages.find]
 exclude = ["build*"]
 
 [tool.setuptools.package-data]
 "BL_Python.database" = ["py.typed"]
 
+[project.scripts]
+bl-alembic = "BL_Python.database.migrations.alembic.__main__:bl_alembic"
+
 [project.optional-dependencies]
 postgres = [
     "psycopg2 ~= 2.9"
 ]
 
 postgres-binary = [
     "psycopg2-binary ~= 2.9"
```

### Comparing `BL_Python.database-0.1.0/test/unit/test_config.py` & `bl_python_database-0.2.0/test/unit/test_config.py`

 * *Files identical despite different names*

