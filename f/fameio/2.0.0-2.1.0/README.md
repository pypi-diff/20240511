# Comparing `tmp/fameio-2.0.0.tar.gz` & `tmp/fameio-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fameio-2.0.0.tar", max compression
+gzip compressed data, was "fameio-2.1.0.tar", max compression
```

## Comparing `fameio-2.0.0.tar` & `fameio-2.1.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0     9874 2024-04-03 16:31:37.396336 fameio-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    10391 2023-04-14 05:55:34.824015 fameio-2.0.0/LICENSE.txt
-drwxr-xr-x   0        0        0        0 2023-05-03 15:01:38.291067 fameio-2.0.0/LICENSES/
--rw-r--r--   0        0        0    10391 2023-04-14 05:55:34.824015 fameio-2.0.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    19051 2023-05-03 15:01:38.291067 fameio-2.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0        0        0     7169 2023-04-14 05:55:34.825013 fameio-2.0.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0     1850 2024-04-03 16:31:37.396336 fameio-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    30287 2024-03-07 15:03:46.249549 fameio-2.0.0/README.md
--rw-r--r--   0        0        0      109 2023-04-14 05:55:34.826011 fameio-2.0.0/src/fameio/__init__.py
--rw-r--r--   0        0        0      741 2024-03-07 15:03:46.250611 fameio-2.0.0/src/fameio/scripts/__init__.py
--rw-r--r--   0        0        0      107 2024-03-07 15:03:46.251544 fameio-2.0.0/src/fameio/scripts/__init__.py.license
--rw-r--r--   0        0        0     3635 2024-04-03 06:43:28.347153 fameio-2.0.0/src/fameio/scripts/convert_results.py
--rw-r--r--   0        0        0      107 2024-02-26 16:17:50.230821 fameio-2.0.0/src/fameio/scripts/convert_results.py.license
--rw-r--r--   0        0        0     1349 2024-04-03 06:43:28.347153 fameio-2.0.0/src/fameio/scripts/make_config.py
--rw-r--r--   0        0        0      107 2024-03-07 15:03:46.252566 fameio-2.0.0/src/fameio/scripts/make_config.py.license
--rw-r--r--   0        0        0      278 2023-04-14 05:55:34.828008 fameio-2.0.0/src/fameio/source/__init__.py
--rw-r--r--   0        0        0      112 2024-03-07 15:03:46.252566 fameio-2.0.0/src/fameio/source/cli/__init__.py
--rw-r--r--   0        0        0     3072 2024-03-07 15:03:46.253544 fameio-2.0.0/src/fameio/source/cli/convert_results.py
--rw-r--r--   0        0        0     2369 2024-03-07 15:03:46.253544 fameio-2.0.0/src/fameio/source/cli/make_config.py
--rw-r--r--   0        0        0     1413 2024-03-07 15:03:46.253544 fameio-2.0.0/src/fameio/source/cli/options.py
--rw-r--r--   0        0        0     9366 2024-03-07 15:03:46.254559 fameio-2.0.0/src/fameio/source/cli/parser.py
--rw-r--r--   0        0        0     7433 2024-01-17 10:31:27.021124 fameio-2.0.0/src/fameio/source/loader.py
--rw-r--r--   0        0        0     2806 2024-01-17 10:31:27.021124 fameio-2.0.0/src/fameio/source/logs.py
--rw-r--r--   0        0        0     1321 2024-01-17 10:31:27.022038 fameio-2.0.0/src/fameio/source/path_resolver.py
--rw-r--r--   0        0        0      109 2023-04-14 05:55:34.829005 fameio-2.0.0/src/fameio/source/results/__init__.py
--rw-r--r--   0        0        0     4321 2024-01-17 10:31:27.022038 fameio-2.0.0/src/fameio/source/results/agent_type.py
--rw-r--r--   0        0        0     3721 2024-03-07 15:03:46.255599 fameio-2.0.0/src/fameio/source/results/conversion.py
--rw-r--r--   0        0        0     4868 2024-02-26 16:17:50.231821 fameio-2.0.0/src/fameio/source/results/csv_writer.py
--rw-r--r--   0        0        0     6264 2024-03-07 15:03:46.255599 fameio-2.0.0/src/fameio/source/results/data_transformer.py
--rw-r--r--   0        0        0     6928 2024-03-07 15:03:46.256605 fameio-2.0.0/src/fameio/source/results/input_dao.py
--rw-r--r--   0        0        0     3960 2024-01-17 10:31:27.024035 fameio-2.0.0/src/fameio/source/results/output_dao.py
--rw-r--r--   0        0        0     5078 2024-04-03 06:43:28.349147 fameio-2.0.0/src/fameio/source/results/reader.py
--rw-r--r--   0        0        0      843 2024-04-03 16:25:46.569642 fameio-2.0.0/src/fameio/source/results/yaml_writer.py
--rw-r--r--   0        0        0      372 2023-04-14 05:55:34.830003 fameio-2.0.0/src/fameio/source/scenario/__init__.py
--rw-r--r--   0        0        0     4713 2024-02-26 16:17:50.232821 fameio-2.0.0/src/fameio/source/scenario/agent.py
--rw-r--r--   0        0        0     4834 2024-02-26 16:17:50.233821 fameio-2.0.0/src/fameio/source/scenario/attribute.py
--rw-r--r--   0        0        0     9448 2024-02-26 16:17:50.233821 fameio-2.0.0/src/fameio/source/scenario/contract.py
--rw-r--r--   0        0        0     1560 2023-11-28 14:30:17.776761 fameio-2.0.0/src/fameio/source/scenario/exception.py
--rw-r--r--   0        0        0     1376 2024-01-26 10:13:38.847488 fameio-2.0.0/src/fameio/source/scenario/fameiofactory.py
--rw-r--r--   0        0        0     4545 2024-02-14 10:56:32.725583 fameio-2.0.0/src/fameio/source/scenario/generalproperties.py
--rw-r--r--   0        0        0     3727 2024-04-03 06:43:28.349147 fameio-2.0.0/src/fameio/source/scenario/scenario.py
--rw-r--r--   0        0        0      270 2023-04-14 05:55:34.831001 fameio-2.0.0/src/fameio/source/schema/__init__.py
--rw-r--r--   0        0        0     5198 2024-01-17 10:31:27.026034 fameio-2.0.0/src/fameio/source/schema/agenttype.py
--rw-r--r--   0        0        0     8308 2024-01-17 10:31:27.027034 fameio-2.0.0/src/fameio/source/schema/attribute.py
--rw-r--r--   0        0        0      224 2023-04-14 05:55:34.832000 fameio-2.0.0/src/fameio/source/schema/exception.py
--rw-r--r--   0        0        0     2240 2024-01-17 10:31:27.027034 fameio-2.0.0/src/fameio/source/schema/schema.py
--rw-r--r--   0        0        0     8120 2024-03-07 15:03:46.257542 fameio-2.0.0/src/fameio/source/series.py
--rw-r--r--   0        0        0     6984 2024-01-17 10:31:27.028034 fameio-2.0.0/src/fameio/source/time.py
--rw-r--r--   0        0        0     1052 2024-03-07 15:03:46.257542 fameio-2.0.0/src/fameio/source/tools.py
--rw-r--r--   0        0        0    15734 2024-04-03 06:43:28.350143 fameio-2.0.0/src/fameio/source/validator.py
--rw-r--r--   0        0        0    11353 2024-04-03 06:43:28.351141 fameio-2.0.0/src/fameio/source/writer.py
--rw-r--r--   0        0        0    30769 1970-01-01 00:00:00.000000 fameio-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10680 2024-05-11 12:41:36.554060 fameio-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10391 2024-05-06 12:30:08.115006 fameio-2.1.0/LICENSE.txt
+drwxr-xr-x   0        0        0        0 2024-05-06 12:30:08.115006 fameio-2.1.0/LICENSES/
+-rw-r--r--   0        0        0    10391 2024-05-06 12:30:08.115006 fameio-2.1.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    19051 2024-05-06 12:30:08.115006 fameio-2.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0     7169 2024-05-06 12:30:08.115006 fameio-2.1.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1850 2024-05-11 12:41:36.554060 fameio-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    30377 2024-05-11 12:41:36.554060 fameio-2.1.0/README.md
+-rw-r--r--   0        0        0      109 2024-05-06 12:30:08.121006 fameio-2.1.0/src/fameio/__init__.py
+-rw-r--r--   0        0        0      741 2024-05-06 12:30:08.121006 fameio-2.1.0/src/fameio/scripts/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-06 12:30:08.121006 fameio-2.1.0/src/fameio/scripts/__init__.py.license
+-rw-r--r--   0        0        0     3615 2024-05-11 12:41:36.555059 fameio-2.1.0/src/fameio/scripts/convert_results.py
+-rw-r--r--   0        0        0      107 2024-05-06 12:30:08.122008 fameio-2.1.0/src/fameio/scripts/convert_results.py.license
+-rw-r--r--   0        0        0     1347 2024-05-11 12:41:36.555059 fameio-2.1.0/src/fameio/scripts/make_config.py
+-rw-r--r--   0        0        0      107 2024-05-06 12:30:08.122008 fameio-2.1.0/src/fameio/scripts/make_config.py.license
+-rw-r--r--   0        0        0      278 2024-05-06 12:30:08.123528 fameio-2.1.0/src/fameio/source/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-06 12:30:08.123528 fameio-2.1.0/src/fameio/source/cli/__init__.py
+-rw-r--r--   0        0        0     3412 2024-05-11 12:41:36.556061 fameio-2.1.0/src/fameio/source/cli/convert_results.py
+-rw-r--r--   0        0        0     2384 2024-05-11 12:41:36.556061 fameio-2.1.0/src/fameio/source/cli/make_config.py
+-rw-r--r--   0        0        0     1393 2024-05-11 12:35:35.384517 fameio-2.1.0/src/fameio/source/cli/options.py
+-rw-r--r--   0        0        0     9423 2024-05-11 12:41:36.556061 fameio-2.1.0/src/fameio/source/cli/parser.py
+-rw-r--r--   0        0        0     7403 2024-05-11 12:41:36.557056 fameio-2.1.0/src/fameio/source/loader.py
+-rw-r--r--   0        0        0     3684 2024-05-11 12:41:36.557056 fameio-2.1.0/src/fameio/source/logs.py
+-rw-r--r--   0        0        0     1321 2024-05-06 12:30:08.125518 fameio-2.1.0/src/fameio/source/path_resolver.py
+-rw-r--r--   0        0        0      109 2024-05-06 12:30:08.125518 fameio-2.1.0/src/fameio/source/results/__init__.py
+-rw-r--r--   0        0        0     4321 2024-05-06 12:30:08.126499 fameio-2.1.0/src/fameio/source/results/agent_type.py
+-rw-r--r--   0        0        0     3709 2024-05-11 12:41:36.558058 fameio-2.1.0/src/fameio/source/results/conversion.py
+-rw-r--r--   0        0        0     4856 2024-05-11 12:41:36.558058 fameio-2.1.0/src/fameio/source/results/csv_writer.py
+-rw-r--r--   0        0        0     5490 2024-05-11 12:35:35.385517 fameio-2.1.0/src/fameio/source/results/data_transformer.py
+-rw-r--r--   0        0        0     6919 2024-05-11 12:41:36.559057 fameio-2.1.0/src/fameio/source/results/input_dao.py
+-rw-r--r--   0        0        0     3960 2024-05-06 12:30:08.127497 fameio-2.1.0/src/fameio/source/results/output_dao.py
+-rw-r--r--   0        0        0     5054 2024-05-11 12:41:36.560056 fameio-2.1.0/src/fameio/source/results/reader.py
+-rw-r--r--   0        0        0      837 2024-05-11 12:41:36.560056 fameio-2.1.0/src/fameio/source/results/yaml_writer.py
+-rw-r--r--   0        0        0      372 2024-05-06 12:30:08.127497 fameio-2.1.0/src/fameio/source/scenario/__init__.py
+-rw-r--r--   0        0        0     4713 2024-05-06 12:30:08.127497 fameio-2.1.0/src/fameio/source/scenario/agent.py
+-rw-r--r--   0        0        0     4834 2024-05-06 12:30:08.128497 fameio-2.1.0/src/fameio/source/scenario/attribute.py
+-rw-r--r--   0        0        0     9442 2024-05-11 12:41:36.560056 fameio-2.1.0/src/fameio/source/scenario/contract.py
+-rw-r--r--   0        0        0     1554 2024-05-11 12:41:36.561056 fameio-2.1.0/src/fameio/source/scenario/exception.py
+-rw-r--r--   0        0        0     1376 2024-05-06 12:30:08.128497 fameio-2.1.0/src/fameio/source/scenario/fameiofactory.py
+-rw-r--r--   0        0        0     4539 2024-05-11 12:41:36.561056 fameio-2.1.0/src/fameio/source/scenario/generalproperties.py
+-rw-r--r--   0        0        0     3727 2024-05-06 12:30:08.129515 fameio-2.1.0/src/fameio/source/scenario/scenario.py
+-rw-r--r--   0        0        0      270 2024-05-06 12:30:08.129515 fameio-2.1.0/src/fameio/source/schema/__init__.py
+-rw-r--r--   0        0        0     5183 2024-05-11 12:41:36.562056 fameio-2.1.0/src/fameio/source/schema/agenttype.py
+-rw-r--r--   0        0        0     8296 2024-05-11 12:41:36.562056 fameio-2.1.0/src/fameio/source/schema/attribute.py
+-rw-r--r--   0        0        0      224 2024-05-06 12:30:08.130497 fameio-2.1.0/src/fameio/source/schema/exception.py
+-rw-r--r--   0        0        0     2656 2024-05-11 12:41:36.563056 fameio-2.1.0/src/fameio/source/schema/java_packages.py
+-rw-r--r--   0        0        0     2975 2024-05-11 12:41:36.563056 fameio-2.1.0/src/fameio/source/schema/schema.py
+-rw-r--r--   0        0        0     8232 2024-05-11 12:41:36.564056 fameio-2.1.0/src/fameio/source/series.py
+-rw-r--r--   0        0        0     6984 2024-05-06 12:30:08.132517 fameio-2.1.0/src/fameio/source/time.py
+-rw-r--r--   0        0        0     1052 2024-05-06 12:30:08.132517 fameio-2.1.0/src/fameio/source/tools.py
+-rw-r--r--   0        0        0    15719 2024-05-11 12:41:36.564056 fameio-2.1.0/src/fameio/source/validator.py
+-rw-r--r--   0        0        0    11921 2024-05-11 12:41:36.564056 fameio-2.1.0/src/fameio/source/writer.py
+-rw-r--r--   0        0        0    30847 1970-01-01 00:00:00.000000 fameio-2.1.0/PKG-INFO
```

### Comparing `fameio-2.0.0/CHANGELOG.md` & `fameio-2.1.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,34 @@
-<!-- SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+<!-- SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 
 SPDX-License-Identifier: CC0-1.0 -->
 
 # Changelog
 
