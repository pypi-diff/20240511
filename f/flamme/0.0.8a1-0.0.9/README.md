# Comparing `tmp/flamme-0.0.8a1.tar.gz` & `tmp/flamme-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamme-0.0.8a1.tar", max compression
+gzip compressed data, was "flamme-0.0.9.tar", max compression
```

## Comparing `flamme-0.0.8a1.tar` & `flamme-0.0.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1501 2023-12-26 20:16:03.743225 flamme-0.0.8a1/LICENSE
--rw-r--r--   0        0        0     3628 2023-12-26 20:16:03.743225 flamme-0.0.8a1/README.md
--rw-r--r--   0        0        0     4478 2023-12-26 20:16:03.743225 flamme-0.0.8a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/__init__.py
--rw-r--r--   0        0        0     1399 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/__init__.py
--rw-r--r--   0        0        0     3673 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/base.py
--rw-r--r--   0        0        0     2071 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/column.py
--rw-r--r--   0        0        0     6877 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/continuous.py
--rw-r--r--   0        0        0     5942 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/discrete.py
--rw-r--r--   0        0        0     1257 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/dtype.py
--rw-r--r--   0        0        0     1783 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/duplicate.py
--rw-r--r--   0        0        0     1856 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/filter.py
--rw-r--r--   0        0        0     1969 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/mapping.py
--rw-r--r--   0        0        0      925 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/markdown.py
--rw-r--r--   0        0        0     4542 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/null.py
--rw-r--r--   0        0        0     3210 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/null_temp_col.py
--rw-r--r--   0        0        0     2714 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/analyzer/null_temp_global.py
--rw-r--r--   0        0        0      485 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/ingestor/__init__.py
--rw-r--r--   0        0        0     3009 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/ingestor/base.py
--rw-r--r--   0        0        0     1517 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/ingestor/csv.py
--rw-r--r--   0        0        0     1565 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/ingestor/parquet.py
--rw-r--r--   0        0        0     1943 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/ingestor/transform.py
--rw-r--r--   0        0        0     1124 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/ingestor/vanilla.py
--rw-r--r--   0        0        0      341 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/reporter/__init__.py
--rw-r--r--   0        0        0     5263 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/reporter/base.py
--rw-r--r--   0        0        0     2205 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/reporter/no_repeat.py
--rw-r--r--   0        0        0      824 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/reporter/utils.py
--rw-r--r--   0        0        0     3689 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/reporter/vanilla.py
--rw-r--r--   0        0        0     1243 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/__init__.py
--rw-r--r--   0        0        0     1773 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/base.py
--rw-r--r--   0        0        0    14559 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/continuous.py
--rw-r--r--   0        0        0    10162 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/continuous_temporal.py
--rw-r--r--   0        0        0     7797 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/discrete.py
--rw-r--r--   0        0        0     5918 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/discrete_temporal.py
--rw-r--r--   0        0        0     3783 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/dtype.py
--rw-r--r--   0        0        0     4319 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/duplicate.py
--rw-r--r--   0        0        0      644 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/empty.py
--rw-r--r--   0        0        0     2270 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/mapping.py
--rw-r--r--   0        0        0     1607 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/markdown.py
--rw-r--r--   0        0        0    15444 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/null.py
--rw-r--r--   0        0        0     8530 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/null_temp_col.py
--rw-r--r--   0        0        0     9952 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/null_temp_global.py
--rw-r--r--   0        0        0     1804 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/section/utils.py
--rw-r--r--   0        0        0        0 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/transformer/__init__.py
--rw-r--r--   0        0        0     2092 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/transformer/df/__init__.py
--rw-r--r--   0        0        0     4743 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/transformer/df/base.py
--rw-r--r--   0        0        0     2657 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/transformer/df/column.py
--rw-r--r--   0        0        0     2002 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/transformer/df/datetime.py
--rw-r--r--   0        0        0     2037 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/transformer/df/decimal.py
--rw-r--r--   0        0        0     2259 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/transformer/df/null.py
--rw-r--r--   0        0        0     2047 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/transformer/df/numeric.py
--rw-r--r--   0        0        0     1762 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/transformer/df/selection.py
--rw-r--r--   0        0        0     2614 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/transformer/df/sequential.py
--rw-r--r--   0        0        0     1954 2023-12-26 20:16:03.743225 flamme-0.0.8a1/src/flamme/transformer/df/string.py
--rw-r--r--   0        0        0     1161 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/transformer/series/__init__.py
--rw-r--r--   0        0        0     3698 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/transformer/series/base.py
--rw-r--r--   0        0        0     1283 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/transformer/series/datetime.py
--rw-r--r--   0        0        0     1251 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/transformer/series/numeric.py
--rw-r--r--   0        0        0     1778 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/transformer/series/sequential.py
--rw-r--r--   0        0        0     1014 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/transformer/series/string.py
--rw-r--r--   0        0        0      110 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/__init__.py
--rw-r--r--   0        0        0     4136 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/columns.py
--rw-r--r--   0        0        0     1624 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/dtype.py
--rw-r--r--   0        0        0      955 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/factory.py
--rw-r--r--   0        0        0     2598 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/figure.py
--rw-r--r--   0        0        0     2870 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/filtering.py
--rw-r--r--   0        0        0      889 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/format.py
--rw-r--r--   0        0        0     1581 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/io.py
--rw-r--r--   0        0        0      515 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/mapping.py
--rw-r--r--   0        0        0     3150 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/mathnan.py
--rw-r--r--   0        0        0     1572 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/null.py
--rw-r--r--   0        0        0     1679 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/path.py
--rw-r--r--   0        0        0     1721 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/range.py
--rw-r--r--   0        0        0     2200 2023-12-26 20:16:03.747225 flamme-0.0.8a1/src/flamme/utils/sorting.py
--rw-r--r--   0        0        0     4983 1970-01-01 00:00:00.000000 flamme-0.0.8a1/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-12-27 00:28:26.930388 flamme-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3845 2023-12-27 00:28:26.930388 flamme-0.0.9/README.md
+-rw-r--r--   0        0        0     4493 2023-12-27 00:28:26.930388 flamme-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/__init__.py
+-rw-r--r--   0        0        0     1399 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/__init__.py
+-rw-r--r--   0        0        0     3673 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/base.py
+-rw-r--r--   0        0        0     2071 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/column.py
+-rw-r--r--   0        0        0     6877 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/continuous.py
+-rw-r--r--   0        0        0     5942 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/discrete.py
+-rw-r--r--   0        0        0     1257 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/dtype.py
+-rw-r--r--   0        0        0     1783 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/duplicate.py
+-rw-r--r--   0        0        0     1856 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/filter.py
+-rw-r--r--   0        0        0     1969 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/mapping.py
+-rw-r--r--   0        0        0      925 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/markdown.py
+-rw-r--r--   0        0        0     4542 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/null.py
+-rw-r--r--   0        0        0     3210 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/null_temp_col.py
+-rw-r--r--   0        0        0     2714 2023-12-27 00:28:26.930388 flamme-0.0.9/src/flamme/analyzer/null_temp_global.py
+-rw-r--r--   0        0        0      485 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/ingestor/__init__.py
+-rw-r--r--   0        0        0     3009 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/ingestor/base.py
+-rw-r--r--   0        0        0     1517 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/ingestor/csv.py
+-rw-r--r--   0        0        0     1565 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/ingestor/parquet.py
+-rw-r--r--   0        0        0     1943 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/ingestor/transform.py
+-rw-r--r--   0        0        0     1124 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/ingestor/vanilla.py
+-rw-r--r--   0        0        0      341 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/reporter/__init__.py
+-rw-r--r--   0        0        0     5263 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/reporter/base.py
+-rw-r--r--   0        0        0     2205 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/reporter/no_repeat.py
+-rw-r--r--   0        0        0      824 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/reporter/utils.py
+-rw-r--r--   0        0        0     3689 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/reporter/vanilla.py
+-rw-r--r--   0        0        0     1243 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/__init__.py
+-rw-r--r--   0        0        0     1773 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/base.py
+-rw-r--r--   0        0        0    14559 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/continuous.py
+-rw-r--r--   0        0        0    10162 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/continuous_temporal.py
+-rw-r--r--   0        0        0     7797 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/discrete.py
+-rw-r--r--   0        0        0     5918 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/discrete_temporal.py
+-rw-r--r--   0        0        0     3783 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/dtype.py
+-rw-r--r--   0        0        0     4319 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/duplicate.py
+-rw-r--r--   0        0        0      644 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/empty.py
+-rw-r--r--   0        0        0     2270 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/mapping.py
+-rw-r--r--   0        0        0     1607 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/markdown.py
+-rw-r--r--   0        0        0    15444 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/null.py
+-rw-r--r--   0        0        0     8530 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/null_temp_col.py
+-rw-r--r--   0        0        0     9952 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/null_temp_global.py
+-rw-r--r--   0        0        0     1804 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/section/utils.py
+-rw-r--r--   0        0        0        0 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/__init__.py
+-rw-r--r--   0        0        0     2092 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/df/__init__.py
+-rw-r--r--   0        0        0     4743 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/df/base.py
+-rw-r--r--   0        0        0     2657 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/df/column.py
+-rw-r--r--   0        0        0     2002 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/df/datetime.py
+-rw-r--r--   0        0        0     2037 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/df/decimal.py
+-rw-r--r--   0        0        0     2259 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/df/null.py
+-rw-r--r--   0        0        0     2047 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/df/numeric.py
+-rw-r--r--   0        0        0     1762 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/df/selection.py
+-rw-r--r--   0        0        0     2614 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/df/sequential.py
+-rw-r--r--   0        0        0     1954 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/df/string.py
+-rw-r--r--   0        0        0     1161 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/series/__init__.py
+-rw-r--r--   0        0        0     3698 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/series/base.py
+-rw-r--r--   0        0        0     1283 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/series/datetime.py
+-rw-r--r--   0        0        0     1251 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/series/numeric.py
+-rw-r--r--   0        0        0     1778 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/series/sequential.py
+-rw-r--r--   0        0        0     1014 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/transformer/series/string.py
+-rw-r--r--   0        0        0      110 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/__init__.py
+-rw-r--r--   0        0        0     4136 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/columns.py
+-rw-r--r--   0        0        0     1624 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/dtype.py
+-rw-r--r--   0        0        0      955 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/factory.py
+-rw-r--r--   0        0        0     2598 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/figure.py
+-rw-r--r--   0        0        0     2870 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/filtering.py
+-rw-r--r--   0        0        0      889 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/format.py
+-rw-r--r--   0        0        0     1581 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/io.py
+-rw-r--r--   0        0        0      515 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/mapping.py
+-rw-r--r--   0        0        0     3150 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/mathnan.py
+-rw-r--r--   0        0        0     1572 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/null.py
+-rw-r--r--   0        0        0     1679 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/path.py
+-rw-r--r--   0        0        0     1721 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/range.py
+-rw-r--r--   0        0        0     2200 2023-12-27 00:28:26.934388 flamme-0.0.9/src/flamme/utils/sorting.py
+-rw-r--r--   0        0        0     5249 1970-01-01 00:00:00.000000 flamme-0.0.9/PKG-INFO
```

### Comparing `flamme-0.0.8a1/LICENSE` & `flamme-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/README.md` & `flamme-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -69,10 +69,11 @@
 pip install flamme[all]
 ```
 
 Please check the [get started page](https://durandtibo.github.io/flamme/get_started) to see how to
 install only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `flamme` versions and tested dependencies.
 
-| `flamme` | `coola`      | `jinja2`     | `markdown`   | `matplotlib` | `objectory`  | `pandas`     | `pyarrow`      | `tqdm`         | `python`      |
-|----------|--------------|--------------|--------------|--------------|--------------|--------------|----------------|----------------|---------------|
-| `main`   | `>=0.2,<0.3` | `>=3.0,<3.2` | `>=3.4,<3.6` | `>=3.6,<4.0` | `>=0.1,<0.2` | `>=1.3,<2.2` | `>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.12` |
+| `flamme` | `coola`      | `jinja2`     | `markdown`   | `matplotlib` | `numpy`       | `objectory`  | `pandas`     | `pyarrow`      | `tqdm`         | `python`      |
+|----------|--------------|--------------|--------------|--------------|---------------|--------------|--------------|----------------|----------------|---------------|
+| `main`   | `>=0.2,<0.3` | `>=3.0,<3.2` | `>=3.4,<3.6` | `>=3.6,<4.0` | `>=1.23,<2.0` | `>=0.1,<0.2` | `>=1.3,<2.2` | `>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.13` |
+| `0.0.8`  | `>=0.2,<0.3` | `>=3.0,<3.2` | `>=3.4,<3.6` | `>=3.6,<4.0` | `>=1.23,<2.0` | `>=0.1,<0.2` | `>=1.3,<2.2` | `>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.12` |
```

