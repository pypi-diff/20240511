# Comparing `tmp/kgdata-7.0.1.tar.gz` & `tmp/kgdata-7.0.2.tar.gz`

## Comparing `kgdata-7.0.1.tar` & `kgdata-7.0.2.tar`

### file list

```diff
@@ -1,181 +1,181 @@
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 kgdata-7.0.1/Cargo.toml
--rw-r--r--   0     1001      127    56429 2024-04-26 15:45:38.000000 kgdata-7.0.1/Cargo.lock
--rw-r--r--   0     1001      127     1064 2024-04-26 15:45:38.000000 kgdata-7.0.1/LICENSE
--rw-r--r--   0     1001      127      839 2024-04-26 15:45:38.000000 kgdata-7.0.1/README.md
--rw-r--r--   0     1001      127    33619 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/conversions.rs
--rw-r--r--   0     1001      127     2536 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/interface.rs
--rw-r--r--   0     1001      127     4415 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/mod.rs
--rw-r--r--   0     1001      127     6266 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/predefined_db.rs
--rw-r--r--   0     1001      127     4987 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/readonly_rocksdb_dict.rs
--rw-r--r--   0     1001      127     6211 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/ipcserde.rs
--rw-r--r--   0     1001      127      926 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/mod.rs
--rw-r--r--   0     1001      127     6376 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/nngserver.rs
--rw-r--r--   0     1001      127    11896 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/remote_rocksdb_dict.rs
--rw-r--r--   0     1001      127     2177 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/request.rs
--rw-r--r--   0     1001      127     6487 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/response.rs
--rw-r--r--   0     1001      127     8671 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/shmemhelper.rs
--rw-r--r--   0     1001      127     2842 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/db/remotedb/zeromqserver.rs
--rw-r--r--   0     1001      127     1648 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/error.rs
--rw-r--r--   0     1001      127      662 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/lib.rs
--rw-r--r--   0     1001      127      732 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/main.rs
--rw-r--r--   0     1001      127     2566 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/dataset.rs
--rw-r--r--   0     1001      127      580 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/filterop.rs
--rw-r--r--   0     1001      127      721 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/foldop.rs
--rw-r--r--   0     1001      127     2788 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/functions.rs
--rw-r--r--   0     1001      127     1188 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/mapop.rs
--rw-r--r--   0     1001      127      468 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/miscop.rs
--rw-r--r--   0     1001      127     4851 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/mod.rs
--rw-r--r--   0     1001      127      630 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/mapreduce/sortop.rs
--rw-r--r--   0     1001      127      534 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/class.rs
--rw-r--r--   0     1001      127     1936 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/entity.rs
--rw-r--r--   0     1001      127      248 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/entity_link.rs
--rw-r--r--   0     1001      127      426 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/entity_metadata.rs
--rw-r--r--   0     1001      127      686 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/kgns.rs
--rw-r--r--   0     1001      127      560 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/mod.rs
--rw-r--r--   0     1001      127      648 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/multilingual.rs
--rw-r--r--   0     1001      127     3434 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/property.rs
--rw-r--r--   0     1001      127     5919 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/models/value.rs
--rw-r--r--   0     1001      127      944 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/hashbrown.rs
--rw-r--r--   0     1001      127     4371 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/macros/list.rs
--rw-r--r--   0     1001      127     5848 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/macros/map.rs
--rw-r--r--   0     1001      127     6339 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/macros/mod.rs
--rw-r--r--   0     1001      127     2133 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/macros/set.rs
--rw-r--r--   0     1001      127      784 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/mod.rs
--rw-r--r--   0     1001      127      805 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/strview.rs
--rw-r--r--   0     1001      127      682 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/pyo3helper/usizeview.rs
--rw-r--r--   0     1001      127       33 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/mod.rs
--rw-r--r--   0     1001      127     1286 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/class.rs
--rw-r--r--   0     1001      127      419 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/conversions.rs
--rw-r--r--   0     1001      127     2378 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/entity.rs
--rw-r--r--   0     1001      127     1133 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/entity_metadata.rs
--rw-r--r--   0     1001      127    10911 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/iterators.rs
--rw-r--r--   0     1001      127     1358 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/mod.rs
--rw-r--r--   0     1001      127     2433 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/multilingual.rs
--rw-r--r--   0     1001      127     1827 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/property.rs
--rw-r--r--   0     1001      127     8042 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/models/value.rs
--rw-r--r--   0     1001      127     7062 2024-04-26 15:45:38.000000 kgdata-7.0.1/src/python/scripts.rs
--rw-r--r--   0     1001      127     1585 2024-04-26 15:45:38.000000 kgdata-7.0.1/pyproject.toml
--rw-r--r--   0     1001      127       42 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/prelude.py
--rw-r--r--   0     1001      127     2499 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/config.py
--rw-r--r--   0     1001      127     2908 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/misc.py
--rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/__init__.py
--rw-r--r--   0     1001      127     2212 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/article_metadata.py
--rw-r--r--   0     1001      127     2427 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/mention_to_articles.py
--rw-r--r--   0     1001      127     4810 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/linked_relational_tables.py
--rw-r--r--   0     1001      127     3025 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/articles.py.deprecated
--rw-r--r--   0     1001      127     4168 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/grouped_articles.py.deprecated
--rw-r--r--   0     1001      127     2267 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/easy_tables_metadata.py
--rw-r--r--   0     1001      127     2290 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/article_aliases.py
--rw-r--r--   0     1001      127     3570 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/html_articles.py
--rw-r--r--   0     1001      127     2765 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/article_links.py
--rw-r--r--   0     1001      127      224 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/__init__.py
--rw-r--r--   0     1001      127     8554 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/easy_tables.py
--rw-r--r--   0     1001      127      108 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/__main__.py
--rw-r--r--   0     1001      127     2822 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/html_tables.py
--rw-r--r--   0     1001      127     1907 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/article_degrees.py
--rw-r--r--   0     1001      127     1318 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/datasets/relational_tables.py
--rw-r--r--   0     1001      127     5053 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/wikiapi.py
--rw-r--r--   0     1001      127     1356 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/models/page_article.py
--rw-r--r--   0     1001      127     3776 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/models/linked_html_table.py
--rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/models/__init__.py
--rw-r--r--   0     1001      127     4433 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikipedia/models/html_article.py
--rw-r--r--   0     1001      127    10271 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/db.py
--rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/py.typed
--rw-r--r--   0     1001      127    13686 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/db.py
--rw-r--r--   0     1001      127     6627 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/extra_ent_db.py
--rw-r--r--   0     1001      127     1786 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/wikidata_prefixes.yml
--rw-r--r--   0     1001      127     4138 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/config.py
--rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/__init__.py
--rw-r--r--   0     1001      127     8586 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/__main__.py
--rw-r--r--   0     1001      127     3490 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_outlinks.py
--rw-r--r--   0     1001      127     5703 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/main_property_connections.py
--rw-r--r--   0     1001      127     1833 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_metadata.py
--rw-r--r--   0     1001      127     1906 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_types_and_degrees.py
--rw-r--r--   0     1001      127     3952 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/classes.py
--rw-r--r--   0     1001      127     3954 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/properties.py
--rw-r--r--   0     1001      127     1559 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_redirection_dump.py
--rw-r--r--   0     1001      127      993 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_types.py
--rw-r--r--   0     1001      127     1543 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/page_dump.py
--rw-r--r--   0     1001      127    11156 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entities.py
--rw-r--r--   0     1001      127     1686 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_dump.py
--rw-r--r--   0     1001      127     2509 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/property_ranges.py
--rw-r--r--   0     1001      127     5369 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/meta_graph.py
--rw-r--r--   0     1001      127     3400 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_degrees.py
--rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/__init__.py
--rw-r--r--   0     1001      127     1953 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/property_domains.py
--rw-r--r--   0     1001      127     2662 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_ids.py
--rw-r--r--   0     1001      127     1557 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/norm_mentions.py
--rw-r--r--   0     1001      127     2198 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_all_types.py
--rw-r--r--   0     1001      127     1025 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/__main__.py
--rw-r--r--   0     1001      127     7003 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_redirections.py
--rw-r--r--   0     1001      127     3095 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/page_ids.py
--rw-r--r--   0     1001      127     7754 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/meta_graph_stats.py
--rw-r--r--   0     1001      127     3241 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_wiki_aliases.py
--rw-r--r--   0     1001      127     5789 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/cross_wiki_mapping.py
--rw-r--r--   0     1001      127     1046 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_labels.py
--rw-r--r--   0     1001      127     1930 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/triple_truthy_dump.py
--rw-r--r--   0     1001      127     2743 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/mention_to_entities.py
--rw-r--r--   0     1001      127     1579 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/class_count.py
--rw-r--r--   0     1001      127     1695 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/property_count.py
--rw-r--r--   0     1001      127     8824 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/entity_pagerank.py
--rw-r--r--   0     1001      127      949 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/datasets/ontology_count.py
--rw-r--r--   0     1001      127      639 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdentitylabel.py
--rw-r--r--   0     1001      127     8071 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdentity.py
--rw-r--r--   0     1001      127     1231 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdentitymetadata.py
--rw-r--r--   0     1001      127     7623 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdproperty.py
--rw-r--r--   0     1001      127     1138 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/__init__.py
--rw-r--r--   0     1001      127     1377 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/propertystats.py
--rw-r--r--   0     1001      127     2148 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdstatement.py
--rw-r--r--   0     1001      127     9107 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdvalue.py
--rw-r--r--   0     1001      127     2024 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdclass.py
--rw-r--r--   0     1001      127      428 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/wikidata/models/wdentitylink.py
--rw-r--r--   0     1001      127     7241 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/splitter.py
--rw-r--r--   0     1001      127     2243 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/modification.py
--rw-r--r--   0     1001      127     2388 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/resource.py
--rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/__init__.py
--rw-r--r--   0     1001      127     7492 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/ntriples_parser.py
--rw-r--r--   0     1001      127     1478 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/funcs.py
--rw-r--r--   0     1001      127     1677 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/hierarchy.py
--rw-r--r--   0     1001      127    18184 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/download.py
--rw-r--r--   0     1001      127     1272 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/misc/query.py
--rw-r--r--   0     1001      127     3679 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/config.py
--rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/__init__.py
--rw-r--r--   0     1001      127     2371 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/__main__.py
--rw-r--r--   0     1001      127     1843 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_metadata.py
--rw-r--r--   0     1001      127     1582 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_types_and_degrees.py
--rw-r--r--   0     1001      127     3348 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/classes.py
--rw-r--r--   0     1001      127     5891 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/properties.py
--rw-r--r--   0     1001      127      995 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_types.py
--rw-r--r--   0     1001      127     1725 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/generic_extractor_dump.py
--rw-r--r--   0     1001      127     6968 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entities.py
--rw-r--r--   0     1001      127     7066 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/meta_graph.py
--rw-r--r--   0     1001      127     3862 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/wikilinks.py
--rw-r--r--   0     1001      127     3513 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_degrees.py
--rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/__init__.py
--rw-r--r--   0     1001      127     1730 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/mapping_extractor_dump.py
--rw-r--r--   0     1001      127      587 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/wikilink_dump.py
--rw-r--r--   0     1001      127     4202 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_all_types.py
--rw-r--r--   0     1001      127     2715 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/__main__.py
--rw-r--r--   0     1001      127     6863 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/ontology_dump.py
--rw-r--r--   0     1001      127     2223 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_redirections.py
--rw-r--r--   0     1001      127     1760 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/page_ids.py
--rw-r--r--   0     1001      127     7788 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/meta_graph_stats.py
--rw-r--r--   0     1001      127      954 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/entity_labels.py
--rw-r--r--   0     1001      127      832 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/page_id_dump.py
--rw-r--r--   0     1001      127     1644 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dbpedia/datasets/class_count.py
--rw-r--r--   0     1001      127     1444 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/config.py
--rw-r--r--   0     1001      127    24445 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/dataset.py
--rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/__init__.py
--rw-r--r--   0     1001      127    20035 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/spark/common.py
--rw-r--r--   0     1001      127      328 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/spark/__init__.py
--rw-r--r--   0     1001      127     4253 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/spark/rdd_alike.py
--rw-r--r--   0     1001      127    24898 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/spark/extended_rdd.py
--rw-r--r--   0     1001      127       27 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/core/__init__.pyi
--rw-r--r--   0     1001      127     1385 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/core/base.pyi
--rw-r--r--   0     1001      127     6044 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/core/models.pyi
--rw-r--r--   0     1001      127     3748 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/models/ont_class.py
--rw-r--r--   0     1001      127     3000 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/models/multilingual.py
--rw-r--r--   0     1001      127     5241 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/models/entity.py
--rw-r--r--   0     1001      127        0 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/models/__init__.py
--rw-r--r--   0     1001      127     4587 2024-04-26 15:45:38.000000 kgdata-7.0.1/kgdata/models/ont_property.py
--rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 kgdata-7.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 kgdata-7.0.2/Cargo.toml
+-rw-r--r--   0     1001      127    56429 2024-05-11 05:31:03.000000 kgdata-7.0.2/Cargo.lock
+-rw-r--r--   0     1001      127     1064 2024-05-11 05:31:03.000000 kgdata-7.0.2/LICENSE
+-rw-r--r--   0     1001      127      839 2024-05-11 05:31:03.000000 kgdata-7.0.2/README.md
+-rw-r--r--   0     1001      127    33619 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/conversions.rs
+-rw-r--r--   0     1001      127     2536 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/interface.rs
+-rw-r--r--   0     1001      127     4415 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/mod.rs
+-rw-r--r--   0     1001      127     6266 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/predefined_db.rs
+-rw-r--r--   0     1001      127     4987 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/readonly_rocksdb_dict.rs
+-rw-r--r--   0     1001      127     6211 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/ipcserde.rs
+-rw-r--r--   0     1001      127      926 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/mod.rs
+-rw-r--r--   0     1001      127     6376 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/nngserver.rs
+-rw-r--r--   0     1001      127    11896 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/remote_rocksdb_dict.rs
+-rw-r--r--   0     1001      127     2177 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/request.rs
+-rw-r--r--   0     1001      127     6487 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/response.rs
+-rw-r--r--   0     1001      127     8671 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/shmemhelper.rs
+-rw-r--r--   0     1001      127     2842 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/zeromqserver.rs
+-rw-r--r--   0     1001      127     1648 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/error.rs
+-rw-r--r--   0     1001      127      662 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/lib.rs
+-rw-r--r--   0     1001      127      732 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/main.rs
+-rw-r--r--   0     1001      127     2566 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/dataset.rs
+-rw-r--r--   0     1001      127      580 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/filterop.rs
+-rw-r--r--   0     1001      127      721 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/foldop.rs
+-rw-r--r--   0     1001      127     2788 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/functions.rs
+-rw-r--r--   0     1001      127     1188 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/mapop.rs
+-rw-r--r--   0     1001      127      468 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/miscop.rs
+-rw-r--r--   0     1001      127     4851 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/mod.rs
+-rw-r--r--   0     1001      127      630 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/sortop.rs
+-rw-r--r--   0     1001      127      534 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/class.rs
+-rw-r--r--   0     1001      127     1936 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/entity.rs
+-rw-r--r--   0     1001      127      248 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/entity_link.rs
+-rw-r--r--   0     1001      127      426 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/entity_metadata.rs
+-rw-r--r--   0     1001      127      686 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/kgns.rs
+-rw-r--r--   0     1001      127      560 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/mod.rs
+-rw-r--r--   0     1001      127      648 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/multilingual.rs
+-rw-r--r--   0     1001      127     3434 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/property.rs
+-rw-r--r--   0     1001      127     5919 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/value.rs
+-rw-r--r--   0     1001      127      944 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/hashbrown.rs
+-rw-r--r--   0     1001      127     4371 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/macros/list.rs
+-rw-r--r--   0     1001      127     5848 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/macros/map.rs
+-rw-r--r--   0     1001      127     6339 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/macros/mod.rs
+-rw-r--r--   0     1001      127     2133 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/macros/set.rs
+-rw-r--r--   0     1001      127      784 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/mod.rs
+-rw-r--r--   0     1001      127      805 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/strview.rs
+-rw-r--r--   0     1001      127      682 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/usizeview.rs
+-rw-r--r--   0     1001      127       33 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/mod.rs
+-rw-r--r--   0     1001      127     1286 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/class.rs
+-rw-r--r--   0     1001      127      419 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/conversions.rs
+-rw-r--r--   0     1001      127     2378 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/entity.rs
+-rw-r--r--   0     1001      127     1133 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/entity_metadata.rs
+-rw-r--r--   0     1001      127    10911 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/iterators.rs
+-rw-r--r--   0     1001      127     1358 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/mod.rs
+-rw-r--r--   0     1001      127     2433 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/multilingual.rs
+-rw-r--r--   0     1001      127     1827 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/property.rs
+-rw-r--r--   0     1001      127     8042 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/value.rs
+-rw-r--r--   0     1001      127     7062 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/scripts.rs
+-rw-r--r--   0     1001      127     1585 2024-05-11 05:31:03.000000 kgdata-7.0.2/pyproject.toml
+-rw-r--r--   0     1001      127       42 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/prelude.py
+-rw-r--r--   0     1001      127     2499 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/config.py
+-rw-r--r--   0     1001      127     2908 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/misc.py
+-rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/__init__.py
+-rw-r--r--   0     1001      127     2212 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/article_metadata.py
+-rw-r--r--   0     1001      127     2427 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/mention_to_articles.py
+-rw-r--r--   0     1001      127     4810 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/linked_relational_tables.py
+-rw-r--r--   0     1001      127     3025 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/articles.py.deprecated
+-rw-r--r--   0     1001      127     4168 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/grouped_articles.py.deprecated
+-rw-r--r--   0     1001      127     2267 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/easy_tables_metadata.py
+-rw-r--r--   0     1001      127     2290 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/article_aliases.py
+-rw-r--r--   0     1001      127     3570 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/html_articles.py
+-rw-r--r--   0     1001      127     2765 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/article_links.py
+-rw-r--r--   0     1001      127      224 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/__init__.py
+-rw-r--r--   0     1001      127     8554 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/easy_tables.py
+-rw-r--r--   0     1001      127      108 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/__main__.py
+-rw-r--r--   0     1001      127     2822 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/html_tables.py
+-rw-r--r--   0     1001      127     1907 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/article_degrees.py
+-rw-r--r--   0     1001      127     1318 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/relational_tables.py
+-rw-r--r--   0     1001      127     5053 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/wikiapi.py
+-rw-r--r--   0     1001      127     1356 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/models/page_article.py
+-rw-r--r--   0     1001      127     3776 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/models/linked_html_table.py
+-rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/models/__init__.py
+-rw-r--r--   0     1001      127     4433 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/models/html_article.py
+-rw-r--r--   0     1001      127    10166 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/db.py
+-rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/py.typed
+-rw-r--r--   0     1001      127    13622 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/db.py
+-rw-r--r--   0     1001      127     6627 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/extra_ent_db.py
+-rw-r--r--   0     1001      127     1786 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/wikidata_prefixes.yml
+-rw-r--r--   0     1001      127     4138 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/config.py
+-rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/__init__.py
+-rw-r--r--   0     1001      127     8586 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/__main__.py
+-rw-r--r--   0     1001      127     3490 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_outlinks.py
+-rw-r--r--   0     1001      127     5703 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/main_property_connections.py
+-rw-r--r--   0     1001      127     1833 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_metadata.py
+-rw-r--r--   0     1001      127     1906 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_types_and_degrees.py
+-rw-r--r--   0     1001      127     3952 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/classes.py
+-rw-r--r--   0     1001      127     3954 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/properties.py
+-rw-r--r--   0     1001      127     1559 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_redirection_dump.py
+-rw-r--r--   0     1001      127      993 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_types.py
+-rw-r--r--   0     1001      127     1543 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/page_dump.py
+-rw-r--r--   0     1001      127    11156 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entities.py
+-rw-r--r--   0     1001      127     1686 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_dump.py
+-rw-r--r--   0     1001      127     2509 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/property_ranges.py
+-rw-r--r--   0     1001      127     5369 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/meta_graph.py
+-rw-r--r--   0     1001      127     3400 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_degrees.py
+-rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/__init__.py
+-rw-r--r--   0     1001      127     1953 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/property_domains.py
+-rw-r--r--   0     1001      127     2662 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_ids.py
+-rw-r--r--   0     1001      127     1557 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/norm_mentions.py
+-rw-r--r--   0     1001      127     2198 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_all_types.py
+-rw-r--r--   0     1001      127     1025 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/__main__.py
+-rw-r--r--   0     1001      127     7003 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_redirections.py
+-rw-r--r--   0     1001      127     3095 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/page_ids.py
+-rw-r--r--   0     1001      127     7754 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/meta_graph_stats.py
+-rw-r--r--   0     1001      127     3241 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_wiki_aliases.py
+-rw-r--r--   0     1001      127     5789 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/cross_wiki_mapping.py
+-rw-r--r--   0     1001      127     1046 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_labels.py
+-rw-r--r--   0     1001      127     1930 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/triple_truthy_dump.py
+-rw-r--r--   0     1001      127     2743 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/mention_to_entities.py
+-rw-r--r--   0     1001      127     1579 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/class_count.py
+-rw-r--r--   0     1001      127     1695 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/property_count.py
+-rw-r--r--   0     1001      127     8824 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_pagerank.py
+-rw-r--r--   0     1001      127      949 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/ontology_count.py
+-rw-r--r--   0     1001      127      639 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdentitylabel.py
+-rw-r--r--   0     1001      127     8071 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdentity.py
+-rw-r--r--   0     1001      127     1231 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdentitymetadata.py
+-rw-r--r--   0     1001      127     7623 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdproperty.py
+-rw-r--r--   0     1001      127     1138 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/__init__.py
+-rw-r--r--   0     1001      127     1377 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/propertystats.py
+-rw-r--r--   0     1001      127     2148 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdstatement.py
+-rw-r--r--   0     1001      127     9107 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdvalue.py
+-rw-r--r--   0     1001      127     2024 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdclass.py
+-rw-r--r--   0     1001      127      428 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdentitylink.py
+-rw-r--r--   0     1001      127     7241 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/splitter.py
+-rw-r--r--   0     1001      127     2243 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/modification.py
+-rw-r--r--   0     1001      127     2388 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/resource.py
+-rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/__init__.py
+-rw-r--r--   0     1001      127     7492 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/ntriples_parser.py
+-rw-r--r--   0     1001      127     1478 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/funcs.py
+-rw-r--r--   0     1001      127     1677 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/hierarchy.py
+-rw-r--r--   0     1001      127    18184 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/download.py
+-rw-r--r--   0     1001      127     1272 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/query.py
+-rw-r--r--   0     1001      127     3679 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/config.py
+-rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/__init__.py
+-rw-r--r--   0     1001      127     2371 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/__main__.py
+-rw-r--r--   0     1001      127     1843 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_metadata.py
+-rw-r--r--   0     1001      127     1582 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_types_and_degrees.py
+-rw-r--r--   0     1001      127     3348 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/classes.py
+-rw-r--r--   0     1001      127     5891 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/properties.py
+-rw-r--r--   0     1001      127      995 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_types.py
+-rw-r--r--   0     1001      127     1725 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/generic_extractor_dump.py
+-rw-r--r--   0     1001      127     6968 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entities.py
+-rw-r--r--   0     1001      127     7066 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/meta_graph.py
+-rw-r--r--   0     1001      127     3862 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/wikilinks.py
+-rw-r--r--   0     1001      127     3513 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_degrees.py
+-rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/__init__.py
+-rw-r--r--   0     1001      127     1730 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/mapping_extractor_dump.py
+-rw-r--r--   0     1001      127      587 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/wikilink_dump.py
+-rw-r--r--   0     1001      127     4202 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_all_types.py
+-rw-r--r--   0     1001      127     2715 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/__main__.py
+-rw-r--r--   0     1001      127     6863 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/ontology_dump.py
+-rw-r--r--   0     1001      127     2223 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_redirections.py
+-rw-r--r--   0     1001      127     1760 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/page_ids.py
+-rw-r--r--   0     1001      127     7788 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/meta_graph_stats.py
+-rw-r--r--   0     1001      127      954 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_labels.py
+-rw-r--r--   0     1001      127      832 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/page_id_dump.py
+-rw-r--r--   0     1001      127     1644 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/class_count.py
+-rw-r--r--   0     1001      127     1444 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/config.py
+-rw-r--r--   0     1001      127    24445 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dataset.py
+-rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/__init__.py
+-rw-r--r--   0     1001      127    20035 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/spark/common.py
+-rw-r--r--   0     1001      127      328 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/spark/__init__.py
+-rw-r--r--   0     1001      127     4253 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/spark/rdd_alike.py
+-rw-r--r--   0     1001      127    24898 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/spark/extended_rdd.py
+-rw-r--r--   0     1001      127       27 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/core/__init__.pyi
+-rw-r--r--   0     1001      127     1385 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/core/base.pyi
+-rw-r--r--   0     1001      127     6044 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/core/models.pyi
+-rw-r--r--   0     1001      127     3748 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/models/ont_class.py
+-rw-r--r--   0     1001      127     3000 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/models/multilingual.py
+-rw-r--r--   0     1001      127     5241 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/models/entity.py
+-rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/models/__init__.py
+-rw-r--r--   0     1001      127     4587 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/models/ont_property.py
+-rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 kgdata-7.0.2/PKG-INFO
```

