# Comparing `tmp/cognite_neat-0.73.2.tar.gz` & `tmp/cognite_neat-0.73.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.73.2.tar", max compression
+gzip compressed data, was "cognite_neat-0.73.3.tar", max compression
```

## Comparing `cognite_neat-0.73.2.tar` & `cognite_neat-0.73.3.tar`

### file list

```diff
@@ -1,233 +1,233 @@
--rw-r--r--   0        0        0    11351 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/LICENSE
--rw-r--r--   0        0        0     6775 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/README.md
--rw-r--r--   0        0        0       61 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4606 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     4208 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/data_classes/configuration.py
--rw-r--r--   0        0        0     1675 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      554 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3583 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4646 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13653 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     6369 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12402 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      629 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-04-19 09:03:04.701977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-04-19 09:03:04.705977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-04-19 09:03:04.705977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1403545 2024-04-19 09:03:04.709977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js
--rw-r--r--   0        0        0     2667 2024-04-19 09:03:04.709977 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt
--rw-r--r--   0        0        0  6234629 2024-04-19 09:03:04.733978 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map
--rw-r--r--   0        0        0   240334 2024-04-19 09:03:04.737978 cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     1503 2024-04-19 09:03:04.741978 cognite_neat-0.73.2/cognite/neat/config.py
--rw-r--r--   0        0        0     1205 2024-04-19 09:03:04.741978 cognite_neat-0.73.2/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-04-19 09:03:04.741978 cognite_neat-0.73.2/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-04-19 09:03:04.741978 cognite_neat-0.73.2/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-19 09:03:04.745978 cognite_neat-0.73.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/extractor/__init__.py
--rw-r--r--   0        0        0      356 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/extractor/_base.py
--rw-r--r--   0        0        0    11720 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/extractor/_dexpi.py
--rw-r--r--   0        0        0    17652 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/extractor/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14872 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/extractor/_mock_graph_generator.py
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14969 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      693 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/loader/__init__.py
--rw-r--r--   0        0        0    23838 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/loader/_asset_loader.py
--rw-r--r--   0        0        0     2370 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/loader/_base.py
--rw-r--r--   0        0        0     2837 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/loader/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/loader/core/__init__.py
--rw-r--r--   0        0        0     2306 2024-04-19 09:03:04.749978 cognite_neat-0.73.2/cognite/neat/graph/loader/core/labels.py
--rw-r--r--   0        0        0     5016 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/loader/core/models.py
--rw-r--r--   0        0        0    40458 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/loader/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22678 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/loader/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12957 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/loader/rdf_to_dms.py
--rw-r--r--   0        0        0     3327 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/loader/validator.py
--rw-r--r--   0        0        0      149 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    14254 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/transformation/__init__.py
--rw-r--r--   0        0        0     4758 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/transformation/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/transformation/query_generator/__init__.py
--rw-r--r--   0        0        0    18659 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/transformation/query_generator/sparql.py
--rw-r--r--   0        0        0    14673 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/graph/transformation/transformer.py
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/_analysis/__init__.py
--rw-r--r--   0        0        0      674 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/_analysis/_base.py
--rw-r--r--   0        0        0    19613 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/_analysis/_information_rules.py
--rw-r--r--   0        0        0      177 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0     8596 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/exporter/__init__.py
--rw-r--r--   0        0        0     1439 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/exporter/_base.py
--rw-r--r--   0        0        0      102 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/exporter/_core/__init__.py
--rw-r--r--   0        0        0      764 2024-04-19 09:03:04.753978 cognite_neat-0.73.2/cognite/neat/rules/exporter/_core/rules2labels.py
--rw-r--r--   0        0        0    36770 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2dms.py
--rw-r--r--   0        0        0     8305 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2excel.py
--rw-r--r--   0        0        0     6215 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2graphql.py
--rw-r--r--   0        0        0    18414 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2ontology.py
--rw-r--r--   0        0        0    28745 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3866 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2rules.py
--rw-r--r--   0        0        0     1104 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2triples.py
--rw-r--r--   0        0        0     5769 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporter/_validation.py
--rw-r--r--   0        0        0      413 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1518 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1645 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    11854 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    13146 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    19922 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3038 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4092 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/__init__.py
--rw-r--r--   0        0        0     2316 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_base.py
--rw-r--r--   0        0        0     6469 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_dict2rules.py
--rw-r--r--   0        0        0     7713 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_dms2rules.py
--rw-r--r--   0        0        0    12097 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_json2rules.py
--rw-r--r--   0        0        0       63 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9320 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10521 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1529 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_spreadsheet2rules.py
--rw-r--r--   0        0        0      448 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_xsd2rules.py
--rw-r--r--   0        0        0     1628 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importer/_yaml2rules.py
--rw-r--r--   0        0        0      408 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4268 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    10427 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12554 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6925 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11926 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7597 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7791 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7443 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     7120 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11481 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4198 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6158 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    15314 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3346 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     7493 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      127 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0      517 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/models/_rules/__init__.py
--rw-r--r--   0        0        0     1299 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/models/_rules/_types/__init__.py
--rw-r--r--   0        0        0    16681 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/models/_rules/_types/_base.py
--rw-r--r--   0        0        0    10295 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/models/_rules/_types/_field.py
--rw-r--r--   0        0        0     6308 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/models/_rules/_types/_value.py
--rw-r--r--   0        0        0    11025 2024-04-19 09:03:04.757978 cognite_neat-0.73.2/cognite/neat/rules/models/_rules/base.py
--rw-r--r--   0        0        0    55886 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/rules/models/_rules/dms_architect_rules.py
--rw-r--r--   0        0        0    30418 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/rules/models/_rules/dms_schema.py
--rw-r--r--   0        0        0     2566 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/rules/models/_rules/domain_rules.py
--rw-r--r--   0        0        0    21555 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/rules/models/_rules/information_rules.py
--rw-r--r--   0        0        0    12368 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7344 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51063 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/rules/models/tables.py
--rw-r--r--   0        0        0     4395 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/rules/models/value_types.py
--rw-r--r--   0        0        0       68 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11063 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6319 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2722 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12826 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26857 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/examples/Export DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/examples/Import DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
--rw-r--r--   0        0        0    13659 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6568 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     2994 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0      257 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0     5161 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/graph_loader.py
--rw-r--r--   0        0        0     6288 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/graph_store.py
--rw-r--r--   0        0        0    16874 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/io_steps.py
--rw-r--r--   0        0        0    18234 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/rules_exporter.py
--rw-r--r--   0        0        0     7327 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/rules_importer.py
--rw-r--r--   0        0        0     4785 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/rules_validator.py
--rw-r--r--   0        0        0      274 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/__init__.py
--rw-r--r--   0        0        0     3921 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
--rw-r--r--   0        0        0    29390 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
--rw-r--r--   0        0        0    27269 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/graph_loader.py
--rw-r--r--   0        0        0    12522 2024-04-19 09:03:04.761978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/graph_store.py
--rw-r--r--   0        0        0     2345 2024-04-19 09:03:04.765978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
--rw-r--r--   0        0        0    20657 2024-04-19 09:03:04.765978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
--rw-r--r--   0        0        0    28072 2024-04-19 09:03:04.765978 cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/rules_importer.py
--rw-r--r--   0        0        0     3010 2024-04-19 09:03:04.765978 cognite_neat-0.73.2/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    10467 2024-04-19 09:03:04.765978 cognite_neat-0.73.2/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-04-19 09:03:04.765978 cognite_neat-0.73.2/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-04-19 09:03:04.765978 cognite_neat-0.73.2/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-04-19 09:03:04.765978 cognite_neat-0.73.2/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4543 2024-04-19 09:03:05.149982 cognite_neat-0.73.2/pyproject.toml
--rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.73.2/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/LICENSE
+-rw-r--r--   0        0        0     6775 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/README.md
+-rw-r--r--   0        0        0       61 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4606 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     4208 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1675 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      554 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3583 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4646 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13653 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-04-19 09:28:53.110716 cognite_neat-0.73.3/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     6369 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12402 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      629 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-04-19 09:28:53.114716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1403545 2024-04-19 09:28:53.122716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js
+-rw-r--r--   0        0        0     2667 2024-04-19 09:28:53.122716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt
+-rw-r--r--   0        0        0  6234629 2024-04-19 09:28:53.146716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map
+-rw-r--r--   0        0        0   240334 2024-04-19 09:28:53.146716 cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     1503 2024-04-19 09:28:53.154716 cognite_neat-0.73.3/cognite/neat/config.py
+-rw-r--r--   0        0        0     1205 2024-04-19 09:28:53.154716 cognite_neat-0.73.3/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-04-19 09:28:53.154716 cognite_neat-0.73.3/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-04-19 09:28:53.154716 cognite_neat-0.73.3/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-19 09:28:53.158716 cognite_neat-0.73.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/extractor/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/extractor/_base.py
+-rw-r--r--   0        0        0    11720 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/extractor/_dexpi.py
+-rw-r--r--   0        0        0    17652 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/extractor/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14872 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/extractor/_mock_graph_generator.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14969 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      693 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/loader/__init__.py
+-rw-r--r--   0        0        0    23838 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/loader/_asset_loader.py
+-rw-r--r--   0        0        0     2370 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/loader/_base.py
+-rw-r--r--   0        0        0     2837 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/loader/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/loader/core/__init__.py
+-rw-r--r--   0        0        0     2306 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/loader/core/labels.py
+-rw-r--r--   0        0        0     5016 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/loader/core/models.py
+-rw-r--r--   0        0        0    40458 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/loader/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22678 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/loader/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12957 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/loader/rdf_to_dms.py
+-rw-r--r--   0        0        0     3327 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/loader/validator.py
+-rw-r--r--   0        0        0      149 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14254 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/transformation/__init__.py
+-rw-r--r--   0        0        0     4758 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/transformation/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/transformation/query_generator/__init__.py
+-rw-r--r--   0        0        0    18659 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/transformation/query_generator/sparql.py
+-rw-r--r--   0        0        0    14673 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/graph/transformation/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/_analysis/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/_analysis/_base.py
+-rw-r--r--   0        0        0    19613 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/_analysis/_information_rules.py
+-rw-r--r--   0        0        0      177 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0     8596 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-04-19 09:28:53.162716 cognite_neat-0.73.3/cognite/neat/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/__init__.py
+-rw-r--r--   0        0        0     1439 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/_base.py
+-rw-r--r--   0        0        0      102 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/_core/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/_core/rules2labels.py
+-rw-r--r--   0        0        0    36770 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2dms.py
+-rw-r--r--   0        0        0     8305 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2excel.py
+-rw-r--r--   0        0        0     6215 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2graphql.py
+-rw-r--r--   0        0        0    18414 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2ontology.py
+-rw-r--r--   0        0        0    28745 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3866 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2rules.py
+-rw-r--r--   0        0        0     1104 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2triples.py
+-rw-r--r--   0        0        0     5769 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporter/_validation.py
+-rw-r--r--   0        0        0      413 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1518 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1645 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    11854 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    13146 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    19922 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3038 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4092 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/__init__.py
+-rw-r--r--   0        0        0     2316 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_base.py
+-rw-r--r--   0        0        0     6469 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_dict2rules.py
+-rw-r--r--   0        0        0     7713 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_dms2rules.py
+-rw-r--r--   0        0        0    12097 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9320 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10521 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1529 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      448 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_xsd2rules.py
+-rw-r--r--   0        0        0     1628 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importer/_yaml2rules.py
+-rw-r--r--   0        0        0      408 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4268 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    10427 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12554 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6925 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11926 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7597 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7791 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7443 2024-04-19 09:28:53.166716 cognite_neat-0.73.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     7120 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11481 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4198 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6158 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    15314 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     4492 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3346 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0     7493 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13763 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      127 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0      517 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/_rules/__init__.py
+-rw-r--r--   0        0        0     1299 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/_rules/_types/__init__.py
+-rw-r--r--   0        0        0    16681 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/_rules/_types/_base.py
+-rw-r--r--   0        0        0    10295 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/_rules/_types/_field.py
+-rw-r--r--   0        0        0     6308 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/_rules/_types/_value.py
+-rw-r--r--   0        0        0    11025 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/_rules/base.py
+-rw-r--r--   0        0        0    55886 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/_rules/dms_architect_rules.py
+-rw-r--r--   0        0        0    30418 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/_rules/dms_schema.py
+-rw-r--r--   0        0        0     2566 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/_rules/domain_rules.py
+-rw-r--r--   0        0        0    21555 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/_rules/information_rules.py
+-rw-r--r--   0        0        0    12368 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7344 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51063 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/tables.py
+-rw-r--r--   0        0        0     4395 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/rules/models/value_types.py
+-rw-r--r--   0        0        0       68 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11063 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6319 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2722 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12826 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26857 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/examples/Export DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/examples/Import DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
+-rw-r--r--   0        0        0    13659 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.170716 cognite_neat-0.73.3/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6568 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     2994 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0      257 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0     5161 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/graph_loader.py
+-rw-r--r--   0        0        0     6288 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/graph_store.py
+-rw-r--r--   0        0        0    16874 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/io_steps.py
+-rw-r--r--   0        0        0    18234 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/rules_exporter.py
+-rw-r--r--   0        0        0     7327 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/rules_importer.py
+-rw-r--r--   0        0        0     4785 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/rules_validator.py
+-rw-r--r--   0        0        0      274 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/__init__.py
+-rw-r--r--   0        0        0     3921 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
+-rw-r--r--   0        0        0    29390 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
+-rw-r--r--   0        0        0    27269 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/graph_loader.py
+-rw-r--r--   0        0        0    12522 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/graph_store.py
+-rw-r--r--   0        0        0     2345 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
+-rw-r--r--   0        0        0    20657 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
+-rw-r--r--   0        0        0    28072 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/rules_importer.py
+-rw-r--r--   0        0        0     3010 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    10467 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-04-19 09:28:53.174716 cognite_neat-0.73.3/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4543 2024-04-19 09:28:53.558716 cognite_neat-0.73.3/pyproject.toml
+-rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.73.3/PKG-INFO
```

### Comparing `cognite_neat-0.73.2/LICENSE` & `cognite_neat-0.73.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/README.md` & `cognite_neat-0.73.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/configuration.py` & `cognite_neat-0.73.3/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/data_classes/configuration.py` & `cognite_neat-0.73.3/cognite/neat/app/api/data_classes/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.73.3/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/explorer.py` & `cognite_neat-0.73.3/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.73.3/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.73.3/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.73.3/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.73.3/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.73.3/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.73.3/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.73.3/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.73.3/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.73.3/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.73.3/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js` & `cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt` & `cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map` & `cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.73.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/config.py` & `cognite_neat-0.73.3/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/constants.py` & `cognite_neat-0.73.3/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/exceptions.py` & `cognite_neat-0.73.3/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.73.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.73.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.73.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/exceptions.py` & `cognite_neat-0.73.3/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/extractor/_dexpi.py` & `cognite_neat-0.73.3/cognite/neat/graph/extractor/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/extractor/_graph_capturing_sheet.py` & `cognite_neat-0.73.3/cognite/neat/graph/extractor/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/extractor/_mock_graph_generator.py` & `cognite_neat-0.73.3/cognite/neat/graph/extractor/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.73.3/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/loader/__init__.py` & `cognite_neat-0.73.3/cognite/neat/graph/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/loader/_asset_loader.py` & `cognite_neat-0.73.3/cognite/neat/graph/loader/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/loader/_base.py` & `cognite_neat-0.73.3/cognite/neat/graph/loader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/loader/_exceptions.py` & `cognite_neat-0.73.3/cognite/neat/graph/loader/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/loader/core/labels.py` & `cognite_neat-0.73.3/cognite/neat/graph/loader/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/loader/core/models.py` & `cognite_neat-0.73.3/cognite/neat/graph/loader/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/loader/core/rdf_to_assets.py` & `cognite_neat-0.73.3/cognite/neat/graph/loader/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/loader/core/rdf_to_relationships.py` & `cognite_neat-0.73.3/cognite/neat/graph/loader/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/loader/rdf_to_dms.py` & `cognite_neat-0.73.3/cognite/neat/graph/loader/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/loader/validator.py` & `cognite_neat-0.73.3/cognite/neat/graph/loader/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.73.3/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.73.3/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.73.3/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.73.3/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.73.3/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.73.3/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.73.3/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/transformation/entity_matcher.py` & `cognite_neat-0.73.3/cognite/neat/graph/transformation/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/transformation/query_generator/sparql.py` & `cognite_neat-0.73.3/cognite/neat/graph/transformation/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/graph/transformation/transformer.py` & `cognite_neat-0.73.3/cognite/neat/graph/transformation/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/_analysis/_base.py` & `cognite_neat-0.73.3/cognite/neat/rules/_analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/_analysis/_information_rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/_analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/analysis.py` & `cognite_neat-0.73.3/cognite/neat/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.73.3/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.73.3/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/examples/__init__.py` & `cognite_neat-0.73.3/cognite/neat/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.73.3/cognite/neat/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.73.3/cognite/neat/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/examples/power-grid-model.yaml` & `cognite_neat-0.73.3/cognite/neat/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/examples/rules-template.xlsx` & `cognite_neat-0.73.3/cognite/neat/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.73.3/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/examples/skos-rules.xlsx` & `cognite_neat-0.73.3/cognite/neat/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.73.3/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.73.3/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exceptions.py` & `cognite_neat-0.73.3/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporter/__init__.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporter/_base.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporter/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporter/_core/rules2labels.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporter/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2dms.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2excel.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2graphql.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2ontology.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2pydantic_models.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporter/_rules2triples.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporter/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporter/_validation.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporter/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.73.3/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/__init__.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/_base.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/_dict2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/_dms2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/_graph2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/_json2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/_owl2rules/_owl2classes.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/_owl2rules/_owl2properties.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/_owl2rules/_owl2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/_spreadsheet2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importer/_yaml2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/importer/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.73.3/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/issues/base.py` & `cognite_neat-0.73.3/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.73.3/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.73.3/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.73.3/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.73.3/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.73.3/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.73.3/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/_base.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/_rules/__init__.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/_rules/_types/__init__.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/_rules/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/_rules/_types/_base.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/_rules/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/_rules/_types/_field.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/_rules/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/_rules/_types/_value.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/_rules/_types/_value.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/_rules/base.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/_rules/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/_rules/dms_architect_rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/_rules/dms_architect_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/_rules/dms_schema.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/_rules/dms_schema.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/_rules/domain_rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/_rules/domain_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/_rules/information_rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/_rules/information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/raw_rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/rdfpath.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/rules.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/rules/models/value_types.py` & `cognite_neat-0.73.3/cognite/neat/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/utils/cdf.py` & `cognite_neat-0.73.3/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.73.3/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.73.3/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.73.3/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.73.3/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/utils/exceptions.py` & `cognite_neat-0.73.3/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.73.3/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/utils/text.py` & `cognite_neat-0.73.3/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/utils/utils.py` & `cognite_neat-0.73.3/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/utils/xml.py` & `cognite_neat-0.73.3/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.73.3/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/base.py` & `cognite_neat-0.73.3/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.73.3/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/examples/Export DMS/workflow.yaml` & `cognite_neat-0.73.3/cognite/neat/workflows/examples/Export DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml` & `cognite_neat-0.73.3/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml` & `cognite_neat-0.73.3/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml` & `cognite_neat-0.73.3/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/examples/Import DMS/workflow.yaml` & `cognite_neat-0.73.3/cognite/neat/workflows/examples/Import DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml` & `cognite_neat-0.73.3/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/examples/Validate Rules/workflow.yaml` & `cognite_neat-0.73.3/cognite/neat/workflows/examples/Validate Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml` & `cognite_neat-0.73.3/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml` & `cognite_neat-0.73.3/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml` & `cognite_neat-0.73.3/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/manager.py` & `cognite_neat-0.73.3/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.73.3/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.73.3/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/model.py` & `cognite_neat-0.73.3/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/graph_extractor.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/graph_loader.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/graph_store.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/io_steps.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/rules_exporter.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/rules_importer.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/rules_validator.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/graph_extractor.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/graph_loader.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/graph_store.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/graph_transformer.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/rules_exporter.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/lib/v1/rules_importer.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/lib/v1/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.73.3/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/tasks.py` & `cognite_neat-0.73.3/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/cognite/neat/workflows/triggers.py` & `cognite_neat-0.73.3/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.73.2/pyproject.toml` & `cognite_neat-0.73.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.73.2"
+version = "0.73.3"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
@@ -64,19 +64,19 @@
 openpyxl = "*"
 # Backport from Python 3.11
 exceptiongroup = { version = "^1.1.3", python = "<3.11" }
 'backports.strenum' = { version = "^1.2", python = "<3.11" }
 typing_extensions = { version = "^4.8", python = "<3.11" }
 tomli = { version = "^2.0.1", python = "<3.11" }
 
