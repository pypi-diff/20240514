# Comparing `tmp/true_noorm-0.1.0.tar.gz` & `tmp/true_noorm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "true_noorm-0.1.0.tar", max compression
+gzip compressed data, was "true_noorm-0.1.1.tar", max compression
```

## Comparing `true_noorm-0.1.0.tar` & `true_noorm-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1096 2024-04-01 20:21:11.302080 true_noorm-0.1.0/LICENSE
--rw-r--r--   0        0        0     9907 2024-05-12 13:06:36.336928 true_noorm-0.1.0/README.md
--rw-r--r--   0        0        0      605 2024-04-14 20:21:28.268083 true_noorm-0.1.0/noorm/__init__.py
--rw-r--r--   0        0        0      344 2024-05-04 10:53:01.777567 true_noorm-0.1.0/noorm/_common.py
--rw-r--r--   0        0        0     2062 2024-04-28 11:20:04.435058 true_noorm-0.1.0/noorm/_db_api_2.py
--rw-r--r--   0        0        0     1590 2024-04-28 12:16:44.233252 true_noorm-0.1.0/noorm/_db_api_2_args_only.py
--rw-r--r--   0        0        0      432 2024-05-01 20:35:54.548011 true_noorm-0.1.0/noorm/_sqlalchemy_common.py
--rw-r--r--   0        0        0     1391 2023-11-06 11:48:02.264890 true_noorm-0.1.0/noorm/_sqlite_common.py
--rw-r--r--   0        0        0     3842 2024-04-28 18:20:20.451564 true_noorm-0.1.0/noorm/aiomysql/__init__.py
--rw-r--r--   0        0        0     8773 2024-05-05 11:09:38.780394 true_noorm-0.1.0/noorm/aiomysql/_aiomysql.py
--rw-r--r--   0        0        0     3828 2024-04-28 18:20:40.095589 true_noorm-0.1.0/noorm/aiosqlite/__init__.py
--rw-r--r--   0        0        0     9253 2024-05-05 11:14:32.816573 true_noorm-0.1.0/noorm/aiosqlite/_aiosqlite.py
--rw-r--r--   0        0        0     3372 2024-04-28 18:20:56.123608 true_noorm-0.1.0/noorm/asyncpg/__init__.py
--rw-r--r--   0        0        0     8757 2024-05-05 11:25:42.985335 true_noorm-0.1.0/noorm/asyncpg/_asyncpg.py
--rw-r--r--   0        0        0     3335 2024-04-28 18:21:20.011638 true_noorm-0.1.0/noorm/psycopg2/__init__.py
--rw-r--r--   0        0        0     7903 2024-05-05 11:30:41.817632 true_noorm-0.1.0/noorm/psycopg2/_psycopg2.py
--rw-r--r--   0        0        0     3393 2024-04-28 18:21:40.595662 true_noorm-0.1.0/noorm/pymysql/__init__.py
--rw-r--r--   0        0        0     7903 2024-05-05 11:42:27.262297 true_noorm-0.1.0/noorm/pymysql/_pymysql.py
--rw-r--r--   0        0        0     5964 2024-05-11 11:28:59.607705 true_noorm-0.1.0/noorm/registry.py
--rw-r--r--   0        0        0     2490 2024-04-28 18:22:12.759701 true_noorm-0.1.0/noorm/sqlalchemy_async/__init__.py
--rw-r--r--   0        0        0     8526 2024-05-05 09:41:02.776289 true_noorm-0.1.0/noorm/sqlalchemy_async/_sqlalchemy_async.py
--rw-r--r--   0        0        0     2387 2024-05-01 17:45:33.683252 true_noorm-0.1.0/noorm/sqlalchemy_sync/__init__.py
--rw-r--r--   0        0        0     7635 2024-05-05 09:42:24.048547 true_noorm-0.1.0/noorm/sqlalchemy_sync/_sqlalchemy_sync.py
--rw-r--r--   0        0        0     3686 2024-04-28 18:23:12.763770 true_noorm-0.1.0/noorm/sqlite3/__init__.py
--rw-r--r--   0        0        0     8385 2024-05-05 09:42:07.068495 true_noorm-0.1.0/noorm/sqlite3/_sqlite3.py
--rw-r--r--   0        0        0     1557 2024-05-12 13:52:55.611207 true_noorm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10924 1970-01-01 00:00:00.000000 true_noorm-0.1.0/setup.py
--rw-r--r--   0        0        0    11007 1970-01-01 00:00:00.000000 true_noorm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-04-01 20:21:11.302080 true_noorm-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9907 2024-05-12 13:06:36.336928 true_noorm-0.1.1/README.md
+-rw-r--r--   0        0        0      605 2024-04-14 20:21:28.268083 true_noorm-0.1.1/noorm/__init__.py
+-rw-r--r--   0        0        0      344 2024-05-04 10:53:01.777567 true_noorm-0.1.1/noorm/_common.py
+-rw-r--r--   0        0        0     2062 2024-04-28 11:20:04.435058 true_noorm-0.1.1/noorm/_db_api_2.py
+-rw-r--r--   0        0        0     1590 2024-04-28 12:16:44.233252 true_noorm-0.1.1/noorm/_db_api_2_args_only.py
+-rw-r--r--   0        0        0      622 2024-05-14 17:21:15.747551 true_noorm-0.1.1/noorm/_sqlalchemy_common.py
+-rw-r--r--   0        0        0     1391 2023-11-06 11:48:02.264890 true_noorm-0.1.1/noorm/_sqlite_common.py
+-rw-r--r--   0        0        0     3842 2024-04-28 18:20:20.451564 true_noorm-0.1.1/noorm/aiomysql/__init__.py
+-rw-r--r--   0        0        0     8773 2024-05-05 11:09:38.780394 true_noorm-0.1.1/noorm/aiomysql/_aiomysql.py
+-rw-r--r--   0        0        0     3828 2024-04-28 18:20:40.095589 true_noorm-0.1.1/noorm/aiosqlite/__init__.py
+-rw-r--r--   0        0        0     9253 2024-05-05 11:14:32.816573 true_noorm-0.1.1/noorm/aiosqlite/_aiosqlite.py
+-rw-r--r--   0        0        0     3372 2024-04-28 18:20:56.123608 true_noorm-0.1.1/noorm/asyncpg/__init__.py
+-rw-r--r--   0        0        0     8757 2024-05-05 11:25:42.985335 true_noorm-0.1.1/noorm/asyncpg/_asyncpg.py
+-rw-r--r--   0        0        0     3335 2024-04-28 18:21:20.011638 true_noorm-0.1.1/noorm/psycopg2/__init__.py
+-rw-r--r--   0        0        0     7903 2024-05-05 11:30:41.817632 true_noorm-0.1.1/noorm/psycopg2/_psycopg2.py
+-rw-r--r--   0        0        0     3393 2024-04-28 18:21:40.595662 true_noorm-0.1.1/noorm/pymysql/__init__.py
+-rw-r--r--   0        0        0     7903 2024-05-05 11:42:27.262297 true_noorm-0.1.1/noorm/pymysql/_pymysql.py
+-rw-r--r--   0        0        0     5964 2024-05-11 11:28:59.607705 true_noorm-0.1.1/noorm/registry.py
+-rw-r--r--   0        0        0     2883 2024-05-14 17:41:50.122011 true_noorm-0.1.1/noorm/sqlalchemy_async/__init__.py
+-rw-r--r--   0        0        0     9547 2024-05-14 17:29:46.440418 true_noorm-0.1.1/noorm/sqlalchemy_async/_sqlalchemy_async.py
+-rw-r--r--   0        0        0     2780 2024-05-14 17:41:43.849992 true_noorm-0.1.1/noorm/sqlalchemy_sync/__init__.py
+-rw-r--r--   0        0        0     8656 2024-05-14 17:29:09.976076 true_noorm-0.1.1/noorm/sqlalchemy_sync/_sqlalchemy_sync.py
+-rw-r--r--   0        0        0     3686 2024-04-28 18:23:12.763770 true_noorm-0.1.1/noorm/sqlite3/__init__.py
+-rw-r--r--   0        0        0     8385 2024-05-05 09:42:07.068495 true_noorm-0.1.1/noorm/sqlite3/_sqlite3.py
+-rw-r--r--   0        0        0     1557 2024-05-14 17:08:10.607288 true_noorm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10924 1970-01-01 00:00:00.000000 true_noorm-0.1.1/setup.py
+-rw-r--r--   0        0        0    11007 1970-01-01 00:00:00.000000 true_noorm-0.1.1/PKG-INFO
```

### Comparing `true_noorm-0.1.0/LICENSE` & `true_noorm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/README.md` & `true_noorm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/__init__.py` & `true_noorm-0.1.1/noorm/__init__.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/_db_api_2.py` & `true_noorm-0.1.1/noorm/_db_api_2.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/_db_api_2_args_only.py` & `true_noorm-0.1.1/noorm/_db_api_2_args_only.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/_sqlite_common.py` & `true_noorm-0.1.1/noorm/_sqlite_common.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/aiomysql/__init__.py` & `true_noorm-0.1.1/noorm/aiomysql/__init__.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/aiomysql/_aiomysql.py` & `true_noorm-0.1.1/noorm/aiomysql/_aiomysql.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/aiosqlite/__init__.py` & `true_noorm-0.1.1/noorm/aiosqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/aiosqlite/_aiosqlite.py` & `true_noorm-0.1.1/noorm/aiosqlite/_aiosqlite.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/asyncpg/__init__.py` & `true_noorm-0.1.1/noorm/asyncpg/__init__.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/asyncpg/_asyncpg.py` & `true_noorm-0.1.1/noorm/asyncpg/_asyncpg.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/psycopg2/__init__.py` & `true_noorm-0.1.1/noorm/psycopg2/__init__.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/psycopg2/_psycopg2.py` & `true_noorm-0.1.1/noorm/psycopg2/_psycopg2.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/pymysql/__init__.py` & `true_noorm-0.1.1/noorm/pymysql/__init__.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/pymysql/_pymysql.py` & `true_noorm-0.1.1/noorm/pymysql/_pymysql.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/registry.py` & `true_noorm-0.1.1/noorm/registry.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/sqlalchemy_async/__init__.py` & `true_noorm-0.1.1/noorm/sqlalchemy_async/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 - (except `sql_execute`) Expected result type. For `sql_fetch_all` and `sql_one_or_none`
   is usually a dataclass or namedtuple; for `sql_scalar_or_none` and `sql_fetch_scalars`
   is usually `int`, `str`, `bool`, `datetime`, or whatever can be produced by scalar
   query.
 - "No commit" flag. Default is False, so if executed statement is data manipulation
   (insert, update, or delete), commit will be automatically invoked. If you need
   to prevent it for some reason, set no_commit=True.