#### html2text {}

```diff
@@ -12,12 +12,15 @@
 install flamme ``` To make the package as slim as possible, only the minimal
 packages required to use `flamme` are installed. To include all the
 dependencies, you can use the following command: ```shell pip install flamme
 [all] ``` Please check the [get started page](https://durandtibo.github.io/
 flamme/get_started) to see how to install only some specific dependencies or
 other alternatives to install the library. The following is the corresponding
 `flamme` versions and tested dependencies. | `flamme` | `coola` | `jinja2` |
-`markdown` | `matplotlib` | `objectory` | `pandas` | `pyarrow` | `tqdm` |
-`python` | |----------|--------------|--------------|--------------|-----------
----|--------------|--------------|----------------|----------------|-----------
-----| | `main` | `>=0.2,<0.3` | `>=3.0,<3.2` | `>=3.4,<3.6` | `>=3.6,<4.0` |
-`>=0.1,<0.2` | `>=1.3,<2.2` | `>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.12` |
+`markdown` | `matplotlib` | `numpy` | `objectory` | `pandas` | `pyarrow` |
+`tqdm` | `python` | |----------|--------------|--------------|--------------|--
+------------|---------------|--------------|--------------|----------------|---
+-------------|---------------| | `main` | `>=0.2,<0.3` | `>=3.0,<3.2` |
+`>=3.4,<3.6` | `>=3.6,<4.0` | `>=1.23,<2.0` | `>=0.1,<0.2` | `>=1.3,<2.2` |
+`>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.13` | | `0.0.8` | `>=0.2,<0.3` |
+`>=3.0,<3.2` | `>=3.4,<3.6` | `>=3.6,<4.0` | `>=1.23,<2.0` | `>=0.1,<0.2` |
+`>=1.3,<2.2` | `>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.12` |
```

### Comparing `flamme-0.0.8a1/pyproject.toml` & `flamme-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flamme"
-version = "0.0.8a1"
+version = "0.0.9"
 description = "A library to generate custom reports of pandas DataFrames"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/flamme"
 repository = "https://github.com/durandtibo/flamme"
 keywords = ["pandas", "analysis", "report"]
 license = "BSD-3-Clause"