-uvicorn = { extras = ["standard"], version = "^0.21.0" }
+uvicorn = { extras = ["standard"], version = "^0.29.0" }
 prometheus-client = "^0.20.0"
 cognite-sdk = "^7.37.0"
 deepdiff = "*"
-fastapi = "^0.100"
+fastapi = "^0.110"
 schedule = "^1"
 python-multipart = "^0.0.6"
 oxrdflib = { version = "^0.3.3", optional = true, extras = ["oxigraph"] }
 
 
 gspread = { version = "*", optional = true }
 google-api-python-client = { version = "*", optional = true }
```

### Comparing `cognite_neat-0.73.2/PKG-INFO` & `cognite_neat-0.73.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.73.2
+Version: 0.73.3
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,15 +18,15 @@
 Provides-Extra: graphql
 Provides-Extra: oxi
 Requires-Dist: PyYAML
 Requires-Dist: backports.strenum (>=1.2,<2.0) ; python_version < "3.11"
 Requires-Dist: cognite-sdk (>=7.37.0,<8.0.0)
 Requires-Dist: deepdiff
 Requires-Dist: exceptiongroup (>=1.1.3,<2.0.0) ; python_version < "3.11"
-Requires-Dist: fastapi (>=0.100,<0.101)
+Requires-Dist: fastapi (>=0.110,<0.111)
 Requires-Dist: google-api-python-client ; extra == "google" or extra == "all"
 Requires-Dist: google-auth-oauthlib ; extra == "google" or extra == "all"
 Requires-Dist: gspread ; extra == "google" or extra == "all"
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "graphql" or extra == "all"
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-autorefs (>=0.5.0,<0.6.0) ; extra == "docs"
 Requires-Dist: mkdocs-git-authors-plugin ; extra == "docs"
@@ -46,15 +46,15 @@
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: rdflib
 Requires-Dist: requests
 Requires-Dist: schedule (>=1,<2)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: typing_extensions (>=4.8,<5.0) ; python_version < "3.11"
 Requires-Dist: urllib3 (>=1.26,<2.0)
-Requires-Dist: uvicorn[standard] (>=0.21.0,<0.22.0)
+Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0)
 Project-URL: Documentation, https://cognite-neat.readthedocs-hosted.com/
 Project-URL: Repository, https://github.com/cognitedata/neat
 Description-Content-Type: text/markdown
 
 # kNowlEdge grAph Transformer (NEAT)
 
 [![release](https://img.shields.io/github/actions/workflow/status/cognitedata/neat/release_pypi.yaml?style=for-the-badge)](https://github.com/cognitedata/neat/actions/workflows/release_pypi.yaml)
```