+- "synchronize_session" SqlAlchemy execution option. By default is False because
+  avoiding using persistent objects is one of the most crucial NoORM ideas. If no
+  persistent object in a session, there is nothing to synchronise. If you really need
+  different behavior, set this `sync_session` parameter to "fetch" or "evaluate", or
+  pass None to turn off the execution option manipulation.
 
 After decoration the decorated function receives an open Session as a first positional
 argument.
 
 Decorated function should return an executable statement (select, insert, update,
 delete).
```

### Comparing `true_noorm-0.1.0/noorm/sqlalchemy_async/_sqlalchemy_async.py` & `true_noorm-0.1.1/noorm/sqlalchemy_async/_sqlalchemy_async.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,20 +20,23 @@
 async def _commit_if_needed(
     session: AsyncSession, sql_stmt: Executable, no_commit: bool
 ):
     if not isinstance(sql_stmt, Select) and not no_commit:
         await session.commit()
 
 
-def sql_fetch_all(row_type: Type[TR], no_commit: bool = False):
+def sql_fetch_all(
+    row_type: Type[TR], no_commit: bool = False, sync_session: bool | str | None = False
+):
     """
     Use this decorator to make `.all()` queries.
 
     :param row_type: type of expected result. Usually some dataclass or named tuple
     :param no_commit: set to False to prevent commit after the DML execution.
+    :param sync_session: execution option `synchronize_session`. Default False.
 
     IMPORTANT: decorated function must not be async, but after decoration it
     becomes async.
 
     More info in the noorm.sqlalchemy_async docstring.
     """
 
