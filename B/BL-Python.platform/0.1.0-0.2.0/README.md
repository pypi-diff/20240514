# Comparing `tmp/BL_Python.platform-0.1.0.tar.gz` & `tmp/bl_python_platform-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BL_Python.platform-0.1.0.tar", last modified: Wed Feb  7 18:58:52 2024, max compression
+gzip compressed data, was "bl_python_platform-0.2.0.tar", last modified: Tue May 14 21:39:45 2024, max compression
```

## Comparing `BL_Python.platform-0.1.0.tar` & `bl_python_platform-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:52.633818 BL_Python.platform-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:52.629818 BL_Python.platform-0.1.0/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:52.633818 BL_Python.platform-0.1.0/BL_Python/platform/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-07 18:58:44.000000 BL_Python.platform-0.1.0/BL_Python/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-02-07 18:58:44.000000 BL_Python.platform-0.1.0/BL_Python/platform/db_feature_flag_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-02-07 18:58:44.000000 BL_Python.platform-0.1.0/BL_Python/platform/feature_flag_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:52.633818 BL_Python.platform-0.1.0/BL_Python.platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-07 18:58:52.000000 BL_Python.platform-0.1.0/BL_Python.platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-07 18:58:52.000000 BL_Python.platform-0.1.0/BL_Python.platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 18:58:52.000000 BL_Python.platform-0.1.0/BL_Python.platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-07 18:58:52.000000 BL_Python.platform-0.1.0/BL_Python.platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-07 18:58:52.000000 BL_Python.platform-0.1.0/BL_Python.platform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-07 18:58:44.000000 BL_Python.platform-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-07 18:58:44.000000 BL_Python.platform-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-07 18:58:52.633818 BL_Python.platform-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-07 18:58:44.000000 BL_Python.platform-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:44.000000 BL_Python.platform-0.1.0/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-07 18:58:44.000000 BL_Python.platform-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 18:58:52.633818 BL_Python.platform-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.477477 bl_python_platform-0.2.0/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/BL_Python/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/dependency_injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/BL_Python/platform/feature_flag/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/feature_flag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/feature_flag/db_feature_flag_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/feature_flag/feature_flag_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/BL_Python/platform/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/identity/user_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/BL_Python.platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-14 21:39:45.000000 bl_python_platform-0.2.0/BL_Python.platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 21:39:45.000000 bl_python_platform-0.2.0/BL_Python.platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:39:45.000000 bl_python_platform-0.2.0/BL_Python.platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 21:39:45.000000 bl_python_platform-0.2.0/BL_Python.platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 21:39:45.000000 bl_python_platform-0.2.0/BL_Python.platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.477477 bl_python_platform-0.2.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.477477 bl_python_platform-0.2.0/test/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/test/unit/feature_flags/
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/test/unit/feature_flags/test_db_feature_flag_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/test/unit/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/test/unit/identity/test_loader.py
```

### Comparing `BL_Python.platform-0.1.0/BL_Python/platform/db_feature_flag_router.py` & `bl_python_platform-0.2.0/BL_Python/platform/feature_flag/db_feature_flag_router.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,74 @@
+from abc import ABC
 from logging import Logger
-from typing import Protocol, Type, cast
+from typing import Type, cast
 
-from BL_Python.programming.patterns import Singleton
 from injector import inject
 from sqlalchemy import Boolean, Column, Unicode
 from sqlalchemy.exc import NoResultFound
 from sqlalchemy.ext.declarative import DeclarativeMeta
 from sqlalchemy.orm.session import Session
 from typing_extensions import override
 
 from .feature_flag_router import FeatureFlagRouter
 
 
-class FeatureFlag(Protocol):
+class FeatureFlag(ABC):
+    def __init__(  # pyright: ignore[reportMissingSuperCall]
+        self,
+        /,
+        name: str,
+        description: str,
+        enabled: bool | None = False,
+    ) -> None:
+        raise NotImplementedError(
+            f"`{FeatureFlag.__class__.__name__}` should only be used for type checking."
+        )
+
     __tablename__: str
     name: Column[Unicode] | str
