# Comparing `tmp/fdk_rdf_parser-2.7.0.tar.gz` & `tmp/fdk_rdf_parser-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdk_rdf_parser-2.7.0.tar", max compression
+gzip compressed data, was "fdk_rdf_parser-2.7.1.tar", max compression
```

## Comparing `fdk_rdf_parser-2.7.0.tar` & `fdk_rdf_parser-2.7.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0    11357 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/LICENSE
--rw-r--r--   0        0        0     1246 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/pyproject.toml
--rw-r--r--   0        0        0      473 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/__init__.py
--rw-r--r--   0        0        0     1587 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/__init__.py
--rw-r--r--   0        0        0      270 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/address.py
--rw-r--r--   0        0        0      342 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/agent.py
--rw-r--r--   0        0        0      766 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/business_event.py
--rw-r--r--   0        0        0      336 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/catalog.py
--rw-r--r--   0        0        0      610 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/channel.py
--rw-r--r--   0        0        0     2711 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/concept.py
--rw-r--r--   0        0        0      189 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/conforms_to.py
--rw-r--r--   0        0        0      750 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/contactpoint.py
--rw-r--r--   0        0        0      436 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/cost.py
--rw-r--r--   0        0        0     2449 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/cpsvno_service.py
--rw-r--r--   0        0        0      356 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/data_distribution_service.py
--rw-r--r--   0        0        0     1668 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dataservice.py
--rw-r--r--   0        0        0     8657 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dataset.py
--rw-r--r--   0        0        0     1143 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dcat_resource.py
--rw-r--r--   0        0        0      274 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dct_standard.py
--rw-r--r--   0        0        0      924 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/distribution.py
--rw-r--r--   0        0        0      777 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/event.py
--rw-r--r--   0        0        0      758 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/evidence.py
--rw-r--r--   0        0        0      355 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/exceptions.py
--rw-r--r--   0        0        0      349 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/format.py
--rw-r--r--   0        0        0      183 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/harvest_meta_data.py
--rw-r--r--   0        0        0     3478 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/info_model.py
--rw-r--r--   0        0        0      331 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/legal_resource.py
--rw-r--r--   0        0        0      758 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/life_event.py
--rw-r--r--   0        0        0      402 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/media_type.py
--rw-r--r--   0        0        0     1910 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/model_element.py
--rw-r--r--   0        0        0     1147 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/model_property.py
--rw-r--r--   0        0        0      430 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/organization.py
--rw-r--r--   0        0        0      466 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/output.py
--rw-r--r--   0        0        0      376 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/participation.py
--rw-r--r--   0        0        0     1888 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/public_service.py
--rw-r--r--   0        0        0      326 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/publisher.py
--rw-r--r--   0        0        0      206 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/qualified_attribution.py
--rw-r--r--   0        0        0      202 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/quality_annotation.py
--rw-r--r--   0        0        0      227 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/reference_data_code.py
--rw-r--r--   0        0        0      277 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/references.py
--rw-r--r--   0        0        0      412 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/requirement.py
--rw-r--r--   0        0        0      424 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/rule.py
--rw-r--r--   0        0        0      317 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/skos_concept.py
--rw-r--r--   0        0        0      271 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/subject.py
--rw-r--r--   0        0        0      191 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/temporal.py
--rw-r--r--   0        0        0      610 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/theme.py
--rw-r--r--   0        0        0      506 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/types.py
--rw-r--r--   0        0        0     8796 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/fdk_rdf_parser.py
--rw-r--r--   0        0        0     1349 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/__init__.py
--rw-r--r--   0        0        0     1070 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/address.py
--rw-r--r--   0        0        0     2175 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/agent.py
--rw-r--r--   0        0        0     1153 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/catalog.py
--rw-r--r--   0        0        0     1739 2024-04-04 07:42:04.685082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/channel.py
--rw-r--r--   0        0        0    11906 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/concept.py
--rw-r--r--   0        0        0      992 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/conforms_to.py
--rw-r--r--   0        0        0     3172 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/contactpoint.py
--rw-r--r--   0        0        0     1336 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/cost.py
--rw-r--r--   0        0        0     6030 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/cpsvno_service.py
--rw-r--r--   0        0        0     1555 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/data_distribution_service.py
--rw-r--r--   0        0        0     1671 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dataservice.py
--rw-r--r--   0        0        0     9262 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dataset.py
--rw-r--r--   0        0        0     2928 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dcat_resource.py
--rw-r--r--   0        0        0      979 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dct_standard.py
--rw-r--r--   0        0        0     2051 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/distribution.py
--rw-r--r--   0        0        0     3093 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/event.py
--rw-r--r--   0        0        0     2018 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/evidence.py
--rw-r--r--   0        0        0     1116 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/format.py
--rw-r--r--   0        0        0      431 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/harvest_meta_data.py
--rw-r--r--   0        0        0     6492 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/info_model.py
--rw-r--r--   0        0        0     1047 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/legal_resource.py
--rw-r--r--   0        0        0     3338 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/media_type.py
--rw-r--r--   0        0        0     4432 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/model_element.py
--rw-r--r--   0        0        0     3439 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/model_property.py
--rw-r--r--   0        0        0     2623 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/organization.py
--rw-r--r--   0        0        0     1247 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/output.py
--rw-r--r--   0        0        0      816 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/participation.py
--rw-r--r--   0        0        0     2155 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/publisher.py
--rw-r--r--   0        0        0      911 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/qualified_attribution.py
--rw-r--r--   0        0        0     1451 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/quality_annotation.py
--rw-r--r--   0        0        0     5858 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/reference_data_code.py
--rw-r--r--   0        0        0     1610 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/references.py
--rw-r--r--   0        0        0     1170 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/requirement.py
--rw-r--r--   0        0        0     1251 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/rule.py
--rw-r--r--   0        0        0     1605 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/skos_concept.py
--rw-r--r--   0        0        0     1049 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/spatial.py
--rw-r--r--   0        0        0      965 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/subject.py
--rw-r--r--   0        0        0     2540 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/temporal.py
--rw-r--r--   0        0        0     2891 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/theme.py
--rw-r--r--   0        0        0      787 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/rdf_utils/__init__.py
--rw-r--r--   0        0        0     3624 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/rdf_utils/ns.py
--rw-r--r--   0        0        0     4335 2024-04-04 07:42:04.689082 fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/rdf_utils/utils.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/LICENSE
+-rw-r--r--   0        0        0     1248 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0      473 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/__init__.py
+-rw-r--r--   0        0        0     1587 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/address.py
+-rw-r--r--   0        0        0      342 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/agent.py
+-rw-r--r--   0        0        0      766 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/business_event.py
+-rw-r--r--   0        0        0      336 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/catalog.py
+-rw-r--r--   0        0        0      610 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/channel.py
+-rw-r--r--   0        0        0     2885 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/concept.py
+-rw-r--r--   0        0        0      189 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/conforms_to.py
+-rw-r--r--   0        0        0      750 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/contactpoint.py
+-rw-r--r--   0        0        0      436 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/cost.py
+-rw-r--r--   0        0        0     2449 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/cpsvno_service.py
+-rw-r--r--   0        0        0      356 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/data_distribution_service.py
+-rw-r--r--   0        0        0     1668 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dataservice.py
+-rw-r--r--   0        0        0     8657 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dataset.py
+-rw-r--r--   0        0        0     1143 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dcat_resource.py
+-rw-r--r--   0        0        0      274 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dct_standard.py
+-rw-r--r--   0        0        0      924 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/distribution.py
+-rw-r--r--   0        0        0      777 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/event.py
+-rw-r--r--   0        0        0      758 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/evidence.py
+-rw-r--r--   0        0        0      355 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/exceptions.py
+-rw-r--r--   0        0        0      349 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/format.py
+-rw-r--r--   0        0        0      174 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/harvest_meta_data.py
+-rw-r--r--   0        0        0     3478 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/info_model.py
+-rw-r--r--   0        0        0      331 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/legal_resource.py
+-rw-r--r--   0        0        0      758 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/life_event.py
+-rw-r--r--   0        0        0      402 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/media_type.py
+-rw-r--r--   0        0        0     1910 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/model_element.py
+-rw-r--r--   0        0        0     1147 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/model_property.py
+-rw-r--r--   0        0        0      430 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/organization.py
+-rw-r--r--   0        0        0      466 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/output.py
+-rw-r--r--   0        0        0      376 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/participation.py
+-rw-r--r--   0        0        0     1888 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/public_service.py
+-rw-r--r--   0        0        0      326 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/publisher.py
+-rw-r--r--   0        0        0      206 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/qualified_attribution.py
+-rw-r--r--   0        0        0      202 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/quality_annotation.py
+-rw-r--r--   0        0        0      227 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/reference_data_code.py
+-rw-r--r--   0        0        0      277 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/references.py
+-rw-r--r--   0        0        0      412 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/requirement.py
+-rw-r--r--   0        0        0      424 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/rule.py
+-rw-r--r--   0        0        0      317 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/skos_concept.py
+-rw-r--r--   0        0        0      271 2024-05-14 08:28:01.764216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/subject.py
+-rw-r--r--   0        0        0      191 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/temporal.py
+-rw-r--r--   0        0        0      610 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/theme.py
+-rw-r--r--   0        0        0      506 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/types.py
+-rw-r--r--   0        0        0     8796 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/fdk_rdf_parser.py
+-rw-r--r--   0        0        0     1349 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/__init__.py
+-rw-r--r--   0        0        0     1070 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/address.py
+-rw-r--r--   0        0        0     2175 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/agent.py
+-rw-r--r--   0        0        0     1153 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/catalog.py
+-rw-r--r--   0        0        0     1739 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/channel.py
+-rw-r--r--   0        0        0    15032 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/concept.py
+-rw-r--r--   0        0        0      992 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/conforms_to.py
+-rw-r--r--   0        0        0     3172 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/contactpoint.py
+-rw-r--r--   0        0        0     1336 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/cost.py
+-rw-r--r--   0        0        0     6030 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/cpsvno_service.py
+-rw-r--r--   0        0        0     1555 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/data_distribution_service.py
+-rw-r--r--   0        0        0     1671 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dataservice.py
+-rw-r--r--   0        0        0     9262 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dataset.py
+-rw-r--r--   0        0        0     2928 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dcat_resource.py
+-rw-r--r--   0        0        0      979 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dct_standard.py
+-rw-r--r--   0        0        0     2051 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/distribution.py
+-rw-r--r--   0        0        0     3093 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/event.py
+-rw-r--r--   0        0        0     2018 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/evidence.py
+-rw-r--r--   0        0        0     1116 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/format.py
+-rw-r--r--   0        0        0      422 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/harvest_meta_data.py
+-rw-r--r--   0        0        0     6492 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/info_model.py
+-rw-r--r--   0        0        0     1047 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/legal_resource.py
+-rw-r--r--   0        0        0     3338 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/media_type.py
+-rw-r--r--   0        0        0     4432 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/model_element.py
+-rw-r--r--   0        0        0     3439 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/model_property.py
+-rw-r--r--   0        0        0     2623 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/organization.py
+-rw-r--r--   0        0        0     1247 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/output.py
+-rw-r--r--   0        0        0      816 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/participation.py
+-rw-r--r--   0        0        0     2155 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/publisher.py
+-rw-r--r--   0        0        0      911 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/qualified_attribution.py
+-rw-r--r--   0        0        0     1451 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/quality_annotation.py
+-rw-r--r--   0        0        0     5858 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/reference_data_code.py
+-rw-r--r--   0        0        0     1610 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/references.py
+-rw-r--r--   0        0        0     1170 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/requirement.py
+-rw-r--r--   0        0        0     1251 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/rule.py
+-rw-r--r--   0        0        0     1605 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/skos_concept.py
+-rw-r--r--   0        0        0     1049 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/spatial.py
+-rw-r--r--   0        0        0      965 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/subject.py
+-rw-r--r--   0        0        0     2540 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/temporal.py
+-rw-r--r--   0        0        0     2891 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/theme.py
+-rw-r--r--   0        0        0      831 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/rdf_utils/__init__.py
+-rw-r--r--   0        0        0     3518 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/rdf_utils/ns.py
+-rw-r--r--   0        0        0     4675 2024-05-14 08:28:01.768216 fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/rdf_utils/utils.py
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.7.1/PKG-INFO
```

### Comparing `fdk_rdf_parser-2.7.0/LICENSE` & `fdk_rdf_parser-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/pyproject.toml` & `fdk_rdf_parser-2.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "fdk-rdf-parser"
-version = "2.7.0"
+version = "2.7.1"
 description = ""
 authors = ["NilsOveTen <nils.ove.tendenes@digdir.no>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 rdflib = "^7.0.0"
 isodate = "^0.6.1"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^8.0.0"
-coverage = {extras = ["toml"], version = "^7.4.1"}
-pytest-cov = "^4.1.0"
-black = "^24.3.0"
+pytest = "^8.2.0"
+coverage = {extras = ["toml"], version = "^7.5.0"}
+pytest-cov = "^5.0.0"
+black = "^24.4.2"
 flake8 = "^7.0.0"
 flake8-bandit = "^4.1.1"
 flake8-black = "^0.3.6"
-flake8-bugbear = "^24.1.17"
+flake8-bugbear = "^24.4.26"
 flake8-import-order = "^0.18.2"
 pep8-naming = "^0.13.3"
-safety = "^3.0.1"
-pytest-mock = "^3.12.0"
+safety = "^3.1.0"
+pytest-mock = "^3.14.0"
 codecov = "^2.1.13"
 flake8-annotations = "^3.0.1"
-mypy = "^1.8.0"
-nox = "^2024.3.2"
+mypy = "^1.10.0"
+nox = "^2024.4.15"
 nox-poetry = "^1.0.3"
 
 [tool.coverage.paths]
 source = ["src"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/__init__.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/business_event.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/business_event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/channel.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/channel.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/concept.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/concept.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     uri: Optional[str] = None
     text: Optional[Dict[str, str]] = None
 
 
 @dataclass
 class Definition:
     text: Optional[Dict[str, str]] = None
-    remark: Optional[Dict[str, str]] = None
+    remark: Optional[Dict[str, str]] = None  # Deprecated
     targetGroup: Optional[str] = None
     sourceRelationship: Optional[str] = None
-    range: Optional[TextAndURI] = None
+    range: Optional[TextAndURI] = None  # Deprecated
     sources: Optional[List[TextAndURI]] = None
     lastUpdated: Optional[str] = None
 
 
 @dataclass
 class AssociativeRelation:
     description: Optional[Dict[str, str]] = None
@@ -75,20 +75,23 @@
     application: Optional[List[Dict[str, str]]] = None
     example: Optional[Dict[str, str]] = None
     prefLabel: Optional[Dict[str, str]] = None
     hiddenLabel: Optional[List[Dict[str, str]]] = None
     altLabel: Optional[List[Dict[str, str]]] = None
     contactPoint: Optional[DCATContactPoint] = None
     definition: Optional[Definition] = None
+    definitions: Optional[List[Definition]] = None
     seeAlso: Optional[Set[str]] = None
     isReplacedBy: Optional[Set[str]] = None
     replaces: Optional[Set[str]] = None
     validFromIncluding: Optional[str] = None
     validToIncluding: Optional[str] = None
     associativeRelation: Optional[List[AssociativeRelation]] = None
     partitiveRelation: Optional[List[PartitiveRelation]] = None
     genericRelation: Optional[List[GenericRelation]] = None
     created: Optional[str] = None
     exactMatch: Optional[Set[str]] = None
     closeMatch: Optional[Set[str]] = None
     memberOf: Optional[Set[str]] = None
+    remark: Optional[List[Dict[str, str]]] = None
+    range: Optional[List[TextAndURI]] = None
     type: str = "concept"  # used by elasticsearch for indexing
```

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/contactpoint.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/cpsvno_service.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/cpsvno_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dataservice.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dataservice.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dataset.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/dcat_resource.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/dcat_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/distribution.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/distribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/event.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/evidence.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/evidence.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/info_model.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/info_model.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/life_event.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/life_event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/model_element.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/model_element.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/model_property.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/model_property.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/public_service.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/public_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/classes/theme.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/classes/theme.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/fdk_rdf_parser.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/fdk_rdf_parser.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/__init__.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/address.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/address.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/agent.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/agent.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/catalog.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/catalog.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/channel.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/channel.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/concept.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/concept.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,16 @@
     List,
     Optional,
 )
 
 from rdflib import (
     BNode,
     Graph,
+    Literal,
+    RDF,
     URIRef,
 )
 from rdflib.namespace import (
     DCTERMS,
     FOAF,
     RDFS,
     SKOS,
@@ -29,17 +31,19 @@
     Subject,
     TextAndURI,
 )
 from fdk_rdf_parser.rdf_utils import (
     date_value,
     dcat_uri,
     euvoc_uri,
+    has_literal_value_on_predicate,
+    has_value_on_predicate,
     is_type,
     object_value,
-    skosno_old_uri,
+    resource_list,
     skosno_uri,
     skosxl_uri,
     uneskos_uri,
     value_set,
     value_translations,
     xkos_uri_v_2,
 )
@@ -52,30 +56,64 @@
 def parse_text_and_uri(graph: Graph, subject: URIRef) -> TextAndURI:
     return TextAndURI(
         text=value_translations(graph, subject, RDFS.label),
         uri=object_value(graph, subject, RDFS.seeAlso),
     )
 
 
-def extract_range(graph: Graph, definition_ref: URIRef) -> Optional[TextAndURI]:
+def extract_range_deprecated(
+    graph: Graph, definition_ref: URIRef
+) -> Optional[TextAndURI]:
     range_list = []
     for range_ref in graph.objects(definition_ref, skosno_uri("omfang")):
         range_list.append(parse_text_and_uri(graph, range_ref))
-    for range_ref in graph.objects(definition_ref, skosno_old_uri("omfang")):
-        range_list.append(parse_text_and_uri(graph, range_ref))
     return range_list[0] if len(range_list) == 1 else None
 
 
-def extract_sources(graph: Graph, definition_ref: URIRef) -> Optional[List[TextAndURI]]:
+def extract_range(graph: Graph, definition_ref: URIRef) -> Optional[List[TextAndURI]]:
+    range_list = []
+    for range_obj in graph.objects(definition_ref, skosno_uri("valueRange")):
+        value = TextAndURI()
+        if isinstance(range_obj, URIRef):
+            value.uri = range_obj.toPython()
+        elif isinstance(range_obj, Literal):
+            if range_obj.language:
+                value.text = {range_obj.language: range_obj.toPython()}
+            else:
+                value.text = {"nb": range_obj.toPython()}
+        if value.uri is not None or value.text is not None:
+            range_list.append(value)
+    return range_list if len(range_list) > 0 else None
+
+
+def extract_sources_deprecated(
+    graph: Graph, definition_ref: URIRef
+) -> Optional[List[TextAndURI]]:
     sources = []
     for source_ref in graph.objects(definition_ref, DCTERMS.source):
         sources.append(parse_text_and_uri(graph, source_ref))
     return sources if len(sources) > 0 else None
 
 
+def extract_sources(graph: Graph, definition_ref: URIRef) -> Optional[List[TextAndURI]]:
+    sources = []
+    for source_ref in graph.objects(definition_ref, DCTERMS.source):
+        sources.append(
+            TextAndURI(
+                text=None,
+                uri=(
+                    source_ref.toPython()
+                    if source_ref and not isinstance(source_ref, BNode)
+                    else None
+                ),
+            )
+        )
+    return sources if len(sources) > 0 else None
+
+
 def extract_subjects(graph: Graph, concept_ref: URIRef) -> Optional[List[Subject]]:
     subjects = []
     for subject_node in graph.objects(concept_ref, DCTERMS.subject):
         label: Optional[Dict[str, str]]
         if isinstance(subject_node, BNode) or isinstance(subject_node, URIRef):
             label = value_translations(graph, subject_node, SKOS.prefLabel)
         else:
@@ -98,89 +136,155 @@
             if subject_node.language:
                 status[subject_node.language] = subject_node.toPython()
             else:
                 status["nb"] = subject_node.toPython()
     return status if len(status) > 0 else None
 
 
-def extract_target_group(graph: Graph, definition_ref: URIRef) -> Optional[str]:
+def extract_target_group_deprecated(
+    graph: Graph, definition_ref: URIRef
+) -> Optional[str]:
     uri = object_value(graph, definition_ref, DCTERMS.audience)
     if not uri:
         return None
     if "allmennheten" in uri:
         return "allmennheten"
     elif "fagspesialist" in uri:
         return "fagspesialist"
     else:
         return None
 
 
-def extract_source_relationship(graph: Graph, definition_ref: URIRef) -> Optional[str]:
+def extract_source_relationship_deprecated(
+    graph: Graph, definition_ref: URIRef
+) -> Optional[str]:
     uri = object_value(graph, definition_ref, skosno_uri("forholdTilKilde"))
-    uri = (
-        uri
-        if uri
-        else object_value(graph, definition_ref, skosno_old_uri("forholdTilKilde"))
-    )
     if not uri:
         return None
     if "sitatFraKilde" in uri:
         return "sitatFraKilde"
     elif "basertPåKilde" in uri:
         return "basertPåKilde"
     elif "egendefinert" in uri:
         return "egendefinert"
     else:
         return None
 
 
-def parse_definition(graph: Graph, definition_ref: URIRef) -> Definition:
+def parse_definition_deprecated(graph: Graph, definition_ref: URIRef) -> Definition:
     return Definition(
         text=value_translations(graph, definition_ref, RDFS.label),
         remark=value_translations(graph, definition_ref, SKOS.scopeNote),
-        targetGroup=extract_target_group(graph, definition_ref),
-        sourceRelationship=extract_source_relationship(graph, definition_ref),
-        range=extract_range(graph, definition_ref),
+        targetGroup=extract_target_group_deprecated(graph, definition_ref),
+        sourceRelationship=extract_source_relationship_deprecated(
+            graph, definition_ref
+        ),
+        range=extract_range_deprecated(graph, definition_ref),
+        sources=extract_sources_deprecated(graph, definition_ref),
+    )
+
+
+def parse_euvoc_definition(graph: Graph, definition_ref: URIRef) -> Definition:
+    return Definition(
+        text=value_translations(graph, definition_ref, RDF.value),
+        targetGroup=object_value(graph, definition_ref, DCTERMS.audience),
+        sourceRelationship=object_value(
+            graph, definition_ref, skosno_uri("relationshipWithSource")
+        ),
         sources=extract_sources(graph, definition_ref),
-        lastUpdated=date_value(graph, definition_ref, DCTERMS.modified),
     )
 
 
-def extract_definition(graph: Graph, concept_uri: URIRef) -> Optional[Definition]:
-    definitions = []
-    for definition_ref in graph.objects(concept_uri, skosno_uri("definisjon")):
-        definitions.append(parse_definition(graph, definition_ref))
-    for definition_ref in graph.objects(
-        concept_uri, skosno_old_uri("betydningsbeskrivelse")
-    ):
-        definitions.append(parse_definition(graph, definition_ref))
-    return definitions[0] if len(definitions) > 0 else None
+def parse_skos_definition(graph: Graph, concept_ref: URIRef) -> Definition:
+    return Definition(text=value_translations(graph, concept_ref, SKOS.definition))
 
 
-def parse_associative_relation(
+def extract_definitions(
+    graph: Graph, concept_uri: URIRef
+) -> Optional[List[Definition]]:
+    definitions: List[Definition] = list()
+    if has_value_on_predicate(graph, concept_uri, euvoc_uri("xlDefinition")):
+        for definition_ref in resource_list(
+            graph, concept_uri, euvoc_uri("xlDefinition")
+        ):
+            definitions.append(parse_euvoc_definition(graph, definition_ref))
+    elif has_value_on_predicate(graph, concept_uri, SKOS.definition):
+        definitions.append(parse_skos_definition(graph, concept_uri))
+    else:
+        for definition_ref in resource_list(
+            graph, concept_uri, skosno_uri("definisjon")
+        ):
+            definitions.append(parse_definition_deprecated(graph, definition_ref))
+
+    if definitions:
+        return definitions
+    return None
+
+
+def definition_has_not_target_group(definition: Definition) -> bool:
+    if definition.targetGroup is None:
+        return True
+    else:
+        return False
+
+
+def get_first_definition_with_no_target_group(
+    definitions: Optional[List[Definition]],
+) -> Optional[Definition]:
+    if definitions is not None:
+        filtered_definitions = list(
+            filter(definition_has_not_target_group, definitions)
+        )
+        if filtered_definitions:
+            return filtered_definitions[0]
+        else:
+            return definitions[0]
+    else:
+        return None
+
+
+def parse_associative_relation_deprecated(
     graph: Graph, associative_relation_ref: URIRef
 ) -> AssociativeRelation:
     return AssociativeRelation(
         description=value_translations(
             graph, associative_relation_ref, DCTERMS.description
         ),
         related=object_value(graph, associative_relation_ref, SKOS.related),
     )
 
 
+def parse_associative_relation(
+    graph: Graph, associative_relation_ref: URIRef
+) -> AssociativeRelation:
+    return AssociativeRelation(
+        description=value_translations(
+            graph, associative_relation_ref, skosno_uri("relationRole")
+        ),
+        related=object_value(graph, associative_relation_ref, SKOS.related),
+    )
+
+
 def extract_associative_relations(
     graph: Graph, concept_uri: URIRef
 ) -> Optional[List[AssociativeRelation]]:
     associative_relations = []
     for associative_relation_ref in graph.objects(
         concept_uri, skosno_uri("assosiativRelasjon")
     ):
-        associative_relations.append(
-            parse_associative_relation(graph, associative_relation_ref)
-        )
+        if has_value_on_predicate(
+            graph, associative_relation_ref, skosno_uri("relationRole")
+        ):
+            associative_relations.append(
+                parse_associative_relation(graph, associative_relation_ref)
+            )
+        else:
+            associative_relations.append(
+                parse_associative_relation_deprecated(graph, associative_relation_ref)
+            )
     return associative_relations if len(associative_relations) > 0 else None
 
 
 def parse_partitive_relation(
     graph: Graph, partitive_relation_ref: URIRef
 ) -> PartitiveRelation:
     return PartitiveRelation(
@@ -249,78 +353,76 @@
                 description=value_translations(
                     graph, collection_uri, DCTERMS.description
                 ),
             )
     return None
 
 
-def create_application_language_dict(application: URIRef) -> Dict[str, str]:
-    dict = {}
-    if application.language:
-        dict[application.language] = application.toPython()
-    else:
-        dict["nb"] = application.toPython()
-    return dict
-
-
-def parse_applications(
-    graph: Graph, concept_uri: URIRef
+def extract_labels(
+    graph: Graph, concept_uri: URIRef, predicate: URIRef, predicate_deprecated: URIRef
 ) -> Optional[List[Dict[str, str]]]:
-    applications = []
-    for application in graph.objects(concept_uri, skosno_uri("bruksområde")):
-        applications.append(create_application_language_dict(application))
-    for application in graph.objects(concept_uri, skosno_old_uri("bruksområde")):
-        applications.append(create_application_language_dict(application))
-    return applications if len(applications) > 0 else None
+    labels = list()
+    if has_literal_value_on_predicate(graph, concept_uri, predicate):
+        main_labels = value_translations(graph, concept_uri, predicate)
+        labels.append(main_labels) if main_labels is not None else None
+
+    else:
+        deprecated_labels = [
+            value_translations(graph, label, skosxl_uri("literalForm"))
+            for label in graph.objects(concept_uri, predicate_deprecated)
+        ]
 
+        for label in deprecated_labels:
+            labels.append(label) if label is not None else None
 
-def parse_label_set(
-    graph: Graph, concept_uri: URIRef, predicate: URIRef
-) -> Optional[List[Dict[str, str]]]:
-    values = []
-    for label in graph.objects(concept_uri, predicate):
-        literal_form = value_translations(graph, label, skosxl_uri("literalForm"))
-        if literal_form:
-            values.append(literal_form)
-    return values if len(values) > 0 else None
+    return labels if len(labels) > 0 else None
 
 
 def _parse_concept(
     graph: Graph, fdk_record_uri: URIRef, concept_uri: URIRef
 ) -> Concept:
     concept_temporal_list = extract_temporal(graph, concept_uri)
     concept_temporal = concept_temporal_list[0] if concept_temporal_list else Temporal()
     contact_points = extract_contact_points(graph, concept_uri)
 
-    pref_label_list = parse_label_set(graph, concept_uri, skosxl_uri("prefLabel"))
+    pref_label_list = extract_labels(
+        graph, concept_uri, SKOS.prefLabel, skosxl_uri("prefLabel")
+    )
+    definition_list = extract_definitions(graph, concept_uri)
 
     return Concept(
         id=object_value(graph, fdk_record_uri, DCTERMS.identifier),
         uri=fdk_record_uri.toPython() if fdk_record_uri else None,
         identifier=concept_uri.toPython() if concept_uri else None,
         harvest=extract_meta_data(graph, fdk_record_uri),
         collection=parse_collection(graph, fdk_record_uri),
         publisher=extract_publisher(graph, concept_uri),
         subject=extract_subjects(graph, concept_uri),
         status=extract_status(graph, concept_uri),
-        application=parse_applications(graph, concept_uri),
         example=value_translations(graph, concept_uri, SKOS.example),
         prefLabel=(
             pref_label_list[0] if pref_label_list and len(pref_label_list) > 0 else None
         ),
-        hiddenLabel=parse_label_set(graph, concept_uri, skosxl_uri("hiddenLabel")),
-        altLabel=parse_label_set(graph, concept_uri, skosxl_uri("altLabel")),
+        hiddenLabel=extract_labels(
+            graph, concept_uri, SKOS.hiddenLabel, skosxl_uri("hiddenLabel")
+        ),
+        altLabel=extract_labels(
+            graph, concept_uri, SKOS.altLabel, skosxl_uri("altLabel")
+        ),
         contactPoint=contact_points[0] if contact_points else None,
-        definition=extract_definition(graph, concept_uri),
+        definition=get_first_definition_with_no_target_group(definition_list),
+        definitions=definition_list,
         seeAlso=value_set(graph, concept_uri, RDFS.seeAlso),
         isReplacedBy=value_set(graph, concept_uri, DCTERMS.isReplacedBy),
         replaces=value_set(graph, concept_uri, DCTERMS.replaces),
         validFromIncluding=concept_temporal.startDate,
         validToIncluding=concept_temporal.endDate,
         associativeRelation=extract_associative_relations(graph, concept_uri),
         partitiveRelation=extract_partitive_relations(graph, concept_uri),
         genericRelation=extract_generic_relations(graph, concept_uri),
         created=date_value(graph, concept_uri, DCTERMS.created),
         exactMatch=value_set(graph, concept_uri, SKOS.exactMatch),
         closeMatch=value_set(graph, concept_uri, SKOS.closeMatch),
         memberOf=value_set(graph, concept_uri, uneskos_uri("memberOf")),
+        remark=extract_labels(graph, concept_uri, SKOS.scopeNote, SKOS.scopeNote),
+        range=extract_range(graph, concept_uri),
     )
```

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/conforms_to.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/conforms_to.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/contactpoint.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/cost.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/cost.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/cpsvno_service.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/cpsvno_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/data_distribution_service.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/data_distribution_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dataservice.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dataservice.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dataset.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dataset.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dcat_resource.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dcat_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/dct_standard.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/dct_standard.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/distribution.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/distribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/event.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/evidence.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/evidence.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/format.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/format.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/info_model.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/info_model.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/legal_resource.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/legal_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/media_type.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/media_type.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/model_element.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/model_element.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/model_property.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/model_property.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/organization.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/organization.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/output.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/output.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/participation.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/participation.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/publisher.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/publisher.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/qualified_attribution.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/qualified_attribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/quality_annotation.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/quality_annotation.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/reference_data_code.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/reference_data_code.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/references.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/references.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/requirement.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/requirement.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/rule.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/rule.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/skos_concept.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/skos_concept.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/spatial.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/spatial.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/subject.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/subject.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/temporal.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/temporal.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/parse_functions/theme.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/parse_functions/theme.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/rdf_utils/ns.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/rdf_utils/ns.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,18 +93,14 @@
     return URIRef(f"https://data.norge.no/vocabulary/cpsvno#{sub_string}")
 
 
 def skosno_uri(sub_string: str) -> URIRef:
     return URIRef(f"https://data.norge.no/vocabulary/skosno#{sub_string}")
 
 
-def skosno_old_uri(sub_string: str) -> URIRef:
-    return URIRef(f"http://difi.no/skosno#{sub_string}")
-
-
 def skosxl_uri(sub_string: str) -> URIRef:
     return URIRef(f"http://www.w3.org/2008/05/skos-xl#{sub_string}")
 
 
 def oa_uri(sub_string: str) -> URIRef:
     return URIRef(f"http://www.w3.org/ns/oa#{sub_string}")
```

### Comparing `fdk_rdf_parser-2.7.0/src/fdk_rdf_parser/rdf_utils/utils.py` & `fdk_rdf_parser-2.7.1/src/fdk_rdf_parser/rdf_utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from isodate import (
     date_isoformat,
     datetime_isoformat,
 )
 from rdflib import (
     BNode,
     Graph,
+    Literal,
     URIRef,
 )
 from rdflib.namespace import (
     DCTERMS,
     RDF,
 )
 
@@ -31,14 +32,25 @@
     for type_uri_ref in resource_list(graph, topic, RDF.type):
         if type_uri_ref == t:
             return True
 
     return False
 
 
+def has_value_on_predicate(graph: Graph, subject: URIRef, predicate: URIRef) -> bool:
+    return graph.value(subject, predicate) is not None
+
+
+def has_literal_value_on_predicate(
+    graph: Graph, subject: URIRef, predicate: URIRef
+) -> bool:
+    value = graph.value(subject, predicate)
+    return isinstance(value, Literal)
+
+
 def object_value(graph: Graph, subject: URIRef, predicate: URIRef) -> Optional[Any]:
     value = graph.value(subject, predicate)
     return value.toPython() if value and not isinstance(value, BNode) else None
 
 
 def duration_string_value(
     graph: Graph, subject: URIRef, predicate: URIRef
```

### Comparing `fdk_rdf_parser-2.7.0/PKG-INFO` & `fdk_rdf_parser-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdk-rdf-parser
-Version: 2.7.0
+Version: 2.7.1
 Summary: 
 Author: NilsOveTen
 Author-email: nils.ove.tendenes@digdir.no
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

