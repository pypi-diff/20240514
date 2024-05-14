# Comparing `tmp/saur-0.2.1.tar.gz` & `tmp/saur-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saur-0.2.1.tar", last modified: Fri Apr 19 14:08:42 2024, max compression
+gzip compressed data, was "saur-0.2.4.tar", last modified: Tue May 14 15:24:36 2024, max compression
```

## Comparing `saur-0.2.1.tar` & `saur-0.2.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.292301 saur-0.2.1/
--rw-rw-r--   0 aition    (1000) aition    (1000)     3125 2023-08-17 19:01:43.000000 saur-0.2.1/.gitignore
--rw-rw-r--   0 aition    (1000) aition    (1000)    15215 2024-01-01 21:07:23.000000 saur-0.2.1/LICENSE.txt
--rw-r--r--   0 aition    (1000) aition    (1000)     1037 2024-04-19 14:08:42.292301 saur-0.2.1/PKG-INFO
--rw-rw-r--   0 aition    (1000) aition    (1000)       82 2023-08-17 18:51:44.000000 saur-0.2.1/README.md
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/examples/
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/examples/fastapi/
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 17:31:45.000000 saur-0.2.1/examples/fastapi/__init__.py
--rw-rw-r--   0 aition    (1000) aition    (1000)      581 2023-08-17 19:05:39.000000 saur-0.2.1/examples/fastapi/app.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     4901 2024-04-05 18:38:16.000000 saur-0.2.1/examples/fastapi/auth.py
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 19:05:53.000000 saur-0.2.1/examples/fastapi/cli.py
--rw-rw-r--   0 aition    (1000) aition    (1000)      885 2023-08-17 19:05:54.000000 saur-0.2.1/examples/fastapi/models.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     1780 2023-08-17 19:05:56.000000 saur-0.2.1/examples/fastapi/routes.py
--rw-rw-r--   0 aition    (1000) aition    (1000)      519 2023-08-17 19:05:57.000000 saur-0.2.1/examples/fastapi/schemas.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     1397 2024-04-19 14:06:44.000000 saur-0.2.1/pyproject.toml
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/saur/
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 16:44:45.000000 saur-0.2.1/saur/__init__.py
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/saur/app/
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 17:27:09.000000 saur-0.2.1/saur/app/__init__.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     2042 2024-03-13 22:25:15.000000 saur-0.2.1/saur/app/fastapi.py
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/saur/mixins/
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-09-17 21:12:38.000000 saur-0.2.1/saur/mixins/__init__.py
--rw-rw-r--   0 aition    (1000) aition    (1000)      786 2024-04-04 22:15:42.000000 saur-0.2.1/saur/mixins/active.py
--rw-rw-r--   0 aition    (1000) aition    (1000)    13279 2024-04-05 01:27:20.000000 saur-0.2.1/saur/mixins/async_access.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     5469 2024-04-04 22:20:37.000000 saur-0.2.1/saur/mixins/watch.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     3886 2024-04-04 22:23:10.000000 saur-0.2.1/saur/settings.py
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/saur/types/
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 16:44:39.000000 saur-0.2.1/saur/types/__init__.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     1414 2024-04-04 22:15:28.000000 saur-0.2.1/saur/types/delimited.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     1976 2024-01-01 21:55:05.000000 saur-0.2.1/saur/types/hashid.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     2541 2023-08-17 17:30:51.000000 saur-0.2.1/saur/types/numeric_datetime.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     1240 2024-03-20 01:44:04.000000 saur-0.2.1/saur/types/pydantic.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     2430 2024-01-03 23:21:18.000000 saur-0.2.1/saur/types/relativedelta.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     2194 2023-09-14 17:06:30.000000 saur-0.2.1/saur/types/uuid.py
--rw-rw-r--   0 aition    (1000) aition    (1000)       91 2024-04-04 22:40:37.000000 saur-0.2.1/saur/utils.py
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/saur.egg-info/
--rw-r--r--   0 aition    (1000) aition    (1000)     1037 2024-04-19 14:08:42.000000 saur-0.2.1/saur.egg-info/PKG-INFO
--rw-rw-r--   0 aition    (1000) aition    (1000)      723 2024-04-19 14:08:42.000000 saur-0.2.1/saur.egg-info/SOURCES.txt
--rw-rw-r--   0 aition    (1000) aition    (1000)        1 2024-04-19 14:08:42.000000 saur-0.2.1/saur.egg-info/dependency_links.txt
--rw-rw-r--   0 aition    (1000) aition    (1000)       54 2024-04-19 14:08:42.000000 saur-0.2.1/saur.egg-info/requires.txt
--rw-rw-r--   0 aition    (1000) aition    (1000)        5 2024-04-19 14:08:42.000000 saur-0.2.1/saur.egg-info/top_level.txt
--rw-rw-r--   0 aition    (1000) aition    (1000)       38 2024-04-19 14:08:42.292301 saur-0.2.1/setup.cfg
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-05-14 15:24:36.112430 saur-0.2.4/
+-rw-rw-r--   0 aition    (1000) aition    (1000)     3125 2023-08-17 19:01:43.000000 saur-0.2.4/.gitignore
+-rw-rw-r--   0 aition    (1000) aition    (1000)    15215 2024-01-01 21:07:23.000000 saur-0.2.4/LICENSE.txt
+-rw-r--r--   0 aition    (1000) aition    (1000)     1102 2024-05-14 15:24:36.112430 saur-0.2.4/PKG-INFO
+-rw-rw-r--   0 aition    (1000) aition    (1000)       82 2023-08-17 18:51:44.000000 saur-0.2.4/README.md
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-05-14 15:24:36.112430 saur-0.2.4/examples/
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-05-14 15:24:36.112430 saur-0.2.4/examples/fastapi/
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 17:31:45.000000 saur-0.2.4/examples/fastapi/__init__.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)      295 2024-05-10 18:36:19.000000 saur-0.2.4/examples/fastapi/app.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     4901 2024-04-05 18:38:16.000000 saur-0.2.4/examples/fastapi/auth.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 19:05:53.000000 saur-0.2.4/examples/fastapi/cli.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)      885 2023-08-17 19:05:54.000000 saur-0.2.4/examples/fastapi/models.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     1780 2023-08-17 19:05:56.000000 saur-0.2.4/examples/fastapi/routes.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)      519 2023-08-17 19:05:57.000000 saur-0.2.4/examples/fastapi/schemas.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     1510 2024-05-14 15:22:58.000000 saur-0.2.4/pyproject.toml
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-05-14 15:24:36.112430 saur-0.2.4/saur/
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2024-04-19 14:22:08.000000 saur-0.2.4/saur/__init__.py
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-05-14 15:24:36.112430 saur-0.2.4/saur/app/
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 17:27:09.000000 saur-0.2.4/saur/app/__init__.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     2180 2024-05-02 16:50:52.000000 saur-0.2.4/saur/app/fastapi.py
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-05-14 15:24:36.112430 saur-0.2.4/saur/mixins/
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-09-17 21:12:38.000000 saur-0.2.4/saur/mixins/__init__.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)      804 2024-04-19 16:11:07.000000 saur-0.2.4/saur/mixins/active.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)    19700 2024-05-09 05:21:22.000000 saur-0.2.4/saur/mixins/async_access.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     5469 2024-04-04 22:20:37.000000 saur-0.2.4/saur/mixins/watch.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     4629 2024-05-02 16:58:37.000000 saur-0.2.4/saur/settings.py
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-05-14 15:24:36.112430 saur-0.2.4/saur/types/
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 16:44:39.000000 saur-0.2.4/saur/types/__init__.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     1700 2024-05-03 20:37:11.000000 saur-0.2.4/saur/types/delimited.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     2291 2024-05-02 15:31:10.000000 saur-0.2.4/saur/types/hashid.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     3149 2024-05-02 15:31:42.000000 saur-0.2.4/saur/types/numeric_datetime.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     2002 2024-05-08 18:16:52.000000 saur-0.2.4/saur/types/pydantic.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     3151 2024-04-19 16:10:18.000000 saur-0.2.4/saur/types/relativedelta.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     2978 2024-04-19 16:10:14.000000 saur-0.2.4/saur/types/uuid.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)      291 2024-05-01 16:08:20.000000 saur-0.2.4/saur/utils.py
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-05-14 15:24:36.112430 saur-0.2.4/saur.egg-info/
+-rw-r--r--   0 aition    (1000) aition    (1000)     1102 2024-05-14 15:24:36.000000 saur-0.2.4/saur.egg-info/PKG-INFO
+-rw-rw-r--   0 aition    (1000) aition    (1000)      723 2024-05-14 15:24:36.000000 saur-0.2.4/saur.egg-info/SOURCES.txt
+-rw-rw-r--   0 aition    (1000) aition    (1000)        1 2024-05-14 15:24:36.000000 saur-0.2.4/saur.egg-info/dependency_links.txt
+-rw-rw-r--   0 aition    (1000) aition    (1000)       72 2024-05-14 15:24:36.000000 saur-0.2.4/saur.egg-info/requires.txt
+-rw-rw-r--   0 aition    (1000) aition    (1000)        5 2024-05-14 15:24:36.000000 saur-0.2.4/saur.egg-info/top_level.txt
+-rw-rw-r--   0 aition    (1000) aition    (1000)       38 2024-05-14 15:24:36.112430 saur-0.2.4/setup.cfg
```

### Comparing `saur-0.2.1/.gitignore` & `saur-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `saur-0.2.1/LICENSE.txt` & `saur-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `saur-0.2.1/PKG-INFO` & `saur-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saur
-Version: 0.2.1
+Version: 0.2.4
 Summary: SQL Alchemy Utilities Repository
 Author-email: Michael Tartre <quantology.org@gmail.com>
 Project-URL: Homepage, https://gitlab.com/sofet-dev/saur
 Project-URL: Repository, https://gitlab.com/sofet-dev/saur.git
 Project-URL: Issues, https://gitlab.com/sofet-dev/saur/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -17,12 +17,14 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: sqlalchemy>=2
 Requires-Dist: pydantic-settings>=2
 Provides-Extra: fastapi
 Requires-Dist: fastapi; extra == "fastapi"
