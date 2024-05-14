# Comparing `tmp/sniffing-io-0.0.4.tar.gz` & `tmp/sniffing-io-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffing-io-0.0.4.tar", last modified: Mon May 13 14:20:34 2024, max compression
+gzip compressed data, was "sniffing-io-0.1.0.tar", last modified: Tue May 14 09:50:46 2024, max compression
```

## Comparing `sniffing-io-0.0.4.tar` & `sniffing-io-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:20:34.492486 sniffing-io-0.0.4/
--rw-rw-rw-   0        0        0       44 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6191 2024-05-13 14:20:34.491483 sniffing-io-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5339 2024-03-07 09:00:19.000000 sniffing-io-0.0.4/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 sniffing-io-0.0.4/build.py
--rw-rw-rw-   0        0        0        5 2024-03-07 08:05:04.000000 sniffing-io-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 14:20:34.492486 sniffing-io-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1546 2024-05-13 14:20:31.000000 sniffing-io-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:20:34.490493 sniffing-io-0.0.4/sniffing_io.egg-info/
--rw-rw-rw-   0        0        0     6191 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/sniffing_io.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/sniffing_io.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/sniffing_io.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/sniffing_io.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 14:20:34.000000 sniffing-io-0.0.4/sniffing_io.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 14:20:34.488483 sniffing-io-0.0.4/sniffingio/
--rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing-io-0.0.4/sniffingio/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing-io-0.0.4/sniffingio/callbacks.py
--rw-rw-rw-   0        0        0      859 2024-03-07 07:55:55.000000 sniffing-io-0.0.4/sniffingio/data.py
--rw-rw-rw-   0        0        0    11192 2024-05-13 14:19:29.000000 sniffing-io-0.0.4/sniffingio/filters.py
--rw-rw-rw-   0        0        0     2490 2024-03-07 07:55:55.000000 sniffing-io-0.0.4/sniffingio/sniff.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:50:46.511855 sniffing-io-0.1.0/
+-rw-rw-rw-   0        0        0       44 2024-05-14 09:50:46.000000 sniffing-io-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6214 2024-05-14 09:50:46.511855 sniffing-io-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5339 2024-03-07 09:00:19.000000 sniffing-io-0.1.0/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 sniffing-io-0.1.0/build.py
+-rw-rw-rw-   0        0        0       13 2024-05-14 06:59:25.000000 sniffing-io-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 09:50:46.512854 sniffing-io-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2024-05-14 09:50:43.000000 sniffing-io-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:50:46.510855 sniffing-io-0.1.0/sniffing_io.egg-info/
+-rw-rw-rw-   0        0        0     6214 2024-05-14 09:50:46.000000 sniffing-io-0.1.0/sniffing_io.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-05-14 09:50:46.000000 sniffing-io-0.1.0/sniffing_io.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 09:50:46.000000 sniffing-io-0.1.0/sniffing_io.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-14 09:50:46.000000 sniffing-io-0.1.0/sniffing_io.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 09:50:46.000000 sniffing-io-0.1.0/sniffing_io.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 09:50:46.509854 sniffing-io-0.1.0/sniffingio/
+-rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing-io-0.1.0/sniffingio/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing-io-0.1.0/sniffingio/callbacks.py
+-rw-rw-rw-   0        0        0      859 2024-03-07 07:55:55.000000 sniffing-io-0.1.0/sniffingio/data.py
+-rw-rw-rw-   0        0        0     9505 2024-05-14 09:50:27.000000 sniffing-io-0.1.0/sniffingio/filters.py
+-rw-rw-rw-   0        0        0     2490 2024-03-07 07:55:55.000000 sniffing-io-0.1.0/sniffingio/sniff.py
```

### Comparing `sniffing-io-0.0.4/PKG-INFO` & `sniffing-io-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffing-io
-Version: 0.0.4
+Version: 0.1.0
 Summary: A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 Home-page: https://github.com/Shahaf-F-S/sniffing-io
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: scapy
+Requires-Dist: dacite
 Provides-Extra: dev
 
 # Sniffing IO
 
 > A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 
 > The sniffing mechanism of sniffing-io is primarily based on the Scapy sniff function, but extends functionality and ease of control.
