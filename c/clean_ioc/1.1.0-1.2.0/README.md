# Comparing `tmp/clean_ioc-1.1.0.tar.gz` & `tmp/clean_ioc-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_ioc-1.1.0.tar", max compression
+gzip compressed data, was "clean_ioc-1.2.0.tar", max compression
```

## Comparing `clean_ioc-1.1.0.tar` & `clean_ioc-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     4195 2024-05-12 00:53:43.029482 clean_ioc-1.1.0/CHANGES.rst
--rw-r--r--   0        0        0     1067 2024-05-12 00:53:43.029482 clean_ioc-1.1.0/LICENSE
--rw-r--r--   0        0        0    20278 2024-05-12 00:53:43.029482 clean_ioc-1.1.0/README.md
--rw-r--r--   0        0        0       20 2024-05-12 00:53:43.029482 clean_ioc-1.1.0/clean_ioc/__init__.py
--rw-r--r--   0        0        0     2118 2024-05-12 00:53:43.029482 clean_ioc-1.1.0/clean_ioc/bundles.py
--rw-r--r--   0        0        0    62448 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/core.py
--rw-r--r--   0        0        0       20 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/ext/fastapi/__init__.py
--rw-r--r--   0        0        0     1909 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/ext/fastapi/core.py
--rw-r--r--   0        0        0     1255 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/ext/fastapi/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/ext/fastapi/py.typed
--rw-r--r--   0        0        0     1262 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/factories.py
--rw-r--r--   0        0        0     2662 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/functional_utils.py
--rw-r--r--   0        0        0      563 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/list_reduction_filters.py
--rw-r--r--   0        0        0     1779 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/node_filters.py
--rw-r--r--   0        0        0        0 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/py.typed
--rw-r--r--   0        0        0     4807 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/registration_filters.py
--rw-r--r--   0        0        0      962 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/type_filters.py
--rw-r--r--   0        0        0     6920 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/typing_utils.py
--rw-r--r--   0        0        0     1828 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/utils.py
--rw-r--r--   0        0        0      564 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/value_factories.py
--rw-r--r--   0        0        0     2146 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    21058 1970-01-01 00:00:00.000000 clean_ioc-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4195 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/CHANGES.rst
+-rw-r--r--   0        0        0     1067 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/LICENSE
+-rw-r--r--   0        0        0    17357 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/README.md
+-rw-r--r--   0        0        0       20 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/__init__.py
+-rw-r--r--   0        0        0     2118 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/bundles.py
+-rw-r--r--   0        0        0    62229 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/core.py
+-rw-r--r--   0        0        0       20 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/ext/fastapi/__init__.py
+-rw-r--r--   0        0        0     2259 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/ext/fastapi/core.py
+-rw-r--r--   0        0        0     1344 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/ext/fastapi/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/ext/fastapi/py.typed
+-rw-r--r--   0        0        0     1262 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/factories.py
+-rw-r--r--   0        0        0     2662 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/functional_utils.py
+-rw-r--r--   0        0        0      563 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/list_reduction_filters.py
+-rw-r--r--   0        0        0     1779 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/node_filters.py
+-rw-r--r--   0        0        0        0 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/py.typed
+-rw-r--r--   0        0        0     4807 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/registration_filters.py
+-rw-r--r--   0        0        0      962 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/type_filters.py
+-rw-r--r--   0        0        0     6920 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/typing_utils.py
+-rw-r--r--   0        0        0     1828 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/utils.py
+-rw-r--r--   0        0        0      564 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/value_factories.py
+-rw-r--r--   0        0        0     2243 2024-05-13 23:05:42.588916 clean_ioc-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    18211 1970-01-01 00:00:00.000000 clean_ioc-1.2.0/PKG-INFO
```

### Comparing `clean_ioc-1.1.0/CHANGES.rst` & `clean_ioc-1.2.0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/LICENSE` & `clean_ioc-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/README.md` & `clean_ioc-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: clean_ioc
+Version: 1.2.0
+Summary: An IOC Container for Python 3.10+
+Home-page: https://peter-daly.github.io/clean_ioc/
+License: MIT
+Keywords: dependency,injection,ioc,inversion of control,type,hints,typing
+Author: Peter Daly
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: fastapi
+Requires-Dist: fastapi (>=0.101.0,<0.102.0) ; extra == "fastapi"
+Project-URL: Documentation, https://peter-daly.github.io/clean_ioc/
+Project-URL: Repository, https://github.com/peter-daly/clean_ioc
+Description-Content-Type: text/markdown
+
 # Clean IoC
 A simple dependency injection library for python that requires nothing of your application code (except that you use typing).
 
 
 ## Basic Registering and resolving
 
 There are 4 basic modes of registering a new set of classes