+Provides-Extra: hashid
+Requires-Dist: randseq; extra == "hashid"
 
 # SQL Alchemy Utility Repository
 
 ## TODO:
  - add testing for fastapi example app
```

### Comparing `saur-0.2.1/examples/fastapi/auth.py` & `saur-0.2.4/examples/fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.1/examples/fastapi/models.py` & `saur-0.2.4/examples/fastapi/models.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.1/examples/fastapi/routes.py` & `saur-0.2.4/examples/fastapi/routes.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.1/examples/fastapi/schemas.py` & `saur-0.2.4/examples/fastapi/schemas.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.1/pyproject.toml` & `saur-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saur"
-version = "0.2.1"
-authors = [
-    {name = "Michael Tartre", email = "quantology.org@gmail.com"},
-]
+version = "0.2.4"
+authors = [{ name = "Michael Tartre", email = "quantology.org@gmail.com" }]
 description = "SQL Alchemy Utilities Repository"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-dependencies = [
-    "sqlalchemy>=2",
-    "pydantic-settings>=2"
-]
+dependencies = ["sqlalchemy>=2", "pydantic-settings>=2"]
 
 [project.urls]
 Homepage = "https://gitlab.com/sofet-dev/saur"
 Repository = "https://gitlab.com/sofet-dev/saur.git"
 Issues = "https://gitlab.com/sofet-dev/saur/-/issues"
 
 [project.optional-dependencies]
 fastapi = ["fastapi"]
