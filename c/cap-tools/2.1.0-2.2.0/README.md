# Comparing `tmp/cap_tools-2.1.0.tar.gz` & `tmp/cap_tools-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cap_tools-2.1.0.tar", max compression
+gzip compressed data, was "cap_tools-2.2.0.tar", max compression
```

## Comparing `cap_tools-2.1.0.tar` & `cap_tools-2.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-05-13 21:56:59.062970 cap_tools-2.1.0/LICENSE
--rw-r--r--   0        0        0      681 2024-05-13 21:56:59.062970 cap_tools-2.1.0/README.md
--rw-r--r--   0        0        0     1894 2024-05-13 21:56:59.062970 cap_tools-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      530 2024-05-13 21:56:59.062970 cap_tools-2.1.0/src/cap_tools/__init__.py
--rw-r--r--   0        0        0    14800 2024-05-13 21:56:59.062970 cap_tools-2.1.0/src/cap_tools/models.py
--rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 cap_tools-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-13 22:15:42.964209 cap_tools-2.2.0/LICENSE
+-rw-r--r--   0        0        0      681 2024-05-13 22:15:42.964209 cap_tools-2.2.0/README.md
+-rw-r--r--   0        0        0     1894 2024-05-13 22:15:42.964209 cap_tools-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      530 2024-05-13 22:15:42.964209 cap_tools-2.2.0/src/cap_tools/__init__.py
+-rw-r--r--   0        0        0    14941 2024-05-13 22:15:42.964209 cap_tools-2.2.0/src/cap_tools/models.py
+-rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 cap_tools-2.2.0/PKG-INFO
```

### Comparing `cap_tools-2.1.0/LICENSE` & `cap_tools-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cap_tools-2.1.0/README.md` & `cap_tools-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cap_tools-2.1.0/pyproject.toml` & `cap_tools-2.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 update_changelog_on_bump = true
 
 [tool.coverage.run]
 source = ["src", "tests"]
 
 [tool.poetry]
 name = "cap-tools"
-version = "2.1.0"
+version = "2.2.0"
 description = "Python data bindings for the Common Alerting Protocol Version."
 authors = ["Björn Reetz <git@bjoern-reetz.de>"]
 readme = "README.md"
 packages = [{include = "cap_tools", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `cap_tools-2.1.0/src/cap_tools/__init__.py` & `cap_tools-2.2.0/src/cap_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cap_tools-2.1.0/src/cap_tools/models.py` & `cap_tools-2.2.0/src/cap_tools/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,19 +274,21 @@
         metadata={
             "type": "Element",
             "namespace": "urn:oasis:names:tc:emergency:cap:1.2",
         },
     )
 
     def geocodes_to_dict(self) -> dict[str, str]:
+        """Return the Area.geocodes as a dictionary."""
         return {
             geocode.value_name.value: geocode.value.value for geocode in self.geocodes
         }
 
     def geocodes_from_dict(self, geocodes: dict[str, str]) -> None:
+        """Overwrite Area.geocodes with values derived from the given dictionary."""
         self.geocodes = [
             Geocode(ValueName(name), Value(value)) for name, value in geocodes.items()
         ]
 
 
 @dataclass(slots=True, kw_only=True)
 class Info:
```

### Comparing `cap_tools-2.1.0/PKG-INFO` & `cap_tools-2.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cap-tools
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python data bindings for the Common Alerting Protocol Version.
 Author: Björn Reetz
 Author-email: git@bjoern-reetz.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