@@ -373,76 +394,14 @@
 h2 = container.resolve(CommandHandler[GoodbyeCommand])
 
 h1.handle(HelloCommand()) # prints 'A VERY BIG\nHELLO'
 h2.handle(GoodbyeCommand()) # prints 'A VERY BIG\nGOODBYE'
 
 ```
 
-## Scopes
-Scopes are a machanism where you guarantee that dependency can be temporarily a singleton within the scope. You can also register dependencies that that are only available withon the scope.
-Some good use cases for scope lifetimes are:
- - http request in a web server
- - message/event if working on a message based system
-For instance you could keep an single database connection open for the entire lifetime of the http request
-
-```python
-class DbConnection:
-    def run_sql(self, statement):
-        # Done some sql Stuff
-        pass
-
-container.register(DbConnection, lifespan=Lifespan.scoped)
-
-with container.get_scope() as scope:
-    db_conn = scope.resolve(DbConnection)
-    db_conn.run_sql("UPDATE table SET column = 1")
-```
-
-Scopes can also be use with asyncio
-
-```python
-class AsyncDbConnection:
-    async def run_sql(self, statement):
-        # Done some sql Stuff
-        pass
-
-container.register(AsyncDbConnection, lifespan=Lifespan.scoped)
-
-async with container.get_scope() as scope:
-    db_conn = scope.resolve(AsyncDbConnection)
-    await db_conn.run_sql("UPDATE table SET column = 1")
-```
-
-
-### Scoped Teardowns
-When you are finished with some dependenies within a scope you might want to perform some teardown action before you exit the scope. For example if we want to close our db connection.
-
-```python
-class AsyncDbConnection:
-    async def run_sql(self, statement):
-        # Done some sql Stuff
-        pass
-    async def close(self):
-        # Close the connection
-        pass
-
-async def close_connection(conn: AsyncDbConnection):
-    await conn.close()
-
-container.register(DbConnection, lifespan=Lifespan.scoped, scoped_teardown=close_connection)
-
-async with container.get_scope() as scope:
-    db_conn = scope.resolve(AsyncDbConnection)
-    await db_conn.run_sql("UPDATE table SET column = 1")
-
-# close connection is run when we exit the scope
-```
-
-***Note***: *When using the scope as an async context manager you need both sync and async teardowns are run, when a scope is used as a normal sync context manager async teardowns are ignored*
-
 
 ## Named registrations & Registration filters
 
 By default the last unnamed registration is what the container will return when resolve is called as below.
 
 ```python
 
@@ -788,41 +747,11 @@
 container = Container()
 container.register(Client)
 container.register(logging.Logger, factory=logger_fac, lifespan=Lifespan.transient)
 client = container.resolve(Client)
 ```
 
 ***Note*** *If using dependency context on your dependency it's recommended that you use a lifespan of **transient**, because any other lifespan will create only use the parent of the first resolved instance*
-## Pre-configurations
-
-Pre configurations run a side-effect for a type before the type gets resolved.
-This is useful if some python modules have some sort of module level functions that need to be called before the object get created
 
-```python
-import logging
-
-class Client:
-    def __init__(self, logger: logging.Logger):
-        self.logger = logger
 
-    def do_a_thing(self):
-        self.logger.info('Doing a thing')
 
-def logger_fac(context: DependencyContext):
-    module = context.parent.implementation.__module__
-    return logging.getLogger(module)
-
-def configure_logging():
-    logging.basicConfig()
-
-
-
-
-container = Container()
-container.register(Client)
-container.register(logging.Logger, factory=logger_fac, lifespan=Lifespan.transient)
-container.pre_configure(logging.Logger, configure_logging)
-
-client = container.resolve(Client)
-
-
-```
+```
```

### Comparing `clean_ioc-1.1.0/clean_ioc/bundles.py` & `clean_ioc-1.2.0/clean_ioc/bundles.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/clean_ioc/core.py` & `clean_ioc-1.2.0/clean_ioc/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1040,19 +1040,21 @@
         lifespan: Lifespan,
         name: str | None,
         dependency_config: DependencyConfig,
         tags: Iterable[Tag] | None,
         parent_node_filter: NodeFilter,
         scoped_teardown: Callable[[TService], Any] | None,
     ):