+hashid = ["randseq"]
 
 [tool.ruff]
 line-length = 100
 
+[tool.ruff.format]
+skip-magic-trailing-comma = true
+
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "D",
+    "A002",
+    "COM812",
     "I001",
     "TID252",
     "ANN204",
     "ANN101",
     "ANN102",
     "ANN003",
     "ANN401",
@@ -52,10 +53,12 @@
     "PLR0913",
     "PLR2004",
     "PGH003",
     "C901",
     "TRY003",
     "PD901",
     "SIM108",
-    "ERA001", # commented out code, ignore on dev only 
-    "T201",   # print statements, ignore on dev only
+    "TD002",
+    "TD003",
+    "ERA001",  # commented out code, ignore on dev only 
+    "T201",    # print statements, ignore on dev only
 ]
```

### Comparing `saur-0.2.1/saur/app/fastapi.py` & `saur-0.2.4/saur/app/fastapi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,64 @@
-# pylint: disable=missing-module-docstring,missing-function-docstring,missing-class-docstring
 from __future__ import annotations
-from typing import Annotated, Collection, Callable
+# Pydantic needs this import outside of a TYPE_CHECKIGN block
+from fastapi.requests import HTTPConnection  # noqa: TCH002
+from typing import Annotated, Callable, TYPE_CHECKING, AsyncIterator, Any
 from contextlib import asynccontextmanager
 
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm.session import sessionmaker
-from sqlalchemy.sql.schema import MetaData
-from fastapi import Depends, FastAPI #, Request
-from fastapi.requests import HTTPConnection
+from fastapi import Depends, FastAPI
 
 from ..settings import DBSettings
