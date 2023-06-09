# Comparing `tmp/oaklib-0.5.8.tar.gz` & `tmp/oaklib-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.5.8.tar", max compression
+gzip compressed data, was "oaklib-0.5.9.tar", max compression
```

## Comparing `oaklib-0.5.8.tar` & `oaklib-0.5.9.tar`

### file list

```diff
@@ -1,274 +1,280 @@
--rw-r--r--   0        0        0    11357 2023-05-20 02:24:55.498869 oaklib-0.5.8/LICENSE
--rw-r--r--   0        0        0     7241 2023-05-20 02:24:55.498869 oaklib-0.5.8/README.md
--rw-r--r--   0        0        0     1880 2023-05-20 02:25:41.823500 oaklib-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      271 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/__init__.py
--rw-r--r--   0        0        0   194032 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      372 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/go-human-input-spec.yaml
--rw-r--r--   0        0        0      162 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/hpoa-g2p-input-spec.yaml
--rw-r--r--   0        0        0      106 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0      562 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/mondo-g2d-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/mondo-gencc-input-spec.yaml
--rw-r--r--   0        0        0      118 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
--rw-r--r--   0        0        0     4537 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      128 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2561 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2371 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12159 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     5713 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     5789 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    36266 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0    11740 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    13328 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     3192 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24246 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35744 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0    14564 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     3560 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15768 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     6339 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17256 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26434 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0   226115 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    32727 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    12889 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     3607 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    46876 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    18191 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   117175 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    30433 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3240 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25145 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6683 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12767 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22226 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5511 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0     9909 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18430 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5879 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    20418 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4219 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    25351 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     7510 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     5614 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     5849 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     5996 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/agrkb/__init__.py
--rw-r--r--   0        0        0     8126 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/agrkb/agrkb_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0     4601 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/amigo/amigo_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/eutils/__init__.py
--rw-r--r--   0        0        0     2179 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/eutils/eutils_implementation.py
--rw-r--r--   0        0        0     1053 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/eutils/pubmed_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     2313 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30434 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/monarch/__init__.py
--rw-r--r--   0        0        0     7009 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/monarch/monarch_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    16240 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     7942 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     2532 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0     1238 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    12106 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    35620 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/semsimian/__init__.py
--rw-r--r--   0        0        0      246 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/semsimian/profiler.py
--rw-r--r--   0        0        0     4110 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/semsimian/semsimian_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    34382 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    21451 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    36699 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2658 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2326 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   106362 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     3283 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    19393 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0     9603 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17121 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0      913 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0    20557 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    50981 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     8830 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    11720 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     2649 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0      977 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/embedding_provider_interface.py
--rw-r--r--   0        0        0    13681 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    18964 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      784 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    10988 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8236 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2459 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     3759 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    12778 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2112 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18296 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0     7566 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0     3033 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     2087 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1379 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     7906 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0     1231 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2088 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3496 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5129 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1318 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3717 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1849 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     2179 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0     1524 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4731 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     2208 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0     1090 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/gencc_association_parser.py
--rw-r--r--   0        0        0     1130 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0      602 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      653 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0     1666 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/mim2gene_association_parser.py
--rw-r--r--   0        0        0      525 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1432 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      707 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     8084 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/resource.py
--rw-r--r--   0        0        0    14702 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/selector.py
--rw-r--r--   0        0        0      177 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0    13441 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     3419 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0     1540 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2490 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2918 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     3345 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19516 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14467 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15328 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0     2270 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2694 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      684 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    22646 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0      379 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2819 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    11592 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    13212 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    10097 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1313 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0     8866 1970-01-01 00:00:00.000000 oaklib-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 14:38:11.671805 oaklib-0.5.9/LICENSE
+-rw-r--r--   0        0        0     7241 2023-06-01 14:38:11.671805 oaklib-0.5.9/README.md
+-rw-r--r--   0        0        0     1880 2023-06-01 14:38:54.392906 oaklib-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      271 2023-06-01 14:38:11.799809 oaklib-0.5.9/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   194196 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      372 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      162 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0      562 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      118 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4537 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      128 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1456 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2561 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2371 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12159 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     6805 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     5789 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    36266 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0    11740 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    13328 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24246 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35744 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    14564 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3560 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15768 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     6339 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17256 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26434 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    32727 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     3607 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    46876 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    18191 2023-06-01 14:38:11.803809 oaklib-0.5.9/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   117175 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    30433 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3344 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25145 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6683 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12767 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22226 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5511 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18430 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5879 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    20418 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4219 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25351 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     7510 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     5985 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     5966 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     6238 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/agrkb/__init__.py
+-rw-r--r--   0        0        0     8126 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/agrkb/agrkb_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0     4601 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/amigo/amigo_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/eutils/__init__.py
+-rw-r--r--   0        0        0     2179 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/eutils/eutils_implementation.py
+-rw-r--r--   0        0        0     1053 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/eutils/pubmed_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     2313 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30487 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.807809 oaklib-0.5.9/src/oaklib/implementations/monarch/__init__.py
+-rw-r--r--   0        0        0     7009 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/monarch/monarch_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    16757 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     7993 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     2641 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0     1238 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    13512 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    36358 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/semsimian/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/semsimian/profiler.py
+-rw-r--r--   0        0        0     4265 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/semsimian/semsimian_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    35951 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    21894 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    37448 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2326 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   107597 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     3283 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    19610 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0    10168 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17267 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/indexes/__init__.py
+-rw-r--r--   0        0        0     3088 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/indexes/edge_index.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/inference/__init__.py
+-rw-r--r--   0        0        0      748 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/inference/owl_reasoner.py
+-rw-r--r--   0        0        0       97 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/inference/reasoner.py
+-rw-r--r--   0        0        0     6959 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/inference/relation_graph_reasoner.py
+-rw-r--r--   0        0        0      913 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    20557 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    54282 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     8830 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    11720 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     2649 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0      788 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/embedding_provider_interface.py
+-rw-r--r--   0        0        0    13681 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    20131 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      784 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    13645 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8236 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2023-06-01 14:38:11.811809 oaklib-0.5.9/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2287 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     3759 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    13502 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2112 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18296 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0     8208 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0     3033 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     2087 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1379 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     7906 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0     1231 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2088 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3496 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5129 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1318 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3717 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1849 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2179 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0     1524 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4731 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     2208 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     1090 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0     1130 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0      602 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      653 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1666 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      525 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1432 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      707 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     8084 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/resource.py
+-rw-r--r--   0        0        0    14702 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/selector.py
+-rw-r--r--   0        0        0      177 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0    13441 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     3419 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0     1540 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2490 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2856 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     3345 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    20949 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14467 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15328 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0     2270 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2694 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      684 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    22907 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0      379 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     1739 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2819 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    11548 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    13212 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.815809 oaklib-0.5.9/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2023-06-01 14:38:11.819809 oaklib-0.5.9/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:38:11.819809 oaklib-0.5.9/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    10097 2023-06-01 14:38:11.819809 oaklib-0.5.9/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2023-06-01 14:38:11.819809 oaklib-0.5.9/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2023-06-01 14:38:11.819809 oaklib-0.5.9/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2023-06-01 14:38:11.819809 oaklib-0.5.9/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1313 2023-06-01 14:38:11.819809 oaklib-0.5.9/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0     8866 1970-01-01 00:00:00.000000 oaklib-0.5.9/PKG-INFO
```

### Comparing `oaklib-0.5.8/LICENSE` & `oaklib-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/README.md` & `oaklib-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/pyproject.toml` & `oaklib-0.5.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.5.8"
+version = "v0.5.9"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
@@ -33,15 +33,15 @@
 linkml-renderer = ">=0.1.2"
 airium = ">=0.2.5"
 ndex2 = "^3.5.0"
 pysolr = "^3.9.0"
 eutils = ">=0.6.0"
 requests-cache = "^1.0.1"
 click = "*"
-semsimian = "0.1.13"
+semsimian = "0.1.14"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 Sphinx = ">=6.1.3"
 pandas = ">=1.5.1"
 jupyter = ">=1.0.0"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `oaklib-0.5.8/src/oaklib/cli.py` & `oaklib-0.5.9/src/oaklib/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
 exclude_predicates_option = click.option(
     "--exclude-predicates", help="A comma-separated list of predicates to exclude"
 )
 graph_traversal_method_option = click.option(
     "-M",
     "--graph-traversal-method",
     type=click.Choice([v.value for v in GraphTraversalMethod]),
-    help="Desired output type",
+    help="Whether formal entailment or graph walking should be used.",
 )
 display_option = click.option(
     "-D",
     "--display",
     default="",
     help="A comma-separated list of display options. Use 'all' for all",
 )
@@ -707,14 +707,16 @@
             subset = query_terms[0]
             query_terms = query_terms[1:]
             chain_results(impl.subset_members(subset))
         elif term.startswith(".is_obsolete"):
             chain_results(impl.obsoletes())
         elif term.startswith(".non_obsolete"):
             chain_results(impl.entities(filter_obsoletes=True))
+        elif term.startswith(".dangling"):
+            chain_results(impl.dangling())
         elif term.startswith(".filter"):
             # arbitrary python expression
             expr = query_terms[0]
             query_terms = query_terms[1:]
             chain_results(eval(expr, {"impl": impl, "terms": results}))
         elif term.startswith(".query"):
             # arbitrary SPARQL query
@@ -2245,15 +2247,15 @@
                 dict(subject=s, object=o, path=path),
                 label_fields=["subject", "object", "path"],
             )
         writer.finish()
     if not node_ids:
         logging.warning("No paths found")
     if viz:
-        for node_id in node_ids:
+        for node_id in node_ids.union({e.pred for e in graph.edges}):
             [n] = [n for n in graph.nodes if n.id == node_id]
             path_graph.nodes.append(n)
         # TODO: abstract this out
         if output_type:
             write_graph(path_graph, format=output_type, output=output)
         else:
             if stylemap is None:
@@ -2625,20 +2627,20 @@
     help="ID file for set1",
 )
 @click.option(
     "--set2-file",
     help="ID file for set2",
 )
 @click.option(
-    "--jaccard-minimum",
+    "--min-jaccard-similarity",
     type=float,
     help="Minimum value for jaccard score",
 )
 @click.option(
-    "--ic-minimum",
+    "--min-ancestor-information-content",
     type=float,
     help="Minimum value for information content",
 )
 @click.option("-o", "--output", help="path to output")
 @click.option(
     "--main-score-field",
     default="phenodigm_score",
@@ -2650,16 +2652,16 @@
 @click.argument("terms", nargs=-1)
 def similarity(
     terms,
     predicates,
     set1_file,
     set2_file,
     autolabel: bool,
-    jaccard_minimum,
-    ic_minimum,
+    min_jaccard_similarity: Optional[float],
+    min_ancestor_information_content: Optional[float],
     main_score_field,
     output_type,
     output,
 ):
     """
     All by all similarity.
 
@@ -2740,27 +2742,25 @@
                 logging.info(f"Getting set2 from {set2_file}")
                 with open(set2_file) as file:
                     set2it = list(curies_from_file(file))
             else:
                 set2it = query_terms_iterator(terms, impl)
         actual_predicates = _process_predicates_arg(predicates)
         for sim in impl.all_by_all_pairwise_similarity(
-            set1it, set2it, predicates=actual_predicates
+            set1it,
+            set2it,
+            predicates=actual_predicates,
+            min_jaccard_similarity=min_jaccard_similarity,
+            min_ancestor_information_content=min_ancestor_information_content,
         ):
             if autolabel:
                 # TODO: this can be made more efficient
                 sim.subject_label = impl.label(sim.subject_id)
                 sim.object_label = impl.label(sim.object_id)
                 sim.ancestor_label = impl.label(sim.ancestor_id)
-            if jaccard_minimum is not None:
-                if sim.jaccard_similarity < jaccard_minimum:
-                    continue
-            if ic_minimum is not None:
-                if sim.ancestor_information_content < ic_minimum:
-                    continue
             writer.emit(sim)
         writer.finish()
         writer.file.close()
     else:
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
 
 
@@ -3604,15 +3604,15 @@
         for mapping in impl.sssom_mappings_by_source(subject_or_object_source=maps_to_source):
             if autolabel:
                 impl.inject_mapping_labels([mapping])
             writer.emit(mapping)
     else:
         logging.info(f"Fetching mappings for {terms}")
         for curie_it in chunk(query_terms_iterator(terms, impl)):
-            for mapping in impl.sssom_mappings(curie_it):
+            for mapping in list(impl.sssom_mappings(curie_it)):
                 if maps_to_source and not mapping.object_id.startswith(f"{maps_to_source}:"):
                     continue
                 if autolabel:
                     impl.inject_mapping_labels([mapping])
                 writer.emit(mapping)
     writer.finish()
 
@@ -4923,15 +4923,15 @@
 
     RULES: Using custom rules:
 
         runoak  -i foo.obo lexmatch -R match_rules.yaml -L foo.index.yaml -o foo.sssom.tsv
 
     Full documentation:
 
-    - https://incatools.github.io/ontology-access-kit/src/oaklib.utilities.lexical.lexical_indexer.html#
+    - https://incatools.github.io/ontology-access-kit/packages/src/oaklib.utilities.lexical.lexical_indexer.html#
     module-oaklib.utilities.lexical.lexical_indexer
     """
     impl = settings.impl
     if rules_file:
         ruleset = load_mapping_rules(rules_file)
     else:
         ruleset = None
```

