# Comparing `tmp/kgdata-7.0.2.tar.gz` & `tmp/kgdata-7.0.4.tar.gz`

## Comparing `kgdata-7.0.2.tar` & `kgdata-7.0.4.tar`

### file list

```diff
@@ -1,181 +1,182 @@
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 kgdata-7.0.2/Cargo.toml
--rw-r--r--   0     1001      127    56429 2024-05-11 05:31:03.000000 kgdata-7.0.2/Cargo.lock
--rw-r--r--   0     1001      127     1064 2024-05-11 05:31:03.000000 kgdata-7.0.2/LICENSE
--rw-r--r--   0     1001      127      839 2024-05-11 05:31:03.000000 kgdata-7.0.2/README.md
--rw-r--r--   0     1001      127    33619 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/conversions.rs
--rw-r--r--   0     1001      127     2536 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/interface.rs
--rw-r--r--   0     1001      127     4415 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/mod.rs
--rw-r--r--   0     1001      127     6266 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/predefined_db.rs
--rw-r--r--   0     1001      127     4987 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/readonly_rocksdb_dict.rs
--rw-r--r--   0     1001      127     6211 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/ipcserde.rs
--rw-r--r--   0     1001      127      926 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/mod.rs
--rw-r--r--   0     1001      127     6376 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/nngserver.rs
--rw-r--r--   0     1001      127    11896 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/remote_rocksdb_dict.rs
--rw-r--r--   0     1001      127     2177 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/request.rs
--rw-r--r--   0     1001      127     6487 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/response.rs
--rw-r--r--   0     1001      127     8671 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/shmemhelper.rs
--rw-r--r--   0     1001      127     2842 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/db/remotedb/zeromqserver.rs
--rw-r--r--   0     1001      127     1648 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/error.rs
--rw-r--r--   0     1001      127      662 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/lib.rs
--rw-r--r--   0     1001      127      732 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/main.rs
--rw-r--r--   0     1001      127     2566 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/dataset.rs
--rw-r--r--   0     1001      127      580 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/filterop.rs
--rw-r--r--   0     1001      127      721 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/foldop.rs
--rw-r--r--   0     1001      127     2788 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/functions.rs
--rw-r--r--   0     1001      127     1188 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/mapop.rs
--rw-r--r--   0     1001      127      468 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/miscop.rs
--rw-r--r--   0     1001      127     4851 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/mod.rs
--rw-r--r--   0     1001      127      630 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/mapreduce/sortop.rs
--rw-r--r--   0     1001      127      534 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/class.rs
--rw-r--r--   0     1001      127     1936 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/entity.rs
--rw-r--r--   0     1001      127      248 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/entity_link.rs
--rw-r--r--   0     1001      127      426 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/entity_metadata.rs
--rw-r--r--   0     1001      127      686 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/kgns.rs
--rw-r--r--   0     1001      127      560 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/mod.rs
--rw-r--r--   0     1001      127      648 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/multilingual.rs
--rw-r--r--   0     1001      127     3434 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/property.rs
--rw-r--r--   0     1001      127     5919 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/models/value.rs
--rw-r--r--   0     1001      127      944 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/hashbrown.rs
--rw-r--r--   0     1001      127     4371 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/macros/list.rs
--rw-r--r--   0     1001      127     5848 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/macros/map.rs
--rw-r--r--   0     1001      127     6339 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/macros/mod.rs
--rw-r--r--   0     1001      127     2133 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/macros/set.rs
--rw-r--r--   0     1001      127      784 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/mod.rs
--rw-r--r--   0     1001      127      805 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/strview.rs
--rw-r--r--   0     1001      127      682 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/pyo3helper/usizeview.rs
--rw-r--r--   0     1001      127       33 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/mod.rs
--rw-r--r--   0     1001      127     1286 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/class.rs
--rw-r--r--   0     1001      127      419 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/conversions.rs
--rw-r--r--   0     1001      127     2378 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/entity.rs
--rw-r--r--   0     1001      127     1133 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/entity_metadata.rs
--rw-r--r--   0     1001      127    10911 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/iterators.rs
--rw-r--r--   0     1001      127     1358 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/mod.rs
--rw-r--r--   0     1001      127     2433 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/multilingual.rs
--rw-r--r--   0     1001      127     1827 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/property.rs
--rw-r--r--   0     1001      127     8042 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/models/value.rs
--rw-r--r--   0     1001      127     7062 2024-05-11 05:31:03.000000 kgdata-7.0.2/src/python/scripts.rs
--rw-r--r--   0     1001      127     1585 2024-05-11 05:31:03.000000 kgdata-7.0.2/pyproject.toml
--rw-r--r--   0     1001      127       42 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/prelude.py
--rw-r--r--   0     1001      127     2499 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/config.py
--rw-r--r--   0     1001      127     2908 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/misc.py
--rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/__init__.py
--rw-r--r--   0     1001      127     2212 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/article_metadata.py
--rw-r--r--   0     1001      127     2427 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/mention_to_articles.py
--rw-r--r--   0     1001      127     4810 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/linked_relational_tables.py
--rw-r--r--   0     1001      127     3025 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/articles.py.deprecated
--rw-r--r--   0     1001      127     4168 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/grouped_articles.py.deprecated
--rw-r--r--   0     1001      127     2267 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/easy_tables_metadata.py
--rw-r--r--   0     1001      127     2290 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/article_aliases.py
--rw-r--r--   0     1001      127     3570 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/html_articles.py
--rw-r--r--   0     1001      127     2765 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/article_links.py
--rw-r--r--   0     1001      127      224 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/__init__.py
--rw-r--r--   0     1001      127     8554 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/easy_tables.py
--rw-r--r--   0     1001      127      108 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/__main__.py
--rw-r--r--   0     1001      127     2822 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/html_tables.py
--rw-r--r--   0     1001      127     1907 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/article_degrees.py
--rw-r--r--   0     1001      127     1318 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/datasets/relational_tables.py
--rw-r--r--   0     1001      127     5053 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/wikiapi.py
--rw-r--r--   0     1001      127     1356 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/models/page_article.py
--rw-r--r--   0     1001      127     3776 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/models/linked_html_table.py
--rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/models/__init__.py
--rw-r--r--   0     1001      127     4433 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikipedia/models/html_article.py
--rw-r--r--   0     1001      127    10166 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/db.py
--rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/py.typed
--rw-r--r--   0     1001      127    13622 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/db.py
--rw-r--r--   0     1001      127     6627 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/extra_ent_db.py
--rw-r--r--   0     1001      127     1786 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/wikidata_prefixes.yml
--rw-r--r--   0     1001      127     4138 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/config.py
--rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/__init__.py
--rw-r--r--   0     1001      127     8586 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/__main__.py
--rw-r--r--   0     1001      127     3490 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_outlinks.py
--rw-r--r--   0     1001      127     5703 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/main_property_connections.py
--rw-r--r--   0     1001      127     1833 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_metadata.py
--rw-r--r--   0     1001      127     1906 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_types_and_degrees.py
--rw-r--r--   0     1001      127     3952 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/classes.py
--rw-r--r--   0     1001      127     3954 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/properties.py
--rw-r--r--   0     1001      127     1559 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_redirection_dump.py
--rw-r--r--   0     1001      127      993 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_types.py
--rw-r--r--   0     1001      127     1543 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/page_dump.py
--rw-r--r--   0     1001      127    11156 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entities.py
--rw-r--r--   0     1001      127     1686 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_dump.py
--rw-r--r--   0     1001      127     2509 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/property_ranges.py
--rw-r--r--   0     1001      127     5369 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/meta_graph.py
--rw-r--r--   0     1001      127     3400 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_degrees.py
--rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/__init__.py
--rw-r--r--   0     1001      127     1953 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/property_domains.py
--rw-r--r--   0     1001      127     2662 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_ids.py
--rw-r--r--   0     1001      127     1557 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/norm_mentions.py
--rw-r--r--   0     1001      127     2198 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_all_types.py
--rw-r--r--   0     1001      127     1025 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/__main__.py
--rw-r--r--   0     1001      127     7003 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_redirections.py
--rw-r--r--   0     1001      127     3095 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/page_ids.py
--rw-r--r--   0     1001      127     7754 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/meta_graph_stats.py
--rw-r--r--   0     1001      127     3241 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_wiki_aliases.py
--rw-r--r--   0     1001      127     5789 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/cross_wiki_mapping.py
--rw-r--r--   0     1001      127     1046 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_labels.py
--rw-r--r--   0     1001      127     1930 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/triple_truthy_dump.py
--rw-r--r--   0     1001      127     2743 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/mention_to_entities.py
--rw-r--r--   0     1001      127     1579 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/class_count.py
--rw-r--r--   0     1001      127     1695 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/property_count.py
--rw-r--r--   0     1001      127     8824 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/entity_pagerank.py
--rw-r--r--   0     1001      127      949 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/datasets/ontology_count.py
--rw-r--r--   0     1001      127      639 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdentitylabel.py
--rw-r--r--   0     1001      127     8071 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdentity.py
--rw-r--r--   0     1001      127     1231 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdentitymetadata.py
--rw-r--r--   0     1001      127     7623 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdproperty.py
--rw-r--r--   0     1001      127     1138 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/__init__.py
--rw-r--r--   0     1001      127     1377 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/propertystats.py
--rw-r--r--   0     1001      127     2148 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdstatement.py
--rw-r--r--   0     1001      127     9107 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdvalue.py
--rw-r--r--   0     1001      127     2024 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdclass.py
--rw-r--r--   0     1001      127      428 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/wikidata/models/wdentitylink.py
--rw-r--r--   0     1001      127     7241 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/splitter.py
--rw-r--r--   0     1001      127     2243 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/modification.py
--rw-r--r--   0     1001      127     2388 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/resource.py
--rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/__init__.py
--rw-r--r--   0     1001      127     7492 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/ntriples_parser.py
--rw-r--r--   0     1001      127     1478 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/funcs.py
--rw-r--r--   0     1001      127     1677 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/hierarchy.py
--rw-r--r--   0     1001      127    18184 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/download.py
--rw-r--r--   0     1001      127     1272 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/misc/query.py
--rw-r--r--   0     1001      127     3679 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/config.py
--rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/__init__.py
--rw-r--r--   0     1001      127     2371 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/__main__.py
--rw-r--r--   0     1001      127     1843 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_metadata.py
--rw-r--r--   0     1001      127     1582 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_types_and_degrees.py
--rw-r--r--   0     1001      127     3348 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/classes.py
--rw-r--r--   0     1001      127     5891 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/properties.py
--rw-r--r--   0     1001      127      995 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_types.py
--rw-r--r--   0     1001      127     1725 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/generic_extractor_dump.py
--rw-r--r--   0     1001      127     6968 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entities.py
--rw-r--r--   0     1001      127     7066 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/meta_graph.py
--rw-r--r--   0     1001      127     3862 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/wikilinks.py
--rw-r--r--   0     1001      127     3513 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_degrees.py
--rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/__init__.py
--rw-r--r--   0     1001      127     1730 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/mapping_extractor_dump.py
--rw-r--r--   0     1001      127      587 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/wikilink_dump.py
--rw-r--r--   0     1001      127     4202 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_all_types.py
--rw-r--r--   0     1001      127     2715 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/__main__.py
--rw-r--r--   0     1001      127     6863 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/ontology_dump.py
--rw-r--r--   0     1001      127     2223 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_redirections.py
--rw-r--r--   0     1001      127     1760 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/page_ids.py
--rw-r--r--   0     1001      127     7788 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/meta_graph_stats.py
--rw-r--r--   0     1001      127      954 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/entity_labels.py
--rw-r--r--   0     1001      127      832 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/page_id_dump.py
--rw-r--r--   0     1001      127     1644 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dbpedia/datasets/class_count.py
--rw-r--r--   0     1001      127     1444 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/config.py
--rw-r--r--   0     1001      127    24445 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/dataset.py
--rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/__init__.py
--rw-r--r--   0     1001      127    20035 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/spark/common.py
--rw-r--r--   0     1001      127      328 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/spark/__init__.py
--rw-r--r--   0     1001      127     4253 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/spark/rdd_alike.py
--rw-r--r--   0     1001      127    24898 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/spark/extended_rdd.py
--rw-r--r--   0     1001      127       27 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/core/__init__.pyi
--rw-r--r--   0     1001      127     1385 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/core/base.pyi
--rw-r--r--   0     1001      127     6044 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/core/models.pyi
--rw-r--r--   0     1001      127     3748 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/models/ont_class.py
--rw-r--r--   0     1001      127     3000 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/models/multilingual.py
--rw-r--r--   0     1001      127     5241 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/models/entity.py
--rw-r--r--   0     1001      127        0 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/models/__init__.py
--rw-r--r--   0     1001      127     4587 2024-05-11 05:31:03.000000 kgdata-7.0.2/kgdata/models/ont_property.py
--rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 kgdata-7.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 kgdata-7.0.4/Cargo.toml
+-rw-r--r--   0     1001      127    56429 2024-05-11 07:27:17.000000 kgdata-7.0.4/Cargo.lock
+-rw-r--r--   0     1001      127     1064 2024-05-11 07:27:17.000000 kgdata-7.0.4/LICENSE
+-rw-r--r--   0     1001      127      839 2024-05-11 07:27:17.000000 kgdata-7.0.4/README.md
+-rw-r--r--   0     1001      127    33619 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/conversions.rs
+-rw-r--r--   0     1001      127     2536 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/interface.rs
+-rw-r--r--   0     1001      127     4415 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/mod.rs
+-rw-r--r--   0     1001      127     6266 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/predefined_db.rs
+-rw-r--r--   0     1001      127     4987 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/readonly_rocksdb_dict.rs
+-rw-r--r--   0     1001      127     6211 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/remotedb/ipcserde.rs
+-rw-r--r--   0     1001      127      926 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/remotedb/mod.rs
+-rw-r--r--   0     1001      127     6376 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/remotedb/nngserver.rs
+-rw-r--r--   0     1001      127    11896 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/remotedb/remote_rocksdb_dict.rs
+-rw-r--r--   0     1001      127     2177 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/remotedb/request.rs
+-rw-r--r--   0     1001      127     6487 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/remotedb/response.rs
+-rw-r--r--   0     1001      127     8671 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/remotedb/shmemhelper.rs
+-rw-r--r--   0     1001      127     2842 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/db/remotedb/zeromqserver.rs
+-rw-r--r--   0     1001      127     1648 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/error.rs
+-rw-r--r--   0     1001      127      662 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/lib.rs
+-rw-r--r--   0     1001      127      732 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/main.rs
+-rw-r--r--   0     1001      127     2566 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/mapreduce/dataset.rs
+-rw-r--r--   0     1001      127      580 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/mapreduce/filterop.rs
+-rw-r--r--   0     1001      127      721 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/mapreduce/foldop.rs
+-rw-r--r--   0     1001      127     2788 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/mapreduce/functions.rs
+-rw-r--r--   0     1001      127     1188 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/mapreduce/mapop.rs
+-rw-r--r--   0     1001      127      468 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/mapreduce/miscop.rs
+-rw-r--r--   0     1001      127     4851 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/mapreduce/mod.rs
+-rw-r--r--   0     1001      127      630 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/mapreduce/sortop.rs
+-rw-r--r--   0     1001      127      534 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/models/class.rs
+-rw-r--r--   0     1001      127     1936 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/models/entity.rs
+-rw-r--r--   0     1001      127      248 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/models/entity_link.rs
+-rw-r--r--   0     1001      127      426 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/models/entity_metadata.rs
+-rw-r--r--   0     1001      127      686 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/models/kgns.rs
+-rw-r--r--   0     1001      127      560 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/models/mod.rs
+-rw-r--r--   0     1001      127      648 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/models/multilingual.rs
+-rw-r--r--   0     1001      127     3434 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/models/property.rs
+-rw-r--r--   0     1001      127     5919 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/models/value.rs
+-rw-r--r--   0     1001      127      944 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/pyo3helper/hashbrown.rs
+-rw-r--r--   0     1001      127     4371 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/pyo3helper/macros/list.rs
+-rw-r--r--   0     1001      127     5848 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/pyo3helper/macros/map.rs
+-rw-r--r--   0     1001      127     6339 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/pyo3helper/macros/mod.rs
+-rw-r--r--   0     1001      127     2133 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/pyo3helper/macros/set.rs
+-rw-r--r--   0     1001      127      784 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/pyo3helper/mod.rs
+-rw-r--r--   0     1001      127      805 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/pyo3helper/strview.rs
+-rw-r--r--   0     1001      127      682 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/pyo3helper/usizeview.rs
+-rw-r--r--   0     1001      127       33 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/python/mod.rs
+-rw-r--r--   0     1001      127     1286 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/python/models/class.rs
+-rw-r--r--   0     1001      127      419 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/python/models/conversions.rs
+-rw-r--r--   0     1001      127     2378 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/python/models/entity.rs
+-rw-r--r--   0     1001      127     1133 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/python/models/entity_metadata.rs
+-rw-r--r--   0     1001      127    10911 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/python/models/iterators.rs
+-rw-r--r--   0     1001      127     1358 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/python/models/mod.rs
+-rw-r--r--   0     1001      127     2433 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/python/models/multilingual.rs
+-rw-r--r--   0     1001      127     1827 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/python/models/property.rs
+-rw-r--r--   0     1001      127     8042 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/python/models/value.rs
+-rw-r--r--   0     1001      127     7062 2024-05-11 07:27:17.000000 kgdata-7.0.4/src/python/scripts.rs
+-rw-r--r--   0     1001      127     1593 2024-05-11 07:27:17.000000 kgdata-7.0.4/pyproject.toml
+-rw-r--r--   0     1001      127       42 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/prelude.py
+-rw-r--r--   0     1001      127     2499 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/config.py
+-rw-r--r--   0     1001      127     2908 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/misc.py
+-rw-r--r--   0     1001      127        0 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/__init__.py
+-rw-r--r--   0     1001      127     2212 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/article_metadata.py
+-rw-r--r--   0     1001      127     2427 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/mention_to_articles.py
+-rw-r--r--   0     1001      127     4810 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/linked_relational_tables.py
+-rw-r--r--   0     1001      127     3025 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/articles.py.deprecated
+-rw-r--r--   0     1001      127     4168 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/grouped_articles.py.deprecated
+-rw-r--r--   0     1001      127     2267 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/easy_tables_metadata.py
+-rw-r--r--   0     1001      127     2290 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/article_aliases.py
+-rw-r--r--   0     1001      127     3570 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/html_articles.py
+-rw-r--r--   0     1001      127     2765 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/article_links.py
+-rw-r--r--   0     1001      127      224 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/__init__.py
+-rw-r--r--   0     1001      127     8554 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/easy_tables.py
+-rw-r--r--   0     1001      127      108 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/__main__.py
+-rw-r--r--   0     1001      127     2822 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/html_tables.py
+-rw-r--r--   0     1001      127     1907 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/article_degrees.py
+-rw-r--r--   0     1001      127     1318 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/datasets/relational_tables.py
+-rw-r--r--   0     1001      127     5053 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/wikiapi.py
+-rw-r--r--   0     1001      127     1356 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/models/page_article.py
+-rw-r--r--   0     1001      127     3776 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/models/linked_html_table.py
+-rw-r--r--   0     1001      127        0 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/models/__init__.py
+-rw-r--r--   0     1001      127     4433 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikipedia/models/html_article.py
+-rw-r--r--   0     1001      127    10166 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/db.py
+-rw-r--r--   0     1001      127        0 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/py.typed
+-rw-r--r--   0     1001      127    13622 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/db.py
+-rw-r--r--   0     1001      127     6627 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/extra_ent_db.py
+-rw-r--r--   0     1001      127     1786 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/wikidata_prefixes.yml
+-rw-r--r--   0     1001      127     4138 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/config.py
+-rw-r--r--   0     1001      127        0 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/__init__.py
+-rw-r--r--   0     1001      127     8556 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/__main__.py
+-rw-r--r--   0     1001      127     3490 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_outlinks.py
+-rw-r--r--   0     1001      127     5703 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/main_property_connections.py
+-rw-r--r--   0     1001      127     1833 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_metadata.py
+-rw-r--r--   0     1001      127     1906 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_types_and_degrees.py
+-rw-r--r--   0     1001      127     3952 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/classes.py
+-rw-r--r--   0     1001      127     3954 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/properties.py
+-rw-r--r--   0     1001      127     1559 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_redirection_dump.py
+-rw-r--r--   0     1001      127      993 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_types.py
+-rw-r--r--   0     1001      127     1543 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/page_dump.py
+-rw-r--r--   0     1001      127    11176 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entities.py
+-rw-r--r--   0     1001      127     1686 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_dump.py
+-rw-r--r--   0     1001      127     2509 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/property_ranges.py
+-rw-r--r--   0     1001      127     5369 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/meta_graph.py
+-rw-r--r--   0     1001      127     3400 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_degrees.py
+-rw-r--r--   0     1001      127        0 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/__init__.py
+-rw-r--r--   0     1001      127     1953 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/property_domains.py
+-rw-r--r--   0     1001      127     2662 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_ids.py
+-rw-r--r--   0     1001      127     1557 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/norm_mentions.py
+-rw-r--r--   0     1001      127     2198 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_all_types.py
+-rw-r--r--   0     1001      127     1025 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/__main__.py
+-rw-r--r--   0     1001      127     7003 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_redirections.py
+-rw-r--r--   0     1001      127     3095 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/page_ids.py
+-rw-r--r--   0     1001      127     7754 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/meta_graph_stats.py
+-rw-r--r--   0     1001      127     3241 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_wiki_aliases.py
+-rw-r--r--   0     1001      127     5789 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/cross_wiki_mapping.py
+-rw-r--r--   0     1001      127     1046 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_labels.py
+-rw-r--r--   0     1001      127     1930 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/triple_truthy_dump.py
+-rw-r--r--   0     1001      127     2743 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/mention_to_entities.py
+-rw-r--r--   0     1001      127     1579 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/class_count.py
+-rw-r--r--   0     1001      127     1695 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/property_count.py
+-rw-r--r--   0     1001      127     8824 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/entity_pagerank.py
+-rw-r--r--   0     1001      127      949 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/datasets/ontology_count.py
+-rw-r--r--   0     1001      127      639 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/models/wdentitylabel.py
+-rw-r--r--   0     1001      127     8071 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/models/wdentity.py
+-rw-r--r--   0     1001      127     1231 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/models/wdentitymetadata.py
+-rw-r--r--   0     1001      127     7623 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/models/wdproperty.py
+-rw-r--r--   0     1001      127     1138 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/models/__init__.py
+-rw-r--r--   0     1001      127     1377 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/models/propertystats.py
+-rw-r--r--   0     1001      127     2148 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/models/wdstatement.py
+-rw-r--r--   0     1001      127     9107 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/models/wdvalue.py
+-rw-r--r--   0     1001      127     2024 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/models/wdclass.py
+-rw-r--r--   0     1001      127      428 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/wikidata/models/wdentitylink.py
+-rw-r--r--   0     1001      127     7241 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/splitter.py
+-rw-r--r--   0     1001      127     2243 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/misc/modification.py
+-rw-r--r--   0     1001      127     2388 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/misc/resource.py
+-rw-r--r--   0     1001      127      606 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/misc/optional_import.py
+-rw-r--r--   0     1001      127        0 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/misc/__init__.py
+-rw-r--r--   0     1001      127     7492 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/misc/ntriples_parser.py
+-rw-r--r--   0     1001      127     1478 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/misc/funcs.py
+-rw-r--r--   0     1001      127     1677 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/misc/hierarchy.py
+-rw-r--r--   0     1001      127    18184 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/misc/download.py
+-rw-r--r--   0     1001      127     1272 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/misc/query.py
+-rw-r--r--   0     1001      127     3679 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/config.py
+-rw-r--r--   0     1001      127        0 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/__init__.py
+-rw-r--r--   0     1001      127     2371 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/__main__.py
+-rw-r--r--   0     1001      127     1843 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/entity_metadata.py
+-rw-r--r--   0     1001      127     1582 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/entity_types_and_degrees.py
+-rw-r--r--   0     1001      127     3348 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/classes.py
+-rw-r--r--   0     1001      127     5891 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/properties.py
+-rw-r--r--   0     1001      127      995 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/entity_types.py
+-rw-r--r--   0     1001      127     1725 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/generic_extractor_dump.py
+-rw-r--r--   0     1001      127     6968 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/entities.py
+-rw-r--r--   0     1001      127     7066 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/meta_graph.py
+-rw-r--r--   0     1001      127     3862 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/wikilinks.py
+-rw-r--r--   0     1001      127     3513 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/entity_degrees.py
+-rw-r--r--   0     1001      127        0 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/__init__.py
+-rw-r--r--   0     1001      127     1730 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/mapping_extractor_dump.py
+-rw-r--r--   0     1001      127      587 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/wikilink_dump.py
+-rw-r--r--   0     1001      127     4202 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/entity_all_types.py
+-rw-r--r--   0     1001      127     2715 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/__main__.py
+-rw-r--r--   0     1001      127     6863 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/ontology_dump.py
+-rw-r--r--   0     1001      127     2223 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/entity_redirections.py
+-rw-r--r--   0     1001      127     1760 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/page_ids.py
+-rw-r--r--   0     1001      127     7788 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/meta_graph_stats.py
+-rw-r--r--   0     1001      127      954 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/entity_labels.py
+-rw-r--r--   0     1001      127      832 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/page_id_dump.py
+-rw-r--r--   0     1001      127     1644 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dbpedia/datasets/class_count.py
+-rw-r--r--   0     1001      127     1444 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/config.py
+-rw-r--r--   0     1001      127    24466 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/dataset.py
+-rw-r--r--   0     1001      127        0 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/__init__.py
+-rw-r--r--   0     1001      127    20089 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/spark/common.py
+-rw-r--r--   0     1001      127      328 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/spark/__init__.py
+-rw-r--r--   0     1001      127     4253 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/spark/rdd_alike.py
+-rw-r--r--   0     1001      127    24866 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/spark/extended_rdd.py
+-rw-r--r--   0     1001      127       27 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/core/__init__.pyi
+-rw-r--r--   0     1001      127     1385 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/core/base.pyi
+-rw-r--r--   0     1001      127     6044 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/core/models.pyi
+-rw-r--r--   0     1001      127     3748 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/models/ont_class.py
+-rw-r--r--   0     1001      127     3000 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/models/multilingual.py
+-rw-r--r--   0     1001      127     5241 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/models/entity.py
+-rw-r--r--   0     1001      127        0 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/models/__init__.py
+-rw-r--r--   0     1001      127     4587 2024-05-11 07:27:17.000000 kgdata-7.0.4/kgdata/models/ont_property.py
+-rw-r--r--   0        0        0     2682 1970-01-01 00:00:00.000000 kgdata-7.0.4/PKG-INFO
```

