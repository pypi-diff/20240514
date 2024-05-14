# Comparing `tmp/cognite_neat-0.77.0.tar.gz` & `tmp/cognite_neat-0.77.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.77.0.tar", max compression
+gzip compressed data, was "cognite_neat-0.77.1.tar", max compression
```

## Comparing `cognite_neat-0.77.0.tar` & `cognite_neat-0.77.1.tar`

### file list

```diff
@@ -1,277 +1,278 @@
--rw-r--r--   0        0        0    11351 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/LICENSE
--rw-r--r--   0        0        0     6775 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/README.md
--rw-r--r--   0        0        0       61 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4232 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     1675 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      585 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3523 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4597 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13686 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     8121 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12393 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-05-13 12:04:56.624934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-05-13 12:04:56.624934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-13 12:04:56.624934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-05-13 12:04:56.624934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-05-13 12:04:56.624934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1423717 2024-05-13 12:04:56.628934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
--rw-r--r--   0        0        0     2667 2024-05-13 12:04:56.628934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
--rw-r--r--   0        0        0  6282875 2024-05-13 12:04:56.652933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
--rw-r--r--   0        0        0   240334 2024-05-13 12:04:56.656933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     6145 2024-05-13 12:04:56.664934 cognite_neat-0.77.0/cognite/neat/config.py
--rw-r--r--   0        0        0     1300 2024-05-13 12:04:56.664934 cognite_neat-0.77.0/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-05-13 12:04:56.664934 cognite_neat-0.77.0/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-05-13 12:04:56.664934 cognite_neat-0.77.0/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-13 12:04:56.664934 cognite_neat-0.77.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-13 12:04:56.668933 cognite_neat-0.77.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-13 12:04:56.668933 cognite_neat-0.77.0/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-13 12:04:56.668933 cognite_neat-0.77.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-13 12:04:56.668933 cognite_neat-0.77.0/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14961 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      149 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    13473 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/legacy/__init__.py
--rw-r--r--   0        0        0       73 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/legacy/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/__init__.py
--rw-r--r--   0        0        0      363 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_base.py
--rw-r--r--   0        0        0    11734 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_dexpi.py
--rw-r--r--   0        0        0    17695 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14908 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      701 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/__init__.py
--rw-r--r--   0        0        0    23823 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_asset_loader.py
--rw-r--r--   0        0        0     2383 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_base.py
--rw-r--r--   0        0        0     2835 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2321 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5023 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/models.py
--rw-r--r--   0        0        0    40464 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22707 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12979 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
--rw-r--r--   0        0        0     3328 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/validator.py
--rw-r--r--   0        0        0      149 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/__init__.py
--rw-r--r--   0        0        0    14289 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/__init__.py
--rw-r--r--   0        0        0     4765 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0    18719 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    14737 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/transformer.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/__init__.py
--rw-r--r--   0        0        0     8610 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_base.py
--rw-r--r--   0        0        0      102 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_core/__init__.py
--rw-r--r--   0        0        0      771 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
--rw-r--r--   0        0        0    36813 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8312 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0     6251 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2graphql.py
--rw-r--r--   0        0        0    18458 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0    28805 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3881 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     1085 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2triples.py
--rw-r--r--   0        0        0     5767 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/__init__.py
--rw-r--r--   0        0        0     2273 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_base.py
--rw-r--r--   0        0        0     6476 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_dict2rules.py
--rw-r--r--   0        0        0     7697 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0    12093 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_json2rules.py
--rw-r--r--   0        0        0       63 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9407 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10557 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1502 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0      421 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_xsd2rules.py
--rw-r--r--   0        0        0     1601 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      127 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/_base.py
--rw-r--r--   0        0        0    12382 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7351 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51091 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/tables.py
--rw-r--r--   0        0        0     4402 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/value_types.py
--rw-r--r--   0        0        0     1898 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0      170 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0      115 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/analysis/__init__.py
--rw-r--r--   0        0        0      669 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/analysis/_base.py
--rw-r--r--   0        0        0    19584 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/analysis/_information_rules.py
--rw-r--r--   0        0        0      374 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    65934 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      413 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1976 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    13530 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    14934 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    20120 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3026 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4078 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      408 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4274 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    18317 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12663 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6717 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11897 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7591 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7786 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7437 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     6925 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11882 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4275 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6438 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    22035 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     5748 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3385 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0    12288 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13936 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      782 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0    10876 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0    11030 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/_rdfpath.py
--rw-r--r--   0        0        0      305 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/_types/__init__.py
--rw-r--r--   0        0        0      929 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/_types/_base.py
--rw-r--r--   0        0        0     3197 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/_types/_field.py
--rw-r--r--   0        0        0     6078 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/data_types.py
--rw-r--r--   0        0        0      491 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/__init__.py
--rw-r--r--   0        0        0     5706 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_converter.py
--rw-r--r--   0        0        0    18809 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_exporter.py
--rw-r--r--   0        0        0    15545 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_rules.py
--rw-r--r--   0        0        0    13620 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_rules_input.py
--rw-r--r--   0        0        0    41719 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_schema.py
--rw-r--r--   0        0        0     6668 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_serializer.py
--rw-r--r--   0        0        0    14273 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_validation.py
--rw-r--r--   0        0        0     2993 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/domain.py
--rw-r--r--   0        0        0    16395 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/entities.py
--rw-r--r--   0        0        0      195 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/information/__init__.py
--rw-r--r--   0        0        0     7964 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/information/_converter.py
--rw-r--r--   0        0        0    15546 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/rules/models/information/_rules.py
--rw-r--r--   0        0        0     6154 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/rules/models/wrapped_entities.py
--rw-r--r--   0        0        0       68 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11336 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6303 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2714 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12818 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26800 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0    14102 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6570 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     3009 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0        0 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0      225 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_loader.py
--rw-r--r--   0        0        0     6295 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_store.py
--rw-r--r--   0        0        0    22898 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_exporter.py
--rw-r--r--   0        0        0    10338 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_importer.py
--rw-r--r--   0        0        0     4729 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_validator.py
--rw-r--r--   0        0        0       32 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/io/__init__.py
--rw-r--r--   0        0        0    16874 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/io/io_steps.py
--rw-r--r--   0        0        0      274 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/__init__.py
--rw-r--r--   0        0        0     3919 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
--rw-r--r--   0        0        0    29357 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
--rw-r--r--   0        0        0    27265 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
--rw-r--r--   0        0        0    12704 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_store.py
--rw-r--r--   0        0        0     2351 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
--rw-r--r--   0        0        0    20462 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
--rw-r--r--   0        0        0    28065 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
--rw-r--r--   0        0        0     2943 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    11007 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4591 2024-05-13 12:04:57.080934 cognite_neat-0.77.0/pyproject.toml
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.77.0/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/LICENSE
+-rw-r--r--   0        0        0     6775 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/README.md
+-rw-r--r--   0        0        0       61 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4232 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     1675 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      585 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3523 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4597 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13686 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8121 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12393 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1423717 2024-05-14 14:34:35.476744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
+-rw-r--r--   0        0        0     2667 2024-05-14 14:34:35.476744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
+-rw-r--r--   0        0        0  6282875 2024-05-14 14:34:35.500744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
+-rw-r--r--   0        0        0   240334 2024-05-14 14:34:35.500744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     6145 2024-05-14 14:34:35.508744 cognite_neat-0.77.1/cognite/neat/config.py
+-rw-r--r--   0        0        0     1300 2024-05-14 14:34:35.508744 cognite_neat-0.77.1/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-05-14 14:34:35.508744 cognite_neat-0.77.1/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-05-14 14:34:35.508744 cognite_neat-0.77.1/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-14 14:34:35.512744 cognite_neat-0.77.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14961 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14908 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23823 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2383 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2835 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40464 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22707 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12979 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3328 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14737 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36813 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5767 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2273 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7697 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0     1898 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      170 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19584 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1976 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    13688 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    14934 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    20120 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3026 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4078 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      408 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4274 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    18274 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12663 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6717 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11897 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7591 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7786 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7437 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     6925 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11882 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4275 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6438 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    22035 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     5748 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3385 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0    12288 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13936 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      782 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0    10876 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0    11030 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/_rdfpath.py
+-rw-r--r--   0        0        0      305 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/_types/__init__.py
+-rw-r--r--   0        0        0      929 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/_types/_base.py
+-rw-r--r--   0        0        0     3197 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/_types/_field.py
+-rw-r--r--   0        0        0     6078 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/data_types.py
+-rw-r--r--   0        0        0      491 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/__init__.py
+-rw-r--r--   0        0        0     5706 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_converter.py
+-rw-r--r--   0        0        0    18903 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_exporter.py
+-rw-r--r--   0        0        0    15568 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_rules.py
+-rw-r--r--   0        0        0    13620 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_rules_input.py
+-rw-r--r--   0        0        0    41973 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_schema.py
+-rw-r--r--   0        0        0     6668 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_serializer.py
+-rw-r--r--   0        0        0    14141 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_validation.py
+-rw-r--r--   0        0        0     2993 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/domain.py
+-rw-r--r--   0        0        0    16395 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/entities.py
+-rw-r--r--   0        0        0      195 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/information/__init__.py
+-rw-r--r--   0        0        0     7964 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/information/_converter.py
+-rw-r--r--   0        0        0    15546 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/information/_rules.py
+-rw-r--r--   0        0        0     7157 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/wrapped_entities.py
+-rw-r--r--   0        0        0       68 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0     5831 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_classes.py
+-rw-r--r--   0        0        0      483 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11336 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6303 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2714 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12818 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26800 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    14102 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6570 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3009 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_store.py
+-rw-r--r--   0        0        0    22898 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_exporter.py
+-rw-r--r--   0        0        0    10338 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_importer.py
+-rw-r--r--   0        0        0     4844 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_validator.py
+-rw-r--r--   0        0        0       32 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/io/__init__.py
+-rw-r--r--   0        0        0    16874 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/io/io_steps.py
+-rw-r--r--   0        0        0      274 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/__init__.py
+-rw-r--r--   0        0        0     3919 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
+-rw-r--r--   0        0        0    29357 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
+-rw-r--r--   0        0        0    27265 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
+-rw-r--r--   0        0        0    12704 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_store.py
+-rw-r--r--   0        0        0     2351 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
+-rw-r--r--   0        0        0    20462 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
+-rw-r--r--   0        0        0    28065 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
+-rw-r--r--   0        0        0     2943 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    11007 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4591 2024-05-14 14:34:35.928751 cognite_neat-0.77.1/pyproject.toml
+-rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.77.1/PKG-INFO
```

### Comparing `cognite_neat-0.77.0/LICENSE` & `cognite_neat-0.77.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/README.md` & `cognite_neat-0.77.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/configuration.py` & `cognite_neat-0.77.1/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.77.1/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/explorer.py` & `cognite_neat-0.77.1/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.77.1/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.77.1/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.77.1/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.77.1/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.77.1/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.77.1/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.77.1/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.77.1/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.77.1/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.77.1/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/config.py` & `cognite_neat-0.77.1/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/constants.py` & `cognite_neat-0.77.1/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/exceptions.py` & `cognite_neat-0.77.1/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.77.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.77.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.77.1/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/exceptions.py` & `cognite_neat-0.77.1/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.77.1/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.77.1/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.77.1/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.77.1/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.77.1/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.77.1/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.77.1/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.77.1/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/exceptions.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_dexpi.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/__init__.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_asset_loader.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_base.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_exceptions.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/labels.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/models.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/rdf_to_dms.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/validator.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/__init__.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_base.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_graphdb_store.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_memory_store.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_oxigraph_store.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_oxrdflib.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/entity_matcher.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/transformer.py` & `cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/analysis.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/__init__.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-model.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/rules-template.xlsx` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/skos-rules.xlsx` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/wind-energy.owl` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exceptions.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/__init__.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_base.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_core/rules2labels.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2dms.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2excel.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2graphql.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2ontology.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2rules.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2triples.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_validation.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/__init__.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_base.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_dict2rules.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_dms2rules.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_graph2rules.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_json2rules.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_yaml2rules.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/models/_base.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/models/raw_rules.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/models/rdfpath.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/models/rules.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/rules/models/value_types.py` & `cognite_neat-0.77.1/cognite/neat/legacy/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/analysis/_base.py` & `cognite_neat-0.77.1/cognite/neat/rules/analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/analysis/_information_rules.py` & `cognite_neat-0.77.1/cognite/neat/rules/analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.77.1/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/exceptions.py` & `cognite_neat-0.77.1/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.77.1/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.77.1/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 import warnings
 from collections.abc import Collection, Iterable
 from pathlib import Path
 from typing import Literal, TypeAlias, cast
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes._base import CogniteResource, CogniteResourceList
-from cognite.client.data_classes.data_modeling import DataModelApply, DataModelApplyList, DataModelId
+from cognite.client.data_classes.data_modeling import (
+    ContainerApplyList,
+    DataModelApply,
+    DataModelApplyList,
+    DataModelId,
+    SpaceApplyList,
+    ViewApplyList,
+)
 from cognite.client.exceptions import CogniteAPIError
 
 from cognite.neat.rules import issues
 from cognite.neat.rules._shared import Rules
 from cognite.neat.rules.issues import IssueList
 from cognite.neat.rules.models import InformationRules
 from cognite.neat.rules.models.dms import DMSRules, DMSSchema, PipelineSchema
@@ -260,19 +267,19 @@
 
     def _prepare_schema_and_exporters(
         self, rules, client
     ) -> tuple[DMSSchema, list[tuple[CogniteResourceList, ResourceLoader]]]:
         schema = self.export(rules)
         to_export: list[tuple[CogniteResourceList, ResourceLoader]] = []
         if self.export_components.intersection({"all", "spaces"}):
-            to_export.append((schema.spaces, SpaceLoader(client)))
+            to_export.append((SpaceApplyList(schema.spaces.values()), SpaceLoader(client)))
         if self.export_components.intersection({"all", "containers"}):
-            to_export.append((schema.containers, ContainerLoader(client)))
+            to_export.append((ContainerApplyList(schema.containers.values()), ContainerLoader(client)))
         if self.export_components.intersection({"all", "views"}):
-            to_export.append((schema.views, ViewLoader(client, self.existing_handling)))
+            to_export.append((ViewApplyList(schema.views.values()), ViewLoader(client, self.existing_handling)))
         if self.export_components.intersection({"all", "data_models"}):
             to_export.append((DataModelApplyList([schema.data_model]), DataModelLoader(client)))
         if isinstance(schema, PipelineSchema):
             to_export.append((schema.databases, RawDatabaseLoader(client)))
             to_export.append((schema.raw_tables, RawTableLoader(client)))
             to_export.append((schema.transformations, TransformationLoader(client)))
         return schema, to_export
```

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.77.1/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_dms2rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,19 +56,17 @@
         # Calling this root schema to distinguish it from
         # * User Schema
         # * Reference Schema
         self.root_schema = schema
         self.metadata = metadata
         self.ref_metadata = ref_metadata
         self.issue_list = IssueList(read_issues)
