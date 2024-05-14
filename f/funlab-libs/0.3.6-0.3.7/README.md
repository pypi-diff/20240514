# Comparing `tmp/funlab_libs-0.3.6-py3-none-any.whl.zip` & `tmp/funlab_libs-0.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 25402 bytes, number of entries: 18
+Zip file size: 25892 bytes, number of entries: 18
 -rw-r--r--  2.0 fat     8616 b- defN 80-Jan-01 00:00 funlab/core/__init__.py
--rw-r--r--  2.0 fat    11375 b- defN 80-Jan-01 00:00 funlab/core/appbase.py
+-rw-r--r--  2.0 fat    11583 b- defN 80-Jan-01 00:00 funlab/core/appbase.py
 -rw-r--r--  2.0 fat     1068 b- defN 80-Jan-01 00:00 funlab/core/auth.py
 -rw-r--r--  2.0 fat    11262 b- defN 80-Jan-01 00:00 funlab/core/config.py
--rw-r--r--  2.0 fat     9020 b- defN 80-Jan-01 00:00 funlab/core/dbmgr.py
--rw-r--r--  2.0 fat     2005 b- defN 80-Jan-01 00:00 funlab/core/jinja_filters.py
+-rw-r--r--  2.0 fat     9058 b- defN 80-Jan-01 00:00 funlab/core/dbmgr.py
+-rw-r--r--  2.0 fat     2293 b- defN 80-Jan-01 00:00 funlab/core/jinja_filters.py
 -rw-r--r--  2.0 fat    10974 b- defN 80-Jan-01 00:00 funlab/core/menu.py
--rw-r--r--  2.0 fat     5656 b- defN 80-Jan-01 00:00 funlab/core/plugin.py
+-rw-r--r--  2.0 fat     5179 b- defN 80-Jan-01 00:00 funlab/core/plugin.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 funlab/utils/__init__.py
 -rw-r--r--  2.0 fat     3260 b- defN 80-Jan-01 00:00 funlab/utils/dtts.py
--rw-r--r--  2.0 fat     1723 b- defN 80-Jan-01 00:00 funlab/utils/lang.py
--rw-r--r--  2.0 fat     4693 b- defN 80-Jan-01 00:00 funlab/utils/log.py
+-rw-r--r--  2.0 fat     1571 b- defN 80-Jan-01 00:00 funlab/utils/lang.py
+-rw-r--r--  2.0 fat     6412 b- defN 80-Jan-01 00:00 funlab/utils/log.py
 -rw-r--r--  2.0 fat      667 b- defN 80-Jan-01 00:00 funlab/utils/url.py
--rw-r--r--  2.0 fat     4240 b- defN 80-Jan-01 00:00 funlab/utils/vars2env.py
--rw-r--r--  2.0 fat     2187 b- defN 80-Jan-01 00:00 funlab_libs-0.3.6.dist-info/LICENSE
--rw-r--r--  2.0 fat      959 b- defN 80-Jan-01 00:00 funlab_libs-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 funlab_libs-0.3.6.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1405 b- defN 16-Jan-01 00:00 funlab_libs-0.3.6.dist-info/RECORD
-18 files, 79198 bytes uncompressed, 23138 bytes compressed:  70.8%
+-rw-r--r--  2.0 fat     4315 b- defN 80-Jan-01 00:00 funlab/utils/vars2env.py
+-rw-r--r--  2.0 fat     1095 b- defN 80-Jan-01 00:00 funlab_libs-0.3.7.dist-info/LICENSE
+-rw-r--r--  2.0 fat      908 b- defN 80-Jan-01 00:00 funlab_libs-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 funlab_libs-0.3.7.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1405 b- defN 16-Jan-01 00:00 funlab_libs-0.3.7.dist-info/RECORD
+18 files, 79754 bytes uncompressed, 23628 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: funlab/utils/url.py
 Comment: 
 
 Filename: funlab/utils/vars2env.py
 Comment: 
 
-Filename: funlab_libs-0.3.6.dist-info/LICENSE
+Filename: funlab_libs-0.3.7.dist-info/LICENSE
 Comment: 
 
-Filename: funlab_libs-0.3.6.dist-info/METADATA
+Filename: funlab_libs-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: funlab_libs-0.3.6.dist-info/WHEEL
+Filename: funlab_libs-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: funlab_libs-0.3.6.dist-info/RECORD
+Filename: funlab_libs-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## funlab/core/appbase.py

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
-import logging
+import logging, os
 from dataclasses import is_dataclass