-## [2.0.0 - 2024-04-03](https://gitlab.com/fame-framework/fame-io/-/tags/v2.0.0)
+## [2.1.0](https://gitlab.com/fame-framework/fame-io/-/tags/v2.1.0) - 2024-05-11
+### Changed
+- Changed format of auto-created timeseries from constant values #196 (@dlr-cjs)
+- Changed default log level to "WARNING" #191 (@dlr_fn @dlr-cjs)
+- Adapted link-formatting in Changelog !155 (@dlr-cjs)
+
+### Added
+- Read java package names from Schema and write to input.pb #198 (@dlr-cjs)
+
+### Fixed
+- Fix docstrings in CLI `handle_args()` #190 (@dlr-cjs @dlr_fn)
+- Fix potential duplicates in logging #191 (@dlr_fn @dlr-cjs)
+
+## [2.0.1](https://gitlab.com/fame-framework/fame-io/-/tags/v2.0.1) - 2024-04-05
+### Fix
+- Fix potential missing columns when memory-saving-mode `-m` is enabled #194 (@dlr_fn @dlr-cjs) 
+
+### Remove
+- Remove convert results option `-cc MERGE` #194 (@dlr_fn @dlr-cjs)
+
+## [2.0.0](https://gitlab.com/fame-framework/fame-io/-/tags/v2.0.0) - 2024-04-03
 ### Changed
 - **Breaking**: Removed support for `python==3.8` #163 (@dlr-cjs @dlr_fn)
 - **Breaking**: Signature of `run` functions in `make_config.py` and `convert_results.py` changed: the input file is now read from the configuration dictionary #163 (@dlr-cjs @dlr_fn)
 - **Breaking**: Created protobuf files now have a header section -> minimum required FAME-Core version is now 1.6.0 #183 (@dlr-cjs @dlr_fn)
 - Raise error for NaN float values in scenario and time series #165 (@dlr-cjs @dlr_fn)
 - Enhance Schema to include metadata and output fields #156 (@dlr-cjs @litotes18 @dlr_fn)
 - Enhance Contracts to include metadata #158 (@dlr-cjs @litotes18 @dlr_fn)
@@ -41,98 +61,98 @@
 - Remove deprecated protobuf test !127 (@dlr-cjs @dlr_fn)
 
 ### Fixed
 - Fix deprecated arguments in pandas groupby !129 (@maurerle)
 - Fix breaking tests in Pytest 8.0 #176 (@dlr-cjs)
 - Fix PyTests for Python 3.12 #182 (@dlr_fn)
 
-## [1.8.1 - 2023-05-04](https://gitlab.com/fame-framework/fame-io/-/tags/v1.8.1)
+## [1.8.1](https://gitlab.com/fame-framework/fame-io/-/tags/v1.8.1) - 2023-05-04
 ### Fixed
 - Fix fail of `ConvertFameResults` when `merge-times` was not specified
 
-## [1.8.0 - 2023-04-14](https://gitlab.com/fame-framework/fame-io/-/tags/v1.8)
+## [1.8.0](https://gitlab.com/fame-framework/fame-io/-/tags/v1.8) - 2023-04-14
 ### Changed
 - Update repository to be compliant to `REUSE` standard
 - Accept custom `date_format` (default: `"%Y-%m-%d_%H:%M:%S"`) for `FameTime.convert_fame_time_step_to_datetime()`
 - Parse command-line arguments case-insensitive for arguments with predefined options
 - Handle potentially missing cli arguments in `cli.update_default_config` for `makeFameRunConfig` and `convertFameResults` in a robust way.
 
 ### Added
 - **Breaking**: Add option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}` for `convertFameResults`
 - Add option to merge time steps in results with `convertFameResults`
 - Add pre-commit hooks enforcing high coding standards and reducing CI runner minutes during development
 
-## [1.7.0 - 2023-02-20](https://gitlab.com/fame-framework/fame-io/-/tags/v1.7)
+## [1.7.0](https://gitlab.com/fame-framework/fame-io/-/tags/v1.7) - 2023-02-20
 ### Added
 - Support dictionaries in Schema for field `Products` in elements of `AgentTypes`
 - Support dictionaries in Schema for field `Values` in elements of `Attributes`
 
 ### Changed
 - Use `Pathlib` for path handling
 - Improve error message when no valid `YAML` file is specified for `makeFameRunConfig`
 
 ### Remove
 - **Breaking**: `Products` in Schema no longer support single non-list values
 
-## [1.6.3 - 2022-11-04](https://gitlab.com/fame-framework/fame-io/-/tags/v1.6.3)
+## [1.6.3](https://gitlab.com/fame-framework/fame-io/-/tags/v1.6.3) - 2022-11-04
 ### Added
 - Allow parsing `Help` for `Attributes` in `schema`
 
-## [1.6.1 - 2022-11-02](https://gitlab.com/fame-framework/fame-io/-/tags/v1.6.1)
+## [1.6.1](https://gitlab.com/fame-framework/fame-io/-/tags/v1.6.1) - 2022-11-02
 ### Changed
 - Use existing logger if already set up to avoid duplicates when `fameio` is used as dependency in third party workflows
 
-## [1.6.0 - 2022-07-08](https://gitlab.com/fame-framework/fame-io/-/tags/v1.6)
+## [1.6.0](https://gitlab.com/fame-framework/fame-io/-/tags/v1.6) - 2022-07-08
 ### Added
 - Add option to enable memory saving mode using the flag `-m` or `--memory-saving`
 - Add options to deal with complex indexed output columns using the flag `-cc` or `--complex-column` with
   options `IGNORE`, `MERGE` or `SPLIT`
 
 ### Changed
 - **Breaking**: Update requirement to `python>=3.8`
 - **Breaking**: Update requirement to `fameprotobuf==v1.2`
 - Enable parsing of protobuf output files > 2 GB
 - Reduce memory profile for `convertFameResults`
 - Extract `source` scripts relevant for `convertFameResults` to be hosted in subpackage `results`
 
-## [1.5.4 - 2022-06-01](https://gitlab.com/fame-framework/fame-io/-/tags/v1.5.4)
+## [1.5.4](https://gitlab.com/fame-framework/fame-io/-/tags/v1.5.4) - 2022-06-01
 ### Changed
 - Limit `protobuf` dependency to `>=3.19,<4.0`
 
-## [1.5.3 - 2022-03-18](https://gitlab.com/fame-framework/fame-io/-/tags/v1.5.3)
+## [1.5.3](https://gitlab.com/fame-framework/fame-io/-/tags/v1.5.3) - 2022-03-18
 ### Changed
 - Harmonize interface with `famegui`
 - Return `None` on failure of `resolve_series_file_path` instead of raising a `FileNotFoundError`
 
-## [1.5.2 - 2022-03-10](https://gitlab.com/fame-framework/fame-io/-/tags/v1.5.2)
+## [1.5.2](https://gitlab.com/fame-framework/fame-io/-/tags/v1.5.2) - 2022-03-10
 ### Changed
 - Allow interfacing of `famegui` with `scenario` (e.g. serialization, error handling)
 - Move `scenario` validation to `validator.py`
 - Extract `path_resolver.py`
 - Increase test coverage by incorporating [AMIRIS examples](https://gitlab.com/dlr-ve/esy/amiris/examples)
 
-## [1.5.1 - 2022-01-10](https://gitlab.com/fame-framework/fame-io/-/tags/v1.5.1)
+## [1.5.1](https://gitlab.com/fame-framework/fame-io/-/tags/v1.5.1) - 2022-01-10
 ### Added
 - Provide documentation on installation using `pipx`
 - Add optional argument `-se`/`--singleexport` for exporting individual files for each agent
 - Add compatibility hook for `famegui` integration
 
 ### Changed
 - Refactor `scenario.py`
 - Ensure code formatting using `black`
 
-## [1.5.0 - 2021-06-30](https://gitlab.com/fame-framework/fame-io/-/tags/v1.5)
+## [1.5.0](https://gitlab.com/fame-framework/fame-io/-/tags/v1.5) - 2021-06-30
 ### Added
 - Support specifying an output folder in command line interface of `convert_results.py`
 
 ### Changed
 - Update to latest protobuf package
 - Refactor code
 
-## [1.4.0 - 2021-06-10](https://gitlab.com/fame-framework/fame-io/-/tags/v1.4)
+## [1.4.0](https://gitlab.com/fame-framework/fame-io/-/tags/v1.4) - 2021-06-10
 ### Added
 - Enable "Default" values for Attributes - these are used in case a mandatory attribute is not specified in the Scenario
 - Allow "List" Attributes with multiple values
 - Add new AttributeTypes "Long", "String" and "TimeStamp"
 - Add compact definition of multiple contracts: enable lists for senders and receivers
 
 ### Changed
@@ -141,64 +161,64 @@
 - Switch to pytest and improved test coverage
 - Make keywords in Schema and Scenario case-insensitive
 - Improve validations for Schema and Scenario
 
 ### Fixed
 - Fixed minor bugs
 
-## [1.3.0 - 2021-04-13](https://gitlab.com/fame-framework/fame-io/-/tags/v1.3)
+## [1.3.0](https://gitlab.com/fame-framework/fame-io/-/tags/v1.3) - 2021-04-13
 ### Added
 - Enable `Attributes` in agents (formerly known as `Fields`) to be structured in complex tree-like data dictionaries
 - Allow contracts to support `Attributes` of type `int`, `float`, `enum` or `dict`
 - Add coverage report badge
 - Add `CHANGELOG.md`
 
 ### Changed
 - **Breaking**: Use new format `DataStorage` for input and output protobuf files allowing `FAME-Core` input and output to be written to the same file (requires `FAME-Core > 1.0`)
 - **Breaking**: Update requirement to `fameprotobuf==1.1.2`
 - Enable automatic detection of `TimeStamps` by string format and conversion to int64
 - Raise proper error when file can not be loaded triggered by `!include` command
 - Raise critical error when trying to convert empty protobuf output file
 - Check if `product` in `contract` is valid according to `schema.yaml`
 
-## [1.2.4 - 2021-02-26](https://gitlab.com/fame-framework/fame-io/-/tags/v1.2.4)
+## [1.2.4](https://gitlab.com/fame-framework/fame-io/-/tags/v1.2.4) - 2021-02-26
 ### Changed
 - Move `is_compatible` function to class `AttributeType`
 
-## [1.2.3 - 2021-02-24](https://gitlab.com/fame-framework/fame-io/-/tags/v1.2.3)
+## [1.2.3](https://gitlab.com/fame-framework/fame-io/-/tags/v1.2.3) - 2021-02-24
 ### Fixed
 - Fix file prefix `IGNORE_` (used when loading a set of contract files with the !include argument) is now working consistently
 
-## [1.2.2 - 2021-02-18](https://gitlab.com/fame-framework/fame-io/-/tags/v1.2.2)
+## [1.2.2](https://gitlab.com/fame-framework/fame-io/-/tags/v1.2.2) - 2021-02-18
 ### Changed
 - **Breaking**: Rename `fieldtype` to `attributetype` in `schema.yaml`
 - Derive protobuf imports from `fameprotobuf` package
 - Improve handling of cases for keys in `scenario.yaml`
 - Improve handling of time stamp strings
 
-## [1.2.1 - 2021-02-10](https://gitlab.com/fame-framework/fame-io/-/tags/v1.2.1)
+## [1.2.1](https://gitlab.com/fame-framework/fame-io/-/tags/v1.2.1) - 2021-02-10
 ### Changed
 - Improve key handling for contracts which are now case-insensitive
 
-## [1.2.0 - 2021-02-04](https://gitlab.com/fame-framework/fame-io/-/tags/v1.2)
+## [1.2.0](https://gitlab.com/fame-framework/fame-io/-/tags/v1.2) - 2021-02-04
 ### Added
 - Add `!include` command to yaml loading to allow integrating additional yaml files
 
 ### Changed
 - **Breaking**: Rename package to `fameio`
 - Improve executables
 - Restructure logging
 - Improve documentation
 
 ### Fixed
 - Fix bugs
 
-## [1.1.0 - 2020-12-09](https://gitlab.com/fame-framework/fame-io/-/tags/v1.1)
+## [1.1.0](https://gitlab.com/fame-framework/fame-io/-/tags/v1.1) - 2020-12-09
 ### Added
 - Package to PyPI
 - Provide executables for calling `makeFameRunConfig` and `convertFameResults`
 
 ### Changed
 - Improve documentation
 
-## [1.0.0 - 2020-11-17](https://gitlab.com/fame-framework/fame-io/-/tags/v1.0)
+## [1.0.0](https://gitlab.com/fame-framework/fame-io/-/tags/v1.0) - 2020-11-17
 _Initial release of `famepy`_
```