```

### Comparing `sniffing-io-0.0.4/README.md` & `sniffing-io-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.4/build.py` & `sniffing-io-0.1.0/build.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.4/setup.py` & `sniffing-io-0.1.0/setup.py`

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
-        version='0.0.4',
+        version='0.1.0',
         description=(
             "A simple package for packet sniffing, "
             "with static/dynamic filtering options, "
             "real-time reaction, I/O operations and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sniffing-io-0.0.4/sniffing_io.egg-info/PKG-INFO` & `sniffing-io-0.1.0/sniffing_io.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffing-io
-Version: 0.0.4
+Version: 0.1.0
 Summary: A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 Home-page: https://github.com/Shahaf-F-S/sniffing-io
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: scapy
+Requires-Dist: dacite
 Provides-Extra: dev
 
 # Sniffing IO
 
 > A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 
 > The sniffing mechanism of sniffing-io is primarily based on the Scapy sniff function, but extends functionality and ease of control.
```

### Comparing `sniffing-io-0.0.4/sniffingio/callbacks.py` & `sniffing-io-0.1.0/sniffingio/callbacks.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.4/sniffingio/data.py` & `sniffing-io-0.1.0/sniffingio/data.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.4/sniffingio/filters.py` & `sniffing-io-0.1.0/sniffingio/filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # filters.py
 
-from typing import Iterable, Callable, ClassVar
-from dataclasses import dataclass
+from typing import Iterable, Callable, ClassVar, Self
+from dataclasses import dataclass, asdict
 from abc import ABCMeta, abstractmethod
 
+from dacite import from_dict
+
 from scapy.all import Packet
 
 __all__ = [
     "PacketFilterOperand",
     "PacketFilter",
     "PacketFilterIntersection",
     "PacketFilterOperator",
@@ -17,49 +19,49 @@
     "BasePacketFilter",
     "StaticPacketFilter",
     "BasePacketFilterOperator",
     "BasePacketFilterIntersection",
     "format_packet_filters",
     "LivePacketFilter",
     "dump_packet_filter",
-    "load_packet_filter"
+    "load_packet_filter",
+    "PacketFilterValues"
 ]
 
+def wrap(value: str) -> str:
+
+    if (" " in value) and not (value.startswith("(") and value.endswith(")")):
+        value = f"({value})"
+
+    return value
+
 class BasePacketFilterOperator(metaclass=ABCMeta):
 
     @staticmethod
     def format_join(values: Iterable[str], joiner: str) -> str:
 
         if not values:
             return ""
 
-        values = tuple(values)
+        values = tuple(str(value) for value in values)
 
         if len(values) == 1:
-            data = values[0]
+            return wrap(values[0])
 
-            if (" " in data) and not (data.startswith("(") and data.endswith(")")):
-                data = f"({data})"
+        data = f" {joiner} ".join(wrap(value) for value in values if value)
 
-            return data
-
-        return f'({f" {joiner} ".join((value for value in values if value))})'
+        return f"({data})"
 
 class BasePacketFilterUnion(BasePacketFilterOperator, metaclass=ABCMeta):
 
     @classmethod
     def format_union(cls, values: Iterable[str]) -> str:
 
         return cls.format_join(values, joiner="or")
 
-    @classmethod
-    def format_intersection(cls, values: Iterable[str]) -> str:
-
-        return cls.format_join(values, joiner="and")
-
 class BasePacketFilterIntersection(BasePacketFilterOperator, metaclass=ABCMeta):
 
     @classmethod
     def format_intersection(cls, values: Iterable[str]) -> str:
 
         return cls.format_join(values, joiner="and")
 
@@ -70,158 +72,112 @@
 ):
 
     @abstractmethod
     def format(self) -> str:
 
         return ""
 
+@dataclass(slots=True, frozen=True)
 class PacketFilterOperand(BasePacketFilter, metaclass=ABCMeta):
 