### Comparing `oaklib-0.5.8/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.5.9/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/conf/mondo-g2d-input-spec.yaml` & `oaklib-0.5.9/src/oaklib/conf/mondo-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/conf/obograph-style.json` & `oaklib-0.5.9/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/converters/data_model_converter.py` & `oaklib-0.5.9/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.5.9/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.5.9/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.5.9/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.5.9/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     return s.replace('"', '\\"').replace("\n", "\\n")
 
 
 @dataclass
 class OboGraphToOboFormatConverter(DataModelConverter):
     """Converts from OboGraph to OBO Format."""
 
+    use_shorthand: bool = True
+
     def dump(self, source: GraphDocument, target: str = None, **kwargs) -> None:
         """
         Dump an OBO Graph Document to a FHIR CodeSystem
 
         :param source:
         :param target:
         :return:
@@ -96,28 +98,36 @@
         """
         if target is None:
             target = OboDocument()
         for g in source.graphs:
             self._convert_graph(g, target=target)
         return target
 
-    def _id(self, uri: CURIE) -> CURIE:
+    def _id(self, uri_or_curie: CURIE) -> CURIE:
         if not self.curie_converter:
-            return uri
-        curie = self.curie_converter.compress(uri)
+            return uri_or_curie
+        curie = self.curie_converter.compress(uri_or_curie)
         if curie is None:
-            return uri
+            return uri_or_curie
         else:
             return curie
 
+    def _predicate_id(self, uri_or_curie: CURIE, target: OboDocument) -> CURIE:
+        curie = self._id(uri_or_curie)
+        return target.curie_to_shorthand_map.get(curie, curie)
+
     def _convert_graph(self, source: Graph, target: OboDocument) -> OboDocument:
         edges_by_subject = index_graph_edges_by_subject(source)
         for n in source.nodes:
+            if n.type == "PROPERTY" and n.lbl:
+                shorthand = n.lbl.replace(" ", "_")
+                target.curie_to_shorthand_map[self._id(n.id)] = shorthand
+        for n in source.nodes:
             logging.debug(f"Converting node {n.id}")
-            self._convert_node(n, index=edges_by_subject, target=target)
+            self._convert_node(n, index=edges_by_subject, target=target, graph=source)
         for lda in source.logicalDefinitionAxioms:
             defined_class_id = self._id(lda.definedClassId)
             if defined_class_id not in target.stanzas:
                 target.add_stanza(Stanza(id=defined_class_id, type="Term"))
             stanza = target.stanzas[defined_class_id]
             for g in lda.genusIds:
                 obj = self._id(g)
@@ -125,17 +135,25 @@
             for r in lda.restrictions:
                 filler = self._id(r.fillerId)
                 pred = self._id(r.propertyId)
                 stanza.add_tag_value_pair(TAG_INTERSECTION_OF, pred, filler)
         return target
 
     def _convert_node(
-        self, source: Node, index: Dict[CURIE, List[Edge]], target: OboDocument
+        self,
+        source: Node,
+        index: Dict[CURIE, List[Edge]],
+        target: OboDocument,
+        graph: Graph = None,
     ) -> None:
         id = self._id(source.id)
+        shorthand_xref = None
+        if id in target.curie_to_shorthand_map:
+            shorthand_xref = id
+            id = target.curie_to_shorthand_map[id]
         logging.debug(f"Converting node {id} from {source}")
         t = source.type
         # if not t:
         #    logging.warning(f"No type for {id}")
         #    return
         if id.startswith("oio:"):
             return
@@ -144,21 +162,32 @@
             return
         stanza = Stanza(id=id, type=typedef_type)
         target.add_stanza(stanza)
         if source.lbl:
             stanza.add_tag_value(TAG_NAME, source.lbl)
         if source.meta:
             self._convert_meta(source, target=stanza)
+        if shorthand_xref:
+            stanza.add_tag_value(TAG_XREF, shorthand_xref)
         for e in index.get(source.id, []):
             obj = self._id(e.obj)
-            pred = self._id(e.pred)
+            obj_lbl = None
+            if graph:
+                nodes = [n for n in graph.nodes if n.id == e.obj]
+                if nodes:
+                    obj_lbl = nodes[0].lbl
+            if obj_lbl:
+                cmt = f" ! {obj_lbl}"
+            else:
+                cmt = ""
+            pred = self._predicate_id(e.pred, target)
             if e.pred in DIRECT_PREDICATE_MAP:
-                stanza.add_tag_value(DIRECT_PREDICATE_MAP[e.pred], obj)
+                stanza.add_tag_value(DIRECT_PREDICATE_MAP[e.pred], f"{obj}{cmt}")
             else:
-                stanza.add_tag_value(TAG_RELATIONSHIP, f"{pred} {obj}")
+                stanza.add_tag_value(TAG_RELATIONSHIP, f"{pred} {obj}{cmt}")
         return
 
     def _convert_meta(self, source: Node, target: Stanza):
         meta = source.meta
         logging.debug(f"ADDING DEF {target}")
         if meta.definition:
             xrefs = ", ".join(meta.definition.xrefs)
```

### Comparing `oaklib-0.5.8/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.5.9/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/association.py` & `oaklib-0.5.9/src/oaklib/datamodels/association.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/association.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/association.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.5.9/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.5.9/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/cx.py` & `oaklib-0.5.9/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/cx.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/fhir.py` & `oaklib-0.5.9/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/input_specification.py` & `oaklib-0.5.9/src/oaklib/datamodels/input_specification.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/input_specification.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/input_specification.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/item_list.py` & `oaklib-0.5.9/src/oaklib/datamodels/item_list.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/item_list.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.5.9/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.5.9/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.5.9/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.5.9/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.5.9/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/obograph.py` & `oaklib-0.5.9/src/oaklib/datamodels/obograph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.5.9/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.5.9/src/oaklib/datamodels/ontology_metadata.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.5.9/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/oxo.py` & `oaklib-0.5.9/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/search.py` & `oaklib-0.5.9/src/oaklib/datamodels/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,11 +86,13 @@
 
 
 @dataclass
 class SearchConfiguration(SearchBaseConfiguration):
     """
     Parameters for altering behavior of search
 
-    .. note ::
+    Examples:
+
+    >>> from oaklib.datamodels.search import SearchConfiguration, SearchTermSyntax
+    >>> cfg = SearchConfiguration(syntax=SearchTermSyntax.REGULAR_EXPRESSION)
 
-        many of these parameters are not yet implemented
     """
