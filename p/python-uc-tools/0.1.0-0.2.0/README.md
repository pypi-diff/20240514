# Comparing `tmp/python_uc_tools-0.1.0.tar.gz` & `tmp/python_uc_tools-0.2.0.tar.gz`

## Comparing `python_uc_tools-0.1.0.tar` & `python_uc_tools-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/test_env.txt
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/src/uc_tools/__about__.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/src/uc_tools/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/src/uc_tools/config/__init__.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/src/uc_tools/config/env.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/src/uc_tools/logger/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/src/uc_tools/redis/__init__.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/src/uc_tools/redis/redis.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/src/uc_tools/tools/__init__.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/src/uc_tools/tools/decode.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/src/uc_tools/tools/retry.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/tests/test_env.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/tests/test_tools.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/README.md
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 python_uc_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/test_env.txt
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/__about__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/config/__init__.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/config/env.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/http_server/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/http_server/routes.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/http_server/server.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/logger/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/redis/__init__.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/redis/redis.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/tools/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/tools/decode.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/src/uc_tools/tools/retry.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/tests/test_env.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/tests/test_server.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/tests/test_tools.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/README.md
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 python_uc_tools-0.2.0/PKG-INFO
```

### Comparing `python_uc_tools-0.1.0/.github/workflows/publish.yml` & `python_uc_tools-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python_uc_tools-0.1.0/src/uc_tools/config/env.py` & `python_uc_tools-0.2.0/src/uc_tools/config/env.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-import os
+from __future__ import annotations
+
 from dataclasses import fields
 from pathlib import Path
-from typing import Type
 
 
 class BaseConfig:
     """
     Abstract base class for the application configuration.
 
     It's used to define the structure of the application configuration
     and validate the environment variables.
     """
 
-    ...
-
 
 class Env:
     @staticmethod
     def find_env(env_name: str) -> Path:
         """
         Find the environment file in the current or root project directory.
         """
@@ -26,23 +24,24 @@
             current_dir / env_name,
             current_dir.parent / env_name,
             current_dir.parent.parent / env_name,
         ]
         for env_file in env_files:
             if env_file.exists():
                 return env_file
+        msg = f'Cannot find {env_name} file in the current or root project directory.'
         raise FileNotFoundError(
-            f"Cannot find {env_name} file in the current or root project directory."
+            msg
         )
 
     @classmethod
     def load(
         cls,
-        env_name: str = ".env",
-        config: Type[BaseConfig] = None,
+        env_name: str = '.env',
+        config: type[BaseConfig] | None = None,
     ) -> BaseConfig:
         """
         Load environment variables from the environment file.
 
         Args:
             environment_file (str | None): The path to the environment file.
 
@@ -51,27 +50,29 @@
 
         Raises:
             ValueError: If a setting is missing or has an invalid type.
         """
         settings_dict: dict[str, str | int] = {}
         env_file = cls.find_env(env_name)
 
-        with Path.open(env_file, "r") as f:
+        with Path.open(env_file, 'r') as f:
             for line in f:
                 stripped_line = line.strip()
-                if stripped_line and not stripped_line.startswith("#"):
-                    key, value = map(str.strip, stripped_line.split("="))
+                if stripped_line and not stripped_line.startswith('#'):
+                    key, value = map(str.strip, stripped_line.split('='))
                     try:
                         value = int(value)
                     except ValueError:
-                        value = value if value else ""
+                        value = value or ''
                     settings_dict[key.lower()] = value
 
         for field in fields(config):
             if field.name.lower() not in settings_dict:
-                raise ValueError(f"Missing setting: {field.name}")
-            if field.type != type(settings_dict[field.name]) and field.type != str:
+                msg = f'Missing setting: {field.name}'
+                raise ValueError(msg)
+            if field.type is not type(settings_dict[field.name]) and field.type is not str:
+                msg = f'Invalid type for setting: {field.name}. Expected {field.type}, got {type(settings_dict[field.name])}'
                 raise ValueError(
-                    f"Invalid type for setting: {field.name}. Expected {field.type}, got {type(settings_dict[field.name])}"
+                    msg
                 )
 
         return config(**settings_dict)
```

### Comparing `python_uc_tools-0.1.0/src/uc_tools/logger/__init__.py` & `python_uc_tools-0.2.0/src/uc_tools/logger/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
-from pathlib import Path
+
 import logging
 from enum import StrEnum
 from logging.handlers import RotatingFileHandler