-    TYPES: ClassVar[dict[str, list[type["PacketFilterOperand"]]]] = {}
-    ATTRIBUTES: ClassVar[set[str]]
-
-    def __init_subclass__(cls, **kwargs) -> None:
-
-        super().__init_subclass__(**kwargs)
-
-        cls.TYPES.setdefault(cls.__name__, []).append(cls)
-
-    def __eq__(self, other: ...) -> bool:
-
-        if (
-            not isinstance(other, PacketFilterOperand) or
-            (self.ATTRIBUTES != other.ATTRIBUTES)
-        ):
-            return NotImplemented
-
-        return all(
-            getattr(self, key) == getattr(other, key)
-            for key in self.ATTRIBUTES
-        )
-
     def __invert__(self) -> "PacketFilterOperand":
 
         if isinstance(self, PacketFilterNegation):
             return self.filter
 
         return PacketFilterNegation(self)
 
     def __or__(self, other: ...) -> "PacketFilterUnion":
 
         if isinstance(other, PacketFilterOperand):
-            return PacketFilterUnion((self, other))
-
-        return NotImplemented
-
-    def __and__(self, other: ...) -> "PacketFilterIntersection":
+            filters = []
 
-        if isinstance(other, PacketFilterOperand):
-            return PacketFilterIntersection((self, other))
+            if isinstance(self, PacketFilterUnion):
+                filters.extend(self.filters)
 
-        return NotImplemented
+            else:
+                filters.append(self)
 
-    @classmethod
-    def load(cls, data: dict[str, ...]) -> "PacketFilterOperand":
+            if isinstance(other, PacketFilterUnion):
+                filters.extend(other.filters)
 
-        data = data.copy()
+            else:
+                filters.append(other)
 
-        return cls.TYPES[data.pop('__type__')][0].load(data)
+            return PacketFilterUnion(tuple(filters))
 
-    def dump(self) -> dict[str, ...]:
+        return NotImplemented
 
-        data = {'__type__': type(self).__name__}
+    def __and__(self, other: ...) -> "PacketFilterIntersection":
 
-        for key in self.ATTRIBUTES:
-            value = getattr(self, key)
+        if isinstance(other, PacketFilterOperand):
+            filters = []
 
-            if isinstance(value, PacketFilterOperand):
-                data[key] = value.dump()
+            if isinstance(self, PacketFilterIntersection):
+                filters.extend(self.filters)
 
-            data[key] = value
+            else:
+                filters.append(self)
 
-        return data
+            if isinstance(other, PacketFilterIntersection):
+                filters.extend(other.filters)
 
-@dataclass(slots=True, frozen=True, eq=False)
-class StaticPacketFilter(PacketFilterOperand):
+            else:
+                filters.append(other)
 
-    filter: str
+            return PacketFilterIntersection(tuple(filters))
 
-    ATTRIBUTES: ClassVar[set[str]] = {'filter'}
+        return NotImplemented
 
     @classmethod
-    def load(cls, data: dict[str, str]) -> "StaticPacketFilter":
+    def load(cls, data: dict[str, ...]) -> Self:
 
-        return cls(data['filter'])
+        return from_dict(cls, data)
 
     def dump(self) -> dict[str, ...]:
 
-        return {'__type__': type(self).__name__, 'filter': self.filter}
+        return asdict(self)
+
+@dataclass(slots=True, frozen=True)
+class StaticPacketFilter(PacketFilterOperand):
+
+    filter: str
 
     def format(self) -> str:
 
         return self.filter
 
-@dataclass(slots=True, frozen=True, eq=False)
+@dataclass(slots=True, frozen=True)
 class PacketFilterOperator(PacketFilterOperand, metaclass=ABCMeta):
 
     filters: tuple["PacketFilterOperand", ...]
 
-    ATTRIBUTES: ClassVar[set[str]] = {'filters'}
-
     def __len__(self) -> int:
 
         return len(self.filters)
 