### Comparing `kgdata-7.0.2/Cargo.toml` & `kgdata-7.0.4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/Cargo.lock` & `kgdata-7.0.4/Cargo.lock`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/LICENSE` & `kgdata-7.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/README.md` & `kgdata-7.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/conversions.rs` & `kgdata-7.0.4/src/conversions.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/interface.rs` & `kgdata-7.0.4/src/db/interface.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/mod.rs` & `kgdata-7.0.4/src/db/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/predefined_db.rs` & `kgdata-7.0.4/src/db/predefined_db.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/readonly_rocksdb_dict.rs` & `kgdata-7.0.4/src/db/readonly_rocksdb_dict.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/remotedb/ipcserde.rs` & `kgdata-7.0.4/src/db/remotedb/ipcserde.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/remotedb/mod.rs` & `kgdata-7.0.4/src/db/remotedb/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/remotedb/nngserver.rs` & `kgdata-7.0.4/src/db/remotedb/nngserver.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/remotedb/remote_rocksdb_dict.rs` & `kgdata-7.0.4/src/db/remotedb/remote_rocksdb_dict.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/remotedb/request.rs` & `kgdata-7.0.4/src/db/remotedb/request.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/remotedb/response.rs` & `kgdata-7.0.4/src/db/remotedb/response.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/remotedb/shmemhelper.rs` & `kgdata-7.0.4/src/db/remotedb/shmemhelper.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/db/remotedb/zeromqserver.rs` & `kgdata-7.0.4/src/db/remotedb/zeromqserver.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/error.rs` & `kgdata-7.0.4/src/error.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/lib.rs` & `kgdata-7.0.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/main.rs` & `kgdata-7.0.4/src/main.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/mapreduce/dataset.rs` & `kgdata-7.0.4/src/mapreduce/dataset.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/mapreduce/filterop.rs` & `kgdata-7.0.4/src/mapreduce/filterop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/mapreduce/foldop.rs` & `kgdata-7.0.4/src/mapreduce/foldop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/mapreduce/functions.rs` & `kgdata-7.0.4/src/mapreduce/functions.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/mapreduce/mapop.rs` & `kgdata-7.0.4/src/mapreduce/mapop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/mapreduce/mod.rs` & `kgdata-7.0.4/src/mapreduce/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/mapreduce/sortop.rs` & `kgdata-7.0.4/src/mapreduce/sortop.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/models/class.rs` & `kgdata-7.0.4/src/models/class.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/models/entity.rs` & `kgdata-7.0.4/src/models/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/models/kgns.rs` & `kgdata-7.0.4/src/models/kgns.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/models/mod.rs` & `kgdata-7.0.4/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/models/multilingual.rs` & `kgdata-7.0.4/src/models/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/models/property.rs` & `kgdata-7.0.4/src/models/property.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/models/value.rs` & `kgdata-7.0.4/src/models/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/pyo3helper/hashbrown.rs` & `kgdata-7.0.4/src/pyo3helper/hashbrown.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/pyo3helper/macros/list.rs` & `kgdata-7.0.4/src/pyo3helper/macros/list.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/pyo3helper/macros/map.rs` & `kgdata-7.0.4/src/pyo3helper/macros/map.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/pyo3helper/macros/mod.rs` & `kgdata-7.0.4/src/pyo3helper/macros/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/pyo3helper/macros/set.rs` & `kgdata-7.0.4/src/pyo3helper/macros/set.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/pyo3helper/mod.rs` & `kgdata-7.0.4/src/pyo3helper/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/pyo3helper/strview.rs` & `kgdata-7.0.4/src/pyo3helper/strview.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/pyo3helper/usizeview.rs` & `kgdata-7.0.4/src/pyo3helper/usizeview.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/python/models/class.rs` & `kgdata-7.0.4/src/python/models/class.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/python/models/entity.rs` & `kgdata-7.0.4/src/python/models/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/python/models/entity_metadata.rs` & `kgdata-7.0.4/src/python/models/entity_metadata.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/python/models/iterators.rs` & `kgdata-7.0.4/src/python/models/iterators.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/python/models/mod.rs` & `kgdata-7.0.4/src/python/models/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/python/models/multilingual.rs` & `kgdata-7.0.4/src/python/models/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/python/models/property.rs` & `kgdata-7.0.4/src/python/models/property.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/python/models/value.rs` & `kgdata-7.0.4/src/python/models/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/src/python/scripts.rs` & `kgdata-7.0.4/src/python/scripts.rs`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/pyproject.toml` & `kgdata-7.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kgdata"
-version = "7.0.2"
+version = "7.0.4"
 description = "Library to process dumps of knowledge graphs (Wikipedia, DBpedia, Wikidata)"
 readme = "README.md"
 authors = [{ name = "Binh Vu", email = "binh@toan2.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -21,21 +21,20 @@
     'six >= 1.16.0, < 2.0.0',
     'ruamel.yaml >= 0.17.21, < 0.18.0',
     'chardet >= 5.0.0, < 6.0.0',
     'ujson >= 5.5.0, < 6.0.0',
     'redis >= 3.5.3, < 4.0.0',
     'numpy >= 1.22.3, < 2.0.0',
     'requests >= 2.28.0, < 3.0.0',
-    'sem-desc >= 6.7.2, < 7.0.0',
+    'sem-desc >= 6.11.2, < 7.0.0',
     'click >= 8.1.3, < 9.0.0',
     'parsimonious >= 0.8.1, < 0.9.0',
     'hugedict >= 2.12.10, < 3.0.0',
     'rsoup >= 3.1.7, < 4.0.0',
     'lxml >= 4.9.0, < 5.0.0',
-    'ray >= 2.0.1, < 3.0.0',
     'pqdict >= 1.3.0, < 2.0.0',
     'ftfy >= 6.1.3, < 7.0.0',
 ]
 
 [project.urls]
 homepage = "https://github.com/binh-vu/kgdata"
 repository = "https://github.com/binh-vu/kgdata"
@@ -43,15 +42,16 @@
 [project.optional-dependencies]
 dev = [
     'python-dotenv >= 0.19.0, < 0.20.0',
     'pytest >= 7.1.3, < 8.0.0',
     'black >= 22.10.0, < 23.0.0',
 ]
 spark = ['pyspark >= 3.5.0, < 4.0.0']
-all = ["kgdata[dev,spark]"]
+ray = ['ray >= 2.0.1, < 3.0.0']
+all = ["kgdata[dev,spark,ray]"]
 
 [tool.maturin]
 module-name = "kgdata.core"
 features = ["extension-module"]
 
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
```

### Comparing `kgdata-7.0.2/kgdata/wikipedia/config.py` & `kgdata-7.0.4/kgdata/wikipedia/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/misc.py` & `kgdata-7.0.4/kgdata/wikipedia/misc.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/article_metadata.py` & `kgdata-7.0.4/kgdata/wikipedia/datasets/article_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/mention_to_articles.py` & `kgdata-7.0.4/kgdata/wikipedia/datasets/mention_to_articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/linked_relational_tables.py` & `kgdata-7.0.4/kgdata/wikipedia/datasets/linked_relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/articles.py.deprecated` & `kgdata-7.0.4/kgdata/wikipedia/datasets/articles.py.deprecated`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/grouped_articles.py.deprecated` & `kgdata-7.0.4/kgdata/wikipedia/datasets/grouped_articles.py.deprecated`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/easy_tables_metadata.py` & `kgdata-7.0.4/kgdata/wikipedia/datasets/easy_tables_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/article_aliases.py` & `kgdata-7.0.4/kgdata/wikipedia/datasets/article_aliases.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/html_articles.py` & `kgdata-7.0.4/kgdata/wikipedia/datasets/html_articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/article_links.py` & `kgdata-7.0.4/kgdata/wikipedia/datasets/article_links.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/easy_tables.py` & `kgdata-7.0.4/kgdata/wikipedia/datasets/easy_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/html_tables.py` & `kgdata-7.0.4/kgdata/wikipedia/datasets/html_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/article_degrees.py` & `kgdata-7.0.4/kgdata/wikipedia/datasets/article_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/datasets/relational_tables.py` & `kgdata-7.0.4/kgdata/wikipedia/datasets/relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/wikiapi.py` & `kgdata-7.0.4/kgdata/wikipedia/wikiapi.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/models/page_article.py` & `kgdata-7.0.4/kgdata/wikipedia/models/page_article.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/models/linked_html_table.py` & `kgdata-7.0.4/kgdata/wikipedia/models/linked_html_table.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikipedia/models/html_article.py` & `kgdata-7.0.4/kgdata/wikipedia/models/html_article.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/db.py` & `kgdata-7.0.4/kgdata/db.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/db.py` & `kgdata-7.0.4/kgdata/wikidata/db.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/extra_ent_db.py` & `kgdata-7.0.4/kgdata/wikidata/extra_ent_db.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/wikidata_prefixes.yml` & `kgdata-7.0.4/kgdata/wikidata/wikidata_prefixes.yml`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/config.py` & `kgdata-7.0.4/kgdata/wikidata/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/__main__.py` & `kgdata-7.0.4/kgdata/wikidata/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 from hugedict.prelude import (
     RocksDBDict,
     RocksDBOptions,
     init_env_logger,
     rocksdb_build_sst_file,
     rocksdb_ingest_sst_files,
 )
+from sm.misc.ray_helper import ray_map, ray_put
+from timer import Timer
+
 from kgdata.config import init_dbdir_from_env
 from kgdata.db import build_database
 from kgdata.wikidata.config import WikidataDirCfg
 from kgdata.wikidata.datasets.class_count import class_count
 from kgdata.wikidata.datasets.property_count import property_count
 from kgdata.wikidata.db import WikidataDB, get_ontcount_db, pack_int
 from kgdata.wikidata.extra_ent_db import EntAttr, build_extra_ent_db
-from timer import Timer
 
 if TYPE_CHECKING:
     from hugedict.core.rocksdb import FileFormat
 
 
 def dataset2db(
     dataset: str,
@@ -244,19 +246,15 @@
 
     options = cast(
         RocksDBDict,
         get_ontcount_db(dbpath, create_if_missing=True, read_only=False),
     ).options
     gc.collect()
 
-    import ray
-    from sm.misc.ray_helper import ray_map, ray_put
-
-    ray.init()
-
+    
     def _build_sst_file(
         infile: str, temp_dir: str, posfix: str, options: RocksDBOptions
     ):
         kvs = []
         for obj in serde.jl.deser(infile):
             kvs.append((obj[0].encode(), pack_int(obj[1])))
         kvs.sort(key=itemgetter(0))
```

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_outlinks.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_outlinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/main_property_connections.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/main_property_connections.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_metadata.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_types_and_degrees.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_types_and_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/classes.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/properties.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/properties.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_redirection_dump.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_redirection_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_types.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/page_dump.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/page_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entities.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from functools import lru_cache, partial
 from typing import Dict, Optional, Set, Union
 
 import orjson
 from loguru import logger
-from pyspark import Broadcast
 from sm.misc.funcs import filter_duplication, is_not_null
 
 from kgdata.dataset import Dataset
 from kgdata.misc.funcs import split_tab_2
+from kgdata.misc.optional_import import Broadcast
 from kgdata.spark import get_spark_context
 from kgdata.wikidata.config import WikidataDirCfg
 from kgdata.wikidata.datasets.entity_dump import entity_dump
 from kgdata.wikidata.datasets.entity_ids import entity_ids
 from kgdata.wikidata.datasets.entity_redirections import entity_redirections
 from kgdata.wikidata.models.wdentity import WDEntity
 from kgdata.wikidata.models.wdstatement import WDStatement
```

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_dump.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/property_ranges.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/property_ranges.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/meta_graph.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/meta_graph.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_degrees.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/property_domains.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/property_domains.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_ids.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/norm_mentions.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/norm_mentions.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_all_types.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_all_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/__main__.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_redirections.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_redirections.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/page_ids.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/meta_graph_stats.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/meta_graph_stats.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_wiki_aliases.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_wiki_aliases.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/cross_wiki_mapping.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/cross_wiki_mapping.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_labels.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_labels.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/triple_truthy_dump.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/triple_truthy_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/mention_to_entities.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/mention_to_entities.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/class_count.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/class_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/property_count.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/property_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/entity_pagerank.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/entity_pagerank.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/datasets/ontology_count.py` & `kgdata-7.0.4/kgdata/wikidata/datasets/ontology_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/models/wdentitylabel.py` & `kgdata-7.0.4/kgdata/wikidata/models/wdentitylabel.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/models/wdentity.py` & `kgdata-7.0.4/kgdata/wikidata/models/wdentity.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/models/wdentitymetadata.py` & `kgdata-7.0.4/kgdata/wikidata/models/wdentitymetadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/models/wdproperty.py` & `kgdata-7.0.4/kgdata/wikidata/models/wdproperty.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/models/__init__.py` & `kgdata-7.0.4/kgdata/wikidata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/models/propertystats.py` & `kgdata-7.0.4/kgdata/wikidata/models/propertystats.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/models/wdstatement.py` & `kgdata-7.0.4/kgdata/wikidata/models/wdstatement.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/models/wdvalue.py` & `kgdata-7.0.4/kgdata/wikidata/models/wdvalue.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/wikidata/models/wdclass.py` & `kgdata-7.0.4/kgdata/wikidata/models/wdclass.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/splitter.py` & `kgdata-7.0.4/kgdata/splitter.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/misc/modification.py` & `kgdata-7.0.4/kgdata/misc/modification.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/misc/resource.py` & `kgdata-7.0.4/kgdata/misc/resource.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/misc/ntriples_parser.py` & `kgdata-7.0.4/kgdata/misc/ntriples_parser.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/misc/funcs.py` & `kgdata-7.0.4/kgdata/misc/funcs.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/misc/hierarchy.py` & `kgdata-7.0.4/kgdata/misc/hierarchy.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/misc/download.py` & `kgdata-7.0.4/kgdata/misc/download.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/misc/query.py` & `kgdata-7.0.4/kgdata/misc/query.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/config.py` & `kgdata-7.0.4/kgdata/dbpedia/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/__main__.py` & `kgdata-7.0.4/kgdata/dbpedia/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_metadata.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/entity_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_types_and_degrees.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/entity_types_and_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/classes.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/properties.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/properties.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_types.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/entity_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/generic_extractor_dump.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/generic_extractor_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/entities.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/meta_graph.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/meta_graph.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/wikilinks.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/wikilinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_degrees.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/entity_degrees.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/mapping_extractor_dump.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/mapping_extractor_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/wikilink_dump.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/wikilink_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_all_types.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/entity_all_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/__main__.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/ontology_dump.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/ontology_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_redirections.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/entity_redirections.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/page_ids.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/meta_graph_stats.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/meta_graph_stats.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/entity_labels.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/entity_labels.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/page_id_dump.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/page_id_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dbpedia/datasets/class_count.py` & `kgdata-7.0.4/kgdata/dbpedia/datasets/class_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/config.py` & `kgdata-7.0.4/kgdata/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/dataset.py` & `kgdata-7.0.4/kgdata/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 )
 
 import click
 import serde.byteline
 import serde.json
 import serde.textline
 from hugedict.misc import Chain2, identity
+from loguru import logger
+from tqdm.auto import tqdm
+
 from kgdata.config import init_dbdir_from_env
+from kgdata.misc.optional_import import RDD
 from kgdata.misc.query import PropQuery, every
 from kgdata.spark import ExtendedRDD, SparkLikeInterface, get_spark_context
 from kgdata.spark.common import does_result_dir_exist, text_file
 from kgdata.spark.extended_rdd import DatasetSignature
-from loguru import logger
-from pyspark import RDD
-from tqdm.auto import tqdm
 
 V = TypeVar("V")
 V2 = TypeVar("V2")
 T_co = TypeVar("T_co", covariant=True)
 K = TypeVar("K", bound=Hashable)
```

### Comparing `kgdata-7.0.2/kgdata/spark/common.py` & `kgdata-7.0.4/kgdata/spark/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,33 +23,41 @@
     TypeVar,
     Union,
     cast,
 )
 
 import orjson
 import zstandard as zstd
