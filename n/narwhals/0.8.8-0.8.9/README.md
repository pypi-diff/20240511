# Comparing `tmp/narwhals-0.8.8.tar.gz` & `tmp/narwhals-0.8.9.tar.gz`

## Comparing `narwhals-0.8.8.tar` & `narwhals-0.8.9.tar`

### file list

```diff
@@ -1,122 +1,124 @@
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.8/mkdocs.yml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.8/requirements-dev.txt
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.8/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.8/.github/workflows/extremes.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.8/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.8/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.8/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/extending.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/generate_members.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/installation.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/quick_start.md
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/related.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/requirements-docs.txt
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/roadmap.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/why.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/dataframe.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/dependencies.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/dtypes.md
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/expressions.md
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/expressions_dt.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/expressions_str.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/index.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/lazyframe.md
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/narwhals.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/series.md
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/series_dt.md
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/series_str.md
--rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/assets/image.png
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/basics/column.md
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/basics/complete_example.md
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/basics/dataframe.md
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/other/pandas_index.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/__init__.py
--rw-r--r--   0        0        0    93496 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/dataframe.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/dependencies.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/dtypes.py
--rw-r--r--   0        0        0    38122 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/expression.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/functions.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/group_by.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/py.typed
--rw-r--r--   0        0        0    15333 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/series.py
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/translate.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/typing.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/__init__.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/dataframe.py
--rw-r--r--   0        0        0    10392 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/expr.py
--rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/group_by.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/namespace.py
--rw-r--r--   0        0        0    16348 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/series.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/typing.py
--rw-r--r--   0        0        0    14015 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/conftest.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/group_by_test.py
--rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_common.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_dt.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_group_by.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_invalid.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_pandas.py
--rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_series.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_str.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/tpch_q1_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/utils.py
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/customer.parquet
--rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/lineitem.parquet
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/nation.parquet
--rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/orders.parquet
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/part.parquet
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/partsupp.parquet
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/region.parquet
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/supplier.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/cum_sum_test.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/diff_test.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/fill_null_test.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/over_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/test_over.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/str/__init__.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/str/head_test.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/str/to_datetime_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/frame/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/frame/pipe_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/hypothesis/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/hypothesis/test_basic_arithmetic.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/hypothesis/test_concat.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/hypothesis/test_join.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/q1.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/q2.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/q3.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/q4.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/q5.py
--rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/gpu/execute.ipynb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/gpu/kernel-metadata.json
--rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q1/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q1/kernel-metadata.json
--rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q2/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q2/kernel-metadata.json
--rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q3/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q3/kernel-metadata.json
--rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q4/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q4/kernel-metadata.json
--rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q5/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q5/kernel-metadata.json
--rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q6/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q6/kernel-metadata.json
--rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q7/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q7/kernel-metadata.json
--rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q8/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q8/kernel-metadata.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/utils/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.8/utils/bump_version.py
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.8/utils/check_api_reference.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.8/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.8/LICENSE.md
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.8/README.md
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.9/mkdocs.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.9/requirements-dev.txt
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.9/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.9/.github/workflows/extremes.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.9/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.9/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.9/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/extending.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/generate_members.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/installation.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/quick_start.md
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/related.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/requirements-docs.txt
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/roadmap.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/why.md
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/dataframe.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/dependencies.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/dtypes.md
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/expressions.md
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/expressions_dt.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/expressions_str.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/index.md
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/lazyframe.md
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/narwhals.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/series.md
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/series_dt.md
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/series_str.md
+-rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/assets/image.png
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/basics/column.md
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/basics/dataframe.md
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/other/pandas_index.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/__init__.py
+-rw-r--r--   0        0        0    96138 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/dataframe.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/dependencies.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/dtypes.py
+-rw-r--r--   0        0        0    39888 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/expression.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/functions.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/group_by.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/py.typed
+-rw-r--r--   0        0        0    16770 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/series.py
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/translate.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/typing.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/__init__.py
+-rw-r--r--   0        0        0     7941 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/dataframe.py
+-rw-r--r--   0        0        0    10488 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/expr.py
+-rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/group_by.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/namespace.py
+-rw-r--r--   0        0        0    16520 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/series.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/typing.py
+-rw-r--r--   0        0        0    14015 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/conftest.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/group_by_test.py
+-rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_common.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_dt.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_group_by.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_invalid.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_pandas.py
+-rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_series.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_str.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/tpch_q1_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/utils.py
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/customer.parquet
+-rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/lineitem.parquet
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/nation.parquet
+-rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/orders.parquet
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/part.parquet
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/partsupp.parquet
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/region.parquet
+-rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/supplier.parquet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/cum_sum_test.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/diff_test.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/fill_null_test.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/over_test.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/shift_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/test_over.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/str/__init__.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/str/head_test.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/str/to_datetime_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/frame/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/frame/drop_nulls_test.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/frame/pipe_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/hypothesis/test_basic_arithmetic.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/hypothesis/test_concat.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/hypothesis/test_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/q1.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/q2.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/q3.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/q4.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/q5.py
+-rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/gpu/execute.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/gpu/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q1/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q1/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q2/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q2/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q3/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q3/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q4/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q4/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q5/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q5/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q6/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q6/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q7/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q7/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q8/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q8/kernel-metadata.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/utils/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.9/utils/bump_version.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.9/utils/check_api_reference.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.9/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.9/LICENSE.md
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.9/README.md
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.9/PKG-INFO
```