@@ -42,15 +45,17 @@
     ) -> Callable[Concatenate[AsyncSession, F_Spec], Coroutine[Any, Any, list[TR]]]:
         class wrapper(WrapperBase):
             async def __call__(
                 self, session: AsyncSession, *args: F_Spec.args, **kwargs: F_Spec.kwargs
             ) -> list[TR]:
                 with MetricsCollector(self._func) as mc:
                     if (
-                        sql_stmt := req_sql_n_params(self._func, args, kwargs)
+                        sql_stmt := req_sql_n_params(
+                            self._func, args, kwargs, sync_session
+                        )
                     ) is not None:
                         q_res = (await session.execute(sql_stmt)).all()
                         await _commit_if_needed(session, sql_stmt, no_commit)
                         res: list[TR] = [
                             row_type(**{n: v for n, v in r._asdict().items()})
                             for r in q_res
                         ]
@@ -59,20 +64,23 @@
                     return []
 
         return wrapper(func)
 
     return decorator
 
 
-def sql_one_or_none(row_type: Type[TR], no_commit: bool = False):
+def sql_one_or_none(
+    row_type: Type[TR], no_commit: bool = False, sync_session: bool | str | None = False
+):
     """
     Use this decorator to make `.one_or_none()` queries.
 
     :param row_type: type of expected result. Usually some dataclass or named tuple
     :param no_commit: set to False to prevent commit after the DML execution.
+    :param sync_session: execution option `synchronize_session`. Default False.
 
     IMPORTANT: decorated function must not be async, but after decoration it
     becomes async.
 
     More info in the noorm.sqlalchemy_async docstring.
     """
 
@@ -81,37 +89,42 @@
     ) -> Callable[Concatenate[AsyncSession, F_Spec], Coroutine[Any, Any, TR | None]]:
         class wrapper(WrapperBase):
             async def __call__(
                 self, session: AsyncSession, *args: F_Spec.args, **kwargs: F_Spec.kwargs
             ) -> TR | None:
                 with MetricsCollector(self._func) as mc:
                     if (
-                        sql_stmt := req_sql_n_params(self._func, args, kwargs)
+                        sql_stmt := req_sql_n_params(
+                            self._func, args, kwargs, sync_session
+                        )
                     ) is not None:
                         q_res = (await session.execute(sql_stmt)).one_or_none()
                         await _commit_if_needed(session, sql_stmt, no_commit)
                         if q_res is None:
                             return None
                         mc.tuples = 1
                         return row_type(**{n: v for n, v in q_res._asdict().items()})
                     return None
 
         return wrapper(func)
 
     return decorator
 
 
-def sql_scalar_or_none(res_type: Type[TR], no_commit: bool = False):
+def sql_scalar_or_none(
+    res_type: Type[TR], no_commit: bool = False, sync_session: bool | str | None = False
+):
     """
     Use this decorator to make a "scalar" SQL statement executor out of
     the function that prepares parameters for the query
 
     :param res_type: type of expected result. For scalar queries it is usually `int`,
     `str`, `bool`, `datetime`, or whatever can be produced by scalar query.
     :param no_commit: set to False to prevent commit after the DML execution.
+    :param sync_session: execution option `synchronize_session`. Default False.
 
     IMPORTANT: decorated function must not be async, but after decoration it
     becomes async.
 
     More info in the noorm.sqlalchemy_async docstring.
     """
 