-from kgdata.misc.funcs import deser_zstd_records
 from loguru import logger
-from pyspark import RDD, SparkConf, SparkContext, TaskContext
 from sm.misc.funcs import assert_not_null
 
+from kgdata.misc.funcs import deser_zstd_records
+from kgdata.misc.optional_import import (
+    RDD,
+    SparkConf,
+    SparkContext,
+    TaskContext,
+    require_spark,
+)
+
 # SparkContext singleton
 _sc = None
 StrPath = Union[Path, str]
 
 R1 = TypeVar("R1")
 R2 = TypeVar("R2")
 R3 = TypeVar("R3")
 K1 = TypeVar("K1")
 K2 = TypeVar("K2")
 K = TypeVar("K")
 V = TypeVar("V")
 V2 = TypeVar("V2")
 
 
+@require_spark
 def get_spark_context() -> SparkContext:
     """Get spark context
 
     Returns
     -------
     SparkContext
     """
@@ -455,15 +463,15 @@
     return get_spark_context().textFile(outfile).map(deserfn)
 
 
 def fix_rdd():
     # template to fix an rdd
     # ###############################
     # TODO: set input file
-    indir = "/nas/home/binhvu/workspace/sm-dev/data/wikidata/step_2/schema"
+    indir = os.path.expanduser("~/workspace/sm-dev/data/wikidata/step_2/schema")
     infile = indir + "/class_schema"
 
     # ###############################
     newfile = infile + "_new"
     rdd = get_spark_context().textFile(infile)
 
     # ###############################