### Comparing `narwhals-0.8.8/.pre-commit-config.yaml` & `narwhals-0.8.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/CONTRIBUTING.md` & `narwhals-0.8.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/mkdocs.yml` & `narwhals-0.8.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/.github/CODE_OF_CONDUCT.md` & `narwhals-0.8.9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/.github/workflows/extremes.yml` & `narwhals-0.8.9/.github/workflows/extremes.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/.github/workflows/mkdocs.yml` & `narwhals-0.8.9/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/.github/workflows/publish_to_pypi.yml` & `narwhals-0.8.9/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/.github/workflows/pytest.yml` & `narwhals-0.8.9/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/extending.md` & `narwhals-0.8.9/docs/extending.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/generate_members.py` & `narwhals-0.8.9/docs/generate_members.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/index.md` & `narwhals-0.8.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/quick_start.md` & `narwhals-0.8.9/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/related.md` & `narwhals-0.8.9/docs/related.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/roadmap.md` & `narwhals-0.8.9/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/why.md` & `narwhals-0.8.9/docs/why.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/api-reference/index.md` & `narwhals-0.8.9/docs/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/api-reference/series.md` & `narwhals-0.8.9/docs/api-reference/series.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         - max
         - mean
         - min
         - name
         - n_unique
         - sample
         - shape
+        - shift
         - sort
         - std
         - sum
         - to_numpy
         - to_pandas
         - unique
       show_source: false
```

### Comparing `narwhals-0.8.8/docs/assets/image.png` & `narwhals-0.8.9/docs/assets/image.png`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/basics/column.md` & `narwhals-0.8.9/docs/basics/column.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/basics/complete_example.md` & `narwhals-0.8.9/docs/basics/complete_example.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/basics/dataframe.md` & `narwhals-0.8.9/docs/basics/dataframe.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/docs/other/pandas_index.md` & `narwhals-0.8.9/docs/other/pandas_index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/narwhals/__init__.py` & `narwhals-0.8.9/narwhals/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from narwhals.expression import sum
 from narwhals.expression import sum_horizontal
 from narwhals.functions import concat
 from narwhals.series import Series
 from narwhals.translate import from_native
 from narwhals.translate import to_native
 
-__version__ = "0.8.8"
+__version__ = "0.8.9"
 
 __all__ = [
     "concat",
     "to_native",
     "from_native",
     "all",
     "col",
```

### Comparing `narwhals-0.8.8/narwhals/dataframe.py` & `narwhals-0.8.9/narwhals/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,19 @@
             k: to_narwhals_dtype(v, is_polars=self._is_polars)
             for k, v in self._dataframe.schema.items()
         }
 
     def pipe(self, function: Callable[[Any], Self], *args: Any, **kwargs: Any) -> Self:
         return function(self, *args, **kwargs)
 
