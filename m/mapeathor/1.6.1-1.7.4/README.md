# Comparing `tmp/mapeathor-1.6.1.tar.gz` & `tmp/mapeathor-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "mapeathor-1.7.4.tar", last modified: Sat May 11 09:55:35 2024, max compression
```

## Comparing `mapeathor-1.6.1.tar` & `mapeathor-1.7.4.tar`

### file list

```diff
@@ -1,109 +1,82 @@
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 mapeathor-1.6.1/Dockerfile
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 mapeathor-1.6.1/MANIFEST.in
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mapeathor-1.6.1/docker-compose.yml
--rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 mapeathor-1.6.1/exec
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mapeathor-1.6.1/requirements.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 mapeathor-1.6.1/setup.cfg
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 mapeathor-1.6.1/setup.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 mapeathor-1.6.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0   102019 2020-02-02 00:00:00.000000 mapeathor-1.6.1/imgs/Square_logo_mapeathor.png
--rw-r--r--   0        0        0   118372 2020-02-02 00:00:00.000000 mapeathor-1.6.1/imgs/general_schema.png
--rw-r--r--   0        0        0    43270 2020-02-02 00:00:00.000000 mapeathor-1.6.1/imgs/logo.png
--rw-r--r--   0        0        0    28475 2020-02-02 00:00:00.000000 mapeathor-1.6.1/imgs/sheet_base-prefix.png
--rw-r--r--   0        0        0    29110 2020-02-02 00:00:00.000000 mapeathor-1.6.1/imgs/sheet_function.png
--rw-r--r--   0        0        0    78234 2020-02-02 00:00:00.000000 mapeathor-1.6.1/imgs/sheet_pom.png
--rw-r--r--   0        0        0    27419 2020-02-02 00:00:00.000000 mapeathor-1.6.1/imgs/sheet_prefix.png
--rw-r--r--   0        0        0    70515 2020-02-02 00:00:00.000000 mapeathor-1.6.1/imgs/sheet_source.png
--rw-r--r--   0        0        0    34589 2020-02-02 00:00:00.000000 mapeathor-1.6.1/imgs/sheet_subject.png
--rw-r--r--   0        0        0   382544 2020-02-02 00:00:00.000000 mapeathor-1.6.1/imgs/sheets.png
--rw-r--r--   0        0        0   142682 2020-02-02 00:00:00.000000 mapeathor-1.6.1/imgs/workflow.png
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/.gitignore
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/_version.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/api.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/datatypes.json
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/global_config.py
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/mapping_generator.py
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/mapping_writer.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/source.py
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/utils.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/r2rml/Base.tmpl
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/r2rml/Function.tmpl
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/r2rml/Join.tmpl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/r2rml/POM.tmpl
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/r2rml/Prefix.tmpl
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/r2rml/Source.tmpl
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/r2rml/SourceQuery.tmpl
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/r2rml/Subject.tmpl
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/r2rml/TriplesMap.tmpl
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/r2rml/config.json
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/r2rml/structure.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/Base.tmpl
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/Function.tmpl
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/FunctionMap.tmpl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/FunctionPOM.tmpl
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/FunctionSource.tmpl
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/Join.tmpl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/POM.tmpl
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/Prefix.tmpl
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/Source.tmpl
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/SourceQuery.tmpl
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/Subject.tmpl
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/TriplesMap.tmpl
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/config.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/rmlMapping.json
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/rml/structure.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/yarrrml/Base.tmpl
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/yarrrml/Function.tmpl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/yarrrml/Join.tmpl
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/yarrrml/POM.tmpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/yarrrml/Prefix.tmpl
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/yarrrml/Source.tmpl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/yarrrml/SourceQuery.tmpl
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/yarrrml/Subject.tmpl
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/yarrrml/TriplesMap.tmpl
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/yarrrml/config.json
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 mapeathor-1.6.1/src/mapeathor/templates/yarrrml/structure.json
--rw-r--r--   0        0        0    16081 2020-02-02 00:00:00.000000 mapeathor-1.6.1/tutorial-kgc22/empty_template.xlsx
--rw-r--r--   0        0        0   352703 2020-02-02 00:00:00.000000 mapeathor-1.6.1/tutorial-kgc22/gtfs.jpeg
--rw-r--r--   0        0        0    18058 2020-02-02 00:00:00.000000 mapeathor-1.6.1/tutorial-kgc22/stop-stoptimes.xlsx
--rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 mapeathor-1.6.1/tutorial-kgc22/mappings/stop-stoptimes.rml.ttl
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 mapeathor-1.6.1/tutorial-kgc22/mappings/stop-stoptimes.yml
--rw-r--r--   0        0        0    14931 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/budget/input/InputBudget.xlsx
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/budget/mappings/OutputBudget.r2rml.ttl
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/budget/mappings/OutputBudget.rml.ttl
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/budget/mappings/OutputBudget.yml
--rw-r--r--   0        0        0    16378 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/financialPublicDebt/input/InputPublicDebt.xlsx
--rw-r--r--   0        0        0    24089 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/financialPublicDebt/mappings/mappings-deuda-rml.ttl
--rw-r--r--   0        0        0    15830 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/grants/input/InputSubvenciones.xlsx
--rw-r--r--   0        0        0    19098 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/grants/mappings/OutputSubvenciones-rml.ttl
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/grants/mappings/OutputSubvenciones.yml
--rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/noisePollution/input/InputStations.xlsx
--rw-r--r--   0        0        0     6623 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/noisePollution/mappings/OutputStations.r2rml.ttl
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/noisePollution/mappings/OutputStations.rml.ttl
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/noisePollution/mappings/OutputStations.yml
--rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/publicBus/input/InputBusOperator.xlsx
--rw-r--r--   0        0        0    16978 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/publicBus/input/InputBusRoute.xlsx
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/publicBus/mappings/OutputBusOperator.r2rml.ttl
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/publicBus/mappings/OutputBusOperator.rml.ttl
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/publicBus/mappings/OutputBusOperator.yml
--rw-r--r--   0        0        0     9806 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/publicBus/mappings/OutputBusRoute.r2rml.ttl
--rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/publicBus/mappings/OutputBusRoute.rml.ttl
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/publicBus/mappings/OutputBusRoute.yml
--rw-r--r--   0        0        0    33646 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/publicEmpolyment/input/mapeathor-empleo.xlsx
--rw-r--r--   0        0        0    13440 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/publicEmpolyment/mappings/empleo-rml.rml
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/publicEmpolyment/mappings/empleo-yml.yml
--rw-r--r--   0        0        0    16307 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/traffic/input/InputEquipment.xlsx
--rw-r--r--   0        0        0    15177 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/traffic/input/InputIncidences.xlsx
--rw-r--r--   0        0        0     6959 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/traffic/mappings/OutputEquipment.r2rml.ttl
--rw-r--r--   0        0        0     7115 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/traffic/mappings/OutputEquipment.rml.ttl
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/traffic/mappings/OutputEquipment.yml
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/traffic/mappings/OutputIncidences.r2rml.ttl
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/traffic/mappings/OutputIncidences.rml.ttl
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 mapeathor-1.6.1/use-cases/traffic/mappings/OutputIncidences.yml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 mapeathor-1.6.1/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 mapeathor-1.6.1/LICENSE
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 mapeathor-1.6.1/README.md
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 mapeathor-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 mapeathor-1.6.1/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.403584 mapeathor-1.7.4/
+-rw-r--r--   0 runner     (501) staff       (20)    11349 2024-05-11 09:55:29.000000 mapeathor-1.7.4/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-11 09:55:29.000000 mapeathor-1.7.4/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    18422 2024-05-11 09:55:35.403424 mapeathor-1.7.4/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3535 2024-05-11 09:55:29.000000 mapeathor-1.7.4/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1828 2024-05-11 09:55:29.000000 mapeathor-1.7.4/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      125 2024-05-11 09:55:35.404396 mapeathor-1.7.4/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1507 2024-05-11 09:55:29.000000 mapeathor-1.7.4/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.365467 mapeathor-1.7.4/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.368810 mapeathor-1.7.4/src/mapeathor/
+-rw-r--r--   0 runner     (501) staff       (20)     1795 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)       22 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/_version.py
+-rw-r--r--   0 runner     (501) staff       (20)     3881 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/api.py
+-rw-r--r--   0 runner     (501) staff       (20)     1206 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/global_config.py
+-rw-r--r--   0 runner     (501) staff       (20)    13044 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/mapping_generator.py
+-rw-r--r--   0 runner     (501) staff       (20)    13026 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/mapping_writer.py
+-rw-r--r--   0 runner     (501) staff       (20)      782 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/source.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.365901 mapeathor-1.7.4/src/mapeathor/templates/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.372872 mapeathor-1.7.4/src/mapeathor/templates/r2rml/
+-rw-r--r--   0 runner     (501) staff       (20)       26 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Base.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       11 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Function.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      318 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Join.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      375 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/POM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Prefix.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       54 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Source.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       98 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/SourceQuery.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      102 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Subject.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       34 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/TriplesMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      384 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/config.json
+-rw-r--r--   0 runner     (501) staff       (20)      758 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/structure.json
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.392098 mapeathor-1.7.4/src/mapeathor/templates/rml/
+-rw-r--r--   0 runner     (501) staff       (20)       26 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Base.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      189 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Function.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/FunctionMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      122 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/FunctionPOM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      145 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/FunctionSource.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      279 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Join.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      388 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/POM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Prefix.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Source.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      103 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/SourceQuery.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      108 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Subject.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/TriplesMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      444 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/config.json
+-rw-r--r--   0 runner     (501) staff       (20)      209 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/rmlMapping.json
+-rw-r--r--   0 runner     (501) staff       (20)     1146 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/structure.json
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.397686 mapeathor-1.7.4/src/mapeathor/templates/rml2014/
+-rw-r--r--   0 runner     (501) staff       (20)       26 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Base.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      186 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Function.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/FunctionMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      122 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/FunctionPOM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      145 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/FunctionSource.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      268 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Join.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      375 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/POM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Prefix.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      123 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Source.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       99 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/SourceQuery.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      102 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Subject.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       34 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/TriplesMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      442 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/config.json
+-rw-r--r--   0 runner     (501) staff       (20)      209 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/rmlMapping.json
+-rw-r--r--   0 runner     (501) staff       (20)     1250 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/structure.json
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.401823 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/
+-rw-r--r--   0 runner     (501) staff       (20)       25 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Base.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       12 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Function.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      198 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Join.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      234 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/POM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      107 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Prefix.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       70 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Source.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       83 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/SourceQuery.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       36 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Subject.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       13 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/TriplesMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      415 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/config.json
+-rw-r--r--   0 runner     (501) staff       (20)     1218 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/structure.json
+-rw-r--r--   0 runner     (501) staff       (20)     3711 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.402243 mapeathor-1.7.4/src/mapeathor.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    18422 2024-05-11 09:55:35.000000 mapeathor-1.7.4/src/mapeathor.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2773 2024-05-11 09:55:35.000000 mapeathor-1.7.4/src/mapeathor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-11 09:55:35.000000 mapeathor-1.7.4/src/mapeathor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-11 09:55:35.000000 mapeathor-1.7.4/src/mapeathor.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       10 2024-05-11 09:55:35.000000 mapeathor-1.7.4/src/mapeathor.egg-info/top_level.txt
```

### Comparing `mapeathor-1.6.1/setup.py` & `mapeathor-1.7.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     requirements = r.read().split("\n")[0:-1]
 
 setup(
     name="mapeathor",
     version=version,
     author="Ana Iglesias-Molina",
     author_email="ana.iglesiasm@upm.es",
-    license="Apache 2.0",
-    description="Mapeathor is a simple spreadsheet parser able to generate mapping rules in three mapping languages: R2RML, RML (with extension to functions from FnO) and YARRRML.",
+    license_files = ('LICENSE'),
+    description="Mapeathor is a simple spreadsheet parser able to generate mapping rules in three mapping languages: R2RML, RML (releases on 2014 and 2023) and YARRRML.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/oeg-upm/Mapeathor",
     project_urls={
         'Documentation': 'https://github.com/oeg-upm/Mapeathor/wiki',
         'Source code': 'https://github.com/oeg-upm/Mapeathor/tree/master/src/mapeathor',
         'Issue tracker': 'https://github.com/oeg-upm/Mapeathor/issues',
```

### Comparing `mapeathor-1.6.1/src/mapeathor/__init__.py` & `mapeathor-1.7.4/src/mapeathor/__init__.py`

 * *Files identical despite different names*

### Comparing `mapeathor-1.6.1/src/mapeathor/api.py` & `mapeathor-1.7.4/src/mapeathor/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,68 +26,68 @@
 ## file: output mapping
 
 SWAGGER_URL = '/api/docs'  # URL for exposing Swagger UI (without trailing '/')
 API_URL = '/api/'  # Our API url (can of course be a local resource)
 
 # Call factory function to create our blueprint
 swaggerui_blueprint = get_swaggerui_blueprint(
-    SWAGGER_URL,  
+    SWAGGER_URL,
     API_URL,
-    config={ 
+    config={
         'app_name': "Mapeathor"
     },
 )
 
 app.register_blueprint(swaggerui_blueprint, url_prefix=SWAGGER_URL)
 
 
 class Mapeathor(Resource):
     def get(self):
         swag = swagger(app)
         swag['info']['version'] = "1.0.0"
         swag['info']['title'] = "Mapeathor"
         return jsonify(swag)
-        
+
     def post(self):
-        
+
         """
         Translate mapping document
         ---
-        
+
         components:
           schemas:
             Excel:
               type: object
               properties:
                 format:
                   type: string
-                  enum: [ "rml", "r2rml", "yarrrml"]
+                  enum: [ "rml", "rml2014", "r2rml", "yarrrml"]
                 file:
                   type: file
                   description: XLS[X] file to convert
             GSpreadSheet:
               type: object
               properties:
                 format:
                   type: string
-                  enum: [ "rml", "r2rml", "yarrrml"]
+                  enum: [ "rml", "rml2014", "r2rml", "yarrrml"]
                 url:
                   type: string
                   description: Google Spreadsheet url to convert
 
         summary: Uploads a file.
         consumes:
             - multipart/form-data
         produces:
             - binary/octet-stream
         parameters:
             - in: formData
               name: format
               type: text
-              enum: [ "rml", "r2rml", "yarrrml"]
+              enum: [ "rml", "rml2014", "r2rml", "yarrrml"]
               description: Mapping output format
             - in: formData
               name: url
               type: string
               description: Google Spreadsheet url to convert
             - in: formData
               name: file
@@ -97,52 +97,51 @@
             '200':
                 description: 'Mapping file in the specified format'
             '401':
                 description: 'Bad request'
             '500':
                 description: 'Internal tool error'
         """
-        
+
         data = parser.parse_args()
-        
+
         print(data)
-        
+
         if data['file'] is None and data['url'] is None:
             return {'message':'File or URL not found'}
         if data['format'] is None:
             return {'message':'No output mapping format specified'}
         else:
-            
+
             temp_out = tempfile.NamedTemporaryFile(prefix="mapeathor-api").name
-            
+
             if data['file'] is None or data['file'].filename == "":
-                
+
                 temp_in = mapeathor.gdriveToXMLX(data['url'])
-            
+
             else:
-                
+
                 temp_in = tempfile.NamedTemporaryFile(prefix="mapeathor-api").name
 
                 data['file'].save(temp_in)
-                
+
                 print(len(temp_in))
-            
+
             mapeathor.setMappingLanguage(data["format"])
-            
+
             outputFile = mapeathor.generateMapping(temp_in, temp_out)
-            
+
             return send_file(outputFile, as_attachment=True)
-            
+
 
 api.add_resource(Mapeathor, API_URL)
 
 
 def run(host="0.0.0.0", port=5000):
-    
+
     print("API URL: "+API_URL)
     print("SWAGGER URL: "+SWAGGER_URL)
-    
+
     app.run(debug=False, host=host, port=port)
 
 if __name__ == '__main__':
     run()
-
```

### Comparing `mapeathor-1.6.1/src/mapeathor/global_config.py` & `mapeathor-1.7.4/src/mapeathor/global_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 import os
 
 
 tmpDir = tempfile.TemporaryDirectory(prefix="mapeathor").name+"/"
 baseTemplatesDir = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'templates') + '/'
 dataTypesFile = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'dataTypes.json')
 resultDir = tempfile.TemporaryDirectory(prefix="mapeathor").name+"/"
-supportedLanguages = {'rml', 'r2rml', 'yarrrml'}
+supportedLanguages = {'rml', 'rml2014', 'r2rml', 'yarrrml'}
 
 
-def setMappingLanguage(language):
+def setMappingLanguage(lang):
     global templatesDir
-    templatesDir = baseTemplatesDir + language.lower() + "/"
+    global language
+
+    templatesDir = baseTemplatesDir + lang.lower() + "/"
+    language = lang.lower()
 
 
 defaultDataTypes = {
 
    "string":[
       "string",
       "nan",
@@ -52,13 +55,17 @@
    ],
    "anyURI":[
       "anyuri",
       "iri",
       "uri",
       "url"
    ],
-"BlankNode":[
-   "blanknode",
-   "blank node",
-   "bn"
-]
+   "BlankNode":[
+      "blanknode",
+      "blank node",
+      "bn"
+    ],
+    "gYear":[
+       "year",
+       "gyear"
+     ]
 }
```

### Comparing `mapeathor-1.6.1/src/mapeathor/mapping_generator.py` & `mapeathor-1.7.4/src/mapeathor/mapping_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from . import utils
 
 def generateJson(path):
     """
     The input excel file 'path' is translated into JSON format, returns the json
     """
     data = pandas.ExcelFile(path, engine='openpyxl')
-    json = {}
+    tmpjson = {}
     for sheet_ in data.sheet_names:
         sheet = str(sheet_)
-        json[sheet] = {}
-        json[sheet] = generateJsonCols(data.parse(sheet))
-    return json
+        tmpjson[sheet] = {}
+        tmpjson[sheet] = generateJsonCols(data.parse(sheet))
+    return tmpjson
 
 
 def generateJsonCols(data):
     """
     Arranges correctly the input pandas dataframe into a json, which is returned as output
     """
     rng = len(data[data.columns[0]])
@@ -37,36 +37,36 @@
     return result
 
 
 def organizeJson(data):
     """
     Rearranges the data in JSON format into the desired structure, returns the resulting json
     """
-    json = {}
-    json['Prefix'] = data['Prefix']
-    json['TriplesMap'] = {}
+    tmpjson = {}
+    tmpjson['Prefix'] = data['Prefix']
+    tmpjson['TriplesMap'] = {}
     formated_subjects = reFormatSubject(data['Subject'])
     function_reference = False
     for subject in formated_subjects:
-        json['TriplesMap'][subject['ID']] = findChilds(data, subject['ID'])
-        json['TriplesMap'][subject['ID']]['Subject'] = subject
-        json['TriplesMap'][subject['ID']]['Subject']['SubjectType'] = utils.predicateTypeIdentifier(subject['URI'])
-        json['TriplesMap'][subject['ID']]['Subject']['SubjectTermType'] = utils.subjectTermTypeIdentifier(subject['URI'])
-        json['TriplesMap'][subject['ID']]['Source'] = reFormatSource(json['TriplesMap'][subject['ID']]['Source'])
-        json['TriplesMap'][subject['ID']]['Predicate_Object']  =  reFormatPredicateObject(json['TriplesMap'][subject['ID']]['Predicate_Object'])
-        if json['TriplesMap'][subject['ID']]['Predicate_Object']['Function'] != []:
+        tmpjson['TriplesMap'][subject['ID']] = findChilds(data, subject['ID'])
+        tmpjson['TriplesMap'][subject['ID']]['Subject'] = subject
+        tmpjson['TriplesMap'][subject['ID']]['Subject']['SubjectType'] = utils.predicateTypeIdentifier(subject['URI'])
+        tmpjson['TriplesMap'][subject['ID']]['Subject']['SubjectTermType'] = utils.subjectTermTypeIdentifier(subject['URI'])
+        tmpjson['TriplesMap'][subject['ID']]['Source'] = reFormatSource(tmpjson['TriplesMap'][subject['ID']]['Source'])
+        tmpjson['TriplesMap'][subject['ID']]['Predicate_Object']  =  reFormatPredicateObject(tmpjson['TriplesMap'][subject['ID']]['Predicate_Object'])
+        if tmpjson['TriplesMap'][subject['ID']]['Predicate_Object']['Function'] != []:
             function_reference = True
-        if 'Graph' in json['TriplesMap'][subject['ID']]['Subject']:
-            json['TriplesMap'][subject['ID']]['Subject']['GraphType'] = utils.predicateTypeIdentifier(subject['Graph'])
+        if 'Graph' in tmpjson['TriplesMap'][subject['ID']]['Subject']:
+            tmpjson['TriplesMap'][subject['ID']]['Subject']['GraphType'] = utils.predicateTypeIdentifier(subject['Graph'])
     # If function references in TMs, process functions
     if function_reference:
-        json['Function'] = reFormatFunction(data['Function'], json)
+        tmpjson['Function'] = reFormatFunction(data['Function'], tmpjson)
     else:
-        json['Function'] = {}
-    return json
+        tmpjson['Function'] = {}
+    return tmpjson
 
 
 def reFormatSubject(data):
     """
     Reorganize subjects in case there is more than one class per ID
     """
     id_class = {}
@@ -125,26 +125,37 @@
 
         element['FunctionID'] = str(element['FunctionID'])[1:-1]
         if element['FunctionID'] not in result.keys():
             result[element['FunctionID']] = {'Predicate_Object':[], 'Source':[]}
             FID = element['FunctionID']
 
         if element['FunctionID'] == FID:
-            if("{" not in str(element['Value']) and "}" not in str(element['Value']) and '<' != str(element['Value'])[0]):
-                element['ValueType'] = 'rr:constant'
-            elif(str(element['Value'])[:1] == '{' and str(element['Value'])[-1:] == '}'):
-                element['Value'] = str(element['Value'])[1:-1]
-                element['ValueType'] = 'rml:reference'
-            elif(str(element['Value'])[:1] == '<' and str(element['Value'])[-1:] == '>'):
-                element['Value'] = '<#' + str(element['Value'])[1:]
-                element['ValueType'] = ''
+            if element['Feature'] == 'executes':
+                result[element['FunctionID']]['Executes'] = element['Value']
+            elif element['Feature'] == 'returns':
+                result[element['FunctionID']]['Returns'] = element['Value']
             else:
-                print('WARNING: Wrong element in Function', FID)
-                element['ValueType'] = 'rr:constant'
-            result[element['FunctionID']]['Predicate_Object'].append(element)
+                if("{" not in str(element['Value']) and "}" not in str(element['Value']) and '<' != str(element['Value'])[0]):
+                    if global_config.language == 'rml2014':
+                        element['ValueType'] = 'rr:constant'
+                    else:
+                        element['ValueType'] = 'rml:constant'
+                elif(str(element['Value'])[:1] == '{' and str(element['Value'])[-1:] == '}'):
+                    element['Value'] = str(element['Value'])[1:-1]
+                    element['ValueType'] = 'rml:reference'
+                elif(str(element['Value'])[:1] == '<' and str(element['Value'])[-1:] == '>'):
+                    element['Value'] = '<#' + str(element['Value'])[1:]
+                    element['ValueType'] = ''
+                else:
+                    print('WARNING: Wrong element in Function', FID)
+                    if global_config.language == 'rml2014':
+                        element['ValueType'] = 'rr:constant'
+                    else:
+                        element['ValueType'] = 'rml:constant'
+                result[element['FunctionID']]['Predicate_Object'].append(element)
 
     for fun in result:
         result[fun]['Source'] = find_source(fun, data, result)
 
     return(result)
 
 
@@ -194,15 +205,15 @@
         element['TermType'], element['isIRI'] = utils.termTypeIdentifier(element['Object'], element['DataType'])
 
         # Populate Join key
         if(str(element['Object'])in nullValues and str(element['InnerRef']) not in nullValues and str(element['OuterRef']) not in nullValues):
             element['ObjectType'] = 'reference'
             result['Join'].append(element)
         # Populate Function key
-        elif(str(element['Object'])[:1] == '<' and str(element['Object'])[-1:] == '>'):
+        elif(bool(re.search("^<[^<]+>$", str(element['Object'])))):
             element['ObjectType'] = 'reference'
             element['Object'] = str(element['Object'])[1:-1]
             result['Function'].append(element)
         # Populate Constant key
         elif("{" not in str(element['Object']) and "}" not in str(element['Object'])):
             element['ObjectType'] = 'constant'
             element['ObjTermMap'] = utils.replaceTermMap(element['ObjectType'])
@@ -235,15 +246,15 @@
             elif result['Format'].lower() == 'xml':
                 result['Format'] = 'XPath'
             elif result['Format'].lower() == 'xquery':
                 result['Format'] = 'XQuery'
             elif result['Format'].lower() == 'csv':
                 result['Format'] = 'CSV'
 
-            if global_config.templatesDir[-8:-1] == 'yarrrml':
+            if global_config.language == 'yarrrml':
                 result['Format'] = str(result['Format']).lower()
 
         elif(element['Feature'].lower() == 'iterator'):
             result['Iterator'] = str(element['Value'])
         elif(element['Feature'].lower() == 'table'):
             result['Table'] = str(element['Value'])
         elif(element['Feature'].lower() == 'query'):
@@ -284,22 +295,24 @@
         outputFile = global_config.resultDir + re.findall(r'\/?([\w\-\_\[\]\(\)]+)\.',inputFile)[0]  ## wider option \/?([^\.\/]+)\.
 
     ## Without try/except
     #json = generateJson(inputFile)
     #json = organizeJson(json)
 
     try:
-        json = generateJson(inputFile)
+        tmpjson = generateJson(inputFile)
         #print("First JSON: ")
         #print(str(json).replace('\'', '\"'))
-        json = organizeJson(json)
+        tmpjson = organizeJson(tmpjson)
         #print("Second JSON: ")
         #print(str(json).replace('\'', '\"'))
+        #with open('tmp.json', 'w') as file:
+        #    json.dump(tmpjson, file, indent=4)
         # sys.exit()
     except KeyError:
         print("ERROR: The spreadsheet template is not correct. Check the sheet and column names are correct.")
         sys.exit()
 
-    mapping_writer.writeValues(json,global_config.tmpDir)
+    mapping_writer.writeValues(tmpjson,global_config.tmpDir)
 
-    outputFile = mapping_writer.writeFinalFile(outputFile, json['TriplesMap'].keys(), json['Function'].keys())
+    outputFile = mapping_writer.writeFinalFile(outputFile, tmpjson['TriplesMap'].keys(), tmpjson['Function'].keys())
     return outputFile
```

### Comparing `mapeathor-1.6.1/src/mapeathor/mapping_writer.py` & `mapeathor-1.7.4/src/mapeathor/mapping_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,22 +15,22 @@
         os.mkdir(global_config.tmpDir)
 
     writePrefix(data,path)
     for triplesmap in data['TriplesMap']:
         writeTriplesMap(triplesmap, path)
         writeSubject(data['TriplesMap'][triplesmap]['Subject'], path)
         writeSource(data['TriplesMap'][triplesmap]['Source'], path)
-        writePredicateObjects(data['TriplesMap'][triplesmap]['Predicate_Object'], path)
+        writePredicateObjects(data['TriplesMap'][triplesmap]['Predicate_Object'],data['Function'], path)
 
     # Functions implemented only in RML
-    if global_config.templatesDir[-5:-1] == '/rml':
+    if global_config.language == 'rml' or global_config.language == 'rml2014':
         for function in data['Function']:
-            writeFunctionMap(function, path)
+            writeFunctionMap(function,data['Function'][function]['Executes'], path)
             writeFunctionPOM(data['Function'][function]['Predicate_Object'], path)
-            writeFunctionSource(data['Function'][function]['Source'], path)
+            #writeFunctionSource(data['Function'][function]['Source'], path)
 
 
 def writePrefix(data, path):
     """
     Writes the prefixes temporal file from the template with the information in 'data' into the path 'path'
     """
     file_loader = FileSystemLoader(global_config.templatesDir)
@@ -74,15 +74,15 @@
     output = template.render(tm=triples_maps)
     f = open(global_config.tmpDir + 'TriplesMap.txt', 'w')
     f.write(output + "\n")
     f.close()
     writeResult(str(data), 'TriplesMap')
 
 
-def writePredicateObjects(data, path):
+def writePredicateObjects(data, functions, path):
     """
     Writes the Predicate_Object temporal file from the template with the information in 'data' into the path 'path'
     """
     file_loader = FileSystemLoader(global_config.templatesDir)
     env = Environment(loader=file_loader)
 
     for key in data:
@@ -92,14 +92,18 @@
 
                 predicateObjects['Object'] = utils.replaceVars(str(predicateObjects['Object']), str(predicateObjects['ObjectType']), str(predicateObjects['TermType']))
                 if not str(predicateObjects['PredicateType']) == "constant":
                     predicateObjects['Predicate'] = utils.replaceVars(str(predicateObjects['Predicate']), str(predicateObjects['PredicateType']), 'nan')
                 if( 'InnerRef' in predicateObjects.keys() and 'OuterRef' in predicateObjects.keys()):
                     predicateObjects['InnerRef'] = utils.replaceVars(str(predicateObjects['InnerRef']), 'join_condition', 'nan')
                     predicateObjects['OuterRef'] = utils.replaceVars(str(predicateObjects['OuterRef']), 'join_condition', 'nan')
+                if key == 'Function':
+                    for fun_pom in data[key]:
+                        fun_pom['Returns'] = functions[fun_pom['Object']]['Returns']
+
 
                 output = template.render(pom=predicateObjects)
                 f = open(global_config.tmpDir + key + '.txt', 'w')
                 f.write(output + "\n")
                 f.close()
                 writeResult(data[key][0]['ID'], key)
 
@@ -162,29 +166,44 @@
     data['URI'] = utils.replaceVars(data['URI'], data['SubjectType'], 'nan')
     data['SubTermMap'] = utils.replaceTermMap(data['SubjectType'])
 
     if 'Graph' in data:
         data['Graph'] = utils.replaceVars(data['Graph'], data['GraphType'], 'nan')
         data['GraphTermMap'] = utils.replaceTermMap(data['GraphType'])
 
-    if global_config.templatesDir[-8:-1] != 'yarrrml':
+    if global_config.language == 'rml2014' or global_config.language == 'r2rml':
         f.write('rr:subjectMap [\n\ta rr:Subject ;\n\trr:termType rr:' + data['SubjectTermType'] + ' ;\n')
         if not isnan:
             f.write('\t' + data['SubTermMap'] + ' ' + data['URI'] + ' ;\n')
 
         if data['Class'] != ['nan']:
             for class_s in data['Class']:
                 f.write('\trr:class ' + class_s + ' ;\n')
 
         if 'Graph' in data:
             if data['Graph'] != '"nan"':
                 f.write('\trr:graphMap [ ' + data['GraphTermMap'] + ' ' + data['Graph'] + ' ] ;\n')
 
+        f.write('];\n')
+
+    elif global_config.language == 'rml':
+        f.write('rml:subjectMap [\n\ta rml:Subject ;\n\trml:termType rml:' + data['SubjectTermType'] + ' ;\n')
+        if not isnan:
+            f.write('\t' + data['SubTermMap'] + ' ' + data['URI'] + ' ;\n')
+
+        if data['Class'] != ['nan']:
+            for class_s in data['Class']:
+                f.write('\trml:class ' + class_s + ' ;\n')
+
+        if 'Graph' in data:
+            if data['Graph'] != '"nan"':
+                f.write('\trml:graphMap [ ' + data['GraphTermMap'] + ' ' + data['Graph'] + ' ] ;\n')
 
         f.write('];\n')
+
     else:
         if not isnan:
             f.write('subjects: ' + data['URI'] + '\n')
 
         if 'Graph' in data:
             if data['Graph'] != '"nan"':
                 f.write('graph: ' + data['Graph'] + '\n')
@@ -195,32 +214,33 @@
             for class_s in data['Class']:
                 f.write('  - [a, ' + class_s + ']\n')
 
     f.close()
     writeResult(data['ID'], 'Subject')
 
 
-def writeFunctionMap(data, path):
+def writeFunctionMap(function_id,function_execution, path):
     """
     Writes the function map temporal file from the template with the information in 'data' into the path 'path'
     """
     file_loader = FileSystemLoader(global_config.templatesDir)
     env = Environment(loader=file_loader)
     template = env.get_template('FunctionMap.tmpl')
 
-    fun_tm = {'FunctionID' : data}
+    fun_tm = {'FunctionID' : function_id, 'Execution' : function_execution}
     output = template.render(fun_tm=fun_tm)
     f = open(global_config.tmpDir + 'FunctionMap.txt', 'w')
     f.write(output + "\n")
     f.close()
-    writeResult(str(data), 'FunctionMap')
+    writeResult(str(function_id), 'FunctionMap')
 
 
 def writeFunctionSource(data, path):
     """
+    DEPRECATED FOR NEW FNML SPEC
     Writes the source of function temporal file from the template with the information in 'data' into the path 'path'
     """
     file_loader = FileSystemLoader(global_config.templatesDir)
     env = Environment(loader=file_loader)
     template = env.get_template('FunctionSource.tmpl')
 
     config  = json.loads(open(global_config.templatesDir + 'config.json').read())
@@ -239,16 +259,16 @@
     Writes the Predicate_Object of function temporal file from the template with the information in 'data' into the path 'path'
     """
     file_loader = FileSystemLoader(global_config.templatesDir)
     env = Environment(loader=file_loader)
     template = env.get_template('FunctionPOM.tmpl')
 
     for pom in data:
-        if pom['Feature'] != 'fno:executes' and str(pom['Value'])[0] != '<':
-            pom['Value'] = '[ \"' + pom['Value'] + '\" ]'
+        if str(pom['Value'])[0] != '<':
+            pom['Value'] = '\"' + pom['Value'] + '\"'
         elif str(pom['Value'])[0] == '<' and str(pom['Value'])[0] == '<' and str(pom['Value'])[-1] == '>':
             pom['Value'] = pom['Value']
 
 
         output = template.render(pom=pom)
         f = open(global_config.tmpDir + 'FunctionPOM.txt', 'w')
         f.write(output + "\n")
```

### Comparing `mapeathor-1.6.1/src/mapeathor/source.py` & `mapeathor-1.7.4/src/mapeathor/source.py`

 * *Files identical despite different names*

### Comparing `mapeathor-1.6.1/src/mapeathor/utils.py` & `mapeathor-1.7.4/src/mapeathor/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 def replaceVars(element, type_, termtype_):
     """
     Writes the objects 'element' correctly according to their type 'type_' and termtype 'termtype_', returns the
     corrected object
     """
     config = json.loads(open(global_config.templatesDir + 'config.json').read())
     # Add "" to the constant literal objects in YARRRML
-    if(global_config.templatesDir[-8:-1] == 'yarrrml' and type_ == 'constant'):
+    if(global_config.language == 'yarrrml' and type_ == 'constant'):
         result = str(config['variable'][type_]['before']) + element + str(config['variable'][type_]['after'])
 
     # Replace '{' and '}' in all but constant objects according to the config.json file of each language
     elif(type_ != 'constant' and str(config['variable'][type_]['before']) != '{' and str(config['variable'][type_]['after']) != '}'):
         result = element.replace("{", str(config['variable'][type_]['before'])).replace("}", config['variable'][type_]['after'])
 
-    elif(((termtype_ != 'IRI' and type_ == 'constant') or type_ == 'template' or (termtype_ == 'IRI' and element[0:4] == 'http')) and (global_config.templatesDir[-4:-1] == 'rml' or global_config.templatesDir[-6:-1] == 'r2rml')):
+    elif(((termtype_ != 'IRI' and type_ == 'constant') or type_ == 'template' or (termtype_ == 'IRI' and element[0:4] == 'http')) and (global_config.language != 'yarrrml')):
         result = "\"" + element + "\""
 
     else:
         result = element
     return result
 
 
@@ -75,23 +75,27 @@
         return 'BlankNode'
 
 
 def predicateTypeIdentifier(element):
     """
     Identifies the type of the predicate, distinguishing between constant, reference and template, and returns it
     """
-    # For constant
-    if(len(str(element).split(":")) == 2 and "{" not in str(element) and "}" not in str(element)):
-        return 'constant'
     # For reference
-    elif(str(element)[:1] == '{' and str(element)[-1:] == '}' and len(str(element).split(" "))  == 1):
+    if(str(element)[:1] == '{' and str(element)[-1:] == '}' and len(str(element).split(" "))  == 1):
         return 'reference'
     # For template
     elif(bool(re.search("{.+}.+", str(element))) or bool(re.search(".+{.+}", str(element)))):
         return 'template'
+    # For star maps
+    #elif(bool(re.search("^<<.+>>$", str(element)))):
+    #    print("\n\n\n")
+    #    return 'starmap'
+    # For constant
+    elif(len(str(element).split(":")) == 2 and "{" not in str(element) and "}" not in str(element)):
+        return 'constant'
     # Constant when not recognized
     else:
         #print("WARNING: type not identified for predicate '" + element + "', 'constant' assigned")
         return 'constant'
 
 
 def cleanDir(path):
```

### Comparing `mapeathor-1.6.1/src/mapeathor/templates/r2rml/structure.json` & `mapeathor-1.7.4/src/mapeathor/templates/rml2014/structure.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.86%*

 * *Differences: {"'unique'": "{0: {'before': '@prefix rr: <http://www.w3.org/ns/r2rml#>.\\n@prefix xsd: "*

 * *             '<http://www.w3.org/2001/XMLSchema#>.\\n@prefix rml: '*

 * *             "<http://semweb.mmlab.be/ns/rml#>.\\n@prefix ql: <http://semweb.mmlab.be/ns/ql#>.'}}",*

 * * "'variable'": "{0: {'childs': {insert: [(4, OrderedDict([('before', ''), ('file', 'Function'), "*

 * *               "('tabs', 1), ('childs', []), ('after', '')]))]}}, insert: [(1, "*

 * *               "OrderedDict([('before', ''), ('file', 'FunctionMap'), ('tab […]*

```diff
@@ -1,12 +1,12 @@
 {
     "unique": [
         {
             "after": "",
-            "before": "@prefix rr: <http://www.w3.org/ns/r2rml#>.\n@prefix xsd: <http://www.w3.org/2001/XMLSchema#>.\n@prefix ql: <http://semweb.mmlab.be/ns/ql#>.",
+            "before": "@prefix rr: <http://www.w3.org/ns/r2rml#>.\n@prefix xsd: <http://www.w3.org/2001/XMLSchema#>.\n@prefix rml: <http://semweb.mmlab.be/ns/rml#>.\n@prefix ql: <http://semweb.mmlab.be/ns/ql#>.",
             "childs": [],
             "file": "Prefix",
             "tabs": 1
         },
         {
             "after": "",
             "before": "",
@@ -43,14 +43,43 @@
                 },
                 {
                     "after": "",
                     "before": "",
                     "childs": [],
                     "file": "Join",
                     "tabs": 1
+                },
+                {
+                    "after": "",
+                    "before": "",
+                    "childs": [],
+                    "file": "Function",
+                    "tabs": 1
                 }
             ],
             "file": "TriplesMap",
             "tabs": 1
+        },
+        {
+            "after": "    ]\n.\n",
+            "before": "",
+            "childs": [
+                {
+                    "after": "",
+                    "before": "",
+                    "childs": [],
+                    "file": "FunctionSource",
+                    "tabs": 2
+                },
+                {
+                    "after": "",
+                    "before": "",
+                    "childs": [],
+                    "file": "FunctionPOM",
+                    "tabs": 2
+                }
+            ],
+            "file": "FunctionMap",
+            "tabs": 1
         }
     ]
 }
```

### Comparing `mapeathor-1.6.1/src/mapeathor/templates/rml/structure.json` & `mapeathor-1.7.4/src/mapeathor/templates/rml/structure.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'unique'": "{0: {'before': '@prefix xsd: <http://www.w3.org/2001/XMLSchema#>.\\n@prefix rml: "*

 * *             "<https://w3id.org/rml/>.'}}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "unique": [
         {
             "after": "",
-            "before": "@prefix rr: <http://www.w3.org/ns/r2rml#>.\n@prefix xsd: <http://www.w3.org/2001/XMLSchema#>.\n@prefix rml: <http://semweb.mmlab.be/ns/rml#>.\n@prefix ql: <http://semweb.mmlab.be/ns/ql#>.",
+            "before": "@prefix xsd: <http://www.w3.org/2001/XMLSchema#>.\n@prefix rml: <https://w3id.org/rml/>.",
             "childs": [],
             "file": "Prefix",
             "tabs": 1
         },
         {
             "after": "",
             "before": "",
```

### Comparing `mapeathor-1.6.1/src/mapeathor/templates/yarrrml/structure.json` & `mapeathor-1.7.4/src/mapeathor/templates/yarrrml/structure.json`

 * *Files identical despite different names*

### Comparing `mapeathor-1.6.1/LICENSE` & `mapeathor-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mapeathor-1.6.1/README.md` & `mapeathor-1.7.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,42 @@
- [![Generic badge](https://img.shields.io/badge/Status-Developing-yellow)](https://shields.io/)
  [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/oeg-upm/Mapeathor/blob/master/LICENSE)
  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5973906.svg)](https://doi.org/10.5281/zenodo.5973906)
  [![version](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
  [![Latest PyPI version](https://img.shields.io/pypi/v/mapeathor?style=flat)](https://pypi.python.org/pypi/mapeathor)
 
 <p align="center">
  <img src="https://raw.githubusercontent.com/oeg-upm/Mapeathor/master/imgs/Square_logo_mapeathor.png" alt="workflow" width="150"/>
 </p>
 
 
 # Mapeathor
 #### Mapeathor translates your mapping rules specified in spreadsheets to a mapping language.  
 
-[Mapeathor](https://morph.oeg.fi.upm.es/tool/mapeathor) is a simple spreadsheet parser able to generate mapping rules in three mapping languages: R2RML, RML (with extension to functions from FnO) and YARRRML. It takes the mapping rules expressed in a spreadsheet and transforms them into the desired language. The spreadsheet template is designed to facilitate the mapping rules' writting, with the aim of being language independent, and thus, lowering the barrier of generating mappings for non-expert users.
+[Mapeathor](https://morph.oeg.fi.upm.es/tool/mapeathor) is a simple spreadsheet parser able to generate mapping rules in three mapping languages: R2RML, RML (releases on [2014](https://rml.io/specs/rml/) and [2023](https://w3id.org/rml/portal)) and YARRRML. It takes the mapping rules expressed in a spreadsheet and transforms them into the desired language. The spreadsheet template is designed to facilitate the mapping rules' writing, with the aim of being language independent, and thus, lowering the barrier of generating mappings for non-expert users.
 
 <p align="center">
  <img src="https://raw.githubusercontent.com/oeg-upm/Mapeathor/master/imgs/workflow.png" alt="workflow" width="600"/>
 </p>
 
 ## Example
 A more detailed explanation is provided in the [wiki](https://github.com/oeg-upm/Mapeathor/wiki).
 
-### First Step: Fill the xlsx template with the transformation rules
-The template has five mandatory sheets, *Prefixes, Source, Subject PredicateObjectMap* and *Functions*. The last one can be left blank in case there are no functions. The spreadsheet can be in XLSX format or a Google Spreadsheet. Here is an example of the structure of the spreadsheet.
+### First Step: Fill the spreadseet template with the transformation rules
+The template has five mandatory sheets, *Prefixes, Source, Subject PredicateObjectMap* and *Functions*. The last one can be left blank in case there are no functions. The spreadsheet can be in XLSX format or a Google Spreadsheet. **Careful!** When using Google Spreasheets, the sharing option must be enabled. Here is an example of the structure of the spreadsheet.
 
 <p align="center">
- <img src="https://raw.githubusercontent.com/oeg-upm/Mapeathor/master/imgs/sheets.png" alt="sheets" width="500"/>
+ <img src="https://raw.githubusercontent.com/oeg-upm/Mapeathor/master/imgs/new_sheets.png" alt="sheets" width="500"/>
 </p>
 
 ### Second Step: Choose the output language
-One of three options can be chosen: R2RML, RML or YARRRML.
+One of three options can be chosen: R2RML, RML, RML2014 or YARRRML.
 
 ### Third Step: Run it!
 The easiest way of running Mapeathor is using the [web service](https://morph.oeg.fi.upm.es/demo/mapeathor) and the [Swagger](https://morph.oeg.fi.upm.es/tool/mapeathor/swagger/) instance. For CLI lovers, the service is available as a [PyPi package](https://pypi.org/project/mapeathor/) and Docker image. The instructions of the latest can be found in the [wiki](https://github.com/oeg-upm/Mapeathor/wiki).
 
 ## Publications
 Iglesias-Molina, A., Pozo-Gilo, L., Dona, D., Ruckhaus, E., Chaves-Fraga, D., & Corcho, O. (2020, January). *Mapeathor: Simplifying the Specification of Declarative Rules for Knowledge Graph Construction. In ISWC (Demos/Industry).* [Online version](http://ceur-ws.org/Vol-2721/paper488.pdf)
 
-Iglesias-Molina, A., Chaves-Fraga, D., Priyatna, F., & Corcho, O. (2019). Towards the Definition of a Language-Independent Mapping Template for Knowledge Graph Creation. *In Proceedings of the Third International Workshop on Capturing Scientific Knowledge co-located with the 10th International Conference on Knowledge Capture (K-CAP 2019)* (pp. 33-36). [Online version](https://sciknow.github.io/sciknow2019/papers/SciKnow_2019_paper_4.pdf)
+Iglesias-Molina, A., Chaves-Fraga, D., Priyatna, F., & Corcho, O. (2019). Towards the Definition of a Language-Independent Mapping Template for Knowledge Graph Creation. *In Proceedings of the Third International Workshop on Capturing Scientific Knowledge co-located with the 10th International Conference on Knowledge Capture (K-CAP 2019)* (pp. 33-36). [Online version](https://ceur-ws.org/Vol-2526/short3.pdf)
 
 ## Authors and contact
 - [Ana Iglesias-Molina](https://github.com/anaigmo) - [ana.iglesiasm@upm.es](mailto:ana.iglesiasm@upm.es)
-- [Luis Pozo](https://github.com/w0xter)
-- [Daniel Doña](https://github.com/daniel-dona)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mapeathor-1.6.1/pyproject.toml` & `mapeathor-1.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 name = 'mapeathor'
 description = 'Mapeathor translates your mapping rules specified in spreadsheets to a mapping language.'
 readme = 'README.md'
 keywords = ['Mapeathor', 'R2RML', 'RML', 'YARRRML', 'Knowledge Graph', 'Data Integration']
 authors = [
   {name = 'Ana Iglesias-Molina', email = 'ana.iglesiasm@upm.es'}
 ]
-license = 'Apache-2.0'
+license =  {file = "LICENSE"}
 classifiers = [
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3.6',
   'Programming Language :: Python :: 3.7',
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
```