-        self._all_containers_by_id = {container.as_id(): container for container in schema.containers}
+        self._all_containers_by_id = schema.containers.copy()
         if self.root_schema.reference:
-            self._all_containers_by_id.update(
-                {container.as_id(): container for container in self.root_schema.reference.containers}
-            )
+            self._all_containers_by_id.update(self.root_schema.reference.containers)
 
     @classmethod
     def from_data_model_id(
         cls,
         client: CogniteClient,
         data_model_id: DataModelIdentifier,
         reference_model_id: DataModelIdentifier | None = None,
@@ -196,15 +194,15 @@
             reference: DMSRules | None = None
             if (ref_schema := self.root_schema.reference) and (ref_model := ref_schema.data_model):
                 # Reference should always be an enterprise model.
                 reference = DMSRules(
                     **self._create_rule_components(
                         ref_model,
                         ref_schema,
-                        self.ref_metadata or self._create_default_metadata(ref_schema.views),
+                        self.ref_metadata or self._create_default_metadata(list(ref_schema.views.values())),
                         DataModelType.enterprise,
                     )
                 )
                 schema_completeness = SchemaCompleteness.extended
                 data_model_type = DataModelType.solution
 
             user_rules = DMSRules(
@@ -224,16 +222,15 @@
         data_model: dm.DataModelApply,
         schema: DMSSchema,
         metadata: DMSMetadata | None = None,
         data_model_type: DataModelType | None = None,
         schema_completeness: SchemaCompleteness | None = None,
     ) -> dict[str, Any]:
         properties = SheetList[DMSProperty]()
-        for view in schema.views:
-            view_id = view.as_id()
+        for view_id, view in schema.views.items():
             view_entity = ViewEntity.from_id(view_id)
             class_entity = view_entity.as_class()
             for prop_id, prop in (view.properties or {}).items():
                 dms_property = self._create_dms_property(prop_id, prop, view_entity, class_entity)
                 if dms_property is not None:
                     properties.append(dms_property)
 
@@ -246,18 +243,21 @@
             metadata.data_model_type = data_model_type
         if schema_completeness is not None:
             metadata.schema_ = schema_completeness
         return dict(
             metadata=metadata,
             properties=properties,
             containers=SheetList[DMSContainer](
-                data=[DMSContainer.from_container(container) for container in schema.containers]
+                data=[DMSContainer.from_container(container) for container in schema.containers.values()]
             ),
             views=SheetList[DMSView](
-                data=[DMSView.from_view(view, in_model=view.as_id() in data_model_view_ids) for view in schema.views]
+                data=[
+                    DMSView.from_view(view, in_model=view_id in data_model_view_ids)
+                    for view_id, view in schema.views.items()
+                ]
             ),
         )
 
     @classmethod
     def _create_default_metadata(cls, views: Sequence[dm.View | dm.ViewApply]) -> DMSMetadata:
         now = datetime.now().replace(microsecond=0)
         space = Counter(view.space for view in views).most_common(1)[0][0]
```

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.77.1/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.77.1/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/issues/base.py` & `cognite_neat-0.77.1/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.77.1/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.77.1/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.77.1/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.77.1/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.77.1/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.77.1/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/__init__.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/_base.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/_rdfpath.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/_rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/_types/_base.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/_types/_field.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/data_types.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_converter.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_exporter.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     DMSNodeEntity,
     DMSUnknownEntity,
     ReferenceEntity,
     ViewEntity,
     ViewPropertyEntity,
 )
 from cognite.neat.rules.models.wrapped_entities import DMSFilter, HasDataFilter, NodeTypeFilter
+from cognite.neat.utils.cdf_classes import ContainerApplyDict, NodeApplyDict, SpaceApplyDict, ViewApplyDict
 
 from ._rules import DMSMetadata, DMSProperty, DMSRules, DMSView
 from ._schema import DMSSchema, PipelineSchema
 
 
 class _DMSExporter:
     """The DMS Exporter is responsible for exporting the DMSRules to a DMSSchema.
@@ -47,29 +48,31 @@
     ):
         self.include_pipeline = include_pipeline
         self.instance_space = instance_space
         self.rules = rules
         self._ref_schema = rules.reference.as_schema() if rules.reference else None
         if self._ref_schema:
             # We skip version as that will always be missing in the reference
-            self._ref_views_by_id = {dm.ViewId(view.space, view.external_id): view for view in self._ref_schema.views}
+            self._ref_views_by_id = {
+                dm.ViewId(view.space, view.external_id): view for view in self._ref_schema.views.values()
+            }
         else:
             self._ref_views_by_id = {}
 
     def to_schema(self) -> DMSSchema:
         rules = self.rules
         container_properties_by_id, view_properties_by_id = self._gather_properties()
         containers = self._create_containers(container_properties_by_id)
 
         views, node_types = self._create_views_with_node_types(view_properties_by_id)
 
         views_not_in_model = {view.view.as_id() for view in rules.views if not view.in_model}
         data_model = rules.metadata.as_data_model()
         data_model.views = sorted(
-            [view_id for view_id in views.as_ids() if view_id not in views_not_in_model],
+            [view_id for view_id in views.keys() if view_id not in views_not_in_model],
             key=lambda v: v.as_tuple(),  # type: ignore[union-attr]
         )
 
         spaces = self._create_spaces(rules.metadata, containers, views, data_model)
 
         output = DMSSchema(
             spaces=spaces,
@@ -85,57 +88,55 @@
             output.reference = self._ref_schema
 
         return output
 
     def _create_spaces(
         self,
         metadata: DMSMetadata,
-        containers: dm.ContainerApplyList,
-        views: dm.ViewApplyList,
+        containers: ContainerApplyDict,
+        views: ViewApplyDict,
         data_model: dm.DataModelApply,
-    ) -> dm.SpaceApplyList:
-        used_spaces = {container.space for container in containers} | {view.space for view in views}
+    ) -> SpaceApplyDict:
+        used_spaces = {container.space for container in containers.values()} | {view.space for view in views.values()}
         if len(used_spaces) == 1:
             # We skip the default space and only use this space for the data model
             data_model.space = used_spaces.pop()
-            spaces = dm.SpaceApplyList([dm.SpaceApply(space=data_model.space)])
+            spaces = SpaceApplyDict([dm.SpaceApply(space=data_model.space)])
         else:
             used_spaces.add(metadata.space)
-            spaces = dm.SpaceApplyList([dm.SpaceApply(space=space) for space in used_spaces])
-        if self.instance_space and self.instance_space not in {space.space for space in spaces}:
-            spaces.append(dm.SpaceApply(space=self.instance_space, name=self.instance_space))
+            spaces = SpaceApplyDict([dm.SpaceApply(space=space) for space in used_spaces])
+        if self.instance_space and self.instance_space not in spaces:
+            spaces[self.instance_space] = dm.SpaceApply(space=self.instance_space, name=self.instance_space)
         return spaces
 
     def _create_views_with_node_types(
         self,
         view_properties_by_id: dict[dm.ViewId, list[DMSProperty]],
-    ) -> tuple[dm.ViewApplyList, dm.NodeApplyList]:
-        views = dm.ViewApplyList([dms_view.as_view() for dms_view in self.rules.views])
+    ) -> tuple[ViewApplyDict, NodeApplyDict]:
+        views = ViewApplyDict([dms_view.as_view() for dms_view in self.rules.views])
         dms_view_by_id = {dms_view.view.as_id(): dms_view for dms_view in self.rules.views}
 
-        for view in views:
-            view_id = view.as_id()
+        for view_id, view in views.items():
             view.properties = {}
             if not (view_properties := view_properties_by_id.get(view_id)):
                 continue
             for prop in view_properties:
                 view_property = self._create_view_property(prop, view_properties_by_id)
                 if view_property is not None:
                     view.properties[prop.view_property] = view_property
 
         data_model_type = self.rules.metadata.data_model_type
         unique_node_types: set[dm.NodeId] = set()
-        parent_views = {parent for view in views for parent in view.implements or []}
-        for view in views:
-            dms_view = dms_view_by_id.get(view.as_id())
-            dms_properties = view_properties_by_id.get(view.as_id(), [])
+        parent_views = {parent for view in views.values() for parent in view.implements or []}
+        for view_id, view in views.items():
+            dms_view = dms_view_by_id.get(view_id)
+            dms_properties = view_properties_by_id.get(view_id, [])
             view_filter = self._create_view_filter(view, dms_view, data_model_type, dms_properties)
 
             view.filter = view_filter.as_dms_filter()
-
             if isinstance(view_filter, NodeTypeFilter):
                 unique_node_types.update(view_filter.nodes)
                 if view.as_id() in parent_views:
                     warnings.warn(issues.dms.NodeTypeFilterOnParentViewWarning(view.as_id()), stacklevel=2)
             elif isinstance(view_filter, HasDataFilter) and data_model_type == DataModelType.solution:
                 if dms_view and isinstance(dms_view.reference, ReferenceEntity):
                     references = {dms_view.reference.as_view_id()}
@@ -147,15 +148,15 @@
                     }
                 else:
                     continue
                 warnings.warn(
                     issues.dms.HasDataFilterOnViewWithReferencesWarning(view.as_id(), list(references)), stacklevel=2
                 )
 
-        return views, dm.NodeApplyList(
+        return views, NodeApplyDict(
             [dm.NodeApply(space=node.space, external_id=node.external_id) for node in unique_node_types]
         )
 
     @classmethod
     def _create_edge_type_from_prop(cls, prop: DMSProperty) -> dm.DirectRelationReference:
         if isinstance(prop.reference, ReferenceEntity):
             ref_view_prop = prop.reference.as_view_property_id()
@@ -170,15 +171,15 @@
             # This is the same convention as used when converting GraphQL to DMS
             external_id=f"{view_id.external_id}.{property_}",
         )
 
     def _create_containers(
         self,
         container_properties_by_id: dict[dm.ContainerId, list[DMSProperty]],
-    ) -> dm.ContainerApplyList:
+    ) -> ContainerApplyDict:
         containers = dm.ContainerApplyList(
             [dms_container.as_container() for dms_container in self.rules.containers or []]
         )
         container_to_drop = set()
         for container in containers:
             container_id = container.as_id()
             if not (container_properties := container_properties_by_id.get(container_id)):
@@ -225,17 +226,15 @@
         for container in containers:
             if container.constraints:
                 container.constraints = {
                     name: const
                     for name, const in container.constraints.items()
                     if not (isinstance(const, dm.RequiresConstraint) and const.require in container_to_drop)
                 }
-        return dm.ContainerApplyList(
-            [container for container in containers if container.as_id() not in container_to_drop]
-        )
+        return ContainerApplyDict([container for container in containers if container.as_id() not in container_to_drop])
 
     def _gather_properties(self) -> tuple[dict[dm.ContainerId, list[DMSProperty]], dict[dm.ViewId, list[DMSProperty]]]:
         container_properties_by_id: dict[dm.ContainerId, list[DMSProperty]] = defaultdict(list)
         view_properties_by_id: dict[dm.ViewId, list[DMSProperty]] = defaultdict(list)
         for prop in self.rules.properties:
             view_id = prop.view.as_id()
             view_properties_by_id[view_id].append(prop)
@@ -250,14 +249,15 @@
         self,
         view: dm.ViewApply,
         dms_view: DMSView | None,
         data_model_type: DataModelType,
         dms_properties: list[DMSProperty],
     ) -> DMSFilter:
         selected_filter_name = (dms_view and dms_view.filter_ and dms_view.filter_.name) or ""
+
         if dms_view and dms_view.filter_ and not dms_view.filter_.is_empty:
             # Has Explicit Filter, use it
             return dms_view.filter_
 
         if data_model_type == DataModelType.solution and selected_filter_name in [NodeTypeFilter.name, ""]:
             if (
                 dms_view
```

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_rules.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     DMSUnknownEntity,
     ReferenceEntity,
     URLEntity,
     ViewEntity,
     ViewEntityList,
     ViewPropertyEntity,
 )