-    @classmethod
-    def load(cls, data: dict[str, ...]) -> "PacketFilterOperator":
-
-        return cls(
-            tuple(
-                PacketFilterOperand.load(value)
-                for value in data['filters']
-            )
-        )
-
-    def dump(self) -> dict[str, ...]:
-
-        return {
-            '__type__': type(self).__name__,
-            'filters': [value.dump() for value in self.filters]
-        }
-
-@dataclass(slots=True, frozen=True, eq=False)
+@dataclass(slots=True, frozen=True)
 class PacketFilterUnion(PacketFilterOperator, BasePacketFilterUnion):
 
     def format(self) -> str:
 
         return self.format_union(
             (f.format() for f in self.filters or ())
         )
 
-@dataclass(slots=True, frozen=True, eq=False)
+@dataclass(slots=True, frozen=True)
 class PacketFilterIntersection(PacketFilterOperator, BasePacketFilterIntersection):
 
-    def __and__(self, other: ...) -> "PacketFilterIntersection":
-
-        if isinstance(other, PacketFilterOperand):
-            if not isinstance(other, PacketFilterIntersection):
-                return PacketFilterIntersection((*self.filters, other))
-
-            else:
-                return PacketFilterIntersection((*self.filters, *other.filters))
-
-        return NotImplemented
-
     def format(self) -> str:
 
         return self.format_intersection(
             (f.format() for f in self.filters or ())
         )
 
-@dataclass(slots=True, frozen=True, eq=False)
+@dataclass(slots=True, frozen=True)
 class PacketFilterNegation(PacketFilterOperand):
 
     filter: PacketFilterOperand
 
     ATTRIBUTES: ClassVar[set[str]] = {'filter'}
 
     def format(self) -> str:
@@ -229,154 +185,136 @@
         data = self.filter.format()
 
         if not data:
             return ""
 
         return f"(not {data})"
 
-    @classmethod
-    def load(cls, data: dict[str, ...]) -> "PacketFilterNegation":
+def layers_names(packet: Packet) -> list[str]:
 
-        return cls(cls.TYPES[data['filter']['__type__']][0].load(data['filter']))
+    names = [packet.name]
 
-    def dump(self) -> dict[str, ...]:
+    while packet.payload:
+        packet = packet.payload
 
-        return {
-            '__type__': type(self).__name__,
-            'filter': self.filter.dump()
-        }
+        names.append(packet.name)
 
-@dataclass(slots=True, frozen=True, eq=False)
-class PacketFilter(PacketFilterOperand):
+    return names
+
+@dataclass(slots=True, frozen=True)
+class PacketFilterValues[T](PacketFilterOperand):
 
-    protocols: list[str] = None
-    hosts: list[str] = None
-    ports: list[int] = None
-    source_hosts: list[str] = None
-    source_ports: list[int] = None
-    destination_hosts: list[str] = None
-    destination_ports: list[int] = None
-
-    ATTRIBUTES: ClassVar[set[str]] = {
-        'protocols',
-        'hosts'
-        'ports'
-        'source_hosts',
-        'source_ports',
-        'destination_hosts',
-        'destination_ports'
-    }
+    types: list[str] = None
+    names: list[str] = None
+    values: list[T] = None
+    source_values: list[T] = None
+    destination_values: list[T] = None
+
+    @classmethod
+    def load(cls, data: dict[str, list[T]]) -> "PacketFilterValues[T]":
+
+        return from_dict(cls, data)
+
+    def dump(self) -> dict[str, list[T]]:
+
+        return asdict(self)
 
     @classmethod
     def format_values(cls, values: Iterable[str], key: str = None) -> str:
 
         if not values:
             return ""
 
         return cls.format_union(
             (
-                " ".join((key, value) if key else (value, ))
+                " ".join((key, str(value)) if key else (str(value),))
                 for value in values
                 if value
             )
         )
 