@@ -120,36 +133,41 @@
     ) -> Callable[Concatenate[AsyncSession, F_Spec], Coroutine[Any, Any, TR | None]]:
         class wrapper(WrapperBase):
             async def __call__(
                 self, session: AsyncSession, *args: F_Spec.args, **kwargs: F_Spec.kwargs
             ) -> TR | None:
                 with MetricsCollector(self._func) as mc:
                     if (
-                        sql_stmt := req_sql_n_params(self._func, args, kwargs)
+                        sql_stmt := req_sql_n_params(
+                            self._func, args, kwargs, sync_session
+                        )
                     ) is not None:
                         q_res = (await session.execute(sql_stmt)).scalar_one_or_none()
                         await _commit_if_needed(session, sql_stmt, no_commit)
                         if q_res is not None:
                             mc.tuples = 1
                         return q_res
                     return None
 
         return wrapper(func)
 
     return decorator
 
 
-def sql_fetch_scalars(res_type: Type[TR], no_commit: bool = False):
+def sql_fetch_scalars(
+    res_type: Type[TR], no_commit: bool = False, sync_session: bool | str | None = False
+):
     """
     Use this decorator to make a "scalars" SQL statement executor out of
     the function that prepares parameters for the query
 
     :param res_type: type of expected result. For scalar queries it is usually `int`,
     `str`, `bool`, `datetime`, or whatever can be produced by scalar query.
     :param no_commit: set to False to prevent commit after the DML execution.
+    :param sync_session: execution option `synchronize_session`. Default False.
 
     IMPORTANT: decorated function must not be async, but after decoration it
     becomes async.
 
     More info in the noorm.sqlalchemy_async docstring.
     """
 
@@ -158,15 +176,17 @@
     ) -> Callable[Concatenate[AsyncSession, F_Spec], Coroutine[Any, Any, list[TR]]]:
         class wrapper(WrapperBase):
             async def __call__(
                 self, session: AsyncSession, *args: F_Spec.args, **kwargs: F_Spec.kwargs
             ) -> list[TR]:
                 with MetricsCollector(self._func) as mc:
                     if (
-                        sql_stmt := req_sql_n_params(self._func, args, kwargs)
+                        sql_stmt := req_sql_n_params(
+                            self._func, args, kwargs, sync_session
+                        )
                     ) is not None:
                         q_res = (await session.execute(sql_stmt)).scalars()
                         await _commit_if_needed(session, sql_stmt, no_commit)
                         res = [el for el in q_res]
                         mc.tuples = len(res)
                         return res
                     return []
@@ -181,30 +201,32 @@
     func: Callable[F_Spec, Executable]
 ) -> Callable[Concatenate[AsyncSession, F_Spec], Coroutine[Any, Any, None]]:
     pass  # pragma: no cover
 
 
 @overload
 def sql_execute(
-    no_commit: bool = False,
+    no_commit: bool = False, sync_session: bool | str | None = False
 ) -> Callable[
     [Callable[F_Spec, Coroutine[Any, Any, None]]],
     Callable[Concatenate[AsyncSession, F_Spec], Coroutine[Any, Any, None]],
 ]:
     pass  # pragma: no cover
 
 
 def sql_execute(  # type: ignore
     func: Callable[F_Spec, Executable] | None = None,
     no_commit: bool = False,
+    sync_session: bool | str | None = False,
 ):
     """
     Use this decorator to execute a statement without responding a result.
 
     :param no_commit: set to False to prevent commit after the DML execution.
+    :param sync_session: execution option `synchronize_session`. Default False.
 
     IMPORTANT: decorated function must not be async, but after decoration it
     becomes async.
 
     More info in the noorm.sqlalchemy_async docstring.
     """
 
@@ -222,15 +244,17 @@
                     self,
                     session: AsyncSession,
                     *args: F_Spec.args,
                     **kwargs: F_Spec.kwargs,
                 ) -> None:
                     with MetricsCollector(self._func):
                         if (
-                            sql_stmt := req_sql_n_params(self._func, args, kwargs)
+                            sql_stmt := req_sql_n_params(
+                                self._func, args, kwargs, sync_session
+                            )
                         ) is not None:
                             await session.execute(sql_stmt)
                             await _commit_if_needed(session, sql_stmt, no_commit)
 
             return wrapper(func)
 
         return decorator
```

### Comparing `true_noorm-0.1.0/noorm/sqlalchemy_sync/__init__.py` & `true_noorm-0.1.1/noorm/sqlalchemy_sync/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 - (except `sql_execute`) Expected result type. For `sql_fetch_all` and `sql_one_or_none`
   is usually a dataclass or namedtuple; for `sql_scalar_or_none` and `sql_fetch_scalars`
   is usually `int`, `str`, `bool`, `datetime`, or whatever can be produced by scalar
   query.
 - "No commit" flag. Default is False, so if executed statement is data manipulation
   (insert, update, or delete), commit will be automatically invoked. If you need
   to prevent it for some reason, set no_commit=True.