+from ..utils import as_list
+
+if TYPE_CHECKING:
+    from sqlalchemy.sql.schema import MetaData
+
+__all__ = ["Session", "db_lifespan", "database_session"]
 
-__all__ = ["Session", "db_lifespan"]
 
-#async def database_session(request: Request):
 # HTTPConnection -> works for Request and Websocket
-async def database_session(connection: HTTPConnection):
+async def database_session(connection: HTTPConnection) -> AsyncIterator[AsyncSession]:
     session: AsyncSession = connection.state.sessionmaker()
     # for auto-commiting:
     # async with session.begin():
     #    yield session
     try:
         yield session
-    #except:
-        # await session.rollback()
+    # except:
+    # await session.rollback()
     #    raise
     finally:
         await session.close()
 
+
+# example usage:
 Session = Annotated[AsyncSession, Depends(database_session)]
 
-# pylint: disable=unused-argument
+
 @asynccontextmanager
 async def db_lifespan(
-    app: FastAPI, settings: DBSettings | None = None,
-    create_metadata: MetaData | Collection[MetaData] | None=None,
-    init_hook: Callable | None=None,
-    execution_options: dict | None=None, **kwargs,
-):
+    app: FastAPI,  # noqa: ARG001
+    settings: DBSettings | None = None,
+    create_metadata: MetaData | list[MetaData] | None = None,
+    init_hook: Callable | None = None,
+    execution_options: dict | None = None,
+    **kwargs,
+) -> AsyncIterator[dict[str, Any]]:
     if settings is None:
-        settings = DBSettings()
-    engine = settings.create_engine(sync=False, execution_options=execution_options)
-    app_sessionmaker = sessionmaker(engine, class_=AsyncSession, **kwargs)
+        settings = DBSettings()  # pyright: ignore[reportCallIssue]
+    engine = settings.create_async_engine(execution_options=execution_options)
+    # pyright ignores because sessionmaker typing is scuffed for async
+    app_sessionmaker: sessionmaker[AsyncSession] = sessionmaker(  # pyright: ignore
+        engine,  # pyright: ignore
+        class_=AsyncSession,
+        **kwargs,
+    )
     if create_metadata:
         async with engine.begin() as conn:
-            try:
-                metadatas = list(create_metadata)
-            except TypeError:
-                metadatas = [create_metadata]
-            for metadata in metadatas:
+            for metadata in as_list(create_metadata):
                 await conn.run_sync(metadata.create_all)
     if init_hook is not None:
         async with app_sessionmaker() as session:
             await init_hook(session)
-    yield {
-        "engine": engine,
-        "sessionmaker": app_sessionmaker,
-    }
+    yield {"engine": engine, "sessionmaker": app_sessionmaker}
```

### Comparing `saur-0.2.1/saur/mixins/active.py` & `saur-0.2.4/saur/mixins/active.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 from datetime import datetime, UTC
 
 from sqlalchemy.orm import Mapped, mapped_column, declarative_mixin
 from sqlalchemy.ext.hybrid import hybrid_property
 
+from ..utils import utcnow
 
 @declarative_mixin
 class ActiveMixin:
-    created: Mapped[datetime] = mapped_column(default=datetime.utcnow)
+    created: Mapped[datetime] = mapped_column(default=utcnow)
     deactivated: Mapped[datetime | None] = mapped_column(default=None)
 
     @hybrid_property
     def active(self) -> bool:
         return self.deactivated == None  # noqa: E711
 
     @active.inplace.setter
```

### Comparing `saur-0.2.1/saur/mixins/watch.py` & `saur-0.2.4/saur/mixins/watch.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.1/saur/settings.py` & `saur-0.2.4/saur/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from types import SimpleNamespace
 from typing import Callable, Awaitable, TYPE_CHECKING
 from functools import cached_property, partial
 
 from sqlalchemy.engine import URL, Engine, create_engine
-from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine
+from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine, AsyncEngine
 from sqlalchemy.orm.session import Session, sessionmaker
 
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
 if TYPE_CHECKING:
     from sqlalchemy.sql.schema import MetaData
     import pandas as pd
@@ -76,56 +76,69 @@
     port: int | None = None  # port constraints?
     username: str | None = None
     password: str | None = None
     database: str | None = None
     driver: str | None = None
     echo: bool = False
 