-    @classmethod
-    def load(cls, data: dict[str, list[str] | list[int] | None]) -> "PacketFilter":
-
-        return cls(**{key: data.get(key) for key in cls.ATTRIBUTES})
-
-    def dump(self) -> dict[str, list[str] | list[int] | str | None]:
-
-        data = {key: getattr(self, key) for key in self.ATTRIBUTES}
-        data['__type__'] = type(self).__name__
-
-        return data
-
-    def format_protocols(self) -> str:
-
-        if not self.protocols:
-            return ""
-
-        return self.format_values(
-            (protocol.lower() for protocol in self.protocols)
-        )
-
-    def format_source_hosts(self) -> str:
-
-        if not self.source_hosts:
-            return ""
-
-        return self.format_values(self.source_hosts, key="src host")
+    def format(self) -> str:
 
-    def format_hosts(self) -> str:
+        values = [
+            self.format_union(values)
+            for values in (
+                self.types,
+                (
+                    self.format_values(self.values, key=name)
+                    for name in self.names or ['']
+                ),
+                (
+                    self.format_values(
+                        self.source_values, key=' '.join(['src', name])
+                    )
+                    for name in self.names or ['']
+                ),
+                (
+                    self.format_values(
+                        self.destination_values, key=' '.join(['dst', name])
+                    )
+                    for name in self.names or ['']
+                )
+            )
+            if values
+        ]
 
-        if not self.hosts:
-            return ""
+        values = [value for value in values if value]
 
-        return self.format_values(self.hosts, key="host")
+        return self.format_intersection(values)
 
-    def format_destination_hosts(self) -> str:
+@dataclass(slots=True, frozen=True, eq=False)
+class PacketFilter(PacketFilterOperand):
 
-        if not self.destination_hosts:
-            return ""
+    data_link: PacketFilterValues[str] = None
+    internet: PacketFilterValues[str] = None
+    transportation: PacketFilterValues[int] = None
 
-        return self.format_values(self.destination_hosts, key="dst host")
+    def match(self, packet: Packet) -> bool:
 
-    def format_ports(self) -> str:
+        layers = (self.data_link, self.internet, self.transportation)
 
-        if not self.ports:
-            return ""
+        for layer, layer_filter in zip(packet.layers(), layers):
+            layer_filter: PacketFilterValues
 
-        return self.format_values((str(port) for port in self.ports), key="port")
+            if layer.name.lower() not in {n.lower() for n in layer_filter.types}:
+                return False
 
-    def format_source_ports(self) -> str:
+            if hasattr(layer, 'src'):
+                src = layer.src
+                dst = layer.dst
 
-        if not self.source_ports:
-            return ""
+            elif hasattr(layer, 'sport'):
+                src = layer.sport
+                dst = layer.dport
 
-        return self.format_values(
-            (str(port) for port in self.source_ports), key="src port"
-        )
+            else:
+                continue
 
-    def format_destination_ports(self) -> str:
+            sources = layer_filter.values + layer_filter.source_values
+            destinations = layer_filter.values + layer_filter.destination_values
 
-        if not self.destination_ports:
-            return ""
+            if (
+                (sources and (src not in sources)) or
+                (destinations and (dst not in destinations))
+            ):
+                return False
 
-        return self.format_values(
-            (str(port) for port in self.destination_ports), key="dst port"
-        )
+        return True
 
-    def format_data(self) -> str:
+    def format(self) -> str:
 
-        data = self.format_intersection(
+        return self.format_intersection(
             (
-                data for data in (
-                    self.format_protocols(),
-                    self.format_hosts(),
-                    self.format_ports(),
-                    self.format_source_hosts(),
-                    self.format_source_ports(),
-                    self.format_destination_hosts(),
-                    self.format_destination_ports()
-                )
-                if data
+                self.data_link.format(),
+                self.internet.format(),
+                self.transportation.format()
             )
         )
 
-        if data == "()":
-            return ""
-
-        return data
-
-    def format(self) -> str:
-
-        return self.format_data()
-
 def format_packet_filters(
         filters: BasePacketFilter | Iterable[BasePacketFilter],
         joiner: PacketFilterOperator = PacketFilterUnion
 ) -> str:
 
     if joiner is None:
         joiner = PacketFilterUnion
```

### Comparing `sniffing-io-0.0.4/sniffingio/sniff.py` & `sniffing-io-0.1.0/sniffingio/sniff.py`

 * *Files identical despite different names*