@@ -15,33 +15,34 @@
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries",
 ]
 
 packages = [
     { include = "flamme", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
 coola = ">=0.2.0,<0.3"
 jinja2 = ">=3.0,<4.0"
 markdown = ">=3.4,<4.0"
-matplotlib = ">=3.6,<4.0"  # TODO: add checks and docs
+matplotlib = ">=3.6,<4.0"
 numpy = ">=1.23,<2.0"
 objectory = ">=0.1,<0.2"
 pandas = ">=1.3,<3.0"
 pyarrow = ">=10.0,<15.0"
-python = ">=3.9,<3.12"
+python = ">=3.9,<3.13"
 tqdm = ">=4.65,<5.0"
 
 # Optional dependencies
 
 
 [tool.poetry.extras]
 all = []
```

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/__init__.py` & `flamme-0.0.9/src/flamme/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/base.py` & `flamme-0.0.9/src/flamme/analyzer/base.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/column.py` & `flamme-0.0.9/src/flamme/analyzer/column.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/continuous.py` & `flamme-0.0.9/src/flamme/analyzer/continuous.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/discrete.py` & `flamme-0.0.9/src/flamme/analyzer/discrete.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/dtype.py` & `flamme-0.0.9/src/flamme/analyzer/dtype.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/duplicate.py` & `flamme-0.0.9/src/flamme/analyzer/duplicate.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/filter.py` & `flamme-0.0.9/src/flamme/analyzer/filter.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/mapping.py` & `flamme-0.0.9/src/flamme/analyzer/mapping.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/markdown.py` & `flamme-0.0.9/src/flamme/analyzer/markdown.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/null.py` & `flamme-0.0.9/src/flamme/analyzer/null.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/null_temp_col.py` & `flamme-0.0.9/src/flamme/analyzer/null_temp_col.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/analyzer/null_temp_global.py` & `flamme-0.0.9/src/flamme/analyzer/null_temp_global.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/ingestor/base.py` & `flamme-0.0.9/src/flamme/ingestor/base.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/ingestor/csv.py` & `flamme-0.0.9/src/flamme/ingestor/csv.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/ingestor/parquet.py` & `flamme-0.0.9/src/flamme/ingestor/parquet.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/ingestor/transform.py` & `flamme-0.0.9/src/flamme/ingestor/transform.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/ingestor/vanilla.py` & `flamme-0.0.9/src/flamme/ingestor/vanilla.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/reporter/base.py` & `flamme-0.0.9/src/flamme/reporter/base.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/reporter/no_repeat.py` & `flamme-0.0.9/src/flamme/reporter/no_repeat.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/reporter/utils.py` & `flamme-0.0.9/src/flamme/reporter/utils.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/reporter/vanilla.py` & `flamme-0.0.9/src/flamme/reporter/vanilla.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/__init__.py` & `flamme-0.0.9/src/flamme/section/__init__.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/base.py` & `flamme-0.0.9/src/flamme/section/base.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/continuous.py` & `flamme-0.0.9/src/flamme/section/continuous.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/continuous_temporal.py` & `flamme-0.0.9/src/flamme/section/continuous_temporal.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/discrete.py` & `flamme-0.0.9/src/flamme/section/discrete.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/discrete_temporal.py` & `flamme-0.0.9/src/flamme/section/discrete_temporal.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/dtype.py` & `flamme-0.0.9/src/flamme/section/dtype.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/duplicate.py` & `flamme-0.0.9/src/flamme/section/duplicate.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/empty.py` & `flamme-0.0.9/src/flamme/section/empty.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/mapping.py` & `flamme-0.0.9/src/flamme/section/mapping.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/markdown.py` & `flamme-0.0.9/src/flamme/section/markdown.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/null.py` & `flamme-0.0.9/src/flamme/section/null.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/null_temp_col.py` & `flamme-0.0.9/src/flamme/section/null_temp_col.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/null_temp_global.py` & `flamme-0.0.9/src/flamme/section/null_temp_global.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/section/utils.py` & `flamme-0.0.9/src/flamme/section/utils.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/df/__init__.py` & `flamme-0.0.9/src/flamme/transformer/df/__init__.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/df/base.py` & `flamme-0.0.9/src/flamme/transformer/df/base.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/df/column.py` & `flamme-0.0.9/src/flamme/transformer/df/column.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/df/datetime.py` & `flamme-0.0.9/src/flamme/transformer/df/datetime.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/df/decimal.py` & `flamme-0.0.9/src/flamme/transformer/df/decimal.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/df/null.py` & `flamme-0.0.9/src/flamme/transformer/df/null.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/df/numeric.py` & `flamme-0.0.9/src/flamme/transformer/df/numeric.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/df/selection.py` & `flamme-0.0.9/src/flamme/transformer/df/selection.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/df/sequential.py` & `flamme-0.0.9/src/flamme/transformer/df/sequential.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/df/string.py` & `flamme-0.0.9/src/flamme/transformer/df/string.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/series/__init__.py` & `flamme-0.0.9/src/flamme/transformer/series/__init__.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/series/base.py` & `flamme-0.0.9/src/flamme/transformer/series/base.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/series/datetime.py` & `flamme-0.0.9/src/flamme/transformer/series/datetime.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/series/numeric.py` & `flamme-0.0.9/src/flamme/transformer/series/numeric.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/series/sequential.py` & `flamme-0.0.9/src/flamme/transformer/series/sequential.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/transformer/series/string.py` & `flamme-0.0.9/src/flamme/transformer/series/string.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/columns.py` & `flamme-0.0.9/src/flamme/utils/columns.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/dtype.py` & `flamme-0.0.9/src/flamme/utils/dtype.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/factory.py` & `flamme-0.0.9/src/flamme/utils/factory.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/figure.py` & `flamme-0.0.9/src/flamme/utils/figure.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/filtering.py` & `flamme-0.0.9/src/flamme/utils/filtering.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/format.py` & `flamme-0.0.9/src/flamme/utils/format.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/io.py` & `flamme-0.0.9/src/flamme/utils/io.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/mapping.py` & `flamme-0.0.9/src/flamme/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/mathnan.py` & `flamme-0.0.9/src/flamme/utils/mathnan.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/null.py` & `flamme-0.0.9/src/flamme/utils/null.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/path.py` & `flamme-0.0.9/src/flamme/utils/path.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/range.py` & `flamme-0.0.9/src/flamme/utils/range.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/src/flamme/utils/sorting.py` & `flamme-0.0.9/src/flamme/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `flamme-0.0.8a1/PKG-INFO` & `flamme-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: flamme
-Version: 0.0.8a1
+Version: 0.0.9
 Summary: A library to generate custom reports of pandas DataFrames
 Home-page: https://github.com/durandtibo/flamme
 License: BSD-3-Clause
 Keywords: pandas,analysis,report
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: all
 Requires-Dist: coola (>=0.2.0,<0.3)
 Requires-Dist: jinja2 (>=3.0,<4.0)
 Requires-Dist: markdown (>=3.4,<4.0)
 Requires-Dist: matplotlib (>=3.6,<4.0)
@@ -104,11 +105,12 @@
 pip install flamme[all]
 ```
 
 Please check the [get started page](https://durandtibo.github.io/flamme/get_started) to see how to
 install only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `flamme` versions and tested dependencies.
 
-| `flamme` | `coola`      | `jinja2`     | `markdown`   | `matplotlib` | `objectory`  | `pandas`     | `pyarrow`      | `tqdm`         | `python`      |
-|----------|--------------|--------------|--------------|--------------|--------------|--------------|----------------|----------------|---------------|
-| `main`   | `>=0.2,<0.3` | `>=3.0,<3.2` | `>=3.4,<3.6` | `>=3.6,<4.0` | `>=0.1,<0.2` | `>=1.3,<2.2` | `>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.12` |
+| `flamme` | `coola`      | `jinja2`     | `markdown`   | `matplotlib` | `numpy`       | `objectory`  | `pandas`     | `pyarrow`      | `tqdm`         | `python`      |
+|----------|--------------|--------------|--------------|--------------|---------------|--------------|--------------|----------------|----------------|---------------|
+| `main`   | `>=0.2,<0.3` | `>=3.0,<3.2` | `>=3.4,<3.6` | `>=3.6,<4.0` | `>=1.23,<2.0` | `>=0.1,<0.2` | `>=1.3,<2.2` | `>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.13` |
+| `0.0.8`  | `>=0.2,<0.3` | `>=3.0,<3.2` | `>=3.4,<3.6` | `>=3.6,<4.0` | `>=1.23,<2.0` | `>=0.1,<0.2` | `>=1.3,<2.2` | `>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.12` |
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: flamme Version: 0.0.8a1 Summary: A library to
+Metadata-Version: 2.1 Name: flamme Version: 0.0.9 Summary: A library to
 generate custom reports of pandas DataFrames Home-page: https://github.com/
 durandtibo/flamme License: BSD-3-Clause Keywords: pandas,analysis,report
 Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com Requires-Python:
->=3.9,<3.12 Classifier: Development Status :: 3 - Alpha Classifier: Intended
+>=3.9,<3.13 Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Scientific/Engineering Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: all Requires-Dist: coola (>=0.2.0,<0.3) Requires-Dist: jinja2
-(>=3.0,<4.0) Requires-Dist: markdown (>=3.4,<4.0) Requires-Dist: matplotlib
-(>=3.6,<4.0) Requires-Dist: numpy (>=1.23,<2.0) Requires-Dist: objectory
-(>=0.1,<0.2) Requires-Dist: pandas (>=1.3,<3.0) Requires-Dist: pyarrow
-(>=10.0,<15.0) Requires-Dist: tqdm (>=4.65,<5.0) Project-URL: Repository,
-https://github.com/durandtibo/flamme Description-Content-Type: text/markdown #
-flamme
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries Provides-Extra: all
+Requires-Dist: coola (>=0.2.0,<0.3) Requires-Dist: jinja2 (>=3.0,<4.0)
+Requires-Dist: markdown (>=3.4,<4.0) Requires-Dist: matplotlib (>=3.6,<4.0)
+Requires-Dist: numpy (>=1.23,<2.0) Requires-Dist: objectory (>=0.1,<0.2)
+Requires-Dist: pandas (>=1.3,<3.0) Requires-Dist: pyarrow (>=10.0,<15.0)
+Requires-Dist: tqdm (>=4.65,<5.0) Project-URL: Repository, https://github.com/
+durandtibo/flamme Description-Content-Type: text/markdown # flamme
            _[_C_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
      _[_C_o_d_e_c_o_v_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_b_1_2_4_c_0_a_1_a_6_4_e_e_0_4_1_e_1_8_9_/
  _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_b_1_2_4_c_0_a_1_a_6_4_e_e_0_4_1_e_1_8_9_/
                                 _t_e_s_t___c_o_v_e_r_a_g_e_]
   _[_P_Y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_B_S_D_-_3_-_C_l_a_u_s_e_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]
                         _[_D_o_w_n_l_o_a_d_s_]_[_M_o_n_t_h_l_y_ _d_o_w_n_l_o_a_d_s_]
 A library to generate custom reports of pandas DataFrames ## Installation We
@@ -30,12 +30,15 @@
 install flamme ``` To make the package as slim as possible, only the minimal
 packages required to use `flamme` are installed. To include all the
 dependencies, you can use the following command: ```shell pip install flamme
 [all] ``` Please check the [get started page](https://durandtibo.github.io/
 flamme/get_started) to see how to install only some specific dependencies or
 other alternatives to install the library. The following is the corresponding
 `flamme` versions and tested dependencies. | `flamme` | `coola` | `jinja2` |
-`markdown` | `matplotlib` | `objectory` | `pandas` | `pyarrow` | `tqdm` |
-`python` | |----------|--------------|--------------|--------------|-----------
----|--------------|--------------|----------------|----------------|-----------
-----| | `main` | `>=0.2,<0.3` | `>=3.0,<3.2` | `>=3.4,<3.6` | `>=3.6,<4.0` |
-`>=0.1,<0.2` | `>=1.3,<2.2` | `>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.12` |
+`markdown` | `matplotlib` | `numpy` | `objectory` | `pandas` | `pyarrow` |
+`tqdm` | `python` | |----------|--------------|--------------|--------------|--
+------------|---------------|--------------|--------------|----------------|---
+-------------|---------------| | `main` | `>=0.2,<0.3` | `>=3.0,<3.2` |
+`>=3.4,<3.6` | `>=3.6,<4.0` | `>=1.23,<2.0` | `>=0.1,<0.2` | `>=1.3,<2.2` |
+`>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.13` | | `0.0.8` | `>=0.2,<0.3` |
+`>=3.0,<3.2` | `>=3.4,<3.6` | `>=3.6,<4.0` | `>=1.23,<2.0` | `>=0.1,<0.2` |
+`>=1.3,<2.2` | `>=10.0,<15.0` | `>=4.65,<4.67` | `>=3.9,<3.12` |
```

