# Comparing `tmp/cheeseapi-1.2.0.tar.gz` & `tmp/cheeseapi-1.2.1.tar.gz`

## Comparing `cheeseapi-1.2.0.tar` & `cheeseapi-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/app.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/cors.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/exception.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/file.py
--rw-r--r--   0        0        0    32445 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/request.py
--rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/response.py
--rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/route.py
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/schedule.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/server.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/signal.py
--rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/text.py
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/validator.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/LICENSE
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/app.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/exception.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/file.py
+-rw-r--r--   0        0        0    32431 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/request.py
+-rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/response.py
+-rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/route.py
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/schedule.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/text.py
+-rw-r--r--   0        0        0    12949 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/validator.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/LICENSE
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 cheeseapi-1.2.1/PKG-INFO
```

### Comparing `cheeseapi-1.2.0/CheeseAPI/app.py` & `cheeseapi-1.2.1/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/CheeseAPI/cors.py` & `cheeseapi-1.2.1/CheeseAPI/cors.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/CheeseAPI/exception.py` & `cheeseapi-1.2.1/CheeseAPI/exception.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/CheeseAPI/file.py` & `cheeseapi-1.2.1/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/CheeseAPI/handle.py` & `cheeseapi-1.2.1/CheeseAPI/handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,15 +357,15 @@
                 await self.http_response(protocol)
             except BaseException as e:
                 await self.http_500(protocol, e, True)
                 await self.http_response(protocol, True)
 
     async def http_static(self, protocol: 'HttpProtocol'):
         if self._app.server.static and self._app.workspace.static and protocol.request.path.startswith(self._app.server.static) and protocol.request.method == http.HTTPMethod.GET:
-            for key in [ '', '.html', 'index.html', '/index.html' ]:
+            for key in [ '', '.html', '/index.html' ]:
                 try:
                     protocol.response = FileResponse(os.path.join(self._app.workspace.static, protocol.request.path[1:] + key))
 
                     await self.http_afterRequest(protocol)
                     if self._app.signal.http_afterRequest.receivers:
                         await self._app.signal.http_afterRequest.async_send(**{
                             'request': protocol.request,
```

### Comparing `cheeseapi-1.2.0/CheeseAPI/protocol.py` & `cheeseapi-1.2.1/CheeseAPI/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,17 +50,14 @@
         self.request._scheme = self.request.headers.get('X-Forwarded-Proto', 'https' if self.transport.get_extra_info('sslcontext') else 'http')
 
         if 'Cookie' in self.request.headers:
             self.request._cookie = {
                 t.split('=')[0]: t.split('=')[1] for t in self.request.headers['Cookie'].split('; ')
             }
 
-        if not self.parser.should_upgrade() and not int(self.request.headers.get('Content-Length', 0)):
-            asyncio.get_event_loop().create_task(app._handle.http(self))
-
     def on_body(self, body: bytes):
         if self.request.body is None:
             self.request._body = b''
         self.request._body += body
 
     def on_message_complete(self):
         if not self.parser.should_upgrade():
```

### Comparing `cheeseapi-1.2.0/CheeseAPI/request.py` & `cheeseapi-1.2.1/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/CheeseAPI/response.py` & `cheeseapi-1.2.1/CheeseAPI/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,15 @@
 
             _value = None
             if isinstance(self.body, Callable):
                 _value = self.body().encode()
             elif isinstance(self.body, str):
                 _value = self.body.encode()
             elif isinstance(self.body, bytes):
-                _value += self.body
+                _value = self.body
             if _value:
                 value += b'%x\r\n' % len(_value) + _value + b'\r\n0\r\n\r\n'
 
             return value, self._transfering
 
     def setCookie(self, key: str, value: str, *, path: str = '/', secure: bool = False, httpOnly: bool = False, domain: str = '', sameSite: Literal['Strict', 'Lax', 'None'] = 'Lax', expires: datetime.datetime | str | None = None, maxAge: datetime.timedelta | int | None = None):
         if 'Set-Cookies' not in self.headers:
```

### Comparing `cheeseapi-1.2.0/CheeseAPI/route.py` & `cheeseapi-1.2.1/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/CheeseAPI/schedule.py` & `cheeseapi-1.2.1/CheeseAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/CheeseAPI/server.py` & `cheeseapi-1.2.1/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/CheeseAPI/signal.py` & `cheeseapi-1.2.1/CheeseAPI/signal.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/CheeseAPI/text.py` & `cheeseapi-1.2.1/CheeseAPI/text.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/CheeseAPI/validator.py` & `cheeseapi-1.2.1/CheeseAPI/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 class Validator:
     def __init__(self,
         scope: Literal['form', 'headers', 'args', 'path', 'cookie'],
         key: str,
         *,
         required: bool = False,
         default: Any = None,
-        type: List[object | Callable] | object | Callable = str,
+        type: List[object | Callable] | object | Callable = None,
         expected_type: str | None = None,
         pattern: str | None = None,
         min: object | None = None,
         max: object | None = None,
         enum: List[Any] = [],
         fn: Callable | None = None,
         response: Response | None = None
@@ -97,15 +97,15 @@
 
                 若有返回值，则为该参数的最终值。
         '''
 
         self._scope: Literal['form', 'headers', 'args', 'path', 'cookie'] = scope
         self.key: str = key
         self._type: List[object | Callable] | object | Callable = type
-        self._expected_type: str = type.__name__ if expected_type is None else expected_type
+        self._expected_type: str | None = type.__name__ if expected_type is None and self._type is not None else expected_type
         self.required: bool = required
         self._default: Any = default
         self._pattern: str | None = pattern
         self.min: object | None = min
         self.max: object | None = max
         if self.min is not None and self.max is not None and self.min > self.max:
             raise ValueError('最小范围不能大于最大范围')
@@ -120,15 +120,16 @@
             else:
                 validatedForm[f'{self.scope}.{self.key}'] = (getattr(request, self.scope) or {}).get(self.key)
 
         if validatedForm[f'{self.scope}.{self.key}'] is None:
             if self.required:
                 raise ValidateError(self.response or Response(app._text.validator_requiredMessage(self.scope, self.key), 400))
             validatedForm[f'{self.scope}.{self.key}'] = self.default
-        else:
+
+        if validatedForm[f'{self.scope}.{self.key}'] is not None:
             if self.type is not None:
                 try:
                     if isinstance(self.type, list):
                         for type in self.type:
                             validatedForm[f'{self.scope}.{self.key}'] = type(validatedForm[f'{self.scope}.{self.key}'])
                     else:
                         validatedForm[f'{self.scope}.{self.key}'] = self.type(validatedForm[f'{self.scope}.{self.key}'])
@@ -199,15 +200,15 @@
         期望的数据类型，不参与校验，仅供提示。
         '''
 
         return self._expected_type
 
     @expected_type.setter
     def expected_type(self, value: str | None):
-        self._expected_type = self.type.__name__ if value is None else value
+        self._expected_type = self.type.__name__ if value is None and self.type is not None else value
 
     @property
     def default(self) -> Any:
         '''
         默认值；该值仍会执行校验流程，而不是直接应用。
         '''
```

### Comparing `cheeseapi-1.2.0/CheeseAPI/websocket.py` & `cheeseapi-1.2.1/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/CheeseAPI/workspace.py` & `cheeseapi-1.2.1/CheeseAPI/workspace.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/LICENSE` & `cheeseapi-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/README.md` & `cheeseapi-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.0/pyproject.toml` & `cheeseapi-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "1.2.0"
+version = "1.2.1"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
```

### Comparing `cheeseapi-1.2.0/PKG-INFO` & `cheeseapi-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 1.2.0
+Version: 1.2.1
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
 Requires-Dist: cheeselog==1.0.*
 Requires-Dist: cheesesignal==1.1.*
```