### Comparing `kgdata-7.0.1/Cargo.toml` & `kgdata-7.0.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/Cargo.lock` & `kgdata-7.0.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/LICENSE` & `kgdata-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/README.md` & `kgdata-7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/conversions.rs` & `kgdata-7.0.2/src/conversions.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/interface.rs` & `kgdata-7.0.2/src/db/interface.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/mod.rs` & `kgdata-7.0.2/src/db/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/predefined_db.rs` & `kgdata-7.0.2/src/db/predefined_db.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/readonly_rocksdb_dict.rs` & `kgdata-7.0.2/src/db/readonly_rocksdb_dict.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/remotedb/ipcserde.rs` & `kgdata-7.0.2/src/db/remotedb/ipcserde.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/remotedb/mod.rs` & `kgdata-7.0.2/src/db/remotedb/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/remotedb/nngserver.rs` & `kgdata-7.0.2/src/db/remotedb/nngserver.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/remotedb/remote_rocksdb_dict.rs` & `kgdata-7.0.2/src/db/remotedb/remote_rocksdb_dict.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/remotedb/request.rs` & `kgdata-7.0.2/src/db/remotedb/request.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/remotedb/response.rs` & `kgdata-7.0.2/src/db/remotedb/response.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/remotedb/shmemhelper.rs` & `kgdata-7.0.2/src/db/remotedb/shmemhelper.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/db/remotedb/zeromqserver.rs` & `kgdata-7.0.2/src/db/remotedb/zeromqserver.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/error.rs` & `kgdata-7.0.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/lib.rs` & `kgdata-7.0.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/main.rs` & `kgdata-7.0.2/src/main.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/mapreduce/dataset.rs` & `kgdata-7.0.2/src/mapreduce/dataset.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/mapreduce/filterop.rs` & `kgdata-7.0.2/src/mapreduce/filterop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/mapreduce/foldop.rs` & `kgdata-7.0.2/src/mapreduce/foldop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/mapreduce/functions.rs` & `kgdata-7.0.2/src/mapreduce/functions.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/mapreduce/mapop.rs` & `kgdata-7.0.2/src/mapreduce/mapop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/mapreduce/mod.rs` & `kgdata-7.0.2/src/mapreduce/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/mapreduce/sortop.rs` & `kgdata-7.0.2/src/mapreduce/sortop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/models/class.rs` & `kgdata-7.0.2/src/models/class.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/models/entity.rs` & `kgdata-7.0.2/src/models/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/models/kgns.rs` & `kgdata-7.0.2/src/models/kgns.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/models/mod.rs` & `kgdata-7.0.2/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/models/multilingual.rs` & `kgdata-7.0.2/src/models/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/models/property.rs` & `kgdata-7.0.2/src/models/property.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/models/value.rs` & `kgdata-7.0.2/src/models/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/pyo3helper/hashbrown.rs` & `kgdata-7.0.2/src/pyo3helper/hashbrown.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/pyo3helper/macros/list.rs` & `kgdata-7.0.2/src/pyo3helper/macros/list.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/pyo3helper/macros/map.rs` & `kgdata-7.0.2/src/pyo3helper/macros/map.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/pyo3helper/macros/mod.rs` & `kgdata-7.0.2/src/pyo3helper/macros/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/pyo3helper/macros/set.rs` & `kgdata-7.0.2/src/pyo3helper/macros/set.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/pyo3helper/mod.rs` & `kgdata-7.0.2/src/pyo3helper/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/pyo3helper/strview.rs` & `kgdata-7.0.2/src/pyo3helper/strview.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/pyo3helper/usizeview.rs` & `kgdata-7.0.2/src/pyo3helper/usizeview.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/python/models/class.rs` & `kgdata-7.0.2/src/python/models/class.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/python/models/entity.rs` & `kgdata-7.0.2/src/python/models/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/python/models/entity_metadata.rs` & `kgdata-7.0.2/src/python/models/entity_metadata.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/python/models/iterators.rs` & `kgdata-7.0.2/src/python/models/iterators.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/python/models/mod.rs` & `kgdata-7.0.2/src/python/models/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/python/models/multilingual.rs` & `kgdata-7.0.2/src/python/models/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/python/models/property.rs` & `kgdata-7.0.2/src/python/models/property.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/python/models/value.rs` & `kgdata-7.0.2/src/python/models/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/src/python/scripts.rs` & `kgdata-7.0.2/src/python/scripts.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/pyproject.toml` & `kgdata-7.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kgdata"
-version = "7.0.1"
+version = "7.0.2"
 description = "Library to process dumps of knowledge graphs (Wikipedia, DBpedia, Wikidata)"
 readme = "README.md"
 authors = [{ name = "Binh Vu", email = "binh@toan2.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `kgdata-7.0.1/kgdata/wikipedia/config.py` & `kgdata-7.0.2/kgdata/wikipedia/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/misc.py` & `kgdata-7.0.2/kgdata/wikipedia/misc.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/article_metadata.py` & `kgdata-7.0.2/kgdata/wikipedia/datasets/article_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/mention_to_articles.py` & `kgdata-7.0.2/kgdata/wikipedia/datasets/mention_to_articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/linked_relational_tables.py` & `kgdata-7.0.2/kgdata/wikipedia/datasets/linked_relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/articles.py.deprecated` & `kgdata-7.0.2/kgdata/wikipedia/datasets/articles.py.deprecated`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/grouped_articles.py.deprecated` & `kgdata-7.0.2/kgdata/wikipedia/datasets/grouped_articles.py.deprecated`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/easy_tables_metadata.py` & `kgdata-7.0.2/kgdata/wikipedia/datasets/easy_tables_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/article_aliases.py` & `kgdata-7.0.2/kgdata/wikipedia/datasets/article_aliases.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/html_articles.py` & `kgdata-7.0.2/kgdata/wikipedia/datasets/html_articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/article_links.py` & `kgdata-7.0.2/kgdata/wikipedia/datasets/article_links.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/easy_tables.py` & `kgdata-7.0.2/kgdata/wikipedia/datasets/easy_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/html_tables.py` & `kgdata-7.0.2/kgdata/wikipedia/datasets/html_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/article_degrees.py` & `kgdata-7.0.2/kgdata/wikipedia/datasets/article_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/datasets/relational_tables.py` & `kgdata-7.0.2/kgdata/wikipedia/datasets/relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/wikiapi.py` & `kgdata-7.0.2/kgdata/wikipedia/wikiapi.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/models/page_article.py` & `kgdata-7.0.2/kgdata/wikipedia/models/page_article.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/models/linked_html_table.py` & `kgdata-7.0.2/kgdata/wikipedia/models/linked_html_table.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikipedia/models/html_article.py` & `kgdata-7.0.2/kgdata/wikipedia/models/html_article.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/db.py` & `kgdata-7.0.2/kgdata/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,20 @@
     CacheDict,
     RocksDBCompressionOptions,
     RocksDBDict,
     RocksDBOptions,
     rocksdb_load,
 )
 from hugedict.types import HugeMutableMapping
+from loguru import logger
+from sm.namespaces.namespace import KnowledgeGraphNamespace
+
 from kgdata.models.entity import Entity, EntityMetadata
-from kgdata.models.multilingual import MultiLingualString, MultiLingualStringList
 from kgdata.models.ont_class import OntologyClass
 from kgdata.models.ont_property import OntologyProperty, get_default_props
-from loguru import logger
-from rdflib import RDF, RDFS, XSD
-from sm.namespaces.namespace import KnowledgeGraphNamespace
 
 if TYPE_CHECKING:
     from hugedict.core.rocksdb import FileFormat
 
 T = TypeVar("T")
 
 
@@ -374,7 +373,8 @@
         else:
             for k in db.keys():
                 print("key:", k)
                 print("value:", db[k])
                 break
 
     cli()
+    cli()
```

### Comparing `kgdata-7.0.1/kgdata/wikidata/db.py` & `kgdata-7.0.2/kgdata/wikidata/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 )
 
 import orjson
 import requests
 import serde.jl as jl
 from hugedict.prelude import CacheDict, RocksDBDict
 from hugedict.types import HugeMutableMapping