@@ -630,10 +638,8 @@
     )
     for r in records:
         print(r[0], r[1][0], r[1][1])
 
 
 @dataclass
 class EmptyBroadcast(Generic[V]):
-    value: V
-    value: V
-    value: V
+    value: V
```

### Comparing `kgdata-7.0.2/kgdata/spark/rdd_alike.py` & `kgdata-7.0.4/kgdata/spark/rdd_alike.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/spark/extended_rdd.py` & `kgdata-7.0.4/kgdata/spark/extended_rdd.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,27 +19,27 @@
     Protocol,
     Sequence,
     TypeVar,
     Union,
 )
 
 import serde.json
-from kgdata.misc.funcs import deser_zstd_records
+from typing_extensions import TypeGuard
+
+from kgdata.misc.optional_import import RDD, portable_hash
 from kgdata.spark.common import (
     StrPath,
     are_records_unique,
     estimate_num_partitions,
     get_spark_context,
     join_repartition,
     left_outer_join_repartition,
     save_as_text_file,
     text_file,
 )
-from pyspark.rdd import RDD, portable_hash
-from typing_extensions import TypeGuard
 
 if TYPE_CHECKING:
     from kgdata.dataset import Dataset
 
 
 class SupportsOrdering(Protocol):
     def __lt__(self, other: SupportsOrdering) -> bool: ...