```

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.5.9/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/similarity.py` & `oaklib-0.5.9/src/oaklib/datamodels/similarity.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.5.9/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.5.9/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.5.9/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.5.9/src/oaklib/datamodels/text_annotator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.5.9/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.5.9/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.5.9/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.5.9/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.5.9/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.5.9/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.5.9/src/oaklib/datamodels/vocabulary.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 OWL_CLASS = "owl:Class"
 OWL_NAMED_INDIVIDUAL = "owl:NamedIndividual"
 OWL_OBJECT_PROPERTY = "owl:ObjectProperty"
 OWL_DATATYPE_PROPERTY = "owl:DatatypeProperty"
 OWL_ANNOTATION_PROPERTY = "owl:AnnotationProperty"
 OWL_TRANSITIVE_PROPERTY = "owl:TransitiveProperty"
 OWL_SYMMETRIC_PROPERTY = "owl:SymmetricProperty"
+OWL_ASYMMETRIC_PROPERTY = "owl:SymmetricProperty"
+OWL_REFLEXIVE_PROPERTY = "owl:ReflexiveProperty"
+OWL_IRREFLEXIVE_PROPERTY = "owl:IrreflexiveProperty"
 OWL_THING = "owl:Thing"
 OWL_NOTHING = "owl:Nothing"
 IS_DEFINED_BY = "rdfs:isDefinedBy"
 RDFS_COMMENT = "rdfs:comment"
 SUBCLASS_OF = omd.slots.subClassOf.curie
 IS_A = omd.slots.subClassOf.curie
 DISJOINT_WITH = "owl:disjointWith"
@@ -71,14 +74,18 @@
 RDFS_RANGE = "rdfs:range"
 INVERSE_OF = "owl:inverseOf"
 RDF_TYPE = "rdf:type"
 RDFS_LABEL = "rdfs:label"
 EQUIVALENT_CLASS = "owl:equivalentClass"
 OWL_SAME_AS = "owl:sameAs"
 RDF_SEE_ALSO = "rdfs:seeAlso"
+OWL_RESTRICTION = "owl:Restriction"
+OWL_ON_PROPERTY = "owl:onProperty"
+OWL_SOME_VALUES_FROM = "owl:someValuesFrom"
+OWL_PROPERTY_CHAIN_AXIOM = "owl:propertyChainAxiom"
 
 OWL_META_CLASSES = [
     OWL_CLASS,
     OWL_OBJECT_PROPERTY,
     OWL_NAMED_INDIVIDUAL,
     OWL_DATATYPE_PROPERTY,
     OWL_ANNOTATION_PROPERTY,
@@ -98,14 +105,16 @@
     TERMS_MERGED,
     HAS_ONTOLOGY_ROOT_TERM,
     HAS_OBO_NAMESPACE,
     LABEL_PREDICATE,
 ]
 
 PART_OF = "BFO:0000050"
+PRECEDED_BY = "BFO:0000062"
+OVERLAPS = "RO:0002131"
 LOCATED_IN = "RO:0001025"
 DEVELOPS_FROM = "RO:0002202"
 HAS_PART = "BFO:0000051"
 ONLY_IN_TAXON = "RO:0002160"
 NEVER_IN_TAXON = "RO:0002161"
 IN_TAXON = "RO:0002162"
 PRESENT_IN_TAXON = "RO:0002175"
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/__init__.py` & `oaklib-0.5.9/src/oaklib/implementations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from oaklib.implementations.sqldb.sql_implementation import SqlImplementation
 from oaklib.implementations.translator.translator_implementation import (
     TranslatorImplementation,
 )
 from oaklib.implementations.ubergraph.ubergraph_implementation import (
     UbergraphImplementation,
 )
+from oaklib.implementations.uniprot.uniprot_implementation import UniprotImplementation
 from oaklib.implementations.wikidata.wikidata_implementation import (
     WikidataImplementation,
 )
 from oaklib.interfaces import OntologyInterface
 
 __all__ = [
     "get_implementation_resolver",
@@ -83,14 +84,15 @@
     "LovImplementation",
     "SparqlImplementation",
     "WikidataImplementation",
     "PubMedImplementation",
     "FunOwlImplementation",
     "GildaImplementation",
     "KGXImplementation",
+    "UniprotImplementation",
     "TranslatorImplementation",
     "OakMetaModelImplementation",
     "SemSimianImplementation",
 ]
 
 
 @cache
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,24 +44,26 @@
 
     This allows for multiple implementations to be wrapped, with calls to
     the aggregator farming out queries to multiple implementations, and weaving
     the results together.
 
     >>> from oaklib import get_adapter
     >>> from oaklib.implementations import AggregatorImplementation
+    >>> from oaklib.datamodels.search import SearchConfiguration, SearchTermSyntax
     >>> hp = get_adapter("sqlite:obo:hp")
     >>> mp = get_adapter("sqlite:obo:mp")
+    >>> cfg = SearchConfiguration(syntax=SearchTermSyntax.REGULAR_EXPRESSION)
     >>> agg = AggregatorImplementation(implementations=[hp, mp])
-    >>> for entity in sorted(agg.basic_search("morphology")):
-    ...     print(entity)
+    >>> for entity in sorted(agg.basic_search("parathyroid", config=cfg)):
+    ...     print(entity, agg.label(entity))
     <BLANKLINE>
     ...
-    HP:3000036
+    HP:0000860 Parathyroid hypoplasia
     ...
-    MP:0031139
+    MP:0000680 absent parathyroid glands
     ...
 
     Command Line Usage
     ------------------
 
     Use the :code:`--add` (:code:`-a`) option before the main command to add additional implementations.
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/agrkb/agrkb_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/agrkb/agrkb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/amigo/amigo_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/amigo/amigo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/eutils/eutils_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/eutils/eutils_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/eutils/pubmed_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/eutils/pubmed_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/gilda.py` & `oaklib-0.5.9/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import rdflib
 import sqlalchemy.orm
 from linkml_runtime import SchemaView
 from linkml_runtime.dumpers import json_dumper
 from linkml_runtime.utils.introspection import package_schemaview
 from sqlalchemy import Column, MetaData, String, Table, create_engine
-from sqlalchemy.orm import declarative_base, mapper
+from sqlalchemy.orm import declarative_base, registry
 
 import oaklib.datamodels.ontology_metadata as om
 from oaklib.datamodels import obograph, ontology_metadata
 from oaklib.datamodels.association import Association
 from oaklib.datamodels.search import SearchConfiguration
 from oaklib.datamodels.search_datamodel import SearchProperty, SearchTermSyntax
 from oaklib.datamodels.vocabulary import (
@@ -248,25 +248,26 @@
             logging.info(f"Locator, post-processed: {locator}")
             self.engine = create_engine(locator)
             self._add_orm_mappings()
 
     def _add_orm_mappings(self):
         # https://stackoverflow.com/questions/2574105/sqlalchemy-dynamic-mapping/2575016#2575016
         engine = self.engine
-        metadata = MetaData(bind=engine)
+        metadata = MetaData()
         colmap = self._introspect()
+        mapper_registry = registry()
         # metadata.reflect(bind=engine)
         for (cls, table_name), cols in colmap.items():
             t = Table(
                 table_name,
                 metadata,
                 Column("id", String, primary_key=True),
                 *(Column(col, String) for col in cols),
             )
-            mapper(cls, t)
+            mapper_registry.map_imperatively(cls, t)
         self._session = sqlalchemy.orm.create_session(bind=engine, autocommit=False, autoflush=True)
         self._add_missing_tables()
 
     def _introspect(self) -> Dict[Tuple[Type, str], List[str]]:
         engine = self.engine
         metadata = MetaData()
         logging.info(f"Reflecting using {engine}")
@@ -283,15 +284,15 @@
                 if column.name == "id":
                     continue
                 colmap[k].append(column.name)
         return colmap
 
     def _add_missing_tables(self):
         engine = self.engine
-        metadata = MetaData(bind=engine)
+        metadata = MetaData()
         metadata.reflect(bind=engine)
         for cls in [NodeProperty]:
             tables = [table for table in metadata.sorted_tables if table.name == cls.__tablename__]
             if len(tables) == 0:
                 logging.info(f"Creating table {cls.__tablename__}")
                 cls.__table__.create(bind=engine)
                 self._populate_table(cls)
@@ -356,15 +357,15 @@
     def obsoletes(self, include_merged=True) -> Iterable[CURIE]:
         raise NotImplementedError("TODO: add to monarch dump")
 
     def all_relationships(self) -> Iterable[RELATIONSHIP]:
         for row in self.session.query(Edge):
             yield row.subject, row.predicate, row.object
 
-    def label(self, curie: CURIE) -> Optional[str]:
+    def label(self, curie: CURIE, **kwargs) -> Optional[str]:
         q = self.session.query(Node.name).filter(Node.id == curie)
         logging.debug(f"Label query: {q} // {curie}")
         for row in q:
             return row[0]
 
     def labels(self, curies: Iterable[CURIE], allow_none=True) -> Iterable[Tuple[CURIE, str]]:
         for curie_it in chunk(curies, self.max_items_for_in_clause):
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/monarch/monarch_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/monarch/monarch_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import re
 from collections import defaultdict
+from copy import deepcopy
 from dataclasses import dataclass
 from typing import Any, Dict, Iterable, Iterator, List, Mapping, Optional, Tuple, Union
 
 import sssom_schema as sssom
 from kgcl_schema.datamodel import kgcl
 from linkml_runtime.dumpers import json_dumper
 from linkml_runtime.loaders import json_loader
@@ -206,14 +207,16 @@
                         else:
                             # previously encountered node was dangling/stub;
                             # replace
                             node = n
                     else:
                         node = n
         if node:
+            node = deepcopy(node)
+            node.id = self.uri_to_curie(node.id)
             return node
         else:
             if strict:
                 raise ValueError(f"No such node {curie}")
 
     def _meta(self, curie: CURIE, strict=False) -> Optional[Meta]:
         n = self._node(curie, strict=strict)
@@ -300,24 +303,22 @@
         predicates: List[PRED_CURIE] = None,
         objects: List[CURIE] = None,
         include_tbox: bool = True,
         include_abox: bool = True,
         include_entailed: bool = False,
         exclude_blank: bool = True,
     ) -> Iterator[RELATIONSHIP]:
-        for s in self._relationship_index.keys():
-            if subjects is not None and s not in subjects:
-                continue
-            for s2, p, o in self._relationship_index[s]:
-                if s2 == s:
-                    if predicates is not None and p not in predicates:
-                        continue
-                    if objects is not None and o not in objects:
-                        continue
-                    yield s, p, o
+        ei = self.edge_index
+        if include_entailed:
+            raise NotImplementedError("Entailment not supported for pronto")
+        yield from ei.edges(
+            subjects=subjects,
+            predicates=predicates,
+            objects=objects,
+        )
 
     # TODO: DRY
     def outgoing_relationships(
         self, curie: CURIE, predicates: List[PRED_CURIE] = None, entailed=False
     ) -> Iterator[Tuple[PRED_CURIE, CURIE]]:
         for s, p, o in self.relationships([curie], predicates, include_entailed=entailed):
             if s == curie:
@@ -457,7 +458,22 @@
         self,
         patch: kgcl.Change,
         activity: kgcl.Activity = None,
         metadata: Mapping[PRED_CURIE, Any] = None,
         configuration: kgcl.Configuration = None,
     ) -> kgcl.Change:
         raise NotImplementedError
+
+    # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+    # Implements: OwlInterface
+    # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+    def transitive_object_properties(self) -> Iterable[CURIE]:
+        # TODO: obographs datamodel needs to be expanded to support this
+        pass
+
+    def simple_subproperty_of_chains(self) -> Iterable[Tuple[CURIE, List[CURIE]]]:
+        for g in self.obograph_document.graphs:
+            for pca in g.propertyChainAxioms:
+                yield self.uri_to_curie(pca.predicateId), [
+                    self.uri_to_curie(p) for p in pca.chainPredicateIds
+                ]
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 from sssom_schema import Mapping
 
 from oaklib.datamodels import oxo
 from oaklib.datamodels.oxo import ScopeEnum
 from oaklib.datamodels.search import SearchConfiguration, SearchProperty
 from oaklib.datamodels.text_annotator import TextAnnotation
 from oaklib.datamodels.vocabulary import IS_A, SEMAPV
+from oaklib.implementations.ols.constants import SEARCH_CONFIG
+from oaklib.implementations.ols.oxo_utils import load_oxo_payload
 from oaklib.interfaces.basic_ontology_interface import PREFIX_MAP
 from oaklib.interfaces.mapping_provider_interface import MappingProviderInterface
 from oaklib.interfaces.search_interface import SearchInterface
 from oaklib.interfaces.text_annotator_interface import TextAnnotatorInterface
 from oaklib.types import CURIE, PRED_CURIE
 
-from .constants import SEARCH_CONFIG
-from .oxo_utils import load_oxo_payload
-
 __all__ = [
     # Abstract classes
     "BaseOlsImplementation",
     # Concrete classes
     "OlsImplementation",
     "TIBOlsImplementation",
 ]
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.5.9/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,19 +43,23 @@
     >>> oi = OntobeeImplementation()
 
     The default ontobee endpoint will be assumed
 
     Alternatively, use a selector:
 
     >>> from oaklib import get_adapter
-    >>> from oaklib.datamodels.vocabulary import IS_A
     >>> oi = get_adapter("ontobee:")
 
+    Or to access a specific ontology, such as the Vaccine Ontology:
+
+    >>> oi = get_adapter("ontobee:vo")
+
     After that you can use any of the methods that OntoBee implements; e.g.
 
+    >>> from oaklib.datamodels.vocabulary import IS_A
     >>> # uncomment to test
     >>> # for a in oi.ancestors("UBERON:0002398", predicates=[IS_A]):
     >>> #    print(a)
 
     Command Line
     ------------
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.5.9/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import collections
 import logging
 from abc import ABC
 from dataclasses import dataclass, field
-from typing import Any, ClassVar, Dict, Iterable, Iterator, List, Tuple, Union
+from typing import Any, ClassVar, Dict, Iterable, Iterator, List, Optional, Tuple, Union
 from urllib.parse import quote
 
 import requests
 from ontoportal_client.api import PreconfiguredOntoPortalClient
 from prefixmaps.io.parser import load_multi_context
 from sssom_schema import Mapping
 
@@ -13,15 +14,19 @@
 from oaklib.datamodels.text_annotator import TextAnnotation, TextAnnotationConfiguration
 from oaklib.datamodels.vocabulary import SEMAPV
 from oaklib.interfaces import (
     MappingProviderInterface,
     SearchInterface,
     TextAnnotatorInterface,
 )
-from oaklib.interfaces.basic_ontology_interface import METADATA_MAP, PREFIX_MAP
+from oaklib.interfaces.basic_ontology_interface import (
+    LANGUAGE_TAG,
+    METADATA_MAP,
+    PREFIX_MAP,
+)
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.types import CURIE, URI
 from oaklib.utilities.apikey_manager import get_apikey_value
 from oaklib.utilities.rate_limiter import check_limit
 
 SEARCH_CONFIG = SearchConfiguration()
 
@@ -118,14 +123,34 @@
             if curie in label_cache:
                 yield curie, label_cache[curie]
             else:
                 label = self.label(curie)
                 label_cache[curie] = label
                 yield curie, label
 
+    def label(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
+        if lang:
+            raise NotImplementedError("Language not supported")
+        _obj = self._class(curie)
+        return _obj.get("prefLabel", None)
+
+    def _class(self, curie: CURIE) -> dict:
+        ontology, class_uri = self._get_ontology_and_uri_from_id(curie)
+        logging.debug(f"Fetching class for {ontology} class = {class_uri}")
+        quoted_class_uri = quote(class_uri, safe="")
+        req_url = f"/ontologies/{ontology}/classes/{quoted_class_uri}"
+        logging.debug(req_url)
+        response = self._get_response(
+            req_url, params={"display_context": "false"}, raise_for_status=False
+        )
+        if response.status_code != requests.codes.ok:
+            logging.warning(f"Could not fetch class for {curie}")
+            return {}
+        return response.json()
+
     def annotate_text(
         self, text: str, configuration: TextAnnotationConfiguration = None
     ) -> Iterator[TextAnnotation]:
         """
          Implements annotate_text from text_annotator_interface by calling the
          `annotate` endpoint using ontoportal client.
 
@@ -216,15 +241,26 @@
                     obj = self._get_json(next_page)
                     collection = obj["collection"]
 
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     # Implements: MappingProviderInterface
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-    def get_sssom_mappings_by_curie(self, id: Union[CURIE, URI]) -> Iterable[Mapping]:
+    def sssom_mappings(
+        self, curies: Optional[Union[CURIE, Iterable[CURIE]]] = None, source: Optional[str] = None
+    ) -> Iterable[Mapping]:
+        if not isinstance(curies, str):
+            if isinstance(curies, collections.Iterable):
+                curies = list(curies)
+            if not isinstance(curies, list):
+                raise ValueError(f"Invalid curies: {curies}")
+            for curie in curies:
+                yield from self.sssom_mappings(curie, source=source)
+            return
+        id = curies
         ontology, class_uri = self._get_ontology_and_uri_from_id(id)
         logging.debug(f"Fetching mappings for {ontology} class = {class_uri}")
         # This may return lots of duplicate mappings
         # See: https://github.com/ncbo/ontologies_linked_data/issues/117
         quoted_class_uri = quote(class_uri, safe="")
         req_url = f"/ontologies/{ontology}/classes/{quoted_class_uri}/mappings"
         logging.debug(req_url)
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,19 @@
     OIO_SYNONYM_TYPE_PROPERTY,
     OWL_CLASS,
     OWL_OBJECT_PROPERTY,
     OWL_VERSION_INFO,
     SCOPE_TO_SYNONYM_PRED_MAP,
     SEMAPV,
     SKOS_CLOSE_MATCH,
+    SKOS_MATCH_PREDICATES,
     TERM_REPLACED_BY,
     TERMS_MERGED,
 )
+from oaklib.inference.relation_graph_reasoner import RelationGraphReasoner
 from oaklib.interfaces import TextAnnotatorInterface
 from oaklib.interfaces.basic_ontology_interface import (
     ALIAS_MAP,
     LANGUAGE_TAG,
     METADATA_MAP,
     PRED_CURIE,
     RELATIONSHIP,
@@ -58,14 +60,15 @@
 )
 from oaklib.interfaces.differ_interface import DifferInterface
 from oaklib.interfaces.dumper_interface import DumperInterface
 from oaklib.interfaces.mapping_provider_interface import MappingProviderInterface
 from oaklib.interfaces.merge_interface import MergeInterface
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.interfaces.obolegacy_interface import OboLegacyInterface
+from oaklib.interfaces.owl_interface import OwlInterface
 from oaklib.interfaces.patcher_interface import PatcherInterface
 from oaklib.interfaces.rdf_interface import RdfInterface
 from oaklib.interfaces.search_interface import SearchInterface
 from oaklib.interfaces.semsim_interface import SemanticSimilarityInterface
 from oaklib.interfaces.summary_statistics_interface import SummaryStatisticsInterface
 from oaklib.interfaces.taxon_constraint_interface import TaxonConstraintInterface
 from oaklib.interfaces.validator_interface import ValidatorInterface
@@ -99,14 +102,15 @@
     ClassEnrichmentCalculationInterface,
     SemanticSimilarityInterface,
     TextAnnotatorInterface,
     SummaryStatisticsInterface,
     TaxonConstraintInterface,
     DumperInterface,
     MergeInterface,
+    OwlInterface,
 ):
     """
     An adapter that standardizes access to OBO Format files by wrapping the Pronto library.
 
     `Pronto <https://github.com/althonos/pronto/>`_ is a high-performance parsing library
     for parsing obo format 1.4 and other formats.
 