-    def url(self, *, sync: bool = True) -> URL:
+    def url(self, *, sync: bool = True) -> str:
         settings = self.model_dump()
         settings.pop("echo")
         return database_url(sync=sync, **settings)
 
-    def create_engine(self, *, sync: bool = True, **kwargs) -> Engine:
-        url = self.url(sync=sync)
+
+    def create_sync_engine(self, **kwargs) -> Engine:
+        url = self.url(sync=False)
+        kwargs.setdefault("echo", self.echo)
+        return create_engine(url, **kwargs)
+
+    def create_async_engine(self, **kwargs) -> AsyncEngine:
+        url = self.url(sync=True)
         kwargs.setdefault("echo", self.echo)
-        if sync:
-            return create_engine(url, **kwargs)
         return create_async_engine(url, **kwargs)
 
+    def create_engine(self, *, sync: bool = True, **kwargs) -> Engine | AsyncEngine:
+        fn = self.create_sync_engine if sync else self.create_async_engine
+        return fn(**kwargs)
+
     @cached_property
     def engine(self) -> Engine:
-        return self.create_engine()
+        return self.create_sync_engine()
 
     def sessionmaker(
         self,
         *,
         sync: bool = True,
-        engine: Engine | None = None,
+        engine: Engine | AsyncEngine | None = None,
         **kwargs,
-    ) -> Session:
+    ) -> sessionmaker[Session]:
         if engine is None:
             engine = self.create_engine(sync=sync)
-        return sessionmaker(engine, class_=Session if sync else AsyncSession, **kwargs)
+        session_class = Session if sync else AsyncSession
+        return sessionmaker(bind=engine, class_=session_class, **kwargs)  # pyright: ignore[reportCallIssue, reportArgumentType]
 
     def read_sql(self, sql: str, **kwargs) -> pd.DataFrame:
         import pandas as pd
-
         return pd.read_sql(sql, con=self.engine, **kwargs)
 
     def create_all(
         self,
         metadata: MetaData,
         *,
         sync: bool = True,
-        engine: Engine | None = None,
+        engine: Engine | AsyncEngine | None = None,
     ) -> Callable[[], Awaitable | None]:
         if engine is None:
             engine = self.create_engine(sync=sync)
         if sync:
+            if not isinstance(engine, Engine):
+                msg = "Sync table creation requires sync engine"
+                raise TypeError(msg)
             return partial(metadata.create_all, engine)
-
+        if not isinstance(engine, AsyncEngine):
+            msg = "Async table creation requires async engine"
+            raise TypeError(msg)
         async def async_create_all() -> None:
             async with engine.begin() as conn:
                 await conn.run_sync(metadata.create_all)  # pylint: disable=no-member
 
         return async_create_all
```

### Comparing `saur-0.2.1/saur/types/hashid.py` & `saur-0.2.4/saur/types/numeric_datetime.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,96 @@
-# pylint: disable=missing-module-docstring,missing-function-docstring,missing-class-docstring
-from typing import Self
-from sqlalchemy.types import TypeDecorator, Integer
-from sqlalchemy.dialects.postgresql import JSONB
+from __future__ import annotations
+from typing import TYPE_CHECKING, Any
+from datetime import datetime, timedelta, timezone, UTC
+
+from sqlalchemy.types import TypeDecorator
+from sqlalchemy import Integer, Float
+
+if TYPE_CHECKING:
+    from sqlalchemy import Dialect
+    from sqlalchemy.sql.operators import OperatorType
+    from sqlalchemy.types import TypeEngine
+
+
+# as numeric b/c dateinterval logic is not supported by sqlalchemy across dialects
+class FloatDateTime(TypeDecorator):
+    impl = Float
+    # python_type = datetime
+    cache_ok = True
+
+    def process_bind_param(self, value: datetime | None, dialect: Dialect) -> float | None: # noqa: ARG002
+        if value is None:
+            return None
+        # all datetimes are UTC
+        return value.replace(tzinfo=timezone.utc).timestamp()
+
+    def process_result_value(self, value: float | None, dialect: Dialect) -> datetime | None: # noqa: ARG002
+        if value is None:
+            return None
+        # all datetimes are UTCtcfromtimestamp(value)
+        return datetime.fromtimestamp(value, tz=UTC)
 
