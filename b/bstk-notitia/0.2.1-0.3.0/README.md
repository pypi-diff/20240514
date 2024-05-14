# Comparing `tmp/bstk_notitia-0.2.1.tar.gz` & `tmp/bstk_notitia-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_notitia-0.2.1.tar", max compression
+gzip compressed data, was "bstk_notitia-0.3.0.tar", max compression
```

## Comparing `bstk_notitia-0.2.1.tar` & `bstk_notitia-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1705 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/README.md
--rw-r--r--   0        0        0     1080 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/__init__.py
--rw-r--r--   0        0        0      903 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/error.py
--rw-r--r--   0        0        0     1333 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/lib/abc/driver.py
--rw-r--r--   0        0        0      996 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/lib/abc/informant.py
--rw-r--r--   0        0        0     2706 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/lib/abc/investigator.py
--rw-r--r--   0        0        0     1947 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/lib/abc/observer.py
--rw-r--r--   0        0        0     1219 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/lib/abc/reporter.py
--rw-r--r--   0        0        0     8815 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/loader.py
--rw-r--r--   0        0        0     5922 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/modules/driver/mongodb.py
--rw-r--r--   0        0        0      565 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/modules/driver/null.py
--rw-r--r--   0        0        0     2316 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/modules/driver/passthrough.py
--rw-r--r--   0        0        0      408 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/modules/informant/internal/datetime.py
--rw-r--r--   0        0        0     1293 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/modules/investigator/internal/clock.py
--rw-r--r--   0        0        0     2111 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/modules/investigator/internal/mongo_record_processor.py
--rw-r--r--   0        0        0     1538 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/modules/observer/internal/mongo_collection_change.py
--rw-r--r--   0        0        0     1302 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/modules/observer/internal/mongo_record.py
--rw-r--r--   0        0        0     1445 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/modules/observer/internal/tick.py
--rw-r--r--   0        0        0      580 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/modules/reporter/internal/echo.py
--rw-r--r--   0        0        0     2993 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/modules/reporter/internal/mongo_record.py
--rw-r--r--   0        0        0    10281 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/notitia.py
--rw-r--r--   0        0        0    15682 2024-04-13 04:20:44.455144 bstk_notitia-0.2.1/bstk_notitia/roster.py
--rw-r--r--   0        0        0      770 2024-04-13 04:20:58.319218 bstk_notitia-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2220 1970-01-01 00:00:00.000000 bstk_notitia-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1705 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/README.md
+-rw-r--r--   0        0        0     1080 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/__init__.py
+-rw-r--r--   0        0        0      903 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/error.py
+-rw-r--r--   0        0        0     1430 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/lib/abc/driver.py
+-rw-r--r--   0        0        0     1086 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/lib/abc/informant.py
+-rw-r--r--   0        0        0     5381 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/lib/abc/investigator.py
+-rw-r--r--   0        0        0     2037 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/lib/abc/observer.py
+-rw-r--r--   0        0        0     1309 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/lib/abc/reporter.py
+-rw-r--r--   0        0        0     9185 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/loader.py
+-rw-r--r--   0        0        0     5974 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/driver/mongodb.py
+-rw-r--r--   0        0        0      565 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/driver/null.py
+-rw-r--r--   0        0        0     2463 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/driver/passthrough.py
+-rw-r--r--   0        0        0      745 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/informant/internal/datetime.py
+-rw-r--r--   0        0        0      400 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/informant/internal/http.py
+-rw-r--r--   0        0        0     1466 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/investigator/internal/clock.py
+-rw-r--r--   0        0        0     2205 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py
+-rw-r--r--   0        0        0     1605 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/mongo_collection_change.py
+-rw-r--r--   0        0        0     1434 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/mongo_record.py
+-rw-r--r--   0        0        0     1460 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/tick.py
+-rw-r--r--   0        0        0      697 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/reporter/internal/echo.py
+-rw-r--r--   0        0        0     3018 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/reporter/internal/mongo_record.py
+-rw-r--r--   0        0        0     4025 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/reporter/internal/notitia_case.py
+-rw-r--r--   0        0        0    10357 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/notitia.py
+-rw-r--r--   0        0        0    15705 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/roster.py
+-rw-r--r--   0        0        0      815 2024-05-14 01:30:21.481951 bstk_notitia-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2307 1970-01-01 00:00:00.000000 bstk_notitia-0.3.0/PKG-INFO
```

### Comparing `bstk_notitia-0.2.1/README.md` & `bstk_notitia-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.2.1/bstk_notitia/__init__.py` & `bstk_notitia-0.3.0/bstk_notitia/__init__.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.2.1/bstk_notitia/error.py` & `bstk_notitia-0.3.0/bstk_notitia/error.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.2.1/bstk_notitia/lib/abc/driver.py` & `bstk_notitia-0.3.0/bstk_notitia/lib/abc/driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 Notitia holds and provides connection strings, authentication information,
 etc, so modules purely need to know what dsn they should use.
 """
 
 
 @dataclass
 class DriverABC(ABC):
+    department: typing.AnyStr = field(kw_only=True, default=None)
     name: typing.AnyStr = field(init=False)
     key: typing.AnyStr = field(init=False)
     type: typing.AnyStr = field(init=False, default="driver")
 
-    connections: typing.Dict[str, typing.Any] = field(init=False, default_factory=dict)
+    connections: typing.Dict[typing.AnyStr, typing.Any] = field(
+        init=False, default_factory=dict
+    )
 
-    def set_up(self, dsn: str) -> typing.Dict:
+    def set_up(self, dsn: typing.Any) -> typing.Dict:
         self.connect(dsn)
 
     @abstractmethod
     def connect(self, dsn: typing.Any):
         """
         Connect to the specified DSN and return a "client like" reference that
         can be used to communicate with the service
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/lib/abc/informant.py` & `bstk_notitia-0.3.0/bstk_notitia/lib/abc/informant.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,22 @@
 """
 
 NOTITIA_DEPENDENCIES: typing.Dict
 
 
 @dataclass
 class InformantABC(ABC):
+    department: typing.AnyStr = field(kw_only=True, default=None)
     name: typing.AnyStr = field(init=False)
     key: typing.AnyStr = field(init=False)
     type: typing.AnyStr = field(init=False, default="informant")
 
-    driver: typing.Dict[str, DriverABC] = field(init=True, kw_only=True, default=None)
+    driver: typing.Dict[typing.AnyStr, DriverABC] = field(
+        init=True, kw_only=True, default=None
+    )
 
     def sign_on(self) -> typing.Dict:
         pass
 
     @abstractmethod
     async def enquire(self, **kwargs):
         pass
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/lib/abc/observer.py` & `bstk_notitia-0.3.0/bstk_notitia/lib/abc/observer.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,19 +31,22 @@
 """
 
 NOTITIA_DEPENDENCIES: typing.Dict
 
 
 @dataclass
 class ObserverABC(ABC):