+        instance_lifespan = lifespan if lifespan == Lifespan.singleton else Lifespan.scoped
+
         registration = _Registration(
             activator_class=FactoryActivator,
             service_type=service_type,
             implementation=constant(instance),
-            lifespan=lifespan,
+            lifespan=instance_lifespan,
             name=name,
             dependency_config=dependency_config,
             parent_node_filter=parent_node_filter,
             scoped_teardown=scoped_teardown,
             tags=tags,
         )
         self._registrations[service_type].appendleft(registration)
@@ -1308,18 +1310,14 @@
         self._generator_finalizers: deque[Callable] = deque()
 
         self.register(ScopeCreator, instance=self)
         self.register(Resolver, instance=self)
         self.register(Registrator, instance=self)
         self.register(Scope, instance=self)
 
-    @classmethod
-    def _instance_lifespan(cls):
-        raise NotImplementedError("Scope._instance_lifespan")
-
     def resolve(
         self,
         service_type: type[TService],
         filter: RegistrationFilter = default_registration_filter,
     ) -> TService:
         graph = self.resolve_dependency_graph(service_type, filter)
         return graph.instance
@@ -1368,15 +1366,15 @@
         parent_node_filter: NodeFilter = default_parent_node_filter,
         scoped_teardown: Callable[[TService], Any] | None = None,
     ):
         if instance is not None:
             self._registry.register_instance(
                 service_type=service_type,
                 instance=instance,
-                lifespan=self._instance_lifespan(),
+                lifespan=lifespan,
                 name=name,
                 tags=tags,
                 dependency_config=dependency_config,
                 parent_node_filter=parent_node_filter,
                 scoped_teardown=scoped_teardown,
             )
         elif factory is not None:
@@ -1541,18 +1539,14 @@
 
 
 class ChildScope(Scope):
     def __init__(self, parent_scope: Scope):
         super().__init__()
         self._parent_scope = parent_scope
 
-    @classmethod
-    def _instance_lifespan(cls) -> Lifespan:
-        return Lifespan.scoped
-
     def add_singleton_node(self, registration: _Registration, node: DependencyNode):
         self._parent_scope.add_singleton_node(registration, node)
 
     def find_singleton_node(self, registration_id: str) -> DependencyNode | None:
         return self._parent_scope.find_singleton_node(registration_id)
 
     def find_scoped_node(self, registration_id: str) -> DependencyNode | None:
@@ -1616,18 +1610,14 @@
 
 class Container(Scope):
     def __init__(self):
         super().__init__()
         self._singletons: dict[str, DependencyNode] = {}
         self.register(Container, instance=self)
 
