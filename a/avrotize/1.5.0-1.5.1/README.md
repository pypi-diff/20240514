# Comparing `tmp/avrotize-1.5.0.tar.gz` & `tmp/avrotize-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.5.0.tar` & `avrotize-1.5.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0    27129 2024-05-13 09:05:17.610896 avrotize-1.5.0/README.md
--rw-r--r--   0        0        0     1673 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-05-13 09:05:21.734894 avrotize-1.5.0/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    15713 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotize.py
--rw-r--r--   0        0        0    48267 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    58076 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12117 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22200 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    13360 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotopython.py
--rw-r--r--   0        0        0    10166 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    13663 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    95346 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    17371 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1138 2024-05-13 09:05:17.614896 avrotize-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    27796 1970-01-01 00:00:00.000000 avrotize-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    30034 2024-05-14 13:35:06.813500 avrotize-1.5.1/README.md
+-rw-r--r--   0        0        0     1673 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-05-14 13:35:11.125550 avrotize-1.5.1/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    16902 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotize.py
+-rw-r--r--   0        0        0    48267 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    58275 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12117 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18104 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     6433 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22200 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    13360 2024-05-14 13:35:06.813500 avrotize-1.5.1/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    10166 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    13663 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/common.py
+-rw-r--r--   0        0        0      112 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/constants.py
+-rw-r--r--   0        0        0    19374 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    95346 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    20642 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/kustotoavro.py
+-rw-r--r--   0        0        0    19742 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    17371 2024-05-14 13:35:06.817500 avrotize-1.5.1/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1169 2024-05-14 13:35:06.817500 avrotize-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    30740 1970-01-01 00:00:00.000000 avrotize-1.5.1/PKG-INFO
```

### Comparing `avrotize-1.5.0/README.md` & `avrotize-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 
 Converting to Avro Schema:
 
 - [`avrotize p2a`´](#convert-proto-schema-to-avro-schema) - Convert Protobuf (2 or 3) schema to Avro schema.
 - [`avrotize j2a`](#convert-json-schema-to-avro-schema) - Convert JSON schema to Avro schema.
 - [`avrotize x2a`](#convert-xml-schema-xsd-to-avro-schema) - Convert XML schema to Avro schema.
 - [`avrotize asn2a`](#convert-asn1-schema-to-avro-schema) - Convert ASN.1 to Avro schema.
+- ['avrotize k2a'](#convert-kusto-table-definition-to-avro-schema) - Convert Kusto table definitions to Avro schema.
 
 Converting from Avro Schema:
 
 - [`avrotize a2p`](#convert-avro-schema-to-proto-schema) - Convert Avro schema to Protobuf 3 schema.
 - [`avrotize a2j`](#convert-avro-schema-to-json-schema) - Convert Avro schema to JSON schema.
 - [`avrotize a2x`](#convert-avro-schema-to-xml-schema) - Convert Avro schema to XML schema.
 - [`avrotize a2k`](#convert-avro-schema-to-kusto-table-declaration) - Convert Avro schema to Kusto table definition.
@@ -333,14 +334,63 @@
     `VideotexString`, `GraphicString`, `VisibleString`, `GeneralString`, `UniversalString`,
     `CharacterString`, `T61String` are all mapped to Avro string type.
   - All other ASN.1 types are mapped to Avro string type.
 - The ability to parse ASN.1 schema files is limited and the tool may not be able
   to parse all ASN.1 files. The tool is based on the Python asn1tools package and
   is limited to that package's capabilities.
 
+### Convert Kusto table definition to Avro schema
+
+```bash
+avrotize k2a --kusto-uri <kusto_cluster_uri> --kusto-database <kusto_database> --avsc <path_to_avro_schema_file> --emit-cloudevents-xregistry
+```
+
+Parameters:
+
+- `--kusto-uri`: The URI of the Kusto cluster to connect to.
+- `--kusto-database`: The name of the Kusto database to read the table definitions from.
+- `--avsc`: The path to the Avro schema file to write the conversion result to.
+- `--emit-cloudevents-xregistry`: (optional) See discussion below.
+
+Conversion notes:
+- The tool directly connects to the Kusto cluster and reads the table
+  definitions from the specified database. The tool will convert all tables in
+  the database to Avro record types, returned in a top-level type union.
+- Connecting to the Kusto cluster leans on the same authentication mechanisms as
+  the Azure CLI. The tool will use the same authentication context as the Azure CLI
+  if it is installed and authenticated.
+- The tool will map the Kusto column types to Avro types as follows:
+  - `bool` is mapped to Avro boolean type.
+  - `datetime` is mapped to Avro long type with logical type `timestamp-millis`.
+  - `decimal` is mapped to a logical Avro type with the `logicalType` set to `decimal`
+    and the `precision` and `scale` set to the values of the `decimal` type in Kusto.
+  - `guid` is mapped to Avro string type.
+  - `int` is mapped to Avro int type.
+  - `long` is mapped to Avro long type.
+  - `real` is mapped to Avro double type.
+  - `string` is mapped to Avro string type.
+  - `timespan` is mapped to a logical Avro type with the `logicalType` set to
+    `duration`.
+- For `dynamic` columns, the tool will sample the data in the table to determine
+  the structure of the dynamic column. The tool will map the dynamic column to an
+  Avro record type with fields that correspond to the fields found in the dynamic
+  column. If the dynamic column contains nested dynamic columns, the tool will
+  recursively map those to Avro record types. If records with conflicting 
+  structures are found in the dynamic column, the tool will emit a union of record
+  types for the dynamic column.
+- If the `--emit-cloudevents-xregistry' option is set, the tool will emit an
+  [xRegistry](http://xregistry.io) registry manifest file with a CloudEvent
+  message definition for each table in the Kusto database and a separate Avro
+  Schema for each table in the embedded schema registry. If one or more tables
+  are found to contain CloudEvent data (as indicated by the presence of the
+  CloudEvents attribute columns), the tool will inspect the content of the
+  `type` (or `__type` or `__type`) columns to determine which CloudEvent types
+  have been stored in the table and will emit a CloudEvent definition and schema
+  for each unique type.
+
 ### Convert Avro schema to Kusto table declaration
 
 ```bash
 avrotize a2k --avsc <path_to_avro_schema_file> --kusto <path_to_kusto_kql_file> [--record-type <record_type>] [--emit-cloudevents-columns]
 ```
 
 Parameters:
```

### Comparing `avrotize-1.5.0/avrotize/__init__.py` & `avrotize-1.5.1/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/asn1toavro.py` & `avrotize-1.5.1/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/avrotize.py` & `avrotize-1.5.1/avrotize/avrotize.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from avrotize.avrotoparquet import convert_avro_to_parquet
 from avrotize.avrotoproto import convert_avro_to_proto
 from avrotize.avrotopython import convert_avro_to_python
 from avrotize.avrotots import convert_avro_to_typescript
 from avrotize.avrototsql import convert_avro_to_tsql
 from avrotize.jsonstoavro import convert_jsons_to_avro
 from avrotize.kstructtoavro import convert_kafka_struct_to_avro_schema
+from avrotize.kustotoavro import convert_kusto_to_avro
 from avrotize.prototoavro import convert_proto_to_avro
 from avrotize.xsdtoavro import convert_xsd_to_avro
 
 
 def main():
     parser = argparse.ArgumentParser(description='Convert a variety of schema formats to Avro Schema and vice versa.')
 
@@ -50,14 +51,21 @@
     a2x_parser.add_argument('--xsd', type=str, help='Path to the XSD schema file', required=True)
 
     a2k_parser = subparsers.add_parser('a2k', help='Convert Avro schema to Kusto schema')
     a2k_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     a2k_parser.add_argument('--kusto', type=str, help='Path to the Kusto table', required=True)
     a2k_parser.add_argument('--record-type', type=str, help='Record type in the Avro schema', required=False)
     a2k_parser.add_argument('--emit-cloudevents-columns', action='store_true', help='Add CloudEvents columns to the Kusto table', default=False)
+    
+    k2a_parser = subparsers.add_parser('k2a', help='Convert Kusto schema to Avro schema')
+    k2a_parser.add_argument('--kusto-uri', type=str, help='Kusto URI', required=True)
+    k2a_parser.add_argument('--kusto-database', type=str, help='Kusto database', required=True)
+    k2a_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
+    k2a_parser.add_argument('--namespace', type=str, help='Namespace for the Avro schema', required=False)
+    k2a_parser.add_argument('--emit-cloudevents-xregistry', action='store_true', help='Emit an xRegistry manifest with CloudEvents declarations for each table instead of a single Avro schema', required=False)
 
     a2tsql_parser = subparsers.add_parser('a2tsql', help='Convert Avro schema to T-SQL schema')
     a2tsql_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     a2tsql_parser.add_argument('--tsql', type=str, help='Path to the T-SQL table', required=True)
     a2tsql_parser.add_argument('--record-type', type=str, help='Record type in the Avro schema', required=False)
     a2tsql_parser.add_argument('--emit-cloudevents-columns', action='store_true', help='Add CloudEvents columns to the T-SQL table', default=False)
 
@@ -152,14 +160,22 @@
     elif args.command == 'a2k':
         avro_schema_path = args.avsc
         avro_record_type = args.record_type
         kusto_file_path = args.kusto
         emit_cloud_events_columns = args.emit_cloudevents_columns
         print(f'Converting Avro {avro_schema_path} to Kusto {kusto_file_path}')
         convert_avro_to_kusto(avro_schema_path, avro_record_type, kusto_file_path, emit_cloud_events_columns)
+    elif args.command == 'k2a':
+        kusto_uri = args.kusto_uri
+        kusto_database = args.kusto_database
+        avro_schema_path = args.avsc
+        namespace = args.namespace
+        emit_cloudevents_xregistry = args.emit_cloudevents_xregistry
+        print(f'Converting Kusto {kusto_uri} to Avro {avro_schema_path}')
+        convert_kusto_to_avro(kusto_uri, kusto_database, namespace, avro_schema_path, emit_cloudevents_xregistry)
     elif args.command == 'a2tsql':
         avro_schema_path = args.avsc
         avro_record_type = args.record_type
         tsql_file_path = args.tsql
         emit_cloud_events_columns = args.emit_cloudevents_columns
         print(f'Converting Avro {avro_schema_path} to T-SQL {tsql_file_path}')
         convert_avro_to_tsql(avro_schema_path, avro_record_type, tsql_file_path, emit_cloud_events_columns)
```

### Comparing `avrotize-1.5.0/avrotize/avrotocsharp.py` & `avrotize-1.5.1/avrotize/avrotocsharp.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/avrotojava.py` & `avrotize-1.5.1/avrotize/avrotojava.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # pylint: disable=too-many-arguments, too-many-locals, too-many-branches, too-many-statements, line-too-long
 
 """ Generates Java classes from Avro schema """
 import json
 import os
 from typing import Dict, List, Tuple, Union
+from avrotize.constants import AVRO_VERSION, JACKSON_VERSION, JDK_VERSION
 
 from avrotize.common import pascal, camel, is_generic_avro_type
 
 INDENT = '    '
 POM_CONTENT = """<?xml version="1.0" encoding="UTF-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0"
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
     xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
     <modelVersion>4.0.0</modelVersion>
     <groupId>{groupid}</groupId>
     <artifactId>{artifactid}</artifactId>
     <version>1.0-SNAPSHOT</version>
     <properties>
-        <maven.compiler.source>21</maven.compiler.source>
-        <maven.compiler.target>21</maven.compiler.target>
+        <maven.compiler.source>{JDK_VERSION}</maven.compiler.source>
+        <maven.compiler.target>{JDK_VERSION}</maven.compiler.target>
     </properties>
     <dependencies>
         <dependency>
             <groupId>org.apache.avro</groupId>
             <artifactId>avro</artifactId>
-            <version>1.11.3</version>
+            <version>{AVRO_VERSION}</version>
         </dependency>
         <dependency>
             <groupId>com.fasterxml.jackson</groupId>
             <artifactId>jackson-bom</artifactId>
-            <version>2.17.0</version>
+            <version>{JACKSON_VERSION}</version>
             <type>pom</type>
         </dependency>
     </dependencies>
 </project>
 """
 
 PREAMBLE_TOBYTEARRAY = \
@@ -346,32 +347,32 @@
         class_body = "\n".join(fields_str)
         class_definition += f"public class {class_name}"
         if self.avro_annotation:
             class_definition += " implements SpecificRecord"
         class_definition += " {\n"
         class_definition += f"{INDENT}public {class_name}() {{}}\n"
         class_definition += class_body
-        
+
         if self.avro_annotation:
             class_definition += f"\n{INDENT}public {class_name}(GenericData.Record record) {{\n"
             class_definition += f"{INDENT*2}for( int i = 0; i < record.getSchema().getFields().size(); i++ ) {{\n"
             class_definition += f"{INDENT*3}this.put(i, record.get(i));\n"
             class_definition += f"{INDENT*2}}}\n"
             class_definition += f"{INDENT}}}\n"
-        
+
         if self.avro_annotation:
             avro_schema_json = json.dumps(avro_schema)
             avro_schema_json = avro_schema_json.replace('"', '§')
             avro_schema_json = f"\"+\n{INDENT}\"".join(
                 [avro_schema_json[i:i+80] for i in range(0, len(avro_schema_json), 80)])
             avro_schema_json = avro_schema_json.replace('§', '\\"')
             class_definition += f"\n\n{INDENT}public static final Schema AVROSCHEMA = new Schema.Parser().parse(\n{INDENT}\"{avro_schema_json}\");"
             class_definition += f"\n{INDENT}public static final DatumWriter<{class_name}> AVROWRITER = new SpecificDatumWriter<{class_name}>(AVROSCHEMA);"
             class_definition += f"\n{INDENT}public static final DatumReader<{class_name}> AVROREADER = new SpecificDatumReader<{class_name}>(AVROSCHEMA);\n"
-            
+
             if self.jackson_annotations:
                 class_definition += f"\n{INDENT}@JsonIgnore"
             class_definition += f"\n{INDENT}@Override\n{INDENT}public Schema getSchema(){{ return AVROSCHEMA; }}\n"
             class_definition += self.generate_avro_get_method(class_name, avro_schema.get('fields', []), namespace)
             class_definition += self.generate_avro_put_method(class_name, avro_schema.get('fields', []), namespace)
 
         # emit toByteArray method
@@ -938,15 +939,15 @@
             os.makedirs(output_dir, exist_ok=True)
         pom_path = os.path.join(output_dir, "pom.xml")
         if not os.path.exists(pom_path):
             package_elements = self.base_package.split('.') if self.base_package else ["com", "example"]
             groupid = '.'.join(package_elements[:-1]) if len(package_elements) > 1 else package_elements[0]
             artifactid = package_elements[-1]
             with open(pom_path, 'w', encoding='utf-8') as file:
-                file.write(POM_CONTENT.format(groupid=groupid, artifactid=artifactid))
+                file.write(POM_CONTENT.format(groupid=groupid, artifactid=artifactid, AVRO_VERSION=AVRO_VERSION, JACKSON_VERSION=JACKSON_VERSION, JDK_VERSION=JDK_VERSION, PACKAGE=self.base_package))
         output_dir = os.path.join(
             output_dir, "src/main/java".replace('/', os.sep))
         if not os.path.exists(output_dir):
             os.makedirs(output_dir, exist_ok=True)
         self.output_dir = output_dir
         for avro_schema in (x for x in schema if isinstance(x, dict)):
             self.generate_class_or_enum(avro_schema, '')
```

### Comparing `avrotize-1.5.0/avrotize/avrotojs.py` & `avrotize-1.5.1/avrotize/avrotojs.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/avrotojsons.py` & `avrotize-1.5.1/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/avrotokusto.py` & `avrotize-1.5.1/avrotize/avrotokusto.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,14 @@
 import json
 import sys
+from typing import List
 
-def convert_avro_to_kusto(avro_schema_path, avro_record_type, kusto_file_path, emit_cloud_events_columns=False):
-    schema_file = avro_schema_path
-    if not schema_file:
-        print("Please specify the avro schema file")
-        sys.exit(1)
-    with open(schema_file, "r") as f:
-        schema_json = f.read()
-
-    # Parse the schema as a JSON object
-    schema = json.loads(schema_json)
-
-    if isinstance(schema, list) and avro_record_type:
-        schema = next((x for x in schema if x["name"] == avro_record_type), None)
-        if schema is None:
-            print(f"No record type {avro_record_type} found in the Avro schema")
-            sys.exit(1)
-    elif not isinstance(schema, dict):
-        print("Expected a single Avro schema as a JSON object, or a list of schema records")
-        sys.exit(1)
 
+def convert_record_to_kusto(schema: dict, emit_cloud_events_columns: bool) -> List[str]:
+    """Converts an Avro record schema to a Kusto table schema."""
     # Get the name and fields of the top-level record
     table_name = schema["name"]
     fields = schema["fields"]
 
     # Create a StringBuilder to store the kusto statements
     kusto = []
 
@@ -65,18 +49,69 @@
         ])
     if doc_string_statement:
         kusto.append(f".alter table [{table_name}] column-docstrings (")
         kusto.extend(doc_string_statement)
         kusto.append(");")
         kusto.append("")
 
-    with open(kusto_file_path, "w") as kusto_file:
+    # add the JSON mapping for the table
+    # .create-or-alter table dfl_data_events ingestion json mapping
+    kusto.append(
+        f".create-or-alter table [{table_name}] ingestion json mapping \"{table_name}_json_mapping\"")
+    kusto.append("```\n[")
+    for field in fields:
+        json_name = column_name = field["name"]
+        if 'altnames' in field:
+            if 'kql' in field['altnames']:
+                column_name = field['altnames']['kql']
+            if 'json' in field['altnames']:
+                json_name = field['altnames']['json']
+        kusto.append(
+            f"  {{\"column\": \"{column_name}\", \"path\": \"$.{json_name}\"}},")
+    kusto.append("]\n```\n\n")
+    return kusto
+
+
+def convert_avro_to_kusto(avro_schema_path, avro_record_type, kusto_file_path, emit_cloud_events_columns=False):
+    schema_file = avro_schema_path
+    if not schema_file:
+        print("Please specify the avro schema file")
+        sys.exit(1)
+    with open(schema_file, "r") as f:
+        schema_json = f.read()
+
+    # Parse the schema as a JSON object
+    schema = json.loads(schema_json)
+
+    if isinstance(schema, list):
+        if avro_record_type:
+            schema = next(
+                (x for x in schema if x["name"] == avro_record_type), None)
+            if schema is None:
+                print(
+                    f"No record type {avro_record_type} found in the Avro schema")
+                sys.exit(1)
+    elif not isinstance(schema, dict) or "type" not in schema or schema["type"] != "record":
+        print("Expected a single Avro schema as a JSON object, or a list of schema records")
+        sys.exit(1)
+
+    if not isinstance(schema, list):
+        schema = [schema]
+
+    kusto = []
+    for record in schema:
+        kusto.extend(convert_record_to_kusto(
+            record, emit_cloud_events_columns))
+
+    with open(kusto_file_path, "w", encoding="utf-8") as kusto_file:
         kusto_file.write("\n".join(kusto))
 
+
 def convert_avro_type_to_kusto_type(avroType):
+    """Converts an Avro type to a Kusto type."""
     if isinstance(avroType, list):
         # If the type is an array, then it is a union type. Look whether it's a pair of a scalar type and null:
         itemCount = len(avroType)
         if itemCount > 2:
             return "dynamic"
         if itemCount == 1:
             return convert_avro_type_to_kusto_type(avroType[0])
@@ -119,14 +154,15 @@
             return "int"
         else:
             return map_scalar_type(type)
     elif isinstance(avroType, str):
         return map_scalar_type(avroType)
     return "dynamic"
 
+
 def map_scalar_type(type):
     if type == "null":
         return "dynamic"
     elif type == "int":
         return "int"
     elif type == "long":
         return "long"
@@ -137,8 +173,8 @@
     elif type == "boolean":
         return "bool"
     elif type == "bytes":
         return "dynamic"
     elif type == "string":
         return "string"
     else:
-        return "dynamic"
+        return "dynamic"
```

### Comparing `avrotize-1.5.0/avrotize/avrotoparquet.py` & `avrotize-1.5.1/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/avrotoproto.py` & `avrotize-1.5.1/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/avrotopython.py` & `avrotize-1.5.1/avrotize/avrotopython.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/avrotots.py` & `avrotize-1.5.1/avrotize/avrotots.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/avrototsql.py` & `avrotize-1.5.1/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/avrotoxsd.py` & `avrotize-1.5.1/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/common.py` & `avrotize-1.5.1/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/dependency_resolver.py` & `avrotize-1.5.1/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/generic/generic.avsc` & `avrotize-1.5.1/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/jsonstoavro.py` & `avrotize-1.5.1/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/kconnect.json` & `avrotize-1.5.1/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/kstructtoavro.py` & `avrotize-1.5.1/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/proto2parser.py` & `avrotize-1.5.1/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/proto3parser.py` & `avrotize-1.5.1/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/prototoavro.py` & `avrotize-1.5.1/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/prototypes/any.avsc` & `avrotize-1.5.1/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/prototypes/api.avsc` & `avrotize-1.5.1/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/prototypes/duration.avsc` & `avrotize-1.5.1/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/prototypes/field_mask.avsc` & `avrotize-1.5.1/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/prototypes/struct.avsc` & `avrotize-1.5.1/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/prototypes/timestamp.avsc` & `avrotize-1.5.1/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/prototypes/type.avsc` & `avrotize-1.5.1/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/prototypes/wrappers.avsc` & `avrotize-1.5.1/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/avrotize/xsdtoavro.py` & `avrotize-1.5.1/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.0/pyproject.toml` & `avrotize-1.5.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "lark>=1.1.9",
     "pyarrow>=15.0.0",
     "asn1tools>=0.166.0",
     "jsonpointer>=2.4",
     "jsonpath-ng>=1.6.1",
     "jsoncomparison>=1.1.0",
     "requests>=2.31.0",
+    "azure-kusto-data>=4.4.1",
 ]
 dev-dependencies = [
     "pytest>=7.2.1",
     "fastavro>=1.9.4",
     "xmlschema>=3.0.2",
     "xmlunittest>=0.5.0",
     "pylint>=3.1.0",
```

### Comparing `avrotize-1.5.0/PKG-INFO` & `avrotize-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.5.0
+Version: 1.5.1
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Requires-Dist: lark>=1.1.9
 Requires-Dist: pyarrow>=15.0.0
 Requires-Dist: asn1tools>=0.166.0
 Requires-Dist: jsonpointer>=2.4
 Requires-Dist: jsonpath-ng>=1.6.1
 Requires-Dist: jsoncomparison>=1.1.0
 Requires-Dist: requests>=2.31.0
+Requires-Dist: azure-kusto-data>=4.4.1
 
 # Avrotize
 
 Avrotize is a command-line tool for converting data structure definitions between
 different schema formats, using [Apache Avro](https://avro.apache.org/) Schema
 as the integration schema model.
 
@@ -146,14 +147,15 @@
 
 Converting to Avro Schema:
 
 - [`avrotize p2a`´](#convert-proto-schema-to-avro-schema) - Convert Protobuf (2 or 3) schema to Avro schema.
 - [`avrotize j2a`](#convert-json-schema-to-avro-schema) - Convert JSON schema to Avro schema.
 - [`avrotize x2a`](#convert-xml-schema-xsd-to-avro-schema) - Convert XML schema to Avro schema.
 - [`avrotize asn2a`](#convert-asn1-schema-to-avro-schema) - Convert ASN.1 to Avro schema.
+- ['avrotize k2a'](#convert-kusto-table-definition-to-avro-schema) - Convert Kusto table definitions to Avro schema.
 
 Converting from Avro Schema:
 
 - [`avrotize a2p`](#convert-avro-schema-to-proto-schema) - Convert Avro schema to Protobuf 3 schema.
 - [`avrotize a2j`](#convert-avro-schema-to-json-schema) - Convert Avro schema to JSON schema.
 - [`avrotize a2x`](#convert-avro-schema-to-xml-schema) - Convert Avro schema to XML schema.
 - [`avrotize a2k`](#convert-avro-schema-to-kusto-table-declaration) - Convert Avro schema to Kusto table definition.
@@ -352,14 +354,63 @@
     `VideotexString`, `GraphicString`, `VisibleString`, `GeneralString`, `UniversalString`,
     `CharacterString`, `T61String` are all mapped to Avro string type.
   - All other ASN.1 types are mapped to Avro string type.
 - The ability to parse ASN.1 schema files is limited and the tool may not be able
   to parse all ASN.1 files. The tool is based on the Python asn1tools package and
   is limited to that package's capabilities.
 
+### Convert Kusto table definition to Avro schema
+
+```bash
+avrotize k2a --kusto-uri <kusto_cluster_uri> --kusto-database <kusto_database> --avsc <path_to_avro_schema_file> --emit-cloudevents-xregistry
+```
+
+Parameters:
+
+- `--kusto-uri`: The URI of the Kusto cluster to connect to.
+- `--kusto-database`: The name of the Kusto database to read the table definitions from.
+- `--avsc`: The path to the Avro schema file to write the conversion result to.
+- `--emit-cloudevents-xregistry`: (optional) See discussion below.
+
+Conversion notes:
+- The tool directly connects to the Kusto cluster and reads the table
+  definitions from the specified database. The tool will convert all tables in
+  the database to Avro record types, returned in a top-level type union.
+- Connecting to the Kusto cluster leans on the same authentication mechanisms as
+  the Azure CLI. The tool will use the same authentication context as the Azure CLI
+  if it is installed and authenticated.
+- The tool will map the Kusto column types to Avro types as follows:
+  - `bool` is mapped to Avro boolean type.
+  - `datetime` is mapped to Avro long type with logical type `timestamp-millis`.
+  - `decimal` is mapped to a logical Avro type with the `logicalType` set to `decimal`
+    and the `precision` and `scale` set to the values of the `decimal` type in Kusto.
+  - `guid` is mapped to Avro string type.
+  - `int` is mapped to Avro int type.
+  - `long` is mapped to Avro long type.
+  - `real` is mapped to Avro double type.
+  - `string` is mapped to Avro string type.
+  - `timespan` is mapped to a logical Avro type with the `logicalType` set to
+    `duration`.
+- For `dynamic` columns, the tool will sample the data in the table to determine
+  the structure of the dynamic column. The tool will map the dynamic column to an
+  Avro record type with fields that correspond to the fields found in the dynamic
+  column. If the dynamic column contains nested dynamic columns, the tool will
+  recursively map those to Avro record types. If records with conflicting 
+  structures are found in the dynamic column, the tool will emit a union of record
+  types for the dynamic column.
+- If the `--emit-cloudevents-xregistry' option is set, the tool will emit an
+  [xRegistry](http://xregistry.io) registry manifest file with a CloudEvent
+  message definition for each table in the Kusto database and a separate Avro
+  Schema for each table in the embedded schema registry. If one or more tables
+  are found to contain CloudEvent data (as indicated by the presence of the
+  CloudEvents attribute columns), the tool will inspect the content of the
+  `type` (or `__type` or `__type`) columns to determine which CloudEvent types
+  have been stored in the table and will emit a CloudEvent definition and schema
+  for each unique type.
+
 ### Convert Avro schema to Kusto table declaration
 
 ```bash
 avrotize a2k --avsc <path_to_avro_schema_file> --kusto <path_to_kusto_kql_file> [--record-type <record_type>] [--emit-cloudevents-columns]
 ```
 
 Parameters:
```

