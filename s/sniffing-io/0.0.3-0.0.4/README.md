# Comparing `tmp/sniffing-io-0.0.3.tar.gz` & `tmp/sniffing-io-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffing-io-0.0.3.tar", last modified: Mon May 13 14:15:06 2024, max compression
+gzip compressed data, was "sniffing-io-0.0.4.tar", last modified: Mon May 13 14:20:34 2024, max compression
```

## Comparing `sniffing-io-0.0.3.tar` & `sniffing-io-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:15:06.680791 sniffing-io-0.0.3/
--rw-rw-rw-   0        0        0       44 2024-05-13 14:15:06.000000 sniffing-io-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6191 2024-05-13 14:15:06.680791 sniffing-io-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5339 2024-03-07 09:00:19.000000 sniffing-io-0.0.3/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 sniffing-io-0.0.3/build.py
--rw-rw-rw-   0        0        0        5 2024-03-07 08:05:04.000000 sniffing-io-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 14:15:06.680791 sniffing-io-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1546 2024-05-13 14:15:03.000000 sniffing-io-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:15:06.679446 sniffing-io-0.0.3/sniffing_io.egg-info/
--rw-rw-rw-   0        0        0     6191 2024-05-13 14:15:06.000000 sniffing-io-0.0.3/sniffing_io.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-05-13 14:15:06.000000 sniffing-io-0.0.3/sniffing_io.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:15:06.000000 sniffing-io-0.0.3/sniffing_io.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-13 14:15:06.000000 sniffing-io-0.0.3/sniffing_io.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 14:15:06.000000 sniffing-io-0.0.3/sniffing_io.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 14:15:06.679446 sniffing-io-0.0.3/sniffingio/
--rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing-io-0.0.3/sniffingio/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing-io-0.0.3/sniffingio/callbacks.py
--rw-rw-rw-   0        0        0      859 2024-03-07 07:55:55.000000 sniffing-io-0.0.3/sniffingio/data.py
--rw-rw-rw-   0        0        0    10812 2024-05-13 14:14:53.000000 sniffing-io-0.0.3/sniffingio/filters.py
--rw-rw-rw-   0        0        0     2490 2024-03-07 07:55:55.000000 sniffing-io-0.0.3/sniffingio/sniff.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:20:34.492486 sniffing-io-0.0.4/
+-rw-rw-rw-   0        0        0       44 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6191 2024-05-13 14:20:34.491483 sniffing-io-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5339 2024-03-07 09:00:19.000000 sniffing-io-0.0.4/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 sniffing-io-0.0.4/build.py
+-rw-rw-rw-   0        0        0        5 2024-03-07 08:05:04.000000 sniffing-io-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:20:34.492486 sniffing-io-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2024-05-13 14:20:31.000000 sniffing-io-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:20:34.490493 sniffing-io-0.0.4/sniffing_io.egg-info/
+-rw-rw-rw-   0        0        0     6191 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/sniffing_io.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/sniffing_io.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/sniffing_io.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/sniffing_io.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/sniffing_io.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 14:20:34.488483 sniffing-io-0.0.4/sniffingio/
+-rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing-io-0.0.4/sniffingio/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing-io-0.0.4/sniffingio/callbacks.py
+-rw-rw-rw-   0        0        0      859 2024-03-07 07:55:55.000000 sniffing-io-0.0.4/sniffingio/data.py
+-rw-rw-rw-   0        0        0    11192 2024-05-13 14:19:29.000000 sniffing-io-0.0.4/sniffingio/filters.py
+-rw-rw-rw-   0        0        0     2490 2024-03-07 07:55:55.000000 sniffing-io-0.0.4/sniffingio/sniff.py
```

### Comparing `sniffing-io-0.0.3/PKG-INFO` & `sniffing-io-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffing-io
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 Home-page: https://github.com/Shahaf-F-S/sniffing-io
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sniffing-io-0.0.3/README.md` & `sniffing-io-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.3/build.py` & `sniffing-io-0.0.4/build.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.3/setup.py` & `sniffing-io-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sniffing-io',
-        version='0.0.3',
+        version='0.0.4',
         description=(
             "A simple package for packet sniffing, "
             "with static/dynamic filtering options, "
             "real-time reaction, I/O operations and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sniffing-io-0.0.3/sniffing_io.egg-info/PKG-INFO` & `sniffing-io-0.0.4/sniffing_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffing-io
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 Home-page: https://github.com/Shahaf-F-S/sniffing-io
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sniffing-io-0.0.3/sniffingio/callbacks.py` & `sniffing-io-0.0.4/sniffingio/callbacks.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.3/sniffingio/data.py` & `sniffing-io-0.0.4/sniffingio/data.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.3/sniffingio/filters.py` & `sniffing-io-0.0.4/sniffingio/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,24 +194,35 @@
     def format(self) -> str:
 
         return self.format_union(
             (f.format() for f in self.filters or ())
         )
 
 @dataclass(slots=True, frozen=True, eq=False)
-class PacketFilterIntersection(PacketFilterOperator, BasePacketFilterUnion):
+class PacketFilterIntersection(PacketFilterOperator, BasePacketFilterIntersection):
+
+    def __and__(self, other: ...) -> "PacketFilterIntersection":
+
+        if isinstance(other, PacketFilterOperand):
+            if not isinstance(other, PacketFilterIntersection):
+                return PacketFilterIntersection((*self.filters, other))
+
+            else:
+                return PacketFilterIntersection((*self.filters, *other.filters))
+
+        return NotImplemented
 
     def format(self) -> str:
 
         return self.format_intersection(
             (f.format() for f in self.filters or ())
         )
 
 @dataclass(slots=True, frozen=True, eq=False)
-class PacketFilterNegation(PacketFilterOperand, BasePacketFilterUnion):
+class PacketFilterNegation(PacketFilterOperand):
 
     filter: PacketFilterOperand
 
     ATTRIBUTES: ClassVar[set[str]] = {'filter'}
 
     def format(self) -> str:
```

### Comparing `sniffing-io-0.0.3/sniffingio/sniff.py` & `sniffing-io-0.0.4/sniffingio/sniff.py`

 * *Files identical despite different names*