@@ -119,29 +123,29 @@
     - ``pronto:https://example.com/my/file``
     - ``prontolib:go`
 
     Examples
     --------
 
     >>> from oaklib.implementations import ProntoImplementation
-    >>> resource = OntologyResource(slug='go-nucleus.obo', directory='test/inputinput', local=True)
-    >>> oi = ProntoImplementation(resource)
+    >>> resource = OntologyResource(slug='go-nucleus.obo', directory='tests/input', local=True)
+    >>> adapter = ProntoImplementation(resource)
 
     Or use a selector:
 
     >>> from oaklib import get_adapter
-    >>> oi = get_adapter("pronto:tests/input/go-nucleus.obo")
+    >>> adapter = get_adapter("pronto:tests/input/go-nucleus.obo")
 
     Then you can use any of the methods implemented by pronto
 
-    >>> rels = oi.outgoing_relationships('GO:0005773')
-    >>> for rel, parents in rels.items():
-    >>>    print(f'  {rel} ! {oi.label(rel)}')
-    >>>        for parent in parents:
-    >>>            print(f'    {parent} ! {oi.label(parent)}')
+    >>> rels = adapter.relationships(['GO:0005773'])
+    >>> for _s, p, o in rels:
+    ...    print(f'  {p} {o} ! {adapter.label(o)}')
+    rdfs:subClassOf GO:0043231 ! intracellular membrane-bounded organelle
+    BFO:0000050 GO:0005737 ! cytoplasm
 
     .. warning::
 
        pronto uses the fastobo library for loading ontologies. This follows a strict
        interpretation of obo format, and some ontologies may fail to load.
        In these cases, consider an alternative implementation
 
@@ -199,14 +203,18 @@
                         pass
                 if term.equivalent_to:
                     for o in term.equivalent_to.ids:
                         # symmetric
                         yield s, EQUIVALENT_CLASS, o
                         yield o, EQUIVALENT_CLASS, s
 
+    def _all_entailed_relationships(self):
+        reasoner = RelationGraphReasoner(self)
+        yield from reasoner.entailed_edges()
+
     def store(self, resource: OntologyResource = None) -> None:
         if resource is None:
             resource = self.resource
         ontology = self.wrapped_ontology
         if resource.local:
             if resource.slug:
                 with open(str(resource.local_path), "wb") as f:
@@ -394,43 +402,44 @@
     def curies_by_label(self, label: str) -> List[CURIE]:
         return [t.id for t in self.wrapped_ontology.terms() if t.name == label]
 
     def _get_pronto_relationship_type_curie(self, rel_type: pronto.Relationship) -> CURIE:
         for x in rel_type.xrefs:
             if x.id.startswith("BFO:") or x.id.startswith("RO:"):
                 return x.id
+        for x in rel_type.xrefs:
+            if x.id.startswith("http"):
+                compacted = self.uri_to_curie(x.id)
+                return compacted
         return rel_type.id
 
     def relationships(
         self,
         subjects: List[CURIE] = None,
         predicates: List[PRED_CURIE] = None,
         objects: List[CURIE] = None,
         include_tbox: bool = True,
         include_abox: bool = True,
         include_entailed: bool = False,
         exclude_blank: bool = True,
     ) -> Iterator[RELATIONSHIP]:
-        for s in self._relationship_index.keys():
-            if subjects is not None and s not in subjects:
-                continue
-            for s2, p, o in self._relationship_index[s]:
-                if s2 == s:
-                    if predicates is not None and p not in predicates:
-                        continue
-                    if objects is not None and o not in objects:
-                        continue
-                    yield s, p, o
+        ei = self.edge_index
+        if include_entailed:
+            ei = self.entailed_edge_index
+        yield from ei.edges(
+            subjects=subjects,
+            predicates=predicates,
+            objects=objects,
+        )
 
     def outgoing_relationships(
         self, curie: CURIE, predicates: List[PRED_CURIE] = None, entailed=False
     ) -> Iterator[Tuple[PRED_CURIE, CURIE]]:
-        for s, p, o in self.relationships([curie], predicates, include_entailed=entailed):
-            if s == curie:
-                yield p, o
+        for _s, p, o in self.relationships([curie], predicates, include_entailed=entailed):
+            yield p, o
 
     def create_entity(
         self,
         curie: CURIE,
         label: Optional[str] = None,
         relationships: Optional[RELATIONSHIP_MAP] = None,
         type: Optional[str] = None,
@@ -496,38 +505,31 @@
         m[LABEL_PREDICATE] = [t.name]
         for s in t.synonyms:
             pred = _synonym_scope_pred(s)
             m[pred].append(s.description)
         return m
 
     def simple_mappings_by_curie(self, curie: CURIE) -> Iterable[Tuple[PRED_CURIE, CURIE]]:
-        m = defaultdict(list)
         t = self._entity(curie)
         if t is None:
-            return m
+            return
         for s in t.xrefs:
-            # m[HAS_DBXREF].append(s.id)
             yield HAS_DBXREF, s.id
         for s in t.annotations:
-            # TODO: less hacky
-            if s.property.startswith("skos"):
+            rel = self._entity(s.property)
+            if ":" in s.property:
+                pred = s.property
+            else:
+                pred = self._get_pronto_relationship_type_curie(rel)
+            if pred in SKOS_MATCH_PREDICATES:
                 if isinstance(s, LiteralPropertyValue):
                     v = s.literal
-                    # m[s.property].append(v)
-                    yield s.property, v
+                    yield pred, v
                 elif isinstance(s, ResourcePropertyValue):
-                    try:
-                        tail = self.uri_to_curie(s.resource)
-                    except ValueError:
-                        logging.warning(
-                            "%s could not compress URI %s", self.__class__.__name__, s.resource
-                        )
-                        continue
-                    else:
-                        yield s.property, tail
+                    yield pred, s.resource
 
     def entity_metadata_map(self, curie: CURIE) -> METADATA_MAP:
         t = self._entity(curie)
         m = defaultdict(list)
         _alt_id_map = self._get_alt_id_to_replacement_map()
         if t:
             for ann in t.annotations:
@@ -613,29 +615,25 @@
             curies = [curies]
         elif curies is None:
             curies = list(self.entities())
         else:
             curies = list(curies)
         # mappings where curie is the subject:
         for curie in curies:
-            t = self._entity(curie)
-            if t:
-                for x in t.xrefs:
-                    m = sssom.Mapping(
-                        subject_id=t.id,
-                        predicate_id=SKOS_CLOSE_MATCH,
-                        object_id=x.id,
-                        mapping_justification=sssom.EntityReference(
-                            SEMAPV.UnspecifiedMatching.value
-                        ),
-                    )
-                    inject_mapping_sources(m)
-                    if source and m.object_source != source and m.subject_source != source:
-                        continue
-                    yield m
+            for pred, obj in self.simple_mappings_by_curie(curie):
+                m = sssom.Mapping(
+                    subject_id=curie,
+                    predicate_id=pred,
+                    object_id=obj,
+                    mapping_justification=sssom.EntityReference(SEMAPV.UnspecifiedMatching.value),
+                )
+                inject_mapping_sources(m)
+                if source and m.object_source != source and m.subject_source != source:
+                    continue
+                yield m
         # mappings where curie is the object:
         # TODO: use a cache to avoid re-calculating
         for e in self.entities():
             t = self._entity(e)
             if t:
                 for x in t.xrefs:
                     if x.id in curies:
@@ -875,7 +873,28 @@
             synonym_to_remove = [
                 syn for syn in t._data().synonyms if syn.description == patch.old_value
             ][0]
             t._data().synonyms.discard(synonym_to_remove)
         else:
             raise NotImplementedError(f"cannot handle KGCL type {type(patch)}")
         return patch
+
+    # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+    # Implements: OwlInterface
+    # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+    def transitive_object_properties(self) -> Iterable[CURIE]:
+        for t in self.wrapped_ontology.relationships():
+            if t.transitive:
+                yield self._get_pronto_relationship_type_curie(t)
+
+    def simple_subproperty_of_chains(self) -> Iterable[Tuple[CURIE, List[CURIE]]]:
+        for t in self.wrapped_ontology.relationships():
+            try:
+                if t.holds_over_chain:
+                    subp = self._get_pronto_relationship_type_curie(t)
+                    r1, r2 = t.holds_over_chain
+                    p1 = self._get_pronto_relationship_type_curie(r1)
+                    p2 = self._get_pronto_relationship_type_curie(r2)
+                    yield subp, [p1, p2]
+            except KeyError as e:
+                logging.warning(f"could not find chain relationships for {t}: {e}")
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/semsimian/semsimian_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/semsimian/semsimian_implementation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """Rust implementation of semantic similarity measures."""
 import inspect
 import logging
 import math
 from dataclasses import dataclass
-from typing import ClassVar, List
+from typing import ClassVar, List, Optional
 
-from semsimian import (
-    max_information_content,
-    relationships_to_closure_table,
-    semantic_jaccard_similarity,
-)
+from semsimian import Semsimian
 
 from oaklib.datamodels.similarity import TermPairwiseSimilarity
 from oaklib.interfaces.basic_ontology_interface import BasicOntologyInterface
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.interfaces.search_interface import SearchInterface
 from oaklib.interfaces.semsim_interface import SemanticSimilarityInterface
 from oaklib.types import CURIE, PRED_CURIE
@@ -55,56 +51,65 @@
         logging.info(f"Wrapping an existing OAK implementation to fetch {slug}")
         self.wrapped_adapter = get_adapter(slug)
         methods = dict(inspect.getmembers(self.wrapped_adapter))
         for m in self.delegated_methods:
             mn = m if isinstance(m, str) else m.__name__
             setattr(SemSimianImplementation, mn, methods[mn])
 
-        rels = [r for r in self.wrapped_adapter.relationships(include_entailed=True)]
-        self._rust_closure_table = relationships_to_closure_table(rels)
-        # TODO: eliminate the need for this
-        self._entities = {r[0] for r in rels}
+        spo = [r for r in self.wrapped_adapter.relationships(include_entailed=True)]
+        self.semsimian = Semsimian(spo)
 
     def pairwise_similarity(
         self,
         subject: CURIE,
         object: CURIE,
         predicates: List[PRED_CURIE] = None,
         subject_ancestors: List[CURIE] = None,
         object_ancestors: List[CURIE] = None,
-    ) -> TermPairwiseSimilarity:
+        min_jaccard_similarity: Optional[float] = None,
+        min_ancestor_information_content: Optional[float] = None,
+    ) -> Optional[TermPairwiseSimilarity]:
         """
         Pairwise similarity between a pair of ontology terms
 
         :param subject:
         :param object:
         :param predicates:
         :param subject_ancestors: optional pre-generated ancestor list
         :param object_ancestors: optional pre-generated ancestor list
+        :param min_jaccard_similarity: optional minimum jaccard similarity
+        :param min_ancestor_information_content: optional minimum ancestor information content
         :return:
         """
-        logging.info(f"Calculating pairwise similarity for {subject} x {object} over {predicates}")
+        logging.debug(f"Calculating pairwise similarity for {subject} x {object} over {predicates}")
+
+        jaccard_val = self.semsimian.jaccard_similarity(subject, object, set(predicates))
+
+        if math.isnan(jaccard_val):
+            return None
+
+        ancestor_information_content_val = self.semsimian.resnik_similarity(
+            subject, object, set(predicates)
+        )
+
+        if math.isnan(ancestor_information_content_val):
+            return None
+
+        if (min_jaccard_similarity is not None and jaccard_val < min_jaccard_similarity) or (
+            min_ancestor_information_content is not None
+            and ancestor_information_content_val < min_ancestor_information_content
+        ):
+            return None
+
         sim = TermPairwiseSimilarity(
             subject_id=subject,
             object_id=object,
             ancestor_id=None,
             ancestor_information_content=None,
         )
-        if subject not in self._entities or object not in self._entities:
-            logging.debug(f"Unknown entity in {subject} x {object}")
-            if subject == object:
-                sim.jaccard_similarity = 1.0
-            else:
-                sim.jaccard_similarity = 0.0
-            sim.ancestor_information_content = 0.0
-            return sim
-
-        if predicates:
-            predicates = set(predicates)
-        sim.jaccard_similarity = semantic_jaccard_similarity(
-            self._rust_closure_table, subject, object, predicates
-        )
-        sim.ancestor_information_content = max_information_content(
-            self._rust_closure_table, subject, object, predicates
-        )
+
+        sim.jaccard_similarity = jaccard_val
+        sim.ancestor_information_content = ancestor_information_content_val
+
         sim.phenodigm_score = math.sqrt(sim.jaccard_similarity * sim.ancestor_information_content)
+
         return sim
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,70 +41,81 @@
     CREATED,
     CREATOR,
     DEPRECATED_PREDICATE,
     EQUIVALENT_CLASS,
     HAS_DBXREF,
     HAS_OBO_NAMESPACE,
     HAS_OBSOLESCENCE_REASON,
+    INVERSE_OF,
     IS_A,
     LABEL_PREDICATE,
     OIO_CREATED_BY,
     OIO_CREATION_DATE,
     OIO_SUBSET_PROPERTY,
     OIO_SYNONYM_TYPE_PROPERTY,
     OWL_CLASS,
     OWL_OBJECT_PROPERTY,
     OWL_VERSION_IRI,
+    RDFS_DOMAIN,
+    RDFS_RANGE,
     SEMAPV,
     SKOS_CLOSE_MATCH,
+    SUBPROPERTY_OF,
     TERM_REPLACED_BY,
     TERMS_MERGED,
 )
 from oaklib.implementations.simpleobo.simple_obo_parser import (
     TAG_ALT_ID,
     TAG_COMMENT,
     TAG_CONSIDER,
     TAG_CREATED_BY,
     TAG_CREATION_DATE,
     TAG_DATA_VERSION,
     TAG_DEFINITION,
+    TAG_DOMAIN,
     TAG_EQUIVALENT_TO,
+    TAG_HOLDS_OVER_CHAIN,
     TAG_ID_SPACE,
+    TAG_INVERSE_OF,
     TAG_IS_A,
     TAG_IS_OBSOLETE,
+    TAG_IS_TRANSITIVE,
     TAG_NAME,
     TAG_NAMESPACE,
     TAG_ONTOLOGY,
     TAG_PROPERTY_VALUE,
+    TAG_RANGE,
     TAG_RELATIONSHIP,
     TAG_REPLACED_BY,
     TAG_SUBSET,
     TAG_SUBSETDEF,
     TAG_SYNONYM,
     TAG_SYNONYMTYPEDEF,
     TAG_XREF,
     OboDocument,
     Stanza,
     _synonym_scope_pred,
     parse_obo_document,
 )
+from oaklib.inference.relation_graph_reasoner import RelationGraphReasoner
 from oaklib.interfaces import TextAnnotatorInterface
 from oaklib.interfaces.basic_ontology_interface import (
     ALIAS_MAP,
     LANGUAGE_TAG,
     METADATA_MAP,
     RELATIONSHIP,
     RELATIONSHIP_MAP,
 )
 from oaklib.interfaces.differ_interface import DifferInterface
 from oaklib.interfaces.dumper_interface import DumperInterface
 from oaklib.interfaces.mapping_provider_interface import MappingProviderInterface
 from oaklib.interfaces.merge_interface import MergeInterface
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.interfaces.obolegacy_interface import PRED_CODE, OboLegacyInterface
+from oaklib.interfaces.owl_interface import OwlInterface
 from oaklib.interfaces.patcher_interface import PatcherInterface
 from oaklib.interfaces.rdf_interface import RdfInterface
 from oaklib.interfaces.search_interface import SearchInterface
 from oaklib.interfaces.summary_statistics_interface import SummaryStatisticsInterface
 from oaklib.interfaces.taxon_constraint_interface import TaxonConstraintInterface
 from oaklib.interfaces.validator_interface import ValidatorInterface
 from oaklib.resource import OntologyResource
@@ -128,14 +139,15 @@
     MappingProviderInterface,
     PatcherInterface,
     SummaryStatisticsInterface,
     TaxonConstraintInterface,
     TextAnnotatorInterface,
     DumperInterface,
     MergeInterface,
+    OwlInterface,
 ):
     """
     Simple OBO-file backed implementation
 
     This implementation is incomplete and is intended primarily as a Patcher implementation
 
     This can be abandoned when pronto is less strict
@@ -193,17 +205,29 @@
         n = 0
         entities = list(self.entities(filter_obsoletes=False))
         for s in entities:
             t = self._stanza(s, strict=False)
             if t is None:
                 # alt_ids
                 continue
+            is_relation = t.type == "Typedef"
             for v in t.simple_values(TAG_IS_A):
                 n += 1
-                yield s, IS_A, v
+                if is_relation:
+                    yield s, SUBPROPERTY_OF, self.map_shorthand_to_curie(v)
+                else:
+                    yield s, IS_A, v
+            for tag, prop in [
+                (TAG_INVERSE_OF, INVERSE_OF),
+                (TAG_DOMAIN, RDFS_DOMAIN),
+                (TAG_RANGE, RDFS_RANGE),
+            ]:
+                for v in t.simple_values(tag):
+                    n += 1
+                    yield s, prop, self.map_shorthand_to_curie(v)
             for v in t.simple_values(TAG_EQUIVALENT_TO):
                 n += 1
                 yield s, EQUIVALENT_CLASS, v
                 yield v, EQUIVALENT_CLASS, s
             for p, v in t.pair_values(TAG_RELATIONSHIP):
                 yield s, self.map_shorthand_to_curie(p), v
             # for p, v in t.intersection_of_tuples():
@@ -218,14 +242,18 @@
                     yield ldef.definedClassId, IS_A, p
                     n += 1
                 for r in ldef.restrictions:
                     yield ldef.definedClassId, r.propertyId, r.fillerId
                     n += 1
             logging.info(f"Relaxed {n} relationships")
 
+    def _all_entailed_relationships(self):
+        reasoner = RelationGraphReasoner(self)
+        yield from reasoner.entailed_edges()
+
     def entities(self, filter_obsoletes=True, owl_type=None) -> Iterable[CURIE]:
         od = self.obo_document
         for s_id, s in od.stanzas.items():
             if filter_obsoletes:
                 if s.get_boolean_value(TAG_IS_OBSOLETE):
                     continue
             if (
@@ -477,24 +505,22 @@
         predicates: List[PRED_CURIE] = None,
         objects: List[CURIE] = None,
         include_tbox: bool = True,
         include_abox: bool = True,
         include_entailed: bool = False,
         exclude_blank: bool = True,
     ) -> Iterator[RELATIONSHIP]:
-        for s in self._relationship_index.keys():
-            if subjects is not None and s not in subjects:
-                continue
-            for s2, p, o in self._relationship_index[s]:
-                if s2 == s:
-                    if predicates is not None and p not in predicates:
-                        continue
-                    if objects is not None and o not in objects:
-                        continue
-                    yield s, p, o
+        ei = self.edge_index
+        if include_entailed:
+            ei = self.entailed_edge_index
+        yield from ei.edges(
+            subjects=subjects,
+            predicates=predicates,
+            objects=objects,
+        )
 
     def basic_search(self, search_term: str, config: SearchConfiguration = None) -> Iterable[CURIE]:
         # TODO: move up, avoid repeating packages
         if config is None:
             config = SearchConfiguration()
         matches = []
         mfunc = None
@@ -866,7 +892,26 @@
         if patch.contributor:
             self.add_contributors(patch.about_node, [patch.contributor])
             modified_entities.append(patch.about_node)
         for e in modified_entities:
             stanza = self._stanza(e, strict=True)
             stanza.normalize_order()
         return patch
+
+    # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+    # Implements: OwlInterface
+    # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+    def transitive_object_properties(self) -> Iterable[CURIE]:
+        od = self.obo_document
+        for s_id, s in od.stanzas.items():
+            if s.type == "Typedef":
+                if s.get_boolean_value(TAG_IS_TRANSITIVE, False):
+                    yield self.map_shorthand_to_curie(s_id)
+
+    def simple_subproperty_of_chains(self) -> Iterable[Tuple[CURIE, List[CURIE]]]:
+        od = self.obo_document
+        for s_id, s in od.stanzas.items():
+            if s.type == "Typedef":
+                for p1, p2 in s.pair_values(TAG_HOLDS_OVER_CHAIN):
+                    curie = self.map_shorthand_to_curie(s_id)
+                    yield curie, [self.map_shorthand_to_curie(p1), self.map_shorthand_to_curie(p2)]
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.5.9/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,25 @@
 TAG_UNION_OF = "union_of"
 TAG_DISJOINT_FROM = "disjoint_from"
 TAG_CREATED_BY = "created_by"
 TAG_CREATION_DATE = "creation_date"
 SYNONYM_TUPLE = Tuple[PRED_CURIE, str, Optional[str], List[CURIE]]
 PROPERTY_VALUE_TUPLE = Tuple[PRED_CURIE, str, Optional[CURIE], Optional[List[CURIE]]]
 
+TAG_IS_TRANSITIVE = "is_transitive"
+TAG_IS_SYMMETRIC = "is_symmetric"
+TAG_IS_ANTI_SYMMETRIC = "is_anti_symmetric"
+TAG_IS_REFLEXIVE = "is_reflexive"
+TAG_IS_ASYMMETRIC = "is_asymmetric"
+TAG_IS_FUNCTIONAL = "is_functional"
+TAG_IS_INVERSE_FUNCTIONAL = "is_inverse_functional"
+TAG_HOLDS_OVER_CHAIN = "holds_over_chain"
+TAG_DOMAIN = "domain"
+TAG_RANGE = "range"
+
 TERM_TAGS = [
     TAG_ID,
     # TAG_IS_ANONYMOUS,
     TAG_NAME,
     TAG_NAMESPACE,
     TAG_ALT_ID,
     TAG_DEF,
@@ -584,14 +595,15 @@
 
 @dataclass
 class OboDocument:
     """An OBO Document is a header plus zero or more stanzas"""
 
     header: Header = field(default_factory=lambda: Header())
     stanzas: Mapping[CURIE, Stanza] = field(default_factory=lambda: {})
+    curie_to_shorthand_map: Mapping[CURIE, CURIE] = field(default_factory=lambda: {})
 
     def add_stanza(self, stanza: Stanza) -> None:
         """
         Adds a stanza to the document.
 
         Ensures stanza added in order.
         :param stanza:
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,41 +532,42 @@
         return rels
 
     def _get_anns(self, curie: CURIE, pred: Union[URIRef, CURIE]):
         uri = self.curie_to_sparql(curie)
         pred = self.curie_to_sparql(pred)
         query = SparqlQuery(select=["?v"], where=[f"{uri} {pred} ?v"])
         if self.multilingual:
-            query.where.append(f'FILTER (LANG(?v) = "{self.preferred_language}")')
+            query.where.append(f'FILTER (LANG(?v) = "{self.default_language}")')
         bindings = self._sparql_query(query)
         return list(set([row[VAL_VAR]["value"] for row in bindings]))
 
     def label(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None):
         if lang:
             raise NotImplementedError("Language selection not implemented yet")
-        labels = list(self.labels([curie]))
+        labels = list(self.labels([curie], lang=lang))
         if labels:
             if len(labels) > 1:
                 logging.warning(f"Multiple labels for {curie} = {labels}")
             return labels[0][1]
         else:
             return None
 
     def labels(
         self, curies: Iterable[CURIE], allow_none=True, lang: Optional[LANGUAGE_TAG] = None
     ) -> Iterable[Tuple[CURIE, str]]:
-        if lang:
-            raise NotImplementedError("Language selection not implemented yet")
         label_uri = self._label_uri()
         uris = [self.curie_to_sparql(x) for x in curies]
         query = SparqlQuery(
             select=["?s ?label"], where=[f"?s <{label_uri}> ?label", _sparql_values("s", uris)]
         )
         if self.multilingual:
-            query.where.append(f'FILTER (LANG(?label) = "{self.preferred_language}")')
+            if not lang:
+                lang = self.default_language
+        if lang:
+            query.where.append(f'FILTER (LANG(?label) = "{lang}")')
         bindings = self._sparql_query(query)
         label_map = {}
         for row in bindings:
             curie, label = self.uri_to_curie(row["s"]["value"]), row["label"]["value"]
             if curie in label_map:
                 if label_map[curie] != label:
                     logging.warning(f"Multiple labels for {curie} = {label_map[curie]} != {label}")
@@ -574,14 +575,32 @@
                 label_map[curie] = label
                 yield curie, label
         if allow_none:
             for curie in curies:
                 if curie not in label_map:
                     yield curie, None
 
+    def multilingual_labels(
+        self, curies: Iterable[CURIE], allow_none=True, langs: Optional[List[LANGUAGE_TAG]] = None
+    ) -> Iterable[Tuple[CURIE, str, LANGUAGE_TAG]]:
+        label_uri = self._label_uri()
+        uris = [self.curie_to_sparql(x) for x in curies]
+        query = SparqlQuery(
+            select=["?s" "?label", "(LANG(?label) AS ?lang)"],
+            where=[
+                f"?s <{label_uri}> ?label",
+                _sparql_values("LANG(?label)", langs),
+                _sparql_values("s", uris),
+            ],
+        )
+        bindings = self._sparql_query(query)
+        for row in bindings:
+            curie, label = self.uri_to_curie(row["s"]["value"]), row["label"]["value"]
+            yield curie, label, row["lang"]["value"]
+
     def defined_bys(self, entities: Iterable[CURIE]) -> Iterable[str]:
         entities = list(entities)
         uris = [self.curie_to_sparql(x) for x in entities]
         query = SparqlQuery(
             select=["?s ?o"], where=[f"?s {IS_DEFINED_BY} ?o", _sparql_values("s", uris)]
         )
         bindings = self._sparql_query(query)
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.5.9/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     RdfFirstStatement,
     RdfRestStatement,
     RdfsLabelStatement,
     RdfsSubclassOfStatement,
     RdfTypeStatement,
     Statements,
     TermAssociation,
+    TransitivePropertyNode,
 )
 from sqlalchemy import and_, create_engine, delete, distinct, func, insert, text, update
 from sqlalchemy.orm import aliased, sessionmaker
 from sssom_schema import Mapping
 
 import oaklib.datamodels.ontology_metadata as om
 import oaklib.datamodels.validation_datamodel as vdm
@@ -95,14 +96,15 @@
     IS_A,
     LABEL_PREDICATE,
     OBSOLETION_RELATIONSHIP_PREDICATES,
     OWL_CLASS,
     OWL_META_CLASSES,
     OWL_NAMED_INDIVIDUAL,
     OWL_NOTHING,
+    OWL_PROPERTY_CHAIN_AXIOM,
     OWL_THING,
     OWL_VERSION_IRI,
     PREFIX_PREDICATE,
     RDF_TYPE,
     RDFS_COMMENT,
     RDFS_DOMAIN,
     RDFS_LABEL,
@@ -254,27 +256,30 @@
     OwlInterface,
     DumperInterface,
     MergeInterface,
 ):
     """
     A :class:`OntologyInterface` implementation that wraps a SQL Relational Database.
 
-    This could be a local file (accessed via SQL Lite) or a local/remote server (e.g PostgreSQL).
+    Currently this must be a SQLite database. PostgreSQL support is planned.
 
     To connect, either use SqlImplementation directly:
 
-    .. packages:: python
+    >>> from oaklib.implementations.sqldb.sql_implementation import SqlImplementation
+    >>> from oaklib.resource import OntologyResource
+    >>> adapter = SqlImplementation(OntologyResource("tests/input/go-nucleus.db"))
 
-        >>> oi = SqlImplementation(OntologyResource(slug=f"sqlite:///{path}"))
+    or
 
-    Or use a selector:
+    >>> from oaklib import get_adapter
+    >>> adapter = get_adapter("sqlite:tests/input/go-nucleus.db")
 
-    .. packages:: python
+    you can also load from the semantic-sql repository:
 
-        >>> oi = get_implementation_from_shorthand('obojson:path/to/my/ontology.db')
+    >>> adapter = get_adapter("sqlite:obo:obi")
 
     The schema is assumed to follow the `semantic-sql <https://github.com/incatools/semantic-sql>`_ schema.
 
     This uses SQLAlchemy ORM Models:
 
     - :class:`Statements`
     - :class:`Edge`
