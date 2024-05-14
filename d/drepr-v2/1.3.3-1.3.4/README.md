# Comparing `tmp/drepr_v2-1.3.3.tar.gz` & `tmp/drepr_v2-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drepr_v2-1.3.3.tar", max compression
+gzip compressed data, was "drepr_v2-1.3.4.tar", max compression
```

## Comparing `drepr_v2-1.3.3.tar` & `drepr_v2-1.3.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1064 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/LICENSE
--rw-r--r--   0        0        0       53 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/README.md
--rw-r--r--   0        0        0        0 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/__init__.py
--rw-r--r--   0        0        0     3754 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/__main__.py
--rw-r--r--   0        0        0     2063 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/main.py
--rw-r--r--   0        0        0        0 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/__init__.py
--rw-r--r--   0        0        0     4710 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/align.py
--rw-r--r--   0        0        0     1263 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/attr.py
--rw-r--r--   0        0        0    12298 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/drepr.py
--rw-r--r--   0        0        0     3416 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/drepr_builder.py
--rw-r--r--   0        0        0       71 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/format.py
--rw-r--r--   0        0        0     8805 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/parse_v1/__init__.py
--rw-r--r--   0        0        0     5815 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/parse_v1/align_parser.py
--rw-r--r--   0        0        0     4520 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/parse_v1/attr_parser.py
--rw-r--r--   0        0        0     5940 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/parse_v1/path_parser.py
--rw-r--r--   0        0        0     5430 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/parse_v1/preprocessing_parser.py
--rw-r--r--   0        0        0     3255 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/parse_v1/resource_parser.py
--rw-r--r--   0        0        0     7107 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/parse_v1/sm_parser.py
--rw-r--r--   0        0        0     9430 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/parse_v2/__init__.py
--rw-r--r--   0        0        0    11569 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/parse_v2/path_parser.py
--rw-r--r--   0        0        0     9359 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/parse_v2/sm_parser.py
--rw-r--r--   0        0        0     6706 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/path.py
--rw-r--r--   0        0        0      326 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/prelude.py
--rw-r--r--   0        0        0     3917 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/preprocessing.py
--rw-r--r--   0        0        0     2200 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/resource.py
--rw-r--r--   0        0        0     9252 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/models/sm.py
--rw-r--r--   0        0        0        0 2024-05-14 03:28:08.445853 drepr_v2-1.3.3/drepr/planning/__init__.py
--rw-r--r--   0        0        0    19809 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/planning/class_map_plan.py
--rw-r--r--   0        0        0    17577 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/planning/drepr_model_alignments.py
--rw-r--r--   0        0        0     4783 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/planning/topological_sorting.py
--rw-r--r--   0        0        0        0 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/program_generation/__init__.py
--rw-r--r--   0        0        0    17908 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/program_generation/alignment_fn.py
--rw-r--r--   0        0        0    23969 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/program_generation/main.py
--rw-r--r--   0        0        0     1569 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/program_generation/predefined_fn.py
--rw-r--r--   0        0        0    16794 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/program_generation/preprocessing.py
--rw-r--r--   0        0        0     1458 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/program_generation/program_space.py
--rw-r--r--   0        0        0     4966 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/program_generation/writers.py
--rw-r--r--   0        0        0        0 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/readers/__init__.py
--rw-r--r--   0        0        0      361 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/readers/csv.py
--rw-r--r--   0        0        0      365 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/readers/json.py
--rw-r--r--   0        0        0      145 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/readers/prelude.py
--rw-r--r--   0        0        0      382 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/readers/spreadsheet.py
--rw-r--r--   0        0        0       61 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/utils/__init__.py
--rw-r--r--   0        0        0     6400 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/utils/attr_data.py
--rw-r--r--   0        0        0     2960 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/utils/misc.py
--rw-r--r--   0        0        0      828 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/utils/namespace_mixin.py
--rw-r--r--   0        0        0      443 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/utils/safe.py
--rw-r--r--   0        0        0     4341 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/utils/udf.py
--rw-r--r--   0        0        0     7798 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/utils/validator.py
--rw-r--r--   0        0        0        0 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/writers/__init__.py
--rw-r--r--   0        0        0     3850 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/writers/base.py
--rw-r--r--   0        0        0     3986 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/drepr/writers/rdfgraph_writer.py
--rw-r--r--   0        0        0      605 2024-05-14 03:28:08.449853 drepr_v2-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 drepr_v2-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-14 04:26:57.299254 drepr_v2-1.3.4/LICENSE
+-rw-r--r--   0        0        0       53 2024-05-14 04:26:57.299254 drepr_v2-1.3.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 04:26:57.299254 drepr_v2-1.3.4/drepr/__init__.py
+-rw-r--r--   0        0        0     3754 2024-05-14 04:26:57.299254 drepr_v2-1.3.4/drepr/__main__.py
+-rw-r--r--   0        0        0     2063 2024-05-14 04:26:57.299254 drepr_v2-1.3.4/drepr/main.py
+-rw-r--r--   0        0        0        0 2024-05-14 04:26:57.299254 drepr_v2-1.3.4/drepr/models/__init__.py
+-rw-r--r--   0        0        0     4710 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/align.py
+-rw-r--r--   0        0        0     1263 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/attr.py
+-rw-r--r--   0        0        0    12298 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/drepr.py
+-rw-r--r--   0        0        0     3416 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/drepr_builder.py
+-rw-r--r--   0        0        0       71 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/format.py
+-rw-r--r--   0        0        0     8805 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/parse_v1/__init__.py
+-rw-r--r--   0        0        0     5815 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/parse_v1/align_parser.py
+-rw-r--r--   0        0        0     4520 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/parse_v1/attr_parser.py
+-rw-r--r--   0        0        0     5940 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/parse_v1/path_parser.py
+-rw-r--r--   0        0        0     5430 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/parse_v1/preprocessing_parser.py
+-rw-r--r--   0        0        0     3255 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/parse_v1/resource_parser.py
+-rw-r--r--   0        0        0     7107 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/parse_v1/sm_parser.py
+-rw-r--r--   0        0        0     9430 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/parse_v2/__init__.py
+-rw-r--r--   0        0        0    11569 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/parse_v2/path_parser.py
+-rw-r--r--   0        0        0     9359 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/parse_v2/sm_parser.py
+-rw-r--r--   0        0        0     6706 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/path.py
+-rw-r--r--   0        0        0      326 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/prelude.py
+-rw-r--r--   0        0        0     3917 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/preprocessing.py
+-rw-r--r--   0        0        0     2200 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/resource.py
+-rw-r--r--   0        0        0     9252 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/models/sm.py
+-rw-r--r--   0        0        0        0 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/planning/__init__.py
+-rw-r--r--   0        0        0    19809 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/planning/class_map_plan.py
+-rw-r--r--   0        0        0    17577 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/planning/drepr_model_alignments.py
+-rw-r--r--   0        0        0     4783 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/planning/topological_sorting.py
+-rw-r--r--   0        0        0        0 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/program_generation/__init__.py
+-rw-r--r--   0        0        0    17908 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/program_generation/alignment_fn.py
+-rw-r--r--   0        0        0    23969 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/program_generation/main.py
+-rw-r--r--   0        0        0     1569 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/program_generation/predefined_fn.py
+-rw-r--r--   0        0        0    16794 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/program_generation/preprocessing.py
+-rw-r--r--   0        0        0     1458 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/program_generation/program_space.py
+-rw-r--r--   0        0        0     4966 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/program_generation/writers.py
+-rw-r--r--   0        0        0        0 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/readers/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/readers/csv.py
+-rw-r--r--   0        0        0      365 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/readers/json.py
+-rw-r--r--   0        0        0      145 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/readers/prelude.py
+-rw-r--r--   0        0        0      382 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/readers/spreadsheet.py
+-rw-r--r--   0        0        0       61 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/utils/__init__.py
+-rw-r--r--   0        0        0     6400 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/utils/attr_data.py
+-rw-r--r--   0        0        0     2960 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/utils/misc.py
+-rw-r--r--   0        0        0      828 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/utils/namespace_mixin.py
+-rw-r--r--   0        0        0      443 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/utils/safe.py
+-rw-r--r--   0        0        0     5729 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/utils/udf.py
+-rw-r--r--   0        0        0     7798 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/utils/validator.py
+-rw-r--r--   0        0        0        0 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/writers/__init__.py
+-rw-r--r--   0        0        0     3850 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/writers/base.py
+-rw-r--r--   0        0        0     3986 2024-05-14 04:26:57.303254 drepr_v2-1.3.4/drepr/writers/rdfgraph_writer.py
+-rw-r--r--   0        0        0      605 2024-05-14 04:26:57.307254 drepr_v2-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 drepr_v2-1.3.4/PKG-INFO
```

### Comparing `drepr_v2-1.3.3/LICENSE` & `drepr_v2-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/__main__.py` & `drepr_v2-1.3.4/drepr/__main__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/main.py` & `drepr_v2-1.3.4/drepr/main.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/align.py` & `drepr_v2-1.3.4/drepr/models/align.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/attr.py` & `drepr_v2-1.3.4/drepr/models/attr.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/drepr.py` & `drepr_v2-1.3.4/drepr/models/drepr.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/drepr_builder.py` & `drepr_v2-1.3.4/drepr/models/drepr_builder.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/parse_v1/__init__.py` & `drepr_v2-1.3.4/drepr/models/parse_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/parse_v1/align_parser.py` & `drepr_v2-1.3.4/drepr/models/parse_v1/align_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/parse_v1/attr_parser.py` & `drepr_v2-1.3.4/drepr/models/parse_v1/attr_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/parse_v1/path_parser.py` & `drepr_v2-1.3.4/drepr/models/parse_v1/path_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/parse_v1/preprocessing_parser.py` & `drepr_v2-1.3.4/drepr/models/parse_v1/preprocessing_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/parse_v1/resource_parser.py` & `drepr_v2-1.3.4/drepr/models/parse_v1/resource_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/parse_v1/sm_parser.py` & `drepr_v2-1.3.4/drepr/models/parse_v1/sm_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/parse_v2/__init__.py` & `drepr_v2-1.3.4/drepr/models/parse_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/parse_v2/path_parser.py` & `drepr_v2-1.3.4/drepr/models/parse_v2/path_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/parse_v2/sm_parser.py` & `drepr_v2-1.3.4/drepr/models/parse_v2/sm_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/path.py` & `drepr_v2-1.3.4/drepr/models/path.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/preprocessing.py` & `drepr_v2-1.3.4/drepr/models/preprocessing.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/resource.py` & `drepr_v2-1.3.4/drepr/models/resource.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/models/sm.py` & `drepr_v2-1.3.4/drepr/models/sm.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/planning/class_map_plan.py` & `drepr_v2-1.3.4/drepr/planning/class_map_plan.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/planning/drepr_model_alignments.py` & `drepr_v2-1.3.4/drepr/planning/drepr_model_alignments.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/planning/topological_sorting.py` & `drepr_v2-1.3.4/drepr/planning/topological_sorting.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/program_generation/alignment_fn.py` & `drepr_v2-1.3.4/drepr/program_generation/alignment_fn.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/program_generation/main.py` & `drepr_v2-1.3.4/drepr/program_generation/main.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/program_generation/predefined_fn.py` & `drepr_v2-1.3.4/drepr/program_generation/predefined_fn.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/program_generation/preprocessing.py` & `drepr_v2-1.3.4/drepr/program_generation/preprocessing.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/program_generation/program_space.py` & `drepr_v2-1.3.4/drepr/program_generation/program_space.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/program_generation/writers.py` & `drepr_v2-1.3.4/drepr/program_generation/writers.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/utils/attr_data.py` & `drepr_v2-1.3.4/drepr/utils/attr_data.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/utils/misc.py` & `drepr_v2-1.3.4/drepr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/utils/namespace_mixin.py` & `drepr_v2-1.3.4/drepr/utils/namespace_mixin.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/utils/udf.py` & `drepr_v2-1.3.4/drepr/utils/udf.py`

 * *Files 14% similar despite different names*

```diff
@@ -93,15 +93,48 @@
             for stmt in tree.body:
                 out[0].children.extend(self._parse_ast(stmt, imports))
             if len(tree.orelse) > 0:
                 out.append(SourceTree("else:", []))
                 for stmt in tree.orelse:
                     out[1].children.extend(self._parse_ast(stmt, imports))
             return out