-    enabled: Column[Boolean] | bool
     description: Column[Unicode] | str
+    enabled: Column[Boolean] | bool
 
 
-class FeatureFlagTable(Singleton):
-    def __new__(cls, base: Type[DeclarativeMeta]):
-        class FeatureFlag(base):
+class FeatureFlagTable:
+    def __new__(cls, base: Type[DeclarativeMeta]) -> type[FeatureFlag]:
+        class _FeatureFlag(base):
             """
             A feature flag.
             """
 
             __tablename__ = "feature_flag"
 
-            name = Column("name", Unicode, primary_key=True, nullable=False)
-            enabled = Column("enabled", Boolean, nullable=True, default=False)
-            description = Column("description", Unicode, nullable=False)
+            name: Column[Unicode] | str = Column(
+                "name", Unicode, primary_key=True, nullable=False
+            )
+            description: Column[Unicode] | str = Column(
+                "description", Unicode, nullable=False
+            )
+            enabled: Column[Boolean] | bool = Column(
+                "enabled", Boolean, nullable=True, default=False
+            )
 
             @override
             def __repr__(self) -> str:
                 return "<FeatureFlag %s>" % (self.name)
 
-        return FeatureFlag
+        return cast(type[FeatureFlag], _FeatureFlag)
 
 
 class DBFeatureFlagRouter(FeatureFlagRouter):
+    _feature_flag: type[FeatureFlag]
     _session: Session
 
     @inject
-    def __init__(self, session: Session, logger: Logger) -> None:
+    def __init__(
+        self, feature_flag: type[FeatureFlag], session: Session, logger: Logger
+    ) -> None:
+        self._feature_flag = feature_flag
         self._session = session
         super().__init__(logger)
 
     @override
     def set_feature_is_enabled(self, name: str, is_enabled: bool):
         """
         Enable or disable a feature flag in the database.
@@ -65,16 +86,16 @@
 
         if not name:
             raise ValueError("`name` parameter is required and cannot be empty.")
 
         feature_flag: FeatureFlag
         try:
             feature_flag = (
-                self._session.query(FeatureFlag)
-                .filter(cast(Column[Unicode], FeatureFlag.name) == name)
+                self._session.query(self._feature_flag)
+                .filter(cast(Column[Unicode], self._feature_flag.name) == name)
                 .one()
             )
         except NoResultFound as e:
             raise LookupError(
                 f"The feature flag `{name}` does not exist. It must be created before being accessed."
             ) from e
 
@@ -98,16 +119,16 @@
         """
         if check_cache:
             enabled = super().feature_is_enabled(name, None)
             if enabled is not None:
                 return enabled
 
         feature_flag = (
-            self._session.query(FeatureFlag)
-            .filter(cast(Column[Unicode], FeatureFlag.name) == name)
+            self._session.query(self._feature_flag)
+            .filter(cast(Column[Unicode], self._feature_flag.name) == name)
             .one_or_none()
         )
 
         if feature_flag is None:
             self._logger.warn(
                 f'Feature flag {name} not found in database. Returning "False" by default.'
             )
```

### Comparing `BL_Python.platform-0.1.0/BL_Python/platform/feature_flag_router.py` & `bl_python_platform-0.2.0/BL_Python/platform/feature_flag/feature_flag_router.py`

 * *Files identical despite different names*

### Comparing `BL_Python.platform-0.1.0/BL_Python.platform.egg-info/PKG-INFO` & `bl_python_platform-0.2.0/BL_Python.platform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.platform
-Version: 0.1.0
+Version: 0.2.0
 Summary: Libraries for developing PaaS software in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BL_Python.platform-0.1.0/LICENSE.md` & `bl_python_platform-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `BL_Python.platform-0.1.0/PKG-INFO` & `bl_python_platform-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.platform
-Version: 0.1.0
+Version: 0.2.0
 Summary: Libraries for developing PaaS software in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BL_Python.platform-0.1.0/pyproject.toml` & `bl_python_platform-0.2.0/pyproject.toml`

 * *Files identical despite different names*