@@ -787,14 +792,18 @@
                 yield str(row.object) if row.object else str(row.value)
 
     def entailed_outgoing_relationships(
         self, curie: CURIE, predicates: List[PRED_CURIE] = None
     ) -> Iterable[Tuple[PRED_CURIE, CURIE]]:
         return self.outgoing_relationships(curie, predicates, entailed=True)
 
+    def _rebuild_relationship_index(self):
+        self._relationships_by_subject_index = None
+        self.precompute_lookups()
+
     def precompute_lookups(self) -> None:
         if self._relationships_by_subject_index is None:
             self._relationships_by_subject_index = {}
         logging.info("Precomputing lookups")
 
         def add(row):
             if not row.object:
@@ -831,14 +840,15 @@
         exclude_blank: bool = True,
         bypass_index: bool = False,
     ) -> Iterator[RELATIONSHIP]:
         if subjects is not None:
             # materialize iterators
             subjects = list(subjects)
         if subjects and not objects and self._relationships_by_subject_index:
+            # TODO: unify indexes with other implementations
             for s in subjects:
                 for _, p, o in self._relationships_by_subject_index.get(s, []):
                     if not o:
                         raise ValueError(f"No object for {s} {p}")
                     if predicates and p not in predicates:
                         continue
                     if not include_abox and p == RDF_TYPE:
