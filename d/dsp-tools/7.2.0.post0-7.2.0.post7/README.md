# Comparing `tmp/dsp_tools-7.2.0.post0.tar.gz` & `tmp/dsp_tools-7.2.0.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-7.2.0.post0.tar", max compression
+gzip compressed data, was "dsp_tools-7.2.0.post7.tar", max compression
```

## Comparing `dsp_tools-7.2.0.post0.tar` & `dsp_tools-7.2.0.post7.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0    35149 2024-05-08 08:29:26.522178 dsp_tools-7.2.0.post0/LICENSE
--rw-r--r--   0        0        0     4941 2024-05-08 08:29:26.538178 dsp_tools-7.2.0.post0/docs/index.md
--rw-r--r--   0        0        0     8372 2024-05-08 08:29:57.150147 dsp_tools-7.2.0.post0/pyproject.toml
--rw-r--r--   0        0        0       41 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/cli/__init__.py
--rw-r--r--   0        0        0     8102 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/cli/call_action.py
--rw-r--r--   0        0        0    13719 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/cli/create_parsers.py
--rw-r--r--   0        0        0     9909 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/cli/entry_point.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/__init__.py
--rw-r--r--   0        0        0    15987 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/lists.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/models/__init__.py
--rw-r--r--   0        0        0    14898 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/models/input_error.py
--rw-r--r--   0        0        0     4018 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/models/list_node.py
--rw-r--r--   0        0        0      501 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/models/list_node_name.py
--rw-r--r--   0        0        0    29990 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/new_lists.py
--rw-r--r--   0        0        0     9829 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/project.py
--rw-r--r--   0        0        0    13232 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/properties.py
--rw-r--r--   0        0        0    11887 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/resources.py
--rw-r--r--   0        0        0    11866 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/utils.py
--rw-r--r--   0        0        0      466 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2xml/__init__.py
--rw-r--r--   0        0        0    21324 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
--rw-r--r--   0        0        0    80279 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
--rw-r--r--   0        0        0     1981 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2xml/propertyelement.py
--rw-r--r--   0        0        0     8275 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/id2iri.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/ingest_xmlupload/__init__.py
--rw-r--r--   0        0        0     2876 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
--rw-r--r--   0        0        0     2351 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
--rw-r--r--   0        0        0     4891 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/ingest_xmlupload/user_information.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/create/__init__.py
--rw-r--r--   0        0        0    45642 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/create/project_create.py
--rw-r--r--   0        0        0     8243 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/create/project_create_lists.py
--rw-r--r--   0        0        0    19703 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/create/project_validate.py
--rw-r--r--   0        0        0     5743 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/get.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/__init__.py
--rw-r--r--   0        0        0    12173 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/context.py
--rw-r--r--   0        0        0     8379 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/group.py
--rw-r--r--   0        0        0      850 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/helpers.py
--rw-r--r--   0        0        0    14910 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/listnode.py
--rw-r--r--   0        0        0      245 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/model.py
--rw-r--r--   0        0        0    12710 2024-05-08 08:29:26.542178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/ontology.py
--rw-r--r--   0        0        0    11594 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/project.py
--rw-r--r--   0        0        0      306 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/project_definition.py
--rw-r--r--   0        0        0    17215 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/propertyclass.py
--rw-r--r--   0        0        0    28164 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/resourceclass.py
--rw-r--r--   0        0        0    17030 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/user.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/resume_xmlupload/__init__.py
--rw-r--r--   0        0        0     4200 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
--rw-r--r--   0        0        0     4177 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/rosetta.py
--rw-r--r--   0        0        0    16102 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/start_stack.py
--rw-r--r--   0        0        0     1134 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/template.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/__init__.py
--rw-r--r--   0        0        0     2350 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/ark2iri.py
--rw-r--r--   0        0        0    10356 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
--rw-r--r--   0        0        0      625 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/iri_resolver.py
--rw-r--r--   0        0        0     3587 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/list_client.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/__init__.py
--rw-r--r--   0        0        0     1334 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
--rw-r--r--   0        0        0     5549 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
--rw-r--r--   0        0        0     6752 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
--rw-r--r--   0        0        0     2388 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/permission.py
--rw-r--r--   0        0        0      812 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/sipi.py
--rw-r--r--   0        0        0      675 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/upload_state.py
--rw-r--r--   0        0        0     2236 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/xmlallow.py
--rw-r--r--   0        0        0      548 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py
--rw-r--r--   0        0        0     1437 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/xmlpermission.py
--rw-r--r--   0        0        0     2026 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/xmlproperty.py
--rw-r--r--   0        0        0     5164 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/xmlresource.py
--rw-r--r--   0        0        0     4004 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/xmlvalue.py
--rw-r--r--   0        0        0     3466 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/ontology_client.py
--rw-r--r--   0        0        0     3063 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/project_client.py
--rw-r--r--   0        0        0     4653 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
--rw-r--r--   0        0        0    13392 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/resource_create_client.py
--rw-r--r--   0        0        0     4585 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/resource_multimedia.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/__init__.py
--rw-r--r--   0        0        0    12372 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
--rw-r--r--   0        0        0     2452 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/graph_models.py
--rw-r--r--   0        0        0     5724 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
--rw-r--r--   0        0        0     3068 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/stash_models.py
--rw-r--r--   0        0        0     4237 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
--rw-r--r--   0        0        0     7727 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
--rw-r--r--   0        0        0     2175 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/upload_config.py
--rw-r--r--   0        0        0      858 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
--rw-r--r--   0        0        0    22379 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/xmlupload.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0      949 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/models/custom_warnings.py
--rw-r--r--   0        0        0     2876 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/models/datetimestamp.py
--rw-r--r--   0        0        0     2663 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     8457 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0     1777 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/py.typed
--rw-r--r--   0        0        0     1488 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    29794 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2024-05-08 08:29:26.546178 dsp_tools-7.2.0.post0/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    42680 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    32411 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4240 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0       61 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/resources/start-stack/docker-compose.override.yml
--rw-r--r--   0        0        0     3281 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0      164 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/resources/start-stack/start-stack-config.yml
--rw-r--r--   0        0        0        0 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0     1030 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/connection.py
--rw-r--r--   0        0        0    14126 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/connection_live.py
--rw-r--r--   0        0        0     4554 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/date_util.py
--rw-r--r--   0        0        0      457 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/iri_util.py
--rw-r--r--   0        0        0      893 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/json_ld_util.py
--rw-r--r--   0        0        0     1157 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/logger_config.py
--rw-r--r--   0        0        0      705 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/set_encoder.py
--rw-r--r--   0        0        0     5754 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0      547 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/uri_util.py
--rw-r--r--   0        0        0      978 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/warnings_config.py
--rw-r--r--   0        0        0     4920 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/xml_utils.py
--rw-r--r--   0        0        0     7359 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/xml_validation.py
--rw-r--r--   0        0        0     2312 2024-05-08 08:29:26.550178 dsp_tools-7.2.0.post0/src/dsp_tools/utils/xml_validation_models.py
--rw-r--r--   0        0        0     6312 1970-01-01 00:00:00.000000 dsp_tools-7.2.0.post0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-14 11:55:58.687635 dsp_tools-7.2.0.post7/LICENSE
+-rw-r--r--   0        0        0     4941 2024-05-14 11:55:58.703635 dsp_tools-7.2.0.post7/docs/index.md
+-rw-r--r--   0        0        0     8406 2024-05-14 11:56:27.899950 dsp_tools-7.2.0.post7/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/__init__.py
+-rw-r--r--   0        0        0     8102 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/call_action.py
+-rw-r--r--   0        0        0    13719 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/create_parsers.py
+-rw-r--r--   0        0        0     9909 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/entry_point.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/__init__.py
+-rw-r--r--   0        0        0    15987 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/lists.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/__init__.py
+-rw-r--r--   0        0        0    14898 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/input_error.py
+-rw-r--r--   0        0        0     4018 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/list_node.py
+-rw-r--r--   0        0        0      501 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/list_node_name.py
+-rw-r--r--   0        0        0    29990 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/new_lists.py
+-rw-r--r--   0        0        0     9829 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/project.py
+-rw-r--r--   0        0        0    13232 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/properties.py
+-rw-r--r--   0        0        0    11887 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/resources.py
+-rw-r--r--   0        0        0    11866 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/utils.py
+-rw-r--r--   0        0        0      466 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/__init__.py
+-rw-r--r--   0        0        0    21361 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
+-rw-r--r--   0        0        0    80208 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
+-rw-r--r--   0        0        0     1981 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/propertyelement.py
+-rw-r--r--   0        0        0     8275 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/id2iri.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/__init__.py
+-rw-r--r--   0        0        0     2876 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
+-rw-r--r--   0        0        0     2351 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0     4891 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/user_information.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/__init__.py
+-rw-r--r--   0        0        0    45642 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create.py
+-rw-r--r--   0        0        0     8243 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create_lists.py
+-rw-r--r--   0        0        0    19703 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_validate.py
+-rw-r--r--   0        0        0     5743 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/get.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/__init__.py
+-rw-r--r--   0        0        0    12173 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/context.py
+-rw-r--r--   0        0        0     8379 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/group.py
+-rw-r--r--   0        0        0      850 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/helpers.py
+-rw-r--r--   0        0        0    14910 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/listnode.py
+-rw-r--r--   0        0        0      245 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/model.py
+-rw-r--r--   0        0        0    12710 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/ontology.py
+-rw-r--r--   0        0        0    11594 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/project.py
+-rw-r--r--   0        0        0      306 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/project_definition.py
+-rw-r--r--   0        0        0    17215 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/propertyclass.py
+-rw-r--r--   0        0        0    28164 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/resourceclass.py
+-rw-r--r--   0        0        0    17030 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/user.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/resume_xmlupload/__init__.py
+-rw-r--r--   0        0        0     3719 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
+-rw-r--r--   0        0        0     4177 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/rosetta.py
+-rw-r--r--   0        0        0    16102 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/start_stack.py
+-rw-r--r--   0        0        0     1134 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/template.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/__init__.py
+-rw-r--r--   0        0        0     2350 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ark2iri.py
+-rw-r--r--   0        0        0    10356 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
+-rw-r--r--   0        0        0      625 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/iri_resolver.py
+-rw-r--r--   0        0        0     3587 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/list_client.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/__init__.py
+-rw-r--r--   0        0        0     6448 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/deserialise_value.py
+-rw-r--r--   0        0        0     3560 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/xmlpermission.py
+-rw-r--r--   0        0        0     5199 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/xmlresource.py
+-rw-r--r--   0        0        0     1334 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
+-rw-r--r--   0        0        0     1464 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/namespace_context.py
+-rw-r--r--   0        0        0     5549 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
+-rw-r--r--   0        0        0     6752 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
+-rw-r--r--   0        0        0     2388 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/permission.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/serialise/__init__.py
+-rw-r--r--   0        0        0     1302 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/serialise/serialise_value.py
+-rw-r--r--   0        0        0      812 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/sipi.py
+-rw-r--r--   0        0        0      730 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/upload_state.py
+-rw-r--r--   0        0        0     3466 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ontology_client.py
+-rw-r--r--   0        0        0     3140 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/project_client.py
+-rw-r--r--   0        0        0     4653 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
+-rw-r--r--   0        0        0    14771 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_create_client.py
+-rw-r--r--   0        0        0     4626 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_multimedia.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/__init__.py
+-rw-r--r--   0        0        0    12372 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
+-rw-r--r--   0        0        0     2452 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/graph_models.py
+-rw-r--r--   0        0        0     5754 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
+-rw-r--r--   0        0        0     3375 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_models.py
+-rw-r--r--   0        0        0     4158 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
+-rw-r--r--   0        0        0     7676 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
+-rw-r--r--   0        0        0     2175 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/upload_config.py
+-rw-r--r--   0        0        0      858 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
+-rw-r--r--   0        0        0    19191 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/xmlupload.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0      949 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/custom_warnings.py
+-rw-r--r--   0        0        0     2876 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/datetimestamp.py
+-rw-r--r--   0        0        0     2785 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     8457 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0     1777 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    29742 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    42680 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    32411 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4240 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0       61 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/docker-compose.override.yml
+-rw-r--r--   0        0        0     3281 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0      164 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/start-stack-config.yml
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0     1030 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection.py
+-rw-r--r--   0        0        0    14126 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection_live.py
+-rw-r--r--   0        0        0     4554 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/date_util.py
+-rw-r--r--   0        0        0      457 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/iri_util.py
+-rw-r--r--   0        0        0     1157 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/logger_config.py
+-rw-r--r--   0        0        0      705 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/set_encoder.py
+-rw-r--r--   0        0        0     5754 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0      547 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/uri_util.py
+-rw-r--r--   0        0        0      978 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/warnings_config.py
+-rw-r--r--   0        0        0     4920 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_utils.py
+-rw-r--r--   0        0        0     7359 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation.py
+-rw-r--r--   0        0        0     2312 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation_models.py
+-rw-r--r--   0        0        0     6388 1970-01-01 00:00:00.000000 dsp_tools-7.2.0.post7/PKG-INFO
```

### Comparing `dsp_tools-7.2.0.post0/LICENSE` & `dsp_tools-7.2.0.post7/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/docs/index.md` & `dsp_tools-7.2.0.post7/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/pyproject.toml` & `dsp_tools-7.2.0.post7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#writing-pyproject-toml
 
 [tool.poetry]
 name = "dsp-tools"
-version = "7.2.0.post0"
+version = "7.2.0.post7"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -33,14 +33,16 @@
 pandas = {version = "^2.2.1", extras = ["excel"]}  # extra package that contains xlrd that is necessary for reading old .xls Excel files
 regex = "^2024.4.28"
 pyyaml = "^6.0.1"
 rustworkx = "^0.14.2"
 termcolor = "^2.4.0"
 packaging = "^24.0"
 loguru = "^0.7.2"
+rdflib = "^7.0.0"
+pyld = "^2.0.4"
 
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.17"
 mkdocs-include-markdown-plugin = "^6.0.5"
 mypy = "^1.10.0"
@@ -51,15 +53,15 @@
 types-lxml = "^2024.3.27"
 types-jsonschema = "^4.21.0.20240331"
 types-openpyxl = "^3.1.0.20240402"
 types-regex = "^2024.4.28.20240430"
 types-pyyaml = "^6.0.12.20240311"
 pytest-unordered = "^0.6.0"
 viztracer = "^0.16.2"
-ruff = "^0.4.2"
+ruff = "^0.4.4"
 pytest-sugar = "^1.0.0"
 pandas-stubs = "^2.2.1.240316"
 types-networkx = "^3.2.1.20240331"
 
 
 [tool.poetry.scripts]
 dsp-tools = "dsp_tools.cli.entry_point:main"  # definition of the CLI entry point
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/cli/call_action.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/cli/call_action.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/cli/create_parsers.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/cli/create_parsers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/cli/entry_point.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/cli/entry_point.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/lists.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/models/input_error.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/input_error.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/models/list_node.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/list_node.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/new_lists.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/new_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/project.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/properties.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/properties.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/resources.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/resources.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2json/utils.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2xml/excel2xml_cli.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             permissions=str(file_permissions),
             calling_resource=row["id"],
         )
     )
     return resource
 
 
-def _convert_resource_row_to_xml(
+def _convert_resource_row_to_xml(  # noqa: PLR0912 (too-many-branches)
     row_number: int,
     row: pd.Series[Any],
 ) -> etree._Element:
     """
     Convert a resource-row to an XML resource element.
     First, check if the mandatory cells are present.
     Then, call the appropriate function, depending on the restype (Resource, LinkObj, Annotation, Region).
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2xml/excel2xml_lib.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -2715,2304 +2715,2299 @@
 0000a9a0: 7661 6c75 6520 6966 2069 7369 6e73 7461  value if isinsta
 0000a9b0: 6e63 6528 7661 6c75 652c 2050 726f 7065  nce(value, Prope
 0000a9c0: 7274 7945 6c65 6d65 6e74 2920 656c 7365  rtyElement) else
 0000a9d0: 2050 726f 7065 7274 7945 6c65 6d65 6e74   PropertyElement
 0000a9e0: 2876 616c 7565 290a 0a20 2020 2023 2063  (value)..    # c
 0000a9f0: 6865 636b 2076 616c 7565 2074 7970 650a  heck value type.
 0000aa00: 2020 2020 6966 206e 6f74 2072 6567 6578      if not regex
-0000aa10: 2e6d 6174 6368 280a 2020 2020 2020 2020  .match(.        
-0000aa20: 7222 285c 2b3f 285b 302d 395d 2b28 5b2e  r"(\+?([0-9]+([.
-0000aa30: 5d5b 302d 395d 2a29 3f7c 5b2e 5d5b 302d  ][0-9]*)?|[.][0-
-0000aa40: 395d 2b29 293a 285c 2b3f 285b 302d 395d  9]+)):(\+?([0-9]
-0000aa50: 2b28 5b2e 5d5b 302d 395d 2a29 3f7c 5b2e  +([.][0-9]*)?|[.
-0000aa60: 5d5b 302d 395d 2b29 2922 2c0a 2020 2020  ][0-9]+))",.    
-0000aa70: 2020 2020 7374 7228 7661 6c75 652e 7661      str(value.va
-0000aa80: 6c75 6529 2c0a 2020 2020 293a 0a20 2020  lue),.    ):.   
-0000aa90: 2020 2020 206d 7367 203d 2028 0a20 2020       msg = (.   
-0000aaa0: 2020 2020 2020 2020 2066 2246 6169 6c65           f"Faile
-0000aab0: 6420 7661 6c69 6461 7469 6f6e 2069 6e20  d validation in 
-0000aac0: 7265 736f 7572 6365 2027 7b63 616c 6c69  resource '{calli
-0000aad0: 6e67 5f72 6573 6f75 7263 657d 272c 2070  ng_resource}', p
-0000aae0: 726f 7065 7274 7920 277b 6e61 6d65 7d27  roperty '{name}'
-0000aaf0: 3a20 220a 2020 2020 2020 2020 2020 2020  : ".            
-0000ab00: 6622 277b 7661 6c75 652e 7661 6c75 657d  f"'{value.value}
-0000ab10: 2720 6973 206e 6f74 2061 2076 616c 6964  ' is not a valid
-0000ab20: 2044 5350 2069 6e74 6572 7661 6c2e 220a   DSP interval.".
-0000ab30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000ab40: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-0000ab50: 4473 7054 6f6f 6c73 5573 6572 5761 726e  DspToolsUserWarn
-0000ab60: 696e 6728 6d73 6729 290a 0a20 2020 2023  ing(msg))..    #
-0000ab70: 206d 616b 6520 786d 6c20 7374 7275 6374   make xml struct
-0000ab80: 7572 6520 6f66 2074 6865 2076 616c 6964  ure of the valid
-0000ab90: 2076 616c 7565 730a 2020 2020 7072 6f70   values.    prop
-0000aba0: 5f20 3d20 6574 7265 652e 456c 656d 656e  _ = etree.Elemen
-0000abb0: 7428 0a20 2020 2020 2020 2022 7b25 737d  t(.        "{%s}
-0000abc0: 696e 7465 7276 616c 2d70 726f 7022 2025  interval-prop" %
-0000abd0: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
-0000abe0: 6170 5b4e 6f6e 655d 2c0a 2020 2020 2020  ap[None],.      
-0000abf0: 2020 6e61 6d65 3d6e 616d 652c 0a20 2020    name=name,.   
-0000ac00: 2020 2020 206e 736d 6170 3d78 6d6c 5f6e       nsmap=xml_n
-0000ac10: 616d 6573 7061 6365 5f6d 6170 2c0a 2020  amespace_map,.  
-0000ac20: 2020 290a 2020 2020 6b77 6172 6773 203d    ).    kwargs =
-0000ac30: 207b 2270 6572 6d69 7373 696f 6e73 223a   {"permissions":
-0000ac40: 2076 616c 7565 2e70 6572 6d69 7373 696f   value.permissio
-0000ac50: 6e73 7d0a 2020 2020 6966 2076 616c 7565  ns}.    if value
-0000ac60: 2e63 6f6d 6d65 6e74 2061 6e64 2063 6865  .comment and che
-0000ac70: 636b 5f6e 6f74 6e61 2876 616c 7565 2e63  ck_notna(value.c
-0000ac80: 6f6d 6d65 6e74 293a 0a20 2020 2020 2020  omment):.       
-0000ac90: 206b 7761 7267 735b 2263 6f6d 6d65 6e74   kwargs["comment
-0000aca0: 225d 203d 2076 616c 7565 2e63 6f6d 6d65  "] = value.comme
-0000acb0: 6e74 0a20 2020 2076 616c 7565 5f20 3d20  nt.    value_ = 
-0000acc0: 6574 7265 652e 456c 656d 656e 7428 0a20  etree.Element(. 
-0000acd0: 2020 2020 2020 2022 7b25 737d 696e 7465         "{%s}inte
-0000ace0: 7276 616c 2220 2520 786d 6c5f 6e61 6d65  rval" % xml_name
-0000acf0: 7370 6163 655f 6d61 705b 4e6f 6e65 5d2c  space_map[None],
-0000ad00: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
-0000ad10: 732c 2020 2320 7479 7065 3a20 6967 6e6f  s,  # type: igno
-0000ad20: 7265 5b61 7267 2d74 7970 655d 0a20 2020  re[arg-type].   
-0000ad30: 2020 2020 206e 736d 6170 3d78 6d6c 5f6e       nsmap=xml_n
-0000ad40: 616d 6573 7061 6365 5f6d 6170 2c0a 2020  amespace_map,.  
-0000ad50: 2020 290a 2020 2020 7661 6c75 655f 2e74    ).    value_.t
-0000ad60: 6578 7420 3d20 7374 7228 7661 6c75 652e  ext = str(value.
-0000ad70: 7661 6c75 6529 0a20 2020 2070 726f 705f  value).    prop_
-0000ad80: 2e61 7070 656e 6428 7661 6c75 655f 290a  .append(value_).
-0000ad90: 0a20 2020 2072 6574 7572 6e20 7072 6f70  .    return prop
-0000ada0: 5f0a 0a0a 6465 6620 6d61 6b65 5f6c 6973  _...def make_lis
-0000adb0: 745f 7072 6f70 280a 2020 2020 6c69 7374  t_prop(.    list
-0000adc0: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
-0000add0: 6e61 6d65 3a20 7374 722c 0a20 2020 2076  name: str,.    v
-0000ade0: 616c 7565 3a20 556e 696f 6e5b 5072 6f70  alue: Union[Prop
-0000adf0: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
-0000ae00: 2c20 4974 6572 6162 6c65 5b55 6e69 6f6e  , Iterable[Union
-0000ae10: 5b50 726f 7065 7274 7945 6c65 6d65 6e74  [PropertyElement
-0000ae20: 2c20 7374 725d 5d5d 2c0a 2020 2020 6361  , str]]],.    ca
-0000ae30: 6c6c 696e 675f 7265 736f 7572 6365 3a20  lling_resource: 
-0000ae40: 7374 7220 3d20 2222 2c0a 2920 2d3e 2065  str = "",.) -> e
-0000ae50: 7472 6565 2e5f 456c 656d 656e 743a 0a20  tree._Element:. 
-0000ae60: 2020 2022 2222 0a20 2020 204d 616b 6520     """.    Make 
-0000ae70: 6120 3c6c 6973 742d 7072 6f70 3e20 6672  a <list-prop> fr
-0000ae80: 6f6d 206f 6e65 206f 7220 6d6f 7265 206c  om one or more l
-0000ae90: 6973 7420 6e6f 6465 732e 2054 6865 206e  ist nodes. The n
-0000aea0: 616d 6528 7329 206f 6620 7468 6520 6c69  ame(s) of the li
-0000aeb0: 7374 206e 6f64 6528 7329 2063 616e 2062  st node(s) can b
-0000aec0: 6520 7072 6f76 6964 6564 2061 7320 7374  e provided as st
-0000aed0: 7269 6e67 206f 7220 6173 0a20 2020 2050  ring or as.    P
-0000aee0: 726f 7065 7274 7945 6c65 6d65 6e74 2077  ropertyElement w
-0000aef0: 6974 6820 6120 7374 7269 6e67 2069 6e73  ith a string ins
-0000af00: 6964 652e 2049 6620 7072 6f76 6964 6564  ide. If provided
-0000af10: 2061 7320 7374 7269 6e67 2c20 7468 6520   as string, the 
-0000af20: 7065 726d 6973 7369 6f6e 7320 6465 6661  permissions defa
-0000af30: 756c 7420 746f 2022 7072 6f70 2d64 6566  ult to "prop-def
-0000af40: 6175 6c74 222e 0a0a 2020 2020 4172 6773  ault"...    Args
-0000af50: 3a0a 2020 2020 2020 2020 6c69 7374 5f6e  :.        list_n
-0000af60: 616d 653a 2074 6865 206e 616d 6520 6f66  ame: the name of
-0000af70: 2074 6865 206c 6973 7420 6173 2064 6566   the list as def
-0000af80: 696e 6564 2069 6e20 7468 6520 6f6e 746f  ined in the onto
-0000af90: 0a20 2020 2020 2020 206e 616d 653a 2074  .        name: t
-0000afa0: 6865 206e 616d 6520 6f66 2074 6869 7320  he name of this 
-0000afb0: 7072 6f70 6572 7479 2061 7320 6465 6669  property as defi
-0000afc0: 6e65 6420 696e 2074 6865 206f 6e74 6f0a  ned in the onto.
-0000afd0: 2020 2020 2020 2020 7661 6c75 653a 206f          value: o
-0000afe0: 6e65 206f 7220 6d6f 7265 206e 6f64 6520  ne or more node 
-0000aff0: 6e61 6d65 732c 2061 7320 7374 7269 6e67  names, as string
-0000b000: 2f50 726f 7065 7274 7945 6c65 6d65 6e74  /PropertyElement
-0000b010: 2c20 6f72 2061 7320 6974 6572 6162 6c65  , or as iterable
-0000b020: 206f 6620 7374 7269 6e67 732f 5072 6f70   of strings/Prop
-0000b030: 6572 7479 456c 656d 656e 7473 0a20 2020  ertyElements.   
-0000b040: 2020 2020 2063 616c 6c69 6e67 5f72 6573       calling_res
-0000b050: 6f75 7263 653a 2074 6865 206e 616d 6520  ource: the name 
-0000b060: 6f66 2074 6865 2070 6172 656e 7420 7265  of the parent re
-0000b070: 736f 7572 6365 2028 666f 7220 6265 7474  source (for bett
-0000b080: 6572 2065 7272 6f72 206d 6573 7361 6765  er error message
-0000b090: 7329 0a0a 2020 2020 5761 726e 733a 0a20  s)..    Warns:. 
-0000b0a0: 2020 2020 2020 2049 6620 7468 6520 6e61         If the na
-0000b0b0: 6d65 206f 6620 6f6e 6520 6f66 2074 6865  me of one of the
-0000b0c0: 206c 6973 7420 6e6f 6465 7320 6973 206e   list nodes is n
-0000b0d0: 6f74 2061 2076 616c 6964 2073 7472 696e  ot a valid strin
-0000b0e0: 670a 0a20 2020 2052 6574 7572 6e73 3a0a  g..    Returns:.
-0000b0f0: 2020 2020 2020 2020 616e 2065 7472 6565          an etree
-0000b100: 2e5f 456c 656d 656e 7420 7468 6174 2063  ._Element that c
-0000b110: 616e 2062 6520 6170 7065 6e64 6564 2074  an be appended t
-0000b120: 6f20 7468 6520 7061 7265 6e74 2072 6573  o the parent res
-0000b130: 6f75 7263 6520 7769 7468 2072 6573 6f75  ource with resou
-0000b140: 7263 652e 6170 7065 6e64 286d 616b 655f  rce.append(make_
-0000b150: 2a5f 7072 6f70 282e 2e2e 2929 0a0a 2020  *_prop(...))..  
-0000b160: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
-0000b170: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
-0000b180: 6c2e 6d61 6b65 5f6c 6973 745f 7072 6f70  l.make_list_prop
-0000b190: 2822 6d79 6c69 7374 222c 2022 3a74 6573  ("mylist", ":tes
-0000b1a0: 7470 726f 7065 7274 7922 2c20 2266 6972  tproperty", "fir
-0000b1b0: 7374 5f6e 6f64 6522 290a 2020 2020 2020  st_node").      
-0000b1c0: 2020 2020 2020 2020 2020 3c6c 6973 742d            <list-
-0000b1d0: 7072 6f70 206c 6973 743d 226d 796c 6973  prop list="mylis
-0000b1e0: 7422 206e 616d 653d 223a 7465 7374 7072  t" name=":testpr
-0000b1f0: 6f70 6572 7479 223e 0a20 2020 2020 2020  operty">.       
-0000b200: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
-0000b210: 7374 2070 6572 6d69 7373 696f 6e73 3d22  st permissions="
-0000b220: 7072 6f70 2d64 6566 6175 6c74 223e 6669  prop-default">fi
-0000b230: 7273 745f 6e6f 6465 3c2f 6c69 7374 3e0a  rst_node</list>.
-0000b240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b250: 3c2f 6c69 7374 2d70 726f 703e 0a20 2020  </list-prop>.   
-0000b260: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
-0000b270: 6d6c 2e6d 616b 655f 6c69 7374 5f70 726f  ml.make_list_pro
-0000b280: 7028 226d 796c 6973 7422 2c20 223a 7465  p("mylist", ":te
-0000b290: 7374 7072 6f70 6572 7479 222c 2065 7863  stproperty", exc
-0000b2a0: 656c 3278 6d6c 2e50 726f 7065 7274 7945  el2xml.PropertyE
-0000b2b0: 6c65 6d65 6e74 2822 6669 7273 745f 6e6f  lement("first_no
-0000b2c0: 6465 222c 2070 6572 6d69 7373 696f 6e73  de", permissions
-0000b2d0: 3d22 7072 6f70 2d72 6573 7472 6963 7465  ="prop-restricte
-0000b2e0: 6422 2c20 636f 6d6d 656e 743d 2265 7861  d", comment="exa
-0000b2f0: 6d70 6c65 2229 290a 2020 2020 2020 2020  mple")).        
-0000b300: 2020 2020 2020 2020 3c6c 6973 742d 7072          <list-pr
-0000b310: 6f70 206c 6973 743d 226d 796c 6973 7422  op list="mylist"
-0000b320: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
-0000b330: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
-0000b340: 2020 2020 2020 2020 2020 203c 6c69 7374             <list
-0000b350: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
-0000b360: 6f70 2d72 6573 7472 6963 7465 6422 2063  op-restricted" c
-0000b370: 6f6d 6d65 6e74 3d22 6578 616d 706c 6522  omment="example"
-0000b380: 3e66 6972 7374 5f6e 6f64 653c 2f6c 6973  >first_node</lis
-0000b390: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-0000b3a0: 2020 203c 2f6c 6973 742d 7072 6f70 3e0a     </list-prop>.
-0000b3b0: 2020 2020 2020 2020 3e3e 3e20 6578 6365          >>> exce
-0000b3c0: 6c32 786d 6c2e 6d61 6b65 5f6c 6973 745f  l2xml.make_list_
-0000b3d0: 7072 6f70 2822 6d79 6c69 7374 222c 2022  prop("mylist", "
-0000b3e0: 3a74 6573 7470 726f 7065 7274 7922 2c20  :testproperty", 
-0000b3f0: 5b22 6669 7273 745f 6e6f 6465 222c 2022  ["first_node", "
-0000b400: 7365 636f 6e64 5f6e 6f64 6522 5d29 0a20  second_node"]). 
-0000b410: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000b420: 6c69 7374 2d70 726f 7020 6c69 7374 3d22  list-prop list="
-0000b430: 6d79 6c69 7374 2220 6e61 6d65 3d22 3a74  mylist" name=":t
-0000b440: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
+0000aa10: 2e6d 6174 6368 2872 225c 642b 285c 2e5c  .match(r"\d+(\.\
+0000aa20: 642b 293f 3a5c 642b 285c 2e5c 642b 293f  d+)?:\d+(\.\d+)?
+0000aa30: 222c 2073 7472 2876 616c 7565 2e76 616c  ", str(value.val
+0000aa40: 7565 2929 3a0a 2020 2020 2020 2020 6d73  ue)):.        ms
+0000aa50: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
+0000aa60: 2020 6622 4661 696c 6564 2076 616c 6964    f"Failed valid
+0000aa70: 6174 696f 6e20 696e 2072 6573 6f75 7263  ation in resourc
+0000aa80: 6520 277b 6361 6c6c 696e 675f 7265 736f  e '{calling_reso
+0000aa90: 7572 6365 7d27 2c20 7072 6f70 6572 7479  urce}', property
+0000aaa0: 2027 7b6e 616d 657d 273a 2022 0a20 2020   '{name}': ".   
+0000aab0: 2020 2020 2020 2020 2066 2227 7b76 616c           f"'{val
+0000aac0: 7565 2e76 616c 7565 7d27 2069 7320 6e6f  ue.value}' is no
+0000aad0: 7420 6120 7661 6c69 6420 4453 5020 696e  t a valid DSP in
+0000aae0: 7465 7276 616c 2e22 0a20 2020 2020 2020  terval.".       
+0000aaf0: 2029 0a20 2020 2020 2020 2077 6172 6e69   ).        warni
+0000ab00: 6e67 732e 7761 726e 2844 7370 546f 6f6c  ngs.warn(DspTool
+0000ab10: 7355 7365 7257 6172 6e69 6e67 286d 7367  sUserWarning(msg
+0000ab20: 2929 0a0a 2020 2020 2320 6d61 6b65 2078  ))..    # make x
+0000ab30: 6d6c 2073 7472 7563 7475 7265 206f 6620  ml structure of 
+0000ab40: 7468 6520 7661 6c69 6420 7661 6c75 6573  the valid values
+0000ab50: 0a20 2020 2070 726f 705f 203d 2065 7472  .    prop_ = etr
+0000ab60: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
+0000ab70: 2020 2020 227b 2573 7d69 6e74 6572 7661      "{%s}interva
+0000ab80: 6c2d 7072 6f70 2220 2520 786d 6c5f 6e61  l-prop" % xml_na
+0000ab90: 6d65 7370 6163 655f 6d61 705b 4e6f 6e65  mespace_map[None
+0000aba0: 5d2c 0a20 2020 2020 2020 206e 616d 653d  ],.        name=
+0000abb0: 6e61 6d65 2c0a 2020 2020 2020 2020 6e73  name,.        ns
+0000abc0: 6d61 703d 786d 6c5f 6e61 6d65 7370 6163  map=xml_namespac
+0000abd0: 655f 6d61 702c 0a20 2020 2029 0a20 2020  e_map,.    ).   
+0000abe0: 206b 7761 7267 7320 3d20 7b22 7065 726d   kwargs = {"perm
+0000abf0: 6973 7369 6f6e 7322 3a20 7661 6c75 652e  issions": value.
+0000ac00: 7065 726d 6973 7369 6f6e 737d 0a20 2020  permissions}.   
+0000ac10: 2069 6620 7661 6c75 652e 636f 6d6d 656e   if value.commen
+0000ac20: 7420 616e 6420 6368 6563 6b5f 6e6f 746e  t and check_notn
+0000ac30: 6128 7661 6c75 652e 636f 6d6d 656e 7429  a(value.comment)
+0000ac40: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
+0000ac50: 5b22 636f 6d6d 656e 7422 5d20 3d20 7661  ["comment"] = va
+0000ac60: 6c75 652e 636f 6d6d 656e 740a 2020 2020  lue.comment.    
+0000ac70: 7661 6c75 655f 203d 2065 7472 6565 2e45  value_ = etree.E
+0000ac80: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
+0000ac90: 227b 2573 7d69 6e74 6572 7661 6c22 2025  "{%s}interval" %
+0000aca0: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
+0000acb0: 6170 5b4e 6f6e 655d 2c0a 2020 2020 2020  ap[None],.      
+0000acc0: 2020 2a2a 6b77 6172 6773 2c20 2023 2074    **kwargs,  # t
+0000acd0: 7970 653a 2069 676e 6f72 655b 6172 672d  ype: ignore[arg-
+0000ace0: 7479 7065 5d0a 2020 2020 2020 2020 6e73  type].        ns
+0000acf0: 6d61 703d 786d 6c5f 6e61 6d65 7370 6163  map=xml_namespac
+0000ad00: 655f 6d61 702c 0a20 2020 2029 0a20 2020  e_map,.    ).   
+0000ad10: 2076 616c 7565 5f2e 7465 7874 203d 2073   value_.text = s
+0000ad20: 7472 2876 616c 7565 2e76 616c 7565 290a  tr(value.value).
+0000ad30: 2020 2020 7072 6f70 5f2e 6170 7065 6e64      prop_.append
+0000ad40: 2876 616c 7565 5f29 0a0a 2020 2020 7265  (value_)..    re
+0000ad50: 7475 726e 2070 726f 705f 0a0a 0a64 6566  turn prop_...def
+0000ad60: 206d 616b 655f 6c69 7374 5f70 726f 7028   make_list_prop(
+0000ad70: 0a20 2020 206c 6973 745f 6e61 6d65 3a20  .    list_name: 
+0000ad80: 7374 722c 0a20 2020 206e 616d 653a 2073  str,.    name: s
+0000ad90: 7472 2c0a 2020 2020 7661 6c75 653a 2055  tr,.    value: U
+0000ada0: 6e69 6f6e 5b50 726f 7065 7274 7945 6c65  nion[PropertyEle
+0000adb0: 6d65 6e74 2c20 7374 722c 2049 7465 7261  ment, str, Itera
+0000adc0: 626c 655b 556e 696f 6e5b 5072 6f70 6572  ble[Union[Proper
+0000add0: 7479 456c 656d 656e 742c 2073 7472 5d5d  tyElement, str]]
+0000ade0: 5d2c 0a20 2020 2063 616c 6c69 6e67 5f72  ],.    calling_r
+0000adf0: 6573 6f75 7263 653a 2073 7472 203d 2022  esource: str = "
+0000ae00: 222c 0a29 202d 3e20 6574 7265 652e 5f45  ",.) -> etree._E
+0000ae10: 6c65 6d65 6e74 3a0a 2020 2020 2222 220a  lement:.    """.
+0000ae20: 2020 2020 4d61 6b65 2061 203c 6c69 7374      Make a <list
+0000ae30: 2d70 726f 703e 2066 726f 6d20 6f6e 6520  -prop> from one 
+0000ae40: 6f72 206d 6f72 6520 6c69 7374 206e 6f64  or more list nod
+0000ae50: 6573 2e20 5468 6520 6e61 6d65 2873 2920  es. The name(s) 
+0000ae60: 6f66 2074 6865 206c 6973 7420 6e6f 6465  of the list node
+0000ae70: 2873 2920 6361 6e20 6265 2070 726f 7669  (s) can be provi
+0000ae80: 6465 6420 6173 2073 7472 696e 6720 6f72  ded as string or
+0000ae90: 2061 730a 2020 2020 5072 6f70 6572 7479   as.    Property
+0000aea0: 456c 656d 656e 7420 7769 7468 2061 2073  Element with a s
+0000aeb0: 7472 696e 6720 696e 7369 6465 2e20 4966  tring inside. If
+0000aec0: 2070 726f 7669 6465 6420 6173 2073 7472   provided as str
+0000aed0: 696e 672c 2074 6865 2070 6572 6d69 7373  ing, the permiss
+0000aee0: 696f 6e73 2064 6566 6175 6c74 2074 6f20  ions default to 
+0000aef0: 2270 726f 702d 6465 6661 756c 7422 2e0a  "prop-default"..
+0000af00: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000af10: 2020 206c 6973 745f 6e61 6d65 3a20 7468     list_name: th
+0000af20: 6520 6e61 6d65 206f 6620 7468 6520 6c69  e name of the li
+0000af30: 7374 2061 7320 6465 6669 6e65 6420 696e  st as defined in
+0000af40: 2074 6865 206f 6e74 6f0a 2020 2020 2020   the onto.      
+0000af50: 2020 6e61 6d65 3a20 7468 6520 6e61 6d65    name: the name
+0000af60: 206f 6620 7468 6973 2070 726f 7065 7274   of this propert
+0000af70: 7920 6173 2064 6566 696e 6564 2069 6e20  y as defined in 
+0000af80: 7468 6520 6f6e 746f 0a20 2020 2020 2020  the onto.       
+0000af90: 2076 616c 7565 3a20 6f6e 6520 6f72 206d   value: one or m
+0000afa0: 6f72 6520 6e6f 6465 206e 616d 6573 2c20  ore node names, 
+0000afb0: 6173 2073 7472 696e 672f 5072 6f70 6572  as string/Proper
+0000afc0: 7479 456c 656d 656e 742c 206f 7220 6173  tyElement, or as
+0000afd0: 2069 7465 7261 626c 6520 6f66 2073 7472   iterable of str
+0000afe0: 696e 6773 2f50 726f 7065 7274 7945 6c65  ings/PropertyEle
+0000aff0: 6d65 6e74 730a 2020 2020 2020 2020 6361  ments.        ca
+0000b000: 6c6c 696e 675f 7265 736f 7572 6365 3a20  lling_resource: 
+0000b010: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
+0000b020: 7061 7265 6e74 2072 6573 6f75 7263 6520  parent resource 
+0000b030: 2866 6f72 2062 6574 7465 7220 6572 726f  (for better erro
+0000b040: 7220 6d65 7373 6167 6573 290a 0a20 2020  r messages)..   
+0000b050: 2057 6172 6e73 3a0a 2020 2020 2020 2020   Warns:.        
+0000b060: 4966 2074 6865 206e 616d 6520 6f66 206f  If the name of o
+0000b070: 6e65 206f 6620 7468 6520 6c69 7374 206e  ne of the list n
+0000b080: 6f64 6573 2069 7320 6e6f 7420 6120 7661  odes is not a va
+0000b090: 6c69 6420 7374 7269 6e67 0a0a 2020 2020  lid string..    
+0000b0a0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0000b0b0: 2061 6e20 6574 7265 652e 5f45 6c65 6d65   an etree._Eleme
+0000b0c0: 6e74 2074 6861 7420 6361 6e20 6265 2061  nt that can be a
+0000b0d0: 7070 656e 6465 6420 746f 2074 6865 2070  ppended to the p
+0000b0e0: 6172 656e 7420 7265 736f 7572 6365 2077  arent resource w
+0000b0f0: 6974 6820 7265 736f 7572 6365 2e61 7070  ith resource.app
+0000b100: 656e 6428 6d61 6b65 5f2a 5f70 726f 7028  end(make_*_prop(
+0000b110: 2e2e 2e29 290a 0a20 2020 2045 7861 6d70  ...))..    Examp
+0000b120: 6c65 733a 0a20 2020 2020 2020 203e 3e3e  les:.        >>>
+0000b130: 2065 7863 656c 3278 6d6c 2e6d 616b 655f   excel2xml.make_
+0000b140: 6c69 7374 5f70 726f 7028 226d 796c 6973  list_prop("mylis
+0000b150: 7422 2c20 223a 7465 7374 7072 6f70 6572  t", ":testproper
+0000b160: 7479 222c 2022 6669 7273 745f 6e6f 6465  ty", "first_node
+0000b170: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0000b180: 2020 203c 6c69 7374 2d70 726f 7020 6c69     <list-prop li
+0000b190: 7374 3d22 6d79 6c69 7374 2220 6e61 6d65  st="mylist" name
+0000b1a0: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
+0000b1b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000b1c0: 2020 2020 2020 3c6c 6973 7420 7065 726d        <list perm
+0000b1d0: 6973 7369 6f6e 733d 2270 726f 702d 6465  issions="prop-de
+0000b1e0: 6661 756c 7422 3e66 6972 7374 5f6e 6f64  fault">first_nod
+0000b1f0: 653c 2f6c 6973 743e 0a20 2020 2020 2020  e</list>.       
+0000b200: 2020 2020 2020 2020 203c 2f6c 6973 742d           </list-
+0000b210: 7072 6f70 3e0a 2020 2020 2020 2020 3e3e  prop>.        >>
+0000b220: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
+0000b230: 5f6c 6973 745f 7072 6f70 2822 6d79 6c69  _list_prop("myli
+0000b240: 7374 222c 2022 3a74 6573 7470 726f 7065  st", ":testprope
+0000b250: 7274 7922 2c20 6578 6365 6c32 786d 6c2e  rty", excel2xml.
+0000b260: 5072 6f70 6572 7479 456c 656d 656e 7428  PropertyElement(
+0000b270: 2266 6972 7374 5f6e 6f64 6522 2c20 7065  "first_node", pe
+0000b280: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
+0000b290: 7265 7374 7269 6374 6564 222c 2063 6f6d  restricted", com
+0000b2a0: 6d65 6e74 3d22 6578 616d 706c 6522 2929  ment="example"))
+0000b2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b2c0: 203c 6c69 7374 2d70 726f 7020 6c69 7374   <list-prop list
+0000b2d0: 3d22 6d79 6c69 7374 2220 6e61 6d65 3d22  ="mylist" name="
+0000b2e0: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
+0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b300: 2020 2020 3c6c 6973 7420 7065 726d 6973      <list permis
+0000b310: 7369 6f6e 733d 2270 726f 702d 7265 7374  sions="prop-rest
+0000b320: 7269 6374 6564 2220 636f 6d6d 656e 743d  ricted" comment=
+0000b330: 2265 7861 6d70 6c65 223e 6669 7273 745f  "example">first_
+0000b340: 6e6f 6465 3c2f 6c69 7374 3e0a 2020 2020  node</list>.    
+0000b350: 2020 2020 2020 2020 2020 2020 3c2f 6c69              </li
+0000b360: 7374 2d70 726f 703e 0a20 2020 2020 2020  st-prop>.       
+0000b370: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
+0000b380: 616b 655f 6c69 7374 5f70 726f 7028 226d  ake_list_prop("m
+0000b390: 796c 6973 7422 2c20 223a 7465 7374 7072  ylist", ":testpr
+0000b3a0: 6f70 6572 7479 222c 205b 2266 6972 7374  operty", ["first
+0000b3b0: 5f6e 6f64 6522 2c20 2273 6563 6f6e 645f  _node", "second_
+0000b3c0: 6e6f 6465 225d 290a 2020 2020 2020 2020  node"]).        
+0000b3d0: 2020 2020 2020 2020 3c6c 6973 742d 7072          <list-pr
+0000b3e0: 6f70 206c 6973 743d 226d 796c 6973 7422  op list="mylist"
+0000b3f0: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
+0000b400: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
+0000b410: 2020 2020 2020 2020 2020 203c 6c69 7374             <list
+0000b420: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
+0000b430: 6f70 2d64 6566 6175 6c74 223e 6669 7273  op-default">firs
+0000b440: 745f 6e6f 6465 3c2f 6c69 7374 3e0a 2020  t_node</list>.  
 0000b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b460: 2020 3c6c 6973 7420 7065 726d 6973 7369    <list permissi
 0000b470: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-0000b480: 7422 3e66 6972 7374 5f6e 6f64 653c 2f6c  t">first_node</l
-0000b490: 6973 743e 0a20 2020 2020 2020 2020 2020  ist>.           
-0000b4a0: 2020 2020 2020 2020 203c 6c69 7374 2070           <list p
-0000b4b0: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
-0000b4c0: 2d64 6566 6175 6c74 223e 7365 636f 6e64  -default">second
-0000b4d0: 5f6e 6f64 653c 2f6c 6973 743e 0a20 2020  _node</list>.   
-0000b4e0: 2020 2020 2020 2020 2020 2020 203c 2f6c               </l
-0000b4f0: 6973 742d 7072 6f70 3e0a 0a20 2020 2053  ist-prop>..    S
-0000b500: 6565 2068 7474 7073 3a2f 2f64 6f63 732e  ee https://docs.
-0000b510: 6461 7363 682e 7377 6973 732f 6c61 7465  dasch.swiss/late
-0000b520: 7374 2f44 5350 2d54 4f4f 4c53 2f66 696c  st/DSP-TOOLS/fil
-0000b530: 652d 666f 726d 6174 732f 786d 6c2d 6461  e-formats/xml-da
-0000b540: 7461 2d66 696c 652f 236c 6973 742d 7072  ta-file/#list-pr
-0000b550: 6f70 0a20 2020 2022 2222 0a0a 2020 2020  op.    """..    
-0000b560: 2320 6368 6563 6b20 7468 6520 696e 7075  # check the inpu
-0000b570: 743a 2070 7265 7061 7265 2061 206c 6973  t: prepare a lis
-0000b580: 7420 7769 7468 2076 616c 6964 2076 616c  t with valid val
-0000b590: 7565 730a 2020 2020 7661 6c75 6573 203d  ues.    values =
-0000b5a0: 2070 7265 7061 7265 5f76 616c 7565 2876   prepare_value(v
-0000b5b0: 616c 7565 290a 0a20 2020 2023 2063 6865  alue)..    # che
-0000b5c0: 636b 2076 616c 7565 2074 7970 650a 2020  ck value type.  
-0000b5d0: 2020 666f 7220 7661 6c20 696e 2076 616c    for val in val
-0000b5e0: 7565 733a 0a20 2020 2020 2020 2069 6620  ues:.        if 
-0000b5f0: 6e6f 7420 6973 696e 7374 616e 6365 2876  not isinstance(v
-0000b600: 616c 2e76 616c 7565 2c20 7374 7229 206f  al.value, str) o
-0000b610: 7220 6e6f 7420 6368 6563 6b5f 6e6f 746e  r not check_notn
-0000b620: 6128 7661 6c2e 7661 6c75 6529 3a0a 2020  a(val.value):.  
-0000b630: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
-0000b640: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000b650: 2020 6622 4661 696c 6564 2076 616c 6964    f"Failed valid
-0000b660: 6174 696f 6e20 696e 2072 6573 6f75 7263  ation in resourc
-0000b670: 6520 277b 6361 6c6c 696e 675f 7265 736f  e '{calling_reso
-0000b680: 7572 6365 7d27 2c20 7072 6f70 6572 7479  urce}', property
-0000b690: 2027 7b6e 616d 657d 273a 2022 0a20 2020   '{name}': ".   
-0000b6a0: 2020 2020 2020 2020 2020 2020 2066 2227               f"'
-0000b6b0: 7b76 616c 2e76 616c 7565 7d27 2069 7320  {val.value}' is 
-0000b6c0: 6e6f 7420 6120 7661 6c69 6420 6e61 6d65  not a valid name
-0000b6d0: 206f 6620 6120 6c69 7374 206e 6f64 652e   of a list node.
-0000b6e0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-0000b6f0: 2020 2020 2020 2020 2020 2020 7761 726e              warn
-0000b700: 696e 6773 2e77 6172 6e28 4473 7054 6f6f  ings.warn(DspToo
-0000b710: 6c73 5573 6572 5761 726e 696e 6728 6d73  lsUserWarning(ms
-0000b720: 6729 290a 0a20 2020 2023 206d 616b 6520  g))..    # make 
-0000b730: 786d 6c20 7374 7275 6374 7572 6520 6f66  xml structure of
-0000b740: 2074 6865 2076 616c 6964 2076 616c 7565   the valid value
-0000b750: 730a 2020 2020 7072 6f70 5f20 3d20 6574  s.    prop_ = et
-0000b760: 7265 652e 456c 656d 656e 7428 0a20 2020  ree.Element(.   
-0000b770: 2020 2020 2022 7b25 737d 6c69 7374 2d70       "{%s}list-p
-0000b780: 726f 7022 2025 2078 6d6c 5f6e 616d 6573  rop" % xml_names
-0000b790: 7061 6365 5f6d 6170 5b4e 6f6e 655d 2c0a  pace_map[None],.
-0000b7a0: 2020 2020 2020 2020 6c69 7374 3d6c 6973          list=lis
-0000b7b0: 745f 6e61 6d65 2c0a 2020 2020 2020 2020  t_name,.        
-0000b7c0: 6e61 6d65 3d6e 616d 652c 0a20 2020 2020  name=name,.     
-0000b7d0: 2020 206e 736d 6170 3d78 6d6c 5f6e 616d     nsmap=xml_nam
-0000b7e0: 6573 7061 6365 5f6d 6170 2c0a 2020 2020  espace_map,.    
-0000b7f0: 290a 2020 2020 666f 7220 7661 6c20 696e  ).    for val in
-0000b800: 2076 616c 7565 733a 0a20 2020 2020 2020   values:.       
-0000b810: 206b 7761 7267 7320 3d20 7b22 7065 726d   kwargs = {"perm
-0000b820: 6973 7369 6f6e 7322 3a20 7661 6c2e 7065  issions": val.pe
-0000b830: 726d 6973 7369 6f6e 737d 0a20 2020 2020  rmissions}.     
-0000b840: 2020 2069 6620 7661 6c2e 636f 6d6d 656e     if val.commen
-0000b850: 7420 616e 6420 6368 6563 6b5f 6e6f 746e  t and check_notn
-0000b860: 6128 7661 6c2e 636f 6d6d 656e 7429 3a0a  a(val.comment):.
-0000b870: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-0000b880: 6773 5b22 636f 6d6d 656e 7422 5d20 3d20  gs["comment"] = 
-0000b890: 7661 6c2e 636f 6d6d 656e 740a 2020 2020  val.comment.    
-0000b8a0: 2020 2020 7661 6c75 655f 203d 2065 7472      value_ = etr
-0000b8b0: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
-0000b8c0: 2020 2020 2020 2020 227b 2573 7d6c 6973          "{%s}lis
-0000b8d0: 7422 2025 2078 6d6c 5f6e 616d 6573 7061  t" % xml_namespa
-0000b8e0: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
-0000b8f0: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000b900: 6773 2c20 2023 2074 7970 653a 2069 676e  gs,  # type: ign
-0000b910: 6f72 655b 6172 672d 7479 7065 5d0a 2020  ore[arg-type].  
-0000b920: 2020 2020 2020 2020 2020 6e73 6d61 703d            nsmap=
-0000b930: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
-0000b940: 702c 0a20 2020 2020 2020 2029 0a20 2020  p,.        ).   
-0000b950: 2020 2020 2076 616c 7565 5f2e 7465 7874       value_.text
-0000b960: 203d 2073 7472 2876 616c 2e76 616c 7565   = str(val.value
-0000b970: 290a 2020 2020 2020 2020 7072 6f70 5f2e  ).        prop_.
-0000b980: 6170 7065 6e64 2876 616c 7565 5f29 0a0a  append(value_)..
-0000b990: 2020 2020 7265 7475 726e 2070 726f 705f      return prop_
-0000b9a0: 0a0a 0a64 6566 206d 616b 655f 7265 7370  ...def make_resp
-0000b9b0: 7472 5f70 726f 7028 0a20 2020 206e 616d  tr_prop(.    nam
-0000b9c0: 653a 2073 7472 2c0a 2020 2020 7661 6c75  e: str,.    valu
-0000b9d0: 653a 2055 6e69 6f6e 5b50 726f 7065 7274  e: Union[Propert
-0000b9e0: 7945 6c65 6d65 6e74 2c20 7374 722c 2049  yElement, str, I
-0000b9f0: 7465 7261 626c 655b 556e 696f 6e5b 5072  terable[Union[Pr
-0000ba00: 6f70 6572 7479 456c 656d 656e 742c 2073  opertyElement, s
-0000ba10: 7472 5d5d 5d2c 0a20 2020 2063 616c 6c69  tr]]],.    calli
-0000ba20: 6e67 5f72 6573 6f75 7263 653a 2073 7472  ng_resource: str
-0000ba30: 203d 2022 222c 0a29 202d 3e20 6574 7265   = "",.) -> etre
-0000ba40: 652e 5f45 6c65 6d65 6e74 3a0a 2020 2020  e._Element:.    
-0000ba50: 2222 220a 2020 2020 4d61 6b65 2061 203c  """.    Make a <
-0000ba60: 7265 7370 7472 2d70 726f 703e 2066 726f  resptr-prop> fro
-0000ba70: 6d20 6f6e 6520 6f72 206d 6f72 6520 4944  m one or more ID
-0000ba80: 7320 6f66 206f 7468 6572 2072 6573 6f75  s of other resou
-0000ba90: 7263 6573 2e20 5468 6520 4944 2873 2920  rces. The ID(s) 
-0000baa0: 6361 6e20 6265 2070 726f 7669 6465 6420  can be provided 
-0000bab0: 6173 2073 7472 696e 6720 6f72 2061 730a  as string or as.
-0000bac0: 2020 2020 5072 6f70 6572 7479 456c 656d      PropertyElem
-0000bad0: 656e 7420 7769 7468 2061 2073 7472 696e  ent with a strin
-0000bae0: 6720 696e 7369 6465 2e20 4966 2070 726f  g inside. If pro
-0000baf0: 7669 6465 6420 6173 2073 7472 696e 672c  vided as string,
-0000bb00: 2074 6865 2070 6572 6d69 7373 696f 6e73   the permissions
-0000bb10: 2064 6566 6175 6c74 2074 6f20 2270 726f   default to "pro
-0000bb20: 702d 6465 6661 756c 7422 2e0a 0a20 2020  p-default"...   
-0000bb30: 2041 7267 733a 0a20 2020 2020 2020 206e   Args:.        n
-0000bb40: 616d 653a 2074 6865 206e 616d 6520 6f66  ame: the name of
-0000bb50: 2074 6869 7320 7072 6f70 6572 7479 2061   this property a
-0000bb60: 7320 6465 6669 6e65 6420 696e 2074 6865  s defined in the
-0000bb70: 206f 6e74 6f0a 2020 2020 2020 2020 7661   onto.        va
-0000bb80: 6c75 653a 206f 6e65 206f 7220 6d6f 7265  lue: one or more
-0000bb90: 2072 6573 6f75 7263 6520 6964 656e 7469   resource identi
-0000bba0: 6669 6572 732c 2061 7320 7374 7269 6e67  fiers, as string
-0000bbb0: 2f50 726f 7065 7274 7945 6c65 6d65 6e74  /PropertyElement
-0000bbc0: 2c20 6f72 2061 7320 6974 6572 6162 6c65  , or as iterable
-0000bbd0: 206f 6620 7374 7269 6e67 732f 5072 6f70   of strings/Prop
-0000bbe0: 6572 7479 456c 656d 656e 7473 0a20 2020  ertyElements.   
-0000bbf0: 2020 2020 2063 616c 6c69 6e67 5f72 6573       calling_res
-0000bc00: 6f75 7263 653a 2074 6865 206e 616d 6520  ource: the name 
-0000bc10: 6f66 2074 6865 2070 6172 656e 7420 7265  of the parent re
-0000bc20: 736f 7572 6365 2028 666f 7220 6265 7474  source (for bett
-0000bc30: 6572 2065 7272 6f72 206d 6573 7361 6765  er error message
-0000bc40: 7329 0a0a 2020 2020 5761 726e 733a 0a20  s)..    Warns:. 
-0000bc50: 2020 2020 2020 2049 6620 7468 6520 4944         If the ID
-0000bc60: 206f 6620 6f6e 6520 6f66 2074 6865 2074   of one of the t
-0000bc70: 6172 6765 7420 7265 736f 7572 6365 7320  arget resources 
-0000bc80: 6973 206e 6f74 2061 2076 616c 6964 2073  is not a valid s
-0000bc90: 7472 696e 670a 0a20 2020 2052 6574 7572  tring..    Retur
-0000bca0: 6e73 3a0a 2020 2020 2020 2020 616e 2065  ns:.        an e
-0000bcb0: 7472 6565 2e5f 456c 656d 656e 7420 7468  tree._Element th
-0000bcc0: 6174 2063 616e 2062 6520 6170 7065 6e64  at can be append
-0000bcd0: 6564 2074 6f20 7468 6520 7061 7265 6e74  ed to the parent
-0000bce0: 2072 6573 6f75 7263 6520 7769 7468 2072   resource with r
-0000bcf0: 6573 6f75 7263 652e 6170 7065 6e64 286d  esource.append(m
-0000bd00: 616b 655f 2a5f 7072 6f70 282e 2e2e 2929  ake_*_prop(...))
-0000bd10: 0a0a 2020 2020 4578 616d 706c 6573 3a0a  ..    Examples:.
-0000bd20: 2020 2020 2020 2020 3e3e 3e20 6578 6365          >>> exce
-0000bd30: 6c32 786d 6c2e 6d61 6b65 5f72 6573 7074  l2xml.make_respt
-0000bd40: 725f 7072 6f70 2822 3a74 6573 7470 726f  r_prop(":testpro
-0000bd50: 7065 7274 7922 2c20 2272 6573 6f75 7263  perty", "resourc
-0000bd60: 655f 3122 290a 2020 2020 2020 2020 2020  e_1").          
-0000bd70: 2020 2020 2020 3c72 6573 7074 722d 7072        <resptr-pr
-0000bd80: 6f70 206e 616d 653d 223a 7465 7374 7072  op name=":testpr
-0000bd90: 6f70 6572 7479 223e 0a20 2020 2020 2020  operty">.       
-0000bda0: 2020 2020 2020 2020 2020 2020 203c 7265               <re
-0000bdb0: 7370 7472 2070 6572 6d69 7373 696f 6e73  sptr permissions
-0000bdc0: 3d22 7072 6f70 2d64 6566 6175 6c74 223e  ="prop-default">
-0000bdd0: 7265 736f 7572 6365 5f31 3c2f 7265 7370  resource_1</resp
-0000bde0: 7472 3e0a 2020 2020 2020 2020 2020 2020  tr>.            
-0000bdf0: 2020 2020 3c2f 7265 7370 7472 2d70 726f      </resptr-pro
-0000be00: 703e 0a20 2020 2020 2020 203e 3e3e 2065  p>.        >>> e
-0000be10: 7863 656c 3278 6d6c 2e6d 616b 655f 7265  xcel2xml.make_re
-0000be20: 7370 7472 5f70 726f 7028 223a 7465 7374  sptr_prop(":test
-0000be30: 7072 6f70 6572 7479 222c 2065 7863 656c  property", excel
-0000be40: 3278 6d6c 2e50 726f 7065 7274 7945 6c65  2xml.PropertyEle
-0000be50: 6d65 6e74 2822 7265 736f 7572 6365 5f31  ment("resource_1
-0000be60: 222c 2070 6572 6d69 7373 696f 6e73 3d22  ", permissions="
-0000be70: 7072 6f70 2d72 6573 7472 6963 7465 6422  prop-restricted"
-0000be80: 2c20 636f 6d6d 656e 743d 2265 7861 6d70  , comment="examp
-0000be90: 6c65 2229 290a 2020 2020 2020 2020 2020  le")).          
-0000bea0: 2020 2020 2020 3c72 6573 7074 722d 7072        <resptr-pr
-0000beb0: 6f70 206e 616d 653d 223a 7465 7374 7072  op name=":testpr
-0000bec0: 6f70 6572 7479 223e 0a20 2020 2020 2020  operty">.       
-0000bed0: 2020 2020 2020 2020 2020 2020 203c 7265               <re
-0000bee0: 7370 7472 2070 6572 6d69 7373 696f 6e73  sptr permissions
-0000bef0: 3d22 7072 6f70 2d72 6573 7472 6963 7465  ="prop-restricte
-0000bf00: 6422 2063 6f6d 6d65 6e74 3d22 6578 616d  d" comment="exam
-0000bf10: 706c 6522 3e72 6573 6f75 7263 655f 313c  ple">resource_1<
-0000bf20: 2f72 6573 7074 723e 0a20 2020 2020 2020  /resptr>.       
-0000bf30: 2020 2020 2020 2020 203c 2f72 6573 7074           </respt
-0000bf40: 722d 7072 6f70 3e0a 2020 2020 2020 2020  r-prop>.        
-0000bf50: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
-0000bf60: 6b65 5f72 6573 7074 725f 7072 6f70 2822  ke_resptr_prop("
-0000bf70: 3a74 6573 7470 726f 7065 7274 7922 2c20  :testproperty", 
-0000bf80: 5b22 7265 736f 7572 6365 5f31 222c 2022  ["resource_1", "
-0000bf90: 7265 736f 7572 6365 5f32 225d 290a 2020  resource_2"]).  
-0000bfa0: 2020 2020 2020 2020 2020 2020 2020 3c72                <r
-0000bfb0: 6573 7074 722d 7072 6f70 206e 616d 653d  esptr-prop name=
-0000bfc0: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
-0000bfd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bfe0: 2020 2020 203c 7265 7370 7472 2070 6572       <resptr per
-0000bff0: 6d69 7373 696f 6e73 3d22 7072 6f70 2d64  missions="prop-d
-0000c000: 6566 6175 6c74 223e 7265 736f 7572 6365  efault">resource
-0000c010: 5f31 3c2f 7265 7370 7472 3e0a 2020 2020  _1</resptr>.    
+0000b480: 7422 3e73 6563 6f6e 645f 6e6f 6465 3c2f  t">second_node</
+0000b490: 6c69 7374 3e0a 2020 2020 2020 2020 2020  list>.          
+0000b4a0: 2020 2020 2020 3c2f 6c69 7374 2d70 726f        </list-pro
+0000b4b0: 703e 0a0a 2020 2020 5365 6520 6874 7470  p>..    See http
+0000b4c0: 733a 2f2f 646f 6373 2e64 6173 6368 2e73  s://docs.dasch.s
+0000b4d0: 7769 7373 2f6c 6174 6573 742f 4453 502d  wiss/latest/DSP-
+0000b4e0: 544f 4f4c 532f 6669 6c65 2d66 6f72 6d61  TOOLS/file-forma
+0000b4f0: 7473 2f78 6d6c 2d64 6174 612d 6669 6c65  ts/xml-data-file
+0000b500: 2f23 6c69 7374 2d70 726f 700a 2020 2020  /#list-prop.    
+0000b510: 2222 220a 0a20 2020 2023 2063 6865 636b  """..    # check
+0000b520: 2074 6865 2069 6e70 7574 3a20 7072 6570   the input: prep
+0000b530: 6172 6520 6120 6c69 7374 2077 6974 6820  are a list with 
+0000b540: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
+0000b550: 2076 616c 7565 7320 3d20 7072 6570 6172   values = prepar
+0000b560: 655f 7661 6c75 6528 7661 6c75 6529 0a0a  e_value(value)..
+0000b570: 2020 2020 2320 6368 6563 6b20 7661 6c75      # check valu
+0000b580: 6520 7479 7065 0a20 2020 2066 6f72 2076  e type.    for v
+0000b590: 616c 2069 6e20 7661 6c75 6573 3a0a 2020  al in values:.  
+0000b5a0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+0000b5b0: 6e73 7461 6e63 6528 7661 6c2e 7661 6c75  nstance(val.valu
+0000b5c0: 652c 2073 7472 2920 6f72 206e 6f74 2063  e, str) or not c
+0000b5d0: 6865 636b 5f6e 6f74 6e61 2876 616c 2e76  heck_notna(val.v
+0000b5e0: 616c 7565 293a 0a20 2020 2020 2020 2020  alue):.         
+0000b5f0: 2020 206d 7367 203d 2028 0a20 2020 2020     msg = (.     
+0000b600: 2020 2020 2020 2020 2020 2066 2246 6169             f"Fai
+0000b610: 6c65 6420 7661 6c69 6461 7469 6f6e 2069  led validation i
+0000b620: 6e20 7265 736f 7572 6365 2027 7b63 616c  n resource '{cal
+0000b630: 6c69 6e67 5f72 6573 6f75 7263 657d 272c  ling_resource}',
+0000b640: 2070 726f 7065 7274 7920 277b 6e61 6d65   property '{name
+0000b650: 7d27 3a20 220a 2020 2020 2020 2020 2020  }': ".          
+0000b660: 2020 2020 2020 6622 277b 7661 6c2e 7661        f"'{val.va
+0000b670: 6c75 657d 2720 6973 206e 6f74 2061 2076  lue}' is not a v
+0000b680: 616c 6964 206e 616d 6520 6f66 2061 206c  alid name of a l
+0000b690: 6973 7420 6e6f 6465 2e22 0a20 2020 2020  ist node.".     
+0000b6a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000b6b0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+0000b6c0: 726e 2844 7370 546f 6f6c 7355 7365 7257  rn(DspToolsUserW
+0000b6d0: 6172 6e69 6e67 286d 7367 2929 0a0a 2020  arning(msg))..  
+0000b6e0: 2020 2320 6d61 6b65 2078 6d6c 2073 7472    # make xml str
+0000b6f0: 7563 7475 7265 206f 6620 7468 6520 7661  ucture of the va
+0000b700: 6c69 6420 7661 6c75 6573 0a20 2020 2070  lid values.    p
+0000b710: 726f 705f 203d 2065 7472 6565 2e45 6c65  rop_ = etree.Ele
+0000b720: 6d65 6e74 280a 2020 2020 2020 2020 227b  ment(.        "{
+0000b730: 2573 7d6c 6973 742d 7072 6f70 2220 2520  %s}list-prop" % 
+0000b740: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
+0000b750: 705b 4e6f 6e65 5d2c 0a20 2020 2020 2020  p[None],.       
+0000b760: 206c 6973 743d 6c69 7374 5f6e 616d 652c   list=list_name,
+0000b770: 0a20 2020 2020 2020 206e 616d 653d 6e61  .        name=na
+0000b780: 6d65 2c0a 2020 2020 2020 2020 6e73 6d61  me,.        nsma
+0000b790: 703d 786d 6c5f 6e61 6d65 7370 6163 655f  p=xml_namespace_
+0000b7a0: 6d61 702c 0a20 2020 2029 0a20 2020 2066  map,.    ).    f
+0000b7b0: 6f72 2076 616c 2069 6e20 7661 6c75 6573  or val in values
+0000b7c0: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
+0000b7d0: 203d 207b 2270 6572 6d69 7373 696f 6e73   = {"permissions
+0000b7e0: 223a 2076 616c 2e70 6572 6d69 7373 696f  ": val.permissio
+0000b7f0: 6e73 7d0a 2020 2020 2020 2020 6966 2076  ns}.        if v
+0000b800: 616c 2e63 6f6d 6d65 6e74 2061 6e64 2063  al.comment and c
+0000b810: 6865 636b 5f6e 6f74 6e61 2876 616c 2e63  heck_notna(val.c
+0000b820: 6f6d 6d65 6e74 293a 0a20 2020 2020 2020  omment):.       
+0000b830: 2020 2020 206b 7761 7267 735b 2263 6f6d       kwargs["com
+0000b840: 6d65 6e74 225d 203d 2076 616c 2e63 6f6d  ment"] = val.com
+0000b850: 6d65 6e74 0a20 2020 2020 2020 2076 616c  ment.        val
+0000b860: 7565 5f20 3d20 6574 7265 652e 456c 656d  ue_ = etree.Elem
+0000b870: 656e 7428 0a20 2020 2020 2020 2020 2020  ent(.           
+0000b880: 2022 7b25 737d 6c69 7374 2220 2520 786d   "{%s}list" % xm
+0000b890: 6c5f 6e61 6d65 7370 6163 655f 6d61 705b  l_namespace_map[
+0000b8a0: 4e6f 6e65 5d2c 0a20 2020 2020 2020 2020  None],.         
+0000b8b0: 2020 202a 2a6b 7761 7267 732c 2020 2320     **kwargs,  # 
+0000b8c0: 7479 7065 3a20 6967 6e6f 7265 5b61 7267  type: ignore[arg
+0000b8d0: 2d74 7970 655d 0a20 2020 2020 2020 2020  -type].         
+0000b8e0: 2020 206e 736d 6170 3d78 6d6c 5f6e 616d     nsmap=xml_nam
+0000b8f0: 6573 7061 6365 5f6d 6170 2c0a 2020 2020  espace_map,.    
+0000b900: 2020 2020 290a 2020 2020 2020 2020 7661      ).        va
+0000b910: 6c75 655f 2e74 6578 7420 3d20 7374 7228  lue_.text = str(
+0000b920: 7661 6c2e 7661 6c75 6529 0a20 2020 2020  val.value).     
+0000b930: 2020 2070 726f 705f 2e61 7070 656e 6428     prop_.append(
+0000b940: 7661 6c75 655f 290a 0a20 2020 2072 6574  value_)..    ret
+0000b950: 7572 6e20 7072 6f70 5f0a 0a0a 6465 6620  urn prop_...def 
+0000b960: 6d61 6b65 5f72 6573 7074 725f 7072 6f70  make_resptr_prop
+0000b970: 280a 2020 2020 6e61 6d65 3a20 7374 722c  (.    name: str,
+0000b980: 0a20 2020 2076 616c 7565 3a20 556e 696f  .    value: Unio
+0000b990: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
+0000b9a0: 742c 2073 7472 2c20 4974 6572 6162 6c65  t, str, Iterable
+0000b9b0: 5b55 6e69 6f6e 5b50 726f 7065 7274 7945  [Union[PropertyE
+0000b9c0: 6c65 6d65 6e74 2c20 7374 725d 5d5d 2c0a  lement, str]]],.
+0000b9d0: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
+0000b9e0: 7572 6365 3a20 7374 7220 3d20 2222 2c0a  urce: str = "",.
+0000b9f0: 2920 2d3e 2065 7472 6565 2e5f 456c 656d  ) -> etree._Elem
+0000ba00: 656e 743a 0a20 2020 2022 2222 0a20 2020  ent:.    """.   
+0000ba10: 204d 616b 6520 6120 3c72 6573 7074 722d   Make a <resptr-
+0000ba20: 7072 6f70 3e20 6672 6f6d 206f 6e65 206f  prop> from one o
+0000ba30: 7220 6d6f 7265 2049 4473 206f 6620 6f74  r more IDs of ot
+0000ba40: 6865 7220 7265 736f 7572 6365 732e 2054  her resources. T
+0000ba50: 6865 2049 4428 7329 2063 616e 2062 6520  he ID(s) can be 
+0000ba60: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
+0000ba70: 6e67 206f 7220 6173 0a20 2020 2050 726f  ng or as.    Pro
+0000ba80: 7065 7274 7945 6c65 6d65 6e74 2077 6974  pertyElement wit
+0000ba90: 6820 6120 7374 7269 6e67 2069 6e73 6964  h a string insid
+0000baa0: 652e 2049 6620 7072 6f76 6964 6564 2061  e. If provided a
+0000bab0: 7320 7374 7269 6e67 2c20 7468 6520 7065  s string, the pe
+0000bac0: 726d 6973 7369 6f6e 7320 6465 6661 756c  rmissions defaul
+0000bad0: 7420 746f 2022 7072 6f70 2d64 6566 6175  t to "prop-defau
+0000bae0: 6c74 222e 0a0a 2020 2020 4172 6773 3a0a  lt"...    Args:.
+0000baf0: 2020 2020 2020 2020 6e61 6d65 3a20 7468          name: th
+0000bb00: 6520 6e61 6d65 206f 6620 7468 6973 2070  e name of this p
+0000bb10: 726f 7065 7274 7920 6173 2064 6566 696e  roperty as defin
+0000bb20: 6564 2069 6e20 7468 6520 6f6e 746f 0a20  ed in the onto. 
+0000bb30: 2020 2020 2020 2076 616c 7565 3a20 6f6e         value: on
+0000bb40: 6520 6f72 206d 6f72 6520 7265 736f 7572  e or more resour
+0000bb50: 6365 2069 6465 6e74 6966 6965 7273 2c20  ce identifiers, 
+0000bb60: 6173 2073 7472 696e 672f 5072 6f70 6572  as string/Proper
+0000bb70: 7479 456c 656d 656e 742c 206f 7220 6173  tyElement, or as
+0000bb80: 2069 7465 7261 626c 6520 6f66 2073 7472   iterable of str
+0000bb90: 696e 6773 2f50 726f 7065 7274 7945 6c65  ings/PropertyEle
+0000bba0: 6d65 6e74 730a 2020 2020 2020 2020 6361  ments.        ca
+0000bbb0: 6c6c 696e 675f 7265 736f 7572 6365 3a20  lling_resource: 
+0000bbc0: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
+0000bbd0: 7061 7265 6e74 2072 6573 6f75 7263 6520  parent resource 
+0000bbe0: 2866 6f72 2062 6574 7465 7220 6572 726f  (for better erro
+0000bbf0: 7220 6d65 7373 6167 6573 290a 0a20 2020  r messages)..   
+0000bc00: 2057 6172 6e73 3a0a 2020 2020 2020 2020   Warns:.        
+0000bc10: 4966 2074 6865 2049 4420 6f66 206f 6e65  If the ID of one
+0000bc20: 206f 6620 7468 6520 7461 7267 6574 2072   of the target r
+0000bc30: 6573 6f75 7263 6573 2069 7320 6e6f 7420  esources is not 
+0000bc40: 6120 7661 6c69 6420 7374 7269 6e67 0a0a  a valid string..
+0000bc50: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0000bc60: 2020 2020 2061 6e20 6574 7265 652e 5f45       an etree._E
+0000bc70: 6c65 6d65 6e74 2074 6861 7420 6361 6e20  lement that can 
+0000bc80: 6265 2061 7070 656e 6465 6420 746f 2074  be appended to t
+0000bc90: 6865 2070 6172 656e 7420 7265 736f 7572  he parent resour
+0000bca0: 6365 2077 6974 6820 7265 736f 7572 6365  ce with resource
+0000bcb0: 2e61 7070 656e 6428 6d61 6b65 5f2a 5f70  .append(make_*_p
+0000bcc0: 726f 7028 2e2e 2e29 290a 0a20 2020 2045  rop(...))..    E
+0000bcd0: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
+0000bce0: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
+0000bcf0: 616b 655f 7265 7370 7472 5f70 726f 7028  ake_resptr_prop(
+0000bd00: 223a 7465 7374 7072 6f70 6572 7479 222c  ":testproperty",
+0000bd10: 2022 7265 736f 7572 6365 5f31 2229 0a20   "resource_1"). 
+0000bd20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000bd30: 7265 7370 7472 2d70 726f 7020 6e61 6d65  resptr-prop name
+0000bd40: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
+0000bd50: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000bd60: 2020 2020 2020 3c72 6573 7074 7220 7065        <resptr pe
+0000bd70: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
+0000bd80: 6465 6661 756c 7422 3e72 6573 6f75 7263  default">resourc
+0000bd90: 655f 313c 2f72 6573 7074 723e 0a20 2020  e_1</resptr>.   
+0000bda0: 2020 2020 2020 2020 2020 2020 203c 2f72               </r
+0000bdb0: 6573 7074 722d 7072 6f70 3e0a 2020 2020  esptr-prop>.    
+0000bdc0: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
+0000bdd0: 6c2e 6d61 6b65 5f72 6573 7074 725f 7072  l.make_resptr_pr
+0000bde0: 6f70 2822 3a74 6573 7470 726f 7065 7274  op(":testpropert
+0000bdf0: 7922 2c20 6578 6365 6c32 786d 6c2e 5072  y", excel2xml.Pr
+0000be00: 6f70 6572 7479 456c 656d 656e 7428 2272  opertyElement("r
+0000be10: 6573 6f75 7263 655f 3122 2c20 7065 726d  esource_1", perm
+0000be20: 6973 7369 6f6e 733d 2270 726f 702d 7265  issions="prop-re
+0000be30: 7374 7269 6374 6564 222c 2063 6f6d 6d65  stricted", comme
+0000be40: 6e74 3d22 6578 616d 706c 6522 2929 0a20  nt="example")). 
+0000be50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000be60: 7265 7370 7472 2d70 726f 7020 6e61 6d65  resptr-prop name
+0000be70: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
+0000be80: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000be90: 2020 2020 2020 3c72 6573 7074 7220 7065        <resptr pe
+0000bea0: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
+0000beb0: 7265 7374 7269 6374 6564 2220 636f 6d6d  restricted" comm
+0000bec0: 656e 743d 2265 7861 6d70 6c65 223e 7265  ent="example">re
+0000bed0: 736f 7572 6365 5f31 3c2f 7265 7370 7472  source_1</resptr
+0000bee0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000bef0: 2020 3c2f 7265 7370 7472 2d70 726f 703e    </resptr-prop>
+0000bf00: 0a20 2020 2020 2020 203e 3e3e 2065 7863  .        >>> exc
+0000bf10: 656c 3278 6d6c 2e6d 616b 655f 7265 7370  el2xml.make_resp
+0000bf20: 7472 5f70 726f 7028 223a 7465 7374 7072  tr_prop(":testpr
+0000bf30: 6f70 6572 7479 222c 205b 2272 6573 6f75  operty", ["resou
+0000bf40: 7263 655f 3122 2c20 2272 6573 6f75 7263  rce_1", "resourc
+0000bf50: 655f 3222 5d29 0a20 2020 2020 2020 2020  e_2"]).         
+0000bf60: 2020 2020 2020 203c 7265 7370 7472 2d70         <resptr-p
+0000bf70: 726f 7020 6e61 6d65 3d22 3a74 6573 7470  rop name=":testp
+0000bf80: 726f 7065 7274 7922 3e0a 2020 2020 2020  roperty">.      
+0000bf90: 2020 2020 2020 2020 2020 2020 2020 3c72                <r
+0000bfa0: 6573 7074 7220 7065 726d 6973 7369 6f6e  esptr permission
+0000bfb0: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
+0000bfc0: 3e72 6573 6f75 7263 655f 313c 2f72 6573  >resource_1</res
+0000bfd0: 7074 723e 0a20 2020 2020 2020 2020 2020  ptr>.           
+0000bfe0: 2020 2020 2020 2020 203c 7265 7370 7472           <resptr
+0000bff0: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
+0000c000: 6f70 2d64 6566 6175 6c74 223e 7265 736f  op-default">reso
+0000c010: 7572 6365 5f32 3c2f 7265 7370 7472 3e0a  urce_2</resptr>.
 0000c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c030: 3c72 6573 7074 7220 7065 726d 6973 7369  <resptr permissi
-0000c040: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-0000c050: 7422 3e72 6573 6f75 7263 655f 323c 2f72  t">resource_2</r
-0000c060: 6573 7074 723e 0a20 2020 2020 2020 2020  esptr>.         
-0000c070: 2020 2020 2020 203c 2f72 6573 7074 722d         </resptr-
-0000c080: 7072 6f70 3e0a 0a20 2020 2053 6565 2068  prop>..    See h
-0000c090: 7474 7073 3a2f 2f64 6f63 732e 6461 7363  ttps://docs.dasc
-0000c0a0: 682e 7377 6973 732f 6c61 7465 7374 2f44  h.swiss/latest/D
-0000c0b0: 5350 2d54 4f4f 4c53 2f66 696c 652d 666f  SP-TOOLS/file-fo
-0000c0c0: 726d 6174 732f 786d 6c2d 6461 7461 2d66  rmats/xml-data-f
-0000c0d0: 696c 652f 2372 6573 7074 722d 7072 6f70  ile/#resptr-prop
-0000c0e0: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
-0000c0f0: 6368 6563 6b20 7468 6520 696e 7075 743a  check the input:
-0000c100: 2070 7265 7061 7265 2061 206c 6973 7420   prepare a list 
-0000c110: 7769 7468 2076 616c 6964 2076 616c 7565  with valid value
-0000c120: 730a 2020 2020 7661 6c75 6573 203d 2070  s.    values = p
-0000c130: 7265 7061 7265 5f76 616c 7565 2876 616c  repare_value(val
-0000c140: 7565 290a 0a20 2020 2023 2063 6865 636b  ue)..    # check
-0000c150: 2076 616c 7565 2074 7970 650a 2020 2020   value type.    
-0000c160: 666f 7220 7661 6c20 696e 2076 616c 7565  for val in value
-0000c170: 733a 0a20 2020 2020 2020 2069 6620 6e6f  s:.        if no
-0000c180: 7420 6973 696e 7374 616e 6365 2876 616c  t isinstance(val
-0000c190: 2e76 616c 7565 2c20 7374 7229 206f 7220  .value, str) or 
-0000c1a0: 6e6f 7420 6368 6563 6b5f 6e6f 746e 6128  not check_notna(
-0000c1b0: 7661 6c2e 7661 6c75 6529 3a0a 2020 2020  val.value):.    
-0000c1c0: 2020 2020 2020 2020 6d73 6720 3d20 280a          msg = (.
-0000c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1e0: 6622 5661 6c69 6461 7469 6f6e 2045 7272  f"Validation Err
-0000c1f0: 6f72 2069 6e20 7265 736f 7572 6365 2027  or in resource '
-0000c200: 7b63 616c 6c69 6e67 5f72 6573 6f75 7263  {calling_resourc
-0000c210: 657d 272c 2070 726f 7065 7274 7920 277b  e}', property '{
-0000c220: 6e61 6d65 7d27 3a20 220a 2020 2020 2020  name}': ".      
-0000c230: 2020 2020 2020 2020 2020 6622 5468 6520            f"The 
-0000c240: 666f 6c6c 6f77 696e 6720 646f 6573 6e27  following doesn'
-0000c250: 7420 7365 656d 2074 6f20 6265 2061 2076  t seem to be a v
-0000c260: 616c 6964 2049 4420 6f66 2061 2074 6172  alid ID of a tar
-0000c270: 6765 7420 7265 736f 7572 6365 3a20 277b  get resource: '{
-0000c280: 7661 6c2e 7661 6c75 657d 2722 0a20 2020  val.value}'".   
-0000c290: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000c2a0: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-0000c2b0: 7761 726e 2844 7370 546f 6f6c 7355 7365  warn(DspToolsUse
-0000c2c0: 7257 6172 6e69 6e67 286d 7367 2929 0a0a  rWarning(msg))..
-0000c2d0: 2020 2020 2320 6d61 6b65 2078 6d6c 2073      # make xml s
-0000c2e0: 7472 7563 7475 7265 206f 6620 7468 6520  tructure of the 
-0000c2f0: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
-0000c300: 2070 726f 705f 203d 2065 7472 6565 2e45   prop_ = etree.E
-0000c310: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
-0000c320: 227b 2573 7d72 6573 7074 722d 7072 6f70  "{%s}resptr-prop
-0000c330: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-0000c340: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-0000c350: 2020 2020 206e 616d 653d 6e61 6d65 2c0a       name=name,.
-0000c360: 2020 2020 2020 2020 6e73 6d61 703d 786d          nsmap=xm
-0000c370: 6c5f 6e61 6d65 7370 6163 655f 6d61 702c  l_namespace_map,
-0000c380: 0a20 2020 2029 0a20 2020 2066 6f72 2076  .    ).    for v
-0000c390: 616c 2069 6e20 7661 6c75 6573 3a0a 2020  al in values:.  
-0000c3a0: 2020 2020 2020 6b77 6172 6773 203d 207b        kwargs = {
-0000c3b0: 2270 6572 6d69 7373 696f 6e73 223a 2076  "permissions": v
-0000c3c0: 616c 2e70 6572 6d69 7373 696f 6e73 7d0a  al.permissions}.
-0000c3d0: 2020 2020 2020 2020 6966 2076 616c 2e63          if val.c
-0000c3e0: 6f6d 6d65 6e74 2061 6e64 2063 6865 636b  omment and check
-0000c3f0: 5f6e 6f74 6e61 2876 616c 2e63 6f6d 6d65  _notna(val.comme
-0000c400: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-0000c410: 206b 7761 7267 735b 2263 6f6d 6d65 6e74   kwargs["comment
-0000c420: 225d 203d 2076 616c 2e63 6f6d 6d65 6e74  "] = val.comment
-0000c430: 0a20 2020 2020 2020 2076 616c 7565 5f20  .        value_ 
-0000c440: 3d20 6574 7265 652e 456c 656d 656e 7428  = etree.Element(
-0000c450: 0a20 2020 2020 2020 2020 2020 2022 7b25  .            "{%
-0000c460: 737d 7265 7370 7472 2220 2520 786d 6c5f  s}resptr" % xml_
-0000c470: 6e61 6d65 7370 6163 655f 6d61 705b 4e6f  namespace_map[No
-0000c480: 6e65 5d2c 0a20 2020 2020 2020 2020 2020  ne],.           
-0000c490: 202a 2a6b 7761 7267 732c 2020 2320 7479   **kwargs,  # ty
-0000c4a0: 7065 3a20 6967 6e6f 7265 5b61 7267 2d74  pe: ignore[arg-t
-0000c4b0: 7970 655d 0a20 2020 2020 2020 2020 2020  ype].           
-0000c4c0: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
-0000c4d0: 7061 6365 5f6d 6170 2c0a 2020 2020 2020  pace_map,.      
-0000c4e0: 2020 290a 2020 2020 2020 2020 7661 6c75    ).        valu
-0000c4f0: 655f 2e74 6578 7420 3d20 7374 7228 7661  e_.text = str(va
-0000c500: 6c2e 7661 6c75 6529 0a20 2020 2020 2020  l.value).       
-0000c510: 2070 726f 705f 2e61 7070 656e 6428 7661   prop_.append(va
-0000c520: 6c75 655f 290a 0a20 2020 2072 6574 7572  lue_)..    retur
-0000c530: 6e20 7072 6f70 5f0a 0a0a 6465 6620 6d61  n prop_...def ma
-0000c540: 6b65 5f74 6578 745f 7072 6f70 280a 2020  ke_text_prop(.  
-0000c550: 2020 6e61 6d65 3a20 7374 722c 0a20 2020    name: str,.   
-0000c560: 2076 616c 7565 3a20 556e 696f 6e5b 5072   value: Union[Pr
-0000c570: 6f70 6572 7479 456c 656d 656e 742c 2073  opertyElement, s
-0000c580: 7472 2c20 4974 6572 6162 6c65 5b55 6e69  tr, Iterable[Uni
-0000c590: 6f6e 5b50 726f 7065 7274 7945 6c65 6d65  on[PropertyEleme
-0000c5a0: 6e74 2c20 7374 725d 5d5d 2c0a 2020 2020  nt, str]]],.    
-0000c5b0: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
-0000c5c0: 3a20 7374 7220 3d20 2222 2c0a 2920 2d3e  : str = "",.) ->
-0000c5d0: 2065 7472 6565 2e5f 456c 656d 656e 743a   etree._Element:
-0000c5e0: 0a20 2020 2022 2222 0a20 2020 204d 616b  .    """.    Mak
-0000c5f0: 6520 6120 3c74 6578 742d 7072 6f70 3e20  e a <text-prop> 
-0000c600: 6672 6f6d 206f 6e65 206f 7220 6d6f 7265  from one or more
-0000c610: 2073 7472 696e 6773 2e20 5468 6520 7374   strings. The st
-0000c620: 7269 6e67 2873 2920 6361 6e20 6265 2070  ring(s) can be p
-0000c630: 726f 7669 6465 6420 6173 2073 7472 696e  rovided as strin
-0000c640: 6720 6f72 2061 7320 5072 6f70 6572 7479  g or as Property
-0000c650: 456c 656d 656e 7420 7769 7468 2061 0a20  Element with a. 
-0000c660: 2020 2073 7472 696e 6720 696e 7369 6465     string inside
-0000c670: 2e20 4966 2070 726f 7669 6465 6420 6173  . If provided as
-0000c680: 2073 7472 696e 672c 2074 6865 2065 6e63   string, the enc
-0000c690: 6f64 696e 6720 6465 6661 756c 7473 2074  oding defaults t
-0000c6a0: 6f20 7574 6638 2c20 616e 6420 7468 6520  o utf8, and the 
-0000c6b0: 7065 726d 6973 7369 6f6e 7320 746f 2022  permissions to "
-0000c6c0: 7072 6f70 2d64 6566 6175 6c74 222e 0a0a  prop-default"...
-0000c6d0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000c6e0: 2020 6e61 6d65 3a20 7468 6520 6e61 6d65    name: the name
-0000c6f0: 206f 6620 7468 6973 2070 726f 7065 7274   of this propert
-0000c700: 7920 6173 2064 6566 696e 6564 2069 6e20  y as defined in 
-0000c710: 7468 6520 6f6e 746f 0a20 2020 2020 2020  the onto.       
-0000c720: 2076 616c 7565 3a20 6f6e 6520 6f72 206d   value: one or m
-0000c730: 6f72 6520 7374 7269 6e67 732c 2061 7320  ore strings, as 
-0000c740: 7374 7269 6e67 2f50 726f 7065 7274 7945  string/PropertyE
-0000c750: 6c65 6d65 6e74 2c20 6f72 2061 7320 6974  lement, or as it
-0000c760: 6572 6162 6c65 206f 6620 7374 7269 6e67  erable of string
-0000c770: 732f 5072 6f70 6572 7479 456c 656d 656e  s/PropertyElemen
-0000c780: 7473 0a20 2020 2020 2020 2063 616c 6c69  ts.        calli
-0000c790: 6e67 5f72 6573 6f75 7263 653a 2074 6865  ng_resource: the
-0000c7a0: 206e 616d 6520 6f66 2074 6865 2070 6172   name of the par
-0000c7b0: 656e 7420 7265 736f 7572 6365 2028 666f  ent resource (fo
-0000c7c0: 7220 6265 7474 6572 2065 7272 6f72 206d  r better error m
-0000c7d0: 6573 7361 6765 7329 0a0a 2020 2020 5261  essages)..    Ra
-0000c7e0: 6973 6573 3a0a 2020 2020 2020 2020 4261  ises:.        Ba
-0000c7f0: 7365 4572 726f 723a 2069 6620 7468 6520  seError: if the 
-0000c800: 584d 4c20 7461 6773 2069 6e20 6120 7269  XML tags in a ri
-0000c810: 6368 7465 7874 2070 726f 7065 7274 7920  chtext property 
-0000c820: 2865 6e63 6f64 696e 673d 786d 6c29 2061  (encoding=xml) a
-0000c830: 7265 206e 6f74 2077 656c 6c2d 666f 726d  re not well-form
-0000c840: 6564 0a20 2020 2020 2020 2057 6172 6e69  ed.        Warni
-0000c850: 6e67 3a20 6966 206f 6e65 206f 6620 7468  ng: if one of th
-0000c860: 6520 7661 6c75 6573 2064 6f65 736e 2774  e values doesn't
-0000c870: 206c 6f6f 6b20 6c69 6b65 2061 2072 6561   look like a rea
-0000c880: 736f 6e61 626c 6520 7374 7269 6e67 0a20  sonable string. 
-0000c890: 2020 2020 2020 2020 2020 2028 652e 672e             (e.g.
-0000c8a0: 2022 3c4e 413e 2220 6973 2061 2076 616c   "<NA>" is a val
-0000c8b0: 6964 2073 7472 696e 672c 2062 7574 2070  id string, but p
-0000c8c0: 726f 6261 626c 7920 6e6f 7420 696e 7465  robably not inte
-0000c8d0: 6e64 6564 290a 0a20 2020 2052 6574 7572  nded)..    Retur
-0000c8e0: 6e73 3a0a 2020 2020 2020 2020 616e 2065  ns:.        an e
-0000c8f0: 7472 6565 2e5f 456c 656d 656e 7420 7468  tree._Element th
-0000c900: 6174 2063 616e 2062 6520 6170 7065 6e64  at can be append
-0000c910: 6564 2074 6f20 7468 6520 7061 7265 6e74  ed to the parent
-0000c920: 2072 6573 6f75 7263 6520 7769 7468 2072   resource with r
-0000c930: 6573 6f75 7263 652e 6170 7065 6e64 286d  esource.append(m
-0000c940: 616b 655f 2a5f 7072 6f70 282e 2e2e 2929  ake_*_prop(...))
-0000c950: 0a0a 2020 2020 4578 616d 706c 6573 3a0a  ..    Examples:.
-0000c960: 2020 2020 2020 2020 3e3e 3e20 6578 6365          >>> exce
-0000c970: 6c32 786d 6c2e 6d61 6b65 5f74 6578 745f  l2xml.make_text_
-0000c980: 7072 6f70 2822 3a74 6573 7470 726f 7065  prop(":testprope
-0000c990: 7274 7922 2c20 2266 6972 7374 2074 6578  rty", "first tex
-0000c9a0: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
-0000c9b0: 2020 2020 3c74 6578 742d 7072 6f70 206e      <text-prop n
-0000c9c0: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
-0000c9d0: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
-0000c9e0: 2020 2020 2020 2020 203c 7465 7874 2065           <text e
-0000c9f0: 6e63 6f64 696e 673d 2275 7466 3822 2070  ncoding="utf8" p
-0000ca00: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
-0000ca10: 2d64 6566 6175 6c74 223e 6669 7273 7420  -default">first 
-0000ca20: 7465 7874 3c2f 7465 7874 3e0a 2020 2020  text</text>.    
-0000ca30: 2020 2020 2020 2020 2020 2020 3c2f 7465              </te
-0000ca40: 7874 2d70 726f 703e 0a20 2020 2020 2020  xt-prop>.       
-0000ca50: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
-0000ca60: 616b 655f 7465 7874 5f70 726f 7028 223a  ake_text_prop(":
-0000ca70: 7465 7374 7072 6f70 6572 7479 222c 2065  testproperty", e
-0000ca80: 7863 656c 3278 6d6c 2e50 726f 7065 7274  xcel2xml.Propert
-0000ca90: 7945 6c65 6d65 6e74 2822 6669 7273 7420  yElement("first 
-0000caa0: 7465 7874 222c 2070 6572 6d69 7373 696f  text", permissio
-0000cab0: 6e73 3d22 7072 6f70 2d72 6573 7472 6963  ns="prop-restric
-0000cac0: 7465 6422 2c20 656e 636f 6469 6e67 3d22  ted", encoding="
-0000cad0: 786d 6c22 2929 0a20 2020 2020 2020 2020  xml")).         
-0000cae0: 2020 2020 2020 203c 7465 7874 2d70 726f         <text-pro
-0000caf0: 7020 6e61 6d65 3d22 3a74 6573 7470 726f  p name=":testpro
-0000cb00: 7065 7274 7922 3e0a 2020 2020 2020 2020  perty">.        
-0000cb10: 2020 2020 2020 2020 2020 2020 3c74 6578              <tex
-0000cb20: 7420 656e 636f 6469 6e67 3d22 786d 6c22  t encoding="xml"
-0000cb30: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
-0000cb40: 6f70 2d72 6573 7472 6963 7465 6422 3e66  op-restricted">f
-0000cb50: 6972 7374 2074 6578 743c 2f74 6578 743e  irst text</text>
-0000cb60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cb70: 203c 2f74 6578 742d 7072 6f70 3e0a 2020   </text-prop>.  
-0000cb80: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
-0000cb90: 786d 6c2e 6d61 6b65 5f74 6578 745f 7072  xml.make_text_pr
-0000cba0: 6f70 2822 3a74 6573 7470 726f 7065 7274  op(":testpropert
-0000cbb0: 7922 2c20 5b22 6669 7273 7420 7465 7874  y", ["first text
-0000cbc0: 222c 2022 7365 636f 6e64 2074 6578 7422  ", "second text"
-0000cbd0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0000cbe0: 2020 203c 7465 7874 2d70 726f 7020 6e61     <text-prop na
-0000cbf0: 6d65 3d22 3a74 6573 7470 726f 7065 7274  me=":testpropert
-0000cc00: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
-0000cc10: 2020 2020 2020 2020 3c74 6578 7420 656e          <text en
-0000cc20: 636f 6469 6e67 3d22 7574 6638 2220 7065  coding="utf8" pe
-0000cc30: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-0000cc40: 6465 6661 756c 7422 3e66 6972 7374 2074  default">first t
-0000cc50: 6578 743c 2f74 6578 743e 0a20 2020 2020  ext</text>.     
-0000cc60: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000cc70: 7465 7874 2065 6e63 6f64 696e 673d 2275  text encoding="u
-0000cc80: 7466 3822 2070 6572 6d69 7373 696f 6e73  tf8" permissions
-0000cc90: 3d22 7072 6f70 2d64 6566 6175 6c74 223e  ="prop-default">
-0000cca0: 7365 636f 6e64 2074 6578 743c 2f74 6578  second text</tex
-0000ccb0: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-0000ccc0: 2020 203c 2f74 6578 742d 7072 6f70 3e0a     </text-prop>.
-0000ccd0: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
-0000cce0: 2f64 6f63 732e 6461 7363 682e 7377 6973  /docs.dasch.swis
-0000ccf0: 732f 6c61 7465 7374 2f44 5350 2d54 4f4f  s/latest/DSP-TOO
-0000cd00: 4c53 2f66 696c 652d 666f 726d 6174 732f  LS/file-formats/
-0000cd10: 786d 6c2d 6461 7461 2d66 696c 652f 2374  xml-data-file/#t
-0000cd20: 6578 742d 7072 6f70 0a20 2020 2022 2222  ext-prop.    """
-0000cd30: 0a0a 2020 2020 2320 6368 6563 6b20 7468  ..    # check th
-0000cd40: 6520 696e 7075 743a 2070 7265 7061 7265  e input: prepare
-0000cd50: 2061 206c 6973 7420 7769 7468 2076 616c   a list with val
-0000cd60: 6964 2076 616c 7565 730a 2020 2020 7661  id values.    va
-0000cd70: 6c75 6573 203d 2070 7265 7061 7265 5f76  lues = prepare_v
-0000cd80: 616c 7565 2876 616c 7565 290a 0a20 2020  alue(value)..   
-0000cd90: 2023 2063 6865 636b 2076 616c 7565 2074   # check value t
-0000cda0: 7970 650a 2020 2020 666f 7220 7661 6c20  ype.    for val 
-0000cdb0: 696e 2076 616c 7565 733a 0a20 2020 2020  in values:.     
-0000cdc0: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-0000cdd0: 616e 6365 2876 616c 2e76 616c 7565 2c20  ance(val.value, 
-0000cde0: 7374 7229 206f 7220 6e6f 7420 6368 6563  str) or not chec
-0000cdf0: 6b5f 6e6f 746e 6128 7661 6c2e 7661 6c75  k_notna(val.valu
-0000ce00: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-0000ce10: 6d73 6720 3d20 280a 2020 2020 2020 2020  msg = (.        
-0000ce20: 2020 2020 2020 2020 6622 4661 696c 6564          f"Failed
-0000ce30: 2076 616c 6964 6174 696f 6e20 696e 2072   validation in r
-0000ce40: 6573 6f75 7263 6520 277b 6361 6c6c 696e  esource '{callin
-0000ce50: 675f 7265 736f 7572 6365 7d27 2c20 7072  g_resource}', pr
-0000ce60: 6f70 6572 7479 2027 7b6e 616d 657d 273a  operty '{name}':
-0000ce70: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0000ce80: 2020 2066 2227 7b76 616c 2e76 616c 7565     f"'{val.value
-0000ce90: 7d27 2069 7320 7072 6f62 6162 6c79 206e  }' is probably n
-0000cea0: 6f74 2061 2075 7361 626c 6520 7374 7269  ot a usable stri
-0000ceb0: 6e67 2e22 0a20 2020 2020 2020 2020 2020  ng.".           
-0000cec0: 2029 0a20 2020 2020 2020 2020 2020 2077   ).            w
-0000ced0: 6172 6e69 6e67 732e 7761 726e 2844 7370  arnings.warn(Dsp
-0000cee0: 546f 6f6c 7355 7365 7257 6172 6e69 6e67  ToolsUserWarning
-0000cef0: 286d 7367 2929 0a0a 2020 2020 2320 6d61  (msg))..    # ma
-0000cf00: 6b65 2078 6d6c 2073 7472 7563 7475 7265  ke xml structure
-0000cf10: 206f 6620 7468 6520 7661 6c69 6420 7661   of the valid va
-0000cf20: 6c75 6573 0a20 2020 2070 726f 705f 203d  lues.    prop_ =
-0000cf30: 2065 7472 6565 2e45 6c65 6d65 6e74 280a   etree.Element(.
-0000cf40: 2020 2020 2020 2020 227b 2573 7d74 6578          "{%s}tex
-0000cf50: 742d 7072 6f70 2220 2520 786d 6c5f 6e61  t-prop" % xml_na
-0000cf60: 6d65 7370 6163 655f 6d61 705b 4e6f 6e65  mespace_map[None
-0000cf70: 5d2c 0a20 2020 2020 2020 206e 616d 653d  ],.        name=
-0000cf80: 6e61 6d65 2c0a 2020 2020 2020 2020 6e73  name,.        ns
-0000cf90: 6d61 703d 786d 6c5f 6e61 6d65 7370 6163  map=xml_namespac
-0000cfa0: 655f 6d61 702c 0a20 2020 2029 0a20 2020  e_map,.    ).   
-0000cfb0: 2066 6f72 2076 616c 2069 6e20 7661 6c75   for val in valu
-0000cfc0: 6573 3a0a 2020 2020 2020 2020 6b77 6172  es:.        kwar
-0000cfd0: 6773 203d 207b 2270 6572 6d69 7373 696f  gs = {"permissio
-0000cfe0: 6e73 223a 2076 616c 2e70 6572 6d69 7373  ns": val.permiss
-0000cff0: 696f 6e73 7d0a 2020 2020 2020 2020 6966  ions}.        if
-0000d000: 2063 6865 636b 5f6e 6f74 6e61 2876 616c   check_notna(val
-0000d010: 2e63 6f6d 6d65 6e74 293a 0a20 2020 2020  .comment):.     
-0000d020: 2020 2020 2020 206b 7761 7267 735b 2263         kwargs["c
-0000d030: 6f6d 6d65 6e74 225d 203d 2076 616c 2e63  omment"] = val.c
-0000d040: 6f6d 6d65 6e74 0a20 2020 2020 2020 206b  omment.        k
-0000d050: 7761 7267 735b 2265 6e63 6f64 696e 6722  wargs["encoding"
-0000d060: 5d20 3d20 7661 6c2e 656e 636f 6469 6e67  ] = val.encoding
-0000d070: 2069 6620 6368 6563 6b5f 6e6f 746e 6128   if check_notna(
-0000d080: 7661 6c2e 656e 636f 6469 6e67 2920 656c  val.encoding) el
-0000d090: 7365 2022 7574 6638 220a 2020 2020 2020  se "utf8".      
-0000d0a0: 2020 7661 6c75 655f 203d 2065 7472 6565    value_ = etree
-0000d0b0: 2e45 6c65 6d65 6e74 280a 2020 2020 2020  .Element(.      
-0000d0c0: 2020 2020 2020 227b 2573 7d74 6578 7422        "{%s}text"
-0000d0d0: 2025 2078 6d6c 5f6e 616d 6573 7061 6365   % xml_namespace
-0000d0e0: 5f6d 6170 5b4e 6f6e 655d 2c0a 2020 2020  _map[None],.    
-0000d0f0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-0000d100: 2c20 2023 2074 7970 653a 2069 676e 6f72  ,  # type: ignor
-0000d110: 655b 6172 672d 7479 7065 5d0a 2020 2020  e[arg-type].    
-0000d120: 2020 2020 2020 2020 6e73 6d61 703d 786d          nsmap=xm
-0000d130: 6c5f 6e61 6d65 7370 6163 655f 6d61 702c  l_namespace_map,
-0000d140: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000d150: 2020 2069 6620 6b77 6172 6773 5b22 656e     if kwargs["en
-0000d160: 636f 6469 6e67 225d 203d 3d20 2275 7466  coding"] == "utf
-0000d170: 3822 3a0a 2020 2020 2020 2020 2020 2020  8":.            
-0000d180: 2320 7772 6974 6520 7468 6520 7465 7874  # write the text
-0000d190: 2069 6e74 6f20 7468 6520 7461 672c 2077   into the tag, w
-0000d1a0: 6974 686f 7574 2076 616c 6964 6174 696f  ithout validatio
-0000d1b0: 6e0a 2020 2020 2020 2020 2020 2020 7661  n.            va
-0000d1c0: 6c75 655f 2e74 6578 7420 3d20 7374 7228  lue_.text = str(
-0000d1d0: 7661 6c2e 7661 6c75 6529 0a20 2020 2020  val.value).     
-0000d1e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000d1f0: 2020 2020 2065 7363 6170 6564 5f74 6578       escaped_tex
-0000d200: 7420 3d20 5f65 7363 6170 655f 7265 7365  t = _escape_rese
-0000d210: 7276 6564 5f63 6861 7273 2873 7472 2876  rved_chars(str(v
-0000d220: 616c 2e76 616c 7565 2929 0a20 2020 2020  al.value)).     
-0000d230: 2020 2020 2020 2023 2065 6e66 6f72 6365         # enforce
-0000d240: 2074 6861 7420 7468 6520 7465 7874 2069   that the text i
-0000d250: 7320 7765 6c6c 2d66 6f72 6d65 6420 584d  s well-formed XM
-0000d260: 4c3a 2073 6572 6961 6c69 7a65 2074 6167  L: serialize tag
-0000d270: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-0000d280: 2073 6572 6961 6c69 7a65 6420 3d20 6574   serialized = et
-0000d290: 7265 652e 746f 7374 7269 6e67 2876 616c  ree.tostring(val
-0000d2a0: 7565 5f2c 2065 6e63 6f64 696e 673d 2275  ue_, encoding="u
-0000d2b0: 6e69 636f 6465 2229 0a20 2020 2020 2020  nicode").       
-0000d2c0: 2020 2020 2023 202e 2e2e 2069 6e73 6572       # ... inser
-0000d2d0: 7420 7465 7874 2061 7420 7468 6520 7665  t text at the ve
-0000d2e0: 7279 2065 6e64 206f 6620 7468 6520 7374  ry end of the st
-0000d2f0: 7269 6e67 2c20 616e 6420 6164 6420 656e  ring, and add en
-0000d300: 6469 6e67 2074 6167 2074 6f20 7468 6520  ding tag to the 
-0000d310: 7072 6576 696f 7573 6c79 2073 696e 676c  previously singl
-0000d320: 6520 3c74 6578 742f 3e20 7461 6720 2e2e  e <text/> tag ..
-0000d330: 2e0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000d340: 7269 616c 697a 6564 203d 2072 6567 6578  rialized = regex
-0000d350: 2e73 7562 2872 222f 3e24 222c 2066 223e  .sub(r"/>$", f">
-0000d360: 7b65 7363 6170 6564 5f74 6578 747d 3c2f  {escaped_text}</
-0000d370: 7465 7874 3e22 2c20 7365 7269 616c 697a  text>", serializ
-0000d380: 6564 290a 2020 2020 2020 2020 2020 2020  ed).            
-0000d390: 2320 2e2e 2e20 7472 7920 746f 2070 6172  # ... try to par
-0000d3a0: 7365 2069 7420 6167 6169 6e0a 2020 2020  se it again.    
-0000d3b0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000d3c0: 2020 2020 2020 2020 2020 2020 2076 616c               val
-0000d3d0: 7565 5f20 3d20 6574 7265 652e 6672 6f6d  ue_ = etree.from
-0000d3e0: 7374 7269 6e67 2873 6572 6961 6c69 7a65  string(serialize
-0000d3f0: 6429 0a20 2020 2020 2020 2020 2020 2065  d).            e
-0000d400: 7863 6570 7420 6574 7265 652e 584d 4c53  xcept etree.XMLS
-0000d410: 796e 7461 7845 7272 6f72 2061 7320 6572  yntaxError as er
-0000d420: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0000d430: 2020 206d 7367 203d 2028 0a20 2020 2020     msg = (.     
-0000d440: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000d450: 5468 6520 584d 4c20 7461 6773 2063 6f6e  The XML tags con
-0000d460: 7461 696e 6564 2069 6e20 6120 7269 6368  tained in a rich
-0000d470: 7465 7874 2070 726f 7065 7274 7920 2865  text property (e
-0000d480: 6e63 6f64 696e 673d 786d 6c29 206d 7573  ncoding=xml) mus
-0000d490: 7420 6265 2077 656c 6c2d 666f 726d 6564  t be well-formed
-0000d4a0: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-0000d4b0: 2020 2020 2020 2020 2254 6865 2073 7065          "The spe
-0000d4c0: 6369 616c 2063 6861 7261 6374 6572 7320  cial characters 
-0000d4d0: 3c2c 203e 2061 6e64 2026 2061 7265 206f  <, > and & are o
-0000d4e0: 6e6c 7920 616c 6c6f 7765 6420 746f 2063  nly allowed to c
-0000d4f0: 6f6e 7374 7275 6374 2061 2074 6167 2e20  onstruct a tag. 
-0000d500: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000d510: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000d520: 2020 2020 6966 2063 616c 6c69 6e67 5f72      if calling_r
-0000d530: 6573 6f75 7263 653a 0a20 2020 2020 2020  esource:.       
-0000d540: 2020 2020 2020 2020 2020 2020 206d 7367               msg
-0000d550: 202b 3d20 6622 5468 6520 6572 726f 7220   += f"The error 
-0000d560: 6f63 6375 7272 6564 2069 6e20 7265 736f  occurred in reso
-0000d570: 7572 6365 207b 6361 6c6c 696e 675f 7265  urce {calling_re
-0000d580: 736f 7572 6365 7d2c 2070 726f 7065 7274  source}, propert
-0000d590: 7920 7b6e 616d 657d 220a 2020 2020 2020  y {name}".      
-0000d5a0: 2020 2020 2020 2020 2020 6d73 6720 2b3d            msg +=
-0000d5b0: 2066 225c 6e4f 7269 6769 6e61 6c20 6572   f"\nOriginal er
-0000d5c0: 726f 7220 6d65 7373 6167 653a 207b 6572  ror message: {er
-0000d5d0: 722e 6d73 677d 220a 2020 2020 2020 2020  r.msg}".        
-0000d5e0: 2020 2020 2020 2020 6d73 6720 2b3d 2066          msg += f
-0000d5f0: 225c 6e45 7665 6e74 7561 6c20 6c69 6e65  "\nEventual line
-0000d600: 2f63 6f6c 756d 6e20 6e75 6d62 6572 7320  /column numbers 
-0000d610: 6172 6520 7265 6c61 7469 7665 2074 6f20  are relative to 
-0000d620: 7468 6973 2073 6572 6961 6c69 7a65 6420  this serialized 
-0000d630: 7465 7874 3a20 7b73 6572 6961 6c69 7a65  text: {serialize
-0000d640: 647d 220a 2020 2020 2020 2020 2020 2020  d}".            
-0000d650: 2020 2020 7261 6973 6520 4261 7365 4572      raise BaseEr
-0000d660: 726f 7228 6d73 6729 2066 726f 6d20 4e6f  ror(msg) from No
-0000d670: 6e65 0a20 2020 2020 2020 2070 726f 705f  ne.        prop_
-0000d680: 2e61 7070 656e 6428 7661 6c75 655f 290a  .append(value_).
-0000d690: 0a20 2020 2072 6574 7572 6e20 7072 6f70  .    return prop
-0000d6a0: 5f0a 0a0a 6465 6620 5f65 7363 6170 655f  _...def _escape_
-0000d6b0: 7265 7365 7276 6564 5f63 6861 7273 2874  reserved_chars(t
-0000d6c0: 6578 743a 2073 7472 2920 2d3e 2073 7472  ext: str) -> str
-0000d6d0: 3a0a 2020 2020 2222 220a 2020 2020 4672  :.    """.    Fr
-0000d6e0: 6f6d 2072 6963 6874 6578 7420 7374 7269  om richtext stri
-0000d6f0: 6e67 7320 2865 6e63 6f64 696e 673d 2278  ngs (encoding="x
-0000d700: 6d6c 2229 2c20 6573 6361 7065 2074 6865  ml"), escape the
-0000d710: 2072 6573 6572 7665 6420 6368 6172 6163   reserved charac
-0000d720: 7465 7273 203c 2c20 3e20 616e 6420 262c  ters <, > and &,
-0000d730: 0a20 2020 2062 7574 206f 6e6c 7920 6966  .    but only if
-0000d740: 2074 6865 7920 6172 6520 6e6f 7420 7061   they are not pa
-0000d750: 7274 206f 6620 6120 7374 616e 6461 7264  rt of a standard
-0000d760: 2073 7461 6e64 6f66 6620 7461 6720 6f72   standoff tag or
-0000d770: 2065 7363 6170 6520 7365 7175 656e 6365   escape sequence
-0000d780: 2e0a 2020 2020 5468 6520 7374 616e 6461  ..    The standa
-0000d790: 7264 2073 7461 6e64 6f66 6620 7461 6773  rd standoff tags
-0000d7a0: 2061 6c6c 6f77 6564 2062 7920 4453 502d   allowed by DSP-
-0000d7b0: 4150 4920 6172 6520 646f 6375 6d65 6e74  API are document
-0000d7c0: 6564 2068 6572 653a 0a20 2020 2068 7474  ed here:.    htt
-0000d7d0: 7073 3a2f 2f64 6f63 732e 6461 7363 682e  ps://docs.dasch.
-0000d7e0: 7377 6973 732f 3230 3233 2e31 322e 3031  swiss/2023.12.01
-0000d7f0: 2f44 5350 2d41 5049 2f30 332d 656e 6470  /DSP-API/03-endp
-0000d800: 6f69 6e74 732f 6170 692d 7632 2f74 6578  oints/api-v2/tex
-0000d810: 742f 7374 616e 6461 7264 2d73 7461 6e64  t/standard-stand
-0000d820: 6f66 662f 0a0a 2020 2020 4172 6773 3a0a  off/..    Args:.
-0000d830: 2020 2020 2020 2020 7465 7874 3a20 7468          text: th
-0000d840: 6520 7269 6368 7465 7874 2073 7472 696e  e richtext strin
-0000d850: 6720 746f 2062 6520 6573 6361 7065 640a  g to be escaped.
-0000d860: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-0000d870: 2020 2020 2020 7468 6520 6573 6361 7065        the escape
-0000d880: 6420 7269 6368 7465 7874 2073 7472 696e  d richtext strin
-0000d890: 670a 2020 2020 2222 220a 2020 2020 616c  g.    """.    al
-0000d8a0: 6c6f 7765 645f 7461 6773 203d 205b 0a20  lowed_tags = [. 
-0000d8b0: 2020 2020 2020 2022 6128 205b 5e3e 5d2b         "a( [^>]+
-0000d8c0: 293f 222c 2020 2320 3c61 3e20 6973 2074  )?",  # <a> is t
-0000d8d0: 6865 206f 6e6c 7920 7461 6720 7468 6174  he only tag that
-0000d8e0: 2063 616e 2068 6176 6520 6174 7472 6962   can have attrib
-0000d8f0: 7574 6573 0a20 2020 2020 2020 2022 7022  utes.        "p"
-0000d900: 2c0a 2020 2020 2020 2020 2265 6d22 2c0a  ,.        "em",.
-0000d910: 2020 2020 2020 2020 2273 7472 6f6e 6722          "strong"
-0000d920: 2c0a 2020 2020 2020 2020 2275 222c 0a20  ,.        "u",. 
-0000d930: 2020 2020 2020 2022 7375 6222 2c0a 2020         "sub",.  
-0000d940: 2020 2020 2020 2273 7570 222c 0a20 2020        "sup",.   
-0000d950: 2020 2020 2022 7374 7269 6b65 222c 0a20       "strike",. 
-0000d960: 2020 2020 2020 2022 6831 222c 0a20 2020         "h1",.   
-0000d970: 2020 2020 2022 6f6c 222c 0a20 2020 2020       "ol",.     
-0000d980: 2020 2022 756c 222c 0a20 2020 2020 2020     "ul",.       
-0000d990: 2022 6c69 222c 0a20 2020 2020 2020 2022   "li",.        "
-0000d9a0: 7462 6f64 7922 2c0a 2020 2020 2020 2020  tbody",.        
-0000d9b0: 2274 6162 6c65 222c 0a20 2020 2020 2020  "table",.       
-0000d9c0: 2022 7472 222c 0a20 2020 2020 2020 2022   "tr",.        "
-0000d9d0: 7464 222c 0a20 2020 2020 2020 2022 6272  td",.        "br
-0000d9e0: 222c 0a20 2020 2020 2020 2022 6872 222c  ",.        "hr",
-0000d9f0: 0a20 2020 2020 2020 2022 7072 6522 2c0a  .        "pre",.
-0000da00: 2020 2020 2020 2020 2263 6974 6522 2c0a          "cite",.
-0000da10: 2020 2020 2020 2020 2262 6c6f 636b 7175          "blockqu
-0000da20: 6f74 6522 2c0a 2020 2020 2020 2020 2263  ote",.        "c
-0000da30: 6f64 6522 2c0a 2020 2020 5d0a 2020 2020  ode",.    ].    
-0000da40: 616c 6c6f 7765 645f 7461 6773 5f72 6567  allowed_tags_reg
-0000da50: 6578 203d 2022 7c22 2e6a 6f69 6e28 616c  ex = "|".join(al
-0000da60: 6c6f 7765 645f 7461 6773 290a 2020 2020  lowed_tags).    
-0000da70: 6c6f 6f6b 6168 6561 6420 3d20 7266 2228  lookahead = rf"(
-0000da80: 3f21 2f3f 287b 616c 6c6f 7765 645f 7461  ?!/?({allowed_ta
-0000da90: 6773 5f72 6567 6578 7d29 2f3f 3e29 220a  gs_regex})/?>)".
-0000daa0: 2020 2020 696c 6c65 6761 6c5f 6c74 203d      illegal_lt =
-0000dab0: 2072 6622 3c7b 6c6f 6f6b 6168 6561 647d   rf"<{lookahead}
-0000dac0: 220a 2020 2020 6c6f 6f6b 6265 6869 6e64  ".    lookbehind
-0000dad0: 203d 2072 6622 283f 3c21 3c2f 3f28 7b61   = rf"(?<!</?({a
-0000dae0: 6c6c 6f77 6564 5f74 6167 735f 7265 6765  llowed_tags_rege
-0000daf0: 787d 292f 3f29 220a 2020 2020 696c 6c65  x})/?)".    ille
-0000db00: 6761 6c5f 6774 203d 2072 6622 7b6c 6f6f  gal_gt = rf"{loo
-0000db10: 6b62 6568 696e 647d 3e22 0a20 2020 2069  kbehind}>".    i
-0000db20: 6c6c 6567 616c 5f61 6d70 203d 2072 2226  llegal_amp = r"&
-0000db30: 283f 215b 2361 2d7a 412d 5a30 2d39 5d2b  (?![#a-zA-Z0-9]+
-0000db40: 3b29 220a 2020 2020 7465 7874 203d 2072  ;)".    text = r
-0000db50: 6567 6578 2e73 7562 2869 6c6c 6567 616c  egex.sub(illegal
-0000db60: 5f6c 742c 2022 266c 743b 222c 2074 6578  _lt, "&lt;", tex
-0000db70: 7429 0a20 2020 2074 6578 7420 3d20 7265  t).    text = re
-0000db80: 6765 782e 7375 6228 696c 6c65 6761 6c5f  gex.sub(illegal_
-0000db90: 6774 2c20 2226 6774 3b22 2c20 7465 7874  gt, "&gt;", text
-0000dba0: 290a 2020 2020 7465 7874 203d 2072 6567  ).    text = reg
-0000dbb0: 6578 2e73 7562 2869 6c6c 6567 616c 5f61  ex.sub(illegal_a
-0000dbc0: 6d70 2c20 2226 616d 703b 222c 2074 6578  mp, "&amp;", tex
-0000dbd0: 7429 0a20 2020 2072 6574 7572 6e20 7465  t).    return te
-0000dbe0: 7874 0a0a 0a64 6566 206d 616b 655f 7469  xt...def make_ti
-0000dbf0: 6d65 5f70 726f 7028 0a20 2020 206e 616d  me_prop(.    nam
-0000dc00: 653a 2073 7472 2c0a 2020 2020 7661 6c75  e: str,.    valu
-0000dc10: 653a 2055 6e69 6f6e 5b50 726f 7065 7274  e: Union[Propert
-0000dc20: 7945 6c65 6d65 6e74 2c20 7374 722c 2049  yElement, str, I
-0000dc30: 7465 7261 626c 655b 556e 696f 6e5b 5072  terable[Union[Pr
-0000dc40: 6f70 6572 7479 456c 656d 656e 742c 2073  opertyElement, s
-0000dc50: 7472 5d5d 5d2c 0a20 2020 2063 616c 6c69  tr]]],.    calli
-0000dc60: 6e67 5f72 6573 6f75 7263 653a 2073 7472  ng_resource: str
-0000dc70: 203d 2022 222c 0a29 202d 3e20 6574 7265   = "",.) -> etre
-0000dc80: 652e 5f45 6c65 6d65 6e74 3a0a 2020 2020  e._Element:.    
-0000dc90: 2222 220a 2020 2020 4d61 6b65 2061 203c  """.    Make a <
-0000dca0: 7469 6d65 2d70 726f 703e 2066 726f 6d20  time-prop> from 
-0000dcb0: 6f6e 6520 6f72 206d 6f72 6520 6461 7465  one or more date
-0000dcc0: 7469 6d65 2076 616c 7565 7320 6f66 2074  time values of t
-0000dcd0: 6865 2066 6f72 6d20 2232 3030 392d 3130  he form "2009-10
-0000dce0: 2d31 3054 3132 3a30 303a 3030 2d30 353a  -10T12:00:00-05:
-0000dcf0: 3030 222e 2054 6865 2074 696d 6528 7329  00". The time(s)
-0000dd00: 2063 616e 2062 650a 2020 2020 7072 6f76   can be.    prov
-0000dd10: 6964 6564 2061 7320 7374 7269 6e67 206f  ided as string o
-0000dd20: 7220 6173 2050 726f 7065 7274 7945 6c65  r as PropertyEle
-0000dd30: 6d65 6e74 2077 6974 6820 6120 7374 7269  ment with a stri
-0000dd40: 6e67 2069 6e73 6964 652e 2049 6620 7072  ng inside. If pr
-0000dd50: 6f76 6964 6564 2061 7320 7374 7269 6e67  ovided as string
-0000dd60: 2c20 7468 6520 7065 726d 6973 7369 6f6e  , the permission
-0000dd70: 7320 6465 6661 756c 7420 746f 0a20 2020  s default to.   
-0000dd80: 2022 7072 6f70 2d64 6566 6175 6c74 222e   "prop-default".
-0000dd90: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-0000dda0: 2020 2020 6e61 6d65 3a20 7468 6520 6e61      name: the na
-0000ddb0: 6d65 206f 6620 7468 6973 2070 726f 7065  me of this prope
-0000ddc0: 7274 7920 6173 2064 6566 696e 6564 2069  rty as defined i
-0000ddd0: 6e20 7468 6520 6f6e 746f 0a20 2020 2020  n the onto.     
-0000dde0: 2020 2076 616c 7565 3a20 6f6e 6520 6f72     value: one or
-0000ddf0: 206d 6f72 6520 4453 5020 7469 6d65 732c   more DSP times,
-0000de00: 2061 7320 7374 7269 6e67 2f50 726f 7065   as string/Prope
-0000de10: 7274 7945 6c65 6d65 6e74 2c20 6f72 2061  rtyElement, or a
-0000de20: 7320 6974 6572 6162 6c65 206f 6620 7374  s iterable of st
-0000de30: 7269 6e67 732f 5072 6f70 6572 7479 456c  rings/PropertyEl
-0000de40: 656d 656e 7473 0a20 2020 2020 2020 2063  ements.        c
-0000de50: 616c 6c69 6e67 5f72 6573 6f75 7263 653a  alling_resource:
-0000de60: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
-0000de70: 2070 6172 656e 7420 7265 736f 7572 6365   parent resource
-0000de80: 2028 666f 7220 6265 7474 6572 2065 7272   (for better err
-0000de90: 6f72 206d 6573 7361 6765 7329 0a0a 2020  or messages)..  
-0000dea0: 2020 5761 726e 733a 0a20 2020 2020 2020    Warns:.       
-0000deb0: 2049 6620 6f6e 6520 6f66 2074 6865 2076   If one of the v
-0000dec0: 616c 7565 7320 6973 206e 6f74 2061 2076  alues is not a v
-0000ded0: 616c 6964 2044 5350 2074 696d 6520 7374  alid DSP time st
-0000dee0: 7269 6e67 0a0a 2020 2020 5265 7475 726e  ring..    Return
-0000def0: 733a 0a20 2020 2020 2020 2061 6e20 6574  s:.        an et
-0000df00: 7265 652e 5f45 6c65 6d65 6e74 2074 6861  ree._Element tha
-0000df10: 7420 6361 6e20 6265 2061 7070 656e 6465  t can be appende
-0000df20: 6420 746f 2074 6865 2070 6172 656e 7420  d to the parent 
-0000df30: 7265 736f 7572 6365 2077 6974 6820 7265  resource with re
-0000df40: 736f 7572 6365 2e61 7070 656e 6428 6d61  source.append(ma
-0000df50: 6b65 5f2a 5f70 726f 7028 2e2e 2e29 290a  ke_*_prop(...)).
-0000df60: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
-0000df70: 2020 2020 2020 203e 3e3e 2065 7863 656c         >>> excel
-0000df80: 3278 6d6c 2e6d 616b 655f 7469 6d65 5f70  2xml.make_time_p
-0000df90: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
-0000dfa0: 7479 222c 2022 3230 3039 2d31 302d 3130  ty", "2009-10-10
-0000dfb0: 5431 323a 3030 3a30 302d 3035 3a30 3022  T12:00:00-05:00"
-0000dfc0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000dfd0: 2020 3c74 696d 652d 7072 6f70 206e 616d    <time-prop nam
-0000dfe0: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
-0000dff0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-0000e000: 2020 2020 2020 203c 7469 6d65 2070 6572         <time per
-0000e010: 6d69 7373 696f 6e73 3d22 7072 6f70 2d64  missions="prop-d
-0000e020: 6566 6175 6c74 223e 0a20 2020 2020 2020  efault">.       
+0000c030: 3c2f 7265 7370 7472 2d70 726f 703e 0a0a  </resptr-prop>..
+0000c040: 2020 2020 5365 6520 6874 7470 733a 2f2f      See https://
+0000c050: 646f 6373 2e64 6173 6368 2e73 7769 7373  docs.dasch.swiss
+0000c060: 2f6c 6174 6573 742f 4453 502d 544f 4f4c  /latest/DSP-TOOL
+0000c070: 532f 6669 6c65 2d66 6f72 6d61 7473 2f78  S/file-formats/x
+0000c080: 6d6c 2d64 6174 612d 6669 6c65 2f23 7265  ml-data-file/#re
+0000c090: 7370 7472 2d70 726f 700a 2020 2020 2222  sptr-prop.    ""
+0000c0a0: 220a 0a20 2020 2023 2063 6865 636b 2074  "..    # check t
+0000c0b0: 6865 2069 6e70 7574 3a20 7072 6570 6172  he input: prepar
+0000c0c0: 6520 6120 6c69 7374 2077 6974 6820 7661  e a list with va
+0000c0d0: 6c69 6420 7661 6c75 6573 0a20 2020 2076  lid values.    v
+0000c0e0: 616c 7565 7320 3d20 7072 6570 6172 655f  alues = prepare_
+0000c0f0: 7661 6c75 6528 7661 6c75 6529 0a0a 2020  value(value)..  
+0000c100: 2020 2320 6368 6563 6b20 7661 6c75 6520    # check value 
+0000c110: 7479 7065 0a20 2020 2066 6f72 2076 616c  type.    for val
+0000c120: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
+0000c130: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+0000c140: 7461 6e63 6528 7661 6c2e 7661 6c75 652c  tance(val.value,
+0000c150: 2073 7472 2920 6f72 206e 6f74 2063 6865   str) or not che
+0000c160: 636b 5f6e 6f74 6e61 2876 616c 2e76 616c  ck_notna(val.val
+0000c170: 7565 293a 0a20 2020 2020 2020 2020 2020  ue):.           
+0000c180: 206d 7367 203d 2028 0a20 2020 2020 2020   msg = (.       
+0000c190: 2020 2020 2020 2020 2066 2256 616c 6964           f"Valid
+0000c1a0: 6174 696f 6e20 4572 726f 7220 696e 2072  ation Error in r
+0000c1b0: 6573 6f75 7263 6520 277b 6361 6c6c 696e  esource '{callin
+0000c1c0: 675f 7265 736f 7572 6365 7d27 2c20 7072  g_resource}', pr
+0000c1d0: 6f70 6572 7479 2027 7b6e 616d 657d 273a  operty '{name}':
+0000c1e0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000c1f0: 2020 2066 2254 6865 2066 6f6c 6c6f 7769     f"The followi
+0000c200: 6e67 2064 6f65 736e 2774 2073 6565 6d20  ng doesn't seem 
+0000c210: 746f 2062 6520 6120 7661 6c69 6420 4944  to be a valid ID
+0000c220: 206f 6620 6120 7461 7267 6574 2072 6573   of a target res
+0000c230: 6f75 7263 653a 2027 7b76 616c 2e76 616c  ource: '{val.val
+0000c240: 7565 7d27 220a 2020 2020 2020 2020 2020  ue}'".          
+0000c250: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000c260: 7761 726e 696e 6773 2e77 6172 6e28 4473  warnings.warn(Ds
+0000c270: 7054 6f6f 6c73 5573 6572 5761 726e 696e  pToolsUserWarnin
+0000c280: 6728 6d73 6729 290a 0a20 2020 2023 206d  g(msg))..    # m
+0000c290: 616b 6520 786d 6c20 7374 7275 6374 7572  ake xml structur
+0000c2a0: 6520 6f66 2074 6865 2076 616c 6964 2076  e of the valid v
+0000c2b0: 616c 7565 730a 2020 2020 7072 6f70 5f20  alues.    prop_ 
+0000c2c0: 3d20 6574 7265 652e 456c 656d 656e 7428  = etree.Element(
+0000c2d0: 0a20 2020 2020 2020 2022 7b25 737d 7265  .        "{%s}re
+0000c2e0: 7370 7472 2d70 726f 7022 2025 2078 6d6c  sptr-prop" % xml
+0000c2f0: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
+0000c300: 6f6e 655d 2c0a 2020 2020 2020 2020 6e61  one],.        na
+0000c310: 6d65 3d6e 616d 652c 0a20 2020 2020 2020  me=name,.       
+0000c320: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
+0000c330: 7061 6365 5f6d 6170 2c0a 2020 2020 290a  pace_map,.    ).
+0000c340: 2020 2020 666f 7220 7661 6c20 696e 2076      for val in v
+0000c350: 616c 7565 733a 0a20 2020 2020 2020 206b  alues:.        k
+0000c360: 7761 7267 7320 3d20 7b22 7065 726d 6973  wargs = {"permis
+0000c370: 7369 6f6e 7322 3a20 7661 6c2e 7065 726d  sions": val.perm
+0000c380: 6973 7369 6f6e 737d 0a20 2020 2020 2020  issions}.       
+0000c390: 2069 6620 7661 6c2e 636f 6d6d 656e 7420   if val.comment 
+0000c3a0: 616e 6420 6368 6563 6b5f 6e6f 746e 6128  and check_notna(
+0000c3b0: 7661 6c2e 636f 6d6d 656e 7429 3a0a 2020  val.comment):.  
+0000c3c0: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
+0000c3d0: 5b22 636f 6d6d 656e 7422 5d20 3d20 7661  ["comment"] = va
+0000c3e0: 6c2e 636f 6d6d 656e 740a 2020 2020 2020  l.comment.      
+0000c3f0: 2020 7661 6c75 655f 203d 2065 7472 6565    value_ = etree
+0000c400: 2e45 6c65 6d65 6e74 280a 2020 2020 2020  .Element(.      
+0000c410: 2020 2020 2020 227b 2573 7d72 6573 7074        "{%s}respt
+0000c420: 7222 2025 2078 6d6c 5f6e 616d 6573 7061  r" % xml_namespa
+0000c430: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
+0000c440: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+0000c450: 6773 2c20 2023 2074 7970 653a 2069 676e  gs,  # type: ign
+0000c460: 6f72 655b 6172 672d 7479 7065 5d0a 2020  ore[arg-type].  
+0000c470: 2020 2020 2020 2020 2020 6e73 6d61 703d            nsmap=
+0000c480: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
+0000c490: 702c 0a20 2020 2020 2020 2029 0a20 2020  p,.        ).   
+0000c4a0: 2020 2020 2076 616c 7565 5f2e 7465 7874       value_.text
+0000c4b0: 203d 2073 7472 2876 616c 2e76 616c 7565   = str(val.value
+0000c4c0: 290a 2020 2020 2020 2020 7072 6f70 5f2e  ).        prop_.
+0000c4d0: 6170 7065 6e64 2876 616c 7565 5f29 0a0a  append(value_)..
+0000c4e0: 2020 2020 7265 7475 726e 2070 726f 705f      return prop_
+0000c4f0: 0a0a 0a64 6566 206d 616b 655f 7465 7874  ...def make_text
+0000c500: 5f70 726f 7028 0a20 2020 206e 616d 653a  _prop(.    name:
+0000c510: 2073 7472 2c0a 2020 2020 7661 6c75 653a   str,.    value:
+0000c520: 2055 6e69 6f6e 5b50 726f 7065 7274 7945   Union[PropertyE
+0000c530: 6c65 6d65 6e74 2c20 7374 722c 2049 7465  lement, str, Ite
+0000c540: 7261 626c 655b 556e 696f 6e5b 5072 6f70  rable[Union[Prop
+0000c550: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
+0000c560: 5d5d 5d2c 0a20 2020 2063 616c 6c69 6e67  ]]],.    calling
+0000c570: 5f72 6573 6f75 7263 653a 2073 7472 203d  _resource: str =
+0000c580: 2022 222c 0a29 202d 3e20 6574 7265 652e   "",.) -> etree.
+0000c590: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
+0000c5a0: 220a 2020 2020 4d61 6b65 2061 203c 7465  ".    Make a <te
+0000c5b0: 7874 2d70 726f 703e 2066 726f 6d20 6f6e  xt-prop> from on
+0000c5c0: 6520 6f72 206d 6f72 6520 7374 7269 6e67  e or more string
+0000c5d0: 732e 2054 6865 2073 7472 696e 6728 7329  s. The string(s)
+0000c5e0: 2063 616e 2062 6520 7072 6f76 6964 6564   can be provided
+0000c5f0: 2061 7320 7374 7269 6e67 206f 7220 6173   as string or as
+0000c600: 2050 726f 7065 7274 7945 6c65 6d65 6e74   PropertyElement
+0000c610: 2077 6974 6820 610a 2020 2020 7374 7269   with a.    stri
+0000c620: 6e67 2069 6e73 6964 652e 2049 6620 7072  ng inside. If pr
+0000c630: 6f76 6964 6564 2061 7320 7374 7269 6e67  ovided as string
+0000c640: 2c20 7468 6520 656e 636f 6469 6e67 2064  , the encoding d
+0000c650: 6566 6175 6c74 7320 746f 2075 7466 382c  efaults to utf8,
+0000c660: 2061 6e64 2074 6865 2070 6572 6d69 7373   and the permiss
+0000c670: 696f 6e73 2074 6f20 2270 726f 702d 6465  ions to "prop-de
+0000c680: 6661 756c 7422 2e0a 0a20 2020 2041 7267  fault"...    Arg
+0000c690: 733a 0a20 2020 2020 2020 206e 616d 653a  s:.        name:
+0000c6a0: 2074 6865 206e 616d 6520 6f66 2074 6869   the name of thi
+0000c6b0: 7320 7072 6f70 6572 7479 2061 7320 6465  s property as de
+0000c6c0: 6669 6e65 6420 696e 2074 6865 206f 6e74  fined in the ont
+0000c6d0: 6f0a 2020 2020 2020 2020 7661 6c75 653a  o.        value:
+0000c6e0: 206f 6e65 206f 7220 6d6f 7265 2073 7472   one or more str
+0000c6f0: 696e 6773 2c20 6173 2073 7472 696e 672f  ings, as string/
+0000c700: 5072 6f70 6572 7479 456c 656d 656e 742c  PropertyElement,
+0000c710: 206f 7220 6173 2069 7465 7261 626c 6520   or as iterable 
+0000c720: 6f66 2073 7472 696e 6773 2f50 726f 7065  of strings/Prope
+0000c730: 7274 7945 6c65 6d65 6e74 730a 2020 2020  rtyElements.    
+0000c740: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
+0000c750: 7572 6365 3a20 7468 6520 6e61 6d65 206f  urce: the name o
+0000c760: 6620 7468 6520 7061 7265 6e74 2072 6573  f the parent res
+0000c770: 6f75 7263 6520 2866 6f72 2062 6574 7465  ource (for bette
+0000c780: 7220 6572 726f 7220 6d65 7373 6167 6573  r error messages
+0000c790: 290a 0a20 2020 2052 6169 7365 733a 0a20  )..    Raises:. 
+0000c7a0: 2020 2020 2020 2042 6173 6545 7272 6f72         BaseError
+0000c7b0: 3a20 6966 2074 6865 2058 4d4c 2074 6167  : if the XML tag
+0000c7c0: 7320 696e 2061 2072 6963 6874 6578 7420  s in a richtext 
+0000c7d0: 7072 6f70 6572 7479 2028 656e 636f 6469  property (encodi
+0000c7e0: 6e67 3d78 6d6c 2920 6172 6520 6e6f 7420  ng=xml) are not 
+0000c7f0: 7765 6c6c 2d66 6f72 6d65 640a 2020 2020  well-formed.    
+0000c800: 2020 2020 5761 726e 696e 673a 2069 6620      Warning: if 
+0000c810: 6f6e 6520 6f66 2074 6865 2076 616c 7565  one of the value
+0000c820: 7320 646f 6573 6e27 7420 6c6f 6f6b 206c  s doesn't look l
+0000c830: 696b 6520 6120 7265 6173 6f6e 6162 6c65  ike a reasonable
+0000c840: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+0000c850: 2020 2020 2865 2e67 2e20 223c 4e41 3e22      (e.g. "<NA>"
+0000c860: 2069 7320 6120 7661 6c69 6420 7374 7269   is a valid stri
+0000c870: 6e67 2c20 6275 7420 7072 6f62 6162 6c79  ng, but probably
+0000c880: 206e 6f74 2069 6e74 656e 6465 6429 0a0a   not intended)..
+0000c890: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0000c8a0: 2020 2020 2061 6e20 6574 7265 652e 5f45       an etree._E
+0000c8b0: 6c65 6d65 6e74 2074 6861 7420 6361 6e20  lement that can 
+0000c8c0: 6265 2061 7070 656e 6465 6420 746f 2074  be appended to t
+0000c8d0: 6865 2070 6172 656e 7420 7265 736f 7572  he parent resour
+0000c8e0: 6365 2077 6974 6820 7265 736f 7572 6365  ce with resource
+0000c8f0: 2e61 7070 656e 6428 6d61 6b65 5f2a 5f70  .append(make_*_p
+0000c900: 726f 7028 2e2e 2e29 290a 0a20 2020 2045  rop(...))..    E
+0000c910: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
+0000c920: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
+0000c930: 616b 655f 7465 7874 5f70 726f 7028 223a  ake_text_prop(":
+0000c940: 7465 7374 7072 6f70 6572 7479 222c 2022  testproperty", "
+0000c950: 6669 7273 7420 7465 7874 2229 0a20 2020  first text").   
+0000c960: 2020 2020 2020 2020 2020 2020 203c 7465               <te
+0000c970: 7874 2d70 726f 7020 6e61 6d65 3d22 3a74  xt-prop name=":t
+0000c980: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
+0000c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9a0: 2020 3c74 6578 7420 656e 636f 6469 6e67    <text encoding
+0000c9b0: 3d22 7574 6638 2220 7065 726d 6973 7369  ="utf8" permissi
+0000c9c0: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
+0000c9d0: 7422 3e66 6972 7374 2074 6578 743c 2f74  t">first text</t
+0000c9e0: 6578 743e 0a20 2020 2020 2020 2020 2020  ext>.           
+0000c9f0: 2020 2020 203c 2f74 6578 742d 7072 6f70       </text-prop
+0000ca00: 3e0a 2020 2020 2020 2020 3e3e 3e20 6578  >.        >>> ex
+0000ca10: 6365 6c32 786d 6c2e 6d61 6b65 5f74 6578  cel2xml.make_tex
+0000ca20: 745f 7072 6f70 2822 3a74 6573 7470 726f  t_prop(":testpro
+0000ca30: 7065 7274 7922 2c20 6578 6365 6c32 786d  perty", excel2xm
+0000ca40: 6c2e 5072 6f70 6572 7479 456c 656d 656e  l.PropertyElemen
+0000ca50: 7428 2266 6972 7374 2074 6578 7422 2c20  t("first text", 
+0000ca60: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
+0000ca70: 702d 7265 7374 7269 6374 6564 222c 2065  p-restricted", e
+0000ca80: 6e63 6f64 696e 673d 2278 6d6c 2229 290a  ncoding="xml")).
+0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000caa0: 3c74 6578 742d 7072 6f70 206e 616d 653d  <text-prop name=
+0000cab0: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
+0000cac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cad0: 2020 2020 203c 7465 7874 2065 6e63 6f64       <text encod
+0000cae0: 696e 673d 2278 6d6c 2220 7065 726d 6973  ing="xml" permis
+0000caf0: 7369 6f6e 733d 2270 726f 702d 7265 7374  sions="prop-rest
+0000cb00: 7269 6374 6564 223e 6669 7273 7420 7465  ricted">first te
+0000cb10: 7874 3c2f 7465 7874 3e0a 2020 2020 2020  xt</text>.      
+0000cb20: 2020 2020 2020 2020 2020 3c2f 7465 7874            </text
+0000cb30: 2d70 726f 703e 0a20 2020 2020 2020 203e  -prop>.        >
+0000cb40: 3e3e 2065 7863 656c 3278 6d6c 2e6d 616b  >> excel2xml.mak
+0000cb50: 655f 7465 7874 5f70 726f 7028 223a 7465  e_text_prop(":te
+0000cb60: 7374 7072 6f70 6572 7479 222c 205b 2266  stproperty", ["f
+0000cb70: 6972 7374 2074 6578 7422 2c20 2273 6563  irst text", "sec
+0000cb80: 6f6e 6420 7465 7874 225d 290a 2020 2020  ond text"]).    
+0000cb90: 2020 2020 2020 2020 2020 2020 3c74 6578              <tex
+0000cba0: 742d 7072 6f70 206e 616d 653d 223a 7465  t-prop name=":te
+0000cbb0: 7374 7072 6f70 6572 7479 223e 0a20 2020  stproperty">.   
+0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbd0: 203c 7465 7874 2065 6e63 6f64 696e 673d   <text encoding=
+0000cbe0: 2275 7466 3822 2070 6572 6d69 7373 696f  "utf8" permissio
+0000cbf0: 6e73 3d22 7072 6f70 2d64 6566 6175 6c74  ns="prop-default
+0000cc00: 223e 6669 7273 7420 7465 7874 3c2f 7465  ">first text</te
+0000cc10: 7874 3e0a 2020 2020 2020 2020 2020 2020  xt>.            
+0000cc20: 2020 2020 2020 2020 3c74 6578 7420 656e          <text en
+0000cc30: 636f 6469 6e67 3d22 7574 6638 2220 7065  coding="utf8" pe
+0000cc40: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
+0000cc50: 6465 6661 756c 7422 3e73 6563 6f6e 6420  default">second 
+0000cc60: 7465 7874 3c2f 7465 7874 3e0a 2020 2020  text</text>.    
+0000cc70: 2020 2020 2020 2020 2020 2020 3c2f 7465              </te
+0000cc80: 7874 2d70 726f 703e 0a0a 2020 2020 5365  xt-prop>..    Se
+0000cc90: 6520 6874 7470 733a 2f2f 646f 6373 2e64  e https://docs.d
+0000cca0: 6173 6368 2e73 7769 7373 2f6c 6174 6573  asch.swiss/lates
+0000ccb0: 742f 4453 502d 544f 4f4c 532f 6669 6c65  t/DSP-TOOLS/file
+0000ccc0: 2d66 6f72 6d61 7473 2f78 6d6c 2d64 6174  -formats/xml-dat
+0000ccd0: 612d 6669 6c65 2f23 7465 7874 2d70 726f  a-file/#text-pro
+0000cce0: 700a 2020 2020 2222 220a 0a20 2020 2023  p.    """..    #
+0000ccf0: 2063 6865 636b 2074 6865 2069 6e70 7574   check the input
+0000cd00: 3a20 7072 6570 6172 6520 6120 6c69 7374  : prepare a list
+0000cd10: 2077 6974 6820 7661 6c69 6420 7661 6c75   with valid valu
+0000cd20: 6573 0a20 2020 2076 616c 7565 7320 3d20  es.    values = 
+0000cd30: 7072 6570 6172 655f 7661 6c75 6528 7661  prepare_value(va
+0000cd40: 6c75 6529 0a0a 2020 2020 2320 6368 6563  lue)..    # chec
+0000cd50: 6b20 7661 6c75 6520 7479 7065 0a20 2020  k value type.   
+0000cd60: 2066 6f72 2076 616c 2069 6e20 7661 6c75   for val in valu
+0000cd70: 6573 3a0a 2020 2020 2020 2020 6966 206e  es:.        if n
+0000cd80: 6f74 2069 7369 6e73 7461 6e63 6528 7661  ot isinstance(va
+0000cd90: 6c2e 7661 6c75 652c 2073 7472 2920 6f72  l.value, str) or
+0000cda0: 206e 6f74 2063 6865 636b 5f6e 6f74 6e61   not check_notna
+0000cdb0: 2876 616c 2e76 616c 7565 293a 0a20 2020  (val.value):.   
+0000cdc0: 2020 2020 2020 2020 206d 7367 203d 2028           msg = (
+0000cdd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cde0: 2066 2246 6169 6c65 6420 7661 6c69 6461   f"Failed valida
+0000cdf0: 7469 6f6e 2069 6e20 7265 736f 7572 6365  tion in resource
+0000ce00: 2027 7b63 616c 6c69 6e67 5f72 6573 6f75   '{calling_resou
+0000ce10: 7263 657d 272c 2070 726f 7065 7274 7920  rce}', property 
+0000ce20: 277b 6e61 6d65 7d27 3a20 220a 2020 2020  '{name}': ".    
+0000ce30: 2020 2020 2020 2020 2020 2020 6622 277b              f"'{
+0000ce40: 7661 6c2e 7661 6c75 657d 2720 6973 2070  val.value}' is p
+0000ce50: 726f 6261 626c 7920 6e6f 7420 6120 7573  robably not a us
+0000ce60: 6162 6c65 2073 7472 696e 672e 220a 2020  able string.".  
+0000ce70: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000ce80: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
+0000ce90: 2e77 6172 6e28 4473 7054 6f6f 6c73 5573  .warn(DspToolsUs
+0000cea0: 6572 5761 726e 696e 6728 6d73 6729 290a  erWarning(msg)).
+0000ceb0: 0a20 2020 2023 206d 616b 6520 786d 6c20  .    # make xml 
+0000cec0: 7374 7275 6374 7572 6520 6f66 2074 6865  structure of the
+0000ced0: 2076 616c 6964 2076 616c 7565 730a 2020   valid values.  
+0000cee0: 2020 7072 6f70 5f20 3d20 6574 7265 652e    prop_ = etree.
+0000cef0: 456c 656d 656e 7428 0a20 2020 2020 2020  Element(.       
+0000cf00: 2022 7b25 737d 7465 7874 2d70 726f 7022   "{%s}text-prop"
+0000cf10: 2025 2078 6d6c 5f6e 616d 6573 7061 6365   % xml_namespace
+0000cf20: 5f6d 6170 5b4e 6f6e 655d 2c0a 2020 2020  _map[None],.    
+0000cf30: 2020 2020 6e61 6d65 3d6e 616d 652c 0a20      name=name,. 
+0000cf40: 2020 2020 2020 206e 736d 6170 3d78 6d6c         nsmap=xml
+0000cf50: 5f6e 616d 6573 7061 6365 5f6d 6170 2c0a  _namespace_map,.
+0000cf60: 2020 2020 290a 2020 2020 666f 7220 7661      ).    for va
+0000cf70: 6c20 696e 2076 616c 7565 733a 0a20 2020  l in values:.   
+0000cf80: 2020 2020 206b 7761 7267 7320 3d20 7b22       kwargs = {"
+0000cf90: 7065 726d 6973 7369 6f6e 7322 3a20 7661  permissions": va
+0000cfa0: 6c2e 7065 726d 6973 7369 6f6e 737d 0a20  l.permissions}. 
+0000cfb0: 2020 2020 2020 2069 6620 6368 6563 6b5f         if check_
+0000cfc0: 6e6f 746e 6128 7661 6c2e 636f 6d6d 656e  notna(val.commen
+0000cfd0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+0000cfe0: 6b77 6172 6773 5b22 636f 6d6d 656e 7422  kwargs["comment"
+0000cff0: 5d20 3d20 7661 6c2e 636f 6d6d 656e 740a  ] = val.comment.
+0000d000: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
+0000d010: 656e 636f 6469 6e67 225d 203d 2076 616c  encoding"] = val
+0000d020: 2e65 6e63 6f64 696e 6720 6966 2063 6865  .encoding if che
+0000d030: 636b 5f6e 6f74 6e61 2876 616c 2e65 6e63  ck_notna(val.enc
+0000d040: 6f64 696e 6729 2065 6c73 6520 2275 7466  oding) else "utf
+0000d050: 3822 0a20 2020 2020 2020 2076 616c 7565  8".        value
+0000d060: 5f20 3d20 6574 7265 652e 456c 656d 656e  _ = etree.Elemen
+0000d070: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
+0000d080: 7b25 737d 7465 7874 2220 2520 786d 6c5f  {%s}text" % xml_
+0000d090: 6e61 6d65 7370 6163 655f 6d61 705b 4e6f  namespace_map[No
+0000d0a0: 6e65 5d2c 0a20 2020 2020 2020 2020 2020  ne],.           
+0000d0b0: 202a 2a6b 7761 7267 732c 2020 2320 7479   **kwargs,  # ty
+0000d0c0: 7065 3a20 6967 6e6f 7265 5b61 7267 2d74  pe: ignore[arg-t
+0000d0d0: 7970 655d 0a20 2020 2020 2020 2020 2020  ype].           
+0000d0e0: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
+0000d0f0: 7061 6365 5f6d 6170 2c0a 2020 2020 2020  pace_map,.      
+0000d100: 2020 290a 2020 2020 2020 2020 6966 206b    ).        if k
+0000d110: 7761 7267 735b 2265 6e63 6f64 696e 6722  wargs["encoding"
+0000d120: 5d20 3d3d 2022 7574 6638 223a 0a20 2020  ] == "utf8":.   
+0000d130: 2020 2020 2020 2020 2023 2077 7269 7465           # write
+0000d140: 2074 6865 2074 6578 7420 696e 746f 2074   the text into t
+0000d150: 6865 2074 6167 2c20 7769 7468 6f75 7420  he tag, without 
+0000d160: 7661 6c69 6461 7469 6f6e 0a20 2020 2020  validation.     
+0000d170: 2020 2020 2020 2076 616c 7565 5f2e 7465         value_.te
+0000d180: 7874 203d 2073 7472 2876 616c 2e76 616c  xt = str(val.val
+0000d190: 7565 290a 2020 2020 2020 2020 656c 7365  ue).        else
+0000d1a0: 3a0a 2020 2020 2020 2020 2020 2020 6573  :.            es
+0000d1b0: 6361 7065 645f 7465 7874 203d 205f 6573  caped_text = _es
+0000d1c0: 6361 7065 5f72 6573 6572 7665 645f 6368  cape_reserved_ch
+0000d1d0: 6172 7328 7374 7228 7661 6c2e 7661 6c75  ars(str(val.valu
+0000d1e0: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
+0000d1f0: 2320 656e 666f 7263 6520 7468 6174 2074  # enforce that t
+0000d200: 6865 2074 6578 7420 6973 2077 656c 6c2d  he text is well-
+0000d210: 666f 726d 6564 2058 4d4c 3a20 7365 7269  formed XML: seri
+0000d220: 616c 697a 6520 7461 6720 2e2e 2e0a 2020  alize tag ....  
+0000d230: 2020 2020 2020 2020 2020 7365 7269 616c            serial
+0000d240: 697a 6564 203d 2065 7472 6565 2e74 6f73  ized = etree.tos
+0000d250: 7472 696e 6728 7661 6c75 655f 2c20 656e  tring(value_, en
+0000d260: 636f 6469 6e67 3d22 756e 6963 6f64 6522  coding="unicode"
+0000d270: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+0000d280: 2e2e 2e20 696e 7365 7274 2074 6578 7420  ... insert text 
+0000d290: 6174 2074 6865 2076 6572 7920 656e 6420  at the very end 
+0000d2a0: 6f66 2074 6865 2073 7472 696e 672c 2061  of the string, a
+0000d2b0: 6e64 2061 6464 2065 6e64 696e 6720 7461  nd add ending ta
+0000d2c0: 6720 746f 2074 6865 2070 7265 7669 6f75  g to the previou
+0000d2d0: 736c 7920 7369 6e67 6c65 203c 7465 7874  sly single <text
+0000d2e0: 2f3e 2074 6167 202e 2e2e 0a20 2020 2020  /> tag ....     
+0000d2f0: 2020 2020 2020 2073 6572 6961 6c69 7a65         serialize
+0000d300: 6420 3d20 7265 6765 782e 7375 6228 7222  d = regex.sub(r"
+0000d310: 2f3e 2422 2c20 6622 3e7b 6573 6361 7065  />$", f">{escape
+0000d320: 645f 7465 7874 7d3c 2f74 6578 743e 222c  d_text}</text>",
+0000d330: 2073 6572 6961 6c69 7a65 6429 0a20 2020   serialized).   
+0000d340: 2020 2020 2020 2020 2023 202e 2e2e 2074           # ... t
+0000d350: 7279 2074 6f20 7061 7273 6520 6974 2061  ry to parse it a
+0000d360: 6761 696e 0a20 2020 2020 2020 2020 2020  gain.           
+0000d370: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000d380: 2020 2020 2020 7661 6c75 655f 203d 2065        value_ = e
+0000d390: 7472 6565 2e66 726f 6d73 7472 696e 6728  tree.fromstring(
+0000d3a0: 7365 7269 616c 697a 6564 290a 2020 2020  serialized).    
+0000d3b0: 2020 2020 2020 2020 6578 6365 7074 2065          except e
+0000d3c0: 7472 6565 2e58 4d4c 5379 6e74 6178 4572  tree.XMLSyntaxEr
+0000d3d0: 726f 7220 6173 2065 7272 3a0a 2020 2020  ror as err:.    
+0000d3e0: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
+0000d3f0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0000d400: 2020 2020 2020 2020 2254 6865 2058 4d4c          "The XML
+0000d410: 2074 6167 7320 636f 6e74 6169 6e65 6420   tags contained 
+0000d420: 696e 2061 2072 6963 6874 6578 7420 7072  in a richtext pr
+0000d430: 6f70 6572 7479 2028 656e 636f 6469 6e67  operty (encoding
+0000d440: 3d78 6d6c 2920 6d75 7374 2062 6520 7765  =xml) must be we
+0000d450: 6c6c 2d66 6f72 6d65 642e 2022 0a20 2020  ll-formed. ".   
+0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d470: 2022 5468 6520 7370 6563 6961 6c20 6368   "The special ch
+0000d480: 6172 6163 7465 7273 203c 2c20 3e20 616e  aracters <, > an
+0000d490: 6420 2620 6172 6520 6f6e 6c79 2061 6c6c  d & are only all
+0000d4a0: 6f77 6564 2074 6f20 636f 6e73 7472 7563  owed to construc
+0000d4b0: 7420 6120 7461 672e 2022 0a20 2020 2020  t a tag. ".     
+0000d4c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000d4d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d4e0: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
+0000d4f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d500: 2020 2020 2020 6d73 6720 2b3d 2066 2254        msg += f"T
+0000d510: 6865 2065 7272 6f72 206f 6363 7572 7265  he error occurre
+0000d520: 6420 696e 2072 6573 6f75 7263 6520 7b63  d in resource {c
+0000d530: 616c 6c69 6e67 5f72 6573 6f75 7263 657d  alling_resource}
+0000d540: 2c20 7072 6f70 6572 7479 207b 6e61 6d65  , property {name
+0000d550: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+0000d560: 2020 206d 7367 202b 3d20 6622 5c6e 4f72     msg += f"\nOr
+0000d570: 6967 696e 616c 2065 7272 6f72 206d 6573  iginal error mes
+0000d580: 7361 6765 3a20 7b65 7272 2e6d 7367 7d22  sage: {err.msg}"
+0000d590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d5a0: 206d 7367 202b 3d20 6622 5c6e 4576 656e   msg += f"\nEven
+0000d5b0: 7475 616c 206c 696e 652f 636f 6c75 6d6e  tual line/column
+0000d5c0: 206e 756d 6265 7273 2061 7265 2072 656c   numbers are rel
+0000d5d0: 6174 6976 6520 746f 2074 6869 7320 7365  ative to this se
+0000d5e0: 7269 616c 697a 6564 2074 6578 743a 207b  rialized text: {
+0000d5f0: 7365 7269 616c 697a 6564 7d22 0a20 2020  serialized}".   
+0000d600: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+0000d610: 7365 2042 6173 6545 7272 6f72 286d 7367  se BaseError(msg
+0000d620: 2920 6672 6f6d 204e 6f6e 650a 2020 2020  ) from None.    
+0000d630: 2020 2020 7072 6f70 5f2e 6170 7065 6e64      prop_.append
+0000d640: 2876 616c 7565 5f29 0a0a 2020 2020 7265  (value_)..    re
+0000d650: 7475 726e 2070 726f 705f 0a0a 0a64 6566  turn prop_...def
+0000d660: 205f 6573 6361 7065 5f72 6573 6572 7665   _escape_reserve
+0000d670: 645f 6368 6172 7328 7465 7874 3a20 7374  d_chars(text: st
+0000d680: 7229 202d 3e20 7374 723a 0a20 2020 2022  r) -> str:.    "
+0000d690: 2222 0a20 2020 2046 726f 6d20 7269 6368  "".    From rich
+0000d6a0: 7465 7874 2073 7472 696e 6773 2028 656e  text strings (en
+0000d6b0: 636f 6469 6e67 3d22 786d 6c22 292c 2065  coding="xml"), e
+0000d6c0: 7363 6170 6520 7468 6520 7265 7365 7276  scape the reserv
+0000d6d0: 6564 2063 6861 7261 6374 6572 7320 3c2c  ed characters <,
+0000d6e0: 203e 2061 6e64 2026 2c0a 2020 2020 6275   > and &,.    bu
+0000d6f0: 7420 6f6e 6c79 2069 6620 7468 6579 2061  t only if they a
+0000d700: 7265 206e 6f74 2070 6172 7420 6f66 2061  re not part of a
+0000d710: 2073 7461 6e64 6172 6420 7374 616e 646f   standard stando
+0000d720: 6666 2074 6167 206f 7220 6573 6361 7065  ff tag or escape
+0000d730: 2073 6571 7565 6e63 652e 0a20 2020 2054   sequence..    T
+0000d740: 6865 2073 7461 6e64 6172 6420 7374 616e  he standard stan
+0000d750: 646f 6666 2074 6167 7320 616c 6c6f 7765  doff tags allowe
+0000d760: 6420 6279 2044 5350 2d41 5049 2061 7265  d by DSP-API are
+0000d770: 2064 6f63 756d 656e 7465 6420 6865 7265   documented here
+0000d780: 3a0a 2020 2020 6874 7470 733a 2f2f 646f  :.    https://do
+0000d790: 6373 2e64 6173 6368 2e73 7769 7373 2f32  cs.dasch.swiss/2
+0000d7a0: 3032 332e 3132 2e30 312f 4453 502d 4150  023.12.01/DSP-AP
+0000d7b0: 492f 3033 2d65 6e64 706f 696e 7473 2f61  I/03-endpoints/a
+0000d7c0: 7069 2d76 322f 7465 7874 2f73 7461 6e64  pi-v2/text/stand
+0000d7d0: 6172 642d 7374 616e 646f 6666 2f0a 0a20  ard-standoff/.. 
+0000d7e0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000d7f0: 2074 6578 743a 2074 6865 2072 6963 6874   text: the richt
+0000d800: 6578 7420 7374 7269 6e67 2074 6f20 6265  ext string to be
+0000d810: 2065 7363 6170 6564 0a0a 2020 2020 5265   escaped..    Re
+0000d820: 7475 726e 733a 0a20 2020 2020 2020 2074  turns:.        t
+0000d830: 6865 2065 7363 6170 6564 2072 6963 6874  he escaped richt
+0000d840: 6578 7420 7374 7269 6e67 0a20 2020 2022  ext string.    "
+0000d850: 2222 0a20 2020 2061 6c6c 6f77 6564 5f74  "".    allowed_t
+0000d860: 6167 7320 3d20 5b0a 2020 2020 2020 2020  ags = [.        
+0000d870: 2261 2820 5b5e 3e5d 2b29 3f22 2c20 2023  "a( [^>]+)?",  #
+0000d880: 203c 613e 2069 7320 7468 6520 6f6e 6c79   <a> is the only
+0000d890: 2074 6167 2074 6861 7420 6361 6e20 6861   tag that can ha
+0000d8a0: 7665 2061 7474 7269 6275 7465 730a 2020  ve attributes.  
+0000d8b0: 2020 2020 2020 2270 222c 0a20 2020 2020        "p",.     
+0000d8c0: 2020 2022 656d 222c 0a20 2020 2020 2020     "em",.       
+0000d8d0: 2022 7374 726f 6e67 222c 0a20 2020 2020   "strong",.     
+0000d8e0: 2020 2022 7522 2c0a 2020 2020 2020 2020     "u",.        
+0000d8f0: 2273 7562 222c 0a20 2020 2020 2020 2022  "sub",.        "
+0000d900: 7375 7022 2c0a 2020 2020 2020 2020 2273  sup",.        "s
+0000d910: 7472 696b 6522 2c0a 2020 2020 2020 2020  trike",.        
+0000d920: 2268 3122 2c0a 2020 2020 2020 2020 226f  "h1",.        "o
+0000d930: 6c22 2c0a 2020 2020 2020 2020 2275 6c22  l",.        "ul"
+0000d940: 2c0a 2020 2020 2020 2020 226c 6922 2c0a  ,.        "li",.
+0000d950: 2020 2020 2020 2020 2274 626f 6479 222c          "tbody",
+0000d960: 0a20 2020 2020 2020 2022 7461 626c 6522  .        "table"
+0000d970: 2c0a 2020 2020 2020 2020 2274 7222 2c0a  ,.        "tr",.
+0000d980: 2020 2020 2020 2020 2274 6422 2c0a 2020          "td",.  
+0000d990: 2020 2020 2020 2262 7222 2c0a 2020 2020        "br",.    
+0000d9a0: 2020 2020 2268 7222 2c0a 2020 2020 2020      "hr",.      
+0000d9b0: 2020 2270 7265 222c 0a20 2020 2020 2020    "pre",.       
+0000d9c0: 2022 6369 7465 222c 0a20 2020 2020 2020   "cite",.       
+0000d9d0: 2022 626c 6f63 6b71 756f 7465 222c 0a20   "blockquote",. 
+0000d9e0: 2020 2020 2020 2022 636f 6465 222c 0a20         "code",. 
+0000d9f0: 2020 205d 0a20 2020 2061 6c6c 6f77 6564     ].    allowed
+0000da00: 5f74 6167 735f 7265 6765 7820 3d20 227c  _tags_regex = "|
+0000da10: 222e 6a6f 696e 2861 6c6c 6f77 6564 5f74  ".join(allowed_t
+0000da20: 6167 7329 0a20 2020 206c 6f6f 6b61 6865  ags).    lookahe
+0000da30: 6164 203d 2072 6622 283f 212f 3f28 7b61  ad = rf"(?!/?({a
+0000da40: 6c6c 6f77 6564 5f74 6167 735f 7265 6765  llowed_tags_rege
+0000da50: 787d 292f 3f3e 2922 0a20 2020 2069 6c6c  x})/?>)".    ill
+0000da60: 6567 616c 5f6c 7420 3d20 7266 223c 7b6c  egal_lt = rf"<{l
+0000da70: 6f6f 6b61 6865 6164 7d22 0a20 2020 206c  ookahead}".    l
+0000da80: 6f6f 6b62 6568 696e 6420 3d20 7266 2228  ookbehind = rf"(
+0000da90: 3f3c 213c 2f3f 287b 616c 6c6f 7765 645f  ?<!</?({allowed_
+0000daa0: 7461 6773 5f72 6567 6578 7d29 2f3f 2922  tags_regex})/?)"
+0000dab0: 0a20 2020 2069 6c6c 6567 616c 5f67 7420  .    illegal_gt 
+0000dac0: 3d20 7266 227b 6c6f 6f6b 6265 6869 6e64  = rf"{lookbehind
+0000dad0: 7d3e 220a 2020 2020 696c 6c65 6761 6c5f  }>".    illegal_
+0000dae0: 616d 7020 3d20 7222 2628 3f21 5b23 612d  amp = r"&(?![#a-
+0000daf0: 7a41 2d5a 302d 395d 2b3b 2922 0a20 2020  zA-Z0-9]+;)".   
+0000db00: 2074 6578 7420 3d20 7265 6765 782e 7375   text = regex.su
+0000db10: 6228 696c 6c65 6761 6c5f 6c74 2c20 2226  b(illegal_lt, "&
+0000db20: 6c74 3b22 2c20 7465 7874 290a 2020 2020  lt;", text).    
+0000db30: 7465 7874 203d 2072 6567 6578 2e73 7562  text = regex.sub
+0000db40: 2869 6c6c 6567 616c 5f67 742c 2022 2667  (illegal_gt, "&g
+0000db50: 743b 222c 2074 6578 7429 0a20 2020 2074  t;", text).    t
+0000db60: 6578 7420 3d20 7265 6765 782e 7375 6228  ext = regex.sub(
+0000db70: 696c 6c65 6761 6c5f 616d 702c 2022 2661  illegal_amp, "&a
+0000db80: 6d70 3b22 2c20 7465 7874 290a 2020 2020  mp;", text).    
+0000db90: 7265 7475 726e 2074 6578 740a 0a0a 6465  return text...de
+0000dba0: 6620 6d61 6b65 5f74 696d 655f 7072 6f70  f make_time_prop
+0000dbb0: 280a 2020 2020 6e61 6d65 3a20 7374 722c  (.    name: str,
+0000dbc0: 0a20 2020 2076 616c 7565 3a20 556e 696f  .    value: Unio
+0000dbd0: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
+0000dbe0: 742c 2073 7472 2c20 4974 6572 6162 6c65  t, str, Iterable
+0000dbf0: 5b55 6e69 6f6e 5b50 726f 7065 7274 7945  [Union[PropertyE
+0000dc00: 6c65 6d65 6e74 2c20 7374 725d 5d5d 2c0a  lement, str]]],.
+0000dc10: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
+0000dc20: 7572 6365 3a20 7374 7220 3d20 2222 2c0a  urce: str = "",.
+0000dc30: 2920 2d3e 2065 7472 6565 2e5f 456c 656d  ) -> etree._Elem
+0000dc40: 656e 743a 0a20 2020 2022 2222 0a20 2020  ent:.    """.   
+0000dc50: 204d 616b 6520 6120 3c74 696d 652d 7072   Make a <time-pr
+0000dc60: 6f70 3e20 6672 6f6d 206f 6e65 206f 7220  op> from one or 
+0000dc70: 6d6f 7265 2064 6174 6574 696d 6520 7661  more datetime va
+0000dc80: 6c75 6573 206f 6620 7468 6520 666f 726d  lues of the form
+0000dc90: 2022 3230 3039 2d31 302d 3130 5431 323a   "2009-10-10T12:
+0000dca0: 3030 3a30 302d 3035 3a30 3022 2e20 5468  00:00-05:00". Th
+0000dcb0: 6520 7469 6d65 2873 2920 6361 6e20 6265  e time(s) can be
+0000dcc0: 0a20 2020 2070 726f 7669 6465 6420 6173  .    provided as
+0000dcd0: 2073 7472 696e 6720 6f72 2061 7320 5072   string or as Pr
+0000dce0: 6f70 6572 7479 456c 656d 656e 7420 7769  opertyElement wi
+0000dcf0: 7468 2061 2073 7472 696e 6720 696e 7369  th a string insi
+0000dd00: 6465 2e20 4966 2070 726f 7669 6465 6420  de. If provided 
+0000dd10: 6173 2073 7472 696e 672c 2074 6865 2070  as string, the p
+0000dd20: 6572 6d69 7373 696f 6e73 2064 6566 6175  ermissions defau
+0000dd30: 6c74 2074 6f0a 2020 2020 2270 726f 702d  lt to.    "prop-
+0000dd40: 6465 6661 756c 7422 2e0a 0a20 2020 2041  default"...    A
+0000dd50: 7267 733a 0a20 2020 2020 2020 206e 616d  rgs:.        nam
+0000dd60: 653a 2074 6865 206e 616d 6520 6f66 2074  e: the name of t
+0000dd70: 6869 7320 7072 6f70 6572 7479 2061 7320  his property as 
+0000dd80: 6465 6669 6e65 6420 696e 2074 6865 206f  defined in the o
+0000dd90: 6e74 6f0a 2020 2020 2020 2020 7661 6c75  nto.        valu
+0000dda0: 653a 206f 6e65 206f 7220 6d6f 7265 2044  e: one or more D
+0000ddb0: 5350 2074 696d 6573 2c20 6173 2073 7472  SP times, as str
+0000ddc0: 696e 672f 5072 6f70 6572 7479 456c 656d  ing/PropertyElem
+0000ddd0: 656e 742c 206f 7220 6173 2069 7465 7261  ent, or as itera
+0000dde0: 626c 6520 6f66 2073 7472 696e 6773 2f50  ble of strings/P
+0000ddf0: 726f 7065 7274 7945 6c65 6d65 6e74 730a  ropertyElements.
+0000de00: 2020 2020 2020 2020 6361 6c6c 696e 675f          calling_
+0000de10: 7265 736f 7572 6365 3a20 7468 6520 6e61  resource: the na
+0000de20: 6d65 206f 6620 7468 6520 7061 7265 6e74  me of the parent
+0000de30: 2072 6573 6f75 7263 6520 2866 6f72 2062   resource (for b
+0000de40: 6574 7465 7220 6572 726f 7220 6d65 7373  etter error mess
+0000de50: 6167 6573 290a 0a20 2020 2057 6172 6e73  ages)..    Warns
+0000de60: 3a0a 2020 2020 2020 2020 4966 206f 6e65  :.        If one
+0000de70: 206f 6620 7468 6520 7661 6c75 6573 2069   of the values i
+0000de80: 7320 6e6f 7420 6120 7661 6c69 6420 4453  s not a valid DS
+0000de90: 5020 7469 6d65 2073 7472 696e 670a 0a20  P time string.. 
+0000dea0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000deb0: 2020 2020 616e 2065 7472 6565 2e5f 456c      an etree._El
+0000dec0: 656d 656e 7420 7468 6174 2063 616e 2062  ement that can b
+0000ded0: 6520 6170 7065 6e64 6564 2074 6f20 7468  e appended to th
+0000dee0: 6520 7061 7265 6e74 2072 6573 6f75 7263  e parent resourc
+0000def0: 6520 7769 7468 2072 6573 6f75 7263 652e  e with resource.
+0000df00: 6170 7065 6e64 286d 616b 655f 2a5f 7072  append(make_*_pr
+0000df10: 6f70 282e 2e2e 2929 0a0a 2020 2020 4578  op(...))..    Ex
+0000df20: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
+0000df30: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
+0000df40: 6b65 5f74 696d 655f 7072 6f70 2822 3a74  ke_time_prop(":t
+0000df50: 6573 7470 726f 7065 7274 7922 2c20 2232  estproperty", "2
+0000df60: 3030 392d 3130 2d31 3054 3132 3a30 303a  009-10-10T12:00:
+0000df70: 3030 2d30 353a 3030 2229 0a20 2020 2020  00-05:00").     
+0000df80: 2020 2020 2020 2020 2020 203c 7469 6d65             <time
+0000df90: 2d70 726f 7020 6e61 6d65 3d22 3a74 6573  -prop name=":tes
+0000dfa0: 7470 726f 7065 7274 7922 3e0a 2020 2020  tproperty">.    
+0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfc0: 3c74 696d 6520 7065 726d 6973 7369 6f6e  <time permission
+0000dfd0: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
+0000dfe0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000dff0: 2020 2020 2020 2020 2020 3230 3039 2d31            2009-1
+0000e000: 302d 3130 5431 323a 3030 3a30 302d 3035  0-10T12:00:00-05
+0000e010: 3a30 300a 2020 2020 2020 2020 2020 2020  :00.            
+0000e020: 2020 2020 2020 2020 3c2f 7469 6d65 3e0a          </time>.
 0000e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e040: 2032 3030 392d 3130 2d31 3054 3132 3a30   2009-10-10T12:0
-0000e050: 303a 3030 2d30 353a 3030 0a20 2020 2020  0:00-05:00.     
-0000e060: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e070: 2f74 696d 653e 0a20 2020 2020 2020 2020  /time>.         
-0000e080: 2020 2020 2020 203c 2f74 696d 652d 7072         </time-pr
-0000e090: 6f70 3e0a 2020 2020 2020 2020 3e3e 3e20  op>.        >>> 
-0000e0a0: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f74  excel2xml.make_t
-0000e0b0: 696d 655f 7072 6f70 2822 3a74 6573 7470  ime_prop(":testp
-0000e0c0: 726f 7065 7274 7922 2c20 6578 6365 6c32  roperty", excel2
-0000e0d0: 786d 6c2e 5072 6f70 6572 7479 456c 656d  xml.PropertyElem
-0000e0e0: 656e 7428 2232 3030 392d 3130 2d31 3054  ent("2009-10-10T
-0000e0f0: 3132 3a30 303a 3030 2d30 353a 3030 222c  12:00:00-05:00",
-0000e100: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
-0000e110: 6f70 2d72 6573 7472 6963 7465 6422 2c20  op-restricted", 
-0000e120: 636f 6d6d 656e 743d 2265 7861 6d70 6c65  comment="example
-0000e130: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
-0000e140: 2020 2020 3c74 696d 652d 7072 6f70 206e      <time-prop n
-0000e150: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
-0000e160: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
-0000e170: 2020 2020 2020 2020 203c 7469 6d65 2070           <time p
-0000e180: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
-0000e190: 2d72 6573 7472 6963 7465 6422 2063 6f6d  -restricted" com
-0000e1a0: 6d65 6e74 3d22 6578 616d 706c 6522 3e0a  ment="example">.
-0000e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1c0: 2020 2020 2020 2020 3230 3039 2d31 302d          2009-10-
-0000e1d0: 3130 5431 323a 3030 3a30 302d 3035 3a30  10T12:00:00-05:0
-0000e1e0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-0000e1f0: 2020 2020 2020 3c2f 7469 6d65 3e0a 2020        </time>.  
-0000e200: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0000e210: 7469 6d65 2d70 726f 703e 0a20 2020 2020  time-prop>.     
-0000e220: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
-0000e230: 2e6d 616b 655f 7469 6d65 5f70 726f 7028  .make_time_prop(
-0000e240: 223a 7465 7374 7072 6f70 6572 7479 222c  ":testproperty",
-0000e250: 205b 2232 3030 392d 3130 2d31 3054 3132   ["2009-10-10T12
-0000e260: 3a30 303a 3030 2d30 353a 3030 222c 2022  :00:00-05:00", "
-0000e270: 3139 3031 2d30 312d 3031 5430 313a 3030  1901-01-01T01:00
-0000e280: 3a30 302d 3030 3a30 3022 5d29 0a20 2020  :00-00:00"]).   
-0000e290: 2020 2020 2020 2020 2020 2020 203c 7469               <ti
-0000e2a0: 6d65 2d70 726f 7020 6e61 6d65 3d22 3a74  me-prop name=":t
-0000e2b0: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
-0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2d0: 2020 3c74 696d 6520 7065 726d 6973 7369    <time permissi
-0000e2e0: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-0000e2f0: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
-0000e300: 2020 2020 2020 2020 2020 2020 3230 3039              2009
-0000e310: 2d31 302d 3130 5431 323a 3030 3a30 302d  -10-10T12:00:00-
-0000e320: 3035 3a30 300a 2020 2020 2020 2020 2020  05:00.          
-0000e330: 2020 2020 2020 2020 2020 3c2f 7469 6d65            </time
-0000e340: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000e350: 2020 2020 2020 3c74 696d 6520 7065 726d        <time perm
-0000e360: 6973 7369 6f6e 733d 2270 726f 702d 6465  issions="prop-de
-0000e370: 6661 756c 7422 3e0a 2020 2020 2020 2020  fault">.        
+0000e040: 3c2f 7469 6d65 2d70 726f 703e 0a20 2020  </time-prop>.   
+0000e050: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
+0000e060: 6d6c 2e6d 616b 655f 7469 6d65 5f70 726f  ml.make_time_pro
+0000e070: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
+0000e080: 222c 2065 7863 656c 3278 6d6c 2e50 726f  ", excel2xml.Pro
+0000e090: 7065 7274 7945 6c65 6d65 6e74 2822 3230  pertyElement("20
+0000e0a0: 3039 2d31 302d 3130 5431 323a 3030 3a30  09-10-10T12:00:0
+0000e0b0: 302d 3035 3a30 3022 2c20 7065 726d 6973  0-05:00", permis
+0000e0c0: 7369 6f6e 733d 2270 726f 702d 7265 7374  sions="prop-rest
+0000e0d0: 7269 6374 6564 222c 2063 6f6d 6d65 6e74  ricted", comment
+0000e0e0: 3d22 6578 616d 706c 6522 2929 0a20 2020  ="example")).   
+0000e0f0: 2020 2020 2020 2020 2020 2020 203c 7469               <ti
+0000e100: 6d65 2d70 726f 7020 6e61 6d65 3d22 3a74  me-prop name=":t
+0000e110: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
+0000e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e130: 2020 3c74 696d 6520 7065 726d 6973 7369    <time permissi
+0000e140: 6f6e 733d 2270 726f 702d 7265 7374 7269  ons="prop-restri
+0000e150: 6374 6564 2220 636f 6d6d 656e 743d 2265  cted" comment="e
+0000e160: 7861 6d70 6c65 223e 0a20 2020 2020 2020  xample">.       
+0000e170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e180: 2032 3030 392d 3130 2d31 3054 3132 3a30   2009-10-10T12:0
+0000e190: 303a 3030 2d30 353a 3030 0a20 2020 2020  0:00-05:00.     
+0000e1a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000e1b0: 2f74 696d 653e 0a20 2020 2020 2020 2020  /time>.         
+0000e1c0: 2020 2020 2020 203c 2f74 696d 652d 7072         </time-pr
+0000e1d0: 6f70 3e0a 2020 2020 2020 2020 3e3e 3e20  op>.        >>> 
+0000e1e0: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f74  excel2xml.make_t
+0000e1f0: 696d 655f 7072 6f70 2822 3a74 6573 7470  ime_prop(":testp
+0000e200: 726f 7065 7274 7922 2c20 5b22 3230 3039  roperty", ["2009
+0000e210: 2d31 302d 3130 5431 323a 3030 3a30 302d  -10-10T12:00:00-
+0000e220: 3035 3a30 3022 2c20 2231 3930 312d 3031  05:00", "1901-01
+0000e230: 2d30 3154 3031 3a30 303a 3030 2d30 303a  -01T01:00:00-00:
+0000e240: 3030 225d 290a 2020 2020 2020 2020 2020  00"]).          
+0000e250: 2020 2020 2020 3c74 696d 652d 7072 6f70        <time-prop
+0000e260: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
+0000e270: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
+0000e280: 2020 2020 2020 2020 2020 203c 7469 6d65             <time
+0000e290: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
+0000e2a0: 6f70 2d64 6566 6175 6c74 223e 0a20 2020  op-default">.   
+0000e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2c0: 2020 2020 2032 3030 392d 3130 2d31 3054       2009-10-10T
+0000e2d0: 3132 3a30 303a 3030 2d30 353a 3030 0a20  12:00:00-05:00. 
+0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2f0: 2020 203c 2f74 696d 653e 0a20 2020 2020     </time>.     
+0000e300: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000e310: 7469 6d65 2070 6572 6d69 7373 696f 6e73  time permissions
+0000e320: 3d22 7072 6f70 2d64 6566 6175 6c74 223e  ="prop-default">
+0000e330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e340: 2020 2020 2020 2020 2031 3930 312d 3031           1901-01
+0000e350: 2d30 3154 3031 3a30 303a 3030 2d30 303a  -01T01:00:00-00:
+0000e360: 3030 320a 2020 2020 2020 2020 2020 2020  002.            
+0000e370: 2020 2020 2020 2020 3c2f 7469 6d65 3e0a          </time>.
 0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e390: 3139 3031 2d30 312d 3031 5430 313a 3030  1901-01-01T01:00
-0000e3a0: 3a30 302d 3030 3a30 3032 0a20 2020 2020  :00-00:002.     
-0000e3b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e3c0: 2f74 696d 653e 0a20 2020 2020 2020 2020  /time>.         
-0000e3d0: 2020 2020 2020 203c 2f74 696d 652d 7072         </time-pr
-0000e3e0: 6f70 3e0a 0a20 2020 2053 6565 2068 7474  op>..    See htt
-0000e3f0: 7073 3a2f 2f64 6f63 732e 6461 7363 682e  ps://docs.dasch.
-0000e400: 7377 6973 732f 6c61 7465 7374 2f44 5350  swiss/latest/DSP
-0000e410: 2d54 4f4f 4c53 2f66 696c 652d 666f 726d  -TOOLS/file-form
-0000e420: 6174 732f 786d 6c2d 6461 7461 2d66 696c  ats/xml-data-fil
-0000e430: 652f 2374 696d 652d 7072 6f70 0a20 2020  e/#time-prop.   
-0000e440: 2022 2222 0a0a 2020 2020 2320 6368 6563   """..    # chec
-0000e450: 6b20 7468 6520 696e 7075 743a 2070 7265  k the input: pre
-0000e460: 7061 7265 2061 206c 6973 7420 7769 7468  pare a list with
-0000e470: 2076 616c 6964 2076 616c 7565 730a 2020   valid values.  
-0000e480: 2020 7661 6c75 6573 203d 2070 7265 7061    values = prepa
-0000e490: 7265 5f76 616c 7565 2876 616c 7565 290a  re_value(value).
-0000e4a0: 0a20 2020 2023 2063 6865 636b 2076 616c  .    # check val
-0000e4b0: 7565 2074 7970 650a 2020 2020 7661 6c69  ue type.    vali
-0000e4c0: 6461 7469 6f6e 5f72 6567 6578 203d 2072  dation_regex = r
-0000e4d0: 225e 5c64 7b34 7d2d 5b30 2d31 5d5c 642d  "^\d{4}-[0-1]\d-
-0000e4e0: 5b30 2d33 5d5c 6454 5b30 2d32 5d5c 643a  [0-3]\dT[0-2]\d:
-0000e4f0: 5b30 2d35 5d5c 643a 5b30 2d35 5d5c 6428  [0-5]\d:[0-5]\d(
-0000e500: 2e5c 647b 312c 3132 7d29 3f28 5a7c 5b2b  .\d{1,12})?(Z|[+
-0000e510: 2d5d 5b30 2d31 5d5c 643a 5b30 2d35 5d5c  -][0-1]\d:[0-5]\
-0000e520: 6429 2422 0a20 2020 2066 6f72 2076 616c  d)$".    for val
-0000e530: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
-0000e540: 2020 2020 6966 206e 6f74 2072 6567 6578      if not regex
-0000e550: 2e73 6561 7263 6828 7661 6c69 6461 7469  .search(validati
-0000e560: 6f6e 5f72 6567 6578 2c20 7374 7228 7661  on_regex, str(va
-0000e570: 6c2e 7661 6c75 6529 293a 0a20 2020 2020  l.value)):.     
-0000e580: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
-0000e590: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000e5a0: 2246 6169 6c65 6420 7661 6c69 6461 7469  "Failed validati
-0000e5b0: 6f6e 2069 6e20 7265 736f 7572 6365 2027  on in resource '
-0000e5c0: 7b63 616c 6c69 6e67 5f72 6573 6f75 7263  {calling_resourc
-0000e5d0: 657d 272c 2070 726f 7065 7274 7920 277b  e}', property '{
-0000e5e0: 6e61 6d65 7d27 3a20 220a 2020 2020 2020  name}': ".      
-0000e5f0: 2020 2020 2020 2020 2020 6622 277b 7661            f"'{va
-0000e600: 6c2e 7661 6c75 657d 2720 6973 206e 6f74  l.value}' is not
-0000e610: 2061 2076 616c 6964 2044 5350 2074 696d   a valid DSP tim
-0000e620: 652e 220a 2020 2020 2020 2020 2020 2020  e.".            
-0000e630: 290a 2020 2020 2020 2020 2020 2020 7761  ).            wa
-0000e640: 726e 696e 6773 2e77 6172 6e28 4473 7054  rnings.warn(DspT
-0000e650: 6f6f 6c73 5573 6572 5761 726e 696e 6728  oolsUserWarning(
-0000e660: 6d73 6729 290a 0a20 2020 2023 206d 616b  msg))..    # mak
-0000e670: 6520 786d 6c20 7374 7275 6374 7572 6520  e xml structure 
-0000e680: 6f66 2074 6865 2076 616c 6964 2076 616c  of the valid val
-0000e690: 7565 730a 2020 2020 7072 6f70 5f20 3d20  ues.    prop_ = 
-0000e6a0: 6574 7265 652e 456c 656d 656e 7428 0a20  etree.Element(. 
-0000e6b0: 2020 2020 2020 2022 7b25 737d 7469 6d65         "{%s}time
-0000e6c0: 2d70 726f 7022 2025 2078 6d6c 5f6e 616d  -prop" % xml_nam
-0000e6d0: 6573 7061 6365 5f6d 6170 5b4e 6f6e 655d  espace_map[None]
-0000e6e0: 2c0a 2020 2020 2020 2020 6e61 6d65 3d6e  ,.        name=n
-0000e6f0: 616d 652c 0a20 2020 2020 2020 206e 736d  ame,.        nsm
-0000e700: 6170 3d78 6d6c 5f6e 616d 6573 7061 6365  ap=xml_namespace
-0000e710: 5f6d 6170 2c0a 2020 2020 290a 2020 2020  _map,.    ).    
-0000e720: 666f 7220 7661 6c20 696e 2076 616c 7565  for val in value
-0000e730: 733a 0a20 2020 2020 2020 206b 7761 7267  s:.        kwarg
-0000e740: 7320 3d20 7b22 7065 726d 6973 7369 6f6e  s = {"permission
-0000e750: 7322 3a20 7661 6c2e 7065 726d 6973 7369  s": val.permissi
-0000e760: 6f6e 737d 0a20 2020 2020 2020 2069 6620  ons}.        if 
-0000e770: 7661 6c2e 636f 6d6d 656e 7420 616e 6420  val.comment and 
-0000e780: 6368 6563 6b5f 6e6f 746e 6128 7661 6c2e  check_notna(val.
-0000e790: 636f 6d6d 656e 7429 3a0a 2020 2020 2020  comment):.      
-0000e7a0: 2020 2020 2020 6b77 6172 6773 5b22 636f        kwargs["co
-0000e7b0: 6d6d 656e 7422 5d20 3d20 7661 6c2e 636f  mment"] = val.co
-0000e7c0: 6d6d 656e 740a 2020 2020 2020 2020 7661  mment.        va
-0000e7d0: 6c75 655f 203d 2065 7472 6565 2e45 6c65  lue_ = etree.Ele
-0000e7e0: 6d65 6e74 280a 2020 2020 2020 2020 2020  ment(.          
-0000e7f0: 2020 227b 2573 7d74 696d 6522 2025 2078    "{%s}time" % x
-0000e800: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
-0000e810: 5b4e 6f6e 655d 2c0a 2020 2020 2020 2020  [None],.        
-0000e820: 2020 2020 2a2a 6b77 6172 6773 2c20 2023      **kwargs,  #
-0000e830: 2074 7970 653a 2069 676e 6f72 655b 6172   type: ignore[ar
-0000e840: 672d 7479 7065 5d0a 2020 2020 2020 2020  g-type].        
-0000e850: 2020 2020 6e73 6d61 703d 786d 6c5f 6e61      nsmap=xml_na
-0000e860: 6d65 7370 6163 655f 6d61 702c 0a20 2020  mespace_map,.   
-0000e870: 2020 2020 2029 0a20 2020 2020 2020 2076       ).        v
-0000e880: 616c 7565 5f2e 7465 7874 203d 2073 7472  alue_.text = str
-0000e890: 2876 616c 2e76 616c 7565 290a 2020 2020  (val.value).    
-0000e8a0: 2020 2020 7072 6f70 5f2e 6170 7065 6e64      prop_.append
-0000e8b0: 2876 616c 7565 5f29 0a0a 2020 2020 7265  (value_)..    re
-0000e8c0: 7475 726e 2070 726f 705f 0a0a 0a64 6566  turn prop_...def
-0000e8d0: 206d 616b 655f 7572 695f 7072 6f70 280a   make_uri_prop(.
-0000e8e0: 2020 2020 6e61 6d65 3a20 7374 722c 0a20      name: str,. 
-0000e8f0: 2020 2076 616c 7565 3a20 556e 696f 6e5b     value: Union[
-0000e900: 5072 6f70 6572 7479 456c 656d 656e 742c  PropertyElement,
-0000e910: 2073 7472 2c20 4974 6572 6162 6c65 5b55   str, Iterable[U
-0000e920: 6e69 6f6e 5b50 726f 7065 7274 7945 6c65  nion[PropertyEle
-0000e930: 6d65 6e74 2c20 7374 725d 5d5d 2c0a 2020  ment, str]]],.  
-0000e940: 2020 6361 6c6c 696e 675f 7265 736f 7572    calling_resour
-0000e950: 6365 3a20 7374 7220 3d20 2222 2c0a 2920  ce: str = "",.) 
-0000e960: 2d3e 2065 7472 6565 2e5f 456c 656d 656e  -> etree._Elemen
-0000e970: 743a 0a20 2020 2022 2222 0a20 2020 204d  t:.    """.    M
-0000e980: 616b 6520 616e 203c 7572 692d 7072 6f70  ake an <uri-prop
-0000e990: 3e20 6672 6f6d 206f 6e65 206f 7220 6d6f  > from one or mo
-0000e9a0: 7265 2055 5249 732e 2054 6865 2055 5249  re URIs. The URI
-0000e9b0: 2873 2920 6361 6e20 6265 2070 726f 7669  (s) can be provi
-0000e9c0: 6465 6420 6173 2073 7472 696e 6720 6f72  ded as string or
-0000e9d0: 2061 7320 5072 6f70 6572 7479 456c 656d   as PropertyElem
-0000e9e0: 656e 7420 7769 7468 2061 2073 7472 696e  ent with a strin
-0000e9f0: 670a 2020 2020 696e 7369 6465 2e20 4966  g.    inside. If
-0000ea00: 2070 726f 7669 6465 6420 6173 2073 7472   provided as str
-0000ea10: 696e 672c 2074 6865 2070 6572 6d69 7373  ing, the permiss
-0000ea20: 696f 6e73 2064 6566 6175 6c74 2074 6f20  ions default to 
-0000ea30: 2270 726f 702d 6465 6661 756c 7422 2e0a  "prop-default"..
-0000ea40: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-0000ea50: 2020 206e 616d 653a 2074 6865 206e 616d     name: the nam
-0000ea60: 6520 6f66 2074 6869 7320 7072 6f70 6572  e of this proper
-0000ea70: 7479 2061 7320 6465 6669 6e65 6420 696e  ty as defined in
-0000ea80: 2074 6865 206f 6e74 6f0a 2020 2020 2020   the onto.      
-0000ea90: 2020 7661 6c75 653a 206f 6e65 206f 7220    value: one or 
-0000eaa0: 6d6f 7265 2055 5249 732c 2061 7320 7374  more URIs, as st
-0000eab0: 7269 6e67 2f50 726f 7065 7274 7945 6c65  ring/PropertyEle
-0000eac0: 6d65 6e74 2c20 6f72 2061 7320 6974 6572  ment, or as iter
-0000ead0: 6162 6c65 206f 6620 7374 7269 6e67 732f  able of strings/
-0000eae0: 5072 6f70 6572 7479 456c 656d 656e 7473  PropertyElements
-0000eaf0: 0a20 2020 2020 2020 2063 616c 6c69 6e67  .        calling
-0000eb00: 5f72 6573 6f75 7263 653a 2074 6865 206e  _resource: the n
-0000eb10: 616d 6520 6f66 2074 6865 2070 6172 656e  ame of the paren
-0000eb20: 7420 7265 736f 7572 6365 2028 666f 7220  t resource (for 
-0000eb30: 6265 7474 6572 2065 7272 6f72 206d 6573  better error mes
-0000eb40: 7361 6765 7329 0a0a 2020 2020 5761 726e  sages)..    Warn
-0000eb50: 733a 0a20 2020 2020 2020 2049 6620 6f6e  s:.        If on
-0000eb60: 6520 6f66 2074 6865 2076 616c 7565 7320  e of the values 
-0000eb70: 6973 206e 6f74 2061 2076 616c 6964 2055  is not a valid U
-0000eb80: 5249 0a0a 2020 2020 5265 7475 726e 733a  RI..    Returns:
-0000eb90: 0a20 2020 2020 2020 2061 6e20 6574 7265  .        an etre
-0000eba0: 652e 5f45 6c65 6d65 6e74 2074 6861 7420  e._Element that 
-0000ebb0: 6361 6e20 6265 2061 7070 656e 6465 6420  can be appended 
-0000ebc0: 746f 2074 6865 2070 6172 656e 7420 7265  to the parent re
-0000ebd0: 736f 7572 6365 2077 6974 6820 7265 736f  source with reso
-0000ebe0: 7572 6365 2e61 7070 656e 6428 6d61 6b65  urce.append(make
-0000ebf0: 5f2a 5f70 726f 7028 2e2e 2e29 290a 0a20  _*_prop(...)).. 
-0000ec00: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
-0000ec10: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
-0000ec20: 6d6c 2e6d 616b 655f 7572 695f 7072 6f70  ml.make_uri_prop
-0000ec30: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
-0000ec40: 2c20 2277 7777 2e74 6573 742e 636f 6d22  , "www.test.com"
-0000ec50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ec60: 2020 3c75 7269 2d70 726f 7020 6e61 6d65    <uri-prop name
-0000ec70: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
+0000e390: 3c2f 7469 6d65 2d70 726f 703e 0a0a 2020  </time-prop>..  
+0000e3a0: 2020 5365 6520 6874 7470 733a 2f2f 646f    See https://do
+0000e3b0: 6373 2e64 6173 6368 2e73 7769 7373 2f6c  cs.dasch.swiss/l
+0000e3c0: 6174 6573 742f 4453 502d 544f 4f4c 532f  atest/DSP-TOOLS/
+0000e3d0: 6669 6c65 2d66 6f72 6d61 7473 2f78 6d6c  file-formats/xml
+0000e3e0: 2d64 6174 612d 6669 6c65 2f23 7469 6d65  -data-file/#time
+0000e3f0: 2d70 726f 700a 2020 2020 2222 220a 0a20  -prop.    """.. 
+0000e400: 2020 2023 2063 6865 636b 2074 6865 2069     # check the i
+0000e410: 6e70 7574 3a20 7072 6570 6172 6520 6120  nput: prepare a 
+0000e420: 6c69 7374 2077 6974 6820 7661 6c69 6420  list with valid 
+0000e430: 7661 6c75 6573 0a20 2020 2076 616c 7565  values.    value
+0000e440: 7320 3d20 7072 6570 6172 655f 7661 6c75  s = prepare_valu
+0000e450: 6528 7661 6c75 6529 0a0a 2020 2020 2320  e(value)..    # 
+0000e460: 6368 6563 6b20 7661 6c75 6520 7479 7065  check value type
+0000e470: 0a20 2020 2076 616c 6964 6174 696f 6e5f  .    validation_
+0000e480: 7265 6765 7820 3d20 7222 5e5c 647b 347d  regex = r"^\d{4}
+0000e490: 2d5b 302d 315d 5c64 2d5b 302d 335d 5c64  -[0-1]\d-[0-3]\d
+0000e4a0: 545b 302d 325d 5c64 3a5b 302d 355d 5c64  T[0-2]\d:[0-5]\d
+0000e4b0: 3a5b 302d 355d 5c64 282e 5c64 7b31 2c31  :[0-5]\d(.\d{1,1
+0000e4c0: 327d 293f 285a 7c5b 2b2d 5d5b 302d 315d  2})?(Z|[+-][0-1]
+0000e4d0: 5c64 3a5b 302d 355d 5c64 2924 220a 2020  \d:[0-5]\d)$".  
+0000e4e0: 2020 666f 7220 7661 6c20 696e 2076 616c    for val in val
+0000e4f0: 7565 733a 0a20 2020 2020 2020 2069 6620  ues:.        if 
+0000e500: 6e6f 7420 7265 6765 782e 7365 6172 6368  not regex.search
+0000e510: 2876 616c 6964 6174 696f 6e5f 7265 6765  (validation_rege
+0000e520: 782c 2073 7472 2876 616c 2e76 616c 7565  x, str(val.value
+0000e530: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000e540: 6d73 6720 3d20 280a 2020 2020 2020 2020  msg = (.        
+0000e550: 2020 2020 2020 2020 6622 4661 696c 6564          f"Failed
+0000e560: 2076 616c 6964 6174 696f 6e20 696e 2072   validation in r
+0000e570: 6573 6f75 7263 6520 277b 6361 6c6c 696e  esource '{callin
+0000e580: 675f 7265 736f 7572 6365 7d27 2c20 7072  g_resource}', pr
+0000e590: 6f70 6572 7479 2027 7b6e 616d 657d 273a  operty '{name}':
+0000e5a0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000e5b0: 2020 2066 2227 7b76 616c 2e76 616c 7565     f"'{val.value
+0000e5c0: 7d27 2069 7320 6e6f 7420 6120 7661 6c69  }' is not a vali
+0000e5d0: 6420 4453 5020 7469 6d65 2e22 0a20 2020  d DSP time.".   
+0000e5e0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000e5f0: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+0000e600: 7761 726e 2844 7370 546f 6f6c 7355 7365  warn(DspToolsUse
+0000e610: 7257 6172 6e69 6e67 286d 7367 2929 0a0a  rWarning(msg))..
+0000e620: 2020 2020 2320 6d61 6b65 2078 6d6c 2073      # make xml s
+0000e630: 7472 7563 7475 7265 206f 6620 7468 6520  tructure of the 
+0000e640: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
+0000e650: 2070 726f 705f 203d 2065 7472 6565 2e45   prop_ = etree.E
+0000e660: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
+0000e670: 227b 2573 7d74 696d 652d 7072 6f70 2220  "{%s}time-prop" 
+0000e680: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
+0000e690: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
+0000e6a0: 2020 206e 616d 653d 6e61 6d65 2c0a 2020     name=name,.  
+0000e6b0: 2020 2020 2020 6e73 6d61 703d 786d 6c5f        nsmap=xml_
+0000e6c0: 6e61 6d65 7370 6163 655f 6d61 702c 0a20  namespace_map,. 
+0000e6d0: 2020 2029 0a20 2020 2066 6f72 2076 616c     ).    for val
+0000e6e0: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
+0000e6f0: 2020 2020 6b77 6172 6773 203d 207b 2270      kwargs = {"p
+0000e700: 6572 6d69 7373 696f 6e73 223a 2076 616c  ermissions": val
+0000e710: 2e70 6572 6d69 7373 696f 6e73 7d0a 2020  .permissions}.  
+0000e720: 2020 2020 2020 6966 2076 616c 2e63 6f6d        if val.com
+0000e730: 6d65 6e74 2061 6e64 2063 6865 636b 5f6e  ment and check_n
+0000e740: 6f74 6e61 2876 616c 2e63 6f6d 6d65 6e74  otna(val.comment
+0000e750: 293a 0a20 2020 2020 2020 2020 2020 206b  ):.            k
+0000e760: 7761 7267 735b 2263 6f6d 6d65 6e74 225d  wargs["comment"]
+0000e770: 203d 2076 616c 2e63 6f6d 6d65 6e74 0a20   = val.comment. 
+0000e780: 2020 2020 2020 2076 616c 7565 5f20 3d20         value_ = 
+0000e790: 6574 7265 652e 456c 656d 656e 7428 0a20  etree.Element(. 
+0000e7a0: 2020 2020 2020 2020 2020 2022 7b25 737d             "{%s}
+0000e7b0: 7469 6d65 2220 2520 786d 6c5f 6e61 6d65  time" % xml_name
+0000e7c0: 7370 6163 655f 6d61 705b 4e6f 6e65 5d2c  space_map[None],
+0000e7d0: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+0000e7e0: 7761 7267 732c 2020 2320 7479 7065 3a20  wargs,  # type: 
+0000e7f0: 6967 6e6f 7265 5b61 7267 2d74 7970 655d  ignore[arg-type]
+0000e800: 0a20 2020 2020 2020 2020 2020 206e 736d  .            nsm
+0000e810: 6170 3d78 6d6c 5f6e 616d 6573 7061 6365  ap=xml_namespace
+0000e820: 5f6d 6170 2c0a 2020 2020 2020 2020 290a  _map,.        ).
+0000e830: 2020 2020 2020 2020 7661 6c75 655f 2e74          value_.t
+0000e840: 6578 7420 3d20 7374 7228 7661 6c2e 7661  ext = str(val.va
+0000e850: 6c75 6529 0a20 2020 2020 2020 2070 726f  lue).        pro
+0000e860: 705f 2e61 7070 656e 6428 7661 6c75 655f  p_.append(value_
+0000e870: 290a 0a20 2020 2072 6574 7572 6e20 7072  )..    return pr
+0000e880: 6f70 5f0a 0a0a 6465 6620 6d61 6b65 5f75  op_...def make_u
+0000e890: 7269 5f70 726f 7028 0a20 2020 206e 616d  ri_prop(.    nam
+0000e8a0: 653a 2073 7472 2c0a 2020 2020 7661 6c75  e: str,.    valu
+0000e8b0: 653a 2055 6e69 6f6e 5b50 726f 7065 7274  e: Union[Propert
+0000e8c0: 7945 6c65 6d65 6e74 2c20 7374 722c 2049  yElement, str, I
+0000e8d0: 7465 7261 626c 655b 556e 696f 6e5b 5072  terable[Union[Pr
+0000e8e0: 6f70 6572 7479 456c 656d 656e 742c 2073  opertyElement, s
+0000e8f0: 7472 5d5d 5d2c 0a20 2020 2063 616c 6c69  tr]]],.    calli
+0000e900: 6e67 5f72 6573 6f75 7263 653a 2073 7472  ng_resource: str
+0000e910: 203d 2022 222c 0a29 202d 3e20 6574 7265   = "",.) -> etre
+0000e920: 652e 5f45 6c65 6d65 6e74 3a0a 2020 2020  e._Element:.    
+0000e930: 2222 220a 2020 2020 4d61 6b65 2061 6e20  """.    Make an 
+0000e940: 3c75 7269 2d70 726f 703e 2066 726f 6d20  <uri-prop> from 
+0000e950: 6f6e 6520 6f72 206d 6f72 6520 5552 4973  one or more URIs
+0000e960: 2e20 5468 6520 5552 4928 7329 2063 616e  . The URI(s) can
+0000e970: 2062 6520 7072 6f76 6964 6564 2061 7320   be provided as 
+0000e980: 7374 7269 6e67 206f 7220 6173 2050 726f  string or as Pro
+0000e990: 7065 7274 7945 6c65 6d65 6e74 2077 6974  pertyElement wit
+0000e9a0: 6820 6120 7374 7269 6e67 0a20 2020 2069  h a string.    i
+0000e9b0: 6e73 6964 652e 2049 6620 7072 6f76 6964  nside. If provid
+0000e9c0: 6564 2061 7320 7374 7269 6e67 2c20 7468  ed as string, th
+0000e9d0: 6520 7065 726d 6973 7369 6f6e 7320 6465  e permissions de
+0000e9e0: 6661 756c 7420 746f 2022 7072 6f70 2d64  fault to "prop-d
+0000e9f0: 6566 6175 6c74 222e 0a0a 2020 2020 4172  efault"...    Ar
+0000ea00: 6773 3a0a 2020 2020 2020 2020 6e61 6d65  gs:.        name
+0000ea10: 3a20 7468 6520 6e61 6d65 206f 6620 7468  : the name of th
+0000ea20: 6973 2070 726f 7065 7274 7920 6173 2064  is property as d
+0000ea30: 6566 696e 6564 2069 6e20 7468 6520 6f6e  efined in the on
+0000ea40: 746f 0a20 2020 2020 2020 2076 616c 7565  to.        value
+0000ea50: 3a20 6f6e 6520 6f72 206d 6f72 6520 5552  : one or more UR
+0000ea60: 4973 2c20 6173 2073 7472 696e 672f 5072  Is, as string/Pr
+0000ea70: 6f70 6572 7479 456c 656d 656e 742c 206f  opertyElement, o
+0000ea80: 7220 6173 2069 7465 7261 626c 6520 6f66  r as iterable of
+0000ea90: 2073 7472 696e 6773 2f50 726f 7065 7274   strings/Propert
+0000eaa0: 7945 6c65 6d65 6e74 730a 2020 2020 2020  yElements.      
+0000eab0: 2020 6361 6c6c 696e 675f 7265 736f 7572    calling_resour
+0000eac0: 6365 3a20 7468 6520 6e61 6d65 206f 6620  ce: the name of 
+0000ead0: 7468 6520 7061 7265 6e74 2072 6573 6f75  the parent resou
+0000eae0: 7263 6520 2866 6f72 2062 6574 7465 7220  rce (for better 
+0000eaf0: 6572 726f 7220 6d65 7373 6167 6573 290a  error messages).
+0000eb00: 0a20 2020 2057 6172 6e73 3a0a 2020 2020  .    Warns:.    
+0000eb10: 2020 2020 4966 206f 6e65 206f 6620 7468      If one of th
+0000eb20: 6520 7661 6c75 6573 2069 7320 6e6f 7420  e values is not 
+0000eb30: 6120 7661 6c69 6420 5552 490a 0a20 2020  a valid URI..   
+0000eb40: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000eb50: 2020 616e 2065 7472 6565 2e5f 456c 656d    an etree._Elem
+0000eb60: 656e 7420 7468 6174 2063 616e 2062 6520  ent that can be 
+0000eb70: 6170 7065 6e64 6564 2074 6f20 7468 6520  appended to the 
+0000eb80: 7061 7265 6e74 2072 6573 6f75 7263 6520  parent resource 
+0000eb90: 7769 7468 2072 6573 6f75 7263 652e 6170  with resource.ap
+0000eba0: 7065 6e64 286d 616b 655f 2a5f 7072 6f70  pend(make_*_prop
+0000ebb0: 282e 2e2e 2929 0a0a 2020 2020 4578 616d  (...))..    Exam
+0000ebc0: 706c 6573 3a0a 2020 2020 2020 2020 3e3e  ples:.        >>
+0000ebd0: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
+0000ebe0: 5f75 7269 5f70 726f 7028 223a 7465 7374  _uri_prop(":test
+0000ebf0: 7072 6f70 6572 7479 222c 2022 7777 772e  property", "www.
+0000ec00: 7465 7374 2e63 6f6d 2229 0a20 2020 2020  test.com").     
+0000ec10: 2020 2020 2020 2020 2020 203c 7572 692d             <uri-
+0000ec20: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
+0000ec30: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
+0000ec40: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000ec50: 7572 6920 7065 726d 6973 7369 6f6e 733d  uri permissions=
+0000ec60: 2270 726f 702d 6465 6661 756c 7422 3e77  "prop-default">w
+0000ec70: 7777 2e74 6573 742e 636f 6d3c 2f75 7269  ww.test.com</uri
 0000ec80: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000ec90: 2020 2020 2020 3c75 7269 2070 6572 6d69        <uri permi
-0000eca0: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
-0000ecb0: 6175 6c74 223e 7777 772e 7465 7374 2e63  ault">www.test.c
-0000ecc0: 6f6d 3c2f 7572 693e 0a20 2020 2020 2020  om</uri>.       
-0000ecd0: 2020 2020 2020 2020 203c 2f75 7269 2d70           </uri-p
-0000ece0: 726f 703e 0a20 2020 2020 2020 203e 3e3e  rop>.        >>>
-0000ecf0: 2065 7863 656c 3278 6d6c 2e6d 616b 655f   excel2xml.make_
-0000ed00: 7572 695f 7072 6f70 2822 3a74 6573 7470  uri_prop(":testp
-0000ed10: 726f 7065 7274 7922 2c20 6578 6365 6c32  roperty", excel2
-0000ed20: 786d 6c2e 5072 6f70 6572 7479 456c 656d  xml.PropertyElem
-0000ed30: 656e 7428 2277 7777 2e74 6573 742e 636f  ent("www.test.co
-0000ed40: 6d22 2c20 7065 726d 6973 7369 6f6e 733d  m", permissions=
-0000ed50: 2270 726f 702d 7265 7374 7269 6374 6564  "prop-restricted
-0000ed60: 222c 2063 6f6d 6d65 6e74 3d22 6578 616d  ", comment="exam
-0000ed70: 706c 6522 2929 0a20 2020 2020 2020 2020  ple")).         
-0000ed80: 2020 2020 2020 203c 7572 692d 7072 6f70         <uri-prop
-0000ed90: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
-0000eda0: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
-0000edb0: 2020 2020 2020 2020 2020 203c 7572 6920             <uri 
-0000edc0: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
-0000edd0: 702d 7265 7374 7269 6374 6564 2220 636f  p-restricted" co
-0000ede0: 6d6d 656e 743d 2265 7861 6d70 6c65 223e  mment="example">
-0000edf0: 7777 772e 7465 7374 2e63 6f6d 3c2f 7572  www.test.com</ur
-0000ee00: 693e 0a20 2020 2020 2020 2020 2020 2020  i>.             
-0000ee10: 2020 203c 2f75 7269 2d70 726f 703e 0a20     </uri-prop>. 
-0000ee20: 2020 2020 2020 203e 3e3e 2065 7863 656c         >>> excel
-0000ee30: 3278 6d6c 2e6d 616b 655f 7572 695f 7072  2xml.make_uri_pr
-0000ee40: 6f70 2822 3a74 6573 7470 726f 7065 7274  op(":testpropert
-0000ee50: 7922 2c20 5b22 7777 772e 312e 636f 6d22  y", ["www.1.com"
-0000ee60: 2c20 2277 7777 2e32 2e63 6f6d 225d 290a  , "www.2.com"]).
-0000ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee80: 3c75 7269 2d70 726f 7020 6e61 6d65 3d22  <uri-prop name="
-0000ee90: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
+0000ec90: 2020 3c2f 7572 692d 7072 6f70 3e0a 2020    </uri-prop>.  
+0000eca0: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+0000ecb0: 786d 6c2e 6d61 6b65 5f75 7269 5f70 726f  xml.make_uri_pro
+0000ecc0: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
+0000ecd0: 222c 2065 7863 656c 3278 6d6c 2e50 726f  ", excel2xml.Pro
+0000ece0: 7065 7274 7945 6c65 6d65 6e74 2822 7777  pertyElement("ww
+0000ecf0: 772e 7465 7374 2e63 6f6d 222c 2070 6572  w.test.com", per
+0000ed00: 6d69 7373 696f 6e73 3d22 7072 6f70 2d72  missions="prop-r
+0000ed10: 6573 7472 6963 7465 6422 2c20 636f 6d6d  estricted", comm
+0000ed20: 656e 743d 2265 7861 6d70 6c65 2229 290a  ent="example")).
+0000ed30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed40: 3c75 7269 2d70 726f 7020 6e61 6d65 3d22  <uri-prop name="
+0000ed50: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
+0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed70: 2020 2020 3c75 7269 2070 6572 6d69 7373      <uri permiss
+0000ed80: 696f 6e73 3d22 7072 6f70 2d72 6573 7472  ions="prop-restr
+0000ed90: 6963 7465 6422 2063 6f6d 6d65 6e74 3d22  icted" comment="
+0000eda0: 6578 616d 706c 6522 3e77 7777 2e74 6573  example">www.tes
+0000edb0: 742e 636f 6d3c 2f75 7269 3e0a 2020 2020  t.com</uri>.    
+0000edc0: 2020 2020 2020 2020 2020 2020 3c2f 7572              </ur
+0000edd0: 692d 7072 6f70 3e0a 2020 2020 2020 2020  i-prop>.        
+0000ede0: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
+0000edf0: 6b65 5f75 7269 5f70 726f 7028 223a 7465  ke_uri_prop(":te
+0000ee00: 7374 7072 6f70 6572 7479 222c 205b 2277  stproperty", ["w
+0000ee10: 7777 2e31 2e63 6f6d 222c 2022 7777 772e  ww.1.com", "www.
+0000ee20: 322e 636f 6d22 5d29 0a20 2020 2020 2020  2.com"]).       
+0000ee30: 2020 2020 2020 2020 203c 7572 692d 7072           <uri-pr
+0000ee40: 6f70 206e 616d 653d 223a 7465 7374 7072  op name=":testpr
+0000ee50: 6f70 6572 7479 223e 0a20 2020 2020 2020  operty">.       
+0000ee60: 2020 2020 2020 2020 2020 2020 203c 7572               <ur
+0000ee70: 6920 7065 726d 6973 7369 6f6e 733d 2270  i permissions="p
+0000ee80: 726f 702d 6465 6661 756c 7422 3e77 7777  rop-default">www
+0000ee90: 2e31 2e63 6f6d 3c2f 7572 693e 0a20 2020  .1.com</uri>.   
 0000eea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eeb0: 2020 2020 3c75 7269 2070 6572 6d69 7373      <uri permiss
-0000eec0: 696f 6e73 3d22 7072 6f70 2d64 6566 6175  ions="prop-defau
-0000eed0: 6c74 223e 7777 772e 312e 636f 6d3c 2f75  lt">www.1.com</u
-0000eee0: 7269 3e0a 2020 2020 2020 2020 2020 2020  ri>.            
-0000eef0: 2020 2020 2020 2020 3c75 7269 2070 6572          <uri per
-0000ef00: 6d69 7373 696f 6e73 3d22 7072 6f70 2d64  missions="prop-d
-0000ef10: 6566 6175 6c74 223e 7777 772e 322e 636f  efault">www.2.co
-0000ef20: 6d3c 2f75 7269 3e0a 2020 2020 2020 2020  m</uri>.        
-0000ef30: 2020 2020 2020 2020 3c2f 7572 692d 7072          </uri-pr
-0000ef40: 6f70 3e0a 0a20 2020 2053 6565 2068 7474  op>..    See htt
-0000ef50: 7073 3a2f 2f64 6f63 732e 6461 7363 682e  ps://docs.dasch.
-0000ef60: 7377 6973 732f 6c61 7465 7374 2f44 5350  swiss/latest/DSP
-0000ef70: 2d54 4f4f 4c53 2f66 696c 652d 666f 726d  -TOOLS/file-form
-0000ef80: 6174 732f 786d 6c2d 6461 7461 2d66 696c  ats/xml-data-fil
-0000ef90: 652f 2375 7269 2d70 726f 700a 2020 2020  e/#uri-prop.    
-0000efa0: 2222 220a 0a20 2020 2023 2063 6865 636b  """..    # check
-0000efb0: 2074 6865 2069 6e70 7574 3a20 7072 6570   the input: prep
-0000efc0: 6172 6520 6120 6c69 7374 2077 6974 6820  are a list with 
-0000efd0: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
-0000efe0: 2076 616c 7565 7320 3d20 7072 6570 6172   values = prepar
-0000eff0: 655f 7661 6c75 6528 7661 6c75 6529 0a0a  e_value(value)..
-0000f000: 2020 2020 2320 6368 6563 6b20 7661 6c75      # check valu
-0000f010: 6520 7479 7065 0a20 2020 2066 6f72 2076  e type.    for v
-0000f020: 616c 2069 6e20 7661 6c75 6573 3a0a 2020  al in values:.  
-0000f030: 2020 2020 2020 6966 206e 6f74 2069 735f        if not is_
-0000f040: 7572 6928 7374 7228 7661 6c2e 7661 6c75  uri(str(val.valu
-0000f050: 6529 293a 0a20 2020 2020 2020 2020 2020  e)):.           
-0000f060: 206d 7367 203d 2028 0a20 2020 2020 2020   msg = (.       
-0000f070: 2020 2020 2020 2020 2066 2246 6169 6c65           f"Faile
-0000f080: 6420 7661 6c69 6461 7469 6f6e 2069 6e20  d validation in 
-0000f090: 7265 736f 7572 6365 2027 7b63 616c 6c69  resource '{calli
-0000f0a0: 6e67 5f72 6573 6f75 7263 657d 272c 2070  ng_resource}', p
-0000f0b0: 726f 7065 7274 7920 277b 6e61 6d65 7d27  roperty '{name}'
-0000f0c0: 3a20 220a 2020 2020 2020 2020 2020 2020  : ".            
-0000f0d0: 2020 2020 6622 277b 7661 6c2e 7661 6c75      f"'{val.valu
-0000f0e0: 657d 2720 6973 206e 6f74 2061 2076 616c  e}' is not a val
-0000f0f0: 6964 2055 5249 2e22 0a20 2020 2020 2020  id URI.".       
-0000f100: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000f110: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
-0000f120: 2844 7370 546f 6f6c 7355 7365 7257 6172  (DspToolsUserWar
-0000f130: 6e69 6e67 286d 7367 2929 0a0a 2020 2020  ning(msg))..    
-0000f140: 2320 6d61 6b65 2078 6d6c 2073 7472 7563  # make xml struc
-0000f150: 7475 7265 206f 6620 7468 6520 7661 6c69  ture of the vali
-0000f160: 6420 7661 6c75 6573 0a20 2020 2070 726f  d values.    pro
-0000f170: 705f 203d 2065 7472 6565 2e45 6c65 6d65  p_ = etree.Eleme
-0000f180: 6e74 280a 2020 2020 2020 2020 227b 2573  nt(.        "{%s
-0000f190: 7d75 7269 2d70 726f 7022 2025 2078 6d6c  }uri-prop" % xml
-0000f1a0: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
-0000f1b0: 6f6e 655d 2c0a 2020 2020 2020 2020 6e61  one],.        na
-0000f1c0: 6d65 3d6e 616d 652c 0a20 2020 2020 2020  me=name,.       
-0000f1d0: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
-0000f1e0: 7061 6365 5f6d 6170 2c0a 2020 2020 290a  pace_map,.    ).
-0000f1f0: 2020 2020 666f 7220 7661 6c20 696e 2076      for val in v
-0000f200: 616c 7565 733a 0a20 2020 2020 2020 206b  alues:.        k
-0000f210: 7761 7267 7320 3d20 7b22 7065 726d 6973  wargs = {"permis
-0000f220: 7369 6f6e 7322 3a20 7661 6c2e 7065 726d  sions": val.perm
-0000f230: 6973 7369 6f6e 737d 0a20 2020 2020 2020  issions}.       
-0000f240: 2069 6620 7661 6c2e 636f 6d6d 656e 7420   if val.comment 
-0000f250: 616e 6420 6368 6563 6b5f 6e6f 746e 6128  and check_notna(
-0000f260: 7661 6c2e 636f 6d6d 656e 7429 3a0a 2020  val.comment):.  
-0000f270: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
-0000f280: 5b22 636f 6d6d 656e 7422 5d20 3d20 7661  ["comment"] = va
-0000f290: 6c2e 636f 6d6d 656e 740a 2020 2020 2020  l.comment.      
-0000f2a0: 2020 7661 6c75 655f 203d 2065 7472 6565    value_ = etree
-0000f2b0: 2e45 6c65 6d65 6e74 280a 2020 2020 2020  .Element(.      
-0000f2c0: 2020 2020 2020 227b 2573 7d75 7269 2220        "{%s}uri" 
-0000f2d0: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
-0000f2e0: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
-0000f2f0: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
-0000f300: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-0000f310: 5b61 7267 2d74 7970 655d 0a20 2020 2020  [arg-type].     
-0000f320: 2020 2020 2020 206e 736d 6170 3d78 6d6c         nsmap=xml
-0000f330: 5f6e 616d 6573 7061 6365 5f6d 6170 2c0a  _namespace_map,.
-0000f340: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000f350: 2020 7661 6c75 655f 2e74 6578 7420 3d20    value_.text = 
-0000f360: 7374 7228 7661 6c2e 7661 6c75 6529 0a20  str(val.value). 
-0000f370: 2020 2020 2020 2070 726f 705f 2e61 7070         prop_.app
-0000f380: 656e 6428 7661 6c75 655f 290a 0a20 2020  end(value_)..   
-0000f390: 2072 6574 7572 6e20 7072 6f70 5f0a 0a0a   return prop_...
-0000f3a0: 6465 6620 6d61 6b65 5f72 6567 696f 6e28  def make_region(
-0000f3b0: 2020 2320 6e6f 7161 3a20 4434 3137 2028    # noqa: D417 (
-0000f3c0: 756e 646f 6375 6d65 6e74 6564 2d70 6172  undocumented-par
-0000f3d0: 616d 290a 2020 2020 6c61 6265 6c3a 2073  am).    label: s
-0000f3e0: 7472 2c0a 2020 2020 6964 3a20 7374 722c  tr,.    id: str,
-0000f3f0: 0a20 2020 2070 6572 6d69 7373 696f 6e73  .    permissions
-0000f400: 3a20 7374 7220 3d20 2272 6573 2d64 6566  : str = "res-def
-0000f410: 6175 6c74 222c 0a20 2020 2061 726b 3a20  ault",.    ark: 
-0000f420: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000f430: 4e6f 6e65 2c0a 2020 2020 6972 693a 204f  None,.    iri: O
-0000f440: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0000f450: 6f6e 652c 0a20 2020 2063 7265 6174 696f  one,.    creatio
-0000f460: 6e5f 6461 7465 3a20 4f70 7469 6f6e 616c  n_date: Optional
-0000f470: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2920  [str] = None,.) 
-0000f480: 2d3e 2065 7472 6565 2e5f 456c 656d 656e  -> etree._Elemen
-0000f490: 743a 0a20 2020 2022 2222 0a20 2020 2043  t:.    """.    C
-0000f4a0: 7265 6174 6573 2061 6e20 656d 7074 7920  reates an empty 
-0000f4b0: 7265 6769 6f6e 2065 6c65 6d65 6e74 2c20  region element, 
-0000f4c0: 7769 7468 2074 6865 2061 7474 7269 6275  with the attribu
-0000f4d0: 7465 7320 6173 2073 7065 6369 6669 6564  tes as specified
-0000f4e0: 2062 7920 7468 6520 6172 6775 6d65 6e74   by the argument
-0000f4f0: 730a 0a20 2020 2041 7267 733a 0a20 2020  s..    Args:.   
-0000f500: 2020 2020 2054 6865 2061 7267 756d 656e       The argumen
-0000f510: 7473 2063 6f72 7265 7370 6f6e 6420 313a  ts correspond 1:
-0000f520: 3120 746f 2074 6865 2061 7474 7269 6275  1 to the attribu
-0000f530: 7465 7320 6f66 2074 6865 203c 7265 6769  tes of the <regi
-0000f540: 6f6e 3e20 656c 656d 656e 742e 0a0a 2020  on> element...  
-0000f550: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
-0000f560: 2020 5761 726e 696e 673a 2069 6620 626f    Warning: if bo
-0000f570: 7468 2061 6e20 4152 4b20 616e 6420 616e  th an ARK and an
-0000f580: 2049 5249 2061 7265 2070 726f 7669 6465   IRI are provide
-0000f590: 640a 2020 2020 2020 2020 4261 7365 4572  d.        BaseEr
-0000f5a0: 726f 723a 2069 6620 7468 6520 6372 6561  ror: if the crea
-0000f5b0: 7469 6f6e 2064 6174 6520 6973 2069 6e76  tion date is inv
-0000f5c0: 616c 6964 0a0a 2020 2020 5265 7475 726e  alid..    Return
-0000f5d0: 733a 0a20 2020 2020 2020 2054 6865 2072  s:.        The r
-0000f5e0: 6567 696f 6e20 656c 656d 656e 742c 2077  egion element, w
-0000f5f0: 6974 686f 7574 2061 6e79 2063 6869 6c64  ithout any child
-0000f600: 7265 6e2c 2062 7574 2077 6974 6820 7468  ren, but with th
-0000f610: 6520 6174 7472 6962 7574 6573 3a0a 2020  e attributes:.  
-0000f620: 2020 2020 2020 3c72 6567 696f 6e20 6c61        <region la
-0000f630: 6265 6c3d 6c61 6265 6c20 6964 3d69 6420  bel=label id=id 
-0000f640: 7065 726d 6973 7369 6f6e 733d 7065 726d  permissions=perm
-0000f650: 6973 7369 6f6e 7320 6172 6b3d 6172 6b20  issions ark=ark 
-0000f660: 6972 693d 6972 693e 3c2f 7265 6769 6f6e  iri=iri></region
-0000f670: 3e0a 0a20 2020 2045 7861 6d70 6c65 733a  >..    Examples:
-0000f680: 0a20 2020 2020 2020 203e 3e3e 2072 6567  .        >>> reg
-0000f690: 696f 6e20 3d20 6578 6365 6c32 786d 6c2e  ion = excel2xml.
-0000f6a0: 6d61 6b65 5f72 6567 696f 6e28 226c 6162  make_region("lab
-0000f6b0: 656c 222c 2022 6964 2229 0a20 2020 2020  el", "id").     
-0000f6c0: 2020 203e 3e3e 2072 6567 696f 6e2e 6170     >>> region.ap
-0000f6d0: 7065 6e64 2865 7863 656c 3278 6d6c 2e6d  pend(excel2xml.m
-0000f6e0: 616b 655f 7465 7874 5f70 726f 7028 2268  ake_text_prop("h
-0000f6f0: 6173 436f 6d6d 656e 7422 2c20 2254 6869  asComment", "Thi
-0000f700: 7320 6973 2061 2063 6f6d 6d65 6e74 2229  s is a comment")
-0000f710: 290a 2020 2020 2020 2020 3e3e 3e20 7265  ).        >>> re
-0000f720: 6769 6f6e 2e61 7070 656e 6428 6578 6365  gion.append(exce
-0000f730: 6c32 786d 6c2e 6d61 6b65 5f63 6f6c 6f72  l2xml.make_color
-0000f740: 5f70 726f 7028 2268 6173 436f 6c6f 7222  _prop("hasColor"
-0000f750: 2c20 2223 3564 3166 3165 2229 290a 2020  , "#5d1f1e")).  
-0000f760: 2020 2020 2020 3e3e 3e20 7265 6769 6f6e        >>> region
-0000f770: 2e61 7070 656e 6428 6578 6365 6c32 786d  .append(excel2xm
-0000f780: 6c2e 6d61 6b65 5f72 6573 7074 725f 7072  l.make_resptr_pr
-0000f790: 6f70 2822 6973 5265 6769 6f6e 4f66 222c  op("isRegionOf",
-0000f7a0: 2022 696d 6167 655f 3022 2929 0a20 2020   "image_0")).   
-0000f7b0: 2020 2020 203e 3e3e 2072 6567 696f 6e2e       >>> region.
-0000f7c0: 6170 7065 6e64 2865 7863 656c 3278 6d6c  append(excel2xml
-0000f7d0: 2e6d 616b 655f 6765 6f6d 6574 7279 5f70  .make_geometry_p
-0000f7e0: 726f 7028 2268 6173 4765 6f6d 6574 7279  rop("hasGeometry
-0000f7f0: 222c 2022 7b2e 2e2e 7d22 2929 0a20 2020  ", "{...}")).   
-0000f800: 2020 2020 203e 3e3e 2072 6f6f 742e 6170       >>> root.ap
-0000f810: 7065 6e64 2872 6567 696f 6e29 0a0a 2020  pend(region)..  
-0000f820: 2020 5365 6520 6874 7470 733a 2f2f 646f    See https://do
-0000f830: 6373 2e64 6173 6368 2e73 7769 7373 2f6c  cs.dasch.swiss/l
-0000f840: 6174 6573 742f 4453 502d 544f 4f4c 532f  atest/DSP-TOOLS/
-0000f850: 6669 6c65 2d66 6f72 6d61 7473 2f78 6d6c  file-formats/xml
-0000f860: 2d64 6174 612d 6669 6c65 2f23 7265 6769  -data-file/#regi
-0000f870: 6f6e 0a20 2020 2022 2222 0a0a 2020 2020  on.    """..    
-0000f880: 6b77 6172 6773 203d 207b 226c 6162 656c  kwargs = {"label
-0000f890: 223a 206c 6162 656c 2c20 2269 6422 3a20  ": label, "id": 
-0000f8a0: 6964 2c20 2270 6572 6d69 7373 696f 6e73  id, "permissions
-0000f8b0: 223a 2070 6572 6d69 7373 696f 6e73 2c20  ": permissions, 
-0000f8c0: 226e 736d 6170 223a 2078 6d6c 5f6e 616d  "nsmap": xml_nam
-0000f8d0: 6573 7061 6365 5f6d 6170 7d0a 2020 2020  espace_map}.    
-0000f8e0: 6966 2061 726b 3a0a 2020 2020 2020 2020  if ark:.        
-0000f8f0: 6b77 6172 6773 5b22 6172 6b22 5d20 3d20  kwargs["ark"] = 
-0000f900: 6172 6b0a 2020 2020 6966 2069 7269 3a0a  ark.    if iri:.
-0000f910: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
-0000f920: 6972 6922 5d20 3d20 6972 690a 2020 2020  iri"] = iri.    
-0000f930: 6966 2061 726b 2061 6e64 2069 7269 3a0a  if ark and iri:.
-0000f940: 2020 2020 2020 2020 6d73 6720 3d20 6622          msg = f"
-0000f950: 426f 7468 2041 524b 2061 6e64 2049 5249  Both ARK and IRI
-0000f960: 2077 6572 6520 7072 6f76 6964 6564 2066   were provided f
-0000f970: 6f72 2072 6573 6f75 7263 6520 277b 6c61  or resource '{la
-0000f980: 6265 6c7d 2720 287b 6964 7d29 2e20 5468  bel}' ({id}). Th
-0000f990: 6520 4152 4b20 7769 6c6c 206f 7665 7272  e ARK will overr
-0000f9a0: 6964 6520 7468 6520 4952 492e 220a 2020  ide the IRI.".  
-0000f9b0: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-0000f9c0: 6172 6e28 4473 7054 6f6f 6c73 5573 6572  arn(DspToolsUser
-0000f9d0: 5761 726e 696e 6728 6d73 6729 290a 2020  Warning(msg)).  
-0000f9e0: 2020 6966 2063 7265 6174 696f 6e5f 6461    if creation_da
-0000f9f0: 7465 3a0a 2020 2020 2020 2020 7472 793a  te:.        try:
-0000fa00: 0a20 2020 2020 2020 2020 2020 2044 6174  .            Dat
-0000fa10: 6554 696d 6553 7461 6d70 2863 7265 6174  eTimeStamp(creat
-0000fa20: 696f 6e5f 6461 7465 290a 2020 2020 2020  ion_date).      
-0000fa30: 2020 6578 6365 7074 2042 6173 6545 7272    except BaseErr
-0000fa40: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-0000fa50: 7261 6973 6520 4261 7365 4572 726f 7228  raise BaseError(
-0000fa60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fa70: 2066 2254 6865 2072 6567 696f 6e20 277b   f"The region '{
-0000fa80: 6c61 6265 6c7d 2720 2849 443a 207b 6964  label}' (ID: {id
-0000fa90: 7d29 2068 6173 2061 6e20 696e 7661 6c69  }) has an invali
-0000faa0: 6420 6372 6561 7469 6f6e 2064 6174 6520  d creation date 
-0000fab0: 277b 6372 6561 7469 6f6e 5f64 6174 657d  '{creation_date}
-0000fac0: 272e 2022 0a20 2020 2020 2020 2020 2020  '. ".           
-0000fad0: 2020 2020 2066 2244 6964 2079 6f75 2070       f"Did you p
-0000fae0: 6572 6861 7073 2066 6f72 6765 7420 7468  erhaps forget th
-0000faf0: 6520 7469 6d65 7a6f 6e65 3f22 0a20 2020  e timezone?".   
-0000fb00: 2020 2020 2020 2020 2029 2066 726f 6d20           ) from 
-0000fb10: 4e6f 6e65 0a20 2020 2020 2020 206b 7761  None.        kwa
-0000fb20: 7267 735b 2263 7265 6174 696f 6e5f 6461  rgs["creation_da
-0000fb30: 7465 225d 203d 2063 7265 6174 696f 6e5f  te"] = creation_
-0000fb40: 6461 7465 0a0a 2020 2020 7265 7475 726e  date..    return
-0000fb50: 2065 7472 6565 2e45 6c65 6d65 6e74 280a   etree.Element(.
-0000fb60: 2020 2020 2020 2020 227b 2573 7d72 6567          "{%s}reg
-0000fb70: 696f 6e22 2025 2078 6d6c 5f6e 616d 6573  ion" % xml_names
-0000fb80: 7061 6365 5f6d 6170 5b4e 6f6e 655d 2c0a  pace_map[None],.
-0000fb90: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-0000fba0: 2c20 2023 2074 7970 653a 2069 676e 6f72  ,  # type: ignor
-0000fbb0: 655b 6172 672d 7479 7065 5d0a 2020 2020  e[arg-type].    
-0000fbc0: 290a 0a0a 6465 6620 6d61 6b65 5f61 6e6e  )...def make_ann
-0000fbd0: 6f74 6174 696f 6e28 2020 2320 6e6f 7161  otation(  # noqa
-0000fbe0: 3a20 4434 3137 2028 756e 646f 6375 6d65  : D417 (undocume
-0000fbf0: 6e74 6564 2d70 6172 616d 290a 2020 2020  nted-param).    
-0000fc00: 6c61 6265 6c3a 2073 7472 2c0a 2020 2020  label: str,.    
-0000fc10: 6964 3a20 7374 722c 0a20 2020 2070 6572  id: str,.    per
-0000fc20: 6d69 7373 696f 6e73 3a20 7374 7220 3d20  missions: str = 
-0000fc30: 2272 6573 2d64 6566 6175 6c74 222c 0a20  "res-default",. 
-0000fc40: 2020 2061 726b 3a20 4f70 7469 6f6e 616c     ark: Optional
-0000fc50: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000fc60: 2020 6972 693a 204f 7074 696f 6e61 6c5b    iri: Optional[
-0000fc70: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0000fc80: 2063 7265 6174 696f 6e5f 6461 7465 3a20   creation_date: 
-0000fc90: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000fca0: 4e6f 6e65 2c0a 2920 2d3e 2065 7472 6565  None,.) -> etree
-0000fcb0: 2e5f 456c 656d 656e 743a 0a20 2020 2022  ._Element:.    "
-0000fcc0: 2222 0a20 2020 2043 7265 6174 6573 2061  "".    Creates a
-0000fcd0: 6e20 656d 7074 7920 616e 6e6f 7461 7469  n empty annotati
-0000fce0: 6f6e 2065 6c65 6d65 6e74 2c20 7769 7468  on element, with
-0000fcf0: 2074 6865 2061 7474 7269 6275 7465 7320   the attributes 
-0000fd00: 6173 2073 7065 6369 6669 6564 2062 7920  as specified by 
-0000fd10: 7468 6520 6172 6775 6d65 6e74 730a 0a20  the arguments.. 
-0000fd20: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000fd30: 2054 6865 2061 7267 756d 656e 7473 2063   The arguments c
-0000fd40: 6f72 7265 7370 6f6e 6420 313a 3120 746f  orrespond 1:1 to
-0000fd50: 2074 6865 2061 7474 7269 6275 7465 7320   the attributes 
-0000fd60: 6f66 2074 6865 203c 616e 6e6f 7461 7469  of the <annotati
-0000fd70: 6f6e 3e20 656c 656d 656e 742e 0a0a 2020  on> element...  
-0000fd80: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
-0000fd90: 2020 5761 726e 696e 673a 2069 6620 626f    Warning: if bo
-0000fda0: 7468 2061 6e20 4152 4b20 616e 6420 616e  th an ARK and an
-0000fdb0: 2049 5249 2061 7265 2070 726f 7669 6465   IRI are provide
-0000fdc0: 640a 2020 2020 2020 2020 4261 7365 4572  d.        BaseEr
-0000fdd0: 726f 723a 2069 6620 7468 6520 6372 6561  ror: if the crea
-0000fde0: 7469 6f6e 2064 6174 6520 6973 2069 6e76  tion date is inv
-0000fdf0: 616c 6964 0a0a 2020 2020 5265 7475 726e  alid..    Return
-0000fe00: 733a 0a20 2020 2020 2020 2054 6865 2061  s:.        The a
-0000fe10: 6e6e 6f74 6174 696f 6e20 656c 656d 656e  nnotation elemen
-0000fe20: 742c 2077 6974 686f 7574 2061 6e79 2063  t, without any c
-0000fe30: 6869 6c64 7265 6e2c 2062 7574 2077 6974  hildren, but wit
-0000fe40: 6820 7468 6520 6174 7472 6962 7574 6573  h the attributes
-0000fe50: 3a0a 2020 2020 2020 2020 3c61 6e6e 6f74  :.        <annot
-0000fe60: 6174 696f 6e20 6c61 6265 6c3d 6c61 6265  ation label=labe
-0000fe70: 6c20 6964 3d69 6420 7065 726d 6973 7369  l id=id permissi
-0000fe80: 6f6e 733d 7065 726d 6973 7369 6f6e 7320  ons=permissions 
-0000fe90: 6172 6b3d 6172 6b20 6972 693d 6972 693e  ark=ark iri=iri>
-0000fea0: 3c2f 616e 6e6f 7461 7469 6f6e 3e0a 0a20  </annotation>.. 
-0000feb0: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
-0000fec0: 2020 2020 203e 3e3e 2061 6e6e 6f74 6174       >>> annotat
-0000fed0: 696f 6e20 3d20 6578 6365 6c32 786d 6c2e  ion = excel2xml.
-0000fee0: 6d61 6b65 5f61 6e6e 6f74 6174 696f 6e28  make_annotation(
-0000fef0: 226c 6162 656c 222c 2022 6964 2229 0a20  "label", "id"). 
-0000ff00: 2020 2020 2020 203e 3e3e 2061 6e6e 6f74         >>> annot
-0000ff10: 6174 696f 6e2e 6170 7065 6e64 2865 7863  ation.append(exc
-0000ff20: 656c 3278 6d6c 2e6d 616b 655f 7465 7874  el2xml.make_text
-0000ff30: 5f70 726f 7028 2268 6173 436f 6d6d 656e  _prop("hasCommen
-0000ff40: 7422 2c20 2254 6869 7320 6973 2061 2063  t", "This is a c
-0000ff50: 6f6d 6d65 6e74 2229 290a 2020 2020 2020  omment")).      
-0000ff60: 2020 3e3e 3e20 616e 6e6f 7461 7469 6f6e    >>> annotation
-0000ff70: 2e61 7070 656e 6428 6578 6365 6c32 786d  .append(excel2xm
-0000ff80: 6c2e 6d61 6b65 5f72 6573 7074 725f 7072  l.make_resptr_pr
-0000ff90: 6f70 2822 6973 416e 6e6f 7461 7469 6f6e  op("isAnnotation
-0000ffa0: 4f66 222c 2022 7265 736f 7572 6365 5f30  Of", "resource_0
-0000ffb0: 2229 290a 2020 2020 2020 2020 3e3e 3e20  ")).        >>> 
-0000ffc0: 726f 6f74 2e61 7070 656e 6428 616e 6e6f  root.append(anno
-0000ffd0: 7461 7469 6f6e 290a 0a20 2020 2053 6565  tation)..    See
-0000ffe0: 2068 7474 7073 3a2f 2f64 6f63 732e 6461   https://docs.da
-0000fff0: 7363 682e 7377 6973 732f 6c61 7465 7374  sch.swiss/latest
-00010000: 2f44 5350 2d54 4f4f 4c53 2f66 696c 652d  /DSP-TOOLS/file-
-00010010: 666f 726d 6174 732f 786d 6c2d 6461 7461  formats/xml-data
-00010020: 2d66 696c 652f 2361 6e6e 6f74 6174 696f  -file/#annotatio
-00010030: 6e0a 2020 2020 2222 220a 0a20 2020 206b  n.    """..    k
-00010040: 7761 7267 7320 3d20 7b22 6c61 6265 6c22  wargs = {"label"
-00010050: 3a20 6c61 6265 6c2c 2022 6964 223a 2069  : label, "id": i
-00010060: 642c 2022 7065 726d 6973 7369 6f6e 7322  d, "permissions"
-00010070: 3a20 7065 726d 6973 7369 6f6e 732c 2022  : permissions, "
-00010080: 6e73 6d61 7022 3a20 786d 6c5f 6e61 6d65  nsmap": xml_name
-00010090: 7370 6163 655f 6d61 707d 0a20 2020 2069  space_map}.    i
-000100a0: 6620 6172 6b3a 0a20 2020 2020 2020 206b  f ark:.        k
-000100b0: 7761 7267 735b 2261 726b 225d 203d 2061  wargs["ark"] = a
-000100c0: 726b 0a20 2020 2069 6620 6972 693a 0a20  rk.    if iri:. 
-000100d0: 2020 2020 2020 206b 7761 7267 735b 2269         kwargs["i
-000100e0: 7269 225d 203d 2069 7269 0a20 2020 2069  ri"] = iri.    i
-000100f0: 6620 6172 6b20 616e 6420 6972 693a 0a20  f ark and iri:. 
-00010100: 2020 2020 2020 2077 6172 6e69 6e67 203d         warning =
-00010110: 2066 2242 6f74 6820 4152 4b20 616e 6420   f"Both ARK and 
-00010120: 4952 4920 7765 7265 2070 726f 7669 6465  IRI were provide
-00010130: 6420 666f 7220 7265 736f 7572 6365 2027  d for resource '
-00010140: 7b6c 6162 656c 7d27 2028 7b69 647d 292e  {label}' ({id}).
-00010150: 2054 6865 2041 524b 2077 696c 6c20 6f76   The ARK will ov
-00010160: 6572 7269 6465 2074 6865 2049 5249 2e22  erride the IRI."
-00010170: 0a20 2020 2020 2020 2077 6172 6e69 6e67  .        warning
-00010180: 732e 7761 726e 2844 7370 546f 6f6c 7355  s.warn(DspToolsU
-00010190: 7365 7257 6172 6e69 6e67 2877 6172 6e69  serWarning(warni
-000101a0: 6e67 2929 0a20 2020 2069 6620 6372 6561  ng)).    if crea
-000101b0: 7469 6f6e 5f64 6174 653a 0a20 2020 2020  tion_date:.     
-000101c0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000101d0: 2020 2020 4461 7465 5469 6d65 5374 616d      DateTimeStam
-000101e0: 7028 6372 6561 7469 6f6e 5f64 6174 6529  p(creation_date)
-000101f0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00010200: 4261 7365 4572 726f 723a 0a20 2020 2020  BaseError:.     
-00010210: 2020 2020 2020 2072 6169 7365 2042 6173         raise Bas
-00010220: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00010230: 2020 2020 2020 2020 6622 5468 6520 616e          f"The an
-00010240: 6e6f 7461 7469 6f6e 2027 7b6c 6162 656c  notation '{label
-00010250: 7d27 2028 4944 3a20 7b69 647d 2920 6861  }' (ID: {id}) ha
-00010260: 7320 616e 2069 6e76 616c 6964 2063 7265  s an invalid cre
-00010270: 6174 696f 6e20 6461 7465 2027 7b63 7265  ation date '{cre
-00010280: 6174 696f 6e5f 6461 7465 7d27 2e20 220a  ation_date}'. ".
-00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 6622 4469 6420 796f 7520 7065 7268 6170  f"Did you perhap
-000102b0: 7320 666f 7267 6574 2074 6865 2074 696d  s forget the tim
-000102c0: 657a 6f6e 653f 220a 2020 2020 2020 2020  ezone?".        
-000102d0: 2020 2020 2920 6672 6f6d 204e 6f6e 650a      ) from None.
-000102e0: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
-000102f0: 6372 6561 7469 6f6e 5f64 6174 6522 5d20  creation_date"] 
-00010300: 3d20 6372 6561 7469 6f6e 5f64 6174 650a  = creation_date.
-00010310: 0a20 2020 2072 6574 7572 6e20 6574 7265  .    return etre
-00010320: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
-00010330: 2020 2022 7b25 737d 616e 6e6f 7461 7469     "{%s}annotati
-00010340: 6f6e 2220 2520 786d 6c5f 6e61 6d65 7370  on" % xml_namesp
-00010350: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
-00010360: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
-00010370: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-00010380: 5b61 7267 2d74 7970 655d 0a20 2020 2029  [arg-type].    )
-00010390: 0a0a 0a64 6566 206d 616b 655f 6c69 6e6b  ...def make_link
-000103a0: 2820 2023 206e 6f71 613a 2044 3431 3720  (  # noqa: D417 
-000103b0: 2875 6e64 6f63 756d 656e 7465 642d 7061  (undocumented-pa
-000103c0: 7261 6d29 0a20 2020 206c 6162 656c 3a20  ram).    label: 
-000103d0: 7374 722c 0a20 2020 2069 643a 2073 7472  str,.    id: str
-000103e0: 2c0a 2020 2020 7065 726d 6973 7369 6f6e  ,.    permission
-000103f0: 733a 2073 7472 203d 2022 7265 732d 6465  s: str = "res-de
-00010400: 6661 756c 7422 2c0a 2020 2020 6172 6b3a  fault",.    ark:
-00010410: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00010420: 204e 6f6e 652c 0a20 2020 2069 7269 3a20   None,.    iri: 
-00010430: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00010440: 4e6f 6e65 2c0a 2020 2020 6372 6561 7469  None,.    creati
-00010450: 6f6e 5f64 6174 653a 204f 7074 696f 6e61  on_date: Optiona
-00010460: 6c5b 7374 725d 203d 204e 6f6e 652c 0a29  l[str] = None,.)
-00010470: 202d 3e20 6574 7265 652e 5f45 6c65 6d65   -> etree._Eleme
-00010480: 6e74 3a0a 2020 2020 2222 220a 2020 2020  nt:.    """.    
-00010490: 4372 6561 7465 7320 616e 2065 6d70 7479  Creates an empty
-000104a0: 206c 696e 6b20 656c 656d 656e 742c 2077   link element, w
-000104b0: 6974 6820 7468 6520 6174 7472 6962 7574  ith the attribut
-000104c0: 6573 2061 7320 7370 6563 6966 6965 6420  es as specified 
-000104d0: 6279 2074 6865 2061 7267 756d 656e 7473  by the arguments
-000104e0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-000104f0: 2020 2020 5468 6520 6172 6775 6d65 6e74      The argument
-00010500: 7320 636f 7272 6573 706f 6e64 2031 3a31  s correspond 1:1
-00010510: 2074 6f20 7468 6520 6174 7472 6962 7574   to the attribut
-00010520: 6573 206f 6620 7468 6520 3c6c 696e 6b3e  es of the <link>
-00010530: 2065 6c65 6d65 6e74 2e0a 0a20 2020 2052   element...    R
-00010540: 6169 7365 733a 0a20 2020 2020 2020 2057  aises:.        W
-00010550: 6172 6e69 6e67 3a20 6966 2062 6f74 6820  arning: if both 
-00010560: 616e 2041 524b 2061 6e64 2061 6e20 4952  an ARK and an IR
-00010570: 4920 6172 6520 7072 6f76 6964 6564 0a20  I are provided. 
-00010580: 2020 2020 2020 2042 6173 6545 7272 6f72         BaseError
-00010590: 3a20 6966 2074 6865 2063 7265 6174 696f  : if the creatio
-000105a0: 6e20 6461 7465 2069 7320 696e 7661 6c69  n date is invali
-000105b0: 640a 0a20 2020 2052 6574 7572 6e73 3a0a  d..    Returns:.
-000105c0: 2020 2020 2020 2020 5468 6520 6c69 6e6b          The link
-000105d0: 2065 6c65 6d65 6e74 2c20 7769 7468 6f75   element, withou
-000105e0: 7420 616e 7920 6368 696c 6472 656e 2c20  t any children, 
-000105f0: 6275 7420 7769 7468 2074 6865 2061 7474  but with the att
-00010600: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
-00010610: 203c 6c69 6e6b 206c 6162 656c 3d6c 6162   <link label=lab
-00010620: 656c 2069 643d 6964 2070 6572 6d69 7373  el id=id permiss
-00010630: 696f 6e73 3d70 6572 6d69 7373 696f 6e73  ions=permissions
-00010640: 2061 726b 3d61 726b 2069 7269 3d69 7269   ark=ark iri=iri
-00010650: 3e3c 2f6c 696e 6b3e 0a0a 2020 2020 4578  ></link>..    Ex
-00010660: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-00010670: 3e3e 3e20 6c69 6e6b 203d 2065 7863 656c  >>> link = excel
-00010680: 3278 6d6c 2e6d 616b 655f 6c69 6e6b 2822  2xml.make_link("
-00010690: 6c61 6265 6c22 2c20 2269 6422 290a 2020  label", "id").  
-000106a0: 2020 2020 2020 3e3e 3e20 6c69 6e6b 2e61        >>> link.a
-000106b0: 7070 656e 6428 6578 6365 6c32 786d 6c2e  ppend(excel2xml.
-000106c0: 6d61 6b65 5f74 6578 745f 7072 6f70 2822  make_text_prop("
-000106d0: 6861 7343 6f6d 6d65 6e74 222c 2022 5468  hasComment", "Th
-000106e0: 6973 2069 7320 6120 636f 6d6d 656e 7422  is is a comment"
-000106f0: 2929 0a20 2020 2020 2020 203e 3e3e 206c  )).        >>> l
-00010700: 696e 6b2e 6170 7065 6e64 2865 7863 656c  ink.append(excel
-00010710: 3278 6d6c 2e6d 616b 655f 7265 7370 7472  2xml.make_resptr
-00010720: 5f70 726f 7028 2268 6173 4c69 6e6b 546f  _prop("hasLinkTo
-00010730: 222c 205b 2272 6573 6f75 7263 655f 3022  ", ["resource_0"
-00010740: 2c20 2272 6573 6f75 7263 655f 3122 5d29  , "resource_1"])
-00010750: 290a 2020 2020 2020 2020 3e3e 3e20 726f  ).        >>> ro
-00010760: 6f74 2e61 7070 656e 6428 6c69 6e6b 290a  ot.append(link).
-00010770: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
-00010780: 2f64 6f63 732e 6461 7363 682e 7377 6973  /docs.dasch.swis
-00010790: 732f 6c61 7465 7374 2f44 5350 2d54 4f4f  s/latest/DSP-TOO
-000107a0: 4c53 2f66 696c 652d 666f 726d 6174 732f  LS/file-formats/
-000107b0: 786d 6c2d 6461 7461 2d66 696c 652f 236c  xml-data-file/#l
-000107c0: 696e 6b0a 2020 2020 2222 220a 0a20 2020  ink.    """..   
-000107d0: 206b 7761 7267 7320 3d20 7b22 6c61 6265   kwargs = {"labe
-000107e0: 6c22 3a20 6c61 6265 6c2c 2022 6964 223a  l": label, "id":
-000107f0: 2069 642c 2022 7065 726d 6973 7369 6f6e   id, "permission
-00010800: 7322 3a20 7065 726d 6973 7369 6f6e 732c  s": permissions,
-00010810: 2022 6e73 6d61 7022 3a20 786d 6c5f 6e61   "nsmap": xml_na
-00010820: 6d65 7370 6163 655f 6d61 707d 0a20 2020  mespace_map}.   
-00010830: 2069 6620 6172 6b3a 0a20 2020 2020 2020   if ark:.       
-00010840: 206b 7761 7267 735b 2261 726b 225d 203d   kwargs["ark"] =
-00010850: 2061 726b 0a20 2020 2069 6620 6972 693a   ark.    if iri:
-00010860: 0a20 2020 2020 2020 206b 7761 7267 735b  .        kwargs[
-00010870: 2269 7269 225d 203d 2069 7269 0a20 2020  "iri"] = iri.   
-00010880: 2069 6620 6172 6b20 616e 6420 6972 693a   if ark and iri:
-00010890: 0a20 2020 2020 2020 206d 7367 203d 2066  .        msg = f
-000108a0: 2242 6f74 6820 4152 4b20 616e 6420 4952  "Both ARK and IR
-000108b0: 4920 7765 7265 2070 726f 7669 6465 6420  I were provided 
-000108c0: 666f 7220 7265 736f 7572 6365 2027 7b6c  for resource '{l
-000108d0: 6162 656c 7d27 2028 7b69 647d 292e 2054  abel}' ({id}). T
-000108e0: 6865 2041 524b 2077 696c 6c20 6f76 6572  he ARK will over
-000108f0: 7269 6465 2074 6865 2049 5249 2e22 0a20  ride the IRI.". 
-00010900: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-00010910: 7761 726e 2844 7370 546f 6f6c 7355 7365  warn(DspToolsUse
-00010920: 7257 6172 6e69 6e67 286d 7367 2929 0a20  rWarning(msg)). 
-00010930: 2020 2069 6620 6372 6561 7469 6f6e 5f64     if creation_d
-00010940: 6174 653a 0a20 2020 2020 2020 2074 7279  ate:.        try
-00010950: 3a0a 2020 2020 2020 2020 2020 2020 4461  :.            Da
-00010960: 7465 5469 6d65 5374 616d 7028 6372 6561  teTimeStamp(crea
-00010970: 7469 6f6e 5f64 6174 6529 0a20 2020 2020  tion_date).     
-00010980: 2020 2065 7863 6570 7420 4261 7365 4572     except BaseEr
-00010990: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-000109a0: 2072 6169 7365 2042 6173 6545 7272 6f72   raise BaseError
-000109b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000109c0: 2020 6622 5468 6520 6c69 6e6b 2027 7b6c    f"The link '{l
-000109d0: 6162 656c 7d27 2028 4944 3a20 7b69 647d  abel}' (ID: {id}
-000109e0: 2920 6861 7320 616e 2069 6e76 616c 6964  ) has an invalid
-000109f0: 2063 7265 6174 696f 6e20 6461 7465 2027   creation date '
-00010a00: 7b63 7265 6174 696f 6e5f 6461 7465 7d27  {creation_date}'
-00010a10: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-00010a20: 2020 2020 6622 4469 6420 796f 7520 7065      f"Did you pe
-00010a30: 7268 6170 7320 666f 7267 6574 2074 6865  rhaps forget the
-00010a40: 2074 696d 657a 6f6e 653f 220a 2020 2020   timezone?".    
-00010a50: 2020 2020 2020 2020 2920 6672 6f6d 204e          ) from N
-00010a60: 6f6e 650a 2020 2020 2020 2020 6b77 6172  one.        kwar
-00010a70: 6773 5b22 6372 6561 7469 6f6e 5f64 6174  gs["creation_dat
-00010a80: 6522 5d20 3d20 6372 6561 7469 6f6e 5f64  e"] = creation_d
-00010a90: 6174 650a 0a20 2020 2072 6574 7572 6e20  ate..    return 
-00010aa0: 6574 7265 652e 456c 656d 656e 7428 0a20  etree.Element(. 
-00010ab0: 2020 2020 2020 2022 7b25 737d 6c69 6e6b         "{%s}link
-00010ac0: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-00010ad0: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-00010ae0: 2020 2020 202a 2a6b 7761 7267 732c 2020       **kwargs,  
-00010af0: 2320 7479 7065 3a20 6967 6e6f 7265 5b61  # type: ignore[a
-00010b00: 7267 2d74 7970 655d 0a20 2020 2029 0a0a  rg-type].    )..
-00010b10: 0a64 6566 206d 616b 655f 6175 6469 6f5f  .def make_audio_
-00010b20: 7365 676d 656e 7428 2020 2320 6e6f 7161  segment(  # noqa
-00010b30: 3a20 4434 3137 2028 756e 646f 6375 6d65  : D417 (undocume
-00010b40: 6e74 6564 2d70 6172 616d 290a 2020 2020  nted-param).    
-00010b50: 6c61 6265 6c3a 2073 7472 2c0a 2020 2020  label: str,.    
-00010b60: 6964 3a20 7374 722c 0a20 2020 2070 6572  id: str,.    per
-00010b70: 6d69 7373 696f 6e73 3a20 7374 7220 3d20  missions: str = 
-00010b80: 2272 6573 2d64 6566 6175 6c74 222c 0a29  "res-default",.)
-00010b90: 202d 3e20 6574 7265 652e 5f45 6c65 6d65   -> etree._Eleme
-00010ba0: 6e74 3a0a 2020 2020 2222 220a 2020 2020  nt:.    """.    
-00010bb0: 4372 6561 7465 7320 616e 2065 6d70 7479  Creates an empty
-00010bc0: 203c 6175 6469 6f2d 7365 676d 656e 743e   <audio-segment>
-00010bd0: 2065 6c65 6d65 6e74 2c20 7769 7468 2074   element, with t
-00010be0: 6865 2061 7474 7269 6275 7465 7320 6173  he attributes as
-00010bf0: 2073 7065 6369 6669 6564 2062 7920 7468   specified by th
-00010c00: 6520 6172 6775 6d65 6e74 730a 0a20 2020  e arguments..   
-00010c10: 2041 7267 733a 0a20 2020 2020 2020 2054   Args:.        T
-00010c20: 6865 2061 7267 756d 656e 7473 2063 6f72  he arguments cor
-00010c30: 7265 7370 6f6e 6420 313a 3120 746f 2074  respond 1:1 to t
-00010c40: 6865 2061 7474 7269 6275 7465 7320 6f66  he attributes of
-00010c50: 2074 6865 203c 6175 6469 6f2d 7365 676d   the <audio-segm
-00010c60: 656e 743e 2065 6c65 6d65 6e74 2e0a 0a20  ent> element... 
-00010c70: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00010c80: 2020 2020 5468 6520 6175 6469 6f2d 7365      The audio-se
-00010c90: 676d 656e 7420 656c 656d 656e 742c 2077  gment element, w
-00010ca0: 6974 686f 7574 2061 6e79 2063 6869 6c64  ithout any child
-00010cb0: 7265 6e2c 2062 7574 2077 6974 6820 7468  ren, but with th
-00010cc0: 6520 6174 7472 6962 7574 6573 3a0a 2020  e attributes:.  
-00010cd0: 2020 2020 2020 3c61 7564 696f 2d73 6567        <audio-seg
-00010ce0: 6d65 6e74 206c 6162 656c 3d6c 6162 656c  ment label=label
-00010cf0: 2069 643d 6964 2070 6572 6d69 7373 696f   id=id permissio
-00010d00: 6e73 3d70 6572 6d69 7373 696f 6e73 3e3c  ns=permissions><
-00010d10: 2f61 7564 696f 2d73 6567 6d65 6e74 3e0a  /audio-segment>.
-00010d20: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
-00010d30: 2020 2020 2020 203e 3e3e 2061 7564 696f         >>> audio
-00010d40: 5f73 6567 6d65 6e74 203d 2065 7863 656c  _segment = excel
-00010d50: 3278 6d6c 2e6d 616b 655f 6175 6469 6f5f  2xml.make_audio_
-00010d60: 7365 676d 656e 7428 226c 6162 656c 222c  segment("label",
-00010d70: 2022 6964 2229 0a20 2020 2020 2020 203e   "id").        >
-00010d80: 3e3e 2061 7564 696f 5f73 6567 6d65 6e74  >> audio_segment
-00010d90: 2e61 7070 656e 6428 6578 6365 6c32 786d  .append(excel2xm
-00010da0: 6c2e 6d61 6b65 5f72 6573 7074 725f 7072  l.make_resptr_pr
-00010db0: 6f70 2822 6973 5365 676d 656e 744f 6622  op("isSegmentOf"
-00010dc0: 2c20 2261 7564 696f 5f72 6573 6f75 7263  , "audio_resourc
-00010dd0: 655f 6964 2229 290a 2020 2020 2020 2020  e_id")).        
-00010de0: 3e3e 3e20 6175 6469 6f5f 7365 676d 656e  >>> audio_segmen
-00010df0: 742e 6170 7065 6e64 2865 7863 656c 3278  t.append(excel2x
-00010e00: 6d6c 2e6d 616b 655f 696e 7465 7276 616c  ml.make_interval
-00010e10: 5f70 726f 7028 2268 6173 5365 676d 656e  _prop("hasSegmen
-00010e20: 7442 6f75 6e64 7322 2c20 2236 303a 3132  tBounds", "60:12
-00010e30: 3022 290a 2020 2020 2020 2020 3e3e 3e20  0").        >>> 
-00010e40: 726f 6f74 2e61 7070 656e 6428 6175 6469  root.append(audi
-00010e50: 6f5f 7365 676d 656e 7429 0a0a 2020 2020  o_segment)..    
-00010e60: 5365 6520 6874 7470 733a 2f2f 646f 6373  See https://docs
-00010e70: 2e64 6173 6368 2e73 7769 7373 2f6c 6174  .dasch.swiss/lat
-00010e80: 6573 742f 4453 502d 544f 4f4c 532f 6669  est/DSP-TOOLS/fi
-00010e90: 6c65 2d66 6f72 6d61 7473 2f78 6d6c 2d64  le-formats/xml-d
-00010ea0: 6174 612d 6669 6c65 2f23 7669 6465 6f2d  ata-file/#video-
-00010eb0: 7365 676d 656e 742d 6175 6469 6f2d 7365  segment-audio-se
-00010ec0: 676d 656e 740a 2020 2020 2222 220a 2020  gment.    """.  
-00010ed0: 2020 7265 7475 726e 2065 7472 6565 2e45    return etree.E
-00010ee0: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
-00010ef0: 227b 2573 7d61 7564 696f 2d73 6567 6d65  "{%s}audio-segme
-00010f00: 6e74 2220 2520 786d 6c5f 6e61 6d65 7370  nt" % xml_namesp
-00010f10: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
-00010f20: 2020 2020 2020 206c 6162 656c 3d6c 6162         label=lab
-00010f30: 656c 2c0a 2020 2020 2020 2020 6964 3d69  el,.        id=i
-00010f40: 642c 0a20 2020 2020 2020 2070 6572 6d69  d,.        permi
-00010f50: 7373 696f 6e73 3d70 6572 6d69 7373 696f  ssions=permissio
-00010f60: 6e73 2c0a 2020 2020 2020 2020 6e73 6d61  ns,.        nsma
-00010f70: 703d 786d 6c5f 6e61 6d65 7370 6163 655f  p=xml_namespace_
-00010f80: 6d61 702c 0a20 2020 2029 0a0a 0a64 6566  map,.    )...def
-00010f90: 206d 616b 655f 7669 6465 6f5f 7365 676d   make_video_segm
-00010fa0: 656e 7428 2020 2320 6e6f 7161 3a20 4434  ent(  # noqa: D4
-00010fb0: 3137 2028 756e 646f 6375 6d65 6e74 6564  17 (undocumented
-00010fc0: 2d70 6172 616d 290a 2020 2020 6c61 6265  -param).    labe
-00010fd0: 6c3a 2073 7472 2c0a 2020 2020 6964 3a20  l: str,.    id: 
-00010fe0: 7374 722c 0a20 2020 2070 6572 6d69 7373  str,.    permiss
-00010ff0: 696f 6e73 3a20 7374 7220 3d20 2272 6573  ions: str = "res
-00011000: 2d64 6566 6175 6c74 222c 0a29 202d 3e20  -default",.) -> 
-00011010: 6574 7265 652e 5f45 6c65 6d65 6e74 3a0a  etree._Element:.
-00011020: 2020 2020 2222 220a 2020 2020 4372 6561      """.    Crea
-00011030: 7465 7320 616e 2065 6d70 7479 203c 7669  tes an empty <vi
-00011040: 6465 6f2d 7365 676d 656e 743e 2065 6c65  deo-segment> ele
-00011050: 6d65 6e74 2c20 7769 7468 2074 6865 2061  ment, with the a
-00011060: 7474 7269 6275 7465 7320 6173 2073 7065  ttributes as spe
-00011070: 6369 6669 6564 2062 7920 7468 6520 6172  cified by the ar
-00011080: 6775 6d65 6e74 730a 0a20 2020 2041 7267  guments..    Arg
-00011090: 733a 0a20 2020 2020 2020 2054 6865 2061  s:.        The a
-000110a0: 7267 756d 656e 7473 2063 6f72 7265 7370  rguments corresp
-000110b0: 6f6e 6420 313a 3120 746f 2074 6865 2061  ond 1:1 to the a
-000110c0: 7474 7269 6275 7465 7320 6f66 2074 6865  ttributes of the
-000110d0: 203c 7669 6465 6f2d 7365 676d 656e 743e   <video-segment>
-000110e0: 2065 6c65 6d65 6e74 2e0a 0a20 2020 2052   element...    R
-000110f0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00011100: 5468 6520 7669 6465 6f2d 7365 676d 656e  The video-segmen
-00011110: 7420 656c 656d 656e 742c 2077 6974 686f  t element, witho
-00011120: 7574 2061 6e79 2063 6869 6c64 7265 6e2c  ut any children,
-00011130: 2062 7574 2077 6974 6820 7468 6520 6174   but with the at
-00011140: 7472 6962 7574 6573 3a0a 2020 2020 2020  tributes:.      
-00011150: 2020 3c76 6964 656f 2d73 6567 6d65 6e74    <video-segment
-00011160: 206c 6162 656c 3d6c 6162 656c 2069 643d   label=label id=
-00011170: 6964 2070 6572 6d69 7373 696f 6e73 3d70  id permissions=p
-00011180: 6572 6d69 7373 696f 6e73 3e3c 2f76 6964  ermissions></vid
-00011190: 656f 2d73 6567 6d65 6e74 3e0a 0a20 2020  eo-segment>..   
-000111a0: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
-000111b0: 2020 203e 3e3e 2076 6964 656f 5f73 6567     >>> video_seg
-000111c0: 6d65 6e74 203d 2065 7863 656c 3278 6d6c  ment = excel2xml
-000111d0: 2e6d 616b 655f 7669 6465 6f5f 7365 676d  .make_video_segm
-000111e0: 656e 7428 226c 6162 656c 222c 2022 6964  ent("label", "id
-000111f0: 2229 0a20 2020 2020 2020 203e 3e3e 2076  ").        >>> v
-00011200: 6964 656f 5f73 6567 6d65 6e74 2e61 7070  ideo_segment.app
-00011210: 656e 6428 6578 6365 6c32 786d 6c2e 6d61  end(excel2xml.ma
-00011220: 6b65 5f72 6573 7074 725f 7072 6f70 2822  ke_resptr_prop("
-00011230: 6973 5365 676d 656e 744f 6622 2c20 2276  isSegmentOf", "v
-00011240: 6964 656f 5f72 6573 6f75 7263 655f 6964  ideo_resource_id
-00011250: 2229 290a 2020 2020 2020 2020 3e3e 3e20  ")).        >>> 
-00011260: 7669 6465 6f5f 7365 676d 656e 742e 6170  video_segment.ap
-00011270: 7065 6e64 2865 7863 656c 3278 6d6c 2e6d  pend(excel2xml.m
-00011280: 616b 655f 696e 7465 7276 616c 5f70 726f  ake_interval_pro
-00011290: 7028 2268 6173 5365 676d 656e 7442 6f75  p("hasSegmentBou
-000112a0: 6e64 7322 2c20 2236 303a 3132 3022 290a  nds", "60:120").
-000112b0: 2020 2020 2020 2020 3e3e 3e20 726f 6f74          >>> root
-000112c0: 2e61 7070 656e 6428 7669 6465 6f5f 7365  .append(video_se
-000112d0: 676d 656e 7429 0a0a 2020 2020 5365 6520  gment)..    See 
-000112e0: 6874 7470 733a 2f2f 646f 6373 2e64 6173  https://docs.das
-000112f0: 6368 2e73 7769 7373 2f6c 6174 6573 742f  ch.swiss/latest/
-00011300: 4453 502d 544f 4f4c 532f 6669 6c65 2d66  DSP-TOOLS/file-f
-00011310: 6f72 6d61 7473 2f78 6d6c 2d64 6174 612d  ormats/xml-data-
-00011320: 6669 6c65 2f23 7669 6465 6f2d 7365 676d  file/#video-segm
-00011330: 656e 742d 6175 6469 6f2d 7365 676d 656e  ent-audio-segmen
-00011340: 740a 2020 2020 2222 220a 2020 2020 7265  t.    """.    re
-00011350: 7475 726e 2065 7472 6565 2e45 6c65 6d65  turn etree.Eleme
-00011360: 6e74 280a 2020 2020 2020 2020 227b 2573  nt(.        "{%s
-00011370: 7d76 6964 656f 2d73 6567 6d65 6e74 2220  }video-segment" 
-00011380: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
-00011390: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
-000113a0: 2020 206c 6162 656c 3d6c 6162 656c 2c0a     label=label,.
-000113b0: 2020 2020 2020 2020 6964 3d69 642c 0a20          id=id,. 
-000113c0: 2020 2020 2020 2070 6572 6d69 7373 696f         permissio
-000113d0: 6e73 3d70 6572 6d69 7373 696f 6e73 2c0a  ns=permissions,.
-000113e0: 2020 2020 2020 2020 6e73 6d61 703d 786d          nsmap=xm
-000113f0: 6c5f 6e61 6d65 7370 6163 655f 6d61 702c  l_namespace_map,
-00011400: 0a20 2020 2029 0a0a 0a64 6566 2063 7265  .    )...def cre
-00011410: 6174 655f 696e 7465 7276 616c 5f76 616c  ate_interval_val
-00011420: 7565 2873 7461 7274 3a20 7374 722c 2065  ue(start: str, e
-00011430: 6e64 3a20 7374 7229 202d 3e20 7374 723a  nd: str) -> str:
-00011440: 0a20 2020 2022 2222 0a20 2020 2054 7261  .    """.    Tra
-00011450: 6e73 666f 726d 2061 2073 7461 7274 2061  nsform a start a
-00011460: 6e64 2065 6e64 2074 696d 6520 696e 746f  nd end time into
-00011470: 2061 2076 616c 6964 2044 5350 2069 6e74   a valid DSP int
-00011480: 6572 7661 6c20 7661 6c75 652c 0a20 2020  erval value,.   
-00011490: 2077 6869 6368 2074 6865 6e20 6361 6e20   which then can 
-000114a0: 6265 2075 7365 6420 696e 2061 6e20 3c69  be used in an <i
-000114b0: 6e74 6572 7661 6c20 6e61 6d65 3d22 6861  nterval name="ha
-000114c0: 7353 6567 6d65 6e74 426f 756e 6473 223e  sSegmentBounds">
-000114d0: 2074 6167 2c0a 2020 2020 7768 6963 6820   tag,.    which 
-000114e0: 6973 2075 7365 6420 696e 203c 6175 6469  is used in <audi
-000114f0: 6f2d 7365 676d 656e 743e 2061 6e64 203c  o-segment> and <
-00011500: 7669 6465 6f2d 7365 676d 656e 743e 2065  video-segment> e
-00011510: 6c65 6d65 6e74 732e 0a0a 2020 2020 4172  lements...    Ar
-00011520: 6773 3a0a 2020 2020 2020 2020 7374 6172  gs:.        star
-00011530: 743a 2073 7461 7274 2074 696d 6520 6f66  t: start time of
-00011540: 2074 6865 2076 6964 656f 2f61 7564 696f   the video/audio
-00011550: 2073 6567 6d65 6e74 2c20 696e 2074 6865   segment, in the
-00011560: 2066 6f72 6d61 7420 2748 2848 293a 4d4d   format 'H(H):MM
-00011570: 3a53 5328 2e73 2927 0a20 2020 2020 2020  :SS(.s)'.       
-00011580: 2065 6e64 3a20 656e 6420 7469 6d65 206f   end: end time o
-00011590: 6620 7468 6520 7669 6465 6f2f 6175 6469  f the video/audi
-000115a0: 6f20 7365 676d 656e 742c 2069 6e20 7468  o segment, in th
-000115b0: 6520 666f 726d 6174 2027 4828 4829 3a4d  e format 'H(H):M
-000115c0: 4d3a 5353 282e 7329 270a 0a20 2020 2052  M:SS(.s)'..    R
-000115d0: 6169 7365 733a 0a20 2020 2020 2020 2056  aises:.        V
-000115e0: 616c 7565 4572 726f 723a 2069 6620 7468  alueError: if th
-000115f0: 6520 7072 6f76 6964 6564 2061 7267 756d  e provided argum
-00011600: 656e 7473 2061 7265 206e 6f74 2069 6e20  ents are not in 
-00011610: 7468 6520 636f 7272 6563 7420 666f 726d  the correct form
-00011620: 6174 2c20 6f72 2069 6620 7468 6520 7374  at, or if the st
-00011630: 6172 7420 7469 6d65 2069 7320 6772 6561  art time is grea
-00011640: 7465 7220 7468 616e 2074 6865 2065 6e64  ter than the end
-00011650: 2074 696d 650a 0a20 2020 2052 6574 7572   time..    Retur
-00011660: 6e73 3a0a 2020 2020 2020 2020 6120 4453  ns:.        a DS
-00011670: 5020 696e 7465 7276 616c 2076 616c 7565  P interval value
-00011680: 2069 6e20 7468 6520 666f 726d 6174 2027   in the format '
-00011690: 7374 6172 745f 7365 636f 6e64 733a 656e  start_seconds:en
-000116a0: 645f 7365 636f 6e64 7327 0a0a 2020 2020  d_seconds'..    
-000116b0: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
-000116c0: 2020 3e3e 3e20 6578 6365 6c32 786d 6c2e    >>> excel2xml.
-000116d0: 6372 6561 7465 5f69 6e74 6572 7661 6c5f  create_interval_
-000116e0: 7661 6c75 6528 2230 3a30 313a 3030 222c  value("0:01:00",
-000116f0: 2022 303a 3032 3a30 3022 290a 2020 2020   "0:02:00").    
-00011700: 2020 2020 2236 303a 3132 3022 0a20 2020      "60:120".   
-00011710: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
-00011720: 6d6c 2e63 7265 6174 655f 696e 7465 7276  ml.create_interv
-00011730: 616c 5f76 616c 7565 2822 303a 3031 3a30  al_value("0:01:0
-00011740: 302e 3522 2c20 2230 3a30 313a 3030 2e36  0.5", "0:01:00.6
-00011750: 2229 0a20 2020 2020 2020 2022 3630 2e35  ").        "60.5
-00011760: 3a36 302e 3622 0a20 2020 2022 2222 0a20  :60.6".    """. 
-00011770: 2020 2073 7461 7274 5f6d 6174 6368 203d     start_match =
-00011780: 2072 6567 6578 2e73 6561 7263 6828 7222   regex.search(r"
-00011790: 5e28 5c64 2b29 3a28 5b30 2d35 5d5b 302d  ^(\d+):([0-5][0-
-000117a0: 395d 293a 285b 302d 355d 5b30 2d39 5d28  9]):([0-5][0-9](
-000117b0: 3f3a 5c2e 5b30 2d39 5d2b 293f 2924 222c  ?:\.[0-9]+)?)$",
-000117c0: 2073 7461 7274 290a 2020 2020 656e 645f   start).    end_
-000117d0: 6d61 7463 6820 3d20 7265 6765 782e 6d61  match = regex.ma
-000117e0: 7463 6828 7222 5e28 5c64 2b29 3a28 5b30  tch(r"^(\d+):([0
-000117f0: 2d35 5d5b 302d 395d 293a 285b 302d 355d  -5][0-9]):([0-5]
-00011800: 5b30 2d39 5d28 3f3a 5c2e 5b30 2d39 5d2b  [0-9](?:\.[0-9]+
-00011810: 293f 2924 222c 2065 6e64 290a 2020 2020  )?)$", end).    
-00011820: 6966 206e 6f74 2073 7461 7274 5f6d 6174  if not start_mat
-00011830: 6368 206f 7220 6e6f 7420 656e 645f 6d61  ch or not end_ma
-00011840: 7463 683a 0a20 2020 2020 2020 2072 6169  tch:.        rai
-00011850: 7365 2056 616c 7565 4572 726f 7228 2254  se ValueError("T
-00011860: 6865 2073 7461 7274 2061 6e64 2065 6e64  he start and end
-00011870: 2076 616c 7565 7320 6d75 7374 2062 6520   values must be 
-00011880: 696e 2074 6865 2066 6f72 6d61 7420 2748  in the format 'H
-00011890: 2848 293a 4d4d 3a53 5328 2e73 2927 2229  (H):MM:SS(.s)'")
-000118a0: 0a20 2020 2073 7461 7274 5f68 2c20 7374  .    start_h, st
-000118b0: 6172 745f 6d2c 2073 7461 7274 5f73 203d  art_m, start_s =
-000118c0: 2073 7461 7274 5f6d 6174 6368 2e67 726f   start_match.gro
-000118d0: 7570 7328 290a 2020 2020 656e 645f 682c  ups().    end_h,
-000118e0: 2065 6e64 5f6d 2c20 656e 645f 7320 3d20   end_m, end_s = 
-000118f0: 656e 645f 6d61 7463 682e 6772 6f75 7073  end_match.groups
-00011900: 2829 0a20 2020 2073 7461 7274 5f73 6563  ().    start_sec
-00011910: 6f6e 6473 203d 2069 6e74 2873 7461 7274  onds = int(start
-00011920: 5f68 2920 2a20 3336 3030 202b 2069 6e74  _h) * 3600 + int
-00011930: 2873 7461 7274 5f6d 2920 2a20 3630 202b  (start_m) * 60 +
-00011940: 2066 6c6f 6174 2873 7461 7274 5f73 290a   float(start_s).
-00011950: 2020 2020 656e 645f 7365 636f 6e64 7320      end_seconds 
-00011960: 3d20 696e 7428 656e 645f 6829 202a 2033  = int(end_h) * 3
-00011970: 3630 3020 2b20 696e 7428 656e 645f 6d29  600 + int(end_m)
-00011980: 202a 2036 3020 2b20 666c 6f61 7428 656e   * 60 + float(en
-00011990: 645f 7329 0a20 2020 2073 7461 7274 5f73  d_s).    start_s
-000119a0: 6563 6f6e 6473 203d 2069 6e74 2873 7461  econds = int(sta
-000119b0: 7274 5f73 6563 6f6e 6473 2920 6966 2073  rt_seconds) if s
-000119c0: 7461 7274 5f73 6563 6f6e 6473 2e69 735f  tart_seconds.is_
-000119d0: 696e 7465 6765 7228 2920 656c 7365 2073  integer() else s
-000119e0: 7461 7274 5f73 6563 6f6e 6473 0a20 2020  tart_seconds.   
-000119f0: 2065 6e64 5f73 6563 6f6e 6473 203d 2069   end_seconds = i
-00011a00: 6e74 2865 6e64 5f73 6563 6f6e 6473 2920  nt(end_seconds) 
-00011a10: 6966 2065 6e64 5f73 6563 6f6e 6473 2e69  if end_seconds.i
-00011a20: 735f 696e 7465 6765 7228 2920 656c 7365  s_integer() else
-00011a30: 2065 6e64 5f73 6563 6f6e 6473 0a20 2020   end_seconds.   
-00011a40: 2069 6620 7374 6172 745f 7365 636f 6e64   if start_second
-00011a50: 7320 3e20 656e 645f 7365 636f 6e64 733a  s > end_seconds:
-00011a60: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-00011a70: 616c 7565 4572 726f 7228 2254 6865 2073  alueError("The s
-00011a80: 7461 7274 2076 616c 7565 206d 7573 7420  tart value must 
-00011a90: 6265 2073 6d61 6c6c 6572 2074 6861 6e20  be smaller than 
-00011aa0: 7468 6520 656e 6420 7661 6c75 6522 290a  the end value").
-00011ab0: 2020 2020 7265 7475 726e 2066 227b 7374      return f"{st
-00011ac0: 6172 745f 7365 636f 6e64 737d 3a7b 656e  art_seconds}:{en
-00011ad0: 645f 7365 636f 6e64 737d 220a 0a0a 6465  d_seconds}"...de
-00011ae0: 6620 6372 6561 7465 5f6a 736f 6e5f 6578  f create_json_ex
-00011af0: 6365 6c5f 6c69 7374 5f6d 6170 7069 6e67  cel_list_mapping
-00011b00: 280a 2020 2020 7061 7468 5f74 6f5f 6a73  (.    path_to_js
-00011b10: 6f6e 3a20 7374 722c 0a20 2020 206c 6973  on: str,.    lis
-00011b20: 745f 6e61 6d65 3a20 7374 722c 0a20 2020  t_name: str,.   
-00011b30: 2065 7863 656c 5f76 616c 7565 733a 2049   excel_values: I
-00011b40: 7465 7261 626c 655b 7374 725d 2c0a 2020  terable[str],.  
-00011b50: 2020 7365 703a 2073 7472 203d 2027 2b22    sep: str = '+"
-00011b60: 2ac3 a725 262f 2829 3d27 2c0a 2020 2020  *..%&/()=',.    
-00011b70: 636f 7272 6563 7469 6f6e 733a 204f 7074  corrections: Opt
-00011b80: 696f 6e61 6c5b 6469 6374 5b73 7472 2c20  ional[dict[str, 
-00011b90: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2920  str]] = None,.) 
-00011ba0: 2d3e 2064 6963 745b 7374 722c 2073 7472  -> dict[str, str
-00011bb0: 5d3a 0a20 2020 2022 2222 0a20 2020 204f  ]:.    """.    O
-00011bc0: 6674 656e 2c20 6461 7461 2073 6f75 7263  ften, data sourc
-00011bd0: 6573 2063 6f6e 7461 696e 206c 6973 7420  es contain list 
-00011be0: 7661 6c75 6573 2074 6861 7420 6172 656e  values that aren
-00011bf0: 2774 2069 6465 6e74 6963 616c 2074 6f20  't identical to 
-00011c00: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-00011c10: 6e6f 6465 2069 6e20 7468 6520 6c69 7374  node in the list
-00011c20: 206f 6620 7468 6520 4a53 4f4e 0a20 2020   of the JSON.   
-00011c30: 2070 726f 6a65 6374 2066 696c 6520 2863   project file (c
-00011c40: 6f6c 6c6f 7175 6961 6c6c 793a 206f 6e74  olloquially: ont
-00011c50: 6f6c 6f67 7929 2e20 496e 206f 7264 6572  ology). In order
-00011c60: 2074 6f20 6372 6561 7465 2061 2063 6f72   to create a cor
-00011c70: 7265 6374 2058 4d4c 2066 6f72 2074 6865  rect XML for the
-00011c80: 2060 6473 702d 746f 6f6c 7320 786d 6c75   `dsp-tools xmlu
-00011c90: 706c 6f61 6460 2c20 6120 6d61 7070 696e  pload`, a mappin
-00011ca0: 6720 6973 0a20 2020 206e 6563 6573 7361  g is.    necessa
-00011cb0: 7279 2e20 5468 6973 2066 756e 6374 696f  ry. This functio
-00011cc0: 6e20 7461 6b65 7320 6120 4a53 4f4e 206c  n takes a JSON l
-00011cd0: 6973 7420 616e 6420 616e 2045 7863 656c  ist and an Excel
-00011ce0: 2063 6f6c 756d 6e20 636f 6e74 6169 6e69   column containi
-00011cf0: 6e67 206c 6973 742d 7661 6c75 6573 2c20  ng list-values, 
-00011d00: 616e 6420 7472 6965 7320 746f 206d 6174  and tries to mat
-00011d10: 6368 2074 6865 6d0a 2020 2020 6175 746f  ch them.    auto
-00011d20: 6d61 7469 6361 6c6c 7920 6261 7365 6420  matically based 
-00011d30: 6f6e 2073 696d 696c 6172 6974 792e 2054  on similarity. T
-00011d40: 6865 2072 6573 756c 7420 6973 2061 2064  he result is a d
-00011d50: 6963 7420 6f66 2074 6865 2066 6f72 6d20  ict of the form 
-00011d60: 7b65 7863 656c 5f76 616c 7565 3a20 6c69  {excel_value: li
-00011d70: 7374 5f6e 6f64 655f 6e61 6d65 7d2e 0a0a  st_node_name}...
-00011d80: 2020 2020 416c 7465 726e 6174 6976 656c      Alternativel
-00011d90: 792c 2063 6f6e 7369 6465 7220 7573 696e  y, consider usin
-00011da0: 6720 7468 6520 6675 6e63 7469 6f6e 2063  g the function c
-00011db0: 7265 6174 655f 6a73 6f6e 5f6c 6973 745f  reate_json_list_
-00011dc0: 6d61 7070 696e 6728 292c 2077 6869 6368  mapping(), which
-00011dd0: 2061 6c73 6f20 6275 696c 6473 2061 2064   also builds a d
-00011de0: 6963 7469 6f6e 6172 792c 0a20 2020 2062  ictionary,.    b
-00011df0: 7574 2066 726f 6d20 7468 6520 6e61 6d65  ut from the name
-00011e00: 7320 616e 6420 6c61 6265 6c73 2069 6e20  s and labels in 
-00011e10: 7468 6520 4a53 4f4e 206c 6973 742c 2077  the JSON list, w
-00011e20: 6869 6368 2069 7320 6c65 7373 2065 7272  hich is less err
-00011e30: 6f72 2d70 726f 6e65 2074 6861 6e20 7468  or-prone than th
-00011e40: 6973 2066 756e 6374 696f 6e27 7320 6170  is function's ap
-00011e50: 7072 6f61 6368 2e20 486f 7765 7665 722c  proach. However,
-00011e60: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
-00011e70: 6f6e 2068 6173 2074 6865 2061 6476 616e  on has the advan
-00011e80: 7461 6765 2074 6861 7420 6974 2065 7665  tage that it eve
-00011e90: 6e20 776f 726b 7320 7768 656e 2079 6f75  n works when you
-00011ea0: 7220 6461 7461 2073 6f75 7263 6520 646f  r data source do
-00011eb0: 6573 6e27 7420 7573 6520 7468 6520 6c69  esn't use the li
-00011ec0: 7374 206c 6162 656c 7320 636f 7272 6563  st labels correc
-00011ed0: 746c 792e 0a0a 2020 2020 4172 6773 3a0a  tly...    Args:.
-00011ee0: 2020 2020 2020 2020 7061 7468 5f74 6f5f          path_to_
-00011ef0: 6a73 6f6e 3a20 7061 7468 2074 6f20 7468  json: path to th
-00011f00: 6520 4a53 4f4e 2070 726f 6a65 6374 2066  e JSON project f
-00011f10: 696c 650a 2020 2020 2020 2020 6c69 7374  ile.        list
-00011f20: 5f6e 616d 653a 206e 616d 6520 6f66 2074  _name: name of t
-00011f30: 6865 206c 6973 7420 696e 2074 6865 204a  he list in the J
-00011f40: 534f 4e20 7072 6f6a 6563 7420 6669 6c65  SON project file
-00011f50: 2028 6361 6e20 616c 736f 2062 6520 6120   (can also be a 
-00011f60: 6e65 7374 6564 206c 6973 7429 0a20 2020  nested list).   
-00011f70: 2020 2020 2065 7863 656c 5f76 616c 7565       excel_value
-00011f80: 733a 2074 6865 2045 7863 656c 2063 6f6c  s: the Excel col
-00011f90: 756d 6e20 2865 2e67 2e20 6173 206c 6973  umn (e.g. as lis
-00011fa0: 7429 2077 6974 6820 7468 6520 6c69 7374  t) with the list
-00011fb0: 2076 616c 7565 7320 696e 2069 740a 2020   values in it.  
-00011fc0: 2020 2020 2020 7365 703a 2073 6570 6172        sep: separ
-00011fd0: 6174 6f72 2073 7472 696e 672c 2069 6620  ator string, if 
-00011fe0: 7468 6520 6365 6c6c 7320 696e 2074 6865  the cells in the
-00011ff0: 2045 7863 656c 2063 6f6e 7461 696e 206d   Excel contain m
-00012000: 6f72 6520 7468 616e 206f 6e65 206c 6973  ore than one lis
-00012010: 7420 656e 7472 790a 2020 2020 2020 2020  t entry.        
-00012020: 636f 7272 6563 7469 6f6e 733a 2064 6963  corrections: dic
-00012030: 7420 7769 7468 2077 726f 6e67 2065 6e74  t with wrong ent
-00012040: 7269 6573 2c20 6561 6368 2070 6f69 6e74  ries, each point
-00012050: 696e 6720 746f 2069 7473 2063 6f72 7265  ing to its corre
-00012060: 6374 2063 6f75 6e74 6572 7061 7274 0a0a  ct counterpart..
-00012070: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-00012080: 2020 2020 5761 726e 696e 673a 2069 6620      Warning: if 
-00012090: 7468 6572 6520 6973 2061 6e20 4578 6365  there is an Exce
-000120a0: 6c20 7661 6c75 6520 7468 6174 2063 6f75  l value that cou
-000120b0: 6c64 6e27 7420 6265 206d 6174 6368 6564  ldn't be matched
-000120c0: 0a20 2020 2020 2020 2045 7863 6570 7469  .        Excepti
-000120d0: 6f6e 3a20 6966 2074 6865 2070 6174 6820  on: if the path 
-000120e0: 646f 6573 6e27 7420 706f 696e 7420 746f  doesn't point to
-000120f0: 2061 204a 534f 4e20 7072 6f6a 6563 7420   a JSON project 
-00012100: 6669 6c65 0a0a 2020 2020 5265 7475 726e  file..    Return
-00012110: 733a 0a20 2020 2020 2020 2064 6963 7420  s:.        dict 
-00012120: 6f66 2074 6865 2066 6f72 6d20 6060 7b65  of the form ``{e
-00012130: 7863 656c 5f76 616c 7565 3a20 6c69 7374  xcel_value: list
-00012140: 5f6e 6f64 655f 6e61 6d65 7d60 602e 0a20  _node_name}``.. 
-00012150: 2020 2020 2020 2020 2020 2045 7665 7279             Every
-00012160: 2065 7863 656c 5f76 616c 7565 2069 7320   excel_value is 
-00012170: 7374 7269 7070 6564 2c20 616e 6420 616c  stripped, and al
-00012180: 736f 2070 7265 7365 6e74 2069 6e20 6120  so present in a 
-00012190: 6c6f 7765 7263 6173 6520 666f 726d 2e0a  lowercase form..
-000121a0: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
-000121b0: 2020 2020 2020 203e 3e3e 206a 736f 6e5f         >>> json_
-000121c0: 6c69 7374 5f6e 6f64 6573 203d 205b 0a20  list_nodes = [. 
-000121d0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000121e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000121f0: 2020 2020 2022 6e61 6d65 223a 2022 6769       "name": "gi
-00012200: 7261 6666 6522 2c0a 2020 2020 2020 2020  raffe",.        
-00012210: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
-00012220: 656c 7322 3a20 7b22 656e 223a 2022 6769  els": {"en": "gi
-00012230: 7261 6666 6522 7d0a 2020 2020 2020 2020  raffe"}.        
-00012240: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00012250: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-00012260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012270: 2022 6e61 6d65 223a 2022 616e 7465 6c6f   "name": "antelo
-00012280: 7065 222c 0a20 2020 2020 2020 2020 2020  pe",.           
-00012290: 2020 2020 2020 2020 2022 6c61 6265 6c73           "labels
-000122a0: 223a 207b 2265 6e22 3a20 2261 6e74 656c  ": {"en": "antel
-000122b0: 6f70 6522 7d0a 2020 2020 2020 2020 2020  ope"}.          
-000122c0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000122d0: 2020 2020 5d0a 2020 2020 2020 2020 3e3e      ].        >>
-000122e0: 3e20 6578 6365 6c5f 726f 775f 3120 3d20  > excel_row_1 = 
-000122f0: 5b22 4769 7261 6666 6565 6820 222c 2022  ["Giraffeeh ", "
-00012300: 2041 6e74 696c 6f75 7065 222c 2022 4769   Antiloupe", "Gi
-00012310: 7272 6166 6665 202c 2041 6e74 696c 6f75  rraffe , Antilou
-00012320: 7065 2022 5d0a 2020 2020 2020 2020 3e3e  pe "].        >>
-00012330: 3e20 6a73 6f6e 5f65 7863 656c 5f6c 6973  > json_excel_lis
-00012340: 745f 6d61 7070 696e 6720 3d20 7b0a 2020  t_mapping = {.  
-00012350: 2020 2020 2020 2020 2020 2020 2020 2247                "G
-00012360: 6972 6166 6665 6568 223a 2022 6769 7261  iraffeeh": "gira
-00012370: 6666 6522 2c0a 2020 2020 2020 2020 2020  ffe",.          
-00012380: 2020 2020 2020 2267 6972 6166 6665 6568        "giraffeeh
-00012390: 223a 2022 6769 7261 6666 6522 2c0a 2020  ": "giraffe",.  
-000123a0: 2020 2020 2020 2020 2020 2020 2020 2247                "G
-000123b0: 6972 7261 6666 6522 3a20 2267 6972 6166  irraffe": "giraf
-000123c0: 6665 222c 0a20 2020 2020 2020 2020 2020  fe",.           
-000123d0: 2020 2020 2022 6769 7272 6166 6665 223a       "girraffe":
-000123e0: 2022 6769 7261 6666 6522 2c0a 2020 2020   "giraffe",.    
-000123f0: 2020 2020 2020 2020 2020 2020 2241 6e74              "Ant
-00012400: 696c 6f75 7065 223a 2022 616e 7465 6c6f  iloupe": "antelo
-00012410: 7065 222c 0a20 2020 2020 2020 2020 2020  pe",.           
-00012420: 2020 2020 2022 616e 7469 6c6f 7570 6522       "antiloupe"
-00012430: 3a20 2261 6e74 656c 6f70 6522 0a20 2020  : "antelope".   
-00012440: 2020 2020 2020 2020 207d 0a20 2020 2022           }.    "
-00012450: 2222 0a0a 2020 2020 2320 6176 6f69 6420  ""..    # avoid 
-00012460: 6d75 7461 626c 6520 6465 6661 756c 7420  mutable default 
-00012470: 6172 6775 6d65 6e74 0a20 2020 2063 6f72  argument.    cor
-00012480: 7265 6374 696f 6e73 203d 2063 6f72 7265  rections = corre
-00012490: 6374 696f 6e73 206f 7220 7b7d 0a0a 2020  ctions or {}..  
-000124a0: 2020 2320 7370 6c69 7420 7468 6520 7661    # split the va
-000124b0: 6c75 6573 2c20 6966 206e 6563 6573 7361  lues, if necessa
-000124c0: 7279 0a20 2020 2065 7863 656c 5f76 616c  ry.    excel_val
-000124d0: 7565 735f 6e65 7720 3d20 5b5d 0a20 2020  ues_new = [].   
-000124e0: 2066 6f72 2076 616c 2069 6e20 6578 6365   for val in exce
-000124f0: 6c5f 7661 6c75 6573 3a0a 2020 2020 2020  l_values:.      
-00012500: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00012510: 7661 6c2c 2073 7472 293a 0a20 2020 2020  val, str):.     
-00012520: 2020 2020 2020 2065 7863 656c 5f76 616c         excel_val
-00012530: 7565 735f 6e65 772e 6578 7465 6e64 285b  ues_new.extend([
-00012540: 782e 7374 7269 7028 2920 666f 7220 7820  x.strip() for x 
-00012550: 696e 2076 616c 2e73 706c 6974 2873 6570  in val.split(sep
-00012560: 2920 6966 2078 5d29 0a0a 2020 2020 2320  ) if x])..    # 
-00012570: 7265 6164 2074 6865 206c 6973 7420 6f66  read the list of
-00012580: 2074 6865 204a 534f 4e20 7072 6f6a 6563   the JSON projec
-00012590: 7420 2877 6f72 6b73 2061 6c73 6f20 666f  t (works also fo
-000125a0: 7220 6e65 7374 6564 206c 6973 7473 290a  r nested lists).
-000125b0: 2020 2020 7769 7468 206f 7065 6e28 7061      with open(pa
-000125c0: 7468 5f74 6f5f 6a73 6f6e 2c20 656e 636f  th_to_json, enco
-000125d0: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
-000125e0: 2066 3a0a 2020 2020 2020 2020 6a73 6f6e   f:.        json
-000125f0: 5f66 696c 6520 3d20 6a73 6f6e 2e6c 6f61  _file = json.loa
-00012600: 6428 6629 0a20 2020 206a 736f 6e5f 7375  d(f).    json_su
-00012610: 6273 6574 203d 205b 5d0a 2020 2020 666f  bset = [].    fo
-00012620: 7220 656c 656d 2069 6e20 6a73 6f6e 5f66  r elem in json_f
-00012630: 696c 655b 2270 726f 6a65 6374 225d 5b22  ile["project"]["
-00012640: 6c69 7374 7322 5d3a 0a20 2020 2020 2020  lists"]:.       
-00012650: 2069 6620 656c 656d 5b22 6e61 6d65 225d   if elem["name"]
-00012660: 203d 3d20 6c69 7374 5f6e 616d 653a 0a20   == list_name:. 
-00012670: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
-00012680: 7375 6273 6574 203d 2065 6c65 6d5b 226e  subset = elem["n
-00012690: 6f64 6573 225d 0a20 2020 206a 736f 6e5f  odes"].    json_
-000126a0: 7661 6c75 6573 203d 2073 6574 285f 6e65  values = set(_ne
-000126b0: 7374 6564 5f64 6963 745f 7661 6c75 6573  sted_dict_values
-000126c0: 5f69 7465 7261 746f 7228 6a73 6f6e 5f73  _iterator(json_s
-000126d0: 7562 7365 7429 290a 0a20 2020 2023 2062  ubset))..    # b
-000126e0: 7569 6c64 2064 6963 7469 6f6e 6172 7920  uild dictionary 
-000126f0: 7769 7468 2074 6865 206d 6170 7069 6e67  with the mapping
-00012700: 2c20 6261 7365 6420 6f6e 2073 7472 696e  , based on strin
-00012710: 6720 7369 6d69 6c61 7269 7479 0a20 2020  g similarity.   
-00012720: 2072 6573 203d 207b 7d0a 2020 2020 666f   res = {}.    fo
-00012730: 7220 6578 6365 6c5f 7661 6c75 6520 696e  r excel_value in
-00012740: 2065 7863 656c 5f76 616c 7565 735f 6e65   excel_values_ne
-00012750: 773a 0a20 2020 2020 2020 2065 7863 656c  w:.        excel
-00012760: 5f76 616c 7565 5f63 6f72 7265 6374 6564  _value_corrected
-00012770: 203d 2063 6f72 7265 6374 696f 6e73 2e67   = corrections.g
-00012780: 6574 2865 7863 656c 5f76 616c 7565 2c20  et(excel_value, 
-00012790: 6578 6365 6c5f 7661 6c75 6529 0a20 2020  excel_value).   
-000127a0: 2020 2020 2065 7863 656c 5f76 616c 7565       excel_value
-000127b0: 5f73 696d 706c 203d 2073 696d 706c 6966  _simpl = simplif
-000127c0: 795f 6e61 6d65 2865 7863 656c 5f76 616c  y_name(excel_val
-000127d0: 7565 5f63 6f72 7265 6374 6564 2920 2023  ue_corrected)  #
-000127e0: 2069 6e63 7265 6173 6520 6d61 7463 6820   increase match 
-000127f0: 7072 6f62 6162 696c 6974 7920 6279 2072  probability by r
-00012800: 656d 6f76 696e 6720 696c 6c65 6761 6c20  emoving illegal 
-00012810: 6368 6172 730a 2020 2020 2020 2020 6966  chars.        if
-00012820: 206d 6174 6368 6573 203a 3d20 6469 6666   matches := diff
-00012830: 6c69 622e 6765 745f 636c 6f73 655f 6d61  lib.get_close_ma
-00012840: 7463 6865 7328 0a20 2020 2020 2020 2020  tches(.         
-00012850: 2020 2077 6f72 643d 6578 6365 6c5f 7661     word=excel_va
-00012860: 6c75 655f 7369 6d70 6c2c 0a20 2020 2020  lue_simpl,.     
-00012870: 2020 2020 2020 2070 6f73 7369 6269 6c69         possibili
-00012880: 7469 6573 3d6a 736f 6e5f 7661 6c75 6573  ties=json_values
-00012890: 2c0a 2020 2020 2020 2020 2020 2020 6e3d  ,.            n=
-000128a0: 312c 0a20 2020 2020 2020 2020 2020 2063  1,.            c
-000128b0: 7574 6f66 663d 302e 362c 0a20 2020 2020  utoff=0.6,.     
-000128c0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-000128d0: 2020 7265 735b 6578 6365 6c5f 7661 6c75    res[excel_valu
-000128e0: 655d 203d 206d 6174 6368 6573 5b30 5d0a  e] = matches[0].
-000128f0: 2020 2020 2020 2020 2020 2020 7265 735b              res[
-00012900: 6578 6365 6c5f 7661 6c75 652e 6c6f 7765  excel_value.lowe
-00012910: 7228 295d 203d 206d 6174 6368 6573 5b30  r()] = matches[0
-00012920: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-00012930: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
-00012940: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00012950: 2020 2020 6622 4469 6420 6e6f 7420 6669      f"Did not fi
-00012960: 6e64 2061 2063 6c6f 7365 206d 6174 6368  nd a close match
-00012970: 2074 6f20 7468 6520 6578 6365 6c20 6c69   to the excel li
-00012980: 7374 2065 6e74 7279 2027 7b65 7863 656c  st entry '{excel
-00012990: 5f76 616c 7565 7d27 2022 0a20 2020 2020  _value}' ".     
-000129a0: 2020 2020 2020 2020 2020 2066 2261 6d6f             f"amo
-000129b0: 6e67 2074 6865 2076 616c 7565 7320 696e  ng the values in
-000129c0: 2074 6865 204a 534f 4e20 7072 6f6a 6563   the JSON projec
-000129d0: 7420 6c69 7374 2027 7b6c 6973 745f 6e61  t list '{list_na
-000129e0: 6d65 7d27 220a 2020 2020 2020 2020 2020  me}'".          
-000129f0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00012a00: 7761 726e 696e 6773 2e77 6172 6e28 4473  warnings.warn(Ds
-00012a10: 7054 6f6f 6c73 5573 6572 5761 726e 696e  pToolsUserWarnin
-00012a20: 6728 6d73 6729 290a 0a20 2020 2072 6574  g(msg))..    ret
-00012a30: 7572 6e20 7265 730a 0a0a 6465 6620 5f6e  urn res...def _n
-00012a40: 6573 7465 645f 6469 6374 5f76 616c 7565  ested_dict_value
-00012a50: 735f 6974 6572 6174 6f72 2864 6963 7473  s_iterator(dicts
-00012a60: 3a20 6c69 7374 5b64 6963 745b 7374 722c  : list[dict[str,
-00012a70: 2041 6e79 5d5d 2920 2d3e 2049 7465 7261   Any]]) -> Itera
-00012a80: 626c 655b 7374 725d 3a0a 2020 2020 2222  ble[str]:.    ""
-00012a90: 220a 2020 2020 5969 656c 6420 616c 6c20  ".    Yield all 
-00012aa0: 7661 6c75 6573 206f 6620 6120 6e65 7374  values of a nest
-00012ab0: 6564 2064 6963 7469 6f6e 6172 792e 0a0a  ed dictionary...
-00012ac0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00012ad0: 2020 6469 6374 733a 206c 6973 7420 6f66    dicts: list of
-00012ae0: 206e 6573 7465 6420 6469 6374 696f 6e61   nested dictiona
-00012af0: 7269 6573 0a0a 2020 2020 5969 656c 6473  ries..    Yields
-00012b00: 3a0a 2020 2020 2020 2020 7661 6c75 6573  :.        values
-00012b10: 206f 6620 7468 6520 6e65 7374 6564 2064   of the nested d
-00012b20: 6963 7469 6f6e 6172 6965 730a 2020 2020  ictionaries.    
-00012b30: 2222 220a 2020 2020 2320 4372 6564 6974  """.    # Credit
-00012b40: 733a 2068 7474 7073 3a2f 2f74 6869 7370  s: https://thisp
-00012b50: 6f69 6e74 6572 2e63 6f6d 2f70 7974 686f  ointer.com/pytho
-00012b60: 6e2d 6974 6572 6174 652d 6c6f 6f70 2d6f  n-iterate-loop-o
-00012b70: 7665 722d 616c 6c2d 6e65 7374 6564 2d64  ver-all-nested-d
-00012b80: 6963 7469 6f6e 6172 792d 7661 6c75 6573  ictionary-values
-00012b90: 2f0a 2020 2020 666f 7220 5f64 6963 7420  /.    for _dict 
-00012ba0: 696e 2064 6963 7473 3a0a 2020 2020 2020  in dicts:.      
-00012bb0: 2020 6966 2022 6e6f 6465 7322 2069 6e20    if "nodes" in 
-00012bc0: 5f64 6963 743a 0a20 2020 2020 2020 2020  _dict:.         
-00012bd0: 2020 2079 6965 6c64 2066 726f 6d20 5f6e     yield from _n
-00012be0: 6573 7465 645f 6469 6374 5f76 616c 7565  ested_dict_value
-00012bf0: 735f 6974 6572 6174 6f72 285f 6469 6374  s_iterator(_dict
-00012c00: 5b22 6e6f 6465 7322 5d29 0a20 2020 2020  ["nodes"]).     
-00012c10: 2020 2069 6620 226e 616d 6522 2069 6e20     if "name" in 
-00012c20: 5f64 6963 743a 0a20 2020 2020 2020 2020  _dict:.         
-00012c30: 2020 2079 6965 6c64 205f 6469 6374 5b22     yield _dict["
-00012c40: 6e61 6d65 225d 0a0a 0a64 6566 2063 7265  name"]...def cre
-00012c50: 6174 655f 6a73 6f6e 5f6c 6973 745f 6d61  ate_json_list_ma
-00012c60: 7070 696e 6728 0a20 2020 2070 6174 685f  pping(.    path_
-00012c70: 746f 5f6a 736f 6e3a 2073 7472 2c0a 2020  to_json: str,.  
-00012c80: 2020 6c69 7374 5f6e 616d 653a 2073 7472    list_name: str
-00012c90: 2c0a 2020 2020 6c61 6e67 7561 6765 5f6c  ,.    language_l
-00012ca0: 6162 656c 3a20 7374 722c 0a29 202d 3e20  abel: str,.) -> 
-00012cb0: 6469 6374 5b73 7472 2c20 7374 725d 3a0a  dict[str, str]:.
-00012cc0: 2020 2020 2222 220a 2020 2020 4f66 7465      """.    Ofte
-00012cd0: 6e2c 2064 6174 6120 736f 7572 6365 7320  n, data sources 
-00012ce0: 636f 6e74 6169 6e20 6c69 7374 2076 616c  contain list val
-00012cf0: 7565 7320 6e61 6d65 6420 6166 7465 7220  ues named after 
-00012d00: 7468 6520 226c 6162 656c 2220 6f66 2074  the "label" of t
-00012d10: 6865 204a 534f 4e20 7072 6f6a 6563 7420  he JSON project 
-00012d20: 6c69 7374 206e 6f64 652c 2069 6e73 7465  list node, inste
-00012d30: 6164 206f 6620 7468 6520 226e 616d 6522  ad of the "name"
-00012d40: 0a20 2020 2077 6869 6368 2069 7320 6e65  .    which is ne
-00012d50: 6564 6564 2066 6f72 2074 6865 2060 6473  eded for the `ds
-00012d60: 702d 746f 6f6c 7320 786d 6c75 706c 6f61  p-tools xmluploa
-00012d70: 6460 2e20 496e 206f 7264 6572 2074 6f20  d`. In order to 
-00012d80: 6372 6561 7465 2061 2063 6f72 7265 6374  create a correct
-00012d90: 2058 4d4c 2c20 796f 7520 6e65 6564 2061   XML, you need a
-00012da0: 2064 6963 7469 6f6e 6172 7920 7468 6174   dictionary that
-00012db0: 206d 6170 7320 7468 650a 2020 2020 226c   maps the.    "l
-00012dc0: 6162 656c 7322 2074 6f20 7468 6569 7220  abels" to their 
-00012dd0: 636f 7272 6563 7420 226e 616d 6573 222e  correct "names".
-00012de0: 0a0a 2020 2020 416c 7465 726e 6174 6976  ..    Alternativ
-00012df0: 656c 792c 2063 6f6e 7369 6465 7220 7573  ely, consider us
-00012e00: 696e 6720 7468 6520 6d65 7468 6f64 2063  ing the method c
-00012e10: 7265 6174 655f 6a73 6f6e 5f65 7863 656c  reate_json_excel
-00012e20: 5f6c 6973 745f 6d61 7070 696e 6728 292c  _list_mapping(),
-00012e30: 2077 6869 6368 2061 6c73 6f20 6372 6561   which also crea
-00012e40: 7465 7320 6120 6469 6374 696f 6e61 7279  tes a dictionary
-00012e50: 2c20 6275 7420 6d61 7073 0a20 2020 2076  , but maps.    v
-00012e60: 616c 7565 7320 6672 6f6d 2079 6f75 7220  alues from your 
-00012e70: 6461 7461 2073 6f75 7263 6520 746f 206c  data source to l
-00012e80: 6973 7420 6e6f 6465 206e 616d 6573 2066  ist node names f
-00012e90: 726f 6d20 7468 6520 4a53 4f4e 2070 726f  rom the JSON pro
-00012ea0: 6a65 6374 2066 696c 652c 2062 6173 6564  ject file, based
-00012eb0: 206f 6e20 7369 6d69 6c61 7269 7479 2e0a   on similarity..
-00012ec0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00012ed0: 2020 2070 6174 685f 746f 5f6a 736f 6e3a     path_to_json:
-00012ee0: 2070 6174 6820 746f 2061 204a 534f 4e20   path to a JSON 
-00012ef0: 7072 6f6a 6563 7420 6669 6c65 2028 612e  project file (a.
-00012f00: 6b2e 612e 206f 6e74 6f6c 6f67 7929 0a20  k.a. ontology). 
-00012f10: 2020 2020 2020 206c 6973 745f 6e61 6d65         list_name
-00012f20: 3a20 6e61 6d65 206f 6620 6120 6c69 7374  : name of a list
-00012f30: 2069 6e20 7468 6520 4a53 4f4e 2070 726f   in the JSON pro
-00012f40: 6a65 6374 2028 776f 726b 7320 616c 736f  ject (works also
-00012f50: 2066 6f72 206e 6573 7465 6420 6c69 7374   for nested list
-00012f60: 7329 0a20 2020 2020 2020 206c 616e 6775  s).        langu
-00012f70: 6167 655f 6c61 6265 6c3a 2077 6869 6368  age_label: which
-00012f80: 206c 616e 6775 6167 6520 6f66 2074 6865   language of the
-00012f90: 206c 6162 656c 2074 6f20 6368 6f6f 7365   label to choose
-00012fa0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-00012fb0: 2020 2020 2020 2061 2064 6963 7469 6f6e         a diction
-00012fc0: 6172 7920 6f66 2074 6865 2066 6f72 6d20  ary of the form 
-00012fd0: 7b6c 6162 656c 3a20 6e61 6d65 7d0a 2020  {label: name}.  
-00012fe0: 2020 2222 220a 2020 2020 7769 7468 206f    """.    with o
-00012ff0: 7065 6e28 7061 7468 5f74 6f5f 6a73 6f6e  pen(path_to_json
-00013000: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-00013010: 3822 2920 6173 2066 3a0a 2020 2020 2020  8") as f:.      
-00013020: 2020 6a73 6f6e 5f66 696c 6520 3d20 6a73    json_file = js
-00013030: 6f6e 2e6c 6f61 6428 6629 0a20 2020 206a  on.load(f).    j
-00013040: 736f 6e5f 7375 6273 6574 203d 205b 7820  son_subset = [x 
-00013050: 666f 7220 7820 696e 206a 736f 6e5f 6669  for x in json_fi
-00013060: 6c65 5b22 7072 6f6a 6563 7422 5d5b 226c  le["project"]["l
-00013070: 6973 7473 225d 2069 6620 785b 226e 616d  ists"] if x["nam
-00013080: 6522 5d20 3d3d 206c 6973 745f 6e61 6d65  e"] == list_name
-00013090: 5d0a 2020 2020 2320 6a73 6f6e 5f73 7562  ].    # json_sub
-000130a0: 7365 7420 6973 2061 206c 6973 7420 636f  set is a list co
-000130b0: 6e74 6169 6e69 6e67 206f 6e65 2069 7465  ntaining one ite
-000130c0: 6d2c 206e 616d 656c 7920 7468 6520 6a73  m, namely the js
-000130d0: 6f6e 206f 626a 6563 7420 636f 6e74 6169  on object contai
-000130e0: 6e69 6e67 2074 6865 2065 6e74 6972 6520  ning the entire 
-000130f0: 6a73 6f6e 2d6c 6973 740a 0a20 2020 2072  json-list..    r
-00013100: 6573 203d 207b 7d0a 2020 2020 666f 7220  es = {}.    for 
-00013110: 6c61 6265 6c2c 206e 616d 6520 696e 205f  label, name in _
-00013120: 6e61 6d65 5f6c 6162 656c 5f6d 6170 7065  name_label_mappe
-00013130: 725f 6974 6572 6174 6f72 286a 736f 6e5f  r_iterator(json_
-00013140: 7375 6273 6574 2c20 6c61 6e67 7561 6765  subset, language
-00013150: 5f6c 6162 656c 293a 0a20 2020 2020 2020  _label):.       
-00013160: 2069 6620 6e61 6d65 2021 3d20 6c69 7374   if name != list
-00013170: 5f6e 616d 653a 0a20 2020 2020 2020 2020  _name:.         
-00013180: 2020 2072 6573 5b6c 6162 656c 5d20 3d20     res[label] = 
-00013190: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
-000131a0: 2072 6573 5b6c 6162 656c 2e73 7472 6970   res[label.strip
-000131b0: 2829 2e6c 6f77 6572 2829 5d20 3d20 6e61  ().lower()] = na
-000131c0: 6d65 0a0a 2020 2020 7265 7475 726e 2072  me..    return r
-000131d0: 6573 0a0a 0a64 6566 205f 6e61 6d65 5f6c  es...def _name_l
-000131e0: 6162 656c 5f6d 6170 7065 725f 6974 6572  abel_mapper_iter
-000131f0: 6174 6f72 280a 2020 2020 6a73 6f6e 5f73  ator(.    json_s
-00013200: 7562 7365 743a 206c 6973 745b 6469 6374  ubset: list[dict
-00013210: 5b73 7472 2c20 416e 795d 5d2c 0a20 2020  [str, Any]],.   
-00013220: 206c 616e 6775 6167 655f 6c61 6265 6c3a   language_label:
-00013230: 2073 7472 2c0a 2920 2d3e 2049 7465 7261   str,.) -> Itera
-00013240: 626c 655b 7475 706c 655b 7374 722c 2073  ble[tuple[str, s
-00013250: 7472 5d5d 3a0a 2020 2020 2222 220a 2020  tr]]:.    """.  
-00013260: 2020 476f 2074 6872 6f75 6768 206c 6973    Go through lis
-00013270: 7420 6e6f 6465 7320 6f66 2061 204a 534f  t nodes of a JSO
-00013280: 4e20 7072 6f6a 6563 7420 616e 6420 7969  N project and yi
-00013290: 656c 6420 286c 6162 656c 2c20 6e61 6d65  eld (label, name
-000132a0: 2920 7061 6972 732e 0a0a 2020 2020 4172  ) pairs...    Ar
-000132b0: 6773 3a0a 2020 2020 2020 2020 6a73 6f6e  gs:.        json
-000132c0: 5f73 7562 7365 743a 206c 6973 7420 6f66  _subset: list of
-000132d0: 2044 5350 206c 6973 7473 2028 6120 4453   DSP lists (a DS
-000132e0: 5020 6c69 7374 2062 6569 6e67 2061 2064  P list being a d
-000132f0: 6963 7469 6f6e 6172 7920 7769 7468 2074  ictionary with t
-00013300: 6865 206b 6579 7320 226e 616d 6522 2c20  he keys "name", 
-00013310: 226c 6162 656c 7322 2061 6e64 2022 6e6f  "labels" and "no
-00013320: 6465 7322 290a 2020 2020 2020 2020 6c61  des").        la
-00013330: 6e67 7561 6765 5f6c 6162 656c 3a20 7768  nguage_label: wh
-00013340: 6963 6820 6c61 6e67 7561 6765 206f 6620  ich language of 
-00013350: 7468 6520 6c61 6265 6c20 746f 2063 686f  the label to cho
-00013360: 6f73 650a 0a20 2020 2059 6965 6c64 733a  ose..    Yields:
-00013370: 0a20 2020 2020 2020 2028 6c61 6265 6c2c  .        (label,
-00013380: 206e 616d 6529 2070 6169 7273 0a20 2020   name) pairs.   
-00013390: 2022 2222 0a20 2020 2066 6f72 206e 6f64   """.    for nod
-000133a0: 6520 696e 206a 736f 6e5f 7375 6273 6574  e in json_subset
-000133b0: 3a0a 2020 2020 2020 2020 2320 6e6f 6465  :.        # node
-000133c0: 2069 7320 7468 6520 6a73 6f6e 206f 626a   is the json obj
-000133d0: 6563 7420 636f 6e74 6169 6e69 6e67 2074  ect containing t
-000133e0: 6865 2065 6e74 6972 6520 6a73 6f6e 2d6c  he entire json-l
-000133f0: 6973 740a 2020 2020 2020 2020 6966 2022  ist.        if "
-00013400: 6e6f 6465 7322 2069 6e20 6e6f 6465 3a0a  nodes" in node:.
-00013410: 2020 2020 2020 2020 2020 2020 2320 226e              # "n
-00013420: 6f64 6573 2220 6973 2074 6865 206a 736f  odes" is the jso
-00013430: 6e20 7375 622d 6f62 6a65 6374 2063 6f6e  n sub-object con
-00013440: 7461 696e 696e 6720 7468 6520 656e 7472  taining the entr
-00013450: 6965 7320 6f66 2074 6865 206a 736f 6e2d  ies of the json-
-00013460: 6c69 7374 0a20 2020 2020 2020 2020 2020  list.           
-00013470: 2079 6965 6c64 2066 726f 6d20 5f6e 616d   yield from _nam
-00013480: 655f 6c61 6265 6c5f 6d61 7070 6572 5f69  e_label_mapper_i
-00013490: 7465 7261 746f 7228 6e6f 6465 5b22 6e6f  terator(node["no
-000134a0: 6465 7322 5d2c 206c 616e 6775 6167 655f  des"], language_
-000134b0: 6c61 6265 6c29 0a20 2020 2020 2020 2020  label).         
-000134c0: 2020 2023 2065 6163 6820 7969 656c 6465     # each yielde
-000134d0: 6420 7661 6c75 6520 6973 2061 2028 6c61  d value is a (la
-000134e0: 6265 6c2c 206e 616d 6529 2070 6169 7220  bel, name) pair 
-000134f0: 6f66 2061 2073 696e 676c 6520 6c69 7374  of a single list
-00013500: 2065 6e74 7279 0a20 2020 2020 2020 2069   entry.        i
-00013510: 6620 226e 616d 6522 2069 6e20 6e6f 6465  f "name" in node
-00013520: 3a0a 2020 2020 2020 2020 2020 2020 7969  :.            yi
-00013530: 656c 6420 286e 6f64 655b 226c 6162 656c  eld (node["label
-00013540: 7322 5d5b 6c61 6e67 7561 6765 5f6c 6162  s"][language_lab
-00013550: 656c 5d2c 206e 6f64 655b 226e 616d 6522  el], node["name"
-00013560: 5d29 0a20 2020 2020 2020 2020 2020 2023  ]).            #
-00013570: 2074 6865 2061 6374 7561 6c20 7661 6c75   the actual valu
-00013580: 6573 206f 6620 7468 6520 6e61 6d65 2061  es of the name a
-00013590: 6e64 2074 6865 206c 6162 656c 0a0a 0a64  nd the label...d
-000135a0: 6566 2077 7269 7465 5f78 6d6c 280a 2020  ef write_xml(.  
-000135b0: 2020 726f 6f74 3a20 6574 7265 652e 5f45    root: etree._E
-000135c0: 6c65 6d65 6e74 2c0a 2020 2020 6669 6c65  lement,.    file
-000135d0: 7061 7468 3a20 7374 7220 7c20 5061 7468  path: str | Path
-000135e0: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
-000135f0: 2022 2222 0a20 2020 2057 7269 7465 2074   """.    Write t
-00013600: 6865 2066 696e 6973 6865 6420 584d 4c20  he finished XML 
-00013610: 746f 2061 2066 696c 652e 0a0a 2020 2020  to a file...    
-00013620: 4172 6773 3a0a 2020 2020 2020 2020 726f  Args:.        ro
-00013630: 6f74 3a20 6574 7265 6520 456c 656d 656e  ot: etree Elemen
-00013640: 7420 7769 7468 2074 6865 2065 6e74 6972  t with the entir
-00013650: 6520 584d 4c20 646f 6375 6d65 6e74 0a20  e XML document. 
-00013660: 2020 2020 2020 2066 696c 6570 6174 683a         filepath:
-00013670: 2077 6865 7265 2074 6f20 7361 7665 2074   where to save t
-00013680: 6865 2066 696c 650a 0a20 2020 2057 6172  he file..    War
-00013690: 6e69 6e67 3a0a 2020 2020 2020 2020 6966  ning:.        if
-000136a0: 2074 6865 2058 4d4c 2069 7320 6e6f 7420   the XML is not 
-000136b0: 7661 6c69 6420 6163 636f 7264 696e 6720  valid according 
-000136c0: 746f 2074 6865 2073 6368 656d 610a 2020  to the schema.  
-000136d0: 2020 2222 220a 2020 2020 6574 7265 652e    """.    etree.
-000136e0: 696e 6465 6e74 2872 6f6f 742c 2073 7061  indent(root, spa
-000136f0: 6365 3d22 2020 2020 2229 0a20 2020 2078  ce="    ").    x
-00013700: 6d6c 5f73 7472 696e 6720 3d20 6574 7265  ml_string = etre
-00013710: 652e 746f 7374 7269 6e67 280a 2020 2020  e.tostring(.    
-00013720: 2020 2020 726f 6f74 2c0a 2020 2020 2020      root,.      
-00013730: 2020 656e 636f 6469 6e67 3d22 756e 6963    encoding="unic
-00013740: 6f64 6522 2c0a 2020 2020 2020 2020 7072  ode",.        pr
-00013750: 6574 7479 5f70 7269 6e74 3d54 7275 652c  etty_print=True,
-00013760: 0a20 2020 2020 2020 2064 6f63 7479 7065  .        doctype
-00013770: 3d27 3c3f 786d 6c20 7665 7273 696f 6e3d  ='<?xml version=
-00013780: 2231 2e30 2220 656e 636f 6469 6e67 3d22  "1.0" encoding="
-00013790: 5554 462d 3822 3f3e 272c 0a20 2020 2029  UTF-8"?>',.    )
-000137a0: 0a20 2020 2078 6d6c 5f73 7472 696e 6720  .    xml_string 
-000137b0: 3d20 786d 6c5f 7374 7269 6e67 2e72 6570  = xml_string.rep
-000137c0: 6c61 6365 2872 225c 2722 2c20 2227 2229  lace(r"\'", "'")
-000137d0: 0a20 2020 2077 6974 6820 6f70 656e 2866  .    with open(f
-000137e0: 696c 6570 6174 682c 2022 7722 2c20 656e  ilepath, "w", en
-000137f0: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-00013800: 6173 2066 3a0a 2020 2020 2020 2020 662e  as f:.        f.
-00013810: 7772 6974 6528 786d 6c5f 7374 7269 6e67  write(xml_string
-00013820: 290a 2020 2020 7472 793a 0a20 2020 2020  ).    try:.     
-00013830: 2020 2076 616c 6964 6174 655f 786d 6c28     validate_xml(
-00013840: 696e 7075 745f 6669 6c65 3d66 696c 6570  input_file=filep
-00013850: 6174 6829 0a20 2020 2020 2020 2070 7269  ath).        pri
-00013860: 6e74 2866 2254 6865 2058 4d4c 2066 696c  nt(f"The XML fil
-00013870: 6520 7761 7320 7375 6363 6573 7366 756c  e was successful
-00013880: 6c79 2073 6176 6564 2074 6f20 7b66 696c  ly saved to {fil
-00013890: 6570 6174 687d 2229 0a20 2020 2065 7863  epath}").    exc
-000138a0: 6570 7420 4261 7365 4572 726f 7220 6173  ept BaseError as
-000138b0: 2065 7272 3a0a 2020 2020 2020 2020 6d73   err:.        ms
-000138c0: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
-000138d0: 2020 6622 5468 6520 584d 4c20 6669 6c65    f"The XML file
-000138e0: 2077 6173 2073 7563 6365 7373 6675 6c6c   was successfull
-000138f0: 7920 7361 7665 6420 746f 207b 6669 6c65  y saved to {file
-00013900: 7061 7468 7d2c 2022 0a20 2020 2020 2020  path}, ".       
-00013910: 2020 2020 2066 2262 7574 2074 6865 2066       f"but the f
-00013920: 6f6c 6c6f 7769 6e67 2053 6368 656d 6120  ollowing Schema 
-00013930: 7661 6c69 6461 7469 6f6e 2065 7272 6f72  validation error
-00013940: 2873 2920 6f63 6375 7272 6564 3a20 7b65  (s) occurred: {e
-00013950: 7272 2e6d 6573 7361 6765 7d22 0a20 2020  rr.message}".   
-00013960: 2020 2020 2029 0a20 2020 2020 2020 2077       ).        w
-00013970: 6172 6e69 6e67 732e 7761 726e 2844 7370  arnings.warn(Dsp
-00013980: 546f 6f6c 7355 7365 7257 6172 6e69 6e67  ToolsUserWarning
-00013990: 286d 7367 2929 0a                        (msg)).
+0000eeb0: 203c 7572 6920 7065 726d 6973 7369 6f6e   <uri permission
+0000eec0: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
+0000eed0: 3e77 7777 2e32 2e63 6f6d 3c2f 7572 693e  >www.2.com</uri>
+0000eee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eef0: 203c 2f75 7269 2d70 726f 703e 0a0a 2020   </uri-prop>..  
+0000ef00: 2020 5365 6520 6874 7470 733a 2f2f 646f    See https://do
+0000ef10: 6373 2e64 6173 6368 2e73 7769 7373 2f6c  cs.dasch.swiss/l
+0000ef20: 6174 6573 742f 4453 502d 544f 4f4c 532f  atest/DSP-TOOLS/
+0000ef30: 6669 6c65 2d66 6f72 6d61 7473 2f78 6d6c  file-formats/xml
+0000ef40: 2d64 6174 612d 6669 6c65 2f23 7572 692d  -data-file/#uri-
+0000ef50: 7072 6f70 0a20 2020 2022 2222 0a0a 2020  prop.    """..  
+0000ef60: 2020 2320 6368 6563 6b20 7468 6520 696e    # check the in
+0000ef70: 7075 743a 2070 7265 7061 7265 2061 206c  put: prepare a l
+0000ef80: 6973 7420 7769 7468 2076 616c 6964 2076  ist with valid v
+0000ef90: 616c 7565 730a 2020 2020 7661 6c75 6573  alues.    values
+0000efa0: 203d 2070 7265 7061 7265 5f76 616c 7565   = prepare_value
+0000efb0: 2876 616c 7565 290a 0a20 2020 2023 2063  (value)..    # c
+0000efc0: 6865 636b 2076 616c 7565 2074 7970 650a  heck value type.
+0000efd0: 2020 2020 666f 7220 7661 6c20 696e 2076      for val in v
+0000efe0: 616c 7565 733a 0a20 2020 2020 2020 2069  alues:.        i
+0000eff0: 6620 6e6f 7420 6973 5f75 7269 2873 7472  f not is_uri(str
+0000f000: 2876 616c 2e76 616c 7565 2929 3a0a 2020  (val.value)):.  
+0000f010: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
+0000f020: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000f030: 2020 6622 4661 696c 6564 2076 616c 6964    f"Failed valid
+0000f040: 6174 696f 6e20 696e 2072 6573 6f75 7263  ation in resourc
+0000f050: 6520 277b 6361 6c6c 696e 675f 7265 736f  e '{calling_reso
+0000f060: 7572 6365 7d27 2c20 7072 6f70 6572 7479  urce}', property
+0000f070: 2027 7b6e 616d 657d 273a 2022 0a20 2020   '{name}': ".   
+0000f080: 2020 2020 2020 2020 2020 2020 2066 2227               f"'
+0000f090: 7b76 616c 2e76 616c 7565 7d27 2069 7320  {val.value}' is 
+0000f0a0: 6e6f 7420 6120 7661 6c69 6420 5552 492e  not a valid URI.
+0000f0b0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+0000f0c0: 2020 2020 2020 2020 2020 2020 7761 726e              warn
+0000f0d0: 696e 6773 2e77 6172 6e28 4473 7054 6f6f  ings.warn(DspToo
+0000f0e0: 6c73 5573 6572 5761 726e 696e 6728 6d73  lsUserWarning(ms
+0000f0f0: 6729 290a 0a20 2020 2023 206d 616b 6520  g))..    # make 
+0000f100: 786d 6c20 7374 7275 6374 7572 6520 6f66  xml structure of
+0000f110: 2074 6865 2076 616c 6964 2076 616c 7565   the valid value
+0000f120: 730a 2020 2020 7072 6f70 5f20 3d20 6574  s.    prop_ = et
+0000f130: 7265 652e 456c 656d 656e 7428 0a20 2020  ree.Element(.   
+0000f140: 2020 2020 2022 7b25 737d 7572 692d 7072       "{%s}uri-pr
+0000f150: 6f70 2220 2520 786d 6c5f 6e61 6d65 7370  op" % xml_namesp
+0000f160: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
+0000f170: 2020 2020 2020 206e 616d 653d 6e61 6d65         name=name
+0000f180: 2c0a 2020 2020 2020 2020 6e73 6d61 703d  ,.        nsmap=
+0000f190: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
+0000f1a0: 702c 0a20 2020 2029 0a20 2020 2066 6f72  p,.    ).    for
+0000f1b0: 2076 616c 2069 6e20 7661 6c75 6573 3a0a   val in values:.
+0000f1c0: 2020 2020 2020 2020 6b77 6172 6773 203d          kwargs =
+0000f1d0: 207b 2270 6572 6d69 7373 696f 6e73 223a   {"permissions":
+0000f1e0: 2076 616c 2e70 6572 6d69 7373 696f 6e73   val.permissions
+0000f1f0: 7d0a 2020 2020 2020 2020 6966 2076 616c  }.        if val
+0000f200: 2e63 6f6d 6d65 6e74 2061 6e64 2063 6865  .comment and che
+0000f210: 636b 5f6e 6f74 6e61 2876 616c 2e63 6f6d  ck_notna(val.com
+0000f220: 6d65 6e74 293a 0a20 2020 2020 2020 2020  ment):.         
+0000f230: 2020 206b 7761 7267 735b 2263 6f6d 6d65     kwargs["comme
+0000f240: 6e74 225d 203d 2076 616c 2e63 6f6d 6d65  nt"] = val.comme
+0000f250: 6e74 0a20 2020 2020 2020 2076 616c 7565  nt.        value
+0000f260: 5f20 3d20 6574 7265 652e 456c 656d 656e  _ = etree.Elemen
+0000f270: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
+0000f280: 7b25 737d 7572 6922 2025 2078 6d6c 5f6e  {%s}uri" % xml_n
+0000f290: 616d 6573 7061 6365 5f6d 6170 5b4e 6f6e  amespace_map[Non
+0000f2a0: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
+0000f2b0: 2a2a 6b77 6172 6773 2c20 2023 2074 7970  **kwargs,  # typ
+0000f2c0: 653a 2069 676e 6f72 655b 6172 672d 7479  e: ignore[arg-ty
+0000f2d0: 7065 5d0a 2020 2020 2020 2020 2020 2020  pe].            
+0000f2e0: 6e73 6d61 703d 786d 6c5f 6e61 6d65 7370  nsmap=xml_namesp
+0000f2f0: 6163 655f 6d61 702c 0a20 2020 2020 2020  ace_map,.       
+0000f300: 2029 0a20 2020 2020 2020 2076 616c 7565   ).        value
+0000f310: 5f2e 7465 7874 203d 2073 7472 2876 616c  _.text = str(val
+0000f320: 2e76 616c 7565 290a 2020 2020 2020 2020  .value).        
+0000f330: 7072 6f70 5f2e 6170 7065 6e64 2876 616c  prop_.append(val
+0000f340: 7565 5f29 0a0a 2020 2020 7265 7475 726e  ue_)..    return
+0000f350: 2070 726f 705f 0a0a 0a64 6566 206d 616b   prop_...def mak
+0000f360: 655f 7265 6769 6f6e 2820 2023 206e 6f71  e_region(  # noq
+0000f370: 613a 2044 3431 3720 2875 6e64 6f63 756d  a: D417 (undocum
+0000f380: 656e 7465 642d 7061 7261 6d29 0a20 2020  ented-param).   
+0000f390: 206c 6162 656c 3a20 7374 722c 0a20 2020   label: str,.   
+0000f3a0: 2069 643a 2073 7472 2c0a 2020 2020 7065   id: str,.    pe
+0000f3b0: 726d 6973 7369 6f6e 733a 2073 7472 203d  rmissions: str =
+0000f3c0: 2022 7265 732d 6465 6661 756c 7422 2c0a   "res-default",.
+0000f3d0: 2020 2020 6172 6b3a 204f 7074 696f 6e61      ark: Optiona
+0000f3e0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+0000f3f0: 2020 2069 7269 3a20 4f70 7469 6f6e 616c     iri: Optional
+0000f400: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000f410: 2020 6372 6561 7469 6f6e 5f64 6174 653a    creation_date:
+0000f420: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0000f430: 204e 6f6e 652c 0a29 202d 3e20 6574 7265   None,.) -> etre
+0000f440: 652e 5f45 6c65 6d65 6e74 3a0a 2020 2020  e._Element:.    
+0000f450: 2222 220a 2020 2020 4372 6561 7465 7320  """.    Creates 
+0000f460: 616e 2065 6d70 7479 2072 6567 696f 6e20  an empty region 
+0000f470: 656c 656d 656e 742c 2077 6974 6820 7468  element, with th
+0000f480: 6520 6174 7472 6962 7574 6573 2061 7320  e attributes as 
+0000f490: 7370 6563 6966 6965 6420 6279 2074 6865  specified by the
+0000f4a0: 2061 7267 756d 656e 7473 0a0a 2020 2020   arguments..    
+0000f4b0: 4172 6773 3a0a 2020 2020 2020 2020 5468  Args:.        Th
+0000f4c0: 6520 6172 6775 6d65 6e74 7320 636f 7272  e arguments corr
+0000f4d0: 6573 706f 6e64 2031 3a31 2074 6f20 7468  espond 1:1 to th
+0000f4e0: 6520 6174 7472 6962 7574 6573 206f 6620  e attributes of 
+0000f4f0: 7468 6520 3c72 6567 696f 6e3e 2065 6c65  the <region> ele
+0000f500: 6d65 6e74 2e0a 0a20 2020 2052 6169 7365  ment...    Raise
+0000f510: 733a 0a20 2020 2020 2020 2057 6172 6e69  s:.        Warni
+0000f520: 6e67 3a20 6966 2062 6f74 6820 616e 2041  ng: if both an A
+0000f530: 524b 2061 6e64 2061 6e20 4952 4920 6172  RK and an IRI ar
+0000f540: 6520 7072 6f76 6964 6564 0a20 2020 2020  e provided.     
+0000f550: 2020 2042 6173 6545 7272 6f72 3a20 6966     BaseError: if
+0000f560: 2074 6865 2063 7265 6174 696f 6e20 6461   the creation da
+0000f570: 7465 2069 7320 696e 7661 6c69 640a 0a20  te is invalid.. 
+0000f580: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000f590: 2020 2020 5468 6520 7265 6769 6f6e 2065      The region e
+0000f5a0: 6c65 6d65 6e74 2c20 7769 7468 6f75 7420  lement, without 
+0000f5b0: 616e 7920 6368 696c 6472 656e 2c20 6275  any children, bu
+0000f5c0: 7420 7769 7468 2074 6865 2061 7474 7269  t with the attri
+0000f5d0: 6275 7465 733a 0a20 2020 2020 2020 203c  butes:.        <
+0000f5e0: 7265 6769 6f6e 206c 6162 656c 3d6c 6162  region label=lab
+0000f5f0: 656c 2069 643d 6964 2070 6572 6d69 7373  el id=id permiss
+0000f600: 696f 6e73 3d70 6572 6d69 7373 696f 6e73  ions=permissions
+0000f610: 2061 726b 3d61 726b 2069 7269 3d69 7269   ark=ark iri=iri
+0000f620: 3e3c 2f72 6567 696f 6e3e 0a0a 2020 2020  ></region>..    
+0000f630: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
+0000f640: 2020 3e3e 3e20 7265 6769 6f6e 203d 2065    >>> region = e
+0000f650: 7863 656c 3278 6d6c 2e6d 616b 655f 7265  xcel2xml.make_re
+0000f660: 6769 6f6e 2822 6c61 6265 6c22 2c20 2269  gion("label", "i
+0000f670: 6422 290a 2020 2020 2020 2020 3e3e 3e20  d").        >>> 
+0000f680: 7265 6769 6f6e 2e61 7070 656e 6428 6578  region.append(ex
+0000f690: 6365 6c32 786d 6c2e 6d61 6b65 5f74 6578  cel2xml.make_tex
+0000f6a0: 745f 7072 6f70 2822 6861 7343 6f6d 6d65  t_prop("hasComme
+0000f6b0: 6e74 222c 2022 5468 6973 2069 7320 6120  nt", "This is a 
+0000f6c0: 636f 6d6d 656e 7422 2929 0a20 2020 2020  comment")).     
+0000f6d0: 2020 203e 3e3e 2072 6567 696f 6e2e 6170     >>> region.ap
+0000f6e0: 7065 6e64 2865 7863 656c 3278 6d6c 2e6d  pend(excel2xml.m
+0000f6f0: 616b 655f 636f 6c6f 725f 7072 6f70 2822  ake_color_prop("
+0000f700: 6861 7343 6f6c 6f72 222c 2022 2335 6431  hasColor", "#5d1
+0000f710: 6631 6522 2929 0a20 2020 2020 2020 203e  f1e")).        >
+0000f720: 3e3e 2072 6567 696f 6e2e 6170 7065 6e64  >> region.append
+0000f730: 2865 7863 656c 3278 6d6c 2e6d 616b 655f  (excel2xml.make_
+0000f740: 7265 7370 7472 5f70 726f 7028 2269 7352  resptr_prop("isR
+0000f750: 6567 696f 6e4f 6622 2c20 2269 6d61 6765  egionOf", "image
+0000f760: 5f30 2229 290a 2020 2020 2020 2020 3e3e  _0")).        >>
+0000f770: 3e20 7265 6769 6f6e 2e61 7070 656e 6428  > region.append(
+0000f780: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f67  excel2xml.make_g
+0000f790: 656f 6d65 7472 795f 7072 6f70 2822 6861  eometry_prop("ha
+0000f7a0: 7347 656f 6d65 7472 7922 2c20 227b 2e2e  sGeometry", "{..
+0000f7b0: 2e7d 2229 290a 2020 2020 2020 2020 3e3e  .}")).        >>
+0000f7c0: 3e20 726f 6f74 2e61 7070 656e 6428 7265  > root.append(re
+0000f7d0: 6769 6f6e 290a 0a20 2020 2053 6565 2068  gion)..    See h
+0000f7e0: 7474 7073 3a2f 2f64 6f63 732e 6461 7363  ttps://docs.dasc
+0000f7f0: 682e 7377 6973 732f 6c61 7465 7374 2f44  h.swiss/latest/D
+0000f800: 5350 2d54 4f4f 4c53 2f66 696c 652d 666f  SP-TOOLS/file-fo
+0000f810: 726d 6174 732f 786d 6c2d 6461 7461 2d66  rmats/xml-data-f
+0000f820: 696c 652f 2372 6567 696f 6e0a 2020 2020  ile/#region.    
+0000f830: 2222 220a 0a20 2020 206b 7761 7267 7320  """..    kwargs 
+0000f840: 3d20 7b22 6c61 6265 6c22 3a20 6c61 6265  = {"label": labe
+0000f850: 6c2c 2022 6964 223a 2069 642c 2022 7065  l, "id": id, "pe
+0000f860: 726d 6973 7369 6f6e 7322 3a20 7065 726d  rmissions": perm
+0000f870: 6973 7369 6f6e 732c 2022 6e73 6d61 7022  issions, "nsmap"
+0000f880: 3a20 786d 6c5f 6e61 6d65 7370 6163 655f  : xml_namespace_
+0000f890: 6d61 707d 0a20 2020 2069 6620 6172 6b3a  map}.    if ark:
+0000f8a0: 0a20 2020 2020 2020 206b 7761 7267 735b  .        kwargs[
+0000f8b0: 2261 726b 225d 203d 2061 726b 0a20 2020  "ark"] = ark.   
+0000f8c0: 2069 6620 6972 693a 0a20 2020 2020 2020   if iri:.       
+0000f8d0: 206b 7761 7267 735b 2269 7269 225d 203d   kwargs["iri"] =
+0000f8e0: 2069 7269 0a20 2020 2069 6620 6172 6b20   iri.    if ark 
+0000f8f0: 616e 6420 6972 693a 0a20 2020 2020 2020  and iri:.       
+0000f900: 206d 7367 203d 2066 2242 6f74 6820 4152   msg = f"Both AR
+0000f910: 4b20 616e 6420 4952 4920 7765 7265 2070  K and IRI were p
+0000f920: 726f 7669 6465 6420 666f 7220 7265 736f  rovided for reso
+0000f930: 7572 6365 2027 7b6c 6162 656c 7d27 2028  urce '{label}' (
+0000f940: 7b69 647d 292e 2054 6865 2041 524b 2077  {id}). The ARK w
+0000f950: 696c 6c20 6f76 6572 7269 6465 2074 6865  ill override the
+0000f960: 2049 5249 2e22 0a20 2020 2020 2020 2077   IRI.".        w
+0000f970: 6172 6e69 6e67 732e 7761 726e 2844 7370  arnings.warn(Dsp
+0000f980: 546f 6f6c 7355 7365 7257 6172 6e69 6e67  ToolsUserWarning
+0000f990: 286d 7367 2929 0a20 2020 2069 6620 6372  (msg)).    if cr
+0000f9a0: 6561 7469 6f6e 5f64 6174 653a 0a20 2020  eation_date:.   
+0000f9b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000f9c0: 2020 2020 2020 4461 7465 5469 6d65 5374        DateTimeSt
+0000f9d0: 616d 7028 6372 6561 7469 6f6e 5f64 6174  amp(creation_dat
+0000f9e0: 6529 0a20 2020 2020 2020 2065 7863 6570  e).        excep
+0000f9f0: 7420 4261 7365 4572 726f 723a 0a20 2020  t BaseError:.   
+0000fa00: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
+0000fa10: 6173 6545 7272 6f72 280a 2020 2020 2020  aseError(.      
+0000fa20: 2020 2020 2020 2020 2020 6622 5468 6520            f"The 
+0000fa30: 7265 6769 6f6e 2027 7b6c 6162 656c 7d27  region '{label}'
+0000fa40: 2028 4944 3a20 7b69 647d 2920 6861 7320   (ID: {id}) has 
+0000fa50: 616e 2069 6e76 616c 6964 2063 7265 6174  an invalid creat
+0000fa60: 696f 6e20 6461 7465 2027 7b63 7265 6174  ion date '{creat
+0000fa70: 696f 6e5f 6461 7465 7d27 2e20 220a 2020  ion_date}'. ".  
+0000fa80: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000fa90: 4469 6420 796f 7520 7065 7268 6170 7320  Did you perhaps 
+0000faa0: 666f 7267 6574 2074 6865 2074 696d 657a  forget the timez
+0000fab0: 6f6e 653f 220a 2020 2020 2020 2020 2020  one?".          
+0000fac0: 2020 2920 6672 6f6d 204e 6f6e 650a 2020    ) from None.  
+0000fad0: 2020 2020 2020 6b77 6172 6773 5b22 6372        kwargs["cr
+0000fae0: 6561 7469 6f6e 5f64 6174 6522 5d20 3d20  eation_date"] = 
+0000faf0: 6372 6561 7469 6f6e 5f64 6174 650a 0a20  creation_date.. 
+0000fb00: 2020 2072 6574 7572 6e20 6574 7265 652e     return etree.
+0000fb10: 456c 656d 656e 7428 0a20 2020 2020 2020  Element(.       
+0000fb20: 2022 7b25 737d 7265 6769 6f6e 2220 2520   "{%s}region" % 
+0000fb30: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
+0000fb40: 705b 4e6f 6e65 5d2c 0a20 2020 2020 2020  p[None],.       
+0000fb50: 202a 2a6b 7761 7267 732c 2020 2320 7479   **kwargs,  # ty
+0000fb60: 7065 3a20 6967 6e6f 7265 5b61 7267 2d74  pe: ignore[arg-t
+0000fb70: 7970 655d 0a20 2020 2029 0a0a 0a64 6566  ype].    )...def
+0000fb80: 206d 616b 655f 616e 6e6f 7461 7469 6f6e   make_annotation
+0000fb90: 2820 2023 206e 6f71 613a 2044 3431 3720  (  # noqa: D417 
+0000fba0: 2875 6e64 6f63 756d 656e 7465 642d 7061  (undocumented-pa
+0000fbb0: 7261 6d29 0a20 2020 206c 6162 656c 3a20  ram).    label: 
+0000fbc0: 7374 722c 0a20 2020 2069 643a 2073 7472  str,.    id: str
+0000fbd0: 2c0a 2020 2020 7065 726d 6973 7369 6f6e  ,.    permission
+0000fbe0: 733a 2073 7472 203d 2022 7265 732d 6465  s: str = "res-de
+0000fbf0: 6661 756c 7422 2c0a 2020 2020 6172 6b3a  fault",.    ark:
+0000fc00: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0000fc10: 204e 6f6e 652c 0a20 2020 2069 7269 3a20   None,.    iri: 
+0000fc20: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000fc30: 4e6f 6e65 2c0a 2020 2020 6372 6561 7469  None,.    creati
+0000fc40: 6f6e 5f64 6174 653a 204f 7074 696f 6e61  on_date: Optiona
+0000fc50: 6c5b 7374 725d 203d 204e 6f6e 652c 0a29  l[str] = None,.)
+0000fc60: 202d 3e20 6574 7265 652e 5f45 6c65 6d65   -> etree._Eleme
+0000fc70: 6e74 3a0a 2020 2020 2222 220a 2020 2020  nt:.    """.    
+0000fc80: 4372 6561 7465 7320 616e 2065 6d70 7479  Creates an empty
+0000fc90: 2061 6e6e 6f74 6174 696f 6e20 656c 656d   annotation elem
+0000fca0: 656e 742c 2077 6974 6820 7468 6520 6174  ent, with the at
+0000fcb0: 7472 6962 7574 6573 2061 7320 7370 6563  tributes as spec
+0000fcc0: 6966 6965 6420 6279 2074 6865 2061 7267  ified by the arg
+0000fcd0: 756d 656e 7473 0a0a 2020 2020 4172 6773  uments..    Args
+0000fce0: 3a0a 2020 2020 2020 2020 5468 6520 6172  :.        The ar
+0000fcf0: 6775 6d65 6e74 7320 636f 7272 6573 706f  guments correspo
+0000fd00: 6e64 2031 3a31 2074 6f20 7468 6520 6174  nd 1:1 to the at
+0000fd10: 7472 6962 7574 6573 206f 6620 7468 6520  tributes of the 
+0000fd20: 3c61 6e6e 6f74 6174 696f 6e3e 2065 6c65  <annotation> ele
+0000fd30: 6d65 6e74 2e0a 0a20 2020 2052 6169 7365  ment...    Raise
+0000fd40: 733a 0a20 2020 2020 2020 2057 6172 6e69  s:.        Warni
+0000fd50: 6e67 3a20 6966 2062 6f74 6820 616e 2041  ng: if both an A
+0000fd60: 524b 2061 6e64 2061 6e20 4952 4920 6172  RK and an IRI ar
+0000fd70: 6520 7072 6f76 6964 6564 0a20 2020 2020  e provided.     
+0000fd80: 2020 2042 6173 6545 7272 6f72 3a20 6966     BaseError: if
+0000fd90: 2074 6865 2063 7265 6174 696f 6e20 6461   the creation da
+0000fda0: 7465 2069 7320 696e 7661 6c69 640a 0a20  te is invalid.. 
+0000fdb0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000fdc0: 2020 2020 5468 6520 616e 6e6f 7461 7469      The annotati
+0000fdd0: 6f6e 2065 6c65 6d65 6e74 2c20 7769 7468  on element, with
+0000fde0: 6f75 7420 616e 7920 6368 696c 6472 656e  out any children
+0000fdf0: 2c20 6275 7420 7769 7468 2074 6865 2061  , but with the a
+0000fe00: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
+0000fe10: 2020 203c 616e 6e6f 7461 7469 6f6e 206c     <annotation l
+0000fe20: 6162 656c 3d6c 6162 656c 2069 643d 6964  abel=label id=id
+0000fe30: 2070 6572 6d69 7373 696f 6e73 3d70 6572   permissions=per
+0000fe40: 6d69 7373 696f 6e73 2061 726b 3d61 726b  missions ark=ark
+0000fe50: 2069 7269 3d69 7269 3e3c 2f61 6e6e 6f74   iri=iri></annot
+0000fe60: 6174 696f 6e3e 0a0a 2020 2020 4578 616d  ation>..    Exam
+0000fe70: 706c 6573 3a0a 2020 2020 2020 2020 3e3e  ples:.        >>
+0000fe80: 3e20 616e 6e6f 7461 7469 6f6e 203d 2065  > annotation = e
+0000fe90: 7863 656c 3278 6d6c 2e6d 616b 655f 616e  xcel2xml.make_an
+0000fea0: 6e6f 7461 7469 6f6e 2822 6c61 6265 6c22  notation("label"
+0000feb0: 2c20 2269 6422 290a 2020 2020 2020 2020  , "id").        
+0000fec0: 3e3e 3e20 616e 6e6f 7461 7469 6f6e 2e61  >>> annotation.a
+0000fed0: 7070 656e 6428 6578 6365 6c32 786d 6c2e  ppend(excel2xml.
+0000fee0: 6d61 6b65 5f74 6578 745f 7072 6f70 2822  make_text_prop("
+0000fef0: 6861 7343 6f6d 6d65 6e74 222c 2022 5468  hasComment", "Th
+0000ff00: 6973 2069 7320 6120 636f 6d6d 656e 7422  is is a comment"
+0000ff10: 2929 0a20 2020 2020 2020 203e 3e3e 2061  )).        >>> a
+0000ff20: 6e6e 6f74 6174 696f 6e2e 6170 7065 6e64  nnotation.append
+0000ff30: 2865 7863 656c 3278 6d6c 2e6d 616b 655f  (excel2xml.make_
+0000ff40: 7265 7370 7472 5f70 726f 7028 2269 7341  resptr_prop("isA
+0000ff50: 6e6e 6f74 6174 696f 6e4f 6622 2c20 2272  nnotationOf", "r
+0000ff60: 6573 6f75 7263 655f 3022 2929 0a20 2020  esource_0")).   
+0000ff70: 2020 2020 203e 3e3e 2072 6f6f 742e 6170       >>> root.ap
+0000ff80: 7065 6e64 2861 6e6e 6f74 6174 696f 6e29  pend(annotation)
+0000ff90: 0a0a 2020 2020 5365 6520 6874 7470 733a  ..    See https:
+0000ffa0: 2f2f 646f 6373 2e64 6173 6368 2e73 7769  //docs.dasch.swi
+0000ffb0: 7373 2f6c 6174 6573 742f 4453 502d 544f  ss/latest/DSP-TO
+0000ffc0: 4f4c 532f 6669 6c65 2d66 6f72 6d61 7473  OLS/file-formats
+0000ffd0: 2f78 6d6c 2d64 6174 612d 6669 6c65 2f23  /xml-data-file/#
+0000ffe0: 616e 6e6f 7461 7469 6f6e 0a20 2020 2022  annotation.    "
+0000fff0: 2222 0a0a 2020 2020 6b77 6172 6773 203d  ""..    kwargs =
+00010000: 207b 226c 6162 656c 223a 206c 6162 656c   {"label": label
+00010010: 2c20 2269 6422 3a20 6964 2c20 2270 6572  , "id": id, "per
+00010020: 6d69 7373 696f 6e73 223a 2070 6572 6d69  missions": permi
+00010030: 7373 696f 6e73 2c20 226e 736d 6170 223a  ssions, "nsmap":
+00010040: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
+00010050: 6170 7d0a 2020 2020 6966 2061 726b 3a0a  ap}.    if ark:.
+00010060: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
+00010070: 6172 6b22 5d20 3d20 6172 6b0a 2020 2020  ark"] = ark.    
+00010080: 6966 2069 7269 3a0a 2020 2020 2020 2020  if iri:.        
+00010090: 6b77 6172 6773 5b22 6972 6922 5d20 3d20  kwargs["iri"] = 
+000100a0: 6972 690a 2020 2020 6966 2061 726b 2061  iri.    if ark a
+000100b0: 6e64 2069 7269 3a0a 2020 2020 2020 2020  nd iri:.        
+000100c0: 7761 726e 696e 6720 3d20 6622 426f 7468  warning = f"Both
+000100d0: 2041 524b 2061 6e64 2049 5249 2077 6572   ARK and IRI wer
+000100e0: 6520 7072 6f76 6964 6564 2066 6f72 2072  e provided for r
+000100f0: 6573 6f75 7263 6520 277b 6c61 6265 6c7d  esource '{label}
+00010100: 2720 287b 6964 7d29 2e20 5468 6520 4152  ' ({id}). The AR
+00010110: 4b20 7769 6c6c 206f 7665 7272 6964 6520  K will override 
+00010120: 7468 6520 4952 492e 220a 2020 2020 2020  the IRI.".      
+00010130: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+00010140: 4473 7054 6f6f 6c73 5573 6572 5761 726e  DspToolsUserWarn
+00010150: 696e 6728 7761 726e 696e 6729 290a 2020  ing(warning)).  
+00010160: 2020 6966 2063 7265 6174 696f 6e5f 6461    if creation_da
+00010170: 7465 3a0a 2020 2020 2020 2020 7472 793a  te:.        try:
+00010180: 0a20 2020 2020 2020 2020 2020 2044 6174  .            Dat
+00010190: 6554 696d 6553 7461 6d70 2863 7265 6174  eTimeStamp(creat
+000101a0: 696f 6e5f 6461 7465 290a 2020 2020 2020  ion_date).      
+000101b0: 2020 6578 6365 7074 2042 6173 6545 7272    except BaseErr
+000101c0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+000101d0: 7261 6973 6520 4261 7365 4572 726f 7228  raise BaseError(
+000101e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000101f0: 2066 2254 6865 2061 6e6e 6f74 6174 696f   f"The annotatio
+00010200: 6e20 277b 6c61 6265 6c7d 2720 2849 443a  n '{label}' (ID:
+00010210: 207b 6964 7d29 2068 6173 2061 6e20 696e   {id}) has an in
+00010220: 7661 6c69 6420 6372 6561 7469 6f6e 2064  valid creation d
+00010230: 6174 6520 277b 6372 6561 7469 6f6e 5f64  ate '{creation_d
+00010240: 6174 657d 272e 2022 0a20 2020 2020 2020  ate}'. ".       
+00010250: 2020 2020 2020 2020 2066 2244 6964 2079           f"Did y
+00010260: 6f75 2070 6572 6861 7073 2066 6f72 6765  ou perhaps forge
+00010270: 7420 7468 6520 7469 6d65 7a6f 6e65 3f22  t the timezone?"
+00010280: 0a20 2020 2020 2020 2020 2020 2029 2066  .            ) f
+00010290: 726f 6d20 4e6f 6e65 0a20 2020 2020 2020  rom None.       
+000102a0: 206b 7761 7267 735b 2263 7265 6174 696f   kwargs["creatio
+000102b0: 6e5f 6461 7465 225d 203d 2063 7265 6174  n_date"] = creat
+000102c0: 696f 6e5f 6461 7465 0a0a 2020 2020 7265  ion_date..    re
+000102d0: 7475 726e 2065 7472 6565 2e45 6c65 6d65  turn etree.Eleme
+000102e0: 6e74 280a 2020 2020 2020 2020 227b 2573  nt(.        "{%s
+000102f0: 7d61 6e6e 6f74 6174 696f 6e22 2025 2078  }annotation" % x
+00010300: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
+00010310: 5b4e 6f6e 655d 2c0a 2020 2020 2020 2020  [None],.        
+00010320: 2a2a 6b77 6172 6773 2c20 2023 2074 7970  **kwargs,  # typ
+00010330: 653a 2069 676e 6f72 655b 6172 672d 7479  e: ignore[arg-ty
+00010340: 7065 5d0a 2020 2020 290a 0a0a 6465 6620  pe].    )...def 
+00010350: 6d61 6b65 5f6c 696e 6b28 2020 2320 6e6f  make_link(  # no
+00010360: 7161 3a20 4434 3137 2028 756e 646f 6375  qa: D417 (undocu
+00010370: 6d65 6e74 6564 2d70 6172 616d 290a 2020  mented-param).  
+00010380: 2020 6c61 6265 6c3a 2073 7472 2c0a 2020    label: str,.  
+00010390: 2020 6964 3a20 7374 722c 0a20 2020 2070    id: str,.    p
+000103a0: 6572 6d69 7373 696f 6e73 3a20 7374 7220  ermissions: str 
+000103b0: 3d20 2272 6573 2d64 6566 6175 6c74 222c  = "res-default",
+000103c0: 0a20 2020 2061 726b 3a20 4f70 7469 6f6e  .    ark: Option
+000103d0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+000103e0: 2020 2020 6972 693a 204f 7074 696f 6e61      iri: Optiona
+000103f0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+00010400: 2020 2063 7265 6174 696f 6e5f 6461 7465     creation_date
+00010410: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00010420: 3d20 4e6f 6e65 2c0a 2920 2d3e 2065 7472  = None,.) -> etr
+00010430: 6565 2e5f 456c 656d 656e 743a 0a20 2020  ee._Element:.   
+00010440: 2022 2222 0a20 2020 2043 7265 6174 6573   """.    Creates
+00010450: 2061 6e20 656d 7074 7920 6c69 6e6b 2065   an empty link e
+00010460: 6c65 6d65 6e74 2c20 7769 7468 2074 6865  lement, with the
+00010470: 2061 7474 7269 6275 7465 7320 6173 2073   attributes as s
+00010480: 7065 6369 6669 6564 2062 7920 7468 6520  pecified by the 
+00010490: 6172 6775 6d65 6e74 730a 0a20 2020 2041  arguments..    A
+000104a0: 7267 733a 0a20 2020 2020 2020 2054 6865  rgs:.        The
+000104b0: 2061 7267 756d 656e 7473 2063 6f72 7265   arguments corre
+000104c0: 7370 6f6e 6420 313a 3120 746f 2074 6865  spond 1:1 to the
+000104d0: 2061 7474 7269 6275 7465 7320 6f66 2074   attributes of t
+000104e0: 6865 203c 6c69 6e6b 3e20 656c 656d 656e  he <link> elemen
+000104f0: 742e 0a0a 2020 2020 5261 6973 6573 3a0a  t...    Raises:.
+00010500: 2020 2020 2020 2020 5761 726e 696e 673a          Warning:
+00010510: 2069 6620 626f 7468 2061 6e20 4152 4b20   if both an ARK 
+00010520: 616e 6420 616e 2049 5249 2061 7265 2070  and an IRI are p
+00010530: 726f 7669 6465 640a 2020 2020 2020 2020  rovided.        
+00010540: 4261 7365 4572 726f 723a 2069 6620 7468  BaseError: if th
+00010550: 6520 6372 6561 7469 6f6e 2064 6174 6520  e creation date 
+00010560: 6973 2069 6e76 616c 6964 0a0a 2020 2020  is invalid..    
+00010570: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00010580: 2054 6865 206c 696e 6b20 656c 656d 656e   The link elemen
+00010590: 742c 2077 6974 686f 7574 2061 6e79 2063  t, without any c
+000105a0: 6869 6c64 7265 6e2c 2062 7574 2077 6974  hildren, but wit
+000105b0: 6820 7468 6520 6174 7472 6962 7574 6573  h the attributes
+000105c0: 3a0a 2020 2020 2020 2020 3c6c 696e 6b20  :.        <link 
+000105d0: 6c61 6265 6c3d 6c61 6265 6c20 6964 3d69  label=label id=i
+000105e0: 6420 7065 726d 6973 7369 6f6e 733d 7065  d permissions=pe
+000105f0: 726d 6973 7369 6f6e 7320 6172 6b3d 6172  rmissions ark=ar
+00010600: 6b20 6972 693d 6972 693e 3c2f 6c69 6e6b  k iri=iri></link
+00010610: 3e0a 0a20 2020 2045 7861 6d70 6c65 733a  >..    Examples:
+00010620: 0a20 2020 2020 2020 203e 3e3e 206c 696e  .        >>> lin
+00010630: 6b20 3d20 6578 6365 6c32 786d 6c2e 6d61  k = excel2xml.ma
+00010640: 6b65 5f6c 696e 6b28 226c 6162 656c 222c  ke_link("label",
+00010650: 2022 6964 2229 0a20 2020 2020 2020 203e   "id").        >
+00010660: 3e3e 206c 696e 6b2e 6170 7065 6e64 2865  >> link.append(e
+00010670: 7863 656c 3278 6d6c 2e6d 616b 655f 7465  xcel2xml.make_te
+00010680: 7874 5f70 726f 7028 2268 6173 436f 6d6d  xt_prop("hasComm
+00010690: 656e 7422 2c20 2254 6869 7320 6973 2061  ent", "This is a
+000106a0: 2063 6f6d 6d65 6e74 2229 290a 2020 2020   comment")).    
+000106b0: 2020 2020 3e3e 3e20 6c69 6e6b 2e61 7070      >>> link.app
+000106c0: 656e 6428 6578 6365 6c32 786d 6c2e 6d61  end(excel2xml.ma
+000106d0: 6b65 5f72 6573 7074 725f 7072 6f70 2822  ke_resptr_prop("
+000106e0: 6861 734c 696e 6b54 6f22 2c20 5b22 7265  hasLinkTo", ["re
+000106f0: 736f 7572 6365 5f30 222c 2022 7265 736f  source_0", "reso
+00010700: 7572 6365 5f31 225d 2929 0a20 2020 2020  urce_1"])).     
+00010710: 2020 203e 3e3e 2072 6f6f 742e 6170 7065     >>> root.appe
+00010720: 6e64 286c 696e 6b29 0a0a 2020 2020 5365  nd(link)..    Se
+00010730: 6520 6874 7470 733a 2f2f 646f 6373 2e64  e https://docs.d
+00010740: 6173 6368 2e73 7769 7373 2f6c 6174 6573  asch.swiss/lates
+00010750: 742f 4453 502d 544f 4f4c 532f 6669 6c65  t/DSP-TOOLS/file
+00010760: 2d66 6f72 6d61 7473 2f78 6d6c 2d64 6174  -formats/xml-dat
+00010770: 612d 6669 6c65 2f23 6c69 6e6b 0a20 2020  a-file/#link.   
+00010780: 2022 2222 0a0a 2020 2020 6b77 6172 6773   """..    kwargs
+00010790: 203d 207b 226c 6162 656c 223a 206c 6162   = {"label": lab
+000107a0: 656c 2c20 2269 6422 3a20 6964 2c20 2270  el, "id": id, "p
+000107b0: 6572 6d69 7373 696f 6e73 223a 2070 6572  ermissions": per
+000107c0: 6d69 7373 696f 6e73 2c20 226e 736d 6170  missions, "nsmap
+000107d0: 223a 2078 6d6c 5f6e 616d 6573 7061 6365  ": xml_namespace
+000107e0: 5f6d 6170 7d0a 2020 2020 6966 2061 726b  _map}.    if ark
+000107f0: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
+00010800: 5b22 6172 6b22 5d20 3d20 6172 6b0a 2020  ["ark"] = ark.  
+00010810: 2020 6966 2069 7269 3a0a 2020 2020 2020    if iri:.      
+00010820: 2020 6b77 6172 6773 5b22 6972 6922 5d20    kwargs["iri"] 
+00010830: 3d20 6972 690a 2020 2020 6966 2061 726b  = iri.    if ark
+00010840: 2061 6e64 2069 7269 3a0a 2020 2020 2020   and iri:.      
+00010850: 2020 6d73 6720 3d20 6622 426f 7468 2041    msg = f"Both A
+00010860: 524b 2061 6e64 2049 5249 2077 6572 6520  RK and IRI were 
+00010870: 7072 6f76 6964 6564 2066 6f72 2072 6573  provided for res
+00010880: 6f75 7263 6520 277b 6c61 6265 6c7d 2720  ource '{label}' 
+00010890: 287b 6964 7d29 2e20 5468 6520 4152 4b20  ({id}). The ARK 
+000108a0: 7769 6c6c 206f 7665 7272 6964 6520 7468  will override th
+000108b0: 6520 4952 492e 220a 2020 2020 2020 2020  e IRI.".        
+000108c0: 7761 726e 696e 6773 2e77 6172 6e28 4473  warnings.warn(Ds
+000108d0: 7054 6f6f 6c73 5573 6572 5761 726e 696e  pToolsUserWarnin
+000108e0: 6728 6d73 6729 290a 2020 2020 6966 2063  g(msg)).    if c
+000108f0: 7265 6174 696f 6e5f 6461 7465 3a0a 2020  reation_date:.  
+00010900: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00010910: 2020 2020 2020 2044 6174 6554 696d 6553         DateTimeS
+00010920: 7461 6d70 2863 7265 6174 696f 6e5f 6461  tamp(creation_da
+00010930: 7465 290a 2020 2020 2020 2020 6578 6365  te).        exce
+00010940: 7074 2042 6173 6545 7272 6f72 3a0a 2020  pt BaseError:.  
+00010950: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00010960: 4261 7365 4572 726f 7228 0a20 2020 2020  BaseError(.     
+00010970: 2020 2020 2020 2020 2020 2066 2254 6865             f"The
+00010980: 206c 696e 6b20 277b 6c61 6265 6c7d 2720   link '{label}' 
+00010990: 2849 443a 207b 6964 7d29 2068 6173 2061  (ID: {id}) has a
+000109a0: 6e20 696e 7661 6c69 6420 6372 6561 7469  n invalid creati
+000109b0: 6f6e 2064 6174 6520 277b 6372 6561 7469  on date '{creati
+000109c0: 6f6e 5f64 6174 657d 272e 2022 0a20 2020  on_date}'. ".   
+000109d0: 2020 2020 2020 2020 2020 2020 2066 2244               f"D
+000109e0: 6964 2079 6f75 2070 6572 6861 7073 2066  id you perhaps f
+000109f0: 6f72 6765 7420 7468 6520 7469 6d65 7a6f  orget the timezo
+00010a00: 6e65 3f22 0a20 2020 2020 2020 2020 2020  ne?".           
+00010a10: 2029 2066 726f 6d20 4e6f 6e65 0a20 2020   ) from None.   
+00010a20: 2020 2020 206b 7761 7267 735b 2263 7265       kwargs["cre
+00010a30: 6174 696f 6e5f 6461 7465 225d 203d 2063  ation_date"] = c
+00010a40: 7265 6174 696f 6e5f 6461 7465 0a0a 2020  reation_date..  
+00010a50: 2020 7265 7475 726e 2065 7472 6565 2e45    return etree.E
+00010a60: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
+00010a70: 227b 2573 7d6c 696e 6b22 2025 2078 6d6c  "{%s}link" % xml
+00010a80: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
+00010a90: 6f6e 655d 2c0a 2020 2020 2020 2020 2a2a  one],.        **
+00010aa0: 6b77 6172 6773 2c20 2023 2074 7970 653a  kwargs,  # type:
+00010ab0: 2069 676e 6f72 655b 6172 672d 7479 7065   ignore[arg-type
+00010ac0: 5d0a 2020 2020 290a 0a0a 6465 6620 6d61  ].    )...def ma
+00010ad0: 6b65 5f61 7564 696f 5f73 6567 6d65 6e74  ke_audio_segment
+00010ae0: 2820 2023 206e 6f71 613a 2044 3431 3720  (  # noqa: D417 
+00010af0: 2875 6e64 6f63 756d 656e 7465 642d 7061  (undocumented-pa
+00010b00: 7261 6d29 0a20 2020 206c 6162 656c 3a20  ram).    label: 
+00010b10: 7374 722c 0a20 2020 2069 643a 2073 7472  str,.    id: str
+00010b20: 2c0a 2020 2020 7065 726d 6973 7369 6f6e  ,.    permission
+00010b30: 733a 2073 7472 203d 2022 7265 732d 6465  s: str = "res-de
+00010b40: 6661 756c 7422 2c0a 2920 2d3e 2065 7472  fault",.) -> etr
+00010b50: 6565 2e5f 456c 656d 656e 743a 0a20 2020  ee._Element:.   
+00010b60: 2022 2222 0a20 2020 2043 7265 6174 6573   """.    Creates
+00010b70: 2061 6e20 656d 7074 7920 3c61 7564 696f   an empty <audio
+00010b80: 2d73 6567 6d65 6e74 3e20 656c 656d 656e  -segment> elemen
+00010b90: 742c 2077 6974 6820 7468 6520 6174 7472  t, with the attr
+00010ba0: 6962 7574 6573 2061 7320 7370 6563 6966  ibutes as specif
+00010bb0: 6965 6420 6279 2074 6865 2061 7267 756d  ied by the argum
+00010bc0: 656e 7473 0a0a 2020 2020 4172 6773 3a0a  ents..    Args:.
+00010bd0: 2020 2020 2020 2020 5468 6520 6172 6775          The argu
+00010be0: 6d65 6e74 7320 636f 7272 6573 706f 6e64  ments correspond
+00010bf0: 2031 3a31 2074 6f20 7468 6520 6174 7472   1:1 to the attr
+00010c00: 6962 7574 6573 206f 6620 7468 6520 3c61  ibutes of the <a
+00010c10: 7564 696f 2d73 6567 6d65 6e74 3e20 656c  udio-segment> el
+00010c20: 656d 656e 742e 0a0a 2020 2020 5265 7475  ement...    Retu
+00010c30: 726e 733a 0a20 2020 2020 2020 2054 6865  rns:.        The
+00010c40: 2061 7564 696f 2d73 6567 6d65 6e74 2065   audio-segment e
+00010c50: 6c65 6d65 6e74 2c20 7769 7468 6f75 7420  lement, without 
+00010c60: 616e 7920 6368 696c 6472 656e 2c20 6275  any children, bu
+00010c70: 7420 7769 7468 2074 6865 2061 7474 7269  t with the attri
+00010c80: 6275 7465 733a 0a20 2020 2020 2020 203c  butes:.        <
+00010c90: 6175 6469 6f2d 7365 676d 656e 7420 6c61  audio-segment la
+00010ca0: 6265 6c3d 6c61 6265 6c20 6964 3d69 6420  bel=label id=id 
+00010cb0: 7065 726d 6973 7369 6f6e 733d 7065 726d  permissions=perm
+00010cc0: 6973 7369 6f6e 733e 3c2f 6175 6469 6f2d  issions></audio-
+00010cd0: 7365 676d 656e 743e 0a0a 2020 2020 4578  segment>..    Ex
+00010ce0: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
+00010cf0: 3e3e 3e20 6175 6469 6f5f 7365 676d 656e  >>> audio_segmen
+00010d00: 7420 3d20 6578 6365 6c32 786d 6c2e 6d61  t = excel2xml.ma
+00010d10: 6b65 5f61 7564 696f 5f73 6567 6d65 6e74  ke_audio_segment
+00010d20: 2822 6c61 6265 6c22 2c20 2269 6422 290a  ("label", "id").
+00010d30: 2020 2020 2020 2020 3e3e 3e20 6175 6469          >>> audi
+00010d40: 6f5f 7365 676d 656e 742e 6170 7065 6e64  o_segment.append
+00010d50: 2865 7863 656c 3278 6d6c 2e6d 616b 655f  (excel2xml.make_
+00010d60: 7265 7370 7472 5f70 726f 7028 2269 7353  resptr_prop("isS
+00010d70: 6567 6d65 6e74 4f66 222c 2022 6175 6469  egmentOf", "audi
+00010d80: 6f5f 7265 736f 7572 6365 5f69 6422 2929  o_resource_id"))
+00010d90: 0a20 2020 2020 2020 203e 3e3e 2061 7564  .        >>> aud
+00010da0: 696f 5f73 6567 6d65 6e74 2e61 7070 656e  io_segment.appen
+00010db0: 6428 6578 6365 6c32 786d 6c2e 6d61 6b65  d(excel2xml.make
+00010dc0: 5f69 6e74 6572 7661 6c5f 7072 6f70 2822  _interval_prop("
+00010dd0: 6861 7353 6567 6d65 6e74 426f 756e 6473  hasSegmentBounds
+00010de0: 222c 2022 3630 3a31 3230 2229 0a20 2020  ", "60:120").   
+00010df0: 2020 2020 203e 3e3e 2072 6f6f 742e 6170       >>> root.ap
+00010e00: 7065 6e64 2861 7564 696f 5f73 6567 6d65  pend(audio_segme
+00010e10: 6e74 290a 0a20 2020 2053 6565 2068 7474  nt)..    See htt
+00010e20: 7073 3a2f 2f64 6f63 732e 6461 7363 682e  ps://docs.dasch.
+00010e30: 7377 6973 732f 6c61 7465 7374 2f44 5350  swiss/latest/DSP
+00010e40: 2d54 4f4f 4c53 2f66 696c 652d 666f 726d  -TOOLS/file-form
+00010e50: 6174 732f 786d 6c2d 6461 7461 2d66 696c  ats/xml-data-fil
+00010e60: 652f 2376 6964 656f 2d73 6567 6d65 6e74  e/#video-segment
+00010e70: 2d61 7564 696f 2d73 6567 6d65 6e74 0a20  -audio-segment. 
+00010e80: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
+00010e90: 6e20 6574 7265 652e 456c 656d 656e 7428  n etree.Element(
+00010ea0: 0a20 2020 2020 2020 2022 7b25 737d 6175  .        "{%s}au
+00010eb0: 6469 6f2d 7365 676d 656e 7422 2025 2078  dio-segment" % x
+00010ec0: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
+00010ed0: 5b4e 6f6e 655d 2c0a 2020 2020 2020 2020  [None],.        
+00010ee0: 6c61 6265 6c3d 6c61 6265 6c2c 0a20 2020  label=label,.   
+00010ef0: 2020 2020 2069 643d 6964 2c0a 2020 2020       id=id,.    
+00010f00: 2020 2020 7065 726d 6973 7369 6f6e 733d      permissions=
+00010f10: 7065 726d 6973 7369 6f6e 732c 0a20 2020  permissions,.   
+00010f20: 2020 2020 206e 736d 6170 3d78 6d6c 5f6e       nsmap=xml_n
+00010f30: 616d 6573 7061 6365 5f6d 6170 2c0a 2020  amespace_map,.  
+00010f40: 2020 290a 0a0a 6465 6620 6d61 6b65 5f76    )...def make_v
+00010f50: 6964 656f 5f73 6567 6d65 6e74 2820 2023  ideo_segment(  #
+00010f60: 206e 6f71 613a 2044 3431 3720 2875 6e64   noqa: D417 (und
+00010f70: 6f63 756d 656e 7465 642d 7061 7261 6d29  ocumented-param)
+00010f80: 0a20 2020 206c 6162 656c 3a20 7374 722c  .    label: str,
+00010f90: 0a20 2020 2069 643a 2073 7472 2c0a 2020  .    id: str,.  
+00010fa0: 2020 7065 726d 6973 7369 6f6e 733a 2073    permissions: s
+00010fb0: 7472 203d 2022 7265 732d 6465 6661 756c  tr = "res-defaul
+00010fc0: 7422 2c0a 2920 2d3e 2065 7472 6565 2e5f  t",.) -> etree._
+00010fd0: 456c 656d 656e 743a 0a20 2020 2022 2222  Element:.    """
+00010fe0: 0a20 2020 2043 7265 6174 6573 2061 6e20  .    Creates an 
+00010ff0: 656d 7074 7920 3c76 6964 656f 2d73 6567  empty <video-seg
+00011000: 6d65 6e74 3e20 656c 656d 656e 742c 2077  ment> element, w
+00011010: 6974 6820 7468 6520 6174 7472 6962 7574  ith the attribut
+00011020: 6573 2061 7320 7370 6563 6966 6965 6420  es as specified 
+00011030: 6279 2074 6865 2061 7267 756d 656e 7473  by the arguments
+00011040: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00011050: 2020 2020 5468 6520 6172 6775 6d65 6e74      The argument
+00011060: 7320 636f 7272 6573 706f 6e64 2031 3a31  s correspond 1:1
+00011070: 2074 6f20 7468 6520 6174 7472 6962 7574   to the attribut
+00011080: 6573 206f 6620 7468 6520 3c76 6964 656f  es of the <video
+00011090: 2d73 6567 6d65 6e74 3e20 656c 656d 656e  -segment> elemen
+000110a0: 742e 0a0a 2020 2020 5265 7475 726e 733a  t...    Returns:
+000110b0: 0a20 2020 2020 2020 2054 6865 2076 6964  .        The vid
+000110c0: 656f 2d73 6567 6d65 6e74 2065 6c65 6d65  eo-segment eleme
+000110d0: 6e74 2c20 7769 7468 6f75 7420 616e 7920  nt, without any 
+000110e0: 6368 696c 6472 656e 2c20 6275 7420 7769  children, but wi
+000110f0: 7468 2074 6865 2061 7474 7269 6275 7465  th the attribute
+00011100: 733a 0a20 2020 2020 2020 203c 7669 6465  s:.        <vide
+00011110: 6f2d 7365 676d 656e 7420 6c61 6265 6c3d  o-segment label=
+00011120: 6c61 6265 6c20 6964 3d69 6420 7065 726d  label id=id perm
+00011130: 6973 7369 6f6e 733d 7065 726d 6973 7369  issions=permissi
+00011140: 6f6e 733e 3c2f 7669 6465 6f2d 7365 676d  ons></video-segm
+00011150: 656e 743e 0a0a 2020 2020 4578 616d 706c  ent>..    Exampl
+00011160: 6573 3a0a 2020 2020 2020 2020 3e3e 3e20  es:.        >>> 
+00011170: 7669 6465 6f5f 7365 676d 656e 7420 3d20  video_segment = 
+00011180: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f76  excel2xml.make_v
+00011190: 6964 656f 5f73 6567 6d65 6e74 2822 6c61  ideo_segment("la
+000111a0: 6265 6c22 2c20 2269 6422 290a 2020 2020  bel", "id").    
+000111b0: 2020 2020 3e3e 3e20 7669 6465 6f5f 7365      >>> video_se
+000111c0: 676d 656e 742e 6170 7065 6e64 2865 7863  gment.append(exc
+000111d0: 656c 3278 6d6c 2e6d 616b 655f 7265 7370  el2xml.make_resp
+000111e0: 7472 5f70 726f 7028 2269 7353 6567 6d65  tr_prop("isSegme
+000111f0: 6e74 4f66 222c 2022 7669 6465 6f5f 7265  ntOf", "video_re
+00011200: 736f 7572 6365 5f69 6422 2929 0a20 2020  source_id")).   
+00011210: 2020 2020 203e 3e3e 2076 6964 656f 5f73       >>> video_s
+00011220: 6567 6d65 6e74 2e61 7070 656e 6428 6578  egment.append(ex
+00011230: 6365 6c32 786d 6c2e 6d61 6b65 5f69 6e74  cel2xml.make_int
+00011240: 6572 7661 6c5f 7072 6f70 2822 6861 7353  erval_prop("hasS
+00011250: 6567 6d65 6e74 426f 756e 6473 222c 2022  egmentBounds", "
+00011260: 3630 3a31 3230 2229 0a20 2020 2020 2020  60:120").       
+00011270: 203e 3e3e 2072 6f6f 742e 6170 7065 6e64   >>> root.append
+00011280: 2876 6964 656f 5f73 6567 6d65 6e74 290a  (video_segment).
+00011290: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
+000112a0: 2f64 6f63 732e 6461 7363 682e 7377 6973  /docs.dasch.swis
+000112b0: 732f 6c61 7465 7374 2f44 5350 2d54 4f4f  s/latest/DSP-TOO
+000112c0: 4c53 2f66 696c 652d 666f 726d 6174 732f  LS/file-formats/
+000112d0: 786d 6c2d 6461 7461 2d66 696c 652f 2376  xml-data-file/#v
+000112e0: 6964 656f 2d73 6567 6d65 6e74 2d61 7564  ideo-segment-aud
+000112f0: 696f 2d73 6567 6d65 6e74 0a20 2020 2022  io-segment.    "
+00011300: 2222 0a20 2020 2072 6574 7572 6e20 6574  "".    return et
+00011310: 7265 652e 456c 656d 656e 7428 0a20 2020  ree.Element(.   
+00011320: 2020 2020 2022 7b25 737d 7669 6465 6f2d       "{%s}video-
+00011330: 7365 676d 656e 7422 2025 2078 6d6c 5f6e  segment" % xml_n
+00011340: 616d 6573 7061 6365 5f6d 6170 5b4e 6f6e  amespace_map[Non
+00011350: 655d 2c0a 2020 2020 2020 2020 6c61 6265  e],.        labe
+00011360: 6c3d 6c61 6265 6c2c 0a20 2020 2020 2020  l=label,.       
+00011370: 2069 643d 6964 2c0a 2020 2020 2020 2020   id=id,.        
+00011380: 7065 726d 6973 7369 6f6e 733d 7065 726d  permissions=perm
+00011390: 6973 7369 6f6e 732c 0a20 2020 2020 2020  issions,.       
+000113a0: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
+000113b0: 7061 6365 5f6d 6170 2c0a 2020 2020 290a  pace_map,.    ).
+000113c0: 0a0a 6465 6620 6372 6561 7465 5f69 6e74  ..def create_int
+000113d0: 6572 7661 6c5f 7661 6c75 6528 7374 6172  erval_value(star
+000113e0: 743a 2073 7472 2c20 656e 643a 2073 7472  t: str, end: str
+000113f0: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
+00011400: 220a 2020 2020 5472 616e 7366 6f72 6d20  ".    Transform 
+00011410: 6120 7374 6172 7420 616e 6420 656e 6420  a start and end 
+00011420: 7469 6d65 2069 6e74 6f20 6120 7661 6c69  time into a vali
+00011430: 6420 4453 5020 696e 7465 7276 616c 2076  d DSP interval v
+00011440: 616c 7565 2c0a 2020 2020 7768 6963 6820  alue,.    which 
+00011450: 7468 656e 2063 616e 2062 6520 7573 6564  then can be used
+00011460: 2069 6e20 616e 203c 696e 7465 7276 616c   in an <interval
+00011470: 206e 616d 653d 2268 6173 5365 676d 656e   name="hasSegmen
+00011480: 7442 6f75 6e64 7322 3e20 7461 672c 0a20  tBounds"> tag,. 
+00011490: 2020 2077 6869 6368 2069 7320 7573 6564     which is used
+000114a0: 2069 6e20 3c61 7564 696f 2d73 6567 6d65   in <audio-segme
+000114b0: 6e74 3e20 616e 6420 3c76 6964 656f 2d73  nt> and <video-s
+000114c0: 6567 6d65 6e74 3e20 656c 656d 656e 7473  egment> elements
+000114d0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+000114e0: 2020 2020 2073 7461 7274 3a20 7374 6172       start: star
+000114f0: 7420 7469 6d65 206f 6620 7468 6520 7669  t time of the vi
+00011500: 6465 6f2f 6175 6469 6f20 7365 676d 656e  deo/audio segmen
+00011510: 742c 2069 6e20 7468 6520 666f 726d 6174  t, in the format
+00011520: 2027 4828 4829 3a4d 4d3a 5353 282e 7329   'H(H):MM:SS(.s)
+00011530: 270a 2020 2020 2020 2020 656e 643a 2065  '.        end: e
+00011540: 6e64 2074 696d 6520 6f66 2074 6865 2076  nd time of the v
+00011550: 6964 656f 2f61 7564 696f 2073 6567 6d65  ideo/audio segme
+00011560: 6e74 2c20 696e 2074 6865 2066 6f72 6d61  nt, in the forma
+00011570: 7420 2748 2848 293a 4d4d 3a53 5328 2e73  t 'H(H):MM:SS(.s
+00011580: 2927 0a0a 2020 2020 5261 6973 6573 3a0a  )'..    Raises:.
+00011590: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+000115a0: 6f72 3a20 6966 2074 6865 2070 726f 7669  or: if the provi
+000115b0: 6465 6420 6172 6775 6d65 6e74 7320 6172  ded arguments ar
+000115c0: 6520 6e6f 7420 696e 2074 6865 2063 6f72  e not in the cor
+000115d0: 7265 6374 2066 6f72 6d61 742c 206f 7220  rect format, or 
+000115e0: 6966 2074 6865 2073 7461 7274 2074 696d  if the start tim
+000115f0: 6520 6973 2067 7265 6174 6572 2074 6861  e is greater tha
+00011600: 6e20 7468 6520 656e 6420 7469 6d65 0a0a  n the end time..
+00011610: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00011620: 2020 2020 2061 2044 5350 2069 6e74 6572       a DSP inter
+00011630: 7661 6c20 7661 6c75 6520 696e 2074 6865  val value in the
+00011640: 2066 6f72 6d61 7420 2773 7461 7274 5f73   format 'start_s
+00011650: 6563 6f6e 6473 3a65 6e64 5f73 6563 6f6e  econds:end_secon
+00011660: 6473 270a 0a20 2020 2045 7861 6d70 6c65  ds'..    Example
+00011670: 733a 0a20 2020 2020 2020 203e 3e3e 2065  s:.        >>> e
+00011680: 7863 656c 3278 6d6c 2e63 7265 6174 655f  xcel2xml.create_
+00011690: 696e 7465 7276 616c 5f76 616c 7565 2822  interval_value("
+000116a0: 303a 3031 3a30 3022 2c20 2230 3a30 323a  0:01:00", "0:02:
+000116b0: 3030 2229 0a20 2020 2020 2020 2022 3630  00").        "60
+000116c0: 3a31 3230 220a 2020 2020 2020 2020 3e3e  :120".        >>
+000116d0: 3e20 6578 6365 6c32 786d 6c2e 6372 6561  > excel2xml.crea
+000116e0: 7465 5f69 6e74 6572 7661 6c5f 7661 6c75  te_interval_valu
+000116f0: 6528 2230 3a30 313a 3030 2e35 222c 2022  e("0:01:00.5", "
+00011700: 303a 3031 3a30 302e 3622 290a 2020 2020  0:01:00.6").    
+00011710: 2020 2020 2236 302e 353a 3630 2e36 220a      "60.5:60.6".
+00011720: 2020 2020 2222 220a 2020 2020 7374 6172      """.    star
+00011730: 745f 6d61 7463 6820 3d20 7265 6765 782e  t_match = regex.
+00011740: 7365 6172 6368 2872 225e 285c 642b 293a  search(r"^(\d+):
+00011750: 285b 302d 355d 5b30 2d39 5d29 3a28 5b30  ([0-5][0-9]):([0
+00011760: 2d35 5d5b 302d 395d 283f 3a5c 2e5b 302d  -5][0-9](?:\.[0-
+00011770: 395d 2b29 3f29 2422 2c20 7374 6172 7429  9]+)?)$", start)
+00011780: 0a20 2020 2065 6e64 5f6d 6174 6368 203d  .    end_match =
+00011790: 2072 6567 6578 2e6d 6174 6368 2872 225e   regex.match(r"^
+000117a0: 285c 642b 293a 285b 302d 355d 5b30 2d39  (\d+):([0-5][0-9
+000117b0: 5d29 3a28 5b30 2d35 5d5b 302d 395d 283f  ]):([0-5][0-9](?
+000117c0: 3a5c 2e5b 302d 395d 2b29 3f29 2422 2c20  :\.[0-9]+)?)$", 
+000117d0: 656e 6429 0a20 2020 2069 6620 6e6f 7420  end).    if not 
+000117e0: 7374 6172 745f 6d61 7463 6820 6f72 206e  start_match or n
+000117f0: 6f74 2065 6e64 5f6d 6174 6368 3a0a 2020  ot end_match:.  
+00011800: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00011810: 6545 7272 6f72 2822 5468 6520 7374 6172  eError("The star
+00011820: 7420 616e 6420 656e 6420 7661 6c75 6573  t and end values
+00011830: 206d 7573 7420 6265 2069 6e20 7468 6520   must be in the 
+00011840: 666f 726d 6174 2027 4828 4829 3a4d 4d3a  format 'H(H):MM:
+00011850: 5353 282e 7329 2722 290a 2020 2020 7374  SS(.s)'").    st
+00011860: 6172 745f 682c 2073 7461 7274 5f6d 2c20  art_h, start_m, 
+00011870: 7374 6172 745f 7320 3d20 7374 6172 745f  start_s = start_
+00011880: 6d61 7463 682e 6772 6f75 7073 2829 0a20  match.groups(). 
+00011890: 2020 2065 6e64 5f68 2c20 656e 645f 6d2c     end_h, end_m,
+000118a0: 2065 6e64 5f73 203d 2065 6e64 5f6d 6174   end_s = end_mat
+000118b0: 6368 2e67 726f 7570 7328 290a 2020 2020  ch.groups().    
+000118c0: 7374 6172 745f 7365 636f 6e64 7320 3d20  start_seconds = 
+000118d0: 696e 7428 7374 6172 745f 6829 202a 2033  int(start_h) * 3
+000118e0: 3630 3020 2b20 696e 7428 7374 6172 745f  600 + int(start_
+000118f0: 6d29 202a 2036 3020 2b20 666c 6f61 7428  m) * 60 + float(
+00011900: 7374 6172 745f 7329 0a20 2020 2065 6e64  start_s).    end
+00011910: 5f73 6563 6f6e 6473 203d 2069 6e74 2865  _seconds = int(e
+00011920: 6e64 5f68 2920 2a20 3336 3030 202b 2069  nd_h) * 3600 + i
+00011930: 6e74 2865 6e64 5f6d 2920 2a20 3630 202b  nt(end_m) * 60 +
+00011940: 2066 6c6f 6174 2865 6e64 5f73 290a 2020   float(end_s).  
+00011950: 2020 7374 6172 745f 7365 636f 6e64 7320    start_seconds 
+00011960: 3d20 696e 7428 7374 6172 745f 7365 636f  = int(start_seco
+00011970: 6e64 7329 2069 6620 7374 6172 745f 7365  nds) if start_se
+00011980: 636f 6e64 732e 6973 5f69 6e74 6567 6572  conds.is_integer
+00011990: 2829 2065 6c73 6520 7374 6172 745f 7365  () else start_se
+000119a0: 636f 6e64 730a 2020 2020 656e 645f 7365  conds.    end_se
+000119b0: 636f 6e64 7320 3d20 696e 7428 656e 645f  conds = int(end_
+000119c0: 7365 636f 6e64 7329 2069 6620 656e 645f  seconds) if end_
+000119d0: 7365 636f 6e64 732e 6973 5f69 6e74 6567  seconds.is_integ
+000119e0: 6572 2829 2065 6c73 6520 656e 645f 7365  er() else end_se
+000119f0: 636f 6e64 730a 2020 2020 6966 2073 7461  conds.    if sta
+00011a00: 7274 5f73 6563 6f6e 6473 203e 2065 6e64  rt_seconds > end
+00011a10: 5f73 6563 6f6e 6473 3a0a 2020 2020 2020  _seconds:.      
+00011a20: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00011a30: 6f72 2822 5468 6520 7374 6172 7420 7661  or("The start va
+00011a40: 6c75 6520 6d75 7374 2062 6520 736d 616c  lue must be smal
+00011a50: 6c65 7220 7468 616e 2074 6865 2065 6e64  ler than the end
+00011a60: 2076 616c 7565 2229 0a20 2020 2072 6574   value").    ret
+00011a70: 7572 6e20 6622 7b73 7461 7274 5f73 6563  urn f"{start_sec
+00011a80: 6f6e 6473 7d3a 7b65 6e64 5f73 6563 6f6e  onds}:{end_secon
+00011a90: 6473 7d22 0a0a 0a64 6566 2063 7265 6174  ds}"...def creat
+00011aa0: 655f 6a73 6f6e 5f65 7863 656c 5f6c 6973  e_json_excel_lis
+00011ab0: 745f 6d61 7070 696e 6728 0a20 2020 2070  t_mapping(.    p
+00011ac0: 6174 685f 746f 5f6a 736f 6e3a 2073 7472  ath_to_json: str
+00011ad0: 2c0a 2020 2020 6c69 7374 5f6e 616d 653a  ,.    list_name:
+00011ae0: 2073 7472 2c0a 2020 2020 6578 6365 6c5f   str,.    excel_
+00011af0: 7661 6c75 6573 3a20 4974 6572 6162 6c65  values: Iterable
+00011b00: 5b73 7472 5d2c 0a20 2020 2073 6570 3a20  [str],.    sep: 
+00011b10: 7374 7220 3d20 272b 222a c3a7 2526 2f28  str = '+"*..%&/(
+00011b20: 293d 272c 0a20 2020 2063 6f72 7265 6374  )=',.    correct
+00011b30: 696f 6e73 3a20 4f70 7469 6f6e 616c 5b64  ions: Optional[d
+00011b40: 6963 745b 7374 722c 2073 7472 5d5d 203d  ict[str, str]] =
+00011b50: 204e 6f6e 652c 0a29 202d 3e20 6469 6374   None,.) -> dict
+00011b60: 5b73 7472 2c20 7374 725d 3a0a 2020 2020  [str, str]:.    
+00011b70: 2222 220a 2020 2020 4f66 7465 6e2c 2064  """.    Often, d
+00011b80: 6174 6120 736f 7572 6365 7320 636f 6e74  ata sources cont
+00011b90: 6169 6e20 6c69 7374 2076 616c 7565 7320  ain list values 
+00011ba0: 7468 6174 2061 7265 6e27 7420 6964 656e  that aren't iden
+00011bb0: 7469 6361 6c20 746f 2074 6865 206e 616d  tical to the nam
+00011bc0: 6520 6f66 2074 6865 206e 6f64 6520 696e  e of the node in
+00011bd0: 2074 6865 206c 6973 7420 6f66 2074 6865   the list of the
+00011be0: 204a 534f 4e0a 2020 2020 7072 6f6a 6563   JSON.    projec
+00011bf0: 7420 6669 6c65 2028 636f 6c6c 6f71 7569  t file (colloqui
+00011c00: 616c 6c79 3a20 6f6e 746f 6c6f 6779 292e  ally: ontology).
+00011c10: 2049 6e20 6f72 6465 7220 746f 2063 7265   In order to cre
+00011c20: 6174 6520 6120 636f 7272 6563 7420 584d  ate a correct XM
+00011c30: 4c20 666f 7220 7468 6520 6064 7370 2d74  L for the `dsp-t
+00011c40: 6f6f 6c73 2078 6d6c 7570 6c6f 6164 602c  ools xmlupload`,
+00011c50: 2061 206d 6170 7069 6e67 2069 730a 2020   a mapping is.  
+00011c60: 2020 6e65 6365 7373 6172 792e 2054 6869    necessary. Thi
+00011c70: 7320 6675 6e63 7469 6f6e 2074 616b 6573  s function takes
+00011c80: 2061 204a 534f 4e20 6c69 7374 2061 6e64   a JSON list and
+00011c90: 2061 6e20 4578 6365 6c20 636f 6c75 6d6e   an Excel column
+00011ca0: 2063 6f6e 7461 696e 696e 6720 6c69 7374   containing list
+00011cb0: 2d76 616c 7565 732c 2061 6e64 2074 7269  -values, and tri
+00011cc0: 6573 2074 6f20 6d61 7463 6820 7468 656d  es to match them
+00011cd0: 0a20 2020 2061 7574 6f6d 6174 6963 616c  .    automatical
+00011ce0: 6c79 2062 6173 6564 206f 6e20 7369 6d69  ly based on simi
+00011cf0: 6c61 7269 7479 2e20 5468 6520 7265 7375  larity. The resu
+00011d00: 6c74 2069 7320 6120 6469 6374 206f 6620  lt is a dict of 
+00011d10: 7468 6520 666f 726d 207b 6578 6365 6c5f  the form {excel_
+00011d20: 7661 6c75 653a 206c 6973 745f 6e6f 6465  value: list_node
+00011d30: 5f6e 616d 657d 2e0a 0a20 2020 2041 6c74  _name}...    Alt
+00011d40: 6572 6e61 7469 7665 6c79 2c20 636f 6e73  ernatively, cons
+00011d50: 6964 6572 2075 7369 6e67 2074 6865 2066  ider using the f
+00011d60: 756e 6374 696f 6e20 6372 6561 7465 5f6a  unction create_j
+00011d70: 736f 6e5f 6c69 7374 5f6d 6170 7069 6e67  son_list_mapping
+00011d80: 2829 2c20 7768 6963 6820 616c 736f 2062  (), which also b
+00011d90: 7569 6c64 7320 6120 6469 6374 696f 6e61  uilds a dictiona
+00011da0: 7279 2c0a 2020 2020 6275 7420 6672 6f6d  ry,.    but from
+00011db0: 2074 6865 206e 616d 6573 2061 6e64 206c   the names and l
+00011dc0: 6162 656c 7320 696e 2074 6865 204a 534f  abels in the JSO
+00011dd0: 4e20 6c69 7374 2c20 7768 6963 6820 6973  N list, which is
+00011de0: 206c 6573 7320 6572 726f 722d 7072 6f6e   less error-pron
+00011df0: 6520 7468 616e 2074 6869 7320 6675 6e63  e than this func
+00011e00: 7469 6f6e 2773 2061 7070 726f 6163 682e  tion's approach.
+00011e10: 2048 6f77 6576 6572 2c0a 2020 2020 7468   However,.    th
+00011e20: 6973 2066 756e 6374 696f 6e20 6861 7320  is function has 
+00011e30: 7468 6520 6164 7661 6e74 6167 6520 7468  the advantage th
+00011e40: 6174 2069 7420 6576 656e 2077 6f72 6b73  at it even works
+00011e50: 2077 6865 6e20 796f 7572 2064 6174 6120   when your data 
+00011e60: 736f 7572 6365 2064 6f65 736e 2774 2075  source doesn't u
+00011e70: 7365 2074 6865 206c 6973 7420 6c61 6265  se the list labe
+00011e80: 6c73 2063 6f72 7265 6374 6c79 2e0a 0a20  ls correctly... 
+00011e90: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00011ea0: 2070 6174 685f 746f 5f6a 736f 6e3a 2070   path_to_json: p
+00011eb0: 6174 6820 746f 2074 6865 204a 534f 4e20  ath to the JSON 
+00011ec0: 7072 6f6a 6563 7420 6669 6c65 0a20 2020  project file.   
+00011ed0: 2020 2020 206c 6973 745f 6e61 6d65 3a20       list_name: 
+00011ee0: 6e61 6d65 206f 6620 7468 6520 6c69 7374  name of the list
+00011ef0: 2069 6e20 7468 6520 4a53 4f4e 2070 726f   in the JSON pro
+00011f00: 6a65 6374 2066 696c 6520 2863 616e 2061  ject file (can a
+00011f10: 6c73 6f20 6265 2061 206e 6573 7465 6420  lso be a nested 
+00011f20: 6c69 7374 290a 2020 2020 2020 2020 6578  list).        ex
+00011f30: 6365 6c5f 7661 6c75 6573 3a20 7468 6520  cel_values: the 
+00011f40: 4578 6365 6c20 636f 6c75 6d6e 2028 652e  Excel column (e.
+00011f50: 672e 2061 7320 6c69 7374 2920 7769 7468  g. as list) with
+00011f60: 2074 6865 206c 6973 7420 7661 6c75 6573   the list values
+00011f70: 2069 6e20 6974 0a20 2020 2020 2020 2073   in it.        s
+00011f80: 6570 3a20 7365 7061 7261 746f 7220 7374  ep: separator st
+00011f90: 7269 6e67 2c20 6966 2074 6865 2063 656c  ring, if the cel
+00011fa0: 6c73 2069 6e20 7468 6520 4578 6365 6c20  ls in the Excel 
+00011fb0: 636f 6e74 6169 6e20 6d6f 7265 2074 6861  contain more tha
+00011fc0: 6e20 6f6e 6520 6c69 7374 2065 6e74 7279  n one list entry
+00011fd0: 0a20 2020 2020 2020 2063 6f72 7265 6374  .        correct
+00011fe0: 696f 6e73 3a20 6469 6374 2077 6974 6820  ions: dict with 
+00011ff0: 7772 6f6e 6720 656e 7472 6965 732c 2065  wrong entries, e
+00012000: 6163 6820 706f 696e 7469 6e67 2074 6f20  ach pointing to 
+00012010: 6974 7320 636f 7272 6563 7420 636f 756e  its correct coun
+00012020: 7465 7270 6172 740a 0a20 2020 2052 6169  terpart..    Rai
+00012030: 7365 733a 0a20 2020 2020 2020 2057 6172  ses:.        War
+00012040: 6e69 6e67 3a20 6966 2074 6865 7265 2069  ning: if there i
+00012050: 7320 616e 2045 7863 656c 2076 616c 7565  s an Excel value
+00012060: 2074 6861 7420 636f 756c 646e 2774 2062   that couldn't b
+00012070: 6520 6d61 7463 6865 640a 2020 2020 2020  e matched.      
+00012080: 2020 4578 6365 7074 696f 6e3a 2069 6620    Exception: if 
+00012090: 7468 6520 7061 7468 2064 6f65 736e 2774  the path doesn't
+000120a0: 2070 6f69 6e74 2074 6f20 6120 4a53 4f4e   point to a JSON
+000120b0: 2070 726f 6a65 6374 2066 696c 650a 0a20   project file.. 
+000120c0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000120d0: 2020 2020 6469 6374 206f 6620 7468 6520      dict of the 
+000120e0: 666f 726d 2060 607b 6578 6365 6c5f 7661  form ``{excel_va
+000120f0: 6c75 653a 206c 6973 745f 6e6f 6465 5f6e  lue: list_node_n
+00012100: 616d 657d 6060 2e0a 2020 2020 2020 2020  ame}``..        
+00012110: 2020 2020 4576 6572 7920 6578 6365 6c5f      Every excel_
+00012120: 7661 6c75 6520 6973 2073 7472 6970 7065  value is strippe
+00012130: 642c 2061 6e64 2061 6c73 6f20 7072 6573  d, and also pres
+00012140: 656e 7420 696e 2061 206c 6f77 6572 6361  ent in a lowerca
+00012150: 7365 2066 6f72 6d2e 0a0a 2020 2020 4578  se form...    Ex
+00012160: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
+00012170: 3e3e 3e20 6a73 6f6e 5f6c 6973 745f 6e6f  >>> json_list_no
+00012180: 6465 7320 3d20 5b0a 2020 2020 2020 2020  des = [.        
+00012190: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000121a0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+000121b0: 616d 6522 3a20 2267 6972 6166 6665 222c  ame": "giraffe",
+000121c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000121d0: 2020 2020 2022 6c61 6265 6c73 223a 207b       "labels": {
+000121e0: 2265 6e22 3a20 2267 6972 6166 6665 227d  "en": "giraffe"}
+000121f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012200: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00012210: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00012220: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+00012230: 3a20 2261 6e74 656c 6f70 6522 2c0a 2020  : "antelope",.  
+00012240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012250: 2020 226c 6162 656c 7322 3a20 7b22 656e    "labels": {"en
+00012260: 223a 2022 616e 7465 6c6f 7065 227d 0a20  ": "antelope"}. 
+00012270: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00012280: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+00012290: 2020 2020 2020 203e 3e3e 2065 7863 656c         >>> excel
+000122a0: 5f72 6f77 5f31 203d 205b 2247 6972 6166  _row_1 = ["Giraf
+000122b0: 6665 6568 2022 2c20 2220 416e 7469 6c6f  feeh ", " Antilo
+000122c0: 7570 6522 2c20 2247 6972 7261 6666 6520  upe", "Girraffe 
+000122d0: 2c20 416e 7469 6c6f 7570 6520 225d 0a20  , Antiloupe "]. 
+000122e0: 2020 2020 2020 203e 3e3e 206a 736f 6e5f         >>> json_
+000122f0: 6578 6365 6c5f 6c69 7374 5f6d 6170 7069  excel_list_mappi
+00012300: 6e67 203d 207b 0a20 2020 2020 2020 2020  ng = {.         
+00012310: 2020 2020 2020 2022 4769 7261 6666 6565         "Giraffee
+00012320: 6822 3a20 2267 6972 6166 6665 222c 0a20  h": "giraffe",. 
+00012330: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00012340: 6769 7261 6666 6565 6822 3a20 2267 6972  giraffeeh": "gir
+00012350: 6166 6665 222c 0a20 2020 2020 2020 2020  affe",.         
+00012360: 2020 2020 2020 2022 4769 7272 6166 6665         "Girraffe
+00012370: 223a 2022 6769 7261 6666 6522 2c0a 2020  ": "giraffe",.  
+00012380: 2020 2020 2020 2020 2020 2020 2020 2267                "g
+00012390: 6972 7261 6666 6522 3a20 2267 6972 6166  irraffe": "giraf
+000123a0: 6665 222c 0a20 2020 2020 2020 2020 2020  fe",.           
+000123b0: 2020 2020 2022 416e 7469 6c6f 7570 6522       "Antiloupe"
+000123c0: 3a20 2261 6e74 656c 6f70 6522 2c0a 2020  : "antelope",.  
+000123d0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+000123e0: 6e74 696c 6f75 7065 223a 2022 616e 7465  ntiloupe": "ante
+000123f0: 6c6f 7065 220a 2020 2020 2020 2020 2020  lope".          
+00012400: 2020 7d0a 2020 2020 2222 220a 0a20 2020    }.    """..   
+00012410: 2023 2061 766f 6964 206d 7574 6162 6c65   # avoid mutable
+00012420: 2064 6566 6175 6c74 2061 7267 756d 656e   default argumen
+00012430: 740a 2020 2020 636f 7272 6563 7469 6f6e  t.    correction
+00012440: 7320 3d20 636f 7272 6563 7469 6f6e 7320  s = corrections 
+00012450: 6f72 207b 7d0a 0a20 2020 2023 2073 706c  or {}..    # spl
+00012460: 6974 2074 6865 2076 616c 7565 732c 2069  it the values, i
+00012470: 6620 6e65 6365 7373 6172 790a 2020 2020  f necessary.    
+00012480: 6578 6365 6c5f 7661 6c75 6573 5f6e 6577  excel_values_new
+00012490: 203d 205b 5d0a 2020 2020 666f 7220 7661   = [].    for va
+000124a0: 6c20 696e 2065 7863 656c 5f76 616c 7565  l in excel_value
+000124b0: 733a 0a20 2020 2020 2020 2069 6620 6973  s:.        if is
+000124c0: 696e 7374 616e 6365 2876 616c 2c20 7374  instance(val, st
+000124d0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000124e0: 6578 6365 6c5f 7661 6c75 6573 5f6e 6577  excel_values_new
+000124f0: 2e65 7874 656e 6428 5b78 2e73 7472 6970  .extend([x.strip
+00012500: 2829 2066 6f72 2078 2069 6e20 7661 6c2e  () for x in val.
+00012510: 7370 6c69 7428 7365 7029 2069 6620 785d  split(sep) if x]
+00012520: 290a 0a20 2020 2023 2072 6561 6420 7468  )..    # read th
+00012530: 6520 6c69 7374 206f 6620 7468 6520 4a53  e list of the JS
+00012540: 4f4e 2070 726f 6a65 6374 2028 776f 726b  ON project (work
+00012550: 7320 616c 736f 2066 6f72 206e 6573 7465  s also for neste
+00012560: 6420 6c69 7374 7329 0a20 2020 2077 6974  d lists).    wit
+00012570: 6820 6f70 656e 2870 6174 685f 746f 5f6a  h open(path_to_j
+00012580: 736f 6e2c 2065 6e63 6f64 696e 673d 2275  son, encoding="u
+00012590: 7466 2d38 2229 2061 7320 663a 0a20 2020  tf-8") as f:.   
+000125a0: 2020 2020 206a 736f 6e5f 6669 6c65 203d       json_file =
+000125b0: 206a 736f 6e2e 6c6f 6164 2866 290a 2020   json.load(f).  
+000125c0: 2020 6a73 6f6e 5f73 7562 7365 7420 3d20    json_subset = 
+000125d0: 5b5d 0a20 2020 2066 6f72 2065 6c65 6d20  [].    for elem 
+000125e0: 696e 206a 736f 6e5f 6669 6c65 5b22 7072  in json_file["pr
+000125f0: 6f6a 6563 7422 5d5b 226c 6973 7473 225d  oject"]["lists"]
+00012600: 3a0a 2020 2020 2020 2020 6966 2065 6c65  :.        if ele
+00012610: 6d5b 226e 616d 6522 5d20 3d3d 206c 6973  m["name"] == lis
+00012620: 745f 6e61 6d65 3a0a 2020 2020 2020 2020  t_name:.        
+00012630: 2020 2020 6a73 6f6e 5f73 7562 7365 7420      json_subset 
+00012640: 3d20 656c 656d 5b22 6e6f 6465 7322 5d0a  = elem["nodes"].
+00012650: 2020 2020 6a73 6f6e 5f76 616c 7565 7320      json_values 
+00012660: 3d20 7365 7428 5f6e 6573 7465 645f 6469  = set(_nested_di
+00012670: 6374 5f76 616c 7565 735f 6974 6572 6174  ct_values_iterat
+00012680: 6f72 286a 736f 6e5f 7375 6273 6574 2929  or(json_subset))
+00012690: 0a0a 2020 2020 2320 6275 696c 6420 6469  ..    # build di
+000126a0: 6374 696f 6e61 7279 2077 6974 6820 7468  ctionary with th
+000126b0: 6520 6d61 7070 696e 672c 2062 6173 6564  e mapping, based
+000126c0: 206f 6e20 7374 7269 6e67 2073 696d 696c   on string simil
+000126d0: 6172 6974 790a 2020 2020 7265 7320 3d20  arity.    res = 
+000126e0: 7b7d 0a20 2020 2066 6f72 2065 7863 656c  {}.    for excel
+000126f0: 5f76 616c 7565 2069 6e20 6578 6365 6c5f  _value in excel_
+00012700: 7661 6c75 6573 5f6e 6577 3a0a 2020 2020  values_new:.    
+00012710: 2020 2020 6578 6365 6c5f 7661 6c75 655f      excel_value_
+00012720: 636f 7272 6563 7465 6420 3d20 636f 7272  corrected = corr
+00012730: 6563 7469 6f6e 732e 6765 7428 6578 6365  ections.get(exce
+00012740: 6c5f 7661 6c75 652c 2065 7863 656c 5f76  l_value, excel_v
+00012750: 616c 7565 290a 2020 2020 2020 2020 6578  alue).        ex
+00012760: 6365 6c5f 7661 6c75 655f 7369 6d70 6c20  cel_value_simpl 
+00012770: 3d20 7369 6d70 6c69 6679 5f6e 616d 6528  = simplify_name(
+00012780: 6578 6365 6c5f 7661 6c75 655f 636f 7272  excel_value_corr
+00012790: 6563 7465 6429 2020 2320 696e 6372 6561  ected)  # increa
+000127a0: 7365 206d 6174 6368 2070 726f 6261 6269  se match probabi
+000127b0: 6c69 7479 2062 7920 7265 6d6f 7669 6e67  lity by removing
+000127c0: 2069 6c6c 6567 616c 2063 6861 7273 0a20   illegal chars. 
+000127d0: 2020 2020 2020 2069 6620 6d61 7463 6865         if matche
+000127e0: 7320 3a3d 2064 6966 666c 6962 2e67 6574  s := difflib.get
+000127f0: 5f63 6c6f 7365 5f6d 6174 6368 6573 280a  _close_matches(.
+00012800: 2020 2020 2020 2020 2020 2020 776f 7264              word
+00012810: 3d65 7863 656c 5f76 616c 7565 5f73 696d  =excel_value_sim
+00012820: 706c 2c0a 2020 2020 2020 2020 2020 2020  pl,.            
+00012830: 706f 7373 6962 696c 6974 6965 733d 6a73  possibilities=js
+00012840: 6f6e 5f76 616c 7565 732c 0a20 2020 2020  on_values,.     
+00012850: 2020 2020 2020 206e 3d31 2c0a 2020 2020         n=1,.    
+00012860: 2020 2020 2020 2020 6375 746f 6666 3d30          cutoff=0
+00012870: 2e36 2c0a 2020 2020 2020 2020 293a 0a20  .6,.        ):. 
+00012880: 2020 2020 2020 2020 2020 2072 6573 5b65             res[e
+00012890: 7863 656c 5f76 616c 7565 5d20 3d20 6d61  xcel_value] = ma
+000128a0: 7463 6865 735b 305d 0a20 2020 2020 2020  tches[0].       
+000128b0: 2020 2020 2072 6573 5b65 7863 656c 5f76       res[excel_v
+000128c0: 616c 7565 2e6c 6f77 6572 2829 5d20 3d20  alue.lower()] = 
+000128d0: 6d61 7463 6865 735b 305d 0a20 2020 2020  matches[0].     
+000128e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000128f0: 2020 2020 206d 7367 203d 2028 0a20 2020       msg = (.   
+00012900: 2020 2020 2020 2020 2020 2020 2066 2244               f"D
+00012910: 6964 206e 6f74 2066 696e 6420 6120 636c  id not find a cl
+00012920: 6f73 6520 6d61 7463 6820 746f 2074 6865  ose match to the
+00012930: 2065 7863 656c 206c 6973 7420 656e 7472   excel list entr
+00012940: 7920 277b 6578 6365 6c5f 7661 6c75 657d  y '{excel_value}
+00012950: 2720 220a 2020 2020 2020 2020 2020 2020  ' ".            
+00012960: 2020 2020 6622 616d 6f6e 6720 7468 6520      f"among the 
+00012970: 7661 6c75 6573 2069 6e20 7468 6520 4a53  values in the JS
+00012980: 4f4e 2070 726f 6a65 6374 206c 6973 7420  ON project list 
+00012990: 277b 6c69 7374 5f6e 616d 657d 2722 0a20  '{list_name}'". 
+000129a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000129b0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+000129c0: 732e 7761 726e 2844 7370 546f 6f6c 7355  s.warn(DspToolsU
+000129d0: 7365 7257 6172 6e69 6e67 286d 7367 2929  serWarning(msg))
+000129e0: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+000129f0: 0a0a 0a64 6566 205f 6e65 7374 6564 5f64  ...def _nested_d
+00012a00: 6963 745f 7661 6c75 6573 5f69 7465 7261  ict_values_itera
+00012a10: 746f 7228 6469 6374 733a 206c 6973 745b  tor(dicts: list[
+00012a20: 6469 6374 5b73 7472 2c20 416e 795d 5d29  dict[str, Any]])
+00012a30: 202d 3e20 4974 6572 6162 6c65 5b73 7472   -> Iterable[str
+00012a40: 5d3a 0a20 2020 2022 2222 0a20 2020 2059  ]:.    """.    Y
+00012a50: 6965 6c64 2061 6c6c 2076 616c 7565 7320  ield all values 
+00012a60: 6f66 2061 206e 6573 7465 6420 6469 6374  of a nested dict
+00012a70: 696f 6e61 7279 2e0a 0a20 2020 2041 7267  ionary...    Arg
+00012a80: 733a 0a20 2020 2020 2020 2064 6963 7473  s:.        dicts
+00012a90: 3a20 6c69 7374 206f 6620 6e65 7374 6564  : list of nested
+00012aa0: 2064 6963 7469 6f6e 6172 6965 730a 0a20   dictionaries.. 
+00012ab0: 2020 2059 6965 6c64 733a 0a20 2020 2020     Yields:.     
+00012ac0: 2020 2076 616c 7565 7320 6f66 2074 6865     values of the
+00012ad0: 206e 6573 7465 6420 6469 6374 696f 6e61   nested dictiona
+00012ae0: 7269 6573 0a20 2020 2022 2222 0a20 2020  ries.    """.   
+00012af0: 2023 2043 7265 6469 7473 3a20 6874 7470   # Credits: http
+00012b00: 733a 2f2f 7468 6973 706f 696e 7465 722e  s://thispointer.
+00012b10: 636f 6d2f 7079 7468 6f6e 2d69 7465 7261  com/python-itera
+00012b20: 7465 2d6c 6f6f 702d 6f76 6572 2d61 6c6c  te-loop-over-all
+00012b30: 2d6e 6573 7465 642d 6469 6374 696f 6e61  -nested-dictiona
+00012b40: 7279 2d76 616c 7565 732f 0a20 2020 2066  ry-values/.    f
+00012b50: 6f72 205f 6469 6374 2069 6e20 6469 6374  or _dict in dict
+00012b60: 733a 0a20 2020 2020 2020 2069 6620 226e  s:.        if "n
+00012b70: 6f64 6573 2220 696e 205f 6469 6374 3a0a  odes" in _dict:.
+00012b80: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+00012b90: 6420 6672 6f6d 205f 6e65 7374 6564 5f64  d from _nested_d
+00012ba0: 6963 745f 7661 6c75 6573 5f69 7465 7261  ict_values_itera
+00012bb0: 746f 7228 5f64 6963 745b 226e 6f64 6573  tor(_dict["nodes
+00012bc0: 225d 290a 2020 2020 2020 2020 6966 2022  "]).        if "
+00012bd0: 6e61 6d65 2220 696e 205f 6469 6374 3a0a  name" in _dict:.
+00012be0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+00012bf0: 6420 5f64 6963 745b 226e 616d 6522 5d0a  d _dict["name"].
+00012c00: 0a0a 6465 6620 6372 6561 7465 5f6a 736f  ..def create_jso
+00012c10: 6e5f 6c69 7374 5f6d 6170 7069 6e67 280a  n_list_mapping(.
+00012c20: 2020 2020 7061 7468 5f74 6f5f 6a73 6f6e      path_to_json
+00012c30: 3a20 7374 722c 0a20 2020 206c 6973 745f  : str,.    list_
+00012c40: 6e61 6d65 3a20 7374 722c 0a20 2020 206c  name: str,.    l
+00012c50: 616e 6775 6167 655f 6c61 6265 6c3a 2073  anguage_label: s
+00012c60: 7472 2c0a 2920 2d3e 2064 6963 745b 7374  tr,.) -> dict[st
+00012c70: 722c 2073 7472 5d3a 0a20 2020 2022 2222  r, str]:.    """
+00012c80: 0a20 2020 204f 6674 656e 2c20 6461 7461  .    Often, data
+00012c90: 2073 6f75 7263 6573 2063 6f6e 7461 696e   sources contain
+00012ca0: 206c 6973 7420 7661 6c75 6573 206e 616d   list values nam
+00012cb0: 6564 2061 6674 6572 2074 6865 2022 6c61  ed after the "la
+00012cc0: 6265 6c22 206f 6620 7468 6520 4a53 4f4e  bel" of the JSON
+00012cd0: 2070 726f 6a65 6374 206c 6973 7420 6e6f   project list no
+00012ce0: 6465 2c20 696e 7374 6561 6420 6f66 2074  de, instead of t
+00012cf0: 6865 2022 6e61 6d65 220a 2020 2020 7768  he "name".    wh
+00012d00: 6963 6820 6973 206e 6565 6465 6420 666f  ich is needed fo
+00012d10: 7220 7468 6520 6064 7370 2d74 6f6f 6c73  r the `dsp-tools
+00012d20: 2078 6d6c 7570 6c6f 6164 602e 2049 6e20   xmlupload`. In 
+00012d30: 6f72 6465 7220 746f 2063 7265 6174 6520  order to create 
+00012d40: 6120 636f 7272 6563 7420 584d 4c2c 2079  a correct XML, y
+00012d50: 6f75 206e 6565 6420 6120 6469 6374 696f  ou need a dictio
+00012d60: 6e61 7279 2074 6861 7420 6d61 7073 2074  nary that maps t
+00012d70: 6865 0a20 2020 2022 6c61 6265 6c73 2220  he.    "labels" 
+00012d80: 746f 2074 6865 6972 2063 6f72 7265 6374  to their correct
+00012d90: 2022 6e61 6d65 7322 2e0a 0a20 2020 2041   "names"...    A
+00012da0: 6c74 6572 6e61 7469 7665 6c79 2c20 636f  lternatively, co
+00012db0: 6e73 6964 6572 2075 7369 6e67 2074 6865  nsider using the
+00012dc0: 206d 6574 686f 6420 6372 6561 7465 5f6a   method create_j
+00012dd0: 736f 6e5f 6578 6365 6c5f 6c69 7374 5f6d  son_excel_list_m
+00012de0: 6170 7069 6e67 2829 2c20 7768 6963 6820  apping(), which 
+00012df0: 616c 736f 2063 7265 6174 6573 2061 2064  also creates a d
+00012e00: 6963 7469 6f6e 6172 792c 2062 7574 206d  ictionary, but m
+00012e10: 6170 730a 2020 2020 7661 6c75 6573 2066  aps.    values f
+00012e20: 726f 6d20 796f 7572 2064 6174 6120 736f  rom your data so
+00012e30: 7572 6365 2074 6f20 6c69 7374 206e 6f64  urce to list nod
+00012e40: 6520 6e61 6d65 7320 6672 6f6d 2074 6865  e names from the
+00012e50: 204a 534f 4e20 7072 6f6a 6563 7420 6669   JSON project fi
+00012e60: 6c65 2c20 6261 7365 6420 6f6e 2073 696d  le, based on sim
+00012e70: 696c 6172 6974 792e 0a0a 2020 2020 4172  ilarity...    Ar
+00012e80: 6773 3a0a 2020 2020 2020 2020 7061 7468  gs:.        path
+00012e90: 5f74 6f5f 6a73 6f6e 3a20 7061 7468 2074  _to_json: path t
+00012ea0: 6f20 6120 4a53 4f4e 2070 726f 6a65 6374  o a JSON project
+00012eb0: 2066 696c 6520 2861 2e6b 2e61 2e20 6f6e   file (a.k.a. on
+00012ec0: 746f 6c6f 6779 290a 2020 2020 2020 2020  tology).        
+00012ed0: 6c69 7374 5f6e 616d 653a 206e 616d 6520  list_name: name 
+00012ee0: 6f66 2061 206c 6973 7420 696e 2074 6865  of a list in the
+00012ef0: 204a 534f 4e20 7072 6f6a 6563 7420 2877   JSON project (w
+00012f00: 6f72 6b73 2061 6c73 6f20 666f 7220 6e65  orks also for ne
+00012f10: 7374 6564 206c 6973 7473 290a 2020 2020  sted lists).    
+00012f20: 2020 2020 6c61 6e67 7561 6765 5f6c 6162      language_lab
+00012f30: 656c 3a20 7768 6963 6820 6c61 6e67 7561  el: which langua
+00012f40: 6765 206f 6620 7468 6520 6c61 6265 6c20  ge of the label 
+00012f50: 746f 2063 686f 6f73 650a 0a20 2020 2052  to choose..    R
+00012f60: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00012f70: 6120 6469 6374 696f 6e61 7279 206f 6620  a dictionary of 
+00012f80: 7468 6520 666f 726d 207b 6c61 6265 6c3a  the form {label:
+00012f90: 206e 616d 657d 0a20 2020 2022 2222 0a20   name}.    """. 
+00012fa0: 2020 2077 6974 6820 6f70 656e 2870 6174     with open(pat
+00012fb0: 685f 746f 5f6a 736f 6e2c 2065 6e63 6f64  h_to_json, encod
+00012fc0: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+00012fd0: 663a 0a20 2020 2020 2020 206a 736f 6e5f  f:.        json_
+00012fe0: 6669 6c65 203d 206a 736f 6e2e 6c6f 6164  file = json.load
+00012ff0: 2866 290a 2020 2020 6a73 6f6e 5f73 7562  (f).    json_sub
+00013000: 7365 7420 3d20 5b78 2066 6f72 2078 2069  set = [x for x i
+00013010: 6e20 6a73 6f6e 5f66 696c 655b 2270 726f  n json_file["pro
+00013020: 6a65 6374 225d 5b22 6c69 7374 7322 5d20  ject"]["lists"] 
+00013030: 6966 2078 5b22 6e61 6d65 225d 203d 3d20  if x["name"] == 
+00013040: 6c69 7374 5f6e 616d 655d 0a20 2020 2023  list_name].    #
+00013050: 206a 736f 6e5f 7375 6273 6574 2069 7320   json_subset is 
+00013060: 6120 6c69 7374 2063 6f6e 7461 696e 696e  a list containin
+00013070: 6720 6f6e 6520 6974 656d 2c20 6e61 6d65  g one item, name
+00013080: 6c79 2074 6865 206a 736f 6e20 6f62 6a65  ly the json obje
+00013090: 6374 2063 6f6e 7461 696e 696e 6720 7468  ct containing th
+000130a0: 6520 656e 7469 7265 206a 736f 6e2d 6c69  e entire json-li
+000130b0: 7374 0a0a 2020 2020 7265 7320 3d20 7b7d  st..    res = {}
+000130c0: 0a20 2020 2066 6f72 206c 6162 656c 2c20  .    for label, 
+000130d0: 6e61 6d65 2069 6e20 5f6e 616d 655f 6c61  name in _name_la
+000130e0: 6265 6c5f 6d61 7070 6572 5f69 7465 7261  bel_mapper_itera
+000130f0: 746f 7228 6a73 6f6e 5f73 7562 7365 742c  tor(json_subset,
+00013100: 206c 616e 6775 6167 655f 6c61 6265 6c29   language_label)
+00013110: 3a0a 2020 2020 2020 2020 6966 206e 616d  :.        if nam
+00013120: 6520 213d 206c 6973 745f 6e61 6d65 3a0a  e != list_name:.
+00013130: 2020 2020 2020 2020 2020 2020 7265 735b              res[
+00013140: 6c61 6265 6c5d 203d 206e 616d 650a 2020  label] = name.  
+00013150: 2020 2020 2020 2020 2020 7265 735b 6c61            res[la
+00013160: 6265 6c2e 7374 7269 7028 292e 6c6f 7765  bel.strip().lowe
+00013170: 7228 295d 203d 206e 616d 650a 0a20 2020  r()] = name..   
+00013180: 2072 6574 7572 6e20 7265 730a 0a0a 6465   return res...de
+00013190: 6620 5f6e 616d 655f 6c61 6265 6c5f 6d61  f _name_label_ma
+000131a0: 7070 6572 5f69 7465 7261 746f 7228 0a20  pper_iterator(. 
+000131b0: 2020 206a 736f 6e5f 7375 6273 6574 3a20     json_subset: 
+000131c0: 6c69 7374 5b64 6963 745b 7374 722c 2041  list[dict[str, A
+000131d0: 6e79 5d5d 2c0a 2020 2020 6c61 6e67 7561  ny]],.    langua
+000131e0: 6765 5f6c 6162 656c 3a20 7374 722c 0a29  ge_label: str,.)
+000131f0: 202d 3e20 4974 6572 6162 6c65 5b74 7570   -> Iterable[tup
+00013200: 6c65 5b73 7472 2c20 7374 725d 5d3a 0a20  le[str, str]]:. 
+00013210: 2020 2022 2222 0a20 2020 2047 6f20 7468     """.    Go th
+00013220: 726f 7567 6820 6c69 7374 206e 6f64 6573  rough list nodes
+00013230: 206f 6620 6120 4a53 4f4e 2070 726f 6a65   of a JSON proje
+00013240: 6374 2061 6e64 2079 6965 6c64 2028 6c61  ct and yield (la
+00013250: 6265 6c2c 206e 616d 6529 2070 6169 7273  bel, name) pairs
+00013260: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00013270: 2020 2020 206a 736f 6e5f 7375 6273 6574       json_subset
+00013280: 3a20 6c69 7374 206f 6620 4453 5020 6c69  : list of DSP li
+00013290: 7374 7320 2861 2044 5350 206c 6973 7420  sts (a DSP list 
+000132a0: 6265 696e 6720 6120 6469 6374 696f 6e61  being a dictiona
+000132b0: 7279 2077 6974 6820 7468 6520 6b65 7973  ry with the keys
+000132c0: 2022 6e61 6d65 222c 2022 6c61 6265 6c73   "name", "labels
+000132d0: 2220 616e 6420 226e 6f64 6573 2229 0a20  " and "nodes"). 
+000132e0: 2020 2020 2020 206c 616e 6775 6167 655f         language_
+000132f0: 6c61 6265 6c3a 2077 6869 6368 206c 616e  label: which lan
+00013300: 6775 6167 6520 6f66 2074 6865 206c 6162  guage of the lab
+00013310: 656c 2074 6f20 6368 6f6f 7365 0a0a 2020  el to choose..  
+00013320: 2020 5969 656c 6473 3a0a 2020 2020 2020    Yields:.      
+00013330: 2020 286c 6162 656c 2c20 6e61 6d65 2920    (label, name) 
+00013340: 7061 6972 730a 2020 2020 2222 220a 2020  pairs.    """.  
+00013350: 2020 666f 7220 6e6f 6465 2069 6e20 6a73    for node in js
+00013360: 6f6e 5f73 7562 7365 743a 0a20 2020 2020  on_subset:.     
+00013370: 2020 2023 206e 6f64 6520 6973 2074 6865     # node is the
+00013380: 206a 736f 6e20 6f62 6a65 6374 2063 6f6e   json object con
+00013390: 7461 696e 696e 6720 7468 6520 656e 7469  taining the enti
+000133a0: 7265 206a 736f 6e2d 6c69 7374 0a20 2020  re json-list.   
+000133b0: 2020 2020 2069 6620 226e 6f64 6573 2220       if "nodes" 
+000133c0: 696e 206e 6f64 653a 0a20 2020 2020 2020  in node:.       
+000133d0: 2020 2020 2023 2022 6e6f 6465 7322 2069       # "nodes" i
+000133e0: 7320 7468 6520 6a73 6f6e 2073 7562 2d6f  s the json sub-o
+000133f0: 626a 6563 7420 636f 6e74 6169 6e69 6e67  bject containing
+00013400: 2074 6865 2065 6e74 7269 6573 206f 6620   the entries of 
+00013410: 7468 6520 6a73 6f6e 2d6c 6973 740a 2020  the json-list.  
+00013420: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
+00013430: 6672 6f6d 205f 6e61 6d65 5f6c 6162 656c  from _name_label
+00013440: 5f6d 6170 7065 725f 6974 6572 6174 6f72  _mapper_iterator
+00013450: 286e 6f64 655b 226e 6f64 6573 225d 2c20  (node["nodes"], 
+00013460: 6c61 6e67 7561 6765 5f6c 6162 656c 290a  language_label).
+00013470: 2020 2020 2020 2020 2020 2020 2320 6561              # ea
+00013480: 6368 2079 6965 6c64 6564 2076 616c 7565  ch yielded value
+00013490: 2069 7320 6120 286c 6162 656c 2c20 6e61   is a (label, na
+000134a0: 6d65 2920 7061 6972 206f 6620 6120 7369  me) pair of a si
+000134b0: 6e67 6c65 206c 6973 7420 656e 7472 790a  ngle list entry.
+000134c0: 2020 2020 2020 2020 6966 2022 6e61 6d65          if "name
+000134d0: 2220 696e 206e 6f64 653a 0a20 2020 2020  " in node:.     
+000134e0: 2020 2020 2020 2079 6965 6c64 2028 6e6f         yield (no
+000134f0: 6465 5b22 6c61 6265 6c73 225d 5b6c 616e  de["labels"][lan
+00013500: 6775 6167 655f 6c61 6265 6c5d 2c20 6e6f  guage_label], no
+00013510: 6465 5b22 6e61 6d65 225d 290a 2020 2020  de["name"]).    
+00013520: 2020 2020 2020 2020 2320 7468 6520 6163          # the ac
+00013530: 7475 616c 2076 616c 7565 7320 6f66 2074  tual values of t
+00013540: 6865 206e 616d 6520 616e 6420 7468 6520  he name and the 
+00013550: 6c61 6265 6c0a 0a0a 6465 6620 7772 6974  label...def writ
+00013560: 655f 786d 6c28 0a20 2020 2072 6f6f 743a  e_xml(.    root:
+00013570: 2065 7472 6565 2e5f 456c 656d 656e 742c   etree._Element,
+00013580: 0a20 2020 2066 696c 6570 6174 683a 2073  .    filepath: s
+00013590: 7472 207c 2050 6174 682c 0a29 202d 3e20  tr | Path,.) -> 
+000135a0: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
+000135b0: 2020 5772 6974 6520 7468 6520 6669 6e69    Write the fini
+000135c0: 7368 6564 2058 4d4c 2074 6f20 6120 6669  shed XML to a fi
+000135d0: 6c65 2e0a 0a20 2020 2041 7267 733a 0a20  le...    Args:. 
+000135e0: 2020 2020 2020 2072 6f6f 743a 2065 7472         root: etr
+000135f0: 6565 2045 6c65 6d65 6e74 2077 6974 6820  ee Element with 
+00013600: 7468 6520 656e 7469 7265 2058 4d4c 2064  the entire XML d
+00013610: 6f63 756d 656e 740a 2020 2020 2020 2020  ocument.        
+00013620: 6669 6c65 7061 7468 3a20 7768 6572 6520  filepath: where 
+00013630: 746f 2073 6176 6520 7468 6520 6669 6c65  to save the file
+00013640: 0a0a 2020 2020 5761 726e 696e 673a 0a20  ..    Warning:. 
+00013650: 2020 2020 2020 2069 6620 7468 6520 584d         if the XM
+00013660: 4c20 6973 206e 6f74 2076 616c 6964 2061  L is not valid a
+00013670: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
+00013680: 7363 6865 6d61 0a20 2020 2022 2222 0a20  schema.    """. 
+00013690: 2020 2065 7472 6565 2e69 6e64 656e 7428     etree.indent(
+000136a0: 726f 6f74 2c20 7370 6163 653d 2220 2020  root, space="   
+000136b0: 2022 290a 2020 2020 786d 6c5f 7374 7269   ").    xml_stri
+000136c0: 6e67 203d 2065 7472 6565 2e74 6f73 7472  ng = etree.tostr
+000136d0: 696e 6728 0a20 2020 2020 2020 2072 6f6f  ing(.        roo
+000136e0: 742c 0a20 2020 2020 2020 2065 6e63 6f64  t,.        encod
+000136f0: 696e 673d 2275 6e69 636f 6465 222c 0a20  ing="unicode",. 
+00013700: 2020 2020 2020 2070 7265 7474 795f 7072         pretty_pr
+00013710: 696e 743d 5472 7565 2c0a 2020 2020 2020  int=True,.      
+00013720: 2020 646f 6374 7970 653d 273c 3f78 6d6c    doctype='<?xml
+00013730: 2076 6572 7369 6f6e 3d22 312e 3022 2065   version="1.0" e
+00013740: 6e63 6f64 696e 673d 2255 5446 2d38 223f  ncoding="UTF-8"?
+00013750: 3e27 2c0a 2020 2020 290a 2020 2020 786d  >',.    ).    xm
+00013760: 6c5f 7374 7269 6e67 203d 2078 6d6c 5f73  l_string = xml_s
+00013770: 7472 696e 672e 7265 706c 6163 6528 7222  tring.replace(r"
+00013780: 5c27 222c 2022 2722 290a 2020 2020 7769  \'", "'").    wi
+00013790: 7468 206f 7065 6e28 6669 6c65 7061 7468  th open(filepath
+000137a0: 2c20 2277 222c 2065 6e63 6f64 696e 673d  , "w", encoding=
+000137b0: 2275 7466 2d38 2229 2061 7320 663a 0a20  "utf-8") as f:. 
+000137c0: 2020 2020 2020 2066 2e77 7269 7465 2878         f.write(x
+000137d0: 6d6c 5f73 7472 696e 6729 0a20 2020 2074  ml_string).    t
+000137e0: 7279 3a0a 2020 2020 2020 2020 7661 6c69  ry:.        vali
+000137f0: 6461 7465 5f78 6d6c 2869 6e70 7574 5f66  date_xml(input_f
+00013800: 696c 653d 6669 6c65 7061 7468 290a 2020  ile=filepath).  
+00013810: 2020 2020 2020 7072 696e 7428 6622 5468        print(f"Th
+00013820: 6520 584d 4c20 6669 6c65 2077 6173 2073  e XML file was s
+00013830: 7563 6365 7373 6675 6c6c 7920 7361 7665  uccessfully save
+00013840: 6420 746f 207b 6669 6c65 7061 7468 7d22  d to {filepath}"
+00013850: 290a 2020 2020 6578 6365 7074 2042 6173  ).    except Bas
+00013860: 6545 7272 6f72 2061 7320 6572 723a 0a20  eError as err:. 
+00013870: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
+00013880: 2020 2020 2020 2020 2020 2066 2254 6865             f"The
+00013890: 2058 4d4c 2066 696c 6520 7761 7320 7375   XML file was su
+000138a0: 6363 6573 7366 756c 6c79 2073 6176 6564  ccessfully saved
+000138b0: 2074 6f20 7b66 696c 6570 6174 687d 2c20   to {filepath}, 
+000138c0: 220a 2020 2020 2020 2020 2020 2020 6622  ".            f"
+000138d0: 6275 7420 7468 6520 666f 6c6c 6f77 696e  but the followin
+000138e0: 6720 5363 6865 6d61 2076 616c 6964 6174  g Schema validat
+000138f0: 696f 6e20 6572 726f 7228 7329 206f 6363  ion error(s) occ
+00013900: 7572 7265 643a 207b 6572 722e 6d65 7373  urred: {err.mess
+00013910: 6167 657d 220a 2020 2020 2020 2020 290a  age}".        ).
+00013920: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
+00013930: 2e77 6172 6e28 4473 7054 6f6f 6c73 5573  .warn(DspToolsUs
+00013940: 6572 5761 726e 696e 6728 6d73 6729 290a  erWarning(msg)).
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/excel2xml/propertyelement.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/id2iri.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/id2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/ingest_xmlupload/user_information.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/user_information.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/create/project_create.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/create/project_create_lists.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/create/project_validate.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_validate.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/get.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/get.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/context.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/context.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/group.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/helpers.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/listnode.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/ontology.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/project.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/propertyclass.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/propertyclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/resourceclass.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/resourceclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/project/models/user.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import pickle
 import sys
-from copy import deepcopy
-from dataclasses import replace
 
 from loguru import logger
 from termcolor import colored
 
-from dsp_tools.commands.xmlupload.iri_resolver import IriResolver
 from dsp_tools.commands.xmlupload.list_client import ListClient
 from dsp_tools.commands.xmlupload.list_client import ListClientLive
 from dsp_tools.commands.xmlupload.models.sipi import Sipi
 from dsp_tools.commands.xmlupload.models.upload_state import UploadState
 from dsp_tools.commands.xmlupload.project_client import ProjectClient
 from dsp_tools.commands.xmlupload.project_client import ProjectClientLive
 from dsp_tools.commands.xmlupload.upload_config import UploadConfig
@@ -32,65 +29,65 @@
 
     Returns:
         True if all resources could be uploaded without errors; False if one of the resources could not be
         uploaded because there is an error in it
     """
     upload_state = _read_upload_state_from_disk(server)
     if skip_first_resource:
-        if len(upload_state.pending_resources) > 0:
-            new_pending = deepcopy(upload_state.pending_resources)
-            new_pending.pop(0)
-            upload_state = replace(upload_state, pending_resources=new_pending)
-        else:
-            msg = (
-                "The list of pending resources is empty.\n"
-                "It is not yet possible to skip the first item of the stashed properties.\n"
-                "Do you want to continue with the upload of the stashed properties anyway? [y/n]"
-            )
-            resp = None
-            while resp not in ["y", "n"]:
-                resp = input(colored(msg, color="red"))
-            if resp == "n":
-                sys.exit(1)
+        _skip_first_resource(upload_state)
 
-    previous_successful = len(upload_state.iri_resolver_lookup)
-    previous_failed = len(upload_state.failed_uploads)
-    previous_total = previous_successful + previous_failed
-    msg = (
-        f"Resuming upload for project {upload_state.config.shortcode} on server {server}. "
-        f"Number of resources uploaded until now: {previous_total}"
-    )
-    if previous_failed:
-        msg += f" ({previous_failed} of them failed)"
-    logger.info(msg)
-    print("\n==========================\n" + msg + "\n==========================\n")
+    _print_and_log(upload_state, server)
 
     con = ConnectionLive(server)
     con.login(user, password)
     sipi_con = ConnectionLive(sipi, token=con.get_token())
     sipi_server = Sipi(sipi_con)
 
     project_client: ProjectClient = ProjectClientLive(con, upload_state.config.shortcode)
     list_client: ListClient = ListClientLive(con, project_client.get_project_iri())
 
-    iri_resolver, failed_uploads, nonapplied_stash = upload_resources(
-        resources=upload_state.pending_resources,
-        failed_uploads=upload_state.failed_uploads,
+    upload_resources(
+        upload_state=upload_state,
         imgdir=".",
         sipi_server=sipi_server,
-        permissions_lookup=upload_state.permissions_lookup,
-        con=con,
-        stash=upload_state.pending_stash,
-        config=upload_state.config,
         project_client=project_client,
         list_client=list_client,
-        iri_resolver=IriResolver(upload_state.iri_resolver_lookup),
     )
 
-    return cleanup_upload(iri_resolver, upload_state.config, failed_uploads, nonapplied_stash)
+    return cleanup_upload(upload_state)
 
 
 def _read_upload_state_from_disk(server: str) -> UploadState:
     save_location = UploadConfig().with_server_info(server, "foo").diagnostics.save_location
     with open(save_location, "rb") as f:
         saved_state: UploadState = pickle.load(f)  # noqa: S301 (deserialization of untrusted data)
     return saved_state
+
+
+def _skip_first_resource(upload_state: UploadState) -> None:
+    if len(upload_state.pending_resources) > 0:
+        upload_state.pending_resources.pop(0)
+    else:
+        msg = (
+            "The list of pending resources is empty.\n"
+            "It is not yet possible to skip the first item of the stashed properties.\n"
+            "Do you want to continue with the upload of the stashed properties anyway? [y/n]"
+        )
+        resp = None
+        while resp not in ["y", "n"]:
+            resp = input(colored(msg, color="red"))
+        if resp == "n":
+            sys.exit(1)
+
+
+def _print_and_log(upload_state: UploadState, server: str) -> None:
+    previous_successful = len(upload_state.iri_resolver.lookup)
+    previous_failed = len(upload_state.failed_uploads)
+    previous_total = previous_successful + previous_failed
+    msg = (
+        f"Resuming upload for project {upload_state.config.shortcode} on server {server}. "
+        f"Number of resources uploaded until now: {previous_total}"
+    )
+    if previous_failed:
+        msg += f" ({previous_failed} of them failed)"
+    logger.info(msg)
+    print("\n==========================\n" + msg + "\n==========================\n")
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/rosetta.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/start_stack.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/start_stack.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/template.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/template.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/ark2iri.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ark2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/iri_resolver.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/iri_resolver.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/list_client.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/list_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/permission.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/sipi.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/sipi.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/upload_state.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/upload_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from dataclasses import dataclass
 
+from dsp_tools.commands.xmlupload.iri_resolver import IriResolver
+from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import XMLResource
 from dsp_tools.commands.xmlupload.models.permission import Permissions
-from dsp_tools.commands.xmlupload.models.xmlresource import XMLResource
 from dsp_tools.commands.xmlupload.stash.stash_models import Stash
 from dsp_tools.commands.xmlupload.upload_config import UploadConfig
 
 
-@dataclass(frozen=True)
+@dataclass
 class UploadState:
     """
     Save the state of an xmlupload, so that after an interruption, it can be resumed.
     """
 
     pending_resources: list[XMLResource]
     failed_uploads: list[str]
-    iri_resolver_lookup: dict[str, str]
+    iri_resolver: IriResolver
     pending_stash: Stash | None
     config: UploadConfig
     permissions_lookup: dict[str, Permissions]
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/xmlallow.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/xmlpermission.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,50 @@
+from __future__ import annotations
+
 from lxml import etree
 
+from dsp_tools.commands.xmlupload.models.permission import Permissions
 from dsp_tools.commands.xmlupload.models.permission import PermissionValue
 from dsp_tools.models.exceptions import XmlUploadError
 from dsp_tools.models.projectContext import ProjectContext
 
 
+class XmlPermission:
+    """Represents the permission set containing several XmlAllow elements in the XML used for data import"""
+
+    permission_id: str
+    _allows: list[XmlAllow]
+
+    def __init__(self, node: etree._Element, project_context: ProjectContext) -> None:
+        """
+        Constructor which parses a XML DOM permissions element representing an named permission set
+
+        Args:
+            node: The DOM node to be processed (representing an a permission set)
+            project_context: Context for DOM node traversal
+        """
+        self._allows = []
+        self.permission_id = node.attrib["id"]
+        for allow_node in node:
+            self._allows.append(XmlAllow(allow_node, project_context))
+
+    def get_permission_instance(self) -> Permissions:
+        """Returns a list of allow elements of this permission instance"""
+        permissions = Permissions()
+        for allow in self._allows:
+            permissions.add(allow.permission, allow.group)
+        return permissions
+
+    def __str__(self) -> str:
+        allow_str: list[str] = []
+        for allow in self._allows:
+            allow_str.append(f"{allow.permission} {allow.group}")
+        return "|".join(allow_str)
+
+
 class XmlAllow:
     """Represents the allow element of the XML used for data import"""
 
     _group: str
     _permission: PermissionValue
 
     def __init__(self, node: etree._Element, project_context: ProjectContext) -> None:
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/models/xmlresource.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/xmlresource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from typing import Optional
 
 from lxml import etree
 
+from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLBitstream
+from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLProperty
 from dsp_tools.commands.xmlupload.models.permission import Permissions
-from dsp_tools.commands.xmlupload.models.xmlbitstream import XMLBitstream
-from dsp_tools.commands.xmlupload.models.xmlproperty import XMLProperty
 from dsp_tools.models.datetimestamp import DateTimeStamp
 
 
 @dataclass(frozen=True)
 class BitstreamInfo:
     """
     Represents a bitstream object,
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/ontology_client.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ontology_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/project_client.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/project_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,18 @@
     project_iri: str
     ontology_iris: list[str]
 
 
 class ProjectClient(Protocol):
     """Interface (protocol) for project-related requests to the DSP-API."""
 
+    con: Connection
+    shortcode: str
+    project_info: ProjectInfo | None
+
     def get_project_iri(self) -> str:
         """Get the IRI of the project to which the data is being uploaded."""
 
     def get_ontology_name_dict(self) -> dict[str, str]:
         """Returns a mapping of ontology names to ontology IRIs."""
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/resource_create_client.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_create_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 import json
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any
 from typing import assert_never
+from typing import cast
 
 from loguru import logger
 
 from dsp_tools.commands.xmlupload.ark2iri import convert_ark_v0_to_resource_iri
 from dsp_tools.commands.xmlupload.iri_resolver import IriResolver
+from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLProperty
+from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLValue
+from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import BitstreamInfo
+from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import XMLResource
 from dsp_tools.commands.xmlupload.models.formatted_text_value import FormattedTextValue
+from dsp_tools.commands.xmlupload.models.namespace_context import get_json_ld_context_for_project
 from dsp_tools.commands.xmlupload.models.permission import Permissions
-from dsp_tools.commands.xmlupload.models.xmlproperty import XMLProperty
-from dsp_tools.commands.xmlupload.models.xmlresource import BitstreamInfo
-from dsp_tools.commands.xmlupload.models.xmlresource import XMLResource
-from dsp_tools.commands.xmlupload.models.xmlvalue import XMLValue
+from dsp_tools.commands.xmlupload.models.serialise.serialise_value import SerialiseProperty
+from dsp_tools.commands.xmlupload.models.serialise.serialise_value import SerialiseURI
+from dsp_tools.commands.xmlupload.models.serialise.serialise_value import SerialiseValue
 from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.exceptions import PermissionNotExistsError
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.connection import Connection
 from dsp_tools.utils.date_util import parse_date_string
 from dsp_tools.utils.iri_util import is_resource_iri
 
 
 @dataclass(frozen=True)
 class ResourceCreateClient:
     """client class that creates resources on a DSP server."""
 
     con: Connection
     project_iri: str
     iri_resolver: IriResolver
-    json_ld_context: dict[str, str]
+    project_onto_dict: dict[str, str]
     permissions_lookup: dict[str, Permissions]
     listnode_lookup: dict[str, str]
     media_previously_ingested: bool = False
 
     def create_resource(
         self,
         resource: XMLResource,
         bitstream_information: BitstreamInfo | None,
-    ) -> tuple[str, str]:
-        """Creates a resource on the DSP server."""
+    ) -> str:
+        """Creates a resource on the DSP server, and returns its IRI"""
         logger.info(
             f"Attempting to create resource {resource.res_id} (label: {resource.label}, iri: {resource.iri})..."
         )
         resource_dict = self._make_resource_with_values(resource, bitstream_information)
         headers = {"X-Asset-Ingested": "true"} if self.media_previously_ingested else None
         res = self.con.post(route="/v2/resources", data=resource_dict, headers=headers)
-        iri = res["@id"]
-        label = res["rdfs:label"]
-        return iri, label
+        return cast(str, res["@id"])
 
     def _make_resource_with_values(
         self,
         resource: XMLResource,
         bitstream_information: BitstreamInfo | None,
     ) -> dict[str, Any]:
         res = self._make_resource(
@@ -66,27 +70,28 @@
         self,
         resource: XMLResource,
         bitstream_information: BitstreamInfo | None,
     ) -> dict[str, Any]:
         resource_iri = resource.iri
         if resource.ark:
             resource_iri = convert_ark_v0_to_resource_iri(resource.ark)
+        context = get_json_ld_context_for_project(self.project_onto_dict)
         res = {
             "@type": resource.restype,
             "rdfs:label": resource.label,
             "knora-api:attachedToProject": {"@id": self.project_iri},
-            "@context": self.json_ld_context,
+            "@context": context,
         }
         if resource_iri:
             res["@id"] = resource_iri
         if resource.permissions:
             if perm := self.permissions_lookup.get(resource.permissions):
                 res["knora-api:hasPermissions"] = str(perm)
             else:
-                raise BaseError(
+                raise PermissionNotExistsError(
                     f"Could not find permissions for resource {resource.res_id} with permissions {resource.permissions}"
                 )
         if resource.creation_date:
             res["knora-api:creationDate"] = {
                 "@type": "xsd:dateTimeStamp",
                 "@value": str(resource.creation_date),
             }
@@ -104,15 +109,24 @@
                 return "knora-api:isAudioSegmentOfValue"
             else:
                 return f"{p.name}Value"
 
         def make_values(p: XMLProperty) -> list[dict[str, Any]]:
             return [self._make_value(v, p.valtype) for v in p.values]
 
-        return {prop_name(prop): make_values(prop) for prop in resource.properties}
+        properties_serialised = {}
+
+        for prop in resource.properties:
+            match prop.valtype:
+                case "uri":
+                    properties_serialised.update(_serialise_uri_prop(prop, self.permissions_lookup))
+                case _:
+                    properties_serialised.update({prop_name(prop): make_values(prop)})
+
+        return properties_serialised
 
     def _make_value(self, value: XMLValue, value_type: str) -> dict[str, Any]:
         match value_type:
             case "boolean":
                 res = _make_boolean_value(value)
             case "color":
                 res = _make_color_value(value)
@@ -132,25 +146,23 @@
                 res = _make_link_value(value, self.iri_resolver)
             case "list":
                 res = _make_list_value(value, self.listnode_lookup)
             case "text":
                 res = _make_text_value(value, self.iri_resolver)
             case "time":
                 res = _make_time_value(value)
-            case "uri":
-                res = _make_uri_value(value)
             case _:
                 raise UserError(f"Unknown value type: {value_type}")
         if value.comment:
             res["knora-api:valueHasComment"] = value.comment
         if value.permissions:
             if perm := self.permissions_lookup.get(value.permissions):
                 res["knora-api:hasPermissions"] = str(perm)
             else:
-                raise BaseError(f"Could not find permissions for value: {value.permissions}")
+                raise PermissionNotExistsError(f"Could not find permissions for value: {value.permissions}")
         return res
 
 
 def _make_bitstream_file_value(bitstream_info: BitstreamInfo) -> dict[str, Any]:
     local_file = Path(bitstream_info.local_file)
     file_ending = local_file.suffix[1:]
     match file_ending.lower():
@@ -346,22 +358,36 @@
         "knora-api:timeValueAsTimeStamp": {
             "@type": "xsd:dateTimeStamp",
             "@value": value.value,
         },
     }
 
 
-def _make_uri_value(value: XMLValue) -> dict[str, Any]:
-    return {
-        "@type": "knora-api:UriValue",
-        "knora-api:uriValueAsUri": {
-            "@type": "xsd:anyURI",
-            "@value": value.value,
-        },
-    }
+def _serialise_uri_prop(prop: XMLProperty, permissions_lookup: dict[str, Permissions]) -> dict[str, Any]:
+    uri_values: list[SerialiseValue] = []
+    for v in prop.values:
+        if v.permissions:
+            if not (per := permissions_lookup.get(v.permissions)):
+                raise PermissionNotExistsError(f"Could not find permissions for value: {v.permissions}")
+            permission = str(per)
+        else:
+            permission = None
+        uri = cast(str, v.value)
+        uri_values.append(
+            SerialiseURI(
+                value=uri,
+                permissions=permission,
+                comment=v.comment,
+            )
+        )
+    prop_serialise = SerialiseProperty(
+        property_name=prop.name,
+        values=uri_values,
+    )
+    return prop_serialise.serialise()
 
 
 def _assert_is_string(value: str | FormattedTextValue) -> str:
     match value:
         case str() as s:
             return s
         case FormattedTextValue() as xml:
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/resource_multimedia.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_multimedia.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from datetime import datetime
 from pathlib import Path
 
 from loguru import logger
 
+from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLBitstream
+from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import BitstreamInfo
+from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import XMLResource
 from dsp_tools.commands.xmlupload.models.permission import Permissions
 from dsp_tools.commands.xmlupload.models.sipi import Sipi
-from dsp_tools.commands.xmlupload.models.xmlbitstream import XMLBitstream
-from dsp_tools.commands.xmlupload.models.xmlresource import BitstreamInfo
-from dsp_tools.commands.xmlupload.models.xmlresource import XMLResource
 from dsp_tools.models.exceptions import PermanentConnectionError
 
 
 def handle_media_info(
     resource: XMLResource,
     media_previously_uploaded: bool,
     sipi_server: Sipi,
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/graph_models.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/graph_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from typing import cast
 from uuid import uuid4
 
 from lxml import etree
 
+from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLProperty
+from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import XMLResource
 from dsp_tools.commands.xmlupload.models.formatted_text_value import FormattedTextValue
 from dsp_tools.commands.xmlupload.models.permission import Permissions
-from dsp_tools.commands.xmlupload.models.xmlproperty import XMLProperty
-from dsp_tools.commands.xmlupload.models.xmlresource import XMLResource
 from dsp_tools.commands.xmlupload.stash.construct_and_analyze_graph import create_info_from_xml_for_graph
 from dsp_tools.commands.xmlupload.stash.construct_and_analyze_graph import generate_upload_order
 from dsp_tools.commands.xmlupload.stash.construct_and_analyze_graph import make_graph
 from dsp_tools.commands.xmlupload.stash.stash_models import LinkValueStash
 from dsp_tools.commands.xmlupload.stash.stash_models import LinkValueStashItem
 from dsp_tools.commands.xmlupload.stash.stash_models import StandoffStash
 from dsp_tools.commands.xmlupload.stash.stash_models import StandoffStashItem
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/stash_models.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,7 +102,13 @@
 
         Returns:
             Stash: A Stash object, or None if both inputs are None.
         """
         if standoff_stash or link_value_stash:
             return Stash(standoff_stash, link_value_stash)
         return None
+
+    def is_empty(self) -> bool:
+        """Check if there are any stashed items in this stash"""
+        standoff = not self.standoff_stash or not self.standoff_stash.res_2_stash_items
+        link = not self.link_value_stash or not self.link_value_stash.res_2_stash_items
+        return standoff and link
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any
+from typing import cast
 
 from loguru import logger
 
-from dsp_tools.commands.xmlupload.iri_resolver import IriResolver
+from dsp_tools.commands.xmlupload.models.upload_state import UploadState
 from dsp_tools.commands.xmlupload.stash.stash_models import LinkValueStash
 from dsp_tools.commands.xmlupload.stash.stash_models import LinkValueStashItem
+from dsp_tools.commands.xmlupload.stash.stash_models import Stash
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.utils.connection import Connection
 
 
 def upload_stashed_resptr_props(
-    iri_resolver: IriResolver,
+    upload_state: UploadState,
     con: Connection,
-    stashed_resptr_props: LinkValueStash,
     context: dict[str, str],
-) -> LinkValueStash | None:
+) -> None:
     """
     After all resources are uploaded, the stashed resptr props must be applied to their resources in DSP.
+    The upload state is updated accordingly, as a side effect.
 
     Args:
-        iri_resolver: resolver with a mapping of ids from the XML file to IRIs in DSP
+        upload_state: the current state of the upload
         con: connection to DSP
-        stashed_resptr_props: all resptr props that have been stashed
         context: the JSON-LD context of the resource
-
-    Returns:
-        nonapplied_resptr_props: the resptr props that could not be uploaded
     """
 
     print(f"{datetime.now()}: Upload the stashed resptrs...")
     logger.info("Upload the stashed resptrs...")
-    not_uploaded: list[LinkValueStashItem] = []
-    for res_id, stash_items in stashed_resptr_props.res_2_stash_items.copy().items():
-        res_iri = iri_resolver.get(res_id)
+    upload_state.pending_stash = cast(Stash, upload_state.pending_stash)
+    link_value_stash = cast(LinkValueStash, upload_state.pending_stash.link_value_stash)
+    for res_id, stash_items in link_value_stash.res_2_stash_items.copy().items():
+        res_iri = upload_state.iri_resolver.get(res_id)
         if not res_iri:
             # resource could not be uploaded to DSP, so the stash cannot be uploaded either
             # no action necessary: this resource will remain in nonapplied_resptr_props,
             # which will be handled by the caller
             continue
         print(f"{datetime.now()}:   Upload resptrs of resource '{res_id}'...")
         logger.info(f"  Upload resptrs of resource '{res_id}'...")
         for stash_item in stash_items:
-            target_iri = iri_resolver.get(stash_item.target_id)
+            target_iri = upload_state.iri_resolver.get(stash_item.target_id)
             if not target_iri:
                 continue
             if _upload_stash_item(stash_item, res_iri, target_iri, con, context):
-                stashed_resptr_props.res_2_stash_items[res_id].remove(stash_item)
-            else:
-                not_uploaded.append(stash_item)
-        if not stashed_resptr_props.res_2_stash_items[res_id]:
-            del stashed_resptr_props.res_2_stash_items[res_id]
-    return LinkValueStash.make(not_uploaded)
+                link_value_stash.res_2_stash_items[res_id].remove(stash_item)
+        if not link_value_stash.res_2_stash_items[res_id]:
+            del link_value_stash.res_2_stash_items[res_id]
 
 
 def _upload_stash_item(
     stash: LinkValueStashItem,
     res_iri: str,
     target_iri: str,
     con: Connection,
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any
+from typing import cast
 from urllib.parse import quote_plus
 
 from loguru import logger
 
 from dsp_tools.commands.xmlupload.iri_resolver import IriResolver
 from dsp_tools.commands.xmlupload.models.formatted_text_value import FormattedTextValue
+from dsp_tools.commands.xmlupload.models.upload_state import UploadState
 from dsp_tools.commands.xmlupload.stash.stash_models import StandoffStash
 from dsp_tools.commands.xmlupload.stash.stash_models import StandoffStashItem
+from dsp_tools.commands.xmlupload.stash.stash_models import Stash
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.utils.connection import Connection
 
 
 def _log_unable_to_retrieve_resource(
     resource: str,
     received_error: BaseError,
@@ -89,36 +92,30 @@
             "knora-api:textValueHasMapping": {"@id": "http://rdfh.ch/standoff/mappings/StandardMapping"},
         },
         "@context": context,
     }
     return jsonobj
 
 
-def upload_stashed_xml_texts(
-    iri_resolver: IriResolver,
-    con: Connection,
-    stashed_xml_texts: StandoffStash,
-) -> StandoffStash | None:
+def upload_stashed_xml_texts(upload_state: UploadState, con: Connection) -> None:
     """
     After all resources are uploaded, the stashed xml texts must be applied to their resources in DSP.
+    The upload state is updated accordingly, as a side effect.
 
     Args:
-        iri_resolver: resolver to map ids from the XML file to IRIs in DSP
+        upload_state: the current state of the upload
         con: connection to DSP
-        stashed_xml_texts: all xml texts that have been stashed
-
-    Returns:
-        the xml texts that could not be uploaded
     """
 
     print(f"{datetime.now()}: Upload the stashed XML texts...")
     logger.info("Upload the stashed XML texts...")
-    not_uploaded: list[StandoffStashItem] = []
-    for res_id, stash_items in stashed_xml_texts.res_2_stash_items.copy().items():
-        res_iri = iri_resolver.get(res_id)
+    upload_state.pending_stash = cast(Stash, upload_state.pending_stash)
+    standoff_stash = cast(StandoffStash, upload_state.pending_stash.standoff_stash)
+    for res_id, stash_items in standoff_stash.res_2_stash_items.copy().items():
+        res_iri = upload_state.iri_resolver.get(res_id)
         if not res_iri:
             # resource could not be uploaded to DSP, so the stash cannot be uploaded either
             # no action necessary: this resource will remain in the list of not uploaded stash items,
             # which will be handled by the caller
             continue
         try:
             resource_in_triplestore = con.get(f"/v2/resources/{quote_plus(res_iri)}")
@@ -127,33 +124,28 @@
             continue
         print(f"{datetime.now()}:   Upload XML text(s) of resource '{res_id}'...")
         logger.info(f"  Upload XML text(s) of resource '{res_id}'...")
         context = resource_in_triplestore["@context"]
         for stash_item in stash_items:
             value_iri = _get_value_iri(stash_item.prop_name, resource_in_triplestore, stash_item.uuid)
             if not value_iri:
-                not_uploaded.append(stash_item)
                 continue
-            success = _upload_stash_item(
+            if _upload_stash_item(
                 stash_item=stash_item,
                 res_iri=res_iri,
                 res_type=stash_item.res_type,
                 res_id=res_id,
                 value_iri=value_iri,
-                iri_resolver=iri_resolver,
+                iri_resolver=upload_state.iri_resolver,
                 con=con,
                 context=context,
-            )
-            if success:
-                stashed_xml_texts.res_2_stash_items[res_id].remove(stash_item)
-            else:
-                not_uploaded.append(stash_item)
-        if not stashed_xml_texts.res_2_stash_items[res_id]:
-            stashed_xml_texts.res_2_stash_items.pop(res_id)
-    return StandoffStash.make(not_uploaded)
+            ):
+                standoff_stash.res_2_stash_items[res_id].remove(stash_item)
+        if not standoff_stash.res_2_stash_items[res_id]:
+            standoff_stash.res_2_stash_items.pop(res_id)
 
 
 def _get_value_iri(
     property_name: str,
     resource: dict[str, Any],
     uuid: str,
 ) -> str | None:
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/upload_config.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/upload_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/commands/xmlupload/xmlupload.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/xmlupload.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 from __future__ import annotations
 
 import pickle
 import sys
+import warnings
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 
 from loguru import logger
 from lxml import etree
 
 from dsp_tools.commands.xmlupload.check_consistency_with_ontology import do_xml_consistency_check_with_ontology
 from dsp_tools.commands.xmlupload.iri_resolver import IriResolver
 from dsp_tools.commands.xmlupload.list_client import ListClient
 from dsp_tools.commands.xmlupload.list_client import ListClientLive
+from dsp_tools.commands.xmlupload.models.deserialise.xmlpermission import XmlPermission
+from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import BitstreamInfo
+from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import XMLResource
+from dsp_tools.commands.xmlupload.models.namespace_context import get_json_ld_context_for_project
 from dsp_tools.commands.xmlupload.models.permission import Permissions
 from dsp_tools.commands.xmlupload.models.sipi import Sipi
 from dsp_tools.commands.xmlupload.models.upload_state import UploadState
-from dsp_tools.commands.xmlupload.models.xmlpermission import XmlPermission
-from dsp_tools.commands.xmlupload.models.xmlresource import BitstreamInfo
-from dsp_tools.commands.xmlupload.models.xmlresource import XMLResource
 from dsp_tools.commands.xmlupload.ontology_client import OntologyClientLive
 from dsp_tools.commands.xmlupload.project_client import ProjectClient
 from dsp_tools.commands.xmlupload.project_client import ProjectClientLive
 from dsp_tools.commands.xmlupload.read_validate_xml_file import validate_and_parse_xml_file
 from dsp_tools.commands.xmlupload.resource_create_client import ResourceCreateClient
 from dsp_tools.commands.xmlupload.resource_multimedia import handle_media_info
 from dsp_tools.commands.xmlupload.stash.stash_circular_references import identify_circular_references
 from dsp_tools.commands.xmlupload.stash.stash_circular_references import stash_circular_references
 from dsp_tools.commands.xmlupload.stash.stash_models import Stash
 from dsp_tools.commands.xmlupload.stash.upload_stashed_resptr_props import upload_stashed_resptr_props
 from dsp_tools.commands.xmlupload.stash.upload_stashed_xml_texts import upload_stashed_xml_texts
 from dsp_tools.commands.xmlupload.upload_config import UploadConfig
 from dsp_tools.commands.xmlupload.write_diagnostic_info import write_id2iri_mapping
+from dsp_tools.models.custom_warnings import DspToolsUserWarning
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.exceptions import PermanentTimeOutError
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.models.exceptions import XmlUploadInterruptedError
 from dsp_tools.models.projectContext import ProjectContext
 from dsp_tools.utils.connection import Connection
 from dsp_tools.utils.connection_live import ConnectionLive
-from dsp_tools.utils.json_ld_util import get_json_ld_context_for_project
 from dsp_tools.utils.logger_config import logger_savepath
 
 
 def xmlupload(
     input_file: str | Path | etree._ElementTree[Any],
     server: str,
     user: str,
@@ -101,68 +103,59 @@
         root=root,
         con=con,
         default_ontology=default_ontology,
     )
 
     project_client: ProjectClient = ProjectClientLive(con, config.shortcode)
     list_client: ListClient = ListClientLive(con, project_client.get_project_iri())
-    iri_resolver = IriResolver()
+    upload_state = UploadState(resources, [], IriResolver(), stash, config, permissions_lookup)
 
-    iri_resolver, failed_uploads, nonapplied_stash = upload_resources(
-        resources=resources,
-        failed_uploads=[],
+    upload_resources(
+        upload_state=upload_state,
         imgdir=imgdir,
         sipi_server=sipi_server,
-        permissions_lookup=permissions_lookup,
-        con=con,
-        stash=stash,
-        config=config,
         project_client=project_client,
         list_client=list_client,
-        iri_resolver=iri_resolver,
     )
 
-    return cleanup_upload(iri_resolver, config, failed_uploads, nonapplied_stash)
+    return cleanup_upload(upload_state)
 
 
-def cleanup_upload(
-    iri_resolver: IriResolver,
-    config: UploadConfig,
-    failed_uploads: list[str],
-    nonapplied_stash: Stash | None,
-) -> bool:
+def cleanup_upload(upload_state: UploadState) -> bool:
     """
     Write the id2iri mapping to a file and print a message to the console.
 
     Args:
-        iri_resolver: mapping from internal IDs to IRIs
-        config: the upload configuration
-        failed_uploads: resources that caused an error when uploading to DSP
-        nonapplied_stash: the stash items that could not be reapplied
+        upload_state: the current state of the upload
 
     Returns:
-        success status (deduced from failed_uploads)
+        success status (deduced from failed_uploads and non-applied stash)
     """
-    write_id2iri_mapping(iri_resolver.lookup, config.diagnostics)
-    if not failed_uploads and not nonapplied_stash:
+    write_id2iri_mapping(upload_state.iri_resolver.lookup, upload_state.config.diagnostics)
+    has_stash_failed = upload_state.pending_stash and not upload_state.pending_stash.is_empty()
+    if not upload_state.failed_uploads and not has_stash_failed:
         success = True
         print(f"{datetime.now()}: All resources have successfully been uploaded.")
         logger.info("All resources have successfully been uploaded.")
     else:
         success = False
-        if failed_uploads:
-            print(f"\n{datetime.now()}: WARNING: Could not upload the following resources: {failed_uploads}\n")
+        if upload_state.failed_uploads:
+            res_msg = f"Could not upload the following resources: {upload_state.failed_uploads}"
+            print(f"\n{datetime.now()}: WARNING: {res_msg}\n")
             print(f"For more information, see the log file: {logger_savepath}\n")
-            logger.warning(f"Could not upload the following resources: {failed_uploads}")
-        if nonapplied_stash:
-            print(f"\n{datetime.now()}: WARNING: Could not reapply the following stash items: {nonapplied_stash}\n")
+            logger.warning(res_msg)
+        if has_stash_failed:
+            stash_msg = f"Could not reapply the following stash items: {upload_state.pending_stash}"
+            print(f"\n{datetime.now()}: WARNING: {stash_msg}\n")
             print(f"For more information, see the log file: {logger_savepath}\n")
-            logger.warning(f"Could not reapply the following stash items: {nonapplied_stash}")
+            logger.warning(stash_msg)
+        msg = _save_upload_state(upload_state)
+        print(msg)
 
-    config.diagnostics.save_location.unlink(missing_ok=True)
+    upload_state.config.diagnostics.save_location.unlink(missing_ok=True)
     return success
 
 
 def _prepare_upload(
     root: etree._Element,
     con: Connection,
     default_ontology: str,
@@ -181,98 +174,42 @@
     logger.info("Stashing circular references...")
     print(f"{datetime.now()}: Stashing circular references...")
     stash = stash_circular_references(resources, stash_lookup, permissions_lookup)
     return resources, permissions_lookup, stash
 
 
 def upload_resources(
-    resources: list[XMLResource],
-    failed_uploads: list[str],
+    upload_state: UploadState,
     imgdir: str,
     sipi_server: Sipi,
-    permissions_lookup: dict[str, Permissions],
-    con: Connection,
-    stash: Stash | None,
-    config: UploadConfig,
     project_client: ProjectClient,
     list_client: ListClient,
-    iri_resolver: IriResolver,
-) -> tuple[IriResolver, list[str], Stash | None]:
+) -> None:
     """
     Actual upload of all resources to DSP.
 
     Args:
-        resources: list of XMLResources to upload to DSP
-        failed_uploads: resources that caused an error in a previous upload
+        upload_state: the current state of the upload
         imgdir: folder containing the multimedia files
         sipi_server: Sipi instance
-        permissions_lookup: dictionary that contains the permission name as string and the corresponding Python object
-        con: connection to the DSP server
-        stash: an object that contains all stashed links that could not be reapplied to their resources
-        config: the upload configuration
         project_client: a client for HTTP communication with the DSP-API
         list_client: a client for HTTP communication with the DSP-API
-        iri_resolver: mapping from internal IDs to IRIs
-
-    Returns:
-        the id2iri mapping of the uploaded resources,
-        a list of resources that could not be uploaded,
-        and the stash items that could not be reapplied.
     """
     try:
-        iri_resolver, failed_uploads = _upload_resources(
-            resources=resources,
-            failed_uploads=failed_uploads,
+        _upload_resources(
+            upload_state=upload_state,
             imgdir=imgdir,
             sipi_server=sipi_server,
-            permissions_lookup=permissions_lookup,
-            con=con,
-            config=config,
             project_client=project_client,
             list_client=list_client,
-            iri_resolver=iri_resolver,
-        )
-    except BaseException as err:  # noqa: BLE001 (blind-except)
-        # The forseeable errors are already handled by failed_uploads
-        # Here we catch the unforseeable exceptions, incl. keyboard interrupt.
-        _handle_upload_error(
-            err=err,
-            iri_resolver=iri_resolver,
-            pending_resources=resources,
-            failed_uploads=failed_uploads,
-            pending_stash=stash,
-            config=config,
-            permissions_lookup=permissions_lookup,
-        )
-
-    nonapplied_stash = None
-    try:
-        nonapplied_stash = (
-            _upload_stash(
-                stash=stash,
-                iri_resolver=iri_resolver,
-                con=con,
-                project_client=project_client,
-            )
-            if stash
-            else None
         )
-    except BaseException as err:  # noqa: BLE001 (blind-except)
-        # The forseeable errors are already handled by failed_uploads and nonapplied_stash.
-        # Here we catch the unforseeable exceptions, incl. keyboard interrupt.
-        _handle_upload_error(
-            err=err,
-            iri_resolver=iri_resolver,
-            pending_resources=resources,
-            failed_uploads=failed_uploads,
-            pending_stash=stash,
-            config=config,
-            permissions_lookup=permissions_lookup,
-        )
-    return iri_resolver, failed_uploads, nonapplied_stash
+        if upload_state.pending_stash:
+            _upload_stash(upload_state, project_client)
+    except XmlUploadInterruptedError as err:
+        _handle_upload_error(err, upload_state)
 
 
 def _get_data_from_xml(
     con: Connection,
     root: etree._Element,
     default_ontology: str,
 ) -> tuple[list[XMLResource], dict[str, Permissions]]:
@@ -280,38 +217,22 @@
     permissions = _extract_permissions_from_xml(root, proj_context)
     resources = _extract_resources_from_xml(root, default_ontology)
     permissions_lookup = {name: perm.get_permission_instance() for name, perm in permissions.items()}
     return resources, permissions_lookup
 
 
 def _upload_stash(
-    stash: Stash,
-    iri_resolver: IriResolver,
-    con: Connection,
+    upload_state: UploadState,
     project_client: ProjectClient,
-) -> Stash | None:
-    if stash.standoff_stash:
-        nonapplied_standoff = upload_stashed_xml_texts(
-            iri_resolver=iri_resolver,
-            con=con,
-            stashed_xml_texts=stash.standoff_stash,
-        )
-    else:
-        nonapplied_standoff = None
+) -> None:
+    if upload_state.pending_stash and upload_state.pending_stash.standoff_stash:
+        upload_stashed_xml_texts(upload_state, project_client.con)
     context = get_json_ld_context_for_project(project_client.get_ontology_name_dict())
-    if stash.link_value_stash:
-        nonapplied_resptr_props = upload_stashed_resptr_props(
-            iri_resolver=iri_resolver,
-            con=con,
-            stashed_resptr_props=stash.link_value_stash,
-            context=context,
-        )
-    else:
-        nonapplied_resptr_props = None
-    return Stash.make(nonapplied_standoff, nonapplied_resptr_props)
+    if upload_state.pending_stash and upload_state.pending_stash.link_value_stash:
+        upload_stashed_resptr_props(upload_state, project_client.con, context)
 
 
 def _get_project_context_from_server(connection: Connection) -> ProjectContext:
     """
     This function retrieves the project context previously uploaded on the server (json file)
 
     Args:
@@ -339,137 +260,145 @@
 
 def _extract_resources_from_xml(root: etree._Element, default_ontology: str) -> list[XMLResource]:
     resources = list(root.iter(tag="resource"))
     return [XMLResource(res, default_ontology) for res in resources]
 
 
 def _upload_resources(
-    resources: list[XMLResource],
-    failed_uploads: list[str],
+    upload_state: UploadState,
     imgdir: str,
     sipi_server: Sipi,
-    permissions_lookup: dict[str, Permissions],
-    con: Connection,
-    config: UploadConfig,
     project_client: ProjectClient,
     list_client: ListClient,
-    iri_resolver: IriResolver,
-) -> tuple[IriResolver, list[str]]:
+) -> None:
     """
     Iterates through all resources and tries to upload them to DSP.
     If a temporary exception occurs, the action is repeated until success,
     and if a permanent exception occurs, the resource is skipped.
 
     Args:
-        resources: list of XMLResources to upload to DSP
-        failed_uploads: resources that caused an error in a previous upload
+        upload_state: the current state of the upload
         imgdir: folder containing the multimedia files
         sipi_server: Sipi instance
-        permissions_lookup: maps permission strings to Permission objects
-        con: connection to DSP
-        config: the upload configuration
         project_client: a client for HTTP communication with the DSP-API
         list_client: a client for HTTP communication with the DSP-API
-        iri_resolver: mapping from internal IDs to IRIs
 
     Raises:
         BaseException: in case of an unhandled exception during resource creation
         XmlUploadInterruptedError: if the number of resources created is equal to the interrupt_after value
-
-    Returns:
-        id2iri_mapping, failed_uploads
     """
     project_iri = project_client.get_project_iri()
-    json_ld_context = get_json_ld_context_for_project(project_client.get_ontology_name_dict())
+    project_onto_dict = project_client.get_ontology_name_dict()
     listnode_lookup = list_client.get_list_node_id_to_iri_lookup()
 
     resource_create_client = ResourceCreateClient(
-        con=con,
+        con=project_client.con,
         project_iri=project_iri,
-        iri_resolver=iri_resolver,
-        json_ld_context=json_ld_context,
-        permissions_lookup=permissions_lookup,
+        iri_resolver=upload_state.iri_resolver,
+        project_onto_dict=project_onto_dict,
+        permissions_lookup=upload_state.permissions_lookup,
         listnode_lookup=listnode_lookup,
-        media_previously_ingested=config.media_previously_uploaded,
+        media_previously_ingested=upload_state.config.media_previously_uploaded,
     )
 
-    total_res = len(resources) + len(iri_resolver.lookup)
-    previous_successful = len(iri_resolver.lookup)
-    previous_failed = len(failed_uploads)
-    previous_total = previous_successful + previous_failed
-    # if the interrupt_after value is not set, the upload will not be interrupted
-    interrupt_after = config.interrupt_after or total_res + 1
+    for creation_attempts_of_this_round, resource in enumerate(upload_state.pending_resources.copy()):
+        _upload_one_resource(
+            upload_state=upload_state,
+            resource=resource,
+            imgdir=imgdir,
+            sipi_server=sipi_server,
+            resource_create_client=resource_create_client,
+            creation_attempts_of_this_round=creation_attempts_of_this_round,
+        )
 
-    for i, resource in enumerate(resources.copy()):
-        current_res = i + 1 + previous_total
-        if i >= interrupt_after:
-            raise XmlUploadInterruptedError(f"Interrupted: Maximum number of resources was reached ({interrupt_after})")
+
+def _upload_one_resource(
+    upload_state: UploadState,
+    resource: XMLResource,
+    imgdir: str,
+    sipi_server: Sipi,
+    resource_create_client: ResourceCreateClient,
+    creation_attempts_of_this_round: int,
+) -> None:
+    try:
         success, media_info = handle_media_info(
-            resource, config.media_previously_uploaded, sipi_server, imgdir, permissions_lookup
+            resource,
+            upload_state.config.media_previously_uploaded,
+            sipi_server,
+            imgdir,
+            upload_state.permissions_lookup,
         )
         if not success:
-            failed_uploads.append(resource.res_id)
-            continue
+            upload_state.failed_uploads.append(resource.res_id)
+            return
+    except KeyboardInterrupt:
+        raise XmlUploadInterruptedError("KeyboardInterrupt during media file upload") from None
+
+    try:
+        iri = _create_resource(resource, media_info, resource_create_client)
+    except (PermanentTimeOutError, KeyboardInterrupt) as err:
+        warnings.warn(DspToolsUserWarning(f"{type(err).__name__}: Tidying up, then exit..."))
+        msg = (
+            f"There was a {type(err).__name__} while trying to create resource '{resource.res_id}'.\n"
+            f"It is unclear if the resource '{resource.res_id}' was created successfully or not.\n"
+            f"Please check manually in the DSP-APP or DB.\n"
+            f"In case of successful creation, call 'resume-xmlupload' with the flag "
+            f"'--skip-first-resource' to prevent duplication.\n"
+            f"If not, a normal 'resume-xmlupload' can be started."
+        )
+        logger.error(msg)
+        raise XmlUploadInterruptedError(msg) from None
+
+    try:
+        _tidy_up_resource_creation_idempotent(upload_state, iri, resource)
+        _interrupt_if_indicated(upload_state, creation_attempts_of_this_round)
+    except KeyboardInterrupt:
+        warnings.warn(DspToolsUserWarning("KeyboardInterrupt: Tidying up, then exit..."))
+        _tidy_up_resource_creation_idempotent(upload_state, iri, resource)
+        raise XmlUploadInterruptedError("KeyboardInterrupt during tidy up") from None
+
+
+def _interrupt_if_indicated(upload_state: UploadState, creation_attempts_of_this_round: int) -> None:
+    # if the interrupt_after value is not set, the upload will not be interrupted
+    interrupt_after = upload_state.config.interrupt_after or 999_999_999
+    if creation_attempts_of_this_round + 1 >= interrupt_after:
+        msg = f"Interrupted: Maximum number of resources was reached ({upload_state.config.interrupt_after})"
+        raise XmlUploadInterruptedError(msg)
 
-        res = None
-        try:
-            res = _create_resource(resource, media_info, resource_create_client)
-            if res == (None, None):
-                # resource creation failed gracefully: register it as failed, then continue
-                failed_uploads.append(resource.res_id)
-                continue
-            else:
-                # resource creation succeeded: update the iri_resolver and remove the resource from the list
-                iri, label = res
-                _tidy_up_resource_creation(iri, label, iri_resolver, resource, current_res, total_res)  # type: ignore[arg-type]
-        except PermanentTimeOutError:
-            msg = (
-                f"There was a timeout while trying to create resource '{resource.res_id}'.\n"
-                f"It is unclear if the resource '{resource.res_id}' was created successfully or not.\n"
-                f"Please check manually in the DSP-APP or DB.\n"
-                f"In case of successful creation, call 'resume-xmlupload' with the flag "
-                f"'--skip-first-resource' to prevent duplication.\n"
-                f"If not, a normal 'resume-xmlupload' can be started."
-            )
-            logger.error(msg)
-            raise XmlUploadInterruptedError(msg)
-        except BaseException as err:  # noqa: BLE001 (blind-except)
-            if res and res[0]:
-                # creation succeeded, but during tidy up, a Keyboard Interrupt occurred. tidy up again before escalating
-                iri, label = res
-                _tidy_up_resource_creation(iri, label, iri_resolver, resource, current_res, total_res)
-            else:
-                # unhandled exception during resource creation
-                failed_uploads.append(resource.res_id)
-            raise err from None
-        finally:
-            resources.remove(resource)
-
-    return iri_resolver, failed_uploads
-
-
-def _tidy_up_resource_creation(
-    iri: str,
-    label: str,
-    iri_resolver: IriResolver,
+
+def _tidy_up_resource_creation_idempotent(
+    upload_state: UploadState,
+    iri: str | None,
     resource: XMLResource,
-    current_res: int,
-    total_res: int,
 ) -> None:
-    iri_resolver.update(resource.res_id, iri)
-    resource_designation = f"'{label}' (ID: '{resource.res_id}', IRI: '{iri}')"
-    print(f"{datetime.now()}: Created resource {current_res}/{total_res}: {resource_designation}")
-    logger.info(f"Created resource {current_res}/{total_res}: {resource_designation}")
+    previous_successful = len(upload_state.iri_resolver.lookup)
+    previous_failed = len(upload_state.failed_uploads)
+    upcoming = len(upload_state.pending_resources)
+    current_res = previous_successful + previous_failed + 1
+    total_res = previous_successful + previous_failed + upcoming
+    if iri:
+        # resource creation succeeded: update the iri_resolver
+        upload_state.iri_resolver.lookup[resource.res_id] = iri
+        msg = f"Created resource {current_res}/{total_res}: '{resource.label}' (ID: '{resource.res_id}', IRI: '{iri}')"
+        print(f"{datetime.now()}: {msg}")
+        logger.info(msg)
+    else:  # noqa: PLR5501
+        # resource creation failed gracefully: register it as failed
+        if resource.res_id not in upload_state.failed_uploads:
+            upload_state.failed_uploads.append(resource.res_id)
+
+    if resource in upload_state.pending_resources:
+        upload_state.pending_resources.remove(resource)
 
 
 def _create_resource(
     resource: XMLResource,
     bitstream_information: BitstreamInfo | None,
     resource_create_client: ResourceCreateClient,
-) -> tuple[str, str] | tuple[None, None]:
+) -> str | None:
     try:
         return resource_create_client.create_resource(resource, bitstream_information)
     except PermanentTimeOutError as err:
         # The following block catches all exceptions and handles them in a generic way.
         # Because the calling function needs to know that this was a PermanentTimeOutError, we need to catch and
         # raise it here.
         raise err
@@ -480,64 +409,48 @@
         print(msg)
         log_msg = (
             f"Unable to create resource '{resource.label}' ({resource.res_id})\n"
             f"Resource details:\n{vars(resource)}\n"
             f"Property details:\n" + "\n".join([str(vars(prop)) for prop in resource.properties])
         )
         logger.exception(log_msg)
-        return None, None
+        return None
 
 
-def _handle_upload_error(
-    err: BaseException,
-    iri_resolver: IriResolver,
-    pending_resources: list[XMLResource],
-    failed_uploads: list[str],
-    pending_stash: Stash | None,
-    config: UploadConfig,
-    permissions_lookup: dict[str, Permissions],
-) -> None:
+def _handle_upload_error(err: BaseException, upload_state: UploadState) -> None:
     """
     In case the xmlupload must be interrupted,
     e.g. because of an error that could not be handled,
     or due to keyboard interrupt,
     this method ensures
     that all information about what is already in DSP
     is written into diagnostic files.
 
     It then quits the Python interpreter with exit code 1.
 
     Args:
         err: the error that was the cause of the abort
-        iri_resolver: a resolver for internal IDs to IRIs
-        pending_resources: resources that were not uploaded to DSP
-        failed_uploads: resources that caused an error when uploading to DSP
-        pending_stash: an object that contains all stashed links that could not yet be reapplied to their resources
-        config: the upload configuration
-        permissions_lookup: dictionary that contains the permission name as string and the corresponding Python object
+        upload_state: the current state of the upload
     """
     if isinstance(err, XmlUploadInterruptedError):
         msg = "\n==========================================\n" + err.message + "\n"
         exit_code = 0
     else:
         msg = (
             f"\n==========================================\n"
             f"{datetime.now()}: xmlupload must be aborted because of an error.\n"
             f"Error message: '{err}'\n"
             f"For more information, see the log file: {logger_savepath}\n"
         )
         exit_code = 1
 
-    upload_state = UploadState(
-        pending_resources, failed_uploads, iri_resolver.lookup, pending_stash, config, permissions_lookup
-    )
     msg += _save_upload_state(upload_state)
 
-    if failed_uploads:
-        msg += f"Independently from this, there were some resources that could not be uploaded: {failed_uploads}\n"
+    if failed := upload_state.failed_uploads:
+        msg += f"Independently from this, there were some resources that could not be uploaded: {failed}\n"
 
     if exit_code == 1:
         logger.exception(msg)
     else:
         logger.info(msg)
     print(msg)
 
@@ -546,8 +459,9 @@
 
 def _save_upload_state(upload_state: UploadState) -> str:
     save_location = upload_state.config.diagnostics.save_location
     save_location.unlink(missing_ok=True)
     save_location.touch(exist_ok=True)
     with open(save_location, "wb") as file:
         pickle.dump(upload_state, file)
+    logger.info(f"Saved the current upload state to {save_location}")
     return f"Saved the current upload state to {save_location}.\n"
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/models/custom_warnings.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/models/custom_warnings.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/models/datetimestamp.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/models/datetimestamp.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/models/exceptions.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/models/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,18 @@
             case True, str():
                 default_msg = f"\n\n{custom_msg}\n--------------------------{default_msg}"
                 super().__init__(default_msg)
             case _:
                 super().__init__(default_msg)
 
 
+class PermissionNotExistsError(BaseError):
+    """Class for errors that are raised when a permission does not exist."""
+
+
 class InputError(BaseError):
     """Class for errors that is called when the user input is invalid."""
 
 
 class UserError(BaseError):
     """
     Class for errors that are intended for user feedback.
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/models/langstring.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/models/projectContext.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/data.xsd`

 * *Files 0% similar despite different names*

#### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/data.xsd`

```diff
@@ -42,15 +42,15 @@
     <xs:restriction base="xs:string">
       <xs:pattern value="([a-z][a-z0-9+.\-]*):(//([\w_.\-~:\[\]]+)(:\d{0,6})?)(/[\w_.\-~:%()]*)*(\?[\w_.,;/\-:%=*&amp;]+)*(#[\w_.\-,~:/]*)?"/>
     </xs:restriction>
   </xs:simpleType>
   <!-- data type for knora interval -->
   <xs:simpleType name="knorainterval_type">
     <xs:restriction base="xs:token">
-      <xs:pattern value="([+-]?([0-9]+([.][0-9]*)?|[.][0-9]+)):([+-]?([0-9]+([.][0-9]*)?|[.][0-9]+))"/>
+      <xs:pattern value="\d+(\.\d+)?:\d+(\.\d+)?"/>
     </xs:restriction>
   </xs:simpleType>
   <!-- encoding types -->
   <xs:simpleType name="encoding_types">
     <xs:restriction base="xs:string">
       <xs:enumeration value="utf8"/>
       <xs:enumeration value="xml"/>
```

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/resources/schema/project.json` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/utils/connection.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/utils/connection_live.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection_live.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/utils/date_util.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/utils/logger_config.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/logger_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/utils/set_encoder.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/set_encoder.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/utils/shared.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/shared.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/utils/uri_util.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/uri_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/utils/warnings_config.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/warnings_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/utils/xml_utils.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/utils/xml_validation.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/src/dsp_tools/utils/xml_validation_models.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post0/PKG-INFO` & `dsp_tools-7.2.0.post7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 7.2.0.post0
+Version: 7.2.0.post7
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,15 +16,17 @@
 Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: networkx (>=3.3,<4.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: pandas[excel] (>=2.2.1,<3.0.0)
+Requires-Dist: pyld (>=2.0.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: rdflib (>=7.0.0,<8.0.0)
 Requires-Dist: regex (>=2024.4.28,<2025.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rustworkx (>=0.14.2,<0.15.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Project-URL: Documentation, https://docs.dasch.swiss/latest/DSP-TOOLS/
 Project-URL: Repository, https://github.com/dasch-swiss/dsp-tools
 Description-Content-Type: text/markdown
```