### Comparing `fameio-2.0.0/LICENSE.txt` & `fameio-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/LICENSES/Apache-2.0.txt` & `fameio-2.1.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/LICENSES/CC-BY-4.0.txt` & `fameio-2.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/LICENSES/CC0-1.0.txt` & `fameio-2.1.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/pyproject.toml` & `fameio-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fameio"
-version = "2.0.0"
+version = "2.1.0"
 description = "Python scripts for operation of FAME models"
 license = "Apache-2.0"
 authors = [
     "Felix Nitsch <fame@dlr.de>",
     "Christoph Schimeczek <fame@dlr.de>",
     "Ulrich Frey <fame@dlr.de>",
     "Benjamin Fuchs <fame@dlr.de>",
@@ -31,15 +31,15 @@
     "Intended Audience :: Science/Research",
 ]
 packages = [{include = "fameio", from = "src"}]
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-fameprotobuf = "^1.4.0"
+fameprotobuf = "^1.5.0"
 pandas = ">= 1.0, <3.0"
 pyyaml = "^6.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `fameio-2.0.0/README.md` & `fameio-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+<!-- SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 
 SPDX-License-Identifier: Apache-2.0 -->
 [![PyPI version](https://badge.fury.io/py/fameio.svg)](https://badge.fury.io/py/fameio)
 [![JOSS](https://joss.theoj.org/papers/10.21105/joss.04958/status.svg)](https://doi.org/10.21105/joss.04958)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.4314337.svg)](https://doi.org/10.5281/zenodo.4314337)
 [![PyPI license](https://img.shields.io/pypi/l/fameio.svg)](https://badge.fury.io/py/fameio)
 [![pipeline status](https://gitlab.com/fame-framework/fame-io/badges/main/pipeline.svg)](https://gitlab.com/fame-framework/fame-io/commits/main)
@@ -96,41 +96,53 @@
 ```
 
 ### Scenario YAML
 The "scenario.yaml" file contains all configuration options for a FAME-based simulation.
 It consists of the sections `Schema`, `GeneralProperties`, `Agents` and `Contracts`, all of them described below.
 
 #### Schema
-The Schema is used to validate the inputs of the "scenario.yaml".
-Since the Schema should be valid across multiple scenarios, it is recommended to defined it in a separate file and include the file here.
+The Schema describes a model's components such as its types of agents, their inputs, what data they exchange, etc. 
+It is also used to validate the model inputs provided in the `scenario.yaml`. 
+Since the Schema is valid until the model itself is changed, it is recommended to defined it in a separate file and include the file here.
 
 Currently, the schema specifies:
 * which type of Agents can be created
 * what type of input attributes an Agent uses
-* what type of Products an Agent can send in Contracts.
+* what type of Products an Agent can send in Contracts, and
+* the names of the Java packages for the classes corresponding to Agents, DataItems and Portables. 
 
-The Schema consists of the sections `Header` and `AgentTypes`.
+The Schema consists of the sections `JavaPackages` and `AgentTypes`.
 
-##### Header
-Scientific applications often evolve, and so do their required input parameters.
-Therefore, the header specifies information what FAME-based application the schema is corresponding to.
-In this way a schema.yaml is tied to a specific version an application, ensuring a match between the inputs required by
-the application, and those provided by the files created with FAME-Io.
-
-```yaml
-Header:
-  Project: MyProjectName
-  RepoUrl: https://mygithosting.com/myProject
-  CommitHash: abc123
+##### JavaPackages
+This section defines the name of the Java packages in which the model code is located.
+A similar data set was formerly specified in the `fameSetup.yaml`, but is now specified in the schema.
+Each of the three sections `Agents`, `DataItems`, and `Portables` contain a list of fully qualified java package names of your model's classes.
+Package names can occur in multiple lists and may overlap.
+It is not necessary (but possible) to specify the nearest enclosing package for each Agent, DataItem or Portable.
+Specifying any super-package will also work.
+Also, package names occur on multiple lists for Agent, DataItem or Portable.
+
+For example, for a project with all its
+* Agent-derived java classes located in packages below the package named "agents",
+* DataItem implementation classes in a subpackage named "msg",
+* Portable implementation classes in a subpackages named "portableItems" and "otherPortables", 
+
+the corresponding section in the schema would look like this:
+
+```yaml
+JavaPackages:
+  Agents:
+    - "agents"
+  DataItems:
+    - "msg"
+  Portables:
+    - "portableItems"
+    - "otherPortables"
 ```
 
-* `Project` name of your project / FAME-based application
-* `RepoUrl` URL of your project
-* `CommitHash` hash of the commit / version of your project
-
 ##### AgentTypes
 Here, each type of agent that can be created in your FAME-based application is listed, its attributes and its available Products for Contracts.
 The structure of this section
 
 ```yaml
 AgentTypes:
   MyAgentType:
@@ -552,25 +564,25 @@
 An individual file for each type of Agent is created in a folder named after the protobuf input file.
 Call structure:
 
     convertFameResults -f <./path/to/protobuf_file.pb>
 
 You may also specify any of the following arguments:
 
-| Command                                     | Action                                                                                                                                                                                                                                              |
-|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `-l` or `--log` <option>                    | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.                                                                                                                                     |
-| `-lf` or `--logfile` <file>                 | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                                                                                                                                          |
-| `-a` or `--agents` <list-of-agents>         | If specified, only a subset of agents is extracted from the protobuf file. Default is to extract all agents.                                                                                                                                        |
-| `-o` or `--output`                          | Sets the path to where the generated output files are written to. If not specified, the folder's name is derived from the input file's name. Folder will be created if it does not exist.                                                           |
-| `-se` or `--single-export`                  | Enables export of individual agents to individual files, when present. If not present (the default) one file per `AgentType` is created.                                                                                                            |
-| `-m` or `--memory-saving`                   | When specified, reduces memory usage profile at the cost of runtime. Use only when necessary.                                                                                                                                                       |
-| `-cc` or `--complex-column` <option>        | Defines how to deal with complex indexed output columns (if any). `IGNORE` ignores complex columns. `MERGE` squashes all data from complex columns in one big string entry. `SPLIT` creates a separate file for each complex indexed output column. |
-| `-t` or `--time` <option>                   | Option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}`                                                                                                                                           |
-| `--input-recovery` or `--no-input-recovery` | If True, all input data are recovered as well as the outputs (default=False).                                                                                                                                                                       |
+| Command                                     | Action                                                                                                                                                                                    |
+|---------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `-l` or `--log` <option>                    | Sets the logging level. Default is `WARNING`. Options are `DEBUG`, `INFO`, `WARNING`, `ERROR`, `CRITICAL`.                                                                                |
+| `-lf` or `--logfile` <file>                 | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                                                                                |
+| `-a` or `--agents` <list-of-agents>         | If specified, only a subset of agents is extracted from the protobuf file. Default is to extract all agents.                                                                              |
+| `-o` or `--output`                          | Sets the path to where the generated output files are written to. If not specified, the folder's name is derived from the input file's name. Folder will be created if it does not exist. |
+| `-se` or `--single-export`                  | Enables export of individual agents to individual files, when present. If not present (the default) one file per `AgentType` is created.                                                  |
+| `-m` or `--memory-saving`                   | When specified, reduces memory usage profile at the cost of runtime. Use only when necessary.                                                                                             |
+| `-cc` or `--complex-column` <option>        | Defines how to deal with complex indexed output columns (if any). `IGNORE` ignores complex columns. `SPLIT` creates a separate file for each complex indexed output column.               |
+| `-t` or `--time` <option>                   | Option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}`                                                                                 |
+| `--input-recovery` or `--no-input-recovery` | If True, all input data are recovered as well as the outputs (default=False).                                                                                                             |
 
 Additionally, you may merge TimeSteps of a certain range of steps in the output files to
 i) associate multiple time steps with a common logical time in your simulation
 ii) reduce number of lines in output files
 
 For this, add the option `merge-times` and specify the arguments as follows:
```

### Comparing `fameio-2.0.0/src/fameio/scripts/__init__.py` & `fameio-2.1.0/src/fameio/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/src/fameio/scripts/convert_results.py` & `fameio-2.1.0/src/fameio/scripts/convert_results.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 from pathlib import Path
 
 from fameio.source.cli.convert_results import handle_args, CLI_DEFAULTS as DEFAULT_CONFIG
 from fameio.source.cli.options import Options
 from fameio.source.cli.parser import update_default_config
-from fameio.source.logs import log_and_raise_critical, set_up_logger, logger
+from fameio.source.logs import log_and_raise_critical, fameio_logger, log
 from fameio.source.results.agent_type import AgentTypeLog
 from fameio.source.results.conversion import apply_time_option, apply_time_merging
 from fameio.source.results.csv_writer import CsvWriter
 from fameio.source.results.data_transformer import DataTransformer
 from fameio.source.results.input_dao import InputDao
 from fameio.source.results.output_dao import OutputDAO
 from fameio.source.results.reader import Reader
@@ -19,53 +19,53 @@
 ERR_MEMORY_ERROR = "Out of memory. Try using `-m` or `--memory-saving` option."
 ERR_MEMORY_SEVERE = "Out of memory despite memory-saving mode. Reduce output interval in `FAME-Core` and rerun model"
 
 
 def run(config: dict = None) -> None:
     """Reads file in protobuf format for configures FILE and extracts its content to .csv file(s)"""
     config = update_default_config(config, DEFAULT_CONFIG)
-    set_up_logger(level_name=config[Options.LOG_LEVEL], file_name=config[Options.LOG_FILE])
+    fameio_logger(log_level_name=config[Options.LOG_LEVEL], file_name=config[Options.LOG_FILE])
 
     file_path = config[Options.FILE]
     output_writer = CsvWriter(config[Options.OUTPUT], Path(file_path), config[Options.SINGLE_AGENT_EXPORT])
     file_stream = open(Path(file_path), "rb")
 
     if config[Options.MEMORY_SAVING]:
-        logger().info("Memory saving mode enabled: Disable on conversion of small files for performance improvements.")
+        log().info("Memory saving mode enabled: Disable on conversion of small files for performance improvements.")
 
-    logger().info("Reading and extracting data...")
+    log().info("Reading and extracting data...")
     reader = Reader.get_reader(file=file_stream, read_single=config[Options.MEMORY_SAVING])
     agent_type_log = AgentTypeLog(requested_agents=config[Options.AGENT_LIST])
     data_transformer = DataTransformer.build(config[Options.RESOLVE_COMPLEX_FIELD])
     try:
         input_dao = InputDao()
         while data_storages := reader.read():
             if config[Options.INPUT_RECOVERY]:
                 input_dao.store_inputs(data_storages)
             output = OutputDAO(data_storages, agent_type_log)
             for agent_name in output.get_sorted_agents_to_extract():
-                logger().debug(f"Extracting data for {agent_name}...")
+                log().debug(f"Extracting data for {agent_name}...")
                 data_frames = output.get_agent_data(agent_name, data_transformer)
                 apply_time_merging(data_frames, config[Options.TIME_MERGING])
                 apply_time_option(data_frames, config[Options.TIME])
-                logger().debug(f"Writing data for {agent_name}...")
+                log().debug(f"Writing data for {agent_name}...")
                 output_writer.write_to_files(agent_name, data_frames)
 
         if config[Options.INPUT_RECOVERY]:
-            logger().info("Recovering inputs...")
+            log().info("Recovering inputs...")
             timeseries, scenario = input_dao.recover_inputs()
             series_writer = CsvWriter(Path(config[Options.OUTPUT], "./recovered"), Path("./"), False)
             series_writer.write_time_series_to_disk(timeseries)
             data_to_yaml_file(scenario.to_dict(), Path(config[Options.OUTPUT], "./recovered/scenario.yaml"))
 
-        logger().info("Data conversion completed.")
+        log().info("Data conversion completed.")
     except MemoryError:
         log_and_raise_critical(ERR_MEMORY_SEVERE if Options.MEMORY_SAVING else ERR_MEMORY_ERROR)
 
     file_stream.close()
     if not agent_type_log.has_any_agent_type():
-        logger().error("Provided file did not contain any output data.")
+        log().error("Provided file did not contain any output data.")
 
 
 if __name__ == "__main__":
     run_config = handle_args(sys.argv[1:])
     run(run_config)
```

### Comparing `fameio-2.0.0/src/fameio/scripts/make_config.py` & `fameio-2.1.0/src/fameio/scripts/make_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 import sys
 from pathlib import Path
 
 from fameio.source.cli.make_config import handle_args, CLI_DEFAULTS as DEFAULT_CONFIG
 from fameio.source.cli.options import Options
 from fameio.source.cli.parser import update_default_config
 from fameio.source.loader import load_yaml, check_for_yaml_file_type
-from fameio.source.logs import set_up_logger, logger
+from fameio.source.logs import fameio_logger, log
 from fameio.source.scenario import Scenario
 from fameio.source.validator import SchemaValidator
 from fameio.source.writer import ProtoWriter
 
 
 def run(config: dict = None) -> None:
     """Executes the main workflow for the building of a FAME configuration file"""
     config = update_default_config(config, DEFAULT_CONFIG)
-    set_up_logger(level_name=config[Options.LOG_LEVEL], file_name=config[Options.LOG_FILE])
+    fameio_logger(log_level_name=config[Options.LOG_LEVEL], file_name=config[Options.LOG_FILE])
 
     file = config[Options.FILE]
     check_for_yaml_file_type(Path(file))
     scenario = Scenario.from_dict(load_yaml(Path(file)))
     SchemaValidator.check_agents_have_contracts(scenario)
 
     timeseries_manager = SchemaValidator.validate_scenario_and_timeseries(scenario)
     writer = ProtoWriter(config[Options.OUTPUT], timeseries_manager)
     writer.write_validated_scenario(scenario)
 
-    logger().info("Configuration completed.")
+    log().info("Configuration completed.")
 
 
 if __name__ == "__main__":
     run_config = handle_args(sys.argv[1:])
     run(run_config)
```

### Comparing `fameio-2.0.0/src/fameio/source/cli/convert_results.py` & `fameio-2.1.0/src/fameio/source/cli/convert_results.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     add_merge_time_parser,
     add_inputs_recovery_argument,
     map_namespace_to_options_dict,
 )
 
 CLI_DEFAULTS = {
     Options.FILE: None,
-    Options.LOG_LEVEL: "info",
+    Options.LOG_LEVEL: "WARN",
     Options.LOG_FILE: None,
     Options.AGENT_LIST: None,
     Options.OUTPUT: None,
     Options.SINGLE_AGENT_EXPORT: False,
     Options.MEMORY_SAVING: False,
     Options.RESOLVE_COMPLEX_FIELD: ResolveOptions.SPLIT,
     Options.TIME: TimeOptions.UTC,
@@ -35,15 +35,24 @@
 }
 
 _INFILE_PATH_HELP = "Provide path to protobuf file"
 _OUTFILE_PATH_HELP = "Provide path to folder to store output .csv files"
 
 
 def handle_args(args: List[str], defaults: Optional[Dict[Options, Any]] = None) -> Dict[Options, Any]:
-    """Handles command line arguments and returns `input_file` and `run_config` for convert_results script"""
+    """
+    Handles command line arguments and returns `run_config` for convert_results script
+
+    Args:
+        args: list of (command line) arguments, e.g., ['-f', 'my_file']; arg values take precedence over defaults
+        defaults: optional default values used for unspecified parameters; missing defaults are replaced by CLI defaults
+
+    Returns:
+        final configuration compiled from (given) `defaults` and given `args`
+    """
     parser = _prepare_parser(defaults)
     parsed = parser.parse_args(args)
     return map_namespace_to_options_dict(parsed)
 
 
 def _prepare_parser(defaults: Optional[Dict[Options, Any]]) -> argparse.ArgumentParser:
     """
```

### Comparing `fameio-2.0.0/src/fameio/source/cli/make_config.py` & `fameio-2.1.0/src/fameio/source/cli/make_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     add_logfile_argument,
     add_output_argument,
     map_namespace_to_options_dict,
 )
 
 CLI_DEFAULTS = {
     Options.FILE: None,
-    Options.LOG_LEVEL: "info",
+    Options.LOG_LEVEL: "WARN",
     Options.LOG_FILE: None,
     Options.OUTPUT: Path("config.pb"),
 }
 
 _INFILE_PATH_HELP = "provide path to configuration file"
 _OUTFILE_PATH_HELP = "provide file-path for the file to generate"
 
@@ -30,15 +30,15 @@
     Converts given `arguments` and returns a configuration for the make_config script
 
     Args:
         args: list of (command line) arguments, e.g., ['-f', 'my_file']; arg values take precedence over defaults
         defaults: optional default values used for unspecified parameters; missing defaults are replaced by CLI defaults
 
     Returns:
-        final configuration compiled from (given) defaults and
+        final configuration compiled from (given) `defaults` and given `args`
     """
     parser = _prepare_parser(defaults)
     parsed = parser.parse_args(args)
     return map_namespace_to_options_dict(parsed)
 
 
 def _prepare_parser(defaults: Optional[Dict[Options, Any]]) -> argparse.ArgumentParser:
```

### Comparing `fameio-2.0.0/src/fameio/source/cli/options.py` & `fameio-2.1.0/src/fameio/source/cli/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
 
 class ResolveOptions(ParsableEnum, Enum):
     """Specifies options for resolving complex fields in output files"""
 
     IGNORE = auto()
     SPLIT = auto()
-    MERGE = auto()
 
 
 class MergingOptions(Enum):
     """Specifies options for merging TimeSteps"""
 
     FOCAL_POINT = auto()
     STEPS_BEFORE = auto()
```

### Comparing `fameio-2.0.0/src/fameio/source/cli/parser.py` & `fameio-2.1.0/src/fameio/source/cli/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import copy
 from argparse import ArgumentParser, ArgumentTypeError, BooleanOptionalAction, Namespace
 from enum import Enum
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
 from fameio.source.cli.options import MergingOptions, TimeOptions, ResolveOptions, Options
-from fameio.source.logs import LOG_LEVELS
+from fameio.source.logs import LogLevel
 
 _ERR_NEGATIVE_INT = "Given value `{}` is not a non-negative int."
 
 _OPTION_ARGUMENT_NAME: Dict[str, Union[Options, Dict]] = {
     "file": Options.FILE,
     "log": Options.LOG_LEVEL,
     "logfile": Options.LOG_FILE,
@@ -70,16 +70,16 @@
 def add_log_level_argument(parser: ArgumentParser, default_value: str) -> None:
     """Adds optional argument 'log' to given `parser`"""
     help_text = "choose logging level (default: {})".format(default_value)
     parser.add_argument(
         "-l",
         "--log",
         default=default_value,
-        choices=list(LOG_LEVELS.keys()),
-        type=str.lower,
+        choices=[level.name for level in LogLevel if level not in [LogLevel.PRINT, LogLevel.WARN]],
+        type=str.upper,
         help=help_text,
     )
 
 
 def add_single_export_argument(parser: ArgumentParser, default_value: bool) -> None:
     """Adds optional repeatable string argument 'agent' to given `parser`"""
     help_text = "Enable export of single agents (default=False)"
```

### Comparing `fameio-2.0.0/src/fameio/source/loader.py` & `fameio-2.1.0/src/fameio/source/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os
 from pathlib import Path
 from fnmatch import fnmatch
 from typing import IO, Any, Callable
 
 import yaml
-from fameio.source.logs import log_and_raise_critical, logger
+from fameio.source.logs import log_and_raise_critical, log
 from fameio.source.path_resolver import PathResolver
 
 DISABLING_YAML_FILE_PREFIX = "IGNORE_"
 
 CRIT_ERR_NO_YAML_GIVEN = "Please provide a valid YAML file. Received `-f/--file {}` instead."
 
 
@@ -24,23 +24,23 @@
 
 def read_args(loader, args):
     """Returns two Strings to be interpreted as files to be read and a sub-node_address from the given `args`"""
     node_string = ""
     file_string = None
     if isinstance(args, yaml.nodes.ScalarNode):
         file_string = loader.construct_scalar(args)
-        logger().debug("Found instance `ScalarNode` in {}".format(file_string))
+        log().debug("Found instance `ScalarNode` in {}".format(file_string))
     elif isinstance(args, yaml.nodes.SequenceNode):
         argument_list = loader.construct_sequence(args)
         if len(argument_list) not in [1, 2]:
             log_and_raise_critical("!include supports but one or two arguments in list")
         elif len(argument_list) == 2:
             node_string = argument_list[1]
         file_string = argument_list[0]
-        logger().debug("Found instance `SequenceNode` in {}".format(file_string))
+        log().debug("Found instance `SequenceNode` in {}".format(file_string))
     elif isinstance(args, yaml.nodes.MappingNode):
         argument_map = loader.construct_mapping(args)
         for key, value in argument_map.items():
             if key.lower() == "file":
                 file_string = value
             elif key.lower() == "node":
                 node_string = value
@@ -51,23 +51,23 @@
     else:
         log_and_raise_critical("YAML node type not implemented: {}".format(args))
     return Args(file_string, node_string)
 
 
 def split_nodes(node_string):
     """Returns a list of nodes created from the given `node_string`"""
-    logger().debug("Splitting given node_string `{}`".format(node_string))
+    log().debug("Splitting given node_string `{}`".format(node_string))
     return node_string.split(":")
 
 
 class FameYamlLoader(yaml.SafeLoader):
     """Custom YAML Loader for `!include` constructor"""
 
     def __init__(self, stream: IO, path_resolver=PathResolver()) -> None:
-        logger().debug("Initialize custom YAML loader")
+        log().debug("Initialize custom YAML loader")
         self._path_resolver = path_resolver
         try:
             self._root_path = os.path.split(stream.name)[0]
         except AttributeError:
             self._root_path = os.path.curdir
         super().__init__(stream)
 
@@ -95,33 +95,33 @@
     """
     file_list = loader.path_resolver.resolve_yaml_imported_file_pattern(loader.root_path, included_path)
 
     ignore_filter = "*" + DISABLING_YAML_FILE_PREFIX + "*"
     cleaned_file_list = []
     for file in file_list:
         if fnmatch(file, ignore_filter):
-            logger().debug("Ignoring file {} due to prefix {}".format(file, DISABLING_YAML_FILE_PREFIX))
+            log().debug("Ignoring file {} due to prefix {}".format(file, DISABLING_YAML_FILE_PREFIX))
         else:
             cleaned_file_list.append(file)
     if not cleaned_file_list:
         log_and_raise_critical("Failed to find any file matching the `!include` directive `{}`".format(included_path))
-    logger().debug("Collected file(s) `{}` from given included path `{}`".format(cleaned_file_list, included_path))
+    log().debug("Collected file(s) `{}` from given included path `{}`".format(cleaned_file_list, included_path))
     return cleaned_file_list
 
 
 def read_data_from_file(file, node_address, path_resolver: PathResolver):
     """Returns data of the specified `node_address` from the specified `file`"""
     data = yaml.load(file, make_yaml_loader_builder(path_resolver))
     for node in node_address:
         if node:
             try:
                 data = data[node]
             except KeyError:
                 log_and_raise_critical("'!include_node [{}, {}]': Cannot find '{}'.".format(file, node_address, node))
-    logger().debug("Searched file `{}` for node `{}`".format(file, node_address))
+    log().debug("Searched file `{}` for node `{}`".format(file, node_address))
     return data
 
 
 def join_data(new_data, previous_data):
     """Joins data from multiple files if both are in list format, otherwise returns"""
     if not previous_data:
         return new_data
@@ -152,24 +152,24 @@
     files = resolve_imported_path(loader, args.file_string)
 
     joined_data = None
     for file_name in files:
         with open(file_name, "r") as open_file:
             data = read_data_from_file(open_file, nodes, loader.path_resolver)
             joined_data = join_data(data, joined_data)
-    logger().debug("Joined all files `{}` to joined data `{}`".format(files, joined_data))
+    log().debug("Joined all files `{}` to joined data `{}`".format(files, joined_data))
     return joined_data
 
 
 FameYamlLoader.add_constructor("!include", construct_include)
 
 
 def load_yaml(yaml_file_path: Path, path_resolver=PathResolver()):
     """Loads the yaml file from given `yaml_file_path` and returns its content"""
-    logger().info("Loading yaml from {}".format(yaml_file_path))
+    log().info("Loading yaml from {}".format(yaml_file_path))
     with open(yaml_file_path, "r") as configfile:
         data = yaml.load(configfile, make_yaml_loader_builder(path_resolver))
     return data
 
 
 def check_for_yaml_file_type(yaml_file_path: Path) -> None:
     """Raises Exception if given `yaml_file_path` is not a valid YAML file"""
```

### Comparing `fameio-2.0.0/src/fameio/source/path_resolver.py` & `fameio-2.1.0/src/fameio/source/path_resolver.py`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/src/fameio/source/results/agent_type.py` & `fameio-2.1.0/src/fameio/source/results/agent_type.py`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/src/fameio/source/results/conversion.py` & `fameio-2.1.0/src/fameio/source/results/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import math
 from typing import Dict, Optional
 
 import pandas as pd
 
 from fameio.source import FameTime
 from fameio.source.cli.options import TimeOptions, MergingOptions
-from fameio.source.logs import log_error_and_raise, logger
+from fameio.source.logs import log_error_and_raise, log
 from fameio.source.time import ConversionException
 
 _ERR_UNIMPLEMENTED = "Time conversion mode '{}' not implemented."
 
 
 def apply_time_merging(data: Dict[Optional[str], pd.DataFrame], config: Optional[Dict[MergingOptions, int]]) -> None:
     """
@@ -23,15 +23,15 @@
         data: one or multiple DataFrames of time series; column `TimeStep` might be modified
         config: dict of MergingOptions defining how to merge the TimeSteps
 
     Returns:
         Nothing - data is modified inplace
     """
     if config:
-        logger().debug(f"Grouping TimeSteps...")
+        log().debug(f"Grouping TimeSteps...")
         offset = config[MergingOptions.STEPS_BEFORE]
         period = config[MergingOptions.STEPS_AFTER] + config[MergingOptions.STEPS_BEFORE] + 1
         first_positive_focal_point = config[MergingOptions.FOCAL_POINT] % period
         for key in data.keys():
             df = data[key]
             index_columns = df.index.names
             df.reset_index(inplace=True)
@@ -63,15 +63,15 @@
         data: one or multiple DataFrames of time series; column `TimeStep` might be modified (depending on mode)
         mode: name of time conversion mode (derived from Enum)
 
     Returns:
         Nothing - data is modified inplace
     """
     if mode == TimeOptions.INT:
-        logger().debug("No time conversion...")
+        log().debug("No time conversion...")
     elif mode == TimeOptions.UTC:
         _convert_time_index(data, "%Y-%m-%d %H:%M:%S")
     elif mode == TimeOptions.FAME:
         _convert_time_index(data, "%Y-%m-%d_%H:%M:%S")
     else:
         log_error_and_raise(ConversionException(_ERR_UNIMPLEMENTED.format(mode)))
 
@@ -84,13 +84,13 @@
     Args:
         data: one or multiple DataFrames of time series; column `TimeStep` will be modified
         datetime_format: used for the conversion
 
     Returns:
         Nothing - data is modified inplace
     """
-    logger().debug(f"Converting TimeStep to format '{datetime_format}'...")
+    log().debug(f"Converting TimeStep to format '{datetime_format}'...")
     for _, df in data.items():
         index_columns = df.index.names
         df.reset_index(inplace=True)
         df["TimeStep"] = df["TimeStep"].apply(lambda t: FameTime.convert_fame_time_step_to_datetime(t, datetime_format))
         df.set_index(keys=index_columns, inplace=True)
```

### Comparing `fameio-2.0.0/src/fameio/source/results/csv_writer.py` & `fameio-2.1.0/src/fameio/source/results/csv_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from pathlib import Path
 from typing import Dict, Union
 
 import pandas as pd
 
-from fameio.source.logs import logger
+from fameio.source.logs import log
 from fameio.source.results.data_transformer import INDEX
 from fameio.source.series import TimeSeriesManager
 from fameio.source.tools import ensure_path_exists
 
 
 class CsvWriter:
     """Writes dataframes to different csv files"""
@@ -26,23 +26,23 @@
         self._create_output_folder()
 
     @staticmethod
     def _get_output_folder_name(config_output: Path, input_file_path: Path) -> Path:
         """Returns name of the output folder derived either from the specified `config_output` or `input_file_path`"""
         if config_output:
             output_folder_name = config_output
-            logger().info(CsvWriter._INFO_USING_PATH.format(config_output))
+            log().info(CsvWriter._INFO_USING_PATH.format(config_output))
         else:
             output_folder_name = input_file_path.stem
-            logger().info(CsvWriter._INFO_USING_DERIVED_PATH.format(output_folder_name))
+            log().info(CsvWriter._INFO_USING_DERIVED_PATH.format(output_folder_name))
         return Path(output_folder_name)
 
     def _create_output_folder(self) -> None:
         """Creates output folder if not yet present"""
-        logger().debug("Creating output folder if required...")
+        log().debug("Creating output folder if required...")
         if not self._output_folder.is_dir():
             self._output_folder.mkdir(parents=True)
 
     def write_to_files(self, agent_name: str, data: Dict[Union[None, str], pd.DataFrame]) -> None:
         """Writes `data` for given `agent_name` to .csv file(s)"""
         for column_name, column_data in data.items():
             column_data.sort_index(inplace=True)
```

### Comparing `fameio-2.0.0/src/fameio/source/results/data_transformer.py` & `fameio-2.1.0/src/fameio/source/results/data_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 
 class DataTransformer(ABC):
     """Extracts and provides series data from parsed and processed output files for requested agents"""
 
     MODES = {
         ResolveOptions.IGNORE: lambda: DataTransformerIgnore(),
-        ResolveOptions.MERGE: lambda: DataTransformerMerge(),
         ResolveOptions.SPLIT: lambda: DataTransformerSplit(),
     }
     SIMPLE_COLUMN_INDEX = -1
 
     @staticmethod
     def build(complex_column_mode: ResolveOptions) -> DataTransformer:
         return DataTransformer.MODES[complex_column_mode]()
@@ -43,22 +42,22 @@
         data_frames = {}
         for column_id, agent_data in container.items():
             data_frame = DataFrame.from_dict(agent_data, orient="index")
             column_name = agent_type.get_column_name_for_id(column_id)
             if column_id == DataTransformer.SIMPLE_COLUMN_INDEX:
                 data_frame.rename(columns=self._get_column_map(agent_type), inplace=True)
                 index = INDEX
+                data_frame = data_frame.loc[:, agent_type.get_simple_column_mask()]
             else:
                 data_frame.rename(columns={0: column_name}, inplace=True)
                 index = INDEX + agent_type.get_inner_columns(column_id)
 
             if not data_frame.empty:
                 data_frame.index = pd.MultiIndex.from_tuples(data_frame.index)
                 data_frame.rename_axis(index, inplace=True)
-            data_frame.dropna(how="all", axis=1, inplace=True)
             data_frames[column_name] = data_frame
         return data_frames
 
     def _extract_agent_data(
         self, series: List[Output.Series], agent_type: AgentType
     ) -> Dict[int, Dict[Tuple, List[Union[float, None, str]]]]:
         """Returns mapping of (agentId, timeStep) to fixed-length list of all output columns for given `class_name`"""
@@ -78,18 +77,18 @@
     def _add_series_data(
         self,
         series: Output.Series,
         mask_simple: List[bool],
         container: Dict[int, Dict[Tuple, List[Union[float, None, str]]]],
     ) -> None:
         """Adds data from given `series` to specified `container` dict as list"""
-        dummy_list = [None] * len(mask_simple)
+        empty_list = [None] * len(mask_simple)
         for line in series.line:
             index = (series.agentId, line.timeStep)
-            simple_values = dummy_list.copy()
+            simple_values = empty_list.copy()
             for column in line.column:
                 if mask_simple[column.fieldId]:
                     simple_values[column.fieldId] = column.value
                 else:
                     self._merge_complex_column(column, simple_values)
                     self._store_complex_values(column, container, index)
             container[DataTransformer.SIMPLE_COLUMN_INDEX][index] = simple_values
@@ -110,30 +109,14 @@
         return agent_type.get_simple_column_map()
 
 
 class DataTransformerIgnore(DataTransformer):
     """Ignores complex columns on output"""
 
 
-class DataTransformerMerge(DataTransformer):
-    """Merges complex columns on output into a single column entry"""
-
-    def _get_column_map(self, agent_type: AgentType) -> Dict[int, str]:
-        """Returns mapping of simple (and merged) column IDs to their name (or enhanced name) for given `agent_type`"""
-        return agent_type.get_merged_column_map()
-
-    @staticmethod
-    def _merge_complex_column(column: Output.Series.Line.Column, values: List) -> None:
-        """Merges given complex `column` content and saves it to given `values` list"""
-        result = []
-        for entry in column.entry:
-            result.append((tuple(entry.indexValue), entry.value))
-        values[column.fieldId] = result
-
-
 class DataTransformerSplit(DataTransformer):
     @staticmethod
     def _store_complex_values(column: Output.Series.Line.Column, container: Dict[int, Dict], base_index: Tuple) -> None:
         """Adds inner data from `column` to given `container` - split by column type"""
         for entry in column.entry:
             index = base_index + tuple(entry.indexValue)
             container[column.fieldId][index] = entry.value
```

### Comparing `fameio-2.0.0/src/fameio/source/results/input_dao.py` & `fameio-2.1.0/src/fameio/source/results/input_dao.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import ast
 from typing import List, Dict, Any, Optional, Tuple
 
 from fameprotobuf.DataStorage_pb2 import DataStorage
 from fameprotobuf.Field_pb2 import NestedField
 from fameprotobuf.InputFile_pb2 import InputData
 
-from fameio.source.logs import logger
+from fameio.source.logs import log
 from fameio.source.scenario import GeneralProperties, Agent, Contract, Scenario
 from fameio.source.schema import Schema, AttributeSpecs, AttributeType
 from fameio.source.series import TimeSeriesManager
 
 
 class InputConversionException(Exception):
     """An Exception indication an error during reconstruction of input from its protobuf representation"""
@@ -76,18 +76,18 @@
         """
         Check that exactly one previously extracted input data exist, otherwise raises an exception
 
         Raises:
             InputConversionException: if no or more than one input is present
         """
         if not self._inputs:
-            logger().error(self._ERR_NO_INPUTS)
+            log().error(self._ERR_NO_INPUTS)
             raise InputConversionException(self._ERR_NO_INPUTS)
         if len(self._inputs) > 1:
-            logger().error(self._ERR_MULTIPLE_INPUTS)
+            log().error(self._ERR_MULTIPLE_INPUTS)
             raise InputConversionException(self._ERR_MULTIPLE_INPUTS)
         return self._inputs[0]
 
     @staticmethod
     def _get_schema(input_data: InputData) -> Schema:
         """Read and return Schema from given `input_data`"""
         return Schema.from_string(input_data.schema)
```

### Comparing `fameio-2.0.0/src/fameio/source/results/output_dao.py` & `fameio-2.1.0/src/fameio/source/results/output_dao.py`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/src/fameio/source/results/reader.py` & `fameio-2.1.0/src/fameio/source/results/reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import typing
 from abc import ABC, abstractmethod
 from typing import IO, List
 
 from fameprotobuf.DataStorage_pb2 import DataStorage
 from google.protobuf.message import DecodeError
 
-from fameio.source.logs import logger
+from fameio.source.logs import log
 
 
 class Reader(ABC):
     """Abstract base class for protobuf file readers"""
 
     _WARN_NO_HEADER = "No header recognised in file. File might be deprecated or corrupted."  # noqa
     _ERR_FILE_CORRUPT_NEGATIVE_LENGTH = "Corrupt file, message length must be positive."
@@ -47,31 +47,31 @@
         Args:
             file: to be read by the returned Reader
             read_single: if True, the returned Reader's `read()` method gets one messages at a time
 
         Returns:
             Reader that can read the specified file
         """
-        logger().debug("Reading file headers...")
+        log().debug("Reading file headers...")
         try:
             header = file.read(Reader._HEADER_LENGTH).decode(Reader.HEADER_ENCODING)
             return Reader._READER_HEADERS[header](file, read_single)
         except (KeyError, UnicodeDecodeError):
-            logger().warning(Reader._WARN_NO_HEADER)
+            log().warning(Reader._WARN_NO_HEADER)
             file.seek(0)
             if read_single:
-                logger().error(Reader._ERR_UNSUPPORTED_MODE)
+                log().error(Reader._ERR_UNSUPPORTED_MODE)
             return ReaderV0(file, False)
 
     @typing.final
     def _read_message_length(self) -> int:
         """Returns length of next DataStorage message in file"""
         message_length_byte = self._file.read(self.BYTES_DEFINING_MESSAGE_LENGTH)
         if not message_length_byte:
-            logger().debug(self._DEBUG_FILE_END_REACHED)
+            log().debug(self._DEBUG_FILE_END_REACHED)
             message_length_int = 0
         else:
             message_length_int = struct.unpack(">i", message_length_byte)[0]
         return message_length_int
 
     @typing.final
     def _read_data_storage_message(self, message_length: int = None) -> DataStorage:
@@ -82,15 +82,15 @@
         if message_length is None:
             message = self._file.read()
         elif message_length > 0:
             message = self._file.read(message_length)
         else:
             raise IOError(self._ERR_FILE_CORRUPT_NEGATIVE_LENGTH)
         if message_length and len(message) != message_length:
-            logger().error(self._ERR_FILE_CORRUPT_MISSING_DATA)
+            log().error(self._ERR_FILE_CORRUPT_MISSING_DATA)
         return self._parse_to_data_storage(message) if message else None
 
     @staticmethod
     @typing.final
     def _parse_to_data_storage(message: bytes) -> DataStorage:
         data_storage = DataStorage()
         try:
@@ -103,15 +103,15 @@
 class ReaderV0(Reader):
     """Reader class for deprecated `fame-core<1.4` output without any header"""
 
     _WARN_DEPRECATED = "DeprecationWarning: Please consider updating to `FAME-Core>=1.4` and `fameio>=1.6`"
 
     def __init__(self, file: IO, read_single):
         super().__init__(file, read_single)
-        logger().warning(self._WARN_DEPRECATED)
+        log().warning(self._WARN_DEPRECATED)
 
     def read(self) -> List[DataStorage]:
         result = self._read_data_storage_message()
         return [result] if result else []
 
 
 class ReaderV1(Reader):
@@ -122,9 +122,9 @@
         while True:
             message_length = self._read_message_length()
             if message_length == 0:
                 break
             messages.append(self._read_data_storage_message(message_length))
             if self._read_single:
                 break
-        logger().debug(f"Read {len(messages)} messages from file.")
+        log().debug(f"Read {len(messages)} messages from file.")
         return messages
```

### Comparing `fameio-2.0.0/src/fameio/source/results/yaml_writer.py` & `fameio-2.1.0/src/fameio/source/results/yaml_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 from pathlib import Path
 from typing import Dict
 
 import yaml
 
-from fameio.source.logs import logger
+from fameio.source.logs import log
 
 ERR_WRITE_EXCEPTION = "Failed to save dictionary to YAML file `{}`"
 INFO_DESTINATION = "Saving scenario to file at {}"
 
 
 def data_to_yaml_file(data: Dict, file_path: Path) -> None:
     """
     Save the given data to a YAML file at given path
 
     Args:
         data: to be saved to yaml file
         file_path: at which the file will be created
     """
-    logger().info(INFO_DESTINATION.format(file_path))
+    log().info(INFO_DESTINATION.format(file_path))
     try:
         with open(file_path, "w") as f:
             yaml.dump(data, f, sort_keys=False)
     except Exception as e:
         raise RuntimeError(ERR_WRITE_EXCEPTION.format(file_path)) from e
```

### Comparing `fameio-2.0.0/src/fameio/source/scenario/agent.py` & `fameio-2.1.0/src/fameio/source/scenario/agent.py`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/src/fameio/source/scenario/attribute.py` & `fameio-2.1.0/src/fameio/source/scenario/attribute.py`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/src/fameio/source/scenario/contract.py` & `fameio-2.1.0/src/fameio/source/scenario/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 
-from fameio.source.logs import logger
+from fameio.source.logs import log
 from fameio.source.scenario.attribute import Attribute
 from fameio.source.scenario.exception import get_or_default, get_or_raise, log_and_raise
 from fameio.source.time import FameTime
 from fameio.source.tools import ensure_is_list, keys_to_lower
 
 
 class Contract:
@@ -43,15 +43,15 @@
         first_delivery_time: int,
         expiration_time: Optional[int] = None,
         meta_data: Optional[dict] = None,
     ) -> None:
         """Constructs a new Contract"""
         assert product_name != ""
         if sender_id == receiver_id:
-            logger().warning(self._ERR_SENDER_IS_RECEIVER.format(sender_id))
+            log().warning(self._ERR_SENDER_IS_RECEIVER.format(sender_id))
         if delivery_interval <= 0:
             raise ValueError(self._ERR_INTERVAL_NOT_POSITIVE.format(delivery_interval))
         self._sender_id = sender_id
         self._receiver_id = receiver_id
         self._product_name = product_name
         self._delivery_interval = delivery_interval
         self._first_delivery_time = first_delivery_time
```

### Comparing `fameio-2.0.0/src/fameio/source/scenario/exception.py` & `fameio-2.1.0/src/fameio/source/scenario/exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 from typing import NoReturn, Any, Union
 
-from fameio.source.logs import log_error_and_raise, logger
+from fameio.source.logs import log_error_and_raise, log
 
 _DEFAULT_USED = "Using default value '{}' for missing key '{}'"
 
 
 def log_and_raise(message: str) -> NoReturn:
     """Raises ScenarioException with given `message`"""
     log_error_and_raise(ScenarioException(message))
@@ -29,15 +29,15 @@
 
 
 def get_or_default(dictionary: dict, key: str, default_value) -> Any:
     """Returns value associated with `key` in given `dictionary`, or the given `default_value` if key is missing"""
     if key in dictionary and dictionary[key] is not None:
         return dictionary[key]
     else:
-        logger().debug(_DEFAULT_USED.format(default_value, key))
+        log().debug(_DEFAULT_USED.format(default_value, key))
         return default_value
 
 
 class ScenarioException(Exception):
     """Indicates an error while parsing a scenario or one of its components"""
 
     pass
```

### Comparing `fameio-2.0.0/src/fameio/source/scenario/fameiofactory.py` & `fameio-2.1.0/src/fameio/source/scenario/fameiofactory.py`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/src/fameio/source/scenario/generalproperties.py` & `fameio-2.1.0/src/fameio/source/scenario/generalproperties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
-from fameio.source.logs import logger
+from fameio.source.logs import log
 from fameio.source.scenario.exception import get_or_default, get_or_raise
 from fameio.source.time import FameTime
 from fameio.source.tools import keys_to_lower
 
 
 class GeneralProperties:
     """Hosts general properties of a scenario"""
@@ -30,15 +30,15 @@
         simulation_start_time: int,
         simulation_stop_time: int,
         simulation_random_seed: int,
         output_interval: int,
         output_process: int,
     ) -> None:
         if simulation_stop_time < simulation_start_time:
-            logger().warning(GeneralProperties._SIMULATION_DURATION)
+            log().warning(GeneralProperties._SIMULATION_DURATION)
         self._run_id = run_id
         self._simulation_start_time = simulation_start_time
         self._simulation_stop_time = simulation_stop_time
         self._simulation_random_seed = simulation_random_seed
         self._output_interval = output_interval
         self._output_process = output_process
```

### Comparing `fameio-2.0.0/src/fameio/source/scenario/scenario.py` & `fameio-2.1.0/src/fameio/source/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/src/fameio/source/schema/agenttype.py` & `fameio-2.1.0/src/fameio/source/schema/agenttype.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from typing import Dict, List, Any
 
-from fameio.source.logs import log_error_and_raise, logger
+from fameio.source.logs import log_error_and_raise, log
 from fameio.source.schema.exception import SchemaException
 from fameio.source.schema.attribute import AttributeSpecs
 from fameio.source.tools import keys_to_lower
 
 
 class AgentType:
     """Schema definitions for an Agent type"""
@@ -59,34 +59,34 @@
 
         definition = keys_to_lower(definitions)
         if AgentType._KEY_ATTRIBUTES in definition:
             for attribute_name, attribute_details in definition[AgentType._KEY_ATTRIBUTES].items():
                 full_name = name + "." + attribute_name
                 agent_type._attributes[attribute_name] = AttributeSpecs(full_name, attribute_details)
         else:
-            logger().info(AgentType._NO_ATTRIBUTES.format(name))
+            log().info(AgentType._NO_ATTRIBUTES.format(name))
 
         if AgentType._KEY_PRODUCTS in definition and definition[AgentType._KEY_PRODUCTS]:
             agent_type._products.update(AgentType._read_products(definition[AgentType._KEY_PRODUCTS], name))
         else:
-            logger().info(AgentType._NO_PRODUCTS.format(name))
+            log().info(AgentType._NO_PRODUCTS.format(name))
 
         if AgentType._KEY_OUTPUTS in definition:
             outputs_to_add = definition[AgentType._KEY_OUTPUTS]
             if outputs_to_add:
                 agent_type._outputs.update(outputs_to_add)
         else:
-            logger().debug(AgentType._NO_OUTPUTS.format(name))
+            log().debug(AgentType._NO_OUTPUTS.format(name))
 
         if AgentType._KEY_METADATA in definition:
             metadata_to_add = definition[AgentType._KEY_METADATA]
             if metadata_to_add:
                 agent_type._metadata.update(metadata_to_add)
         else:
-            logger().debug(AgentType._NO_METADATA.format(name))
+            log().debug(AgentType._NO_METADATA.format(name))
 
         return agent_type
 
     @staticmethod
     def _read_products(products: Any, agent_type: str) -> Dict[str, Any]:
         """Returns a dict obtained from given `products` defined for `agent_type`"""
         product_names = None
```

### Comparing `fameio-2.0.0/src/fameio/source/schema/attribute.py` & `fameio-2.1.0/src/fameio/source/schema/attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import typing
 from enum import Enum, auto
 from typing import Any, Dict
 
-from fameio.source.logs import logger
+from fameio.source.logs import log
 from fameio.source.schema.exception import SchemaException
 from fameio.source.time import FameTime
 from fameio.source.tools import keys_to_lower
 
 
 class AttributeType(Enum):
     """Specifies known types that Attributes can take"""
@@ -66,26 +66,26 @@
         self._full_name = name
         definition = keys_to_lower(definition)
 
         if AttributeSpecs._KEY_MANDATORY in definition:
             self._is_mandatory = definition[AttributeSpecs._KEY_MANDATORY]
         else:
             self._is_mandatory = True
-            logger().warning(AttributeSpecs._MISSING_SPEC_DEFAULT.format(AttributeSpecs._KEY_MANDATORY, name, True))
+            log().warning(AttributeSpecs._MISSING_SPEC_DEFAULT.format(AttributeSpecs._KEY_MANDATORY, name, True))
 
         if AttributeSpecs._KEY_LIST in definition:
             self._is_list = definition[AttributeSpecs._KEY_LIST]
         else:
             self._is_list = False
-            logger().warning(AttributeSpecs._MISSING_SPEC_DEFAULT.format(AttributeSpecs._KEY_LIST, name, False))
+            log().warning(AttributeSpecs._MISSING_SPEC_DEFAULT.format(AttributeSpecs._KEY_LIST, name, False))
 
         if AttributeSpecs._KEY_TYPE in definition:
             self._attr_type = AttributeSpecs._get_type_for_name(definition[AttributeSpecs._KEY_TYPE])
         else:
-            logger().error(AttributeSpecs._MISSING_TYPE.format(name))
+            log().error(AttributeSpecs._MISSING_TYPE.format(name))
             raise SchemaException(AttributeSpecs._MISSING_TYPE.format(name))
 
         if self._attr_type == AttributeType.TIME_SERIES and self._is_list:
             raise SchemaException(AttributeSpecs._LIST_DISALLOWED.format(name))
 
         self._values = []
         if AttributeSpecs._KEY_VALUES in definition:
```

### Comparing `fameio-2.0.0/src/fameio/source/schema/schema.py` & `fameio-2.1.0/src/fameio/source/schema/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,57 @@
-# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+# SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import ast
-from typing import Dict
+from typing import Dict, Optional
 
-from fameio.source.logs import log_error_and_raise
+from fameio.source.logs import log_error_and_raise, log
 from fameio.source.schema.agenttype import AgentType
 from fameio.source.schema.exception import SchemaException
+from fameio.source.schema.java_packages import JavaPackages
 from fameio.source.tools import keys_to_lower
 
 
 class Schema:
     """Definition of a schema"""
 
-    _AGENT_TYPES_MISSING = "Required keyword `AgentTypes` missing in Schema."
-    _AGENT_TYPES_EMPTY = "`AgentTypes` must not be empty - at least one type of agent is required."
+    _ERR_AGENT_TYPES_MISSING = "Required keyword `AgentTypes` missing in Schema."
+    _ERR_AGENT_TYPES_EMPTY = "`AgentTypes` must not be empty - at least one type of agent is required."
+    _WARN_MISSING_PACKAGES = "No `JavaPackages` defined Schema. Future versions of fameio will require it."
+
     _KEY_AGENT_TYPE = "AgentTypes".lower()
+    _KEY_PACKAGES = "JavaPackages".lower()
 
     def __init__(self, definitions: dict):
         self._original_input_dict = definitions
         self._agent_types = {}
+        self._packages: Optional[JavaPackages] = None
 
     @classmethod
     def from_dict(cls, definitions: dict) -> Schema:
         """Load given dictionary `definitions` into a new Schema"""
         definitions = keys_to_lower(definitions)
         if Schema._KEY_AGENT_TYPE not in definitions:
-            log_error_and_raise(SchemaException(Schema._AGENT_TYPES_MISSING))
+            log_error_and_raise(SchemaException(Schema._ERR_AGENT_TYPES_MISSING))
         schema = cls(definitions)
         agent_types = definitions[Schema._KEY_AGENT_TYPE]
         if len(agent_types) == 0:
-            log_error_and_raise(SchemaException(Schema._AGENT_TYPES_EMPTY))
+            log_error_and_raise(SchemaException(Schema._ERR_AGENT_TYPES_EMPTY))
 
         for agent_type_name, agent_definition in agent_types.items():
             agent_type = AgentType.from_dict(agent_type_name, agent_definition)
             schema._agent_types[agent_type_name] = agent_type
+
+        if Schema._KEY_PACKAGES in definitions:
+            schema._packages = JavaPackages.from_dict(definitions[Schema._KEY_PACKAGES])
+        else:
+            log().warning(Schema._WARN_MISSING_PACKAGES)
+            schema._packages = JavaPackages()
         return schema
 
     @classmethod
     def from_string(cls, definitions: str) -> Schema:
         """Load given string `definitions` into a new Schema"""
         return cls.from_dict(ast.literal_eval(definitions))
 
@@ -52,7 +63,12 @@
         """Returns a string representation of the Schema of which the class can be rebuilt"""
         return repr(self.to_dict())
 
     @property
     def agent_types(self) -> Dict[str, AgentType]:
         """Returns all the agent types by their name"""
         return self._agent_types
+
+    @property
+    def packages(self) -> JavaPackages:
+        """Returns JavaPackages, i.e. names where model classes are defined in"""
+        return self._packages
```

### Comparing `fameio-2.0.0/src/fameio/source/series.py` & `fameio-2.1.0/src/fameio/source/series.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 import os
 from enum import Enum, auto
 from pathlib import Path
 from typing import Dict, Union, Tuple, Any, List
 
 import pandas as pd
 from fameprotobuf.InputFile_pb2 import InputData
+from google.protobuf.internal.wire_format import INT64_MIN, INT64_MAX
 
 from fameio.source import PathResolver
-from fameio.source.logs import log_error_and_raise, logger
+from fameio.source.logs import log_error_and_raise, log
 from fameio.source.time import ConversionException, FameTime
 from fameio.source.tools import clean_up_file_name
 
 
 class TimeSeriesException(Exception):
     """Indicates that an error occurred during management of time series"""
 
@@ -110,15 +111,16 @@
         return value
 
     @staticmethod
     def _create_timeseries_from_value(value: Union[int, float]) -> Tuple[str, pd.DataFrame]:
         """Returns name and dataframe for a new static timeseries created from the given `value`"""
         if math.isnan(value):
             log_error_and_raise(TimeSeriesException(TimeSeriesManager._ERR_NAN_VALUE))
-        return TimeSeriesManager._CONSTANT_IDENTIFIER.format(value), pd.DataFrame({0: [0], 1: [value]})
+        data = pd.DataFrame({0: [INT64_MIN, INT64_MAX], 1: [value, value]})
+        return TimeSeriesManager._CONSTANT_IDENTIFIER.format(value), data
 
     def get_series_id_by_identifier(self, identifier: Union[str, int, float]) -> int:
         """
         Returns id for a previously stored time series by given `identifier`
 
         Args:
             identifier: to get the unique ID for
@@ -132,15 +134,15 @@
         if not self._time_series_is_registered(identifier):
             log_error_and_raise(TimeSeriesException(self._ERR_UNREGISTERED_SERIES.format(identifier)))
         return self._series_by_id.get(identifier)[Entry.ID]
 
     def get_all_series(self) -> List[Tuple[int, str, pd.DataFrame]]:
         """Returns iterator over id, name and dataframe of all stored series"""
         if len(self._series_by_id) == 0:
-            logger().warning(self._WARN_NO_DATA)
+            log().warning(self._WARN_NO_DATA)
         return [(v[Entry.ID], v[Entry.NAME], v[Entry.DATA]) for v in self._series_by_id.values()]
 
     def reconstruct_time_series(self, timeseries: List[InputData.TimeSeriesDao]) -> None:
         """Reconstructs and stores time series from given list of `timeseries_dao`"""
         for one_series in timeseries:
             self._id_count += 1
             reconstructed = {Entry.ID: one_series.seriesId}
```

### Comparing `fameio-2.0.0/src/fameio/source/time.py` & `fameio-2.1.0/src/fameio/source/time.py`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/src/fameio/source/tools.py` & `fameio-2.1.0/src/fameio/source/tools.py`

 * *Files identical despite different names*

### Comparing `fameio-2.0.0/src/fameio/source/validator.py` & `fameio-2.1.0/src/fameio/source/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import math
 from collections import Counter
 from typing import Any, Dict, List
 
 from fameio.source import PathResolver
-from fameio.source.logs import log_error_and_raise, logger
+from fameio.source.logs import log_error_and_raise, log
 from fameio.source.scenario import Agent, Attribute, Contract, Scenario
 from fameio.source.schema.agenttype import AgentType
 from fameio.source.schema.attribute import AttributeSpecs, AttributeType
 from fameio.source.schema.schema import Schema
 from fameio.source.series import TimeSeriesManager, TimeSeriesException
 from fameio.source.time import FameTime
 
@@ -121,17 +121,17 @@
                 if specification.is_mandatory:
                     if not specification.has_default_value:
                         log_error_and_raise(
                             ValidationException(SchemaValidator._ATTRIBUTE_MISSING.format(specification.full_name))
                         )
                 else:
                     if specification.has_default_value:
-                        logger().warning(SchemaValidator._DEFAULT_IGNORED.format(specification.full_name))
+                        log().warning(SchemaValidator._DEFAULT_IGNORED.format(specification.full_name))
                     else:
-                        logger().info(SchemaValidator._OPTIONAL_MISSING.format(specification.full_name))
+                        log().info(SchemaValidator._OPTIONAL_MISSING.format(specification.full_name))
             if name in attributes and specification.has_nested_attributes:
                 attribute = attributes[name]
                 if specification.is_list:
                     for entry in attribute.nested_list:
                         SchemaValidator._ensure_mandatory_present(entry, specification.nested_attributes)
                 else:
                     SchemaValidator._ensure_mandatory_present(attribute.nested, specification.nested_attributes)
@@ -175,15 +175,15 @@
     @staticmethod
     def _is_compatible(specification: AttributeSpecs, value_or_values: Any) -> bool:
         """Returns True if given `value_or_values` is compatible to specified `attribute_type` and `should_be_list`"""
         is_list = isinstance(value_or_values, list)
         attribute_type = specification.attr_type
         if specification.is_list:
             if not is_list:
-                logger().warning(SchemaValidator._IS_NO_LIST.format(specification.full_name, value_or_values))
+                log().warning(SchemaValidator._IS_NO_LIST.format(specification.full_name, value_or_values))
                 return SchemaValidator._is_compatible_value(attribute_type, value_or_values)
             for value in value_or_values:
                 if not SchemaValidator._is_compatible_value(attribute_type, value):
                     return False
             return True
         else:
             return (not is_list) and SchemaValidator._is_compatible_value(attribute_type, value_or_values)
@@ -276,8 +276,8 @@
         senders = [contract.sender_id for contract in scenario.contracts]
         receivers = [contract.receiver_id for contract in scenario.contracts]
         active_agents = set(senders + receivers)
         inactive_agents = {agent.id: agent.type_name for agent in scenario.agents if agent.id not in active_agents}
 
         if inactive_agents:
             for agent_id, agent_name in inactive_agents.items():
-                logger().warning(SchemaValidator._MISSING_CONTRACTS_FOR_AGENTS.format(agent_id, agent_name))
+                log().warning(SchemaValidator._MISSING_CONTRACTS_FOR_AGENTS.format(agent_id, agent_name))
```

### Comparing `fameio-2.0.0/src/fameio/source/writer.py` & `fameio-2.1.0/src/fameio/source/writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-# SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+# SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 from pathlib import Path
 from typing import Any, Dict, List, Union
 
 from fameprotobuf.DataStorage_pb2 import DataStorage
 from fameprotobuf.InputFile_pb2 import InputData
 from fameprotobuf.Field_pb2 import NestedField
 from fameprotobuf.Contract_pb2 import ProtoContract
+from fameprotobuf.Model_pb2 import ModelData
 
-from fameio.source.logs import log_error_and_raise, logger
+from fameio.source.logs import log_error_and_raise, log
 from fameio.source.results.reader import Reader
 from fameio.source.scenario import (
     Agent,
     Attribute,
     Contract,
     GeneralProperties,
     Scenario,
 )
 from fameio.source.schema import Schema
 from fameio.source.schema.attribute import AttributeSpecs, AttributeType
+from fameio.source.schema.java_packages import JavaPackages
 from fameio.source.series import TimeSeriesManager
 from fameio.source.time import FameTime
 from fameio.source.tools import ensure_is_list
 
 
 class ProtoWriterException(Exception):
     """Indicates an error during writing of protobuf file"""
@@ -55,40 +57,41 @@
     def write_validated_scenario(self, scenario: Scenario) -> None:
         """Writes given validated Scenario to file"""
         pb_data_storage = self._create_protobuf_from_scenario(scenario)
         self._write_protobuf_to_disk(pb_data_storage)
 
     def _create_protobuf_from_scenario(self, scenario: Scenario) -> DataStorage:
         """Returns given `scenario` written to new DataStorage protobuf"""
-        logger().info("Converting scenario to protobuf.")
+        log().info("Converting scenario to protobuf.")
         pb_data_storage = DataStorage()
         pb_input = pb_data_storage.input
 
         self._set_general_properties(pb_input, scenario.general_properties)
         self._add_agents(pb_input, scenario.agents, scenario.schema)
         self._add_contracts(pb_input, scenario.contracts)
         self._set_time_series(pb_input)
         self._set_schema(pb_input, scenario.schema)
 
+        self._set_java_package_names(pb_data_storage.model, scenario.schema.packages)
         return pb_data_storage
 
     @staticmethod
     def _set_general_properties(pb_input: InputData, general_properties: GeneralProperties) -> None:
         """Saves a scenario's general properties to specified protobuf `pb_input` container"""
-        logger().info("Adding General Properties")
+        log().info("Adding General Properties")
         pb_input.runId = general_properties.run_id
         pb_input.simulation.startTime = general_properties.simulation_start_time
         pb_input.simulation.stopTime = general_properties.simulation_stop_time
         pb_input.simulation.randomSeed = general_properties.simulation_random_seed
         pb_input.output.interval = general_properties.output_interval
         pb_input.output.process = general_properties.output_process
 
     def _add_agents(self, pb_input: InputData, agents: List[Agent], schema: Schema) -> None:
         """Triggers setting of `agents` to `pb_input`"""
-        logger().info("Adding Agents")
+        log().info("Adding Agents")
         for agent in agents:
             pb_agent = self._set_agent(pb_input.agent.add(), agent)
             attribute_specs = schema.agent_types[agent.type_name].attributes
             self._set_attributes(pb_agent, agent.attributes, attribute_specs)
             pb_agent.metadata = repr(agent.meta_data)
 
     @staticmethod
@@ -121,15 +124,15 @@
             else:
                 self._set_attribute(pb_field, attribute.value, attribute_type)
         for name in values_not_set:
             attribute_specs = specs[name]
             if attribute_specs.is_mandatory:
                 pb_field = self._add_field(pb_parent, name)
                 self._set_attribute(pb_field, attribute_specs.default_value, attribute_specs.attr_type)
-                logger().info(self._USING_DEFAULT.format(name))
+                log().info(self._USING_DEFAULT.format(name))
 
     @staticmethod
     def _add_field(pb_parent: Union[InputData.AgentDao, NestedField], name: str) -> NestedField:
         """Returns new field with given `name` that is added to given `pb_parent`"""
         pb_field = pb_parent.field.add()
         pb_field.fieldName = name
         return pb_field
@@ -150,15 +153,15 @@
             pb_field.seriesId = self._time_series_manager.get_series_id_by_identifier(value)
         else:
             log_error_and_raise(ProtoWriterException(self._TYPE_NOT_IMPLEMENTED.format(attribute_type)))
 
     @staticmethod
     def _add_contracts(pb_input: InputData, contracts: List[Contract]) -> None:
         """Triggers setting of `contracts` to `pb_input`"""
-        logger().info("Adding Contracts")
+        log().info("Adding Contracts")
         for contract in contracts:
             pb_contract = ProtoWriter._set_contract(pb_input.contract.add(), contract)
             ProtoWriter._set_contract_attributes(pb_contract, contract.attributes)
             pb_contract.metadata = repr(contract.meta_data)
 
     @staticmethod
     def _set_contract(pb_contract: ProtoContract, contract: Contract) -> ProtoContract:
@@ -174,15 +177,15 @@
 
     @staticmethod
     def _set_contract_attributes(
         pb_parent: Union[ProtoContract, NestedField], attributes: Dict[str, Attribute]
     ) -> None:
         """Assign (nested) Attributes to given protobuf container `pb_parent`"""
         for name, attribute in attributes.items():
-            logger().debug("Assigning contract attribute `{}`.".format(name))
+            log().debug("Assigning contract attribute `{}`.".format(name))
             pb_field = ProtoWriter._add_field(pb_parent, name)
 
             if attribute.has_value:
                 value = attribute.value
                 if isinstance(value, int):
                     pb_field.intValue.extend([value])
                 elif isinstance(value, float):
@@ -192,15 +195,15 @@
                 else:
                     log_error_and_raise(ProtoWriterException(ProtoWriter._CONTRACT_UNSUPPORTED.format(str(attribute))))
             elif attribute.has_nested:
                 ProtoWriter._set_contract_attributes(pb_field, attribute.nested)
 
     def _set_time_series(self, pb_input: InputData) -> None:
         """Adds all time series from TimeSeriesManager to given `pb_input`"""
-        logger().info("Adding TimeSeries")
+        log().info("Adding TimeSeries")
         for unique_id, identifier, data in self._time_series_manager.get_all_series():
             pb_series = pb_input.timeSeries.add()
             pb_series.seriesId = unique_id
             pb_series.seriesName = identifier
             ProtoWriter._add_rows_to_series(pb_series, data)
 
     @staticmethod
@@ -209,22 +212,30 @@
             row = series.row.add()
             row.timeStep = int(key)
             row.value = value
 
     @staticmethod
     def _set_schema(pb_input: InputData, schema: Schema) -> None:
         """Sets the given `schema` `pb_input`"""
-        logger().info("Adding Schema")
+        log().info("Adding Schema")
         pb_input.schema = schema.to_string()
 
+    @staticmethod
+    def _set_java_package_names(pb_model: ModelData, java_packages: JavaPackages) -> None:
+        """Adds given JavaPackages names to given ModelData section"""
+        pb_packages = pb_model.packages
+        pb_packages.agent.extend(java_packages.agents)
+        pb_packages.dataItem.extend(java_packages.data_items)
+        pb_packages.portable.extend(java_packages.portables)
+
     def _write_protobuf_to_disk(self, pb_data_storage: DataStorage) -> None:
         """Writes given `protobuf_input_data` to disk"""
-        logger().info(self._INFO_WRITING.format(self.file_path))
+        log().info(self._INFO_WRITING.format(self.file_path))
         try:
             with open(self.file_path, "wb") as file:
                 serialised_data_storage = pb_data_storage.SerializeToString()
                 file.write(self._FAME_PROTOBUF_STREAM_HEADER.encode(Reader.HEADER_ENCODING))
                 file.write(len(serialised_data_storage).to_bytes(Reader.BYTES_DEFINING_MESSAGE_LENGTH, byteorder="big"))
                 file.write(serialised_data_storage)
         except OSError as e:
             log_error_and_raise(ProtoWriterException(ProtoWriter._NO_FILE_SPECIFIED.format(self.file_path), e))
-        logger().info(self._INFO_WRITING_COMPLETED.format(self.file_path))
+        log().info(self._INFO_WRITING_COMPLETED.format(self.file_path))
```

### Comparing `fameio-2.0.0/PKG-INFO` & `fameio-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fameio
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python scripts for operation of FAME models
 Home-page: https://gitlab.com/fame-framework/wiki/-/wikis/home
 License: Apache-2.0
 Keywords: FAME,fameio,agent-based modelling,energy systems
 Author: Felix Nitsch
 Author-email: fame@dlr.de
 Maintainer: Felix Nitsch
@@ -17,21 +17,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: fameprotobuf (>=1.4.0,<2.0.0)
+Requires-Dist: fameprotobuf (>=1.5.0,<2.0.0)
 Requires-Dist: pandas (>=1.0,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://gitlab.com/fame-framework/fame-io/
 Description-Content-Type: text/markdown
 
-<!-- SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
+<!-- SPDX-FileCopyrightText: 2024 German Aerospace Center <fame@dlr.de>
 
 SPDX-License-Identifier: Apache-2.0 -->
 [![PyPI version](https://badge.fury.io/py/fameio.svg)](https://badge.fury.io/py/fameio)
 [![JOSS](https://joss.theoj.org/papers/10.21105/joss.04958/status.svg)](https://doi.org/10.21105/joss.04958)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.4314337.svg)](https://doi.org/10.5281/zenodo.4314337)
 [![PyPI license](https://img.shields.io/pypi/l/fameio.svg)](https://badge.fury.io/py/fameio)
 [![pipeline status](https://gitlab.com/fame-framework/fame-io/badges/main/pipeline.svg)](https://gitlab.com/fame-framework/fame-io/commits/main)
@@ -125,41 +125,53 @@
 ```
 
 ### Scenario YAML
 The "scenario.yaml" file contains all configuration options for a FAME-based simulation.
 It consists of the sections `Schema`, `GeneralProperties`, `Agents` and `Contracts`, all of them described below.
 
 #### Schema
-The Schema is used to validate the inputs of the "scenario.yaml".
-Since the Schema should be valid across multiple scenarios, it is recommended to defined it in a separate file and include the file here.
+The Schema describes a model's components such as its types of agents, their inputs, what data they exchange, etc. 
+It is also used to validate the model inputs provided in the `scenario.yaml`. 
+Since the Schema is valid until the model itself is changed, it is recommended to defined it in a separate file and include the file here.
 
 Currently, the schema specifies:
 * which type of Agents can be created
 * what type of input attributes an Agent uses
-* what type of Products an Agent can send in Contracts.
+* what type of Products an Agent can send in Contracts, and
+* the names of the Java packages for the classes corresponding to Agents, DataItems and Portables. 
 
-The Schema consists of the sections `Header` and `AgentTypes`.
+The Schema consists of the sections `JavaPackages` and `AgentTypes`.
 
-##### Header
-Scientific applications often evolve, and so do their required input parameters.
-Therefore, the header specifies information what FAME-based application the schema is corresponding to.
-In this way a schema.yaml is tied to a specific version an application, ensuring a match between the inputs required by
-the application, and those provided by the files created with FAME-Io.
-
-```yaml
-Header:
-  Project: MyProjectName
-  RepoUrl: https://mygithosting.com/myProject
-  CommitHash: abc123
+##### JavaPackages
+This section defines the name of the Java packages in which the model code is located.
+A similar data set was formerly specified in the `fameSetup.yaml`, but is now specified in the schema.
+Each of the three sections `Agents`, `DataItems`, and `Portables` contain a list of fully qualified java package names of your model's classes.
+Package names can occur in multiple lists and may overlap.
+It is not necessary (but possible) to specify the nearest enclosing package for each Agent, DataItem or Portable.
+Specifying any super-package will also work.
+Also, package names occur on multiple lists for Agent, DataItem or Portable.
+
+For example, for a project with all its
+* Agent-derived java classes located in packages below the package named "agents",
+* DataItem implementation classes in a subpackage named "msg",
+* Portable implementation classes in a subpackages named "portableItems" and "otherPortables", 
+
+the corresponding section in the schema would look like this:
+
+```yaml
+JavaPackages:
+  Agents:
+    - "agents"
+  DataItems:
+    - "msg"
+  Portables:
+    - "portableItems"
+    - "otherPortables"
 ```
 
-* `Project` name of your project / FAME-based application
-* `RepoUrl` URL of your project
-* `CommitHash` hash of the commit / version of your project
-
 ##### AgentTypes
 Here, each type of agent that can be created in your FAME-based application is listed, its attributes and its available Products for Contracts.
 The structure of this section
 
 ```yaml
 AgentTypes:
   MyAgentType:
@@ -581,25 +593,25 @@
 An individual file for each type of Agent is created in a folder named after the protobuf input file.
 Call structure:
 
     convertFameResults -f <./path/to/protobuf_file.pb>
 
 You may also specify any of the following arguments:
 
-| Command                                     | Action                                                                                                                                                                                                                                              |
-|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `-l` or `--log` <option>                    | Sets the logging level. Default is `info`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.                                                                                                                                     |
-| `-lf` or `--logfile` <file>                 | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                                                                                                                                          |
-| `-a` or `--agents` <list-of-agents>         | If specified, only a subset of agents is extracted from the protobuf file. Default is to extract all agents.                                                                                                                                        |
-| `-o` or `--output`                          | Sets the path to where the generated output files are written to. If not specified, the folder's name is derived from the input file's name. Folder will be created if it does not exist.                                                           |
-| `-se` or `--single-export`                  | Enables export of individual agents to individual files, when present. If not present (the default) one file per `AgentType` is created.                                                                                                            |
-| `-m` or `--memory-saving`                   | When specified, reduces memory usage profile at the cost of runtime. Use only when necessary.                                                                                                                                                       |
-| `-cc` or `--complex-column` <option>        | Defines how to deal with complex indexed output columns (if any). `IGNORE` ignores complex columns. `MERGE` squashes all data from complex columns in one big string entry. `SPLIT` creates a separate file for each complex indexed output column. |
-| `-t` or `--time` <option>                   | Option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}`                                                                                                                                           |
-| `--input-recovery` or `--no-input-recovery` | If True, all input data are recovered as well as the outputs (default=False).                                                                                                                                                                       |
+| Command                                     | Action                                                                                                                                                                                    |
+|---------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `-l` or `--log` <option>                    | Sets the logging level. Default is `WARNING`. Options are `DEBUG`, `INFO`, `WARNING`, `ERROR`, `CRITICAL`.                                                                                |
+| `-lf` or `--logfile` <file>                 | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.                                                                                |
+| `-a` or `--agents` <list-of-agents>         | If specified, only a subset of agents is extracted from the protobuf file. Default is to extract all agents.                                                                              |
+| `-o` or `--output`                          | Sets the path to where the generated output files are written to. If not specified, the folder's name is derived from the input file's name. Folder will be created if it does not exist. |
+| `-se` or `--single-export`                  | Enables export of individual agents to individual files, when present. If not present (the default) one file per `AgentType` is created.                                                  |
+| `-m` or `--memory-saving`                   | When specified, reduces memory usage profile at the cost of runtime. Use only when necessary.                                                                                             |
+| `-cc` or `--complex-column` <option>        | Defines how to deal with complex indexed output columns (if any). `IGNORE` ignores complex columns. `SPLIT` creates a separate file for each complex indexed output column.               |
+| `-t` or `--time` <option>                   | Option to define conversion of time steps to given format (default=`UTC`) by `-t/--time {UTC, INT, FAME}`                                                                                 |
+| `--input-recovery` or `--no-input-recovery` | If True, all input data are recovered as well as the outputs (default=False).                                                                                                             |
 
 Additionally, you may merge TimeSteps of a certain range of steps in the output files to
 i) associate multiple time steps with a common logical time in your simulation
 ii) reduce number of lines in output files
 
 For this, add the option `merge-times` and specify the arguments as follows:
```