@@ -1594,20 +1604,24 @@
         predicates = tuple(ALL_MATCH_PREDICATES)
         base_query = self.session.query(Statements).filter(Statements.predicate.in_(predicates))
         if curies is None:
             by_subject_query = base_query
         else:
             by_subject_query = base_query.filter(Statements.subject.in_(curies))
         for row in by_subject_query:
-            mpg = Mapping(
-                subject_id=row.subject,
-                object_id=row.value if row.value is not None else row.object,
-                predicate_id=row.predicate,
-                mapping_justification=justification,
-            )
+            try:
+                mpg = Mapping(
+                    subject_id=row.subject,
+                    object_id=row.value if row.value is not None else row.object,
+                    predicate_id=row.predicate,
+                    mapping_justification=justification,
+                )
+            except ValueError as e:
+                logging.error(f"Skipping {row}; ValueError: {e}")
+                continue
             inject_mapping_sources(mpg)
             if source and mpg.subject_source != source and mpg.object_source != source:
                 continue
             yield mpg
         if curies is None:
             # all mappings have been returned
             return
@@ -1915,14 +1929,25 @@
         q = q.filter(ee2.subject == object, ee2.object == Statements.object, ee2.predicate == IS_A)
         if q.first():
             return True
         if bidirectional:
             return self.is_disjoint(object, subject, bidirectional=False)
         return False
 