+    department: typing.AnyStr = field(kw_only=True, default=None)
     name: typing.AnyStr = field(init=False)
     key: typing.AnyStr = field(init=False)
     type: typing.AnyStr = field(init=False, default="observer")
 
-    driver: typing.Dict[str, DriverABC] = field(init=True, kw_only=True, default=None)
+    driver: typing.Dict[typing.AnyStr, DriverABC] = field(
+        init=True, kw_only=True, default=None
+    )
 
     def sign_on(self) -> typing.Dict:
         pass
 
     @abstractmethod
     async def glance(self, *args, **kwargs) -> bool:
         """Quickly review the input data and see whether this observe should be looking at the data"""
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/lib/abc/reporter.py` & `bstk_notitia-0.3.0/bstk_notitia/lib/abc/reporter.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,19 +23,22 @@
 """
 
 NOTITIA_DEPENDENCIES: typing.Dict
 
 
 @dataclass
 class ReporterABC(ABC):
+    department: typing.AnyStr = field(kw_only=True, default=None)
     name: typing.AnyStr = field(init=False)
     key: typing.AnyStr = field(init=False)
     type: typing.AnyStr = field(init=False, default="reporter")
 
-    driver: typing.Dict[str, DriverABC] = field(init=True, kw_only=True, default=None)
+    driver: typing.Dict[typing.AnyStr, DriverABC] = field(
+        init=True, kw_only=True, default=None
+    )
 
     def sign_on(self) -> typing.Dict:
         pass
 
     @abstractmethod
     async def receive(self, **kwargs):
         pass
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/loader.py` & `bstk_notitia-0.3.0/bstk_notitia/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,14 +150,18 @@
             if _mod_type not in self.module_types:
                 continue
 
             if _mod_type not in self.modules:
                 self.modules[_mod_type] = []
 
             module_name = re.sub(r"\.py$", "", module_file.name)
+            if module_name[0:1] == "_":
+                # It's a valid module that's passed signature checks - but it's not executable, so we don't load it
+                continue
+
             if module_file.parent.name != _mod_type:
                 module_name = f"{module_file.parent.name}/{module_name}"
 
             self.modules[_mod_type].append(module_name)
             self._module_path_lookup[f"{_mod_type}/{module_name}"] = module_file
 
     def load_module(self, module_type: typing.AnyStr, module_name: typing.AnyStr):
@@ -183,14 +187,16 @@
         module_file = self._module_path_lookup[_mod_name]
 
         if not os.path.exists(module_file):
             raise NotitiaInvalidModulePath()
 
         _mod = __class__._import_module(_mod_name, module_file)
         self._modules[module_type][module_name] = _mod
+        if not _mod:
+            return
 
         self._load_module_deps(module_type, _mod)
 
     def _load_module_deps(self, module_type: str, module: ModuleType):
         acceptable_deps = NOTITIA_MODULE_DEPLIST[module_type]
 
         _deps: typing.Dict[str, typing.Union[typing.List, typing.Dict]] = getattr(
@@ -241,26 +247,32 @@
             _contents = _file.read_text()
             _signature = hmac.new(
                 self.signing_key.encode(), _contents.encode(), hashlib.sha256
             ).hexdigest()
 
             if _signature != _signatures[_fileref]:
                 raise NotitiaPathExtensionFileSignatureInvalid(
-                    "Signature verification failed"
+                    f"Signature verification failed for {_fileref}"
                 )
 
     @staticmethod
     def _import_module(name: str, source: Path) -> ModuleType:
         try:
             spec = importlib.util.spec_from_file_location(
                 "notitia_module." + name.replace("/", "."), source
             )
             loader = importlib.util.LazyLoader(spec.loader)
             spec.loader = loader
             module = importlib.util.module_from_spec(spec)
             loader.exec_module(module)
+            if hasattr(module, "BaseNotitiaModule"):
+                return False
+
             if not hasattr(module, "NotitiaModule"):
-                raise ValueError("Invalid module - NotitiaModule class not defined")
+                raise ValueError(
+                    f"Invalid module {module} - NotitiaModule class not defined"
+                )
             return module
+
         except Exception as e:
             print(f"failed to load module {source} // {str(e)}")
             return False
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/modules/driver/mongodb.py` & `bstk_notitia-0.3.0/bstk_notitia/modules/driver/mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,24 +75,24 @@
     by this module that wouldn't normally be available is the `watch` command
     which provides a functional wrapper around a mongo change stream.
     """
 
     name = "MongoDB (Motor) driver"
     key = "driver/mongodb"
 