-from cryptography.fernet import Fernet
+# from cryptography.fernet import Fernet
 from flask import Flask, g, request
 from flask_login import AnonymousUserMixin, LoginManager, current_user
 from funlab.core.plugin import SecurityPlugin, ViewPlugin, load_plugins
 from funlab.utils import log
 from funlab.core import _Configuable, jinja_filters
 from funlab.core.config import Config
 from funlab.core.dbmgr import DbMgr
@@ -101,15 +101,16 @@
                                            level=logging.getLevelNamesMapping()[logging_level])
         else:
             self.mylogger = log.get_logger(self.__class__.__name__, level=logging.INFO)
         self.mylogger.info('Funlab Flask create started ...')
         # flask's config, different from self._config
         self.config.from_mapping(app_config.as_dict())
         if not self.config['SECRET_KEY']:
-            self.config.update({'SECRET_KEY': Fernet.generate_key().decode(), })
+            secret_key = os.urandom(24).hex()
+            self.config.update({'SECRET_KEY': secret_key} )  # Fernet.generate_key().decode(), })
 
         self.dbmgr: DbMgr = None
         if db_config := app_config.get(attrname='DATABASE'):
             self.dbmgr = DbMgr(db_config)
 
         if 'ENV' in self._config:
             del self._config.ENV
@@ -182,16 +183,17 @@
             if plugin_cls:=plugin_classes.pop(plugin_classname, None):
                 ordered_plugins.append(plugin_cls)
         # add rest of plugins
         for plugin_cls in plugin_classes.values() :
             ordered_plugins.append(plugin_cls)
 
         for plugin_cls in ordered_plugins :
-            self.mylogger.info(f"Loading plugin: {plugin_cls.__name__}")
+            self.mylogger.info(f"Loading plugin: {plugin_cls.__name__} ...", end='')
             self.register_plugin(plugin_cls=plugin_cls)
+            self.mylogger.info(f"Plugins {plugin_cls.__name__} loaded.")
 
         if self.login_manager is None:
             self.login_manager = LoginManager()
             self.login_manager.init_app(self)
             self.login_manager.login_view = 'root_bp.blank'
             @self.login_manager.user_loader
             def user_loader(user_id):
@@ -202,15 +204,15 @@
     @property
     def app(self)->Flask:
         """ Your own Flask implementation"""
         return self
 
     @property
     def app_config(self):
-        """ Original Flask config"""
+        """ This is Original Flask config, means to differencial my Config class obj """
         return self.config
 
     def append_mainmenu(self, menus:list[AbstractMenu]|AbstractMenu)->Menu:
         """ For App plugin to append main menu"""
         self._mainmenu.append(menus)
 
     def insert_mainmenu(self, idx:int, menus:list[AbstractMenu]|AbstractMenu)->Menu:
```

## funlab/core/dbmgr.py

```diff
@@ -48,15 +48,16 @@
         self._db_engines: Engine = None
         self._thread_safe_session_factories = {}
         self.__lock = threading.Lock()
 
     def __del__(self):
         try:
             self.remove_all_sessions(current_thread_only=False)  # remove all
-            self._db_engines.dispose
+            if self._db_engines:
+                self._db_engines.dispose
         except Exception as err:
             mylogger.error(f'DbMgr __del__ exception:{err}')
 
     def get_db_url(self) -> str:
         """
         Retrieves the database URL from the configuration.
```

## funlab/core/jinja_filters.py

```diff
@@ -1,14 +1,14 @@
 
 from datetime import date, datetime, time, timedelta
 from enum import Enum
 import math
 from funlab.utils import dtts
 
-__all__ = ['timestamp_natation', 'common_formatter']
+__all__ = ['timestamp_natation', 'common_formatter', 'slope2angle']
 
 def timestamp_natation(timestamp:float, formatstr:str='%Y-%m-%d %H:%M:%S')->str:
     """
     Converts a float timestamp() value to a formatted notation string in python.
     And, provide extra notation %q, this prsent the quarter number, e.g., %q got 2 for 2023-04-01. No %Q needed and supported.
 
     Args:
@@ -50,8 +50,20 @@
             value = value.date()
         return value.isoformat()
     # elif isinstance(value, pd.Timestamp):  暫不import & 處理 pandas.Timestamp type
     #     return value.isoformat()
     elif value is None:
         return 'NA'
     else:
-        return str(value)
+        return str(value)
+
+def slope2angle(slope:float)->float:
+    """
+    Convert the slope value to the angle in degrees.
+
+    Args:
+        slope (float): The slope value.
+
+    Returns:
+        float: The angle in degrees.
+    """
+    return f'{math.degrees(math.atan(slope)):,.3f}'
```

## funlab/core/plugin.py

```diff
@@ -1,47 +1,47 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+import logging
 from importlib.metadata import entry_points
 from flask_login import LoginManager
-from flask import Blueprint
+from flask import Blueprint, render_template
 from .menu import Menu
 from funlab.core.config import Config
 from funlab.core import _Configuable
+from funlab.utils import log
 from pathlib import Path
 import inspect
 from flask_login import current_user
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from funlab.core.appbase import _FlaskBase
 
 def load_plugins(group:str)->dict:
     plugins = {}
     # load dynamically, ref: https://packaging.python.org/en/latest/guides/creating-and-discovering-plugins/
     plugin_entry_points = entry_points(group=group)
     for entry_point in plugin_entry_points:
         plugin_name = entry_point.name
         try:
-            # print(entry_point)
             plugin_class = entry_point.load()
             plugins[plugin_name] = plugin_class
-            #_mylogger.info(f"Loaded plugin: {plugin_name}:{entry_point.value}")
         except Exception as e:
-            # _mylogger.error(f"Error loading plugin: {plugin_name} - {str(e)}")
             raise e
     return plugins
 
 class ViewPlugin(_Configuable, ABC):
     def __init__(self, app:_FlaskBase, url_prefix:str=None):
         """_summary_
         Args:
             app (FunlabFlask): The FunlabFlask app that have this plugin
             url_prefix (str, optional): The blueprint's url_prefix that represet plugin's view.
             Defaults to self.__class__.__name__.removesuffix('View').removesuffix('Security').removesuffix('Service').removesuffix('Plugin').lower().
         """
+        self.mylogger = log.get_logger(self.__class__.__name__, level=logging.INFO)
         self.app:_FlaskBase = app
         self.name = self.__class__.__name__.removesuffix('View').removesuffix('Security').removesuffix('Service').removesuffix('Plugin').lower()  #
         ext_config = self.app.get_section_config(section=self.__class__.__name__
                                                 , default=Config({self.__class__.__name__:{}}, env_file_or_values=self.app._config._env_vars)
                                                 , keep_section=True)
 
         self.plugin_config = self.get_config(file_name='plugin.toml', ext_config=ext_config)
@@ -87,27 +87,16 @@
         return True
 
     @property
     def entities_registry(self):
         """ FunlabFlask use to table creation by sqlalchemy in __init__ for application initiation """
         return None
 
-    # def register_errorhandler_routes(self):
-    #     @self.blueprint.errorhandler(403)
-    #     def access_forbidden(error):
-    #         return render_template('error-403.html'), 403
-
-    #     @self.blueprint.errorhandler(404)
-    #     def not_found_error(error):
-    #         return render_template('error-404.html'), 404
-
-    #     @self.blueprint.errorhandler(500)
-    #     def internal_error(error):
-    #         return render_template('error-500.html'), 500
-
+    def reload_config(self):
+        return NotImplemented
 class SecurityPlugin(ViewPlugin):
     def __init__(self, app:_FlaskBase, url_prefix:str=None):
         super().__init__(app, url_prefix)
         self._login_manager = LoginManager()  # LoginManager(app), not pass app, use init_app in
         self._login_manager.login_view = self.bp_name+".login"
         self._login_manager.login_message = "Please log in to access this page."
         self._login_manager.login_message_category = "warning"
```

## funlab/utils/lang.py

```diff
@@ -37,10 +37,7 @@
     attrs = {}
     for field in fields:
         if field.init:
             attrs[field.name] = getattr(dataclassobj, field.name)
     entity = entityclass(**attrs)
     return entity
 
-def create_log_entity_from_dataclass(dataclassobj, from_module):
-    return create_entity_from_dataclass(dataclassobj, from_module, name_ext='Log')
-
```

## funlab/utils/log.py

```diff
@@ -1,8 +1,9 @@
 import enum