+- "synchronize_session" SqlAlchemy execution option. By default is False because
+  avoiding using persistent objects is one of the most crucial NoORM ideas. If no
+  persistent object in a session, there is nothing to synchronise. If you really need
+  different behavior, set this `sync_session` parameter to "fetch" or "evaluate", or
+  pass None to turn off the execution option manipulation.
 
 After decoration the decorated function receives an open Session as a first positional
 argument.
 
 Decorated function should return an executable statement (select, insert, update,
 delete).
```

### Comparing `true_noorm-0.1.0/noorm/sqlalchemy_sync/_sqlalchemy_sync.py` & `true_noorm-0.1.1/noorm/sqlalchemy_sync/_sqlalchemy_sync.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,34 +18,39 @@
 
 
 def _commit_if_needed(session: Session, sql_stmt: Executable, no_commit: bool):
     if not isinstance(sql_stmt, Select) and not no_commit:
         session.commit()
 
 
-def sql_fetch_all(row_type: Type[TR], no_commit: bool = False):
+def sql_fetch_all(
+    row_type: Type[TR], no_commit: bool = False, sync_session: bool | str | None = False
+):
     """
     Use this decorator to make `.all()` queries.
 
     :param row_type: type of expected result. Usually some dataclass or named tuple
     :param no_commit: set to False to prevent commit after the DML execution.
+    :param sync_session: execution option `synchronize_session`. Default False.
 
     More info in the noorm.sqlalchemy_sync docstring.
     """
 
     def decorator(
         func: Callable[F_Spec, Executable]
     ) -> Callable[Concatenate[Session, F_Spec], list[TR]]:
         class wrapper(WrapperBase):
             def __call__(
                 self, session: Session, *args: F_Spec.args, **kwargs: F_Spec.kwargs
             ) -> list[TR]:
                 with MetricsCollector(self._func) as mc:
                     if (
-                        sql_stmt := req_sql_n_params(self._func, args, kwargs)
+                        sql_stmt := req_sql_n_params(
+                            self._func, args, kwargs, sync_session
+                        )
                     ) is not None:
                         q_res = session.execute(sql_stmt).all()
                         _commit_if_needed(session, sql_stmt, no_commit)
                         res: list[TR] = [
                             row_type(**{n: v for n, v in r._asdict().items()})
                             for r in q_res
                         ]
@@ -54,105 +59,120 @@
                     return []
 
         return wrapper(func)
 
     return decorator
 
 
-def sql_one_or_none(row_type: Type[TR], no_commit: bool = False):
+def sql_one_or_none(
+    row_type: Type[TR], no_commit: bool = False, sync_session: bool | str | None = False
+):
     """
     Use this decorator to make `.one_or_none()` queries.
 
     :param row_type: type of expected result. Usually some dataclass or named tuple
     :param no_commit: set to False to prevent commit after the DML execution.
+    :param sync_session: execution option `synchronize_session`. Default False.
 
     More info in the noorm.sqlalchemy_sync docstring.
     """
 
     def decorator(
         func: Callable[F_Spec, Executable],
     ) -> Callable[Concatenate[Session, F_Spec], TR | None]:
         class wrapper(WrapperBase):
             def __call__(
                 self, session: Session, *args: F_Spec.args, **kwargs: F_Spec.kwargs
             ) -> TR | None:
                 with MetricsCollector(self._func) as mc:
                     if (
-                        sql_stmt := req_sql_n_params(self._func, args, kwargs)
+                        sql_stmt := req_sql_n_params(
+                            self._func, args, kwargs, sync_session
+                        )
                     ) is not None:
                         q_res = session.execute(sql_stmt).one_or_none()
                         _commit_if_needed(session, sql_stmt, no_commit)
                         if q_res is None:
                             return None
                         mc.tuples = 1
                         return row_type(**{n: v for n, v in q_res._asdict().items()})
                     return None
 
         return wrapper(func)
 
     return decorator
 
 
-def sql_scalar_or_none(res_type: Type[TR], no_commit: bool = False):
+def sql_scalar_or_none(
+    res_type: Type[TR], no_commit: bool = False, sync_session: bool | str | None = False
+):
     """
     Use this decorator to make a "scalar" SQL statement executor out of
     the function that prepares parameters for the query
 
     :param res_type: type of expected result. For scalar queries it is usually `int`,
     `str`, `bool`, `datetime`, or whatever can be produced by scalar query.
     :param no_commit: set to False to prevent commit after the DML execution.
+    :param sync_session: execution option `synchronize_session`. Default False.
 
     More info in the noorm.sqlalchemy_sync docstring.
     """
 
     def decorator(
         func: Callable[F_Spec, Executable],
     ) -> Callable[Concatenate[Session, F_Spec], TR | None]:
         class wrapper(WrapperBase):
             def __call__(
                 self, session: Session, *args: F_Spec.args, **kwargs: F_Spec.kwargs
             ) -> TR | None:
                 with MetricsCollector(self._func) as mc:
                     if (
-                        sql_stmt := req_sql_n_params(self._func, args, kwargs)
+                        sql_stmt := req_sql_n_params(
+                            self._func, args, kwargs, sync_session
+                        )
                     ) is not None:
                         q_res = session.execute(sql_stmt).scalar_one_or_none()
                         _commit_if_needed(session, sql_stmt, no_commit)
                         if q_res is not None:
                             mc.tuples = 1
                         return q_res
                     return None
 
         return wrapper(func)
 
     return decorator
 
 
