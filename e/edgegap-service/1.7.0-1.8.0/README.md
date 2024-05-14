# Comparing `tmp/edgegap_service-1.7.0.tar.gz` & `tmp/edgegap_service-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-1.7.0.tar", max compression
+gzip compressed data, was "edgegap_service-1.8.0.tar", max compression
```

## Comparing `edgegap_service-1.7.0.tar` & `edgegap_service-1.8.0.tar`

### file list

```diff
@@ -1,27 +1,24 @@
--rw-r--r--   0        0        0     1993 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/LICENSE
--rw-r--r--   0        0        0     2188 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/README.md
--rw-r--r--   0        0        0       17 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/BUILD
--rw-r--r--   0        0        0      291 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2931 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      735 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      717 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2951 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     8268 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/_service.py
--rw-r--r--   0        0        0     1019 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/_templating.py
--rw-r--r--   0        0        0       17 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/health/BUILD
--rw-r--r--   0        0        0      102 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/health/_model.py
--rw-r--r--   0        0        0       17 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/health/checks/BUILD
--rw-r--r--   0        0        0      300 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      577 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0      152 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/logging/__init__.py
--rw-r--r--   0        0        0     2135 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/logging/_configuration.py
--rw-r--r--   0        0        0     1657 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/logging/_logger.py
--rw-r--r--   0        0        0     1880 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0     4286 2024-05-07 13:27:48.731497 edgegap_service-1.7.0/edgegap_service/static/images/favicon.ico
--rw-r--r--   0        0        0      990 2024-05-07 13:28:05.115637 edgegap_service-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/LICENSE
+-rw-r--r--   0        0        0     2188 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/README.md
+-rw-r--r--   0        0        0      291 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     3206 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      735 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      717 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2951 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     8444 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/_service.py
+-rw-r--r--   0        0        0     1019 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/_templating.py
+-rw-r--r--   0        0        0      102 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0      300 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      577 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0      152 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/logging/__init__.py
+-rw-r--r--   0        0        0     2135 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/logging/_configuration.py
+-rw-r--r--   0        0        0     1657 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/logging/_logger.py
+-rw-r--r--   0        0        0     1880 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-05-14 17:37:22.051682 edgegap_service-1.8.0/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      990 2024-05-14 17:37:30.243746 edgegap_service-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.8.0/PKG-INFO
```

### Comparing `edgegap_service-1.7.0/LICENSE` & `edgegap_service-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/README.md` & `edgegap_service-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/_configuration.py` & `edgegap_service-1.8.0/edgegap_service/_configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import os
-from typing import Callable, Optional
+from typing import Callable, Optional, TypeVar
 
 from edgegap_scheduling import Scheduler
 from edgegap_settings import ProjectBaseSettings, SettingsFactory
 from fastapi import APIRouter
 from pydantic import BaseModel, ConfigDict, Field
 from pydantic_settings import BaseSettings
+from starlette.types import ExceptionHandler
 
 from ._environment import EnvironmentConfiguration
 from .health.checks import CheckInterface
 from .logging import LoggingConfiguration
 
+Exc = TypeVar('Exc', bound=Exception)
+
 
 def get_default_root_dir() -> str:
     return os.getcwd()
 
 
 class ServiceConfiguration(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     name: str = Field(..., description='The name of the Service')
     version: str = Field(..., description='The version of the Service')
     description: str = Field(..., description='The description of the Service')
     routers: list[APIRouter] = Field([], description='The FastAPI routers')
+    exception_handlers: list[tuple[type[Exc], ExceptionHandler]] = Field(
+        default_factory=list,
+        description='The Exception Handlers to add to the FastAPI App',
+    )
     root_dir: str = Field(default_factory=get_default_root_dir, description='The Root Directory of the Service')
     static_dir: str = Field(default='static', description='The Static Directory of the Service')
     html_index_path: str | None = Field(default=None, description='The full path to the html index file')
     checks: list[type(CheckInterface)] = Field([], description='The list of Checks to run on the Service')
     depend: Optional[Callable] = Field(default=None, description='The Base Depend Attribute for DB Session')
     port: int = Field(default=8000, description='The Port of the Service')
     host: str = Field(default='0.0.0.0', description='The Host of the Service')
```

### Comparing `edgegap_service-1.7.0/edgegap_service/_documentation.py` & `edgegap_service-1.8.0/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/_environment.py` & `edgegap_service-1.8.0/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/_scheduling.py` & `edgegap_service-1.8.0/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/_service.py` & `edgegap_service-1.8.0/edgegap_service/_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,17 @@
         )
 
         Path(self.__static_folder).mkdir(parents=True, exist_ok=True)
 
         for router in self.__configuration.routers:
             self.__app.include_router(router)
 