+from pathlib import Path
 
 
 class LoggingLevel(StrEnum):
-    DEBUG = "DEBUG"
-    INFO = "INFO"
-    WARNING = "WARNING"
-    ERROR = "ERROR"
-    CRITICAL = "CRITICAL"
+    DEBUG = 'DEBUG'
+    INFO = 'INFO'
+    WARNING = 'WARNING'
+    ERROR = 'ERROR'
+    CRITICAL = 'CRITICAL'
 
 
 class FixedLengthFilter(logging.Filter):
     def __init__(self, max_length: int) -> None:
         """Initialize the filter with a maximum length.
 
         Args:
@@ -37,15 +38,15 @@
         return True
 
     @staticmethod
     def limit_string_length(string: str, max_length: int = 100):
         if len(string) <= max_length:
             return string
         half = max_length // 2
-        return string[:half] + "..." + string[-half:]
+        return string[:half] + '...' + string[-half:]
 
 
 def setup_logger(
     name: str,
     file_max_size_bytes: int = 1000000,
     files_count: int = 5,
     log_length: int = 100,
@@ -63,19 +64,19 @@
     Returns:
         logging.Logger: The logger instance.
     """
     logger = logging.getLogger(name)
     logger.setLevel(level)
 
     formatter = logging.Formatter(
-        "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+        '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
     )
 
-    logs_folder = Path(__file__).resolve().parent.parent / "logs"
-    log_file = logs_folder / f"{name}.log"
+    logs_folder = Path(__file__).resolve().parent.parent / 'logs'
+    log_file = logs_folder / f'{name}.log'
     log_file.parent.mkdir(parents=True, exist_ok=True)
     if not log_file.exists():
         log_file.touch()
 
     file_handler = RotatingFileHandler(
         log_file, maxBytes=file_max_size_bytes, backupCount=files_count
     )
```

### Comparing `python_uc_tools-0.1.0/src/uc_tools/redis/redis.py` & `python_uc_tools-0.2.0/src/uc_tools/redis/redis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-import redis
 import json
-from ..logger import setup_logger
+import logging
+
+import redis
 
-logger = setup_logger(__name__)
+logger = logging.getLogger('uc_tools').addHandler(logging.NullHandler())
 
 
 class Redis:
-    def __init__(self, host, port, username="", password="", db=0):
+    def __init__(self, host, port, username='', password='', db=0):
         self.host = host
         self.port = port
         self.db = db
         self.username = username
         self.password = password
         self.client = self.connect()
 
     def connect(self):
-        logger.info(f"Connecting to Redis server at " f"{self.host}:{self.port}...")
+        logger.info(f'Connecting to Redis server at ' f'{self.host}:{self.port}...')
         try:
             client = redis.StrictRedis(
                 host=self.host,
                 port=self.port,
                 db=self.db,
                 username=self.username,
                 password=self.password,
             )
-            logger.info("Connected to Redis server.")
-            return client
+            logger.info('Connected to Redis server.')
         except Exception as e:
-            logger.error(f"Failed to connect to Redis server: {e}")
+            logger.exception(f'Failed to connect to Redis server: {e}')
             raise
+        else:
+            return client
 
     def get(self, key, decode_type=str):
         """
         Get value for key from Redis.
         """
         value = self.client.get(key)
         if value is None:
             return None
-        if decode_type == bytes:
+        if decode_type is bytes:
             return value
         try:
-            return decode_type(value.decode("utf-8"))
+            return decode_type(value.decode('utf-8'))
         except (ValueError, AttributeError):
-            logger.error(f"Failed to decode value for key '{key}'")
+            logger.exception(f"Failed to decode value for key '{key}'")
             raise
 
     def set(self, key, value, ex=-1, encode_type=str):
         """
         Set value for key in Redis.
 
         Args:
@@ -56,34 +58,38 @@
             encode_type: The type to encode the value to.
 
         Returns:
             The result of the set operation.
         """
         logger.info(f"Setting value '{value}' for key '{key}' in Redis...")
         try:
-            if encode_type == str:
+            if encode_type is str:
                 encoded_value = value.encode('utf-8')
-            elif encode_type in [int, float, bool]:
+            elif encode_type in {int, float, bool}:
                 encoded_value = str(value).encode('utf-8')
-            elif encode_type in [list, dict]:
+            elif encode_type in {list, dict}:
                 encoded_value = json.dumps(value)
             else:
-                raise ValueError("Unsupported encode_type")
+                msg = 'Unsupported encode_type'
+                raise ValueError(msg)
 
-            result = self.client.set(key, encoded_value)  # WARNING: Удалил ex проблемы на винде
-            logger.info(f"Set operation result: {result}")
-            return result
+            result = self.client.set(
+                key, encoded_value
+            )  # WARNING: Удалил ex проблемы на винде
+            logger.info(f'Set operation result: {result}')
         except Exception as e:
-            logger.error(
-                f"Failed to set value '{value}' for key '{key}' " f"in Redis: {e}"
+            logger.exception(
+                f"Failed to set value '{value}' for key '{key}' " f'in Redis: {e}'
             )
             raise
+        else:
+            return result
 
     def delete(self, key):
         logger.info(f"Deleting key '{key}' from Redis...")
         try:
             result = self.client.delete(key)
-            logger.info(f"Delete operation result: {result}")
+            logger.info(f'Delete operation result: {result}')
             return result
         except Exception as e:
-            logger.error(f"Failed to delete key '{key}' from Redis: {e}")
+            logger.exception(f"Failed to delete key '{key}' from Redis: {e}")
             raise
```

### Comparing `python_uc_tools-0.1.0/src/uc_tools/tools/retry.py` & `python_uc_tools-0.2.0/src/uc_tools/tools/retry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
+import logging
+from typing import Any, Callable, Coroutine, TypeVar
 
-from typing import Any, Callable, Coroutine, TypeVar, Union
-from ..logger import setup_logger
-
-T = TypeVar("T")
+T = TypeVar('T')
 
+logger = logging.getLogger(__name__)
 
 def retry(
-    max_retries: int = 5, max_delay: Union[int, float] = 5
+    max_retries: int = 5, max_delay: float = 5
 ) -> Callable[
     [Callable[..., Coroutine[Any, Any, T]]], Callable[..., Coroutine[Any, Any, T]]
 ]:
     """
     Decorator that retries a coroutine function multiple times if it fails.
 
     Args:
@@ -22,34 +22,32 @@
         Callable[[Callable[..., Coroutine[Any, Any, T]]], Callable[..., Coroutine[Any, Any, T]]]:
             The decorated function.
     """
 
     def decorator(
         func: Callable[..., Coroutine[Any, Any, T]],
     ) -> Callable[..., Coroutine[Any, Any, T]]:
-        logger = setup_logger(__name__)
-
         async def wrapper(*args: Any, **kwargs: Any) -> T:
             for retries_count in range(max_retries + 1):
                 try:
                     return await func(*args, **kwargs)
                 except Exception as e:
                     if retries_count < max_retries:
                         logger.warning(
-                            f"Retry attempt {retries_count+1} for function "
-                            f"{func.__name__}: {e}"
+                            f'Retry attempt {retries_count + 1} for function {func.__name__!r}: {e!r}'
                         )
                         await asyncio.sleep(
                             min(
                                 max_delay,
                                 max_delay / max_retries * (max_retries - retries_count),
                             )
                         )
                     else:
                         logger.error(
-                            f"Max retries reached for function {func.__name__}"
+                            f'Max retries reached for function {func.__name__!r}'
                         )
                         raise
+            return None
 
         return wrapper
 
     return decorator
```

### Comparing `python_uc_tools-0.1.0/.gitignore` & `python_uc_tools-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python_uc_tools-0.1.0/LICENSE.txt` & `python_uc_tools-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_uc_tools-0.1.0/README.md` & `python_uc_tools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python_uc_tools-0.1.0/PKG-INFO` & `python_uc_tools-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.3
 Name: python-uc-tools
-Version: 0.1.0
+Version: 0.2.0
 Project-URL: Documentation, https://github.com/fennr/uc-tools#readme
 Project-URL: Issues, https://github.com/fennr/uc-tools/issues
 Project-URL: Source, https://github.com/fennr/uc-tools
 Author-email: fennr <fenrir1121@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Requires-Dist: fastapi>=0.95.0
 Requires-Dist: redis>=5.0.4
+Requires-Dist: tenacity>=8.3.0
 Description-Content-Type: text/markdown
 
 # uc_tools
 
 [![PyPI - Version](https://img.shields.io/pypi/v/python-uc-tools.svg)](https://pypi.org/project/python-uc-tools)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-uc-tools.svg)](https://pypi.org/project/python-uc-tools)
```