-def sql_fetch_scalars(res_type: Type[TR], no_commit: bool = False):
+def sql_fetch_scalars(
+    res_type: Type[TR], no_commit: bool = False, sync_session: bool | str | None = False
+):
     """
     Use this decorator to make a "scalars" SQL statement executor out of
     the function that prepares parameters for the query
 
     :param res_type: type of expected result. For scalar queries it is usually `int`,
     `str`, `bool`, `datetime`, or whatever can be produced by scalar query.
     :param no_commit: set to False to prevent commit after the DML execution.
+    :param sync_session: execution option `synchronize_session`. Default False.
 
     More info in the noorm.sqlalchemy_sync docstring.
     """
 
     def decorator(
         func: Callable[F_Spec, Executable],
     ) -> Callable[Concatenate[Session, F_Spec], list[TR]]:
         class wrapper(WrapperBase):
             def __call__(
                 self, session: Session, *args: F_Spec.args, **kwargs: F_Spec.kwargs
             ) -> list[TR]:
                 with MetricsCollector(self._func) as mc:
                     if (
-                        sql_stmt := req_sql_n_params(self._func, args, kwargs)
+                        sql_stmt := req_sql_n_params(
+                            self._func, args, kwargs, sync_session
+                        )
                     ) is not None:
                         q_res = session.execute(sql_stmt).scalars()
                         _commit_if_needed(session, sql_stmt, no_commit)
                         res = [el for el in q_res]
                         mc.tuples = len(res)
                         return res
                     return []
@@ -167,27 +187,29 @@
     func: Callable[F_Spec, Executable]
 ) -> Callable[Concatenate[Session, F_Spec], None]:
     pass  # pragma: no cover
 
 
 @overload
 def sql_execute(
-    no_commit: bool = False,
+    no_commit: bool = False, sync_session: bool | str | None = False
 ) -> Callable[[Callable[F_Spec, None]], Callable[Concatenate[Session, F_Spec], None]]:
     pass  # pragma: no cover
 
 
 def sql_execute(  # type: ignore
     func: Callable[F_Spec, Executable] | None = None,
     no_commit: bool = False,
+    sync_session: bool | str | None = False,
 ):
     """
     Use this decorator to execute a statement without responding a result.
 
     :param no_commit: set to False to prevent commit after the DML execution.
+    :param sync_session: execution option `synchronize_session`. Default False.
 
     More info in the noorm.sqlalchemy_sync docstring.
     """
 
     if callable(func):
         the_func = func
     else:
@@ -199,15 +221,17 @@
         ) -> Callable[Concatenate[Session, F_Spec], None]:
             class wrapper(WrapperBase):
                 def __call__(
                     self, session: Session, *args: F_Spec.args, **kwargs: F_Spec.kwargs
                 ) -> None:
                     with MetricsCollector(self._func):
                         if (
-                            sql_stmt := req_sql_n_params(self._func, args, kwargs)
+                            sql_stmt := req_sql_n_params(
+                                self._func, args, kwargs, sync_session
+                            )
                         ) is not None:
                             session.execute(sql_stmt)
                             _commit_if_needed(session, sql_stmt, no_commit)
 
             return wrapper(func)
 
         return decorator
```

### Comparing `true_noorm-0.1.0/noorm/sqlite3/__init__.py` & `true_noorm-0.1.1/noorm/sqlite3/__init__.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/noorm/sqlite3/_sqlite3.py` & `true_noorm-0.1.1/noorm/sqlite3/_sqlite3.py`

 * *Files identical despite different names*

### Comparing `true_noorm-0.1.0/pyproject.toml` & `true_noorm-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "true-noorm"
 packages = [{ include = "noorm" }]