-import randseq
+    def coerce_compared_value(self, op: OperatorType | None, value: Any) -> TypeEngine:
+        return self.impl.coerce_compared_value(op, value)  # pyright: ignore[reportCallIssue]
+        if isinstance(value, float):
+            return Float()
+        if isinstance(value, int):
+            return Integer()
+        return self
 
-class StringInteger(TypeDecorator):
-    # no-op type as fallback for undefined HashID
+    def __repr__(self) -> str:
+        return "FloatDateTime"
+
+
+class IntDateTime(FloatDateTime):
     impl = Integer
-    python_type = str
-    cache_ok = True
 
-    def __init__(self, nullable: bool=True):
-        self.nullable = nullable
-        super().__init__()
+    def process_bind_param(self, value: datetime | None, dialect: Dialect) -> int | None:
+        result = super().process_bind_param(value, dialect)
+        if result is None:
+            return None
+        return int(result)
+
+    def __repr__(self) -> str:
+        return "IntDateTime"
+
 
-    def process_bind_param(self, value: str | None, dialect) -> int | None:
-        if self.nullable and value is None:
+class FloatTimeDelta(TypeDecorator):
+    impl = Float
+    # python_type = timedelta
+    cache_ok = True
+
+    def process_bind_param(self, value: timedelta | float | None, dialect: Dialect) -> float | None: # noqa: ARG002
+        if value is None:
             return None
-        return int(value)
+        if isinstance(value, (float, int)):
+            return value
+        return timedelta.total_seconds(value)
 
-    def process_result_value(self, value: int | None, dialect) -> str | None:
-        if self.nullable and value is None:
+    def process_result_value(self, value: float | None, dialect: Dialect) -> timedelta | None: # noqa: ARG002
+        if value is None:
             return None
-        return str(value)
+        return timedelta(seconds=value)
+
+    def coerce_compared_value(self, op: OperatorType | None, value: Any) -> TypeEngine:
+        return self.impl.coerce_compared_value(op, value)  # pyright: ignore[reportCallIssue]
+        if isinstance(value, float):
+            return Float()
+        if isinstance(value, int):
+            return Integer()
+        return self
 
-class HashID(TypeDecorator):
+    def __repr__(self) -> str:
+        return "FloatTimeDelta"
+
+
+class IntTimeDelta(FloatTimeDelta):
     impl = Integer
-    python_type = str
-    cache_ok = True
 
-    @classmethod
-    def loads(cls, spec: str | None, nullable: bool=True) -> Self | StringInteger:
-        if spec is None:
-            return StringInteger(nullable=nullable)
-        hashid = HashID.loads(spec)
-        return cls(**hashid.to_dict(), nullable=nullable)
-
-    def __init__(
-        self,
-        bound: int,
-        init: int,
-        prog: int,
-        alphabet: str,
-        outlen: int,
-        nullable: bool=True,
-    ):
-        self.hashid = randseq.HashID(
-            bound=bound,
-            init=init,
-            prog=prog,
-            alphabet=alphabet,
-            outlen=outlen,
-        )
-        self.nullable = nullable
-        super().__init__()
-
-    def process_bind_param(self, value: str | None, dialect) -> int | None:
-        if self.nullable and value is None:
+    def process_bind_param(self, value: timedelta | float | None, dialect: Dialect) -> int | None:
+        result = super().process_bind_param(value, dialect)
+        if result is None:
             return None
-        return self.hashid.invert(value)
+        return int(result)
 
-    def process_result_value(self, value: int | None, dialect) -> str | None:
-        if self.nullable and value is None:
-            return None
-        return self.hashid.hash(value)
+    def __repr__(self) -> str:
+        return "IntTimeDelta"
```

### Comparing `saur-0.2.1/saur/types/relativedelta.py` & `saur-0.2.4/saur/types/relativedelta.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,23 @@
-# pylint: disable=missing-module-docstring,missing-function-docstring,missing-class-docstring
+from __future__ import annotations
+from typing import TYPE_CHECKING, Any
 from dateutil.relativedelta import relativedelta
 
 from sqlalchemy.types import TypeDecorator, JSON
 from sqlalchemy.dialects.postgresql import JSONB
 from pydantic import BaseModel
 
-def not_private(attr: str):
-    return not attr.startswith('_')
+if TYPE_CHECKING:
+    from sqlalchemy import Dialect
+    from sqlalchemy.types import TypeEngine
+
+
+def not_private(attr: str) -> bool:
+    return not attr.startswith("_")
+
 
 class RelativeDeltaModel(BaseModel):
     years: int = 0
     months: int = 0
     days: int = 0
     leapdays: int = 0
     hours: int = 0