-        raise NotImplementedError()
+
+        if isinstance(tree, ast.Continue):
+            return [SourceTree("continue", [])]
+
+        if isinstance(tree, ast.Break):
+            return [SourceTree("break", [])]
+
+        if isinstance(tree, ast.Try):
+            out = [SourceTree("try:", [])]
+            for stmt in tree.body:
+                out[0].children.extend(self._parse_ast(stmt, imports))
+
+            if len(tree.handlers) > 0:
+                for handler in tree.handlers:
+                    except_args = ["except"]
+                    if handler.type is not None:
+                        except_args.append(self._get_node_code(handler.type))
+                    if handler.name is not None:
+                        except_args.append(handler.name)
+
+                    out.append(SourceTree(" ".join(except_args) + ":", []))
+                    for stmt in handler.body:
+                        out[-1].children.extend(self._parse_ast(stmt, imports))
+            if len(tree.orelse) > 0:
+                out.append(SourceTree("else:", []))
+                for stmt in tree.orelse:
+                    out[-1].children.extend(self._parse_ast(stmt, imports))
+            if len(tree.finalbody) > 0:
+                out.append(SourceTree("finally:", []))
+                for stmt in tree.finalbody:
+                    out[-1].children.extend(self._parse_ast(stmt, imports))
+            return out
+
+        raise NotImplementedError(type(tree))
 
     def _get_node_code(self, node: ast.AST) -> str:
         lines = self.source_code_lines[node.lineno - 1 : node.end_lineno]
         lines[0] = lines[0][node.col_offset :]
         lines[-1] = lines[-1][: node.end_col_offset]
         return "\n".join(lines)
```

### Comparing `drepr_v2-1.3.3/drepr/utils/validator.py` & `drepr_v2-1.3.4/drepr/utils/validator.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/writers/base.py` & `drepr_v2-1.3.4/drepr/writers/base.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/drepr/writers/rdfgraph_writer.py` & `drepr_v2-1.3.4/drepr/writers/rdfgraph_writer.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.3/pyproject.toml` & `drepr_v2-1.3.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drepr-v2"
-version = "1.3.3"
+version = "1.3.4"
 description = ""
 authors = ["Binh Vu <binh@toan2.com>"]
 readme = "README.md"
 packages = [{ include = "drepr" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `drepr_v2-1.3.3/PKG-INFO` & `drepr_v2-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drepr-v2
-Version: 1.3.3
+Version: 1.3.4
 Summary: 
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