-    dsn: typing.Optional[str] = field(kw_only=True, default=None)
-    database: typing.Optional[str] = field(kw_only=True, default=None)
-    collection: typing.Optional[str] = field(kw_only=True, default=None)
-    connections: typing.Dict[str, motor.motor_asyncio.AsyncIOMotorClient] = field(
-        init=False, default_factory=dict
+    dsn: typing.Optional[typing.AnyStr] = field(kw_only=True, default=None)
+    database: typing.Optional[typing.AnyStr] = field(kw_only=True, default=None)
+    collection: typing.Optional[typing.AnyStr] = field(kw_only=True, default=None)
+    connections: typing.Dict[typing.AnyStr, motor.motor_asyncio.AsyncIOMotorClient] = (
+        field(init=False, default_factory=dict)
     )
 
     # Notitia
     def connect(
-        self, dsn: typing.Optional[str] = None
+        self, dsn: typing.Optional[typing.AnyStr] = None
     ) -> motor.motor_asyncio.AsyncIOMotorClient:
         if not dsn and self.dsn:
             dsn = self.dsn
 
         if dsn not in self.connections:
             self.connections[dsn] = motor.motor_asyncio.AsyncIOMotorClient(
                 dsn, **mongod_params
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/modules/driver/null.py` & `bstk_notitia-0.3.0/bstk_notitia/modules/driver/null.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.2.1/bstk_notitia/modules/driver/passthrough.py` & `bstk_notitia-0.3.0/bstk_notitia/modules/driver/passthrough.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,26 +12,28 @@
 class NotitiaModule(DriverABC):
     name = "Passthrough driver"
     key = "driver/passthrough"
     connections: typing.Dict[str, typing.Any]
 
     #
     # The passthrough driver provides a consistent interface for custom drivers.
+    # You can use it as a simple registry to provide functionality to your modules without
+    # having to create a full blown driver.
     #
     # The "dsn" provided to connect will be the object the driver will use, we generate
     # and return a "reference", which can be used to later disconnect or make calls.
     # You can make a "call" by providing the connection reference along with the method / params to execute.
     # Because we don't have a proper dsn, calling connect multiple times with the same
     # client will generate multiple references - so don't do that.
     #
     # Note that passthrough / custom drivers are not licenses to do random things in random ways.
     # Notitia modules exist to provide consistent and predictable behaviour, i.e. don't do weird shit.
     #
     def connect(self, dsn: typing.Any) -> typing.Any:
-        if not dsn or not callable(dsn):
+        if not dsn or not hasattr(dsn, "__class__"):
             raise NotitiaInvalidDriverParameter("Invalid DSN")
 
         _ref = self._genref()
         self.connections[_ref] = dsn
 
         return _ref
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/modules/investigator/internal/clock.py` & `bstk_notitia-0.3.0/bstk_notitia/modules/investigator/internal/clock.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+from dataclasses import dataclass, field
 import datetime
+import typing
 from bstk_notitia.lib.abc.investigator import InvestigatorABC
 
 """
 This sample investigator is a clock watcher.
 
 It doesn't do anything interesting, but it does it reliably
 from the moment it clocks on, until it clocks off.
@@ -31,18 +33,23 @@
     "reporter": {
         "type": "internal/echo",
         "required": True,
     },
 }
 
 
+@dataclass
 class NotitiaModule(InvestigatorABC):
     name = "Internal Clock Investigator"
     key = "internal/clock"
 
+    target_timezone: typing.List[typing.AnyStr] = field(
+        kw_only=True, default_factory=list
+    )
+
     async def start(self, **kwargs):
         if not self.observer or not self.informant or not self.reporter:
             return
 
         async for _ in self.observer["internal/tick"].monitor():
             data: datetime.datetime = await self.informant[
                 "internal/datetime"
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/modules/investigator/internal/mongo_record_processor.py` & `bstk_notitia-0.3.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,15 +53,19 @@
     key = "internal/mongo_record_processor"
     driver: typing.Dict[str, typing.Union[MongoDBDriver, DriverABC]]
 
     async def start(self, **kwargs):
         res = await self.reporter["internal/mongo_record"].receive(
             action="insert",
             record=None,
-            data={"uuid": str(uuid4()), "collected": False},
+            data={
+                "uuid": str(uuid4()),
+                "collected": False,
+                "department": self.department,
+            },
         )
 
         async for document in self.observer["internal/mongo_record"].monitor():
             data: datetime.datetime = await self.informant[
                 "internal/datetime"
             ].enquire()
             res = await self.reporter["internal/mongo_record"].receive(
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/modules/observer/internal/mongo_collection_change.py` & `bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/mongo_collection_change.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 import typing
 
 import bson
-from lib.abc.observer import ObserverABC
+from bstk_notitia.lib.abc.observer import ObserverABC
 
 if typing.TYPE_CHECKING:
     from modules.driver.mongodb import NotitiaModule as MongoDBDriver, DriverABC
 
 NOTITIA_DEPENDENCIES = {
     "driver": {
         "type": "mongodb",
@@ -15,18 +15,19 @@
     }
 }
 
 
 @dataclass
 class NotitiaModule(ObserverABC):
     name = "Internal MongoDB Changestream"
-    key = "internal/mongodb_change"
-    resume_token: str = field(init=False, default=None)
+    key = "internal/mongodb_collection_change"
+    resume_token: typing.AnyStr = field(init=False, default=None)
 
-    driver: typing.Dict[str, typing.Union[MongoDBDriver, DriverABC]]
+    if typing.TYPE_CHECKING:
+        driver: typing.Dict[str, typing.Union[MongoDBDriver, DriverABC]]
 
     async def glance(self, document: typing.Dict) -> typing.Union[None, typing.Dict]:
         if "fullDocument" not in document:
             return None
         return document["fullDocument"]
 
     async def monitor(
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/modules/observer/internal/mongo_record.py` & `bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/mongo_record.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 import typing
 
-from lib.abc.observer import ObserverABC
+from bstk_notitia.lib.abc.observer import ObserverABC
 
 if typing.TYPE_CHECKING:
     from modules.driver.mongodb import NotitiaModule as MongoDBDriver, DriverABC
 
 NOTITIA_DEPENDENCIES = {
     "driver": {
         "type": "mongodb",
@@ -16,15 +16,16 @@
 
 
 @dataclass
 class NotitiaModule(ObserverABC):
     name = "Internal MongoDB Record"
     key = "internal/mongo_record"
 
-    driver: typing.Dict[str, typing.Union[MongoDBDriver, DriverABC]]
+    if typing.TYPE_CHECKING:
+        driver: typing.Dict[str, typing.Union[MongoDBDriver, DriverABC]]
 
     collection: typing.AnyStr = field(kw_only=True, default=None)
     lookup: typing.Optional[typing.Union[typing.List[typing.Dict], typing.Dict]] = (
         field(kw_only=True, default=None)
     )
 
     async def glance(self, document: typing.Dict) -> typing.Union[None, typing.Dict]:
@@ -33,13 +34,17 @@
     async def monitor(
         self,
         options: typing.Optional[typing.Dict] = None,
         lookup: typing.Optional[
             typing.Union[typing.List[typing.Dict], typing.Dict]
         ] = None,
     ) -> typing.AsyncGenerator[typing.Dict, None]:
-        if not lookup and self.lookup:
-            lookup = self.lookup
+        if self.lookup:
+            if not lookup:
+                lookup = self.lookup
+            else:
+                lookup = {**lookup, **self.lookup}
+
         async for _doc in (
             self.driver["mongodb"].get_collection(self.collection).find(lookup)
         ):
             yield _doc
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/modules/observer/internal/tick.py` & `bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/tick.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 }
 
 
 @dataclass
 class NotitiaModule(ObserverABC):
     name = "Internal Tick Observer"
     key = "internal/tick"
-    interval: float = field(kw_only=True, default=2)
+    interval: typing.SupportsFloat = field(kw_only=True, default=2)
 
     async def glance(self, target: typing.AnyStr) -> bool:
         if not target:
             return False
 
         try:
             timedelta.fromisoformat(target)
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/modules/reporter/internal/echo.py` & `bstk_notitia-0.3.0/bstk_notitia/modules/reporter/internal/echo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+from dataclasses import dataclass, field
 import typing
 from bstk_notitia.lib.abc.reporter import ReporterABC
 
 NOTITIA_DEPENDENCIES = {
     "driver": {
         "type": "null",
         "required": True,
     },
 }
 
 
+@dataclass
 class NotitiaModule(ReporterABC):
     name = "Internal Echo Reporter"
     key = "internal/echo"
 
+    timezone: typing.AnyStr = field(kw_only=True, default=None)
+
     async def receive(self, *args, **kwargs):
         if args:
             for _v in args:
                 await self.publish(f"{_v}")
 
         if kwargs:
             for _k, _v in args:
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/modules/reporter/internal/mongo_record.py` & `bstk_notitia-0.3.0/bstk_notitia/modules/reporter/internal/mongo_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,20 @@
 }
 
 
 class NotitiaModule(ReporterABC):
     name = "Internal MongoDB Record Reporter"
     key = "internal/mongodb_record"
 
-    driver: typing.Dict[str, typing.Union[MongoDBDriver, DriverABC]]
+    if typing.TYPE_CHECKING:
+        driver: typing.Dict[str, typing.Union[MongoDBDriver, DriverABC]]
 
     async def receive(
         self,
-        action: typing.Dict,
+        action: str,
         data: typing.Union[typing.List[typing.Dict], typing.Dict],
         record: typing.Optional[typing.Dict] = None,
         constraints: typing.Optional[typing.Dict[str, typing.Any]] = None,
     ):
         brief = None
         if action == "update":
             if not record or not record.get("_id"):
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/notitia.py` & `bstk_notitia-0.3.0/bstk_notitia/notitia.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,30 +123,32 @@
         **kwargs,
     ):
         if investigator not in self.investigators:
             raise ValueError("Invalid investigator")
 
         _mod = self.get_from_registry("investigator", investigator)
         if _mod is False:
-            raise ValueError("Investigator not elisted or failed to load")
+            raise ValueError("Investigator not enlisted or failed to load")
 
         _obj = self._load_and_resolve_investigator(
             _mod,
             investigator_params=investigator_params,
             dependency_params=dependency_params,
         )
         self._add_to_roster(
             _obj,
             {"args": args, "kwargs": kwargs},
         )
 
     def _boot_investigator(
         self, investigator_module, investigator_params
     ) -> InvestigatorABC:
-        _obj: InvestigatorABC = investigator_module.NotitiaModule()
+        _obj: InvestigatorABC = investigator_module.NotitiaModule(
+            department=self.department
+        )
         _obj.sign_on(**investigator_params)
         return _obj
 
     def _load_and_resolve_investigator(
         self,
         investigator_module: ModuleType[InvestigatorABC],
         investigator_params: typing.Optional[typing.Dict] = None,
@@ -166,15 +168,15 @@
         for _mod_type, _mod_entries in _deps.items():
             if not isinstance(_mod_entries, list):
                 _mod_entries = [_mod_entries]
 
             for _mod_config in _mod_entries:
                 _mod_key = f"{_mod_type}/{_mod_config['type']}"
                 if _mod_key not in _modules or not _modules[_mod_key]["module"]:
-                    if _mod_config.get("required", False):
+                    if _mod_config.get("required", True):
                         raise RuntimeError(
                             f"Failed to load required dependency {_mod_key}"
                         )
                     continue
 
         for _type in ("driver", "observer", "informant", "reporter"):
             self._resolve_investigator_params(
@@ -278,15 +280,15 @@
 
         return _modules
 
     def _load_resolve_module(
         self, _mod: ModuleType, init_params: typing.Optional[typing.Dict]
     ):
         try:
-            return _mod.NotitiaModule(**init_params)
+            return _mod.NotitiaModule(**init_params, department=self.department)
         except TypeError as ex:
             raise NotitiaBootstrapError from ex
 
     def _add_to_roster(
         self, investigator: InvestigatorABC, startup_params: typing.Dict
     ):
         if not self._roster:
```

### Comparing `bstk_notitia-0.2.1/bstk_notitia/roster.py` & `bstk_notitia-0.3.0/bstk_notitia/roster.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,22 +324,22 @@
                 continue
 
             idle_workstations = [_w for _w in self.workstations if _w.available is True]
             if not idle_workstations:
                 print(f"<o {_ticker} o>")
                 continue
 
-            idle_workstation = idle_workstations.pop(0)
-            if not idle_workstation:
-                print(f"<? {_ticker} ?>")
-                continue
+            for idle_workstation in idle_workstations:
+                if not idle_workstation:
+                    print(f"<? {_ticker} ?>")
+                    continue
 
-            idle_workstation.available = False
-            self.open_workstation(idle_workstation)
-            print(f"< {_ticker} +{idle_workstation.id} >")
+                idle_workstation.available = False
+                self.open_workstation(idle_workstation)
+                print(f"< {_ticker} +{idle_workstation.id} >")
 
         while self.occupied_workstation_count > 0:
             await self.finish()
             await asyncio.sleep(0.1)
 
     async def finish(self):
         """
```

### Comparing `bstk_notitia-0.2.1/pyproject.toml` & `bstk_notitia-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [tool.poetry]
 name = "bstk_notitia"
-version = "0.2.1"
+version = "0.3.0"
 description = "notitia core runtime & modules"
 authors = ["colin <colin@broadstack.com.au>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = { extras = ["cli"], version = "^1.0.0" }
 timedelta-isoformat = "^0.6.2.11"
 motor = "^3.3.2"
+simplejson = "^3.19.2"
+dateparser = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 pytest-asyncio = "^0.23.2"
 coverage = "^7.3.2"
 flake8 = "^7.0.0"
 black = "^24.0.0"
```

### Comparing `bstk_notitia-0.2.1/PKG-INFO` & `bstk_notitia-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: bstk_notitia
-Version: 0.2.1
+Version: 0.3.0
 Summary: notitia core runtime & modules
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dateparser (>=1.2.0,<2.0.0)
 Requires-Dist: motor (>=3.3.2,<4.0.0)
 Requires-Dist: python-dotenv[cli] (>=1.0.0,<2.0.0)
+Requires-Dist: simplejson (>=3.19.2,<4.0.0)
 Requires-Dist: timedelta-isoformat (>=0.6.2.11,<0.7.0.0)
 Description-Content-Type: text/markdown
 
 # Notitia core - pluggable payload procesing - everything is famous.. sort of..
 
 ```python
 import motor.motor_asyncio
```