@@ -23,58 +30,76 @@
     hour: int | None = None
     minute: int | None = None
     second: int | None = None
     microsecond: int | None = None
     weekday: int | None = None
     # _has_time: int ?
 
-    def relativedelta(self):
+    def relativedelta(self) -> relativedelta:
         return relativedelta(**self.model_dump())
 
-def _screen_values(delta: dict[str, int | None]):
+
+def _screen_values(delta: dict[str, int | None]) -> dict[str, int]:
     return {
-        k: v for k, v in delta.items()
-        if not (
-            k.startswith("_") or
-            v is None or
-            (k.endswith("s") and v == 0)
-        )
+        k: v
+        for k, v in delta.items()
+        if not (k.startswith("_") or v is None or (k.endswith("s") and v == 0))
     }
 
-def serialize_relativedelta(
-    delta: relativedelta | RelativeDeltaModel | dict,
-) -> dict[str, int | None]:
+
+def serialize_relativedelta(delta: relativedelta | RelativeDeltaModel | dict) -> dict[str, int]:
     if isinstance(delta, relativedelta):
         return _screen_values(delta.__dict__)
     if isinstance(delta, RelativeDeltaModel):
         return _screen_values(delta.model_dump())
     if isinstance(delta, dict):
         return _screen_values(delta)
-    raise TypeError(f"Unknown type for relativedelta: {type(delta)}")
+    msg = f"Unknown type for relativedelta: {type(delta)}"
+    raise TypeError(msg)
+
 
 def deserialize_relativedelta(delta: dict[str, int | None]) -> relativedelta:
-    return relativedelta(**delta)
+    if "dt1" in delta or "dt2" in delta:
+        msg = "Unsupported arguments"
+        raise ValueError(msg)
+    return relativedelta(**delta)  # pyright: ignore[reportArgumentType]
+
 
 class RelativeDelta(TypeDecorator):
     impl = JSON
-    python_type = relativedelta
+    # python_type = relativedelta
     cache_ok = True
 
-    def __init__(self, nullable: bool=True):
+    def __init__(self, *, nullable: bool = True):
         self.nullable = nullable
         super().__init__()
 
-    def process_bind_param(self, value, dialect):
-        if self.nullable and value is None:
-            return None
+    def process_bind_param(
+        self,
+        value: relativedelta | RelativeDeltaModel | dict | None,
+        dialect: Dialect,  # noqa: ARG002
+    ) -> None | dict[str, int]:
+        if value is None:
+            if self.nullable:
+                return None
+            msg = "Null value in non-nullable column"
+            raise ValueError(msg)
         return serialize_relativedelta(value)
 
-    def process_result_value(self, value, dialect):
-        if self.nullable and value is None:
-            return None
+    def process_result_value(
+        self,
+        value: dict[str, int | None] | None,
+        dialect: Dialect,  # noqa: ARG002
+    ) -> relativedelta | None:
+        if value is None:
+            if self.nullable:
+                return None
+            msg = "Null value in non-nullable column"
+            raise ValueError(msg)
         return deserialize_relativedelta(value)
 
+
 class RelativeDeltaB(RelativeDelta):
-    def load_dialect_impl(self, dialect):
-        if dialect.name == 'postgresql':
+    def load_dialect_impl(self, dialect: Dialect) -> TypeEngine[Any]:
+        if dialect.name == "postgresql":
             return dialect.type_descriptor(JSONB())
         return dialect.type_descriptor(JSON())
```

### Comparing `saur-0.2.1/saur/types/uuid.py` & `saur-0.2.4/saur/types/uuid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,82 @@
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
 # adapted from https://stackoverflow.com/a/30604002
 # and from https://sqlalchemy-utils.readthedocs.io/en/latest/_modules/sqlalchemy_utils/types/uuid.html#UUIDType
 import uuid
 
 from sqlalchemy.types import TypeDecorator, BINARY, CHAR
 from sqlalchemy.dialects import postgresql, mssql
 
+if TYPE_CHECKING:
+    from sqlalchemy import Dialect
+    from sqlalchemy.types import TypeEngine
+
+
 class UUID(TypeDecorator):
     """Platform-independent GUID type.
 
     Uses Postgresql's UUID type, otherwise uses
     BINARY(16), to store UUID.
 
     """