+import sys
 import logging
 from datetime import date
 
 from colorama import Fore, Style, init
 
 init(autoreset=True)
 
@@ -15,14 +16,32 @@
 
 class LogFmtType(enum.IntEnum):
     EMPTY = 0
     SHORT = 1
     LONG = 2
     BASIC = 3
 
+def get_fmtstr(fmt:LogFmtType):
+    if isinstance(fmt, LogFmtType) and fmt == LogFmtType.EMPTY:
+        fmt = ''
+        datefmt = ''
+    elif isinstance(fmt, LogFmtType) and fmt == LogFmtType.SHORT:
+        fmt = '%(asctime)s[%(name)s] %(message)s'
+        datefmt = '%Y%m%dT%H%M%S'
+    elif isinstance(fmt, LogFmtType) and fmt == LogFmtType.LONG:
+        fmt = '%(asctime)s[%(name)s] %(levelname)s: %(message)s'
+        datefmt = '%Y-%m-%d %H:%M:%S.%f'
+    elif isinstance(fmt, LogFmtType) and fmt == LogFmtType.BASIC:
+        fmt = logging.BASIC_FORMAT
+        datefmt = '%Y-%m-%d %H:%M:%S'
+    else:
+        datefmt = '%Y-%m-%d %H:%M:%S'
+
+    return fmt, datefmt
+
 def get_logger(name:str, logtype:LogType=LogType.STDOUT, fmt:str | LogFmtType=LogFmtType.SHORT
                , level=logging.ERROR, **fmtkwargs)->logging.Logger:
     """
     Get a colored logger with the specified configuration.
     Use ColorFormatter to log colored message based on the log level as below:
         logging.DEBUG: Fore.GREEN
         logging.INFO: Fore.BLUE
@@ -36,42 +55,33 @@
         fmt (str | LogFmtType, optional): The log message format. Defaults to LogFmtType.SHORT.
         level (int, optional): The logging level. Defaults to logging.ERROR.
         **fmtkwargs: Additional keyword arguments for formatting the log message.
 
     Returns:
         logging.Logger: The configured logger instance.
     """
-
-    logger = logging.getLogger(name)
+    # logger = logging.getLogger(name)
+    logger = CustomLogger(name)
     logger.propagate = False # disable propagate so the parent, e.g. webserver waitress, will not show my log again
     for handler in logger.handlers.copy():
         try:
             logger.removeHandler(handler)
         except ValueError:  # in case another thread has already removed it
             pass
-    if isinstance(fmt, LogFmtType) and fmt == LogFmtType.EMPTY:
-        fmt = ''
-        datefmt = ''
-    elif isinstance(fmt, LogFmtType) and fmt == LogFmtType.SHORT:
-        fmt = '%(asctime)s[%(name)s] %(message)s'
-        datefmt = '%Y%m%dT%H%M%S'
-    elif isinstance(fmt, LogFmtType) and fmt == LogFmtType.LONG:
-        fmt = '%(asctime)s[%(name)s] %(levelname)s: %(message)s'
-        datefmt = '%Y-%m-%d %H:%M:%S.%f'
-    elif isinstance(fmt, LogFmtType) and fmt == LogFmtType.BASIC:
-        fmt = logging.BASIC_FORMAT
-        datefmt = '%Y-%m-%d %H:%M:%S'
+    if isinstance(fmt, LogFmtType):
+        fmt, datefmt = get_fmtstr(fmt)
     else:
+        fmt = fmt
         datefmt = '%Y-%m-%d %H:%M:%S'
 
     if logtype == LogType.OFF:
         logger.addHandler(logging.NullHandler())
         # logger.propagate = False
     elif logtype in (LogType.ON, LogType.STDOUT, LogType.BOTH):
-        handler = logging.StreamHandler()
+        handler = CustomHandler()
         handler.setFormatter(ColorFormatter(fmt=fmt, datefmt=datefmt))
         handler.setLevel(level)
         logger.addHandler(handler)
     elif logtype in (LogType.FILE, LogType.BOTH):
         handler = logging.FileHandler(f'{name}_{date.today().strftime("%y%m%d")}.log')
         handler.setLevel(level)
         handler.setFormatter(logging.Formatter(fmt=fmt, datefmt=datefmt))