-    @classmethod
-    def _instance_lifespan(cls) -> Lifespan:
-        return Lifespan.singleton
-
     def register_subclasses(
         self,
         base_type: type,
         *,
         lifespan: Lifespan = Lifespan.once_per_graph,
         subclass_type_filter: Callable[[type], bool] = always_true,
         name: str | None = None,
```

### Comparing `clean_ioc-1.1.0/clean_ioc/ext/fastapi/core.py` & `clean_ioc-1.2.0/clean_ioc/ext/fastapi/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,50 @@
+import logging
+from contextlib import asynccontextmanager
 from typing import Annotated, AsyncGenerator
 
 from clean_ioc.core import (
     Container,
     RegistrationFilter,
     Scope,
     TService,
     default_registration_filter,
 )
 from fastapi import Depends, FastAPI, Request, params
 
+logger = logging.getLogger(__name__)
 
-def add_container_to_app(app: FastAPI, container: Container):
+
+@asynccontextmanager
+async def add_container_to_app(app: FastAPI, container: Container):
     """
     Adds a container to the given FastAPI app.
 
     Args:
         app (FastAPI): The FastAPI app to add the container to.
         container (Container): The container to be added.
     """
-    add_root_scope_to_app(app, container)
+    async with add_root_scope_to_app(app, container):
+        yield
 
 
-def add_root_scope_to_app(app: FastAPI, root_scope: Scope):
+@asynccontextmanager
+async def add_root_scope_to_app(app: FastAPI, root_scope: Scope):
     """
     Adds the root scope to the given FastAPI app.
 
     Args:
         app (FastAPI): The FastAPI app to add the container to.
         root_scope (Scope): The scope to be added.
     """
-    app.state.root_scope = root_scope
+    async with root_scope:
+        logger.debug("adding root scope to the fast api app")
+        app.state.root_scope = root_scope
+        yield
+        logger.debug("releasing root scope from the fast api app")
 
 
 def get_root_scope_from_app(app: FastAPI) -> Scope:
     return app.state.root_scope
 
 
 async def get_scope(
```

### Comparing `clean_ioc-1.1.0/clean_ioc/ext/fastapi/dependencies.py` & `clean_ioc-1.2.0/clean_ioc/ext/fastapi/dependencies.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,19 +22,23 @@
     def __init__(self, response: Response):
         self.response = response
 
     def write(self, key: str, value: str):
         self.response.headers[key] = value
 
 
-def _add_request_header_reader_to_scope(request: Request, scope: Scope = Depends(get_scope)):
+def add_request_to_scope(request: Request, scope: Scope = Depends(get_scope)):
+    scope.register(Request, instance=request)
+
+
+def add_response_to_scope(response: Response, scope: Scope = Depends(get_scope)):
+    scope.register(Response, instance=response)
+
+
+def add_request_header_reader_to_scope(request: Request, scope: Scope = Depends(get_scope)):
     reader = RequestHeaderReader(request)
     scope.register(RequestHeaderReader, instance=reader)
 
 
-def _add_response_header_writer_to_scope(response: Response, scope: Scope = Depends(get_scope)):
+def add_response_header_writer_to_scope(response: Response, scope: Scope = Depends(get_scope)):
     writer = ResponseHeaderWriter(response)
     scope.register(ResponseHeaderWriter, instance=writer)
-
-
-add_request_header_reader_to_scope = Depends(_add_request_header_reader_to_scope)
-add_response_header_writer_to_scope = Depends(_add_response_header_writer_to_scope)
```

### Comparing `clean_ioc-1.1.0/clean_ioc/factories.py` & `clean_ioc-1.2.0/clean_ioc/factories.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/clean_ioc/functional_utils.py` & `clean_ioc-1.2.0/clean_ioc/functional_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/clean_ioc/list_reduction_filters.py` & `clean_ioc-1.2.0/clean_ioc/list_reduction_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/clean_ioc/node_filters.py` & `clean_ioc-1.2.0/clean_ioc/node_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/clean_ioc/registration_filters.py` & `clean_ioc-1.2.0/clean_ioc/registration_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/clean_ioc/type_filters.py` & `clean_ioc-1.2.0/clean_ioc/type_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/clean_ioc/typing_utils.py` & `clean_ioc-1.2.0/clean_ioc/typing_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/clean_ioc/utils.py` & `clean_ioc-1.2.0/clean_ioc/utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/clean_ioc/value_factories.py` & `clean_ioc-1.2.0/clean_ioc/value_factories.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.1.0/pyproject.toml` & `clean_ioc-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "clean_ioc"
-version = "1.1.0"
+version = "1.2.0"
 description = "An IOC Container for Python 3.10+"
 authors = ["Peter Daly"]
 license = "MIT"
 homepage = "https://peter-daly.github.io/clean_ioc/"
 repository = "https://github.com/peter-daly/clean_ioc"
 documentation = "https://peter-daly.github.io/clean_ioc/"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
 ]
+keywords = ["dependency", "injection", "ioc", "inversion of control", "type", "hints", "typing"]
 packages = [
     { include = "clean_ioc" },
 ]
 include = ["CHANGES.rst", "clean_ioc/py.typed", "clean_ioc/ext/fastapi/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `clean_ioc-1.1.0/PKG-INFO` & `clean_ioc-1.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: clean_ioc
-Version: 1.1.0
-Summary: An IOC Container for Python 3.10+
-Home-page: https://peter-daly.github.io/clean_ioc/
-License: MIT
-Author: Peter Daly
-Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: fastapi
-Requires-Dist: fastapi (>=0.101.0,<0.102.0) ; extra == "fastapi"
-Project-URL: Documentation, https://peter-daly.github.io/clean_ioc/
-Project-URL: Repository, https://github.com/peter-daly/clean_ioc
-Description-Content-Type: text/markdown
-
 # Clean IoC
 A simple dependency injection library for python that requires nothing of your application code (except that you use typing).
 
 
 ## Basic Registering and resolving
 
 There are 4 basic modes of registering a new set of classes
@@ -393,76 +373,14 @@
 h2 = container.resolve(CommandHandler[GoodbyeCommand])
 
 h1.handle(HelloCommand()) # prints 'A VERY BIG\nHELLO'
 h2.handle(GoodbyeCommand()) # prints 'A VERY BIG\nGOODBYE'
 
 ```
 
-## Scopes
-Scopes are a machanism where you guarantee that dependency can be temporarily a singleton within the scope. You can also register dependencies that that are only available withon the scope.
-Some good use cases for scope lifetimes are:
- - http request in a web server
- - message/event if working on a message based system
-For instance you could keep an single database connection open for the entire lifetime of the http request
-
-```python
-class DbConnection:
-    def run_sql(self, statement):
-        # Done some sql Stuff
-        pass
-
-container.register(DbConnection, lifespan=Lifespan.scoped)
-
-with container.get_scope() as scope:
-    db_conn = scope.resolve(DbConnection)
-    db_conn.run_sql("UPDATE table SET column = 1")
-```
-
-Scopes can also be use with asyncio
-
-```python
-class AsyncDbConnection:
-    async def run_sql(self, statement):
-        # Done some sql Stuff
-        pass
-
-container.register(AsyncDbConnection, lifespan=Lifespan.scoped)
-
-async with container.get_scope() as scope:
-    db_conn = scope.resolve(AsyncDbConnection)
-    await db_conn.run_sql("UPDATE table SET column = 1")
-```
-
-
-### Scoped Teardowns
-When you are finished with some dependenies within a scope you might want to perform some teardown action before you exit the scope. For example if we want to close our db connection.
-
-```python
-class AsyncDbConnection:
-    async def run_sql(self, statement):
-        # Done some sql Stuff
-        pass
-    async def close(self):
-        # Close the connection
-        pass
-
-async def close_connection(conn: AsyncDbConnection):
-    await conn.close()
-
-container.register(DbConnection, lifespan=Lifespan.scoped, scoped_teardown=close_connection)
-
-async with container.get_scope() as scope:
-    db_conn = scope.resolve(AsyncDbConnection)
-    await db_conn.run_sql("UPDATE table SET column = 1")
-
-# close connection is run when we exit the scope
-```
-
-***Note***: *When using the scope as an async context manager you need both sync and async teardowns are run, when a scope is used as a normal sync context manager async teardowns are ignored*
-
 
 ## Named registrations & Registration filters
 
 By default the last unnamed registration is what the container will return when resolve is called as below.
 
 ```python
 
@@ -808,41 +726,11 @@
 container = Container()
 container.register(Client)
 container.register(logging.Logger, factory=logger_fac, lifespan=Lifespan.transient)
 client = container.resolve(Client)
 ```
 
 ***Note*** *If using dependency context on your dependency it's recommended that you use a lifespan of **transient**, because any other lifespan will create only use the parent of the first resolved instance*
-## Pre-configurations
-
-Pre configurations run a side-effect for a type before the type gets resolved.
-This is useful if some python modules have some sort of module level functions that need to be called before the object get created
 
-```python
-import logging
-
-class Client:
-    def __init__(self, logger: logging.Logger):
-        self.logger = logger
 
-    def do_a_thing(self):
-        self.logger.info('Doing a thing')
 
-def logger_fac(context: DependencyContext):
-    module = context.parent.implementation.__module__
-    return logging.getLogger(module)
-
-def configure_logging():
-    logging.basicConfig()
-
-
-
-
-container = Container()
-container.register(Client)
-container.register(logging.Logger, factory=logger_fac, lifespan=Lifespan.transient)
-container.pre_configure(logging.Logger, configure_logging)
-
-client = container.resolve(Client)
-
-
-```
+```
```