+from sm.misc.funcs import import_func
+
 from kgdata.db import (
     GenericDB,
     deser_from_dict,
     deser_from_tuple,
     get_rocksdb,
     large_dbopts,
     make_get_rocksdb,
@@ -36,22 +38,20 @@
     ser_to_dict,
     ser_to_tuple,
     small_dbopts,
     unpack_float,
     unpack_int,
 )
 from kgdata.models.entity import EntityOutLinks
-from kgdata.wikidata.datasets.mention_to_entities import MentionToEntities
 from kgdata.wikidata.extra_ent_db import EntAttr, get_entity_attr_db
 from kgdata.wikidata.models import WDClass, WDProperty
 from kgdata.wikidata.models.wdentity import WDEntity
 from kgdata.wikidata.models.wdentitylabel import WDEntityLabel
 from kgdata.wikidata.models.wdentitylink import WDEntityWikiLink
 from kgdata.wikidata.models.wdentitymetadata import WDEntityMetadata
-from sm.misc.funcs import import_func
 
 V = TypeVar("V", WDEntity, WDClass, WDProperty, WDEntityLabel, WDEntityWikiLink)
 
 
 class WDProxyDB(RocksDBDict, HugeMutableMapping[str, V]):
     def set_extract_ent_from_entity(self, func: Callable[[WDEntity], V]):
         self.extract_ent_from_entity = func