@@ -115,14 +125,47 @@
             record (logging.LogRecord): The log record to be formatted.
 
         Returns:
             str: The formatted log message with color added.
         """
         return self.FMT_COLOR.get(record.levelno, '') + super().format(record)
 
+class CustomLogger(logging.Logger):
+    """This class is a custom logger that change info method to accept 'end' parameter to add end of line character.
+        whed end is not '\n', the log message will not add new line character at the end of the message."""
+    def __init__(self, name, level='INFO', end='\n'):
+        super().__init__(name, level)
+        self.end = end
+
+    def info(self, msg, *args, **kwargs):
+        end = kwargs.pop('end', self.end)
+        if self.isEnabledFor(logging.INFO):
+            self._log(logging.INFO, msg, args, **kwargs, end=end)
+
+    def _log(self, level, msg, args, exc_info=None, extra=None, stack_info=False, end='\n'):
+        sinfo = None
+        if logging._srcfile:
+            if stack_info:
+                # sinfo = traceback.extract_stack()[-4]
+                fn, lno, func, sinfo = self.findCaller(stack_info)
+            else:
+                fn, lno, func = "(unknown file)", 0, "(unknown function)"
+                sinfo = None
+        if exc_info:
+            if not isinstance(exc_info, tuple):
+                exc_info = sys.exc_info()
+        record = self.makeRecord(self.name, level, fn, lno, msg, args, exc_info, func, sinfo, extra)
+        record.end = end
+        self.handle(record)
+
+class CustomHandler(logging.StreamHandler):
+    def emit(self, record):
+        msg = self.format(record)
+        self.stream.write(msg + getattr(record, 'end', '\n'))
+        self.flush()
 
 if __name__ == '__main__':
     _logger = get_logger(__name__)
     _logger.debug('test')
     _logger.info('info')
     _logger.warning('warning')
     _logger.error('error')
```

## funlab/utils/vars2env.py

```diff
@@ -1,22 +1,22 @@
 import argparse
 import os
 import sys
 from pathlib import Path
 import tomllib
-from cryptography.fernet import Fernet, InvalidToken      
+from cryptography.fernet import Fernet, InvalidToken
 import re
 
 def validate_env_name(key_name, default_name='DEFAULT'):
     key_name = re.sub('[^a-zA-Z0-9_]', '', key_name)
     if key_name and key_name[0].isdigit():
         key_name = '_' + key_name
     if not key_name:
         return default_name
-    return key_name        
+    return key_name
 
 def generate_key(key_name:str=None):
     """
     This function generates a key and saves it into environment variable named 'key_name'
     """
     if not key_name:
         key_name = Fernet.generate_key().decode()
@@ -91,12 +91,12 @@
     args = parser.parse_args(args)
     print(f"This program will encoding variables value into OS. environment for application's sensitive data.")
     input("Press Enter to continue...")
     print(f'Encoding file: {args.envfile}')
     keyname = encode_envfile_vars(args.envfile, args.keyname)
     print(f"Encoding done, and use key:'{keyname}'' to get the value.")
 
-import sys
-
 if __name__ == "__main__":
+    # FLASK SECRET_KEY = 'cd81683f98378019ff1996c16971f7eb32256ea3cad5e6cf'
     args = None
-    args= ['-e', '.env'] # , '-k', '304929681ec4cf040877a7b8161b34e0']
+    args= ['-e', '.env', '-k', 'cd81683f98378019ff1996c16971f7eb32256ea3cad5e6cf']
+    main(args)
```

## Comparing `funlab_libs-0.3.6.dist-info/LICENSE` & `funlab_libs-0.3.7.dist-info/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023-2024 Sunny Lin(013)
+Copyright (c) 2023- Sunny Lin(013)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -16,28 +16,7 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
```

## Comparing `funlab_libs-0.3.6.dist-info/METADATA` & `funlab_libs-0.3.7.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: funlab-libs
-Version: 0.3.6
+Version: 0.3.7
 Summary: Some core libraries for funlab-flaskr.
 Home-page: https://github.com/sunnylin13/funlab-libs
 License: MIT
 Author: SunnyLin
 Author-email: 013.lin@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: cryptography (>=42.0.2,<43.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.17,<3.0.0)
 Project-URL: Repository, https://github.com/sunnylin13/funlab-libs
 Description-Content-Type: text/markdown
```

## Comparing `funlab_libs-0.3.6.dist-info/RECORD` & `funlab_libs-0.3.7.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 funlab/core/__init__.py,sha256=R9tTNMs-eCUEvNOqk6I1mUjgB6fgbKonjcPUaCY4o_4,8616
-funlab/core/appbase.py,sha256=RwfDd4luVuTwImm4NB3SZigcpv_CrRTDj4Fz20OriZU,11375
+funlab/core/appbase.py,sha256=sgTbRYKF5e6hjMenKrkFGY2zhLXYtJwv7Mqf0zktgDQ,11583
 funlab/core/auth.py,sha256=V_mrNcDwFHwtUwx0IKWFBNhlTq5Oi_vf2xbbmMWixxs,1068
 funlab/core/config.py,sha256=wCcDTmdTGYdu0nsSBZKd-gRIfHzFHF9nNsPmeRLo8wA,11262
-funlab/core/dbmgr.py,sha256=KxlTO-hPCgOoRCBsUv0bBnxEjhEyjZNSOeIWtJ1bgkw,9020
-funlab/core/jinja_filters.py,sha256=VxJzUANZhhmc5WKt_Qhvs_8Wkg632BS0JK_PEVflTKY,2005
+funlab/core/dbmgr.py,sha256=MxTLZRJ9QruygK0IqtK2dAJwCmrXkWMTyDwElVUDbdg,9058
+funlab/core/jinja_filters.py,sha256=udPvg1WvZzIhNktPh1Ndl3yshCCzk3BNL0XGeS_Gv3k,2293
 funlab/core/menu.py,sha256=9uAyPmTXHbIedFwT6DQNjdnXXb-DRc6lJyquAommHAE,10974
-funlab/core/plugin.py,sha256=GK_7-2o0tWgFogivE0jMRjXQFtfRbqqlHaknjrVwHWU,5656
+funlab/core/plugin.py,sha256=9u8YAJEqIgBVSl5qWErHlLgpvp2ag41B_IEUsgrG-VY,5179
 funlab/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funlab/utils/dtts.py,sha256=8ffmb72Crcc7PirRX0rMvdqYCCUwKRIGGc1ywSZ-Fss,3260
-funlab/utils/lang.py,sha256=lfAQQRXP1_8ZA6geJ6By9fbeDpZyufmb4qsjgrwmCpg,1723
-funlab/utils/log.py,sha256=d-Oz5SUIDIYHjYXRdms2L-Vcxw7Fex4BU9ZUrUyZJ1o,4693
+funlab/utils/lang.py,sha256=gOkzORa6H-kg-X4nSI2g8MVbQczfSQu7KbuNcQzDGaU,1571
+funlab/utils/log.py,sha256=W73gB9ncEiDZB5fYKzXPc8s1h5j76K-t7kwRC6cQJ48,6412
 funlab/utils/url.py,sha256=ewx8qstyaVzR_Ej0ndaQQrLgpZqjzTpuJf4jJgrYzN8,667
-funlab/utils/vars2env.py,sha256=aahyDOgFnDrwz1koJ2nu07NcPu-RW-fFwDZFUBim3i8,4240
-funlab_libs-0.3.6.dist-info/LICENSE,sha256=TjC17uJWdDbaNndmKEgtkiT7f7EXpfCouxpgF5y2_nA,2187
-funlab_libs-0.3.6.dist-info/METADATA,sha256=PZhOXVt-2bnj6hS1dv2UfRzeds-QfDZzeDocX2IXkmM,959
-funlab_libs-0.3.6.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-funlab_libs-0.3.6.dist-info/RECORD,,
+funlab/utils/vars2env.py,sha256=pcI-SMJ9NkFLvGu6U8LwcrViacsI-t8duLVNQhIaU1c,4315
+funlab_libs-0.3.7.dist-info/LICENSE,sha256=mJN5gP4iK8rod_JrMy6ztf5NrCOH5tBDeETa9DM7xMs,1095
+funlab_libs-0.3.7.dist-info/METADATA,sha256=WM5QNHJMqoVCkop7Q2e0tFCfRAKqT8hx0qBS78_JvBg,908
+funlab_libs-0.3.7.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+funlab_libs-0.3.7.dist-info/RECORD,,
```