+        for exception_class, handler in self.__configuration.exception_handlers:
+            self.__app.add_exception_handler(exception_class, handler)
+
         self.__app.mount(
             '/static',
             staticfiles.StaticFiles(
                 directory=self.__static_folder,
                 packages=[('edgegap_service', 'static')],
             ),
             name='static',
@@ -106,16 +109,16 @@
         self.__init_logstash()
 
         dictConfig(self.__configuration.log_config.model_dump())
         logger = logging.getLogger(self.__configuration.name)
         logger.info(f'Logging for service {Format.squared(self.__configuration.name, Color.GREEN)} is configured')
 
         if (
-            isinstance(self.__configuration.settings, ProjectBaseSettings)
-            and self.__configuration.settings.logstash.enabled
+                isinstance(self.__configuration.settings, ProjectBaseSettings)
+                and self.__configuration.settings.logstash.enabled
         ):
             logger.info('Logstash is enabled')
 
         return logger
 
     def __init_apm(self):
         if isinstance(self.__configuration.settings, ProjectBaseSettings):
@@ -147,16 +150,16 @@
                 }
                 handlers = {
                     'logstash': {
                         'class': 'logstash_async.handler.AsynchronousLogstashHandler',
                         'formatter': 'logstash',
                         'transport': 'logstash_async.transport.TcpTransport',
                         'args': "('%(host)s', %(port)s, '%(database_path)s', '%(transport)s', "
-                        "%(ssl_enable)s, %(ssl_verify)s, '%(keyfile)s', '%(certfile)s', "
-                        "'%(ca_certs)s', %(enable)s)",
+                                "%(ssl_enable)s, %(ssl_verify)s, '%(keyfile)s', '%(certfile)s', "
+                                "'%(ca_certs)s', %(enable)s)",
                         'host': logstash.server,
                         'port': logstash.port,
                         'enable': logstash.enabled,
                         'ssl_enable': False,
                         'ssl_verify': False,
                         'database_path': None,
                     },
@@ -164,15 +167,14 @@
                 self.__configuration.log_config.root['handlers'] = ['default', 'logstash']
                 self.__configuration.log_config.loggers['root']['handlers'] = ['default', 'logstash']
                 self.__configuration.log_config.formatters.update(formatter)
                 self.__configuration.log_config.handlers.update(handlers)
 
     def __init_scheduling(self):
         if isinstance(self.__configuration.scheduler, Scheduler):
-
             @self.__app.on_event('startup')
             def start_scheduling():
                 SchedulingAPI().init_scheduling_api(self.__app)
                 asyncio.create_task(self.__configuration.scheduler.start_all())
 
     def __init_sigterm(self):
         @self.__app.on_event('shutdown')
```

### Comparing `edgegap_service-1.7.0/edgegap_service/_templating.py` & `edgegap_service-1.8.0/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/health/_health.py` & `edgegap_service-1.8.0/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/health/checks/_consul.py` & `edgegap_service-1.8.0/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/health/checks/_database.py` & `edgegap_service-1.8.0/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/health/checks/_interface.py` & `edgegap_service-1.8.0/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/logging/_configuration.py` & `edgegap_service-1.8.0/edgegap_service/logging/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/logging/_logger.py` & `edgegap_service-1.8.0/edgegap_service/logging/_logger.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/static/html/index.html` & `edgegap_service-1.8.0/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/edgegap_service/static/images/favicon.ico` & `edgegap_service-1.8.0/edgegap_service/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.7.0/pyproject.toml` & `edgegap_service-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "1.7.0"
+version = "1.8.0"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-1.7.0/PKG-INFO` & `edgegap_service-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 1.7.0
+Version: 1.8.0
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