```

### Comparing `kgdata-7.0.2/kgdata/core/base.pyi` & `kgdata-7.0.4/kgdata/core/base.pyi`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/core/models.pyi` & `kgdata-7.0.4/kgdata/core/models.pyi`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/models/ont_class.py` & `kgdata-7.0.4/kgdata/models/ont_class.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/models/multilingual.py` & `kgdata-7.0.4/kgdata/models/multilingual.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/models/entity.py` & `kgdata-7.0.4/kgdata/models/entity.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/kgdata/models/ont_property.py` & `kgdata-7.0.4/kgdata/models/ont_property.py`

 * *Files identical despite different names*

### Comparing `kgdata-7.0.2/PKG-INFO` & `kgdata-7.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.3
 Name: kgdata
-Version: 7.0.2
+Version: 7.0.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: orjson >=3.9.0, <4.0.0
 Requires-Dist: tqdm >=4.64.0, <5.0.0
 Requires-Dist: beautifulsoup4 >=4.9.3, <5.0.0
 Requires-Dist: loguru >=0.7.0, <0.8.0
 Requires-Dist: rdflib >=7.0.0, <8.0.0
 Requires-Dist: six >=1.16.0, <2.0.0
 Requires-Dist: ruamel-yaml >=0.17.21, <0.18.0
 Requires-Dist: chardet >=5.0.0, <6.0.0
 Requires-Dist: ujson >=5.5.0, <6.0.0
 Requires-Dist: redis >=3.5.3, <4.0.0
 Requires-Dist: numpy >=1.22.3, <2.0.0
 Requires-Dist: requests >=2.28.0, <3.0.0