+    def transitive_object_properties(self) -> Iterable[CURIE]:
+        for row in self.session.query(TransitivePropertyNode.id):
+            yield row[0]
+
+    def simple_subproperty_of_chains(self) -> Iterable[Tuple[CURIE, List[CURIE]]]:
+        q = self.session.query(Statements)
+        q = q.filter(Statements.predicate == OWL_PROPERTY_CHAIN_AXIOM)
+        for row in q:
+            chain = list(self._rdf_list(row.object))
+            yield row.subject, chain
+
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     # Implements: SemSim
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
     def information_content_scores(
         self,
         curies: Iterable[CURIE],
@@ -1971,14 +1996,16 @@
             yield OWL_THING, 0.0
 
     def all_by_all_pairwise_similarity(
         self,
         subjects: Iterable[CURIE],
         objects: Iterable[CURIE],
         predicates: List[PRED_CURIE] = None,
+        min_jaccard_similarity: Optional[float] = None,
+        min_ancestor_information_content: Optional[float] = None,
     ) -> Iterator[TermPairwiseSimilarity]:
         def tuples_to_map(
             entities: List[CURIE], relationships: Iterable[RELATIONSHIP]
         ) -> Dict[CURIE, Set[CURIE]]:
             rmap = defaultdict(set)
             for r in relationships:
                 rmap[r[0]].add(r[2])
@@ -2173,14 +2200,15 @@
             about = patch.about_edge
             if isinstance(patch, kgcl.EdgeCreation):
                 self._execute(
                     insert(Statements).values(
                         subject=patch.subject, predicate=patch.predicate, object=patch.object
                     )
                 )
+                self._rebuild_relationship_index()
                 logging.warning("entailed_edge is now stale")
             elif isinstance(patch, kgcl.EdgeDeletion):
                 self._execute(
                     delete(Statements).where(
                         and_(
                             Statements.subject == patch.subject,
                             Statements.predicate == patch.predicate,
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.5.9/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,25 @@
     See: `<https://github.com/INCATools/ubergraph>`_
 
     This is a specialization of the more generic :class:`.SparqlImplementation`, which
     has knowledge of some of the specialized patterns found in Ubergraph
 
     An UbergraphImplementation can be initialed by:
 
-        .. packages:: python
+    >>> from oaklib.implementations.ubergraph.ubergraph_implementation import UbergraphImplementation
+    >>> adapter = UbergraphImplementation()
 
-           >>>  oi = UbergraphImplementation()
+    or
 
-        The default ubergraph endpoint will be assumed
+    >>> from oaklib import get_adapter
+    >>> adapter = get_adapter("ubergraph:")
+
+    to use a specific ontology or named graph within ubergraph:
+
+    >>> adapter = get_adapter("ubergraph:cl")
 
     """
 
     def _default_url(self) -> str:
         return "https://ubergraph.apps.renci.org/sparql"
 
     def _is_blazegraph(self) -> bool:
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files 20% similar despite different names*

```diff
@@ -80,17 +80,21 @@
     Wraps the Uniprot sparql endpoint.
 
     This is a specialization of the more generic :class:`.SparqlImplementation`, which
     has knowledge of some of the specialized patterns found in Uniprot
 
     An UniprotImplementation can be initialed by:
 
-        .. packages:: python
+    >>> from oaklib.implementations.uniprot.uniprot_implementation import UniprotImplementation
+    >>> adapter = UniprotImplementation()
 
-           >>>  oi = UniprotImplementation()
+    or
+
+    >>> from oaklib import get_adapter
+    >>> adapter = get_adapter("uniprot:")
 
     The default Uniprot endpoint will be assumed
 
     """
 
     def _default_url(self) -> str:
         return "https://sparql.uniprot.org/sparql"
@@ -194,25 +198,34 @@
         predicate_closure_predicates: Optional[List[PRED_CURIE]] = None,
         object_closure_predicates: Optional[List[PRED_CURIE]] = None,
         include_modified: bool = False,
     ) -> Iterator[Association]:
         """
         Uniprot implementation of :ref:`associations`
 
-        To query for all associations for a protein:
+        To query for some associations for a protein:
 
-            >>> for assoc in oi.associations(["UniProtKB:Q62226"]):
-            >>>     print(assoc)
+        >>> import itertools
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("uniprot:")
+        >>> # for demo purposes we pick the first N
+        >>> for assoc in itertools.islice(adapter.associations(["UniProtKB:Q62226"]), 5):
+        ...     print(assoc.subject, assoc.predicate, assoc.object)
+        <BLANKLINE>
+        UniProtKB:Q62226 up:classifiedWith GO:...
+        ...
 
         To query for all associations to a keyword, including closures
 
-            >>> for assoc in oi.associations(
-            >>>         objects=["UniProtKB-KW:9993"],
-            >>>         object_closure_predicates=[IS_A]):
-            >>>     print(assoc)
+        >>> from oaklib.datamodels.vocabulary import IS_A
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("uniprot:")
+        >>> assocs = adapter.associations(
+        ...         objects=["UniProtKB-KW:9993"],
+        ...         object_closure_predicates=[IS_A])
 
         Note: this may be slow
 
         :param subjects: typically Uniprot entries
         :param predicates: defaults to up:classifiedWith
         :param objects: can be GO, EC, KW, ...
         :param property_filter: not implemented
```

### Comparing `oaklib-0.5.8/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.5.9/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,23 @@
     See: `<https://github.com/INCATools/wikidata>`_
 
     This is a specialization of the more generic :class:`.SparqlImplementation`, which
     has knowledge of some of the specialized patterns found in wikidata
 
     An wikidataImplementation can be initialed by:
 
-        .. packages:: python
+    >>> from oaklib.implementations.wikidata.wikidata_implementation import WikidataImplementation
+    >>> adapter = WikidataImplementation()
 
-           >>>  oi = WikidataImplementation.create()
+    or
 
-        The default wikidata endpoint will be assumed
+    >>> from oaklib import get_adapter
+    >>> adapter = get_adapter("wikidata:")
+
+    The default wikidata endpoint will be assumed
 
     """
 
     wikidata_curie_map: Dict[str, str] = field(default_factory=lambda: DEFAULT_CURIE_MAP)
 
     def __post_init__(self):
         super().__post_init__()
```

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/__init__.py` & `oaklib-0.5.9/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/association_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 import logging
 from abc import ABC
 from collections import defaultdict
 from dataclasses import dataclass, field
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, Iterable, Iterator, List, Mapping, Optional, Tuple, Union
@@ -20,18 +21,20 @@
     OBSOLETION_RELATIONSHIP_PREDICATES,
     OWL_CLASS,
     OWL_NOTHING,
     OWL_THING,
     PREFIX_PREDICATE,
     URL_PREDICATE,
 )
+from oaklib.indexes.edge_index import EdgeIndex
 from oaklib.interfaces.ontology_interface import OntologyInterface
 from oaklib.mappers.ontology_metadata_mapper import OntologyMetadataMapper
 from oaklib.types import CATEGORY_CURIE, CURIE, PRED_CURIE, SUBSET_CURIE, URI
 from oaklib.utilities.basic_utils import get_curie_prefix, pairs_as_dict
+from oaklib.utilities.iterator_utils import chunk
 
 LANGUAGE_TAG = str
 NC_NAME = str
 PREFIX_MAP = Mapping[NC_NAME, URI]
 RELATIONSHIP_MAP = Dict[PRED_CURIE, List[CURIE]]
 ALIAS_MAP = Dict[PRED_CURIE, List[str]]
 METADATA_MAP = Dict[PRED_CURIE, List[str]]
@@ -151,14 +154,17 @@
 
     auto_relax_axioms: bool = None
     """If True, relax some OWL axioms as per https://robot.obolibrary.org/relax"""
 
     cache_lookups: bool = False
     """If True, the implementation may choose to cache lookup operations"""
 
+    _edge_index: Optional[EdgeIndex] = None
+    _entailed_edge_index: Optional[EdgeIndex] = None
+
     def prefix_map(self) -> PREFIX_MAP:
         """
         Return a dictionary mapping all prefixes known to the resource to their URI expansion.
 
         >>> from oaklib import get_adapter
         >>> adapter = get_adapter('tests/input/go-nucleus.db')
         >>> for prefix, expansion in adapter.prefix_map().items():
@@ -270,31 +276,74 @@
                 f"This ontology interface contains {len(self.prefix_map()):,} prefixes:\n{prefix_map_text}"
             )
         if rv is None and use_uri_fallback:
             return uri
         return rv
 
     @property
+    def edge_index(self) -> EdgeIndex:
+        """
+        An index of all asserted edges in the ontology.
+
+        .. note::
+
+            not all adapters populate this index.
+
+        :return: index of edges
+        """
+        if self._edge_index is None:
+            self._edge_index = EdgeIndex(lambda: self._all_relationships())
+        return self._edge_index
+
+    @property
+    def entailed_edge_index(self) -> EdgeIndex:
+        """
+        An index of all entailed edges in the ontology.
+
+        .. note::
+
+            not all adapters populate this index.
+
+        :return: index of entailed edges
+        """
+        if self._entailed_edge_index is None:
+            self._entailed_edge_index = EdgeIndex(lambda: self._all_entailed_relationships())
+        return self._entailed_edge_index
+
+    def _all_entailed_relationships(self):
+        raise NotImplementedError("This adapter does not support entailed relationships")
+
+    @property
     def _relationship_index(self) -> Dict[CURIE, List[RELATIONSHIP]]:
+        """
+        An index of relationships keyed by either subject or object.
+
+        The first time this is called, it will build the index.
+        Subsequent calls will return the cached index.
+
+        :return: dictionary mapping subject or object to list of relationships
+        """
         if self._relationship_index_cache:
             return self._relationship_index_cache
-        logging.info("Building relationship")
+        logging.info("Building relationship index")
         ix = defaultdict(list)
         for rel in self._all_relationships():
             s, p, o = rel
             ix[s].append(rel)
             ix[o].append(rel)
         self._relationship_index_cache = ix
         return self._relationship_index_cache
 
     def _rebuild_relationship_index(self):
         self._relationship_index_cache = None
+        self._edge_index = None
         _ = self._relationship_index  # force re-index
 
     def _clear_relationship_index(self):
+        self._edge_index = None
         self._relationship_index_cache = None
 
     def _all_relationships(self) -> Iterator[RELATIONSHIP]:
         raise NotImplementedError
 
     @property
     def multilingual(self) -> bool:
@@ -478,14 +527,57 @@
                     for val in vals:
                         yield entity, prop, val
 
     @deprecated("Replaced by obsoletes()")
     def all_obsolete_curies(self) -> Iterable[CURIE]:
         return self.obsoletes()
 
+    def dangling(self, curies: Optional[Iterable[CURIE]] = None) -> Iterable[CURIE]:
+        """
+        Yields all known entities in provided set that are dangling.
+
+        Example:
+
+        This example is over an OBO file with one stanza:
+
+        .. code-block:: obo
+
+            [Term]
+            id: GO:0012505
+            name: endomembrane system
+            is_a: GO:0110165 ! cellular anatomical entity
+            relationship: has_part GO:0005773 ! vacuole
+
+        The two edges point to entities that do not exist in the file.
+
+        The following code will show these:
+
+        >>> from oaklib import get_adapter
+        >>> # Note: pronto adapter refuses to parse ontology files with dangling
+        >>> adapter = get_adapter("simpleobo:tests/input/dangling-node-test.obo")
+        >>> for entity in sorted(adapter.dangling()):
+        ...     print(entity)
+        GO:0005773
+        GO:0110165
+
+        :param curies: CURIEs to check for dangling; if empty will check all
+        :return: iterator over CURIEs
+        """
+        if curies is None:
+            curies = self.entities(filter_obsoletes=False)
+            curies = itertools.chain(curies, {rel[2] for rel in self.relationships()})
+        for curie_it in chunk(curies):
+            chunked_curies = list(curie_it)
+            logging.debug(f"Checking {len(chunked_curies)} curies for dangling")
+            curie_labels = self.labels(chunked_curies, allow_none=True)
+            candidates = [curie for curie, label in curie_labels if label is None]
+            exclude = {rel[0] for rel in self.relationships(candidates)}
+            logging.debug(f"Candidates {len(candidates)} exclude: {len(exclude)}")
+            yield from [curie for curie in candidates if curie not in exclude]
+
     def ontology_versions(self, ontology: CURIE) -> Iterable[str]:
         """
         Yields all version identifiers for an ontology.
 
         .. warning ::
 
             This method is not yet implemented for all OntologyInterface implementations.
```

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/embedding_provider_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/embedding_provider_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,16 +22,11 @@
     def entities_vectors(
         self,
         entities: Iterable[CURIE],
     ) -> Iterable[ENTITY_EMBEDDING]:
         """
         Generate embeddings.
 
-        >>> from oaklib import get_adapter
-        >>> adapter = get_adapter("go.db")
-        >>> for entity, _text, embedding in adapter.entities_vectors():
-        >>>     print(entity)
-
         :param entities: A collection of entities to generate embeddings for.
         :yield: A generator function that yields embedding vectors.
         """
         raise NotImplementedError
```

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/obograph_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 from abc import ABC
 from collections import defaultdict
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union
 
+from sssom.constants import RDFS_SUBCLASS_OF, RDFS_SUBPROPERTY_OF
+
 from oaklib.datamodels.obograph import (
     Edge,
     Graph,
     LogicalDefinitionAxiom,
     Node,
     SynonymPropertyValue,
 )
@@ -198,15 +200,17 @@
         )
         if self.transitive_query_cache is not None:
             if key in self.transitive_query_cache:
                 return self.transitive_query_cache[key]
         # this implements a traversal approach that iteratively walks up the graph;
         # this may be inefficient. It is recommended that different implementations
         # override this with a more efficient method that leverages cached tables
-        logging.info(f"Computing ancestor graph for {start_curies} using graph walking")
+        logging.info(
+            f"Computing ancestor graph for {start_curies} / {predicates} using graph walking"
+        )
         g = self._graph(walk_up(self, start_curies, predicates=predicates))
         if self.transitive_query_cache is not None:
             self.transitive_query_cache[key] = g
         return g
 
     def descendant_graph(
         self, start_curies: Union[CURIE, List[CURIE]], predicates: List[PRED_CURIE] = None
@@ -249,18 +253,27 @@
         :param start_curies: curie or curies to start the walk from
         :param predicates: only traverse over these (traverses over all if this is not set)
         :param reflexive: include self
         :param method:
         :return: all ancestor CURIEs
         """
         if method and method == GraphTraversalMethod.ENTAILMENT:
-            raise NotImplementedError(f"entailment method not implemented in {type(self)}")
-        return _edges_to_nodes(
-            start_curies, self.ancestor_graph(start_curies, predicates).edges, reflexive
-        )
+            if isinstance(start_curies, str):
+                start_curies = [start_curies]
+            yielded = set()
+            for rel in self.relationships(
+                start_curies, predicates=predicates, include_entailed=True
+            ):
+                o = rel[2]
+                if o not in yielded:
+                    yield o
+                    yielded.add(o)
+        else:
+            g = self.ancestor_graph(start_curies, predicates).edges
+            yield from _edges_to_nodes(start_curies, g, reflexive)
 
     def descendants(
         self,
         start_curies: Union[CURIE, List[CURIE]],
         predicates: List[PRED_CURIE] = None,
         reflexive=True,
         method: Optional[GraphTraversalMethod] = None,
@@ -276,18 +289,27 @@
         :param start_curies: curie or curies to start the walk from
         :param predicates: only traverse over these (traverses over all if this is not set)
         :param reflexive: include self
         :param method:
         :return: all descendant CURIEs
         """
         if method and method == GraphTraversalMethod.ENTAILMENT:
-            raise NotImplementedError(f"entailment method not implemented in {type(self)}")
-        return _edges_to_nodes(
-            start_curies, self.descendant_graph(start_curies, predicates).edges, reflexive
-        )
+            if isinstance(start_curies, str):
+                start_curies = [start_curies]
+            yielded = set()
+            for rel in self.relationships(
+                objects=start_curies, predicates=predicates, include_entailed=True
+            ):
+                s = rel[0]
+                if s not in yielded:
+                    yield s
+                    yielded.add(s)
+        else:
+            g = self.descendant_graph(start_curies, predicates).edges
+            yield from _edges_to_nodes(start_curies, g, reflexive)
 
     def descendant_count(
         self,
         start_curies: Union[CURIE, List[CURIE]],
         predicates: List[PRED_CURIE] = None,
         reflexive=True,
     ) -> int:
@@ -369,29 +391,37 @@
         :param dangling: if true, include dangling nodes
         :return: subgraph
         """
         logging.info(f"Extracting using seed of {len(entities)} entities")
         nodes = [self.node(e, include_metadata=include_metadata) for e in entities]
         edges = []
         logging.info(f"extracting rels for {len(entities)} p={predicates} dangling={dangling}")
+        used_predicates = set()
         for s, p, o in self.relationships(subjects=entities, predicates=predicates):
             if dangling or o in entities:
                 edges.append(Edge(sub=s, pred=p, obj=o))
+                if p not in [RDFS_SUBCLASS_OF, RDFS_SUBPROPERTY_OF]:
+                    used_predicates.add(p)
         ontologies = list(self.ontologies())
         curr_id = ontologies[0]
         g = Graph(id=f"{curr_id}-transformed", nodes=nodes, edges=edges)
         for lda in self.logical_definitions(entities):
             if predicates:
                 if any(r for r in lda.restrictions if r.propertyId not in predicates):
                     continue
             if not dangling:
                 signature = set(lda.genusIds + [r.fillerId for r in lda.restrictions])
                 if signature.difference(entities):
                     continue
             g.logicalDefinitionAxioms.append(lda)
+            for r in lda.restrictions:
+                used_predicates.add(r.propertyId)
+        logging.info(f"Used predicates = {used_predicates}")
+        pred_nodes = [self.node(e, include_metadata=include_metadata) for e in used_predicates]
+        g.nodes.extend([n for n in pred_nodes if n])
         return g
 
     def relationships_to_graph(self, relationships: Iterable[RELATIONSHIP]) -> Graph:
         """
         Generates an OboGraph from a list of relationships
 
         :param relationships:
```

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/owl_interface.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,30 +6,44 @@
 from typing import Any, Callable, Iterable, List, Optional, Tuple, Type, Union
 
 # TODO: add funowl to dependencies
 import funowl
 from funowl import (
     IRI,
     AnnotationAssertion,
+    AsymmetricObjectProperty,
     Axiom,
     Class,
     ClassExpression,
     DisjointClasses,
     EquivalentClasses,
+    IrreflexiveObjectProperty,
     Literal,
     ObjectAllValuesFrom,
     ObjectIntersectionOf,
+    ObjectPropertyChain,
     ObjectPropertyExpression,
     ObjectSomeValuesFrom,
     ObjectUnionOf,
     Ontology,
+    ReflexiveObjectProperty,
     SubClassOf,
+    SubObjectPropertyOf,
+    SymmetricObjectProperty,
+    TransitiveObjectProperty,
 )
 from funowl.writers import FunctionalWriter
 
+from oaklib.datamodels.vocabulary import (
+    OWL_ASYMMETRIC_PROPERTY,
+    OWL_IRREFLEXIVE_PROPERTY,
+    OWL_REFLEXIVE_PROPERTY,
+    OWL_SYMMETRIC_PROPERTY,
+    OWL_TRANSITIVE_PROPERTY,
+)
 from oaklib.interfaces.basic_ontology_interface import BasicOntologyInterface
 from oaklib.types import CURIE
 
 
 class OwlProfile(Enum):
     EL = "EL"
     DL = "DL"
@@ -47,14 +61,15 @@
 
 @dataclass
 class AxiomFilter:
     type: Optional[Type[Axiom]] = None
     about: Optional[Union[CURIE, List[CURIE]]] = None
     references: Optional[CURIE] = None
     func: Callable = None
+    ontologies: Optional[List[CURIE]] = None
 
     def set_type(self, axiom_type: Union[str, Type[Axiom]]) -> None:
         if isinstance(axiom_type, str):
             matches = [obj for n, obj in inspect.getmembers(funowl) if n == axiom_type]
             if len(matches) == 1:
                 self.type = matches[0]
             elif len(matches) == 0:
@@ -323,7 +338,56 @@
 
     def _axiom_references_curies(self, axiom: Axiom) -> Iterable[CURIE]:
         for e in self.axiom_references(axiom):
             yield self.entity_iri_to_curie(e)
 
     def _axiom_is_about_curies(self, axiom: Axiom) -> List[CURIE]:
         return [self.entity_iri_to_curie(e) for e in self.axiom_is_about(axiom)]
+
+    def property_characteristics(self, property: CURIE) -> Iterable[CURIE]:
+        """
+        Gets all property characteristics for a given property
+
+        :param property:
+        :return:
+        """
+        pc_tuples = [
+            (TransitiveObjectProperty, OWL_TRANSITIVE_PROPERTY),
+            (SymmetricObjectProperty, OWL_SYMMETRIC_PROPERTY),
+            (AsymmetricObjectProperty, OWL_ASYMMETRIC_PROPERTY),
+            (ReflexiveObjectProperty, OWL_REFLEXIVE_PROPERTY),
+            (IrreflexiveObjectProperty, OWL_IRREFLEXIVE_PROPERTY),
+        ]
+        pcs = tuple([pc[0] for pc in pc_tuples])
+        for axiom in self.axioms():
+            if isinstance(axiom, pcs):
+                for pc, pc_curie in pc_tuples:
+                    if isinstance(axiom, pc):
+                        if isinstance(axiom.objectPropertyExpression, IRI):
+                            if self.entity_iri_to_curie(axiom.objectPropertyExpression) == property:
+                                yield pc_curie
+
+    def transitive_object_properties(self) -> Iterable[CURIE]:
+        """
+        Gets all transitive object properties
+
+        :return:
+        """
+        for axiom in self.axioms():
+            if isinstance(axiom, TransitiveObjectProperty):
+                if isinstance(axiom.objectPropertyExpression, IRI):
+                    yield self.entity_iri_to_curie(axiom.objectPropertyExpression)
+
+    def simple_subproperty_of_chains(self) -> Iterable[Tuple[CURIE, List[CURIE]]]:
+        """
+        Gets all property chains of where the super property is a chain of IRIs
+
+        :return:
+        """
+        for axiom in self.axioms():
+            if isinstance(axiom, SubObjectPropertyOf):
+                if isinstance(axiom.superObjectPropertyExpression, ObjectPropertyChain):
+                    if isinstance(axiom.subObjectPropertyExpression, IRI):
+                        chain_exprs = axiom.superObjectPropertyExpression.objectPropertyExpressions
+                        if all(isinstance(p, IRI) for p in chain_exprs):
+                            chain = [self.entity_iri_to_curie(p) for p in chain_exprs]
+                            yield self.entity_iri_to_curie(axiom.subObjectPropertyExpression), chain
```

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 
 from oaklib.interfaces.basic_ontology_interface import BasicOntologyInterface
 from oaklib.types import CURIE, PRED_CURIE
 
 
 class RelationGraphInterface(BasicOntologyInterface, ABC):
     """
-    an interface that provides relation graph abstractions
+    An interface that provides relation graph abstractions.
 
     .. note ::
 
-        that the operations provided here are similar to the graph-walking
-        operations provided in :class:`.OboGraphInterface`.
-        The main difference is that a RG provides a more restricted
-        and formally correct set of entailments.
+        this interface is now largely subsumed into the BasicOntologyInterface
     """
 
     def entailed_outgoing_relationships(
         self, curie: CURIE, predicates: List[PRED_CURIE] = None
     ) -> Iterable[Tuple[PRED_CURIE, CURIE]]:
         """
         The return relationship map is keyed by relationship type, where the values
```

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/search_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/semsim_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,23 +216,27 @@
     def pairwise_similarity(
         self,
         subject: CURIE,
         object: CURIE,
         predicates: List[PRED_CURIE] = None,
         subject_ancestors: List[CURIE] = None,
         object_ancestors: List[CURIE] = None,
+        min_jaccard_similarity: Optional[float] = None,
+        min_ancestor_information_content: Optional[float] = None,
     ) -> TermPairwiseSimilarity:
         """
         Pairwise similarity between a pair of ontology terms
 
         :param subject:
         :param object:
         :param predicates:
         :param subject_ancestors: optional pre-generated ancestor list
         :param object_ancestors: optional pre-generated ancestor list
+        :param min_jaccard_similarity: minimum Jaccard similarity for a pair to be considered
+        :param min_ancestor_information_content: minimum IC for a common ancestor to be considered
         :return:
         """
         logging.info(f"Calculating pairwise similarity for {subject} x {object} over {predicates}")
         cas = list(
             self.common_ancestors(
                 subject,
                 object,
@@ -341,20 +345,30 @@
         return sim
 
     def all_by_all_pairwise_similarity(
         self,
         subjects: Iterable[CURIE],
         objects: Iterable[CURIE],
         predicates: List[PRED_CURIE] = None,
+        min_jaccard_similarity: Optional[float] = None,
+        min_ancestor_information_content: Optional[float] = None,
     ) -> Iterator[TermPairwiseSimilarity]:
         """
         Compute similarity for all combinations of terms in subsets vs all terms in objects
 
         :param subjects:
         :param objects:
         :param predicates:
         :return:
         """
         objects = list(objects)
         for s in subjects:
             for o in objects:
-                yield self.pairwise_similarity(s, o, predicates=predicates)
+                val = self.pairwise_similarity(
+                    s,
+                    o,
+                    predicates=predicates,
+                    min_jaccard_similarity=min_jaccard_similarity,
+                    min_ancestor_information_content=min_ancestor_information_content,
+                )
+                if val:
+                    yield val
```

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,19 +54,26 @@
     to build a simple textual index from an ontology, using all labels and synonyms, and to perform
     simple string matching.
 
     Adapters that talk to a remote endpoint may leverage more advanced strategies, and may obviate
     the need for a local indexing step. For example, the :ref:`bioportal_implementation` will use
     the OntoPortal annotate endpoint which is pre-indexed over all >1000 ontologies in bioportal.
 
-
-
     All return payloads conform to the `TextAnnotation` data model:
 
      - `<https://w3id.org/oak/text-annotator>`_
+
+    Additional plugins may be available to provide more advanced functionality:
+
+    - `OAK SciSpacy plugin <https://pypi.org/project/oakx-spacy/>`_ - provides a Spacy pipeline component
+    - `OAK OGER plugin <https://pypi.org/project/oakx-oger/>`_ - provides a OGER pipeline component
+
+    For more advanced extraction use cases, see:
+
+    - `OntoGPT <https://github.com/monarch-initiative/ontogpt>`_ - LLM-based NER and schema extraction
     """
 
     lexical_index: Optional[LexicalIndex] = None
     """If present, some implementations may choose to use this"""
 
     cache_directory: Optional[str] = None
     """If present, some implementations may choose to cache any ontology indexes here.
@@ -82,17 +89,20 @@
         text: TEXT,
         configuration: Optional[TextAnnotationConfiguration] = None,
     ) -> Iterable[TextAnnotation]:
         """
         Annotate a piece of text.
 
         >>> from oaklib import get_adapter
-        >>> adapter = get_adapter("go.db")
-        >>> for annotation in adapter.annotate_text("The mitochondrion is a membrane-bound organelle"):
-        >>>     print(annotation)
+        >>> adapter = get_adapter("tests/input/go-nucleus.obo")
+        >>> for annotation in adapter.annotate_text("The nucleus is a organelle with a membrane"):
+        ...     print(annotation.object_id, annotation.object_label, annotation.subject_start, annotation.subject_end)
+        GO:0005634 nucleus 5 11
+        GO:0016020 membrane 35 42
+        GO:0043226 organelle 18 26
 
         :param text: Text to be annotated.
         :param configuration: Text annotation configuration.
         :yield: A generator function that yields annotated results.
         """
         if not configuration:
             configuration = TextAnnotationConfiguration()
```

### Comparing `oaklib-0.5.8/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.5.9/src/oaklib/interfaces/validator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/heatmap_writer.py` & `oaklib-0.5.9/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/html_writer.py` & `oaklib-0.5.9/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/obograph_writer.py` & `oaklib-0.5.9/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.5.9/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_csv_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.5.9/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/mappers/base_mapper.py` & `oaklib-0.5.9/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.5.9/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/__init__.py` & `oaklib-0.5.9/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/association_parser.py` & `oaklib-0.5.9/src/oaklib/parsers/association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.5.9/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.5.9/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.5.9/src/oaklib/parsers/gaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/gencc_association_parser.py` & `oaklib-0.5.9/src/oaklib/parsers/gencc_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.5.9/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.5.9/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.5.9/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/mim2gene_association_parser.py` & `oaklib-0.5.9/src/oaklib/parsers/mim2gene_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.5.9/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/parser_base.py` & `oaklib-0.5.9/src/oaklib/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.5.9/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.5.9/src/oaklib/parsers/xaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/resource.py` & `oaklib-0.5.9/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/selector.py` & `oaklib-0.5.9/src/oaklib/selector.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.5.9/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.5.9/src/oaklib/utilities/associations/association_differ.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.5.9/src/oaklib/utilities/associations/association_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/basic_utils.py` & `oaklib-0.5.9/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.5.9/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.5.9/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,20 +70,17 @@
     :param predicates: Predicates of interest.
     :return:
     """
     if isinstance(start_curies, CURIE):
         next_curies = [start_curies]
     else:
         next_curies = copy(start_curies)  # do not mutate
-    rels = []
     visited = copy(next_curies)
     while len(next_curies) > 0:
         next_curie = next_curies.pop()
         for pred, subjects in oi.incoming_relationship_map(next_curie).items():
             if not predicates or pred in predicates:
                 for subject in subjects:
                     if subject not in visited:
                         next_curies.append(subject)
                         visited.append(subject)
-                    rels.append((subject, pred, next_curie))
-    for rel in rels:
-        yield rel
+                    yield subject, pred, next_curie
```

### Comparing `oaklib-0.5.8/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.5.9/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.5.9/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.5.9/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/label_utilities.py` & `oaklib-0.5.9/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.5.9/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 )
 from oaklib.datamodels.mapping_rules_datamodel import (
     MappingRuleCollection,
     Precondition,
     Synonymizer,
 )
 from oaklib.datamodels.vocabulary import (
+    IDENTIFIER_PREDICATE,
     SEMAPV,
     SKOS_BROAD_MATCH,
     SKOS_CLOSE_MATCH,
     SKOS_EXACT_MATCH,
     SKOS_NARROW_MATCH,
 )
 from oaklib.interfaces import BasicOntologyInterface
@@ -111,21 +112,34 @@
         if synonym_rules:
             steps.append(
                 LexicalTransformation(TransformationType.Synonymization, params=synonym_rules)
             )
         pipelines = [LexicalTransformationPipeline(name="default", transformations=steps)]
     logging.info(f"Creating lexical index, pipelines={pipelines}")
     ix = LexicalIndex(pipelines={p.name: p for p in pipelines})
+
+    def _invert_mapping_pred(mapping_pred: PRED_CURIE) -> PRED_CURIE:
+        return f"{mapping_pred}-INVERSE"
+
+    logging.info("Creating mapping index")
+    mapping_pairs_by_curie = defaultdict(list)
+    for curie in oi.entities():
+        pairs = list(oi.simple_mappings_by_curie(curie))
+        for pred, object_id in pairs:
+            mapping_pairs_by_curie[curie].append((pred, object_id))
+            mapping_pairs_by_curie[object_id].append((_invert_mapping_pred(pred), curie))
+            mapping_pairs_by_curie[curie].append((IDENTIFIER_PREDICATE, curie))
+    logging.info(f"Created mapping index; {len(mapping_pairs_by_curie)} mappings")
     for curie in oi.entities():
         logging.debug(f"Indexing {curie}")
         if not URIorCURIE.is_valid(curie):
             logging.warning(f"Skipping {curie} as it is not a valid CURIE")
             continue
         alias_map = oi.entity_alias_map(curie)
-        mapping_map = pairs_as_dict(oi.simple_mappings_by_curie(curie))
+        mapping_map = pairs_as_dict(mapping_pairs_by_curie.get(curie, []))
         for pred, terms in {**alias_map, **mapping_map}.items():
             for term in terms:
                 if not term:
                     logging.debug(f"No term for {curie}.{pred} (expected for aggregator interface)")
                     continue
 
                 for pipeline in pipelines:
@@ -255,31 +269,44 @@
     if subjects:
         subjects = set(subjects)
     if objects:
         objects = set(objects)
     if subjects and objects and subjects != objects:
         symmetric = True
         logging.info("Forcing symmetric comparison")
+    logging.info(f"Iterating over {len(lexical_index.groupings)} groupings")
     for term, grouping in lexical_index.groupings.items():
         # elements = set([r.element for r in grouping.relationships])
         elementmap = defaultdict(list)
         for r in grouping.relationships:
             elementmap[r.element].append(r)
         if len(elementmap.keys()) < 2:
             continue
+        logging.debug(f"Processing {term} with {len(elementmap.keys())} elements")
         for e1 in elementmap:
             for e2 in elementmap:
                 for r1 in elementmap[e1]:
                     if subjects and r1.element not in subjects:
                         continue
                     for r2 in elementmap[e2]:
                         if objects and r2.element not in objects:
                             continue
                         if symmetric or r1.element < r2.element:
-                            mappings.append(inferred_mapping(oi, term, r1, r2, ruleset=ruleset))
+                            mapping = inferred_mapping(oi, term, r1, r2, ruleset=ruleset)
+                            if (
+                                ruleset
+                                and ruleset.minimum_confidence is not None
+                                and mapping.confidence < ruleset.minimum_confidence
+                            ):
+                                logging.debug(
+                                    "Skipping low confidence mapping:"
+                                    f"{mapping.confidence} < {ruleset.minimum_confidence}"
+                                )
+                                continue
+                            mappings.append(mapping)
 
         # for r1 in grouping.relationships:
         #    for r2 in grouping.relationships:
         #        if r1.element < r2.element:
         #            mappings.append(create_mapping(oi, term, r1, r2))
     logging.info("Done creating SSSOM mappings")
```

### Comparing `oaklib-0.5.8/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.5.9/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.5.9/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.5.9/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.5.9/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.5.9/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.5.9/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.5.9/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.5.9/src/oaklib/utilities/obograph_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterator, List, Optional, TextIO, Tuple, Union
 
 import networkx as nx
 import yaml
 from curies import Converter
 from linkml_runtime.dumpers import json_dumper
+from linkml_runtime.loaders import json_loader
 
 # https://stackoverflow.com/questions/6028000/how-to-read-a-static-file-from-inside-a-python-package
 from oaklib import conf as conf_package
 from oaklib.datamodels.obograph import Edge, Graph, GraphDocument, Node
 from oaklib.datamodels.vocabulary import IS_A, PART_OF, RDF_TYPE
 from oaklib.types import CURIE, PRED_CURIE
 
@@ -41,14 +42,24 @@
 
 
 class TreeFormatEnum(Enum):
     markdown = "md"
     text = "text"
 
 
+def load_obograph_document(path: str) -> GraphDocument:
+    """
+    Load an OBOGraph document from a file
+
+    :param path:
+    :return:
+    """
+    return json_loader.load(str(path), target_class=GraphDocument)
+
+
 def default_stylemap_path():
     conf_path = os.path.dirname(conf_package.__file__)
     return str(Path(conf_path) / DEFAULT_STYLEMAP)
 
 
 def graph_as_dict(graph: Graph) -> Dict[str, Any]:
     """
```

### Comparing `oaklib-0.5.8/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.5.9/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.5.9/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.5.9/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.5.9/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.5.9/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.5.9/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.5.9/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     AnonymousEnumExpression,
     EnumExpression,
     SchemaDefinition,
 )
 from linkml_runtime.loaders import yaml_loader
 from ruamel.yaml import YAML
 
-from oaklib import get_implementation_from_shorthand
+from oaklib import get_adapter
 from oaklib.datamodels.search import SearchConfiguration
 from oaklib.datamodels.search_datamodel import SearchProperty, SearchTermSyntax
 from oaklib.datamodels.value_set_configuration import Resolver, ValueSetConfiguration
 from oaklib.datamodels.vocabulary import IS_A
 from oaklib.interfaces import SearchInterface
 from oaklib.interfaces.basic_ontology_interface import BasicOntologyInterface
 from oaklib.interfaces.obograph_interface import OboGraphInterface
@@ -168,15 +168,15 @@
         if resolver:
             if resolver.shorthand_prefix:
                 shorthand = f"{resolver.shorthand_prefix}:{local_name}"
             elif resolver.shorthand:
                 shorthand = resolver.shorthand
             else:
                 raise ValueError(f"Invalid resolver configuration: {resolver}")
-            return get_implementation_from_shorthand(shorthand)
+            return get_adapter(shorthand)
         else:
             raise ValueError(f"Don't know how to resolve: {ontology_id}")
 
     def _generate_permissible_value(
         self,
         curie: CURIE,
         oi: BasicOntologyInterface,
```

### Comparing `oaklib-0.5.8/src/oaklib/utilities/table_filler.py` & `oaklib-0.5.9/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.5.9/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.5.9/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.5.9/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.5.9/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.5.9/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.5.9/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.8/PKG-INFO` & `oaklib-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.5.8
+Version: 0.5.9
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -34,15 +34,15 @@
 Requires-Dist: ontoportal-client (>=0.0.3)
 Requires-Dist: prefixmaps (>=0.1.2)
 Requires-Dist: pronto (>=2.5.0)
 Requires-Dist: pysolr (>=3.9.0,<4.0.0)
 Requires-Dist: pystow (>=0.5.0)
 Requires-Dist: ratelimit (>=2.2.1)
 Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
-Requires-Dist: semsimian (==0.1.13)
+Requires-Dist: semsimian (==0.1.14)
 Requires-Dist: semsql (>=0.3.1)
 Requires-Dist: sssom (>=0.3.26)
 Requires-Dist: sssom-schema (>=0.11.0)
 Description-Content-Type: text/markdown
 
 # Ontology Access Kit (OAK)
```