-version = "0.1.0"
+version = "0.1.1"
 description = "NoORM (Not only ORM) - make your database operations convenient and natural"
 authors = ["Alexander Maslyeav <maslyaev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/amaslyaev/noorm/"
 repository = "https://github.com/amaslyaev/noorm/"
 documentation = ""
```

### Comparing `true_noorm-0.1.0/setup.py` & `true_noorm-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'noorm.sqlite3']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'true-noorm',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'NoORM (Not only ORM) - make your database operations convenient and natural',
     'long_description': '[![PyPI pyversions](https://img.shields.io/pypi/pyversions/true-noorm.svg)](https://pypi.python.org/pypi/true-noorm/)\n[![PyPI status](https://img.shields.io/pypi/status/true-noorm.svg)](https://pypi.python.org/pypi/true-noorm/)\n[![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/amaslyaev/noorm/blob/master/LICENSE)\n[![codecov](https://codecov.io/gh/amaslyaev/noorm/graph/badge.svg?token=31YWXNHPMM)](https://codecov.io/gh/amaslyaev/noorm)\n[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black/)\n\n## noorm\n\nNoORM (Not only ORM) - make your database operations convenient and natural\n\n## Install\n\n**noorm** requires Python 3.10 or newer. Install it from PyPI:\n```shell\n$ pip install true-noorm\n```\nPlease note that the correct name is "**true**-noorm".\n\n## NoORM principles\n\n1. It is not a holy war against ORM but "in addition to".\n2. It is not one more "finally perfect" ORM. It is not an ORM at all. **No persistent objects, no "ideal" entities.**\n3. It should be good for for medium-sized and big project.\n4. Focus on developer experience.\n5. Not only a set of helpers to write less code, but first of all, an approach that guides to more understandable, performant, scalable, robust, and maintainable solutions.\n\n## Usage\n\nImpotring `noorm` depends on DB you use in your project. Available options:\n\n- `import noorm.sqlite3 as nm` – for SQLite\n- `import noorm.aiosqlite as nm` – for asynchronous SQLite via **aiosqlite**\n- `import noorm.psycopg2 as nm` – for synchronous Postgres via **psycopg2**\n- `import noorm.asyncpg as nm` – for asynchronous Postgres via **asyncpg**\n- `import noorm.pymysql as nm` – for synchronous MySQL/MariaDB via **PyMySQL**\n- `import noorm.aiomysql as nm` – for asynchronous MySQL/MariaDB via **aiomysql**\n- `import noorm.sqlalchemy_sync as nm` – for synchronous **SqlAlchemy**\n- `import noorm.sqlalchemy_async as nm` – for asynchronous **SqlAlchemy**\n\nYes, using the SqlAlchemy ORM through NoORM is a nice idea.\n\nAfter importing "nm" you use `@nm.sql_...` decorators to create functions that perform database operations. All other your application code uses these functions as a so-called "DB API layer". The decorators are:\n- **@nm.sql_fetch_all** – to make a query and produce a list of objects of specified type. The query is usually SELECT, but it is also useful with data manipulations RETURNING data.\n- **@nm.sql_one_or_none** – to make a query and produce one object or None if nothing is found.\n- **@nm.sql_scalar_or_none** – to get a scalar or None if nothing is found.\n- **@nm.sql_fetch_scalars** – to get a list of scalars.\n- **@nm.sql_execute** – to execute something, usually INSERT, UPDATE, or DELETE.\n\nUsage of these decorators in different submodules and underlying databases might have own peculiarities, so check docstring documentation of the chosen "nm".\n\n#### Example for SQLite through the sqlite3 standard library\n\nAssume we have a **users** table with fields:\n- Integer `id` (`rowid` in SQLite)\n- String `username`\n- String `email`\n\nAnd an **orders** table:\n- Integer `id` (`rowid` in SQLite)\n- Integer `user_id` references to user id\n- Datetime `order_date` (TEXT in SQLite)\n- Decimal `amount` (TEXT in SQLite)\n\n```python\nfrom dataclasses import dataclass\nfrom decimal import Decimal\nfrom datetime import datetime\nimport sqlite3\nimport noorm.sqlite3 as nm\n\n@dataclass\nclass DbUser:  # When we need only basic info. Not a "model"! Just a dataclass!\n    id: int\n    username: str\n    email: str\n\n@nm.sql_fetch_all(DbUser, "SELECT rowid AS id, username, email FROM users")\ndef get_all_users():\n    pass  # no parameters, so just "pass"\n\n@nm.sql_one_or_none(\n    DbUser, "SELECT rowid AS id, username, email FROM users WHERE rowid = :id"\n)\ndef get_user_by_id(id_: int):\n    return nm.params(id=id_)\n\n@dataclass\nclass DbUserWithOrdersSummary:  # With additional info from `orders` table\n    id: int\n    username: str\n    sum_orders: Decimal | None  # SQLite noorm can make decimal out of TEXT\n    first_order: datetime | None  # and datatime too.\n    last_order: datetime | None\n\n@nm.sql_fetch_all(\n    DbUserWithOrdersSummary,\n    """SELECT\n        u.rowid AS id, u.username,\n        SUM(o.amount) AS sum_orders,\n        MIN(o.order_date) AS first_order, MAX(o.order_date) AS last_order\n    FROM users u\n        LEFT OUTER JOIN orders o ON o.user_id = u.rowid\n    GROUP BY u.rowid, u.username ORDER BY u.rowid\n    """,\n)\ndef get_users_with_order_summary():\n    pass\n\ndef main():\n    with sqlite3.connect("data.sqlite") as conn:\n        # will use our DB API functions\n        for usr in get_all_users(conn):\n            print(usr)\n\n        print(f"{get_user_by_id(conn, 1)=}")\n\n        for usr_summary in get_users_with_order_summary(conn):\n            print(usr_summary)\n```\n\n#### Example for SQLite through SqlAlchemy\n\nWill use asynchronous version of SqlAlchemy "nm".\n```python\nimport sqlalchemy as sa\nfrom sqlalchemy.ext.asyncio import create_async_engine, AsyncSession\nimport noorm.sqlalchemy_async as nm\n...\n\n@nm.sql_fetch_all(DbUser)\ndef get_all_users():  # Notice no "async"\n    return sa.select(User.id, User.username, User.email)\n\n@nm.sql_one_or_none(DbUser)\ndef get_user_by_id(id_: int):\n    return sa.select(User.id, User.username, User.email).where(User.id == id_)\n\n@nm.sql_fetch_all(DbUserWithOrdersSummary)\ndef get_users_with_order_summary():\n    return (\n        sa.select(\n            User.id,\n            User.username,\n            sa.func.sum(Order.amount).label("sum_orders"),\n            sa.func.min(Order.order_date).label("first_order"),\n            sa.func.max(Order.order_date).label("last_order"),\n        )\n        .select_from(User)  # `User` and `Order` are ORM model classes\n        .outerjoin(Order, Order.user_id == User.id)\n        .group_by(User.id)\n        .order_by(User.id)\n    )\n\nasync def main():\n    engine = create_async_engine("sqlite+aiosqlite:///data.sqlite")\n    async with AsyncSession(engine) as session:\n        for usr in await get_all_users(session):  # Notice "await"\n            print(usr)\n\n        print(f"user_1={await get_user_by_id(session, 1)}")\n\n        for usr_summary in await get_users_with_order_summary(session):\n            print(usr_summary)\n```\n\n## Suggestions\n\n1. Code structure:\n   - Avoid scattering DB API functions throughout the codebase. It\'s preferable to consolidate them in dedicated locations.\n   - For small applications, consider housing all DB API functions in a single module, which becomes the DB API layer.\n   - In larger applications, dividing the DB API layer into multiple modules is advisable. For example, organize user management functions in `db_api/users.py` and order processing functions in `db_api/orders.py`.\n   - For systems with distinct, independent subsystems, consider placing common functions in a shared location, such as the `db/db_api/` folder, and specific functions in subsystem folders like `external_api/db_api/`.\n   - Declare the "Db..." dataclasses immediately preceding the functions that produce them.\n2. Naming:\n   - Prefix classes returned from DB API functions with "Db". For instance, use "DbUsers", "DbOrders", "DbOrdersWithDetails", "DbInvoicesReportLine".\n   - Prefix functions that SELECT data from the DB with "get_". For example, "get_user_by_id", "get_orders_by_user", etc.\n   - For data manipulation functions:\n     - Use prefixes "ins_", "upd_", "del_" for INSERTs, UPDATEs, DELETEs respectively.\n     - Employ "upsert_" for upsert operations.\n\n## Advanced features\n\n#### Cancelling operations\n\nIf, for any reason, you need to terminate execution and produce a default result in your function, raise the `nm.CancelExecException` exception. Example:\n```python\n@nm.sql_fetch_all(DbOrder)\ndef get_orders_by_ids(order_ids: list[int]):\n    if not order_ids:\n        raise nm.CancelExecException\n    return select(Order.id, Order.date, Order.amount).where(\n        Order.id.in_(order_ids)  # <<< empty list is not acceptable here\n    )\n```\nThe `nm.CancelExecException` triggers production of a default empty result without querying the DB:\n- `@nm.sql_fetch_all` and `@nm.sql_fetch_scalars` return an empty list\n- `@nm.sql_one_or_none` and `@nm.sql_scalar_or_none` return None\n- `@nm.sql_execute` takes no action\n\n#### Registry\n\nObservability is crucial. This library facilitates collecting statistics on DB API function usage out of the box. Statistics include:\n- **calls** – number of calls\n- **duration** – total execution time\n- **tuples** – total number of retrieved tuples\n- **fails** – number of failed calls\n- **fails_by_error** – dict[str, int] – detailed fails categorized by exception types\n```python\nfrom noorm.registry import get_registry\nregistry = get_registry()\nstat = registry.stat_by_name["db.db_api.orders.get_orders_by_user"]\nprint(stat)  # Stat(calls=3, duration=0.0324, tuples=11, fails=0, fails_by_error={})\n```\nTo collect statistics in a multiprocessing application, initialize this option in your MainProcess:\n```python\n# Example for uvicorn\nimport uvicorn\nfrom noorm.registry import get_registry\n\nasync def app(scope, receive, send):\n    ...\n\nif __name__ == "__main__":\n    get_registry().init_multiprocess_registry()  # <<< here\n    uvicorn.run("main:app", port=5000, workers=3, log_level="info")\n```\nConsequently, all DB operations occurring in child processes will be aggregated in the MainProcess registry.\n\n#### Executing unwrapped functions\n\nTo call an unwrapped version of a DB API function for evaluation, testing, or debugging purposes:\n```python\norders_list = await get_orders_by_user(session, 1)  # A "normal" call\norders_list_q = get_orders_by_user.unwrapped(1)  # An "unwrapped" call\nprint(str(orders_list_q.compile()))  # Want to see a compiled SqlAlchemy "SELECT ..."\n```\n\n## Acknowledgements\n\nInspired and sponsored by [FRAMEN](https://www.framen.com/)\n',
     'author': 'Alexander Maslyeav',
     'author_email': 'maslyaev@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/amaslyaev/noorm/',
```

### Comparing `true_noorm-0.1.0/PKG-INFO` & `true_noorm-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: true-noorm
-Version: 0.1.0
+Version: 0.1.1
 Summary: NoORM (Not only ORM) - make your database operations convenient and natural
 Home-page: https://github.com/amaslyaev/noorm/
 License: MIT
 Keywords: database,sql,orm,noorm,sqlite,postgres,postgresql,mysql
 Author: Alexander Maslyeav
 Author-email: maslyaev@gmail.com
 Requires-Python: >=3.10,<4.0
```