-from cognite.neat.rules.models.wrapped_entities import HasDataFilter, NodeTypeFilter
+from cognite.neat.rules.models.wrapped_entities import HasDataFilter, NodeTypeFilter, RawFilter
 
 from ._schema import DMSSchema
 
 if TYPE_CHECKING:
     from cognite.neat.rules.models.information._rules import InformationRules
 
 if sys.version_info >= (3, 11):
@@ -253,15 +253,15 @@
 
 class DMSView(SheetEntity):
     view: ViewEntity = Field(alias="View")
     name: str | None = Field(alias="Name", default=None)
     description: str | None = Field(alias="Description", default=None)
     implements: ViewEntityList | None = Field(None, alias="Implements")
     reference: URLEntity | ReferenceEntity | None = Field(alias="Reference", default=None, union_mode="left_to_right")
-    filter_: HasDataFilter | NodeTypeFilter | None = Field(None, alias="Filter")
+    filter_: HasDataFilter | NodeTypeFilter | RawFilter | None = Field(None, alias="Filter")
     in_model: bool = Field(True, alias="In Model")
     class_: ClassEntity = Field(alias="Class (linage)")
 
     def as_view(self) -> dm.ViewApply:
         view_id = self.view.as_id()
         return dm.ViewApply(
             space=view_id.space,
```

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_rules_input.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_rules_input.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_schema.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import sys
 import warnings
 import zipfile
 from collections import Counter, defaultdict
-from collections.abc import Sequence
 from dataclasses import Field, dataclass, field, fields
 from pathlib import Path
 from typing import Any, ClassVar, cast
 
 import yaml
 from cognite.client import CogniteClient
 from cognite.client import data_modeling as dm
@@ -27,32 +26,39 @@
     MissingEdgeViewError,
     MissingParentViewError,
     MissingSourceViewError,
     MissingSpaceError,
     MissingViewError,
 )
 from cognite.neat.rules.models.data_types import _DATA_TYPE_BY_DMS_TYPE
+from cognite.neat.utils.cdf_classes import (
+    CogniteResourceDict,
+    ContainerApplyDict,
+    NodeApplyDict,
+    SpaceApplyDict,
+    ViewApplyDict,
+)
 from cognite.neat.utils.cdf_loaders import ViewLoader
 from cognite.neat.utils.cdf_loaders.data_classes import RawTableWrite, RawTableWriteList
 from cognite.neat.utils.text import to_camel
 from cognite.neat.utils.utils import get_inheritance_path
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 
 @dataclass
 class DMSSchema:
     data_model: dm.DataModelApply | None = None
-    spaces: dm.SpaceApplyList = field(default_factory=lambda: dm.SpaceApplyList([]))
-    views: dm.ViewApplyList = field(default_factory=lambda: dm.ViewApplyList([]))
-    containers: dm.ContainerApplyList = field(default_factory=lambda: dm.ContainerApplyList([]))
-    node_types: dm.NodeApplyList = field(default_factory=lambda: dm.NodeApplyList([]))
+    spaces: SpaceApplyDict = field(default_factory=SpaceApplyDict)
+    views: ViewApplyDict = field(default_factory=ViewApplyDict)
+    containers: ContainerApplyDict = field(default_factory=ContainerApplyDict)
+    node_types: NodeApplyDict = field(default_factory=NodeApplyDict)
     # The last schema is the previous version of the data model. In the case, extension=addition, this
     # should not be modified.
     last: "DMSSchema | None" = None
     # Reference is typically the Enterprise model, while this is the solution model.
     reference: "DMSSchema | None" = None
 
     _FIELD_NAME_BY_RESOURCE_TYPE: ClassVar[dict[str, str]] = {
@@ -61,30 +67,29 @@
         "datamodel": "data_model",
         "space": "spaces",
         "node": "node_types",
     }
 
     def _get_mapped_container_from_view(self, view_id: dm.ViewId) -> set[dm.ContainerId]:
         # index all views, including ones from reference
-        indexed_views = {
-            **{view.as_id(): view for view in self.views},
-            **({view.as_id(): view for view in self.reference.views} if self.reference else {}),
-        }
+        view_by_id = self.views.copy()
+        if self.reference:
+            view_by_id.update(self.reference.views)
 
-        if view_id not in indexed_views:
+        if view_id not in view_by_id:
             raise ValueError(f"View {view_id} not found")
 
-        indexed_implemented_views = {id_: view.implements for id_, view in indexed_views.items()}
+        indexed_implemented_views = {id_: view.implements for id_, view in view_by_id.items()}
         view_inheritance = get_inheritance_path(view_id, indexed_implemented_views)
 
-        directly_referenced_containers = indexed_views[view_id].referenced_containers()
+        directly_referenced_containers = view_by_id[view_id].referenced_containers()
         inherited_referenced_containers = set()
 
         for view_id in view_inheritance:
-            if implemented_view := indexed_views.get(view_id):
+            if implemented_view := view_by_id.get(view_id):
                 inherited_referenced_containers |= implemented_view.referenced_containers()
             else:
                 raise IncompleteSchemaError(missing_component=view_id).as_exception()
 
         return directly_referenced_containers | inherited_referenced_containers
 
     @classmethod
@@ -147,47 +152,55 @@
         parents = view_loader.retrieve_all_parents(list(parent_view_ids - existing_view_ids))
         views.extend([parent for parent in parents if parent.as_id() not in existing_view_ids])
 
         # Converting views from read to write format requires to account for parents (implements)
         # as the read format contains all properties from all parents, while the write formate should not contain
         # properties from any parents.
         # The ViewLoader as_write method looks up parents and remove properties from them.
-        view_write = dm.ViewApplyList([view_loader.as_write(view) for view in views])
+        view_write = ViewApplyDict([view_loader.as_write(view) for view in views])
 
-        container_write = containers.as_write()
+        container_write = ContainerApplyDict(containers.as_write())
         user_space = data_model.space
         if reference_model:
             user_model_view_ids = set(data_model_write.views)
             ref_model_write = reference_model.as_write()
             ref_model_write.views = [view.as_id() for view in reference_model.views]
 
-            ref_views = dm.ViewApplyList(
-                [view for view in view_write if (view.space != user_space) or (view.as_id() not in user_model_view_ids)]
+            ref_views = ViewApplyDict(
+                [
+                    view
+                    for view_id, view in view_write.items()
+                    if (view.space != user_space) or (view_id not in user_model_view_ids)
+                ]
             )
-            view_write = dm.ViewApplyList(
-                [view for view in view_write if view.space == user_space or view.as_id() in user_model_view_ids]
+            view_write = ViewApplyDict(
+                [
+                    view
+                    for view_id, view in view_write.items()
+                    if view.space == user_space or view_id in user_model_view_ids
+                ]
             )
 
-            ref_containers = dm.ContainerApplyList(
-                [container for container in container_write if container.space != user_space]
+            ref_containers = ContainerApplyDict(
+                [container for container in container_write.values() if container.space != user_space]
             )
-            container_write = dm.ContainerApplyList(
-                [container for container in container_write if container.space == user_space]
+            container_write = ContainerApplyDict(
+                [container for container in container_write.values() if container.space == user_space]
             )
 
             ref_schema: DMSSchema | None = cls(
-                spaces=dm.SpaceApplyList([s for s in space_write if s.space != user_space]),
+                spaces=SpaceApplyDict([s for s in space_write if s.space != user_space]),
                 data_model=ref_model_write,
                 views=ref_views,
                 containers=ref_containers,
             )
         else:
             ref_schema = None
         return cls(
-            spaces=dm.SpaceApplyList([s for s in space_write if s.space == user_space]),
+            spaces=SpaceApplyDict([s for s in space_write if s.space == user_space]),
             data_model=data_model_write,
             views=view_write,
             containers=container_write,
             reference=ref_schema,
         )
 
     @classmethod
@@ -241,40 +254,40 @@
             encoding (str): The encoding to use in the output files. Defaults to "utf-8".
         """
         path_dir = Path(directory)
         exclude_set = exclude or set()
         data_models = path_dir / "data_models"
         data_models.mkdir(parents=True, exist_ok=True)
         if "spaces" not in exclude_set:
-            for space in self.spaces:
+            for space in self.spaces.values():
                 (data_models / f"{space.space}.space.yaml").write_text(
                     space.dump_yaml(), newline=new_line, encoding=encoding
                 )
         if "data_models" not in exclude_set and self.data_model:
             (data_models / f"{self.data_model.external_id}.datamodel.yaml").write_text(
                 self.data_model.dump_yaml(), newline=new_line, encoding=encoding
             )
         if "views" not in exclude_set and self.views:
             view_dir = data_models / "views"
             view_dir.mkdir(parents=True, exist_ok=True)
-            for view in self.views:
+            for view in self.views.values():
                 (view_dir / f"{view.external_id}.view.yaml").write_text(
                     view.dump_yaml(), newline=new_line, encoding=encoding
                 )
         if "containers" not in exclude_set and self.containers:
             container_dir = data_models / "containers"
             container_dir.mkdir(parents=True, exist_ok=True)
-            for container in self.containers:
+            for container in self.containers.values():
                 (container_dir / f"{container.external_id}.container.yaml").write_text(
                     container.dump_yaml(), newline=new_line, encoding=encoding
                 )
         if "node_types" not in exclude_set and self.node_types:
             node_dir = data_models / "nodes"
             node_dir.mkdir(parents=True, exist_ok=True)
-            for node in self.node_types:
+            for node in self.node_types.values():
                 (node_dir / f"{node.external_id}.node.yaml").write_text(
                     node.dump_yaml(), newline=new_line, encoding=encoding
                 )
 
     @classmethod
     def from_zip(cls, zip_file: str | Path) -> Self:
         """Load a schema from a ZIP file containing YAML files.
@@ -320,30 +333,30 @@
         Args:
             zip_file (str | Path): The ZIP file to save the schema to.
             exclude (set[str]): A set of attributes to exclude from the output.
         """
         exclude_set = exclude or set()
         with zipfile.ZipFile(zip_file, "w") as zip_ref:
             if "spaces" not in exclude_set:
-                for space in self.spaces:
+                for space in self.spaces.values():
                     zip_ref.writestr(f"data_models/{space.space}.space.yaml", space.dump_yaml())
             if "data_models" not in exclude_set and self.data_model:
                 zip_ref.writestr(
                     f"data_models/{self.data_model.external_id}.datamodel.yaml", self.data_model.dump_yaml()
                 )
             if "views" not in exclude_set:
-                for view in self.views:
+                for view in self.views.values():
                     zip_ref.writestr(f"data_models/views/{view.external_id}.view.yaml", view.dump_yaml())
             if "containers" not in exclude_set:
-                for container in self.containers:
+                for container in self.containers.values():
                     zip_ref.writestr(
                         f"data_models/containers{container.external_id}.container.yaml", container.dump_yaml()
                     )
             if "node_types" not in exclude_set:
-                for node in self.node_types:
+                for node in self.node_types.values():
                     zip_ref.writestr(f"data_models/nodes/{node.external_id}.node.yaml", node.dump_yaml())
 
     @classmethod
     def load(cls, data: str | dict[str, list[Any]], context: dict[str, list[Path]] | None = None) -> Self:
         """Loads a schema from a dictionary or a YAML or JSON formatted string.
 
         Args:
@@ -432,17 +445,21 @@
             dict: The schema as a dictionary.
         """
         output: dict[str, Any] = {}
         cls_fields = sorted(fields(self), key=lambda f: f.name) if sort else fields(self)
         for attr in cls_fields:
             if items := getattr(self, attr.name):
                 key = to_camel(attr.name) if camel_case else attr.name
-                if isinstance(items, Sequence):
-                    items = sorted(items, key=self._to_sortable_identifier) if sort else items
-                    output[key] = [item.dump(camel_case=camel_case) for item in items]
+                if isinstance(items, CogniteResourceDict):
+                    if sort:
+                        output[key] = [
+                            item.dump(camel_case) for item in sorted(items.values(), key=self._to_sortable_identifier)
+                        ]
+                    else:
+                        output[key] = items.dump(camel_case)
                 else:
                     output[key] = items.dump(camel_case=camel_case)
         return output
 
     @classmethod
     def _to_sortable_identifier(cls, item: Any) -> str | tuple[str, str] | tuple[str, str, str]:
         if isinstance(item, dm.ContainerApply | dm.ViewApply | dm.DataModelApply | dm.NodeApply | RawTableWrite):
@@ -457,27 +474,27 @@
         elif isinstance(item, DatabaseWrite):
             return item.name or ""
         else:
             raise ValueError(f"Cannot sort item of type {type(item)}")
 
     def validate(self) -> list[DMSSchemaError]:
         errors: set[DMSSchemaError] = set()
-        defined_spaces = {space.space for space in self.spaces}
-        defined_containers = {container.as_id(): container for container in self.containers}
-        defined_views = {view.as_id() for view in self.views}
+        defined_spaces = self.spaces.copy()
+        defined_containers = self.containers.copy()
+        defined_views = self.views.copy()
         if self.reference:
-            defined_spaces |= {space.space for space in self.reference.spaces}
-            defined_containers |= {container.as_id(): container for container in self.reference.containers}
-            defined_views |= {view.as_id() for view in self.reference.views}
+            defined_spaces |= self.reference.spaces
+            defined_containers |= self.reference.containers
+            defined_views |= self.reference.views
 
-        for container in self.containers:
+        for container in self.containers.values():
             if container.space not in defined_spaces:
                 errors.add(MissingSpaceError(space=container.space, referred_by=container.as_id()))
 
-        for view in self.views:
+        for view in self.views.values():
             view_id = view.as_id()
             if view.space not in defined_spaces:
                 errors.add(MissingSpaceError(space=view.space, referred_by=view_id))
 
             for parent in view.implements or []:
                 if parent not in defined_views:
                     errors.add(MissingParentViewError(view=parent, referred_by=view_id))
@@ -597,24 +614,26 @@
 
         Args:
             include_indirect_references (bool): If True, the spaces referenced by as view.implements, and
                 view.referenced_containers will be included in the output.
         Returns:
             set[str]: The spaces referenced by the schema.
         """
-        referenced_spaces = {view.space for view in self.views}
-        referenced_spaces |= {container.space for container in self.containers}
+        referenced_spaces = {view.space for view in self.views.values()}
+        referenced_spaces |= {container.space for container in self.containers.values()}
         if include_indirect_references:
-            referenced_spaces |= {container.space for view in self.views for container in view.referenced_containers()}
-            referenced_spaces |= {parent.space for view in self.views for parent in view.implements or []}
-        referenced_spaces |= {node.space for node in self.node_types}
+            referenced_spaces |= {
+                container.space for view in self.views.values() for container in view.referenced_containers()
+            }
+            referenced_spaces |= {parent.space for view in self.views.values() for parent in view.implements or []}
+        referenced_spaces |= {node.space for node in self.node_types.values()}
         if self.data_model:
             referenced_spaces |= {self.data_model.space}
             referenced_spaces |= {view.space for view in self.data_model.views or []}
-        referenced_spaces |= {s.space for s in self.spaces}
+        referenced_spaces |= {s.space for s in self.spaces.values()}
         return referenced_spaces
 
 
 @dataclass
 class PipelineSchema(DMSSchema):
     transformations: TransformationWriteList = field(default_factory=lambda: TransformationWriteList([]))
     databases: DatabaseWriteList = field(default_factory=lambda: DatabaseWriteList([]))
@@ -723,20 +742,20 @@
         if not schema.data_model:
             raise ValueError("PipelineSchema must contain at least one data model")
         first_data_model = schema.data_model
         # The database name is limited to 32 characters
         database_name = first_data_model.external_id[:32]
         instance_space = instance_space or first_data_model.space
         database = DatabaseWrite(name=database_name)
-        parent_views = {parent for view in schema.views for parent in view.implements or []}
-        container_by_id = {container.as_id(): container for container in schema.containers}
+        parent_views = {parent for view in schema.views.values() for parent in view.implements or []}
+        container_by_id = schema.containers.copy()
 
         transformations = TransformationWriteList([])
         raw_tables = RawTableWriteList([])
-        for view in schema.views:
+        for view in schema.views.values():
             if view.as_id() in parent_views:
                 # Skipping parents as they do not have their own data
                 continue
             mapped_properties = {
                 prop_name: prop
                 for prop_name, prop in (view.properties or {}).items()
                 if isinstance(prop, dm.MappedPropertyApply)
```

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_serializer.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_validation.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,16 +162,16 @@
             return None
         if self.metadata.extension is ExtensionCategory.rebuild:
             # Everything is allowed
             return None
         # Is an extension of an existing model.
         user_schema = self.rules.as_schema()
         ref_schema = self.rules.reference.as_schema()
-        new_containers = {container.as_id(): container for container in user_schema.containers}
-        existing_containers = {container.as_id(): container for container in ref_schema.containers}
+        new_containers = user_schema.containers.copy()
+        existing_containers = ref_schema.containers.copy()
 
         for container_id, container in new_containers.items():
             existing_container = existing_containers.get(container_id)
             if not existing_container or existing_container == container:
                 # No problem
                 continue
             new_dumped = container.dump()
@@ -189,16 +189,16 @@
 
         if self.metadata.extension is ExtensionCategory.reshape and self.issue_list:
             return None
         elif self.metadata.extension is ExtensionCategory.reshape:
             # Reshape allows changes to views
             return None
 
-        new_views = {view.as_id(): view for view in user_schema.views}
-        existing_views = {view.as_id(): view for view in ref_schema.views}
+        new_views = user_schema.views.copy()
+        existing_views = ref_schema.views.copy()
         for view_id, view in new_views.items():
             existing_view = existing_views.get(view_id)
             if not existing_view or existing_view == view:
                 # No problem
                 continue
             changed_attributes, changed_properties = self._changed_attributes_and_properties(
                 view.dump(), existing_view.dump()
@@ -215,32 +215,32 @@
         # we can only validate performance on complete schemas due to the need
         # to access all the container mappings
         if self.metadata.schema_ is not SchemaCompleteness.complete:
             return None
 
         dms_schema = self.rules.as_schema()
 
-        for view in dms_schema.views:
-            mapped_containers = dms_schema._get_mapped_container_from_view(view.as_id())
+        for view_id, view in dms_schema.views.items():
+            mapped_containers = dms_schema._get_mapped_container_from_view(view_id)
 
             if mapped_containers and len(mapped_containers) > 10:
                 self.issue_list.append(
                     issues.dms.ViewMapsToTooManyContainersWarning(
-                        view_id=view.as_id(),
+                        view_id=view_id,
                         container_ids=mapped_containers,
                     )
                 )
                 if (
                     view.filter
                     and isinstance(view.filter, dm.filters.HasData)
                     and len(view.filter.dump()["hasData"]) > 10
                 ):
                     self.issue_list.append(
                         issues.dms.HasDataFilterAppliedToTooManyContainersWarning(
-                            view_id=view.as_id(),
+                            view_id=view_id,
                             container_ids=mapped_containers,
                         )
                     )
 
     @staticmethod
     def _changed_attributes_and_properties(
         new_dumped: dict[str, Any], existing_dumped: dict[str, Any]
```

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/domain.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/domain.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/entities.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/entities.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/information/_converter.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/information/_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/information/_rules.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/information/_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/rules/models/wrapped_entities.py` & `cognite_neat-0.77.1/cognite/neat/rules/models/wrapped_entities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+import re
 from abc import ABC, abstractmethod
 from collections.abc import Collection
 from functools import total_ordering
 from typing import Any, ClassVar, TypeVar
 
 from cognite.client import data_modeling as dm
 from cognite.client.data_classes.data_modeling import ContainerId, NodeId
@@ -33,16 +35,27 @@
         result = cls._parse(data)
         return result
 
     @classmethod
     def _parse(cls, data: str) -> dict:
         if data.casefold() == cls.name.casefold():
             return {"inner": None}
-        inner = data[len(cls.name) :].removeprefix("(").removesuffix(")")
-        return {"inner": [cls._inner_cls.load(entry.strip()) for entry in inner.split(",")]}
+
+        # raw filter case:
+        if cls.__name__ == "RawFilter":
+            if match := re.search(r"rawFilter\(([\s\S]*?)\)", data):
+                return {"filter": match.group(1), "inner": None}
+            else:
+                raise ValueError(f"Cannot parse {cls.name} from {data}. Ill formatted raw filter.")
+
+        # nodeType and hasData case:
+        elif inner := data[len(cls.name) :].removeprefix("(").removesuffix(")"):
+            return {"inner": [cls._inner_cls.load(entry.strip()) for entry in inner.split(",")]}
+        else:
+            raise ValueError(f"Cannot parse {cls.name} from {data}")
 
     @model_serializer(when_used="unless-none", return_type=str)
     def as_str(self) -> str:
         return str(self)
 
     def __str__(self):
         return self.id
@@ -160,7 +173,26 @@
         else:
             raise ValueError("Empty hasData filter, please provide a default containers.")
 
         return dm.filters.HasData(
             # Sorting to ensure deterministic order
             containers=sorted(containers, key=lambda container: container.as_tuple())  # type: ignore[union-attr]
         )
+
+
+class RawFilter(DMSFilter):
+    name: ClassVar[str] = "rawFilter"
+    filter: str
+    inner: None = None  # type: ignore[assignment]
+
+    def as_dms_filter(self) -> dm.Filter:  # type: ignore[override]
+        try:
+            return dm.Filter.load(json.loads(self.filter))
+        except json.JSONDecodeError as e:
+            raise ValueError(f"Error loading raw filter: {e}") from e
+
+    @property
+    def is_empty(self) -> bool:
+        return self.filter is None
+
+    def __repr__(self) -> str:
+        return self.filter
```

### Comparing `cognite_neat-0.77.0/cognite/neat/utils/cdf.py` & `cognite_neat-0.77.1/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/utils/exceptions.py` & `cognite_neat-0.77.1/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.77.1/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/utils/text.py` & `cognite_neat-0.77.1/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/utils/utils.py` & `cognite_neat-0.77.1/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/utils/xml.py` & `cognite_neat-0.77.1/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.77.1/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/base.py` & `cognite_neat-0.77.1/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.77.1/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.77.1/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/manager.py` & `cognite_neat-0.77.1/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.77.1/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.77.1/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/model.py` & `cognite_neat-0.77.1/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_extractor.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_loader.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_store.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_exporter.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_importer.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_validator.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,17 +74,17 @@
             view_loader.as_write(view) for view in cdf_client.data_modeling.views.retrieve(missing_views)
         ]
         logging.info(
             f"Retrieved {len(retrieved_spaces)} spaces, {len(retrieved_containers)} containers, "
             f"and {len(retrieved_views)} views from CDF."
         )
 
-        schema.spaces.extend(retrieved_spaces)
-        schema.containers.extend(retrieved_containers)
-        schema.views.extend(retrieved_views)
+        schema.spaces.update({space.space: space for space in retrieved_spaces})
+        schema.containers.update({container.as_id(): container for container in retrieved_containers})
+        schema.views.update({view.as_id(): view for view in retrieved_views})
 
         errors = schema.validate()
         if errors:
             output_dir = self.data_store_path / Path("staging")
             report_writer = FORMATTER_BY_NAME[self.configs["Report Formatter"]]()
             report_writer.write_to_file(
                 IssueList(errors, title=dms_rules.metadata.name or dms_rules.metadata.external_id),
```

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/io/io_steps.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/io/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_loader.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_store.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/rules_importer.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.77.1/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/tasks.py` & `cognite_neat-0.77.1/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/cognite/neat/workflows/triggers.py` & `cognite_neat-0.77.1/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.0/pyproject.toml` & `cognite_neat-0.77.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.77.0"
+version = "0.77.1"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.77.0/PKG-INFO` & `cognite_neat-0.77.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.77.0
+Version: 0.77.1
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

