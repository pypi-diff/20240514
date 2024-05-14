# Comparing `tmp/avrotize-1.5.1.tar.gz` & `tmp/avrotize-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.5.1.tar` & `avrotize-1.5.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    30034 2024-05-14 13:35:06.813500 avrotize-1.5.1/README.md
--rw-r--r--   0        0        0     1673 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-05-14 13:35:11.125550 avrotize-1.5.1/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    16902 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotize.py
--rw-r--r--   0        0        0    48267 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    58275 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12117 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     6433 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22200 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    13360 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotopython.py
--rw-r--r--   0        0        0    10166 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    13663 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/common.py
--rw-r--r--   0        0        0      112 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/constants.py
--rw-r--r--   0        0        0    19374 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    95346 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    20642 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/kustotoavro.py
--rw-r--r--   0        0        0    19742 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    17371 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1169 2024-05-14 13:35:06.817500 avrotize-1.5.1/pyproject.toml
--rw-r--r--   0        0        0    30740 1970-01-01 00:00:00.000000 avrotize-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    30034 2024-05-14 18:14:27.070084 avrotize-1.5.2/README.md
+-rw-r--r--   0        0        0     1673 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-05-14 18:14:31.266114 avrotize-1.5.2/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    16902 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotize.py
+-rw-r--r--   0        0        0    48409 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    58275 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12117 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18104 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     6433 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22200 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    13360 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    10166 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    13758 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/common.py
+-rw-r--r--   0        0        0      112 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/constants.py
+-rw-r--r--   0        0        0    19374 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    95346 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    20738 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/kustotoavro.py
+-rw-r--r--   0        0        0    19742 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    17371 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1169 2024-05-14 18:14:27.074084 avrotize-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0    30740 1970-01-01 00:00:00.000000 avrotize-1.5.2/PKG-INFO
```

### Comparing `avrotize-1.5.1/README.md` & `avrotize-1.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 Converting to Avro Schema:
 
 - [`avrotize p2a`´](#convert-proto-schema-to-avro-schema) - Convert Protobuf (2 or 3) schema to Avro schema.
 - [`avrotize j2a`](#convert-json-schema-to-avro-schema) - Convert JSON schema to Avro schema.
 - [`avrotize x2a`](#convert-xml-schema-xsd-to-avro-schema) - Convert XML schema to Avro schema.
 - [`avrotize asn2a`](#convert-asn1-schema-to-avro-schema) - Convert ASN.1 to Avro schema.
-- ['avrotize k2a'](#convert-kusto-table-definition-to-avro-schema) - Convert Kusto table definitions to Avro schema.
+- [`avrotize k2a`](#convert-kusto-table-definition-to-avro-schema) - Convert Kusto table definitions to Avro schema.
 
 Converting from Avro Schema:
 
 - [`avrotize a2p`](#convert-avro-schema-to-proto-schema) - Convert Avro schema to Protobuf 3 schema.
 - [`avrotize a2j`](#convert-avro-schema-to-json-schema) - Convert Avro schema to JSON schema.
 - [`avrotize a2x`](#convert-avro-schema-to-xml-schema) - Convert Avro schema to XML schema.
 - [`avrotize a2k`](#convert-avro-schema-to-kusto-table-declaration) - Convert Avro schema to Kusto table definition.
@@ -373,15 +373,15 @@
 - For `dynamic` columns, the tool will sample the data in the table to determine
   the structure of the dynamic column. The tool will map the dynamic column to an
   Avro record type with fields that correspond to the fields found in the dynamic
   column. If the dynamic column contains nested dynamic columns, the tool will
   recursively map those to Avro record types. If records with conflicting 
   structures are found in the dynamic column, the tool will emit a union of record
   types for the dynamic column.
-- If the `--emit-cloudevents-xregistry' option is set, the tool will emit an
+- If the `--emit-cloudevents-xregistry` option is set, the tool will emit an
   [xRegistry](http://xregistry.io) registry manifest file with a CloudEvent
   message definition for each table in the Kusto database and a separate Avro
   Schema for each table in the embedded schema registry. If one or more tables
   are found to contain CloudEvent data (as indicated by the presence of the
   CloudEvents attribute columns), the tool will inspect the content of the
   `type` (or `__type` or `__type`) columns to determine which CloudEvent types
   have been stored in the table and will emit a CloudEvent definition and schema
```

### Comparing `avrotize-1.5.1/avrotize/__init__.py` & `avrotize-1.5.2/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/asn1toavro.py` & `avrotize-1.5.2/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/avrotize.py` & `avrotize-1.5.2/avrotize/avrotize.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/avrotocsharp.py` & `avrotize-1.5.2/avrotize/avrotocsharp.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,14 +426,16 @@
             if self.is_csharp_reserved_word(field_name):
                 field_name = f"@{field_name}"
             if field_name == class_name:
                 field_name += "_"
             field_type = self.convert_avro_type_to_csharp(
                     class_name, field_name, field['type'], parent_namespace)
             class_definition += self.get_is_json_match_clause(class_name, field_name, field_type)
+        if field_count == 0:
+            class_definition += "true"
         class_definition += f";\n{INDENT}}}"
         return class_definition
 
     def get_is_json_match_clause(self, class_name, field_name, field_type) -> str:
         """ Generates the IsJsonMatch clause for a field """
         class_definition = ''
         field_name_js = field_name[1:] if field_name[0] == '@' else field_name
@@ -519,14 +521,15 @@
         return ref
 
     def generate_embedded_union(self, class_name: str, field_name: str, avro_type: List, parent_namespace: str, write_file: bool) -> str:
         """ Generates an embedded Union Class """
         class_definition_ctors = class_definition_decls = class_definition_read = ''
         class_definition_write = class_definition = class_definition_toobject = ''
         class_definition_objctr = class_definition_genericrecordctor = ''
+        namespace = pascal(self.concat_namespace(self.base_namespace, parent_namespace))
         list_is_json_match: List [str] = []
         union_class_name = pascal(field_name)+'Union'
         union_types = [self.convert_avro_type_to_csharp(class_name, field_name+"Option"+str(i), t, parent_namespace) for i,t in enumerate(avro_type)]
         for i, union_type in enumerate(union_types):
             is_dict = is_list = False
             if union_type.startswith("Dictionary<"):
                 # get the type information from the dictionary
@@ -639,15 +642,15 @@
                 f"{INDENT*3}else\n{INDENT*3}{{\n{INDENT*4}throw new NotSupportedException(\"No record type is set in the union\");\n{INDENT*3}}}\n{INDENT*2}}}\n" + \
                 f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Checks if the JSON element matches the schema\n{INDENT*2}/// </summary>\n" + \
                 f"{INDENT*2}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT*2}{{" + \
                 f"\n{INDENT*3}return "+f"\n{INDENT*3} || ".join(list_is_json_match)+f";\n{INDENT*2}}}\n"
         class_definition += f"{INDENT}}}\n}}"
 
         if write_file:
-            self.write_to_file(pascal(parent_namespace), class_name +"."+union_class_name, class_definition)
+            self.write_to_file(namespace, class_name +"."+union_class_name, class_definition)
         self.generated_types[class_name+'.'+union_class_name] = "union" # it doesn't matter if the names clash, we just need to know whether it's a union
         return union_class_name
 
     def find_type(self, kind: str, avro_schema: JsonNode, type_name: str, type_namespace: str, parent_namespace = '') -> JsonNode:
         """ recursively find the type (kind 'record' or 'enum') in the schema """
         if isinstance(avro_schema, list):
             for s in avro_schema:
```

### Comparing `avrotize-1.5.1/avrotize/avrotojava.py` & `avrotize-1.5.2/avrotize/avrotojava.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/avrotojs.py` & `avrotize-1.5.2/avrotize/avrotojs.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/avrotojsons.py` & `avrotize-1.5.2/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/avrotokusto.py` & `avrotize-1.5.2/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/avrotoparquet.py` & `avrotize-1.5.2/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/avrotoproto.py` & `avrotize-1.5.2/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/avrotopython.py` & `avrotize-1.5.2/avrotize/avrotopython.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/avrotots.py` & `avrotize-1.5.2/avrotize/avrotots.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/avrototsql.py` & `avrotize-1.5.2/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/avrotoxsd.py` & `avrotize-1.5.2/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/common.py` & `avrotize-1.5.2/avrotize/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -307,24 +307,27 @@
         return strings[0] + '::' + '::'.join(pascal(s) for s in strings[1:])
     if '.' in string:
         strings = string.split('.')
         return '.'.join(pascal(s) for s in strings)
     if not string or len(string) == 0:
         return string
     words = []
+    startswith_under = string[0] == '_'
     if '_' in string:
         # snake_case
         words = re.split(r'_', string)
     elif string[0].isupper():
         # PascalCase
         words = re.findall(r'[A-Z][a-z0-9_]*\.?', string)
     else:
         # camelCase
         words = re.findall(r'[a-z0-9]+\.?|[A-Z][a-z0-9_]*\.?', string)
     result = ''.join(word.capitalize() for word in words)
+    if startswith_under:
+        result = '_' + result
     return result
 
 def camel(string):
     """ Convert a string to camelCase """
     if '::' in string:
         strings = string.split('::')
         return strings[0] + '::' + '::'.join(camel(s) for s in strings[1:])
```

### Comparing `avrotize-1.5.1/avrotize/dependency_resolver.py` & `avrotize-1.5.2/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/generic/generic.avsc` & `avrotize-1.5.2/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/jsonstoavro.py` & `avrotize-1.5.2/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/kconnect.json` & `avrotize-1.5.2/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/kstructtoavro.py` & `avrotize-1.5.2/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/kustotoavro.py` & `avrotize-1.5.2/avrotize/kustotoavro.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import json
 from typing import Any, Dict, List, Tuple
 from azure.kusto.data import KustoClient, KustoConnectionStringBuilder
 from avrotize.common import get_tree_hash
 from avrotize.constants import AVRO_VERSION
 
-JsonNode = Dict[str, 'JsonNode'] | List['JsonNode'] | str | bool | None
+JsonNode = Dict[str, 'JsonNode'] | List['JsonNode'] | str | bool | int | None
 
 
 class KustoToAvro:
     """ Converts Kusto table schemas to Avro schema format."""
 
     def __init__(self, kusto_uri, kusto_database, avro_namespace: str, avro_schema_path, emit_cloudevents_xregistry: bool):
         """ Initializes the KustoToAvro class with the Kusto URI and database name. """
@@ -63,15 +63,15 @@
         """ Maps Python types to Avro types."""
         simple_types = {
             int: "int", float: "double", str: "string",
             bool: "boolean", bytes: {"type": "bytes", "logicalType": "decimal"}
         }
         if isinstance(python_value, dict):
             type_name_name = type_name.rsplit('.', 1)[-1]
-            type_name_namespace = type_name.rsplit('.', 1)[0] if '.' in type_name else ''
+            type_name_namespace = (type_name.rsplit('.', 1)[0])+"Types" if '.' in type_name else ''
             type_namespace = self.avro_namespace + ('.' if self.avro_namespace and type_name_namespace else '') + type_name_namespace
             record: Dict[str, JsonNode] = {
                 "type": "record",
                 "name": f"{type_name_name}",
             }
             if type_name_namespace:
                 record["namespace"] = type_namespace
@@ -179,29 +179,31 @@
         if len(unique_types) > 1:
             # Using a union of inferred types
             return unique_types
         else:
             # Single type, no need for union
             return unique_types[0]
 
-    def map_kusto_type_to_avro_type(self, kusto_type, table_name, column_name, type_column: dict | None, type_value: str | None) -> JsonNode:
-        """ Maps Kusto types to Avro types."""
-        if kusto_type == "dynamic":
-            return self.infer_dynamic_schema(table_name, column_name, type_column, type_value)
-        return str({
+    type_map : Dict[str, JsonNode] = {
             "int": "int", 
             "long": "long", 
             "string": "string",
             "real": "double", 
             "bool": "boolean",
             "datetime": {"type": "long", "logicalType": "timestamp-millis"},
             "timespan": {"type": "fixed", "size": 12, "logicalType": "duration"},
             "decimal": {"type": "fixed", "size": 16, "precision": 38, "logicalType": "decimal"},
             "dynamic": "bytes"
-        }.get(kusto_type, "string"))
+        }
+    
+    def map_kusto_type_to_avro_type(self, kusto_type, table_name, column_name, type_column: dict | None, type_value: str | None) -> JsonNode:
+        """ Maps Kusto types to Avro types."""
+        if kusto_type == "dynamic":
+            return self.infer_dynamic_schema(table_name, column_name, type_column, type_value)
+        return self.type_map.get(kusto_type, "string")
 
     def kusto_to_avro_schema(self, kusto_schema: dict, table_name: str) -> JsonNode:
         """ Converts a Kusto schema to Avro schema."""
         column_names = set([column['Name'].lstrip('_')
                            for column in kusto_schema['OrderedColumns']])
         type_values: List[str|None] = []
         type_column: Dict[str, JsonNode] = {}
@@ -250,16 +252,14 @@
                             schema["ce_attribs"] = ce_attribs
                         self.apply_schema_attributes(schema, kusto_schema, table_name, type_value, type_namespace)
                         schemas.append(schema)
             else:
                 for column in kusto_schema['OrderedColumns']:
                     avro_type = self.map_kusto_type_to_avro_type(
                         column['CslType'], table_name, column['Name'], type_column, type_value)
-                    if not isinstance(avro_type, dict) or "type" not in avro_type or avro_type["type"] != "record":
-                        avro_type = self.wrap_schema_in_root_record(avro_type, type_name_name, type_namespace)
                     field: Dict[str, JsonNode] = {"name": column['Name'], "type": avro_type}
                     doc: JsonNode = column.get('DocString', '')
                     if doc:
                         field["doc"] = doc
                     fields.append(field)
                 schema = {
                     "type": "record",
@@ -358,14 +358,16 @@
 
         output = None
         if self.emit_cloudevents_xregistry:
             xregistry_messages = {}
             xregistry_schemas = {}
             groupname = self.avro_namespace
             for schema in union_schema:
+                self.generated_types = []
+                self.make_type_names_unique([schema])
                 ce_attribs: Dict[str, JsonNode] = {}
                 if "ce_attribs" in schema:
                     ce_attribs = schema.get("ce_attribs", {})
                     del schema["ce_attribs"]                
                 schemaid = schema['ce_type'] if 'ce_type' in schema else f"{self.avro_namespace}.{schema['name']}"
                 schema_name = schemaid.rsplit('.', 1)[-1] 
                 xregistry_schemas[schemaid] = {
@@ -390,15 +392,16 @@
                             "value": schemaid
                         }
                     },
                     "schemaformat": f"Avro/{AVRO_VERSION}",
                     "schemaurl": f"#/schemagroups/{groupname}/schemas/{schemaid}"
                 }
                 for key, value in ce_attribs.items():
-                    if key == "type":
+                    # skip the required attributes
+                    if key == "type" or key == "source" or key == "id" or key == "specversion":
                         continue
                     xregistry_messages[schemaid]["metadata"][key] = {
                         "type": value,
                         "required": True
                     }
             output = {
                 "messagegroups": {
@@ -411,20 +414,21 @@
                     groupname: {
                         "id": groupname,
                         "schemas": xregistry_schemas
                     }
                 }
             }
         else:
+            self.generated_types = []
             self.make_type_names_unique(union_schema)
             output = union_schema
 
         # create the directory if it doesn't exist
         base_dir = os.path.dirname(self.avro_schema_path)
-        if not os.path.exists(base_dir):
+        if base_dir and not os.path.exists(base_dir):
             os.makedirs(base_dir)
         with open(self.avro_schema_path, 'w', encoding='utf-8') as avro_file:
             json.dump(output, avro_file, indent=4)
 
 
 def convert_kusto_to_avro(kusto_uri: str, kusto_database: str, avro_namespace: str, avro_schema_file: str, emit_cloudevents_xregistry: bool):
     """ Converts Kusto table schemas to Avro schema format."""
```

### Comparing `avrotize-1.5.1/avrotize/proto2parser.py` & `avrotize-1.5.2/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/proto3parser.py` & `avrotize-1.5.2/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/prototoavro.py` & `avrotize-1.5.2/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/prototypes/any.avsc` & `avrotize-1.5.2/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/prototypes/api.avsc` & `avrotize-1.5.2/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/prototypes/duration.avsc` & `avrotize-1.5.2/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/prototypes/field_mask.avsc` & `avrotize-1.5.2/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/prototypes/struct.avsc` & `avrotize-1.5.2/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/prototypes/timestamp.avsc` & `avrotize-1.5.2/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/prototypes/type.avsc` & `avrotize-1.5.2/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/prototypes/wrappers.avsc` & `avrotize-1.5.2/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/avrotize/xsdtoavro.py` & `avrotize-1.5.2/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/pyproject.toml` & `avrotize-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.1/PKG-INFO` & `avrotize-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.5.1
+Version: 1.5.2
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -147,15 +147,15 @@
 
 Converting to Avro Schema:
 
 - [`avrotize p2a`´](#convert-proto-schema-to-avro-schema) - Convert Protobuf (2 or 3) schema to Avro schema.
 - [`avrotize j2a`](#convert-json-schema-to-avro-schema) - Convert JSON schema to Avro schema.
 - [`avrotize x2a`](#convert-xml-schema-xsd-to-avro-schema) - Convert XML schema to Avro schema.
 - [`avrotize asn2a`](#convert-asn1-schema-to-avro-schema) - Convert ASN.1 to Avro schema.
-- ['avrotize k2a'](#convert-kusto-table-definition-to-avro-schema) - Convert Kusto table definitions to Avro schema.
+- [`avrotize k2a`](#convert-kusto-table-definition-to-avro-schema) - Convert Kusto table definitions to Avro schema.
 
 Converting from Avro Schema:
 
 - [`avrotize a2p`](#convert-avro-schema-to-proto-schema) - Convert Avro schema to Protobuf 3 schema.
 - [`avrotize a2j`](#convert-avro-schema-to-json-schema) - Convert Avro schema to JSON schema.
 - [`avrotize a2x`](#convert-avro-schema-to-xml-schema) - Convert Avro schema to XML schema.
 - [`avrotize a2k`](#convert-avro-schema-to-kusto-table-declaration) - Convert Avro schema to Kusto table definition.
@@ -393,15 +393,15 @@
 - For `dynamic` columns, the tool will sample the data in the table to determine
   the structure of the dynamic column. The tool will map the dynamic column to an
   Avro record type with fields that correspond to the fields found in the dynamic
   column. If the dynamic column contains nested dynamic columns, the tool will
   recursively map those to Avro record types. If records with conflicting 
   structures are found in the dynamic column, the tool will emit a union of record
   types for the dynamic column.
-- If the `--emit-cloudevents-xregistry' option is set, the tool will emit an
+- If the `--emit-cloudevents-xregistry` option is set, the tool will emit an
   [xRegistry](http://xregistry.io) registry manifest file with a CloudEvent
   message definition for each table in the Kusto database and a separate Avro
   Schema for each table in the embedded schema registry. If one or more tables
   are found to contain CloudEvent data (as indicated by the presence of the
   CloudEvents attribute columns), the tool will inspect the content of the
   `type` (or `__type` or `__type`) columns to determine which CloudEvent types
   have been stored in the table and will emit a CloudEvent definition and schema
```