+    def drop_nulls(self) -> Self:
+        return self._from_dataframe(
+            self._dataframe.drop_nulls(),
+        )
+
     @property
     def columns(self) -> list[str]:
         return self._dataframe.columns  # type: ignore[no-any-return]
 
     def lazy(self) -> LazyFrame:
         return LazyFrame(
             self._dataframe.lazy(),
@@ -473,14 +478,54 @@
             │ 1   │
             │ 2   │
             │ 3   │
             └─────┘
         """
         return super().pipe(function, *args, **kwargs)
 
+    def drop_nulls(self) -> Self:
+        """
+        Drop null values.
+
+        Notes:
+            pandas and Polars handle null values differently. Polars distinguishes
+            between NaN and Null, whereas pandas doesn't.
+
+        Examples:
+            >>> import polars as pl
+            >>> import pandas as pd
+            >>> import narwhals as nw
+            >>> data = {'a': [1., 2., None], 'ba': [1, None, 2.]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.drop_nulls()
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars:
+
+            >>> func(df_pd)
+                 a   ba
+            0  1.0  1.0
+            >>> func(df_pl)
+            shape: (1, 2)
+            ┌─────┬─────┐
+            │ a   ┆ ba  │
+            │ --- ┆ --- │
+            │ f64 ┆ f64 │
+            ╞═════╪═════╡
+            │ 1.0 ┆ 1.0 │
+            └─────┴─────┘
+        """
+        return super().drop_nulls()
+
     @property
     def schema(self) -> dict[str, DType]:
         r"""
         Get a dict[column name, DataType].
 
         Examples:
             >>> import polars as pl
@@ -1422,14 +1467,54 @@
             │ 1   │
             │ 2   │
             │ 3   │
             └─────┘
         """
         return super().pipe(function, *args, **kwargs)
 
+    def drop_nulls(self) -> Self:
+        """
+        Drop null values.
+
+        Notes:
+            pandas and Polars handle null values differently. Polars distinguishes
+            between NaN and Null, whereas pandas doesn't.
+
+        Examples:
+            >>> import polars as pl
+            >>> import pandas as pd
+            >>> import narwhals as nw
+            >>> data = {'a': [1., 2., None], 'ba': [1, None, 2.]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.LazyFrame(data)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.drop_nulls()
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars:
+
+            >>> func(df_pd)
+                 a   ba
+            0  1.0  1.0
+            >>> func(df_pl).collect()
+            shape: (1, 2)
+            ┌─────┬─────┐
+            │ a   ┆ ba  │
+            │ --- ┆ --- │
+            │ f64 ┆ f64 │
+            ╞═════╪═════╡
+            │ 1.0 ┆ 1.0 │
+            └─────┴─────┘
+        """
+        return super().drop_nulls()
+
     @property
     def schema(self) -> dict[str, DType]:
         r"""
         Get a dict[column name, DType].
 
         Examples:
             >>> import polars as pl
```

### Comparing `narwhals-0.8.8/narwhals/dependencies.py` & `narwhals-0.8.9/narwhals/dependencies.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/narwhals/dtypes.py` & `narwhals-0.8.9/narwhals/dtypes.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/narwhals/expression.py` & `narwhals-0.8.9/narwhals/expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,14 +620,68 @@
             │ 2      │
             │ 2      │
             │ 0      │
             └────────┘
         """
         return self.__class__(lambda plx: self._call(plx).diff())
 
+    def shift(self, n: int) -> Expr:
+        """
+        Shift values by `n` positions.
+
+        Notes:
+            pandas may change the dtype here, for example when introducing missing
+            values in an integer column. To ensure, that the dtype doesn't change,
+            you may want to use `fill_null` and `cast`. For example, to shift
+            and fill missing values with `0` in a Int64 column, you could
+            do:
+
+            ```python
+            nw.col('a').shift(1).fill_null(0).cast(nw.Int64)
+            ```
+
+        Examples:
+            >>> import polars as pl
+            >>> import pandas as pd
+            >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame({'a': [1, 1, 3, 5, 5]})
+            >>> df_pl = pl.DataFrame({'a': [1, 1, 3, 5, 5]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...    df = nw.from_native(df_any)
+            ...    df = df.select(a_shift=nw.col('a').shift(n=1))
+            ...    return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+               a_shift
+            0      NaN
+            1      1.0
+            2      1.0
+            3      3.0
+            4      5.0
+            >>> func(df_pl)
+            shape: (5, 1)
+            ┌─────────┐
+            │ a_shift │
+            │ ---     │
+            │ i64     │
+            ╞═════════╡
+            │ null    │
+            │ 1       │
+            │ 1       │
+            │ 3       │
+            │ 5       │
+            └─────────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).shift(n))
+
     def sort(self, *, descending: bool = False) -> Expr:
         return self.__class__(lambda plx: self._call(plx).sort(descending=descending))
 
     # --- transform ---
     def is_between(
         self, lower_bound: Any, upper_bound: Any, closed: str = "both"
     ) -> Expr:
```

### Comparing `narwhals-0.8.8/narwhals/functions.py` & `narwhals-0.8.9/narwhals/functions.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/narwhals/group_by.py` & `narwhals-0.8.9/narwhals/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/narwhals/series.py` & `narwhals-0.8.9/narwhals/series.py`

 * *Files 5% similar despite different names*

```diff
@@ -334,14 +334,62 @@
                null
                2
                -1
             ]
         """
         return self._from_series(self._series.diff())
 
+    def shift(self, n: int) -> Self:
+        """
+        Shift values by `n` positions.
+
+        Notes:
+            pandas may change the dtype here, for example when introducing missing
+            values in an integer column. To ensure, that the dtype doesn't change,
+            you may want to use `fill_null` and `cast`. For example, to shift
+            and fill missing values with `0` in a Int64 column, you could
+            do:
+
+            ```python
+            s.shift(1).fill_null(0).cast(nw.Int64)
+            ```
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> import narwhals as nw
+            >>> s = [2, 4, 3]
+            >>> s_pd = pd.Series(s)
+            >>> s_pl = pl.Series(s)
+
+            We define a dataframe-agnostic function:
+
+            >>> def func(s_any):
+            ...     s = nw.from_native(s_any, series_only=True)
+            ...     s = s.shift(1)
+            ...     return nw.to_native(s)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(s_pd)
+            0    NaN
+            1    2.0
+            2    4.0
+            dtype: float64
+            >>> func(s_pl)  # doctest: +NORMALIZE_WHITESPACE
+            shape: (3,)
+            Series: '' [i64]
+            [
+               null
+               2
+               4
+            ]
+        """
+        return self._from_series(self._series.shift(n))
+
     def sample(
         self,
         n: int | None = None,
         fraction: float | None = None,
         *,
         with_replacement: bool = False,
     ) -> Self:
```

### Comparing `narwhals-0.8.8/narwhals/translate.py` & `narwhals-0.8.9/narwhals/translate.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/narwhals/typing.py` & `narwhals-0.8.9/narwhals/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/narwhals/utils.py` & `narwhals-0.8.9/narwhals/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/narwhals/_pandas_like/dataframe.py` & `narwhals-0.8.9/narwhals/_pandas_like/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,17 @@
         new_series = validate_indices(new_series)
         df = horizontal_concat(
             new_series,
             implementation=self._implementation,
         )
         return self._from_dataframe(df)
 
+    def drop_nulls(self) -> Self:
+        return self._from_dataframe(self._dataframe.dropna(axis=0))
+
     def filter(
         self,
         *predicates: IntoPandasExpr | Iterable[IntoPandasExpr],
     ) -> Self:
         from narwhals._pandas_like.namespace import PandasNamespace
 
         plx = PandasNamespace(self._implementation)
```

### Comparing `narwhals-0.8.8/narwhals/_pandas_like/expr.py` & `narwhals-0.8.9/narwhals/_pandas_like/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,14 +201,17 @@
 
     def unique(self) -> Self:
         return register_expression_call(self, "unique")
 
     def diff(self) -> Self:
         return register_expression_call(self, "diff")
 
+    def shift(self, n: int) -> Self:
+        return register_expression_call(self, "shift", n)
+
     def sample(
         self,
         n: int | None = None,
         fraction: float | None = None,
         *,
         with_replacement: bool = False,
     ) -> Self:
```

### Comparing `narwhals-0.8.8/narwhals/_pandas_like/group_by.py` & `narwhals-0.8.9/narwhals/_pandas_like/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/narwhals/_pandas_like/namespace.py` & `narwhals-0.8.9/narwhals/_pandas_like/namespace.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/narwhals/_pandas_like/series.py` & `narwhals-0.8.9/narwhals/_pandas_like/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,14 +371,19 @@
         )
 
     def diff(self) -> PandasSeries:
         return self._from_series(
             self._series.__class__(self._series.diff(), name=self._series.name)
         )
 
+    def shift(self, n: int) -> PandasSeries:
+        return self._from_series(
+            self._series.__class__(self._series.shift(n), name=self._series.name)
+        )
+
     def sort(
         self,
         *,
         descending: bool | Sequence[bool] = False,
     ) -> PandasSeries:
         ser = self._series
         return self._from_series(
```

### Comparing `narwhals-0.8.8/narwhals/_pandas_like/typing.py` & `narwhals-0.8.9/narwhals/_pandas_like/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/narwhals/_pandas_like/utils.py` & `narwhals-0.8.9/narwhals/_pandas_like/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/conftest.py` & `narwhals-0.8.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/group_by_test.py` & `narwhals-0.8.9/tests/group_by_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/test_common.py` & `narwhals-0.8.9/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/test_dt.py` & `narwhals-0.8.9/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/test_group_by.py` & `narwhals-0.8.9/tests/test_group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/test_series.py` & `narwhals-0.8.9/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/test_str.py` & `narwhals-0.8.9/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/tpch_q1_test.py` & `narwhals-0.8.9/tests/tpch_q1_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/utils.py` & `narwhals-0.8.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/data/customer.parquet` & `narwhals-0.8.9/tests/data/customer.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/data/lineitem.parquet` & `narwhals-0.8.9/tests/data/lineitem.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/data/nation.parquet` & `narwhals-0.8.9/tests/data/nation.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/data/orders.parquet` & `narwhals-0.8.9/tests/data/orders.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/data/part.parquet` & `narwhals-0.8.9/tests/data/part.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/data/partsupp.parquet` & `narwhals-0.8.9/tests/data/partsupp.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/data/region.parquet` & `narwhals-0.8.9/tests/data/region.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/data/supplier.parquet` & `narwhals-0.8.9/tests/data/supplier.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/expr/cum_sum_test.py` & `narwhals-0.8.9/tests/expr/cum_sum_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/expr/diff_test.py` & `narwhals-0.8.9/tests/expr/diff_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/expr/fill_null_test.py` & `narwhals-0.8.9/tests/expr/fill_null_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/expr/over_test.py` & `narwhals-0.8.9/tests/expr/over_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/expr/str/head_test.py` & `narwhals-0.8.9/tests/expr/str/head_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/expr/str/to_datetime_test.py` & `narwhals-0.8.9/tests/expr/str/to_datetime_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/frame/pipe_test.py` & `narwhals-0.8.9/tests/frame/pipe_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/hypothesis/test_basic_arithmetic.py` & `narwhals-0.8.9/tests/hypothesis/test_basic_arithmetic.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/hypothesis/test_concat.py` & `narwhals-0.8.9/tests/hypothesis/test_concat.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tests/hypothesis/test_join.py` & `narwhals-0.8.9/tests/hypothesis/test_join.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/q1.py` & `narwhals-0.8.9/tpch/q1.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/q2.py` & `narwhals-0.8.9/tpch/q2.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/q3.py` & `narwhals-0.8.9/tpch/q3.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/q4.py` & `narwhals-0.8.9/tpch/q4.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/q5.py` & `narwhals-0.8.9/tpch/q5.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/notebooks/gpu/execute.ipynb` & `narwhals-0.8.9/tpch/notebooks/gpu/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/notebooks/q1/execute.ipynb` & `narwhals-0.8.9/tpch/notebooks/q1/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/notebooks/q2/execute.ipynb` & `narwhals-0.8.9/tpch/notebooks/q2/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/notebooks/q3/execute.ipynb` & `narwhals-0.8.9/tpch/notebooks/q3/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/notebooks/q4/execute.ipynb` & `narwhals-0.8.9/tpch/notebooks/q4/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/notebooks/q5/execute.ipynb` & `narwhals-0.8.9/tpch/notebooks/q5/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/notebooks/q6/execute.ipynb` & `narwhals-0.8.9/tpch/notebooks/q6/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/notebooks/q7/execute.ipynb` & `narwhals-0.8.9/tpch/notebooks/q7/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/tpch/notebooks/q8/execute.ipynb` & `narwhals-0.8.9/tpch/notebooks/q8/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/utils/bump_version.py` & `narwhals-0.8.9/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/utils/check_api_reference.py` & `narwhals-0.8.9/utils/check_api_reference.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/LICENSE.md` & `narwhals-0.8.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/README.md` & `narwhals-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.8/pyproject.toml` & `narwhals-0.8.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "narwhals"
-version = "0.8.8"
+version = "0.8.9"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `narwhals-0.8.8/PKG-INFO` & `narwhals-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: narwhals
-Version: 0.8.8
+Version: 0.8.9
 Summary: Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin
 Project-URL: Homepage, https://github.com/MarcoGorelli/narwhals
 Project-URL: Bug Tracker, https://github.com/MarcoGorelli/narwhals
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