+
     impl = BINARY(16)
-    python_type = uuid.UUID
+    # python_type = uuid.UUID
     cache_ok = True
 
-    def __init__(self, binary: bool=True, native: bool=True):
+    def __init__(self, *, binary: bool = True, native: bool = True):
         self.binary = binary
         self.native = native
         super().__init__()
 
-    def load_dialect_impl(self, dialect):
+    def load_dialect_impl(self, dialect: Dialect) -> TypeEngine:
         if self.native:
-            if dialect.name in ('postgresql', 'cockroachdb'):
+            if dialect.name in ("postgresql", "cockroachdb"):
                 return dialect.type_descriptor(postgresql.UUID())
-            if dialect.name == 'mssql':
+            if dialect.name == "mssql":
                 return dialect.type_descriptor(mssql.UNIQUEIDENTIFIER())
-        impl = BINARY(16) if self.binary else CHAR(32)
-        return dialect.type_descriptor(impl)
-
-    def process_bind_param(self, value, dialect) -> None | str | bytes:
+        if self.binary:
+            return dialect.type_descriptor(BINARY(16))
+        return dialect.type_descriptor(CHAR(32))
+
+    def process_bind_param(
+        self, value: None | bytes | int | str | uuid.UUID, dialect: Dialect
+    ) -> None | str | bytes:
         if value is None:
             return value
         if not isinstance(value, uuid.UUID):
-            if isinstance(value, bytes):
+            if isinstance(value, (bytes, bytearray, memoryview)):
                 value = uuid.UUID(bytes=value)
             elif isinstance(value, int):
                 value = uuid.UUID(int=value)
             elif isinstance(value, str):
                 value = uuid.UUID(value)
-        if self.native and dialect.name in (
-            'postgresql', 'mssql', 'cockroachdb',
-        ):
+        if self.native and dialect.name in ("postgresql", "mssql", "cockroachdb"):
             return str(value)
         return value.bytes if self.binary else value.hex
 
-    def process_result_value(self, value, dialect) -> None | uuid.UUID:
+    def process_result_value(
+        self,
+        value: None | str | bytes | uuid.UUID,
+        dialect: Dialect,  # noqa: ARG002
+    ) -> None | uuid.UUID:
         if value is None:
             return value
-        if self.native and dialect.name in (
-            'postgresql', 'mssql', 'cockroachdb',
-        ):
-            if isinstance(value, uuid.UUID):
-                result = value
-            else:
-                result = uuid.UUID(value)
-        elif self.binary:
-            result = uuid.UUID(bytes=value)
-        else:
-            result = uuid.UUID(value)
-        return result
+        if isinstance(value, uuid.UUID):
+            return value
+        # if self.native and dialect.name in ("postgresql", "mssql", "cockroachdb"):
+        #    if isinstance(value, (bytes, bytearray, memoryview)):
+        #        msg = "Must specify binary=True to allow bytes values"
+        #        raise TypeError(msg)
+        #    result = uuid.UUID(value)
+        is_binary = isinstance(value, (bytes, bytearray, memoryview))
+        if self.binary:
+            if not is_binary:
+                msg = "Must specify byte values with binary=True"
+                raise TypeError(msg)
+            return uuid.UUID(bytes=value)
+        if is_binary:
+            msg = "Must specify binary=True to allow bytes values"
+            raise TypeError(msg)
+        return uuid.UUID(value)
```

### Comparing `saur-0.2.1/saur.egg-info/PKG-INFO` & `saur-0.2.4/saur.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saur
-Version: 0.2.1
+Version: 0.2.4
 Summary: SQL Alchemy Utilities Repository
 Author-email: Michael Tartre <quantology.org@gmail.com>
 Project-URL: Homepage, https://gitlab.com/sofet-dev/saur
 Project-URL: Repository, https://gitlab.com/sofet-dev/saur.git
 Project-URL: Issues, https://gitlab.com/sofet-dev/saur/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -17,12 +17,14 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: sqlalchemy>=2
 Requires-Dist: pydantic-settings>=2
 Provides-Extra: fastapi
 Requires-Dist: fastapi; extra == "fastapi"
+Provides-Extra: hashid
+Requires-Dist: randseq; extra == "hashid"
 
 # SQL Alchemy Utility Repository
 
 ## TODO:
  - add testing for fastapi example app
```

### Comparing `saur-0.2.1/saur.egg-info/SOURCES.txt` & `saur-0.2.4/saur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