@@ -444,7 +444,8 @@
         else:
             for k in db.keys():
                 print("key:", k)
                 print("value:", fmt(db[k]))
                 break
 
     cli()
+    cli()
```

### Comparing `kgdata-7.0.1/kgdata/wikidata/extra_ent_db.py` & `kgdata-7.0.2/kgdata/wikidata/extra_ent_db.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/wikidata_prefixes.yml` & `kgdata-7.0.2/kgdata/wikidata/wikidata_prefixes.yml`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/config.py` & `kgdata-7.0.2/kgdata/wikidata/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/__main__.py` & `kgdata-7.0.2/kgdata/wikidata/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_outlinks.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_outlinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/main_property_connections.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/main_property_connections.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_metadata.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_types_and_degrees.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_types_and_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/classes.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/properties.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/properties.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_redirection_dump.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_redirection_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_types.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/page_dump.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/page_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entities.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_dump.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/property_ranges.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/property_ranges.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/meta_graph.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/meta_graph.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_degrees.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/property_domains.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/property_domains.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_ids.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/norm_mentions.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/norm_mentions.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_all_types.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_all_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/__main__.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_redirections.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_redirections.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/page_ids.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/meta_graph_stats.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/meta_graph_stats.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_wiki_aliases.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_wiki_aliases.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/cross_wiki_mapping.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/cross_wiki_mapping.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_labels.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_labels.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/triple_truthy_dump.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/triple_truthy_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/mention_to_entities.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/mention_to_entities.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/class_count.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/class_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/property_count.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/property_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/entity_pagerank.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/entity_pagerank.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/datasets/ontology_count.py` & `kgdata-7.0.2/kgdata/wikidata/datasets/ontology_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/models/wdentitylabel.py` & `kgdata-7.0.2/kgdata/wikidata/models/wdentitylabel.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/models/wdentity.py` & `kgdata-7.0.2/kgdata/wikidata/models/wdentity.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/models/wdentitymetadata.py` & `kgdata-7.0.2/kgdata/wikidata/models/wdentitymetadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/models/wdproperty.py` & `kgdata-7.0.2/kgdata/wikidata/models/wdproperty.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/models/__init__.py` & `kgdata-7.0.2/kgdata/wikidata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/models/propertystats.py` & `kgdata-7.0.2/kgdata/wikidata/models/propertystats.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/models/wdstatement.py` & `kgdata-7.0.2/kgdata/wikidata/models/wdstatement.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/models/wdvalue.py` & `kgdata-7.0.2/kgdata/wikidata/models/wdvalue.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/wikidata/models/wdclass.py` & `kgdata-7.0.2/kgdata/wikidata/models/wdclass.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/splitter.py` & `kgdata-7.0.2/kgdata/splitter.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/misc/modification.py` & `kgdata-7.0.2/kgdata/misc/modification.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/misc/resource.py` & `kgdata-7.0.2/kgdata/misc/resource.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/misc/ntriples_parser.py` & `kgdata-7.0.2/kgdata/misc/ntriples_parser.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/misc/funcs.py` & `kgdata-7.0.2/kgdata/misc/funcs.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/misc/hierarchy.py` & `kgdata-7.0.2/kgdata/misc/hierarchy.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/misc/download.py` & `kgdata-7.0.2/kgdata/misc/download.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/misc/query.py` & `kgdata-7.0.2/kgdata/misc/query.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/config.py` & `kgdata-7.0.2/kgdata/dbpedia/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/__main__.py` & `kgdata-7.0.2/kgdata/dbpedia/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_metadata.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_types_and_degrees.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_types_and_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/classes.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/properties.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/properties.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_types.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/generic_extractor_dump.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/generic_extractor_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/entities.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/meta_graph.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/meta_graph.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/wikilinks.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/wikilinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_degrees.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/mapping_extractor_dump.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/mapping_extractor_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/wikilink_dump.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/wikilink_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_all_types.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_all_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/__main__.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/ontology_dump.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/ontology_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_redirections.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_redirections.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/page_ids.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/meta_graph_stats.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/meta_graph_stats.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/entity_labels.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_labels.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/page_id_dump.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/page_id_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dbpedia/datasets/class_count.py` & `kgdata-7.0.2/kgdata/dbpedia/datasets/class_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/config.py` & `kgdata-7.0.2/kgdata/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/dataset.py` & `kgdata-7.0.2/kgdata/dataset.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/spark/common.py` & `kgdata-7.0.2/kgdata/spark/common.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/spark/rdd_alike.py` & `kgdata-7.0.2/kgdata/spark/rdd_alike.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/spark/extended_rdd.py` & `kgdata-7.0.2/kgdata/spark/extended_rdd.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/core/base.pyi` & `kgdata-7.0.2/kgdata/core/base.pyi`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/core/models.pyi` & `kgdata-7.0.2/kgdata/core/models.pyi`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/models/ont_class.py` & `kgdata-7.0.2/kgdata/models/ont_class.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/models/multilingual.py` & `kgdata-7.0.2/kgdata/models/multilingual.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/models/entity.py` & `kgdata-7.0.2/kgdata/models/entity.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/kgdata/models/ont_property.py` & `kgdata-7.0.2/kgdata/models/ont_property.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.1/PKG-INFO` & `kgdata-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kgdata
-Version: 7.0.1
+Version: 7.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: orjson >=3.9.0, <4.0.0
 Requires-Dist: tqdm >=4.64.0, <5.0.0
 Requires-Dist: beautifulsoup4 >=4.9.3, <5.0.0
 Requires-Dist: loguru >=0.7.0, <0.8.0
 Requires-Dist: rdflib >=7.0.0, <8.0.0
```