-Requires-Dist: sem-desc >=6.7.2, <7.0.0
+Requires-Dist: sem-desc >=6.11.2, <7.0.0
 Requires-Dist: click >=8.1.3, <9.0.0
 Requires-Dist: parsimonious >=0.8.1, <0.9.0
 Requires-Dist: hugedict >=2.12.10, <3.0.0
 Requires-Dist: rsoup >=3.1.7, <4.0.0
 Requires-Dist: lxml >=4.9.0, <5.0.0
-Requires-Dist: ray >=2.0.1, <3.0.0
 Requires-Dist: pqdict >=1.3.0, <2.0.0
 Requires-Dist: ftfy >=6.1.3, <7.0.0
 Requires-Dist: python-dotenv >=0.19.0, <0.20.0 ; extra == 'dev'
 Requires-Dist: pytest >=7.1.3, <8.0.0 ; extra == 'dev'
 Requires-Dist: black >=22.10.0, <23.0.0 ; extra == 'dev'
 Requires-Dist: pyspark >=3.5.0, <4.0.0 ; extra == 'spark'
-Requires-Dist: kgdata[dev,spark] ; extra == 'all'
+Requires-Dist: ray >=2.0.1, <3.0.0 ; extra == 'ray'
+Requires-Dist: kgdata[dev,spark,ray] ; extra == 'all'
 Provides-Extra: dev
 Provides-Extra: spark
+Provides-Extra: ray
 Provides-Extra: all
 License-File: LICENSE
 License-File: LICENSE
 Summary: Library to process dumps of knowledge graphs (Wikipedia, DBpedia, Wikidata)
 Keywords: knowledge-graph,wikidata,wikipedia,dbpedia
 Home-Page: https://github.com/binh-vu/kgdata
 Author-email: Binh Vu <binh@toan2.com>
```

