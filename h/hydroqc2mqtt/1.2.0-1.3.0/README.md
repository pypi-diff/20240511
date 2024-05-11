# Comparing `tmp/hydroqc2mqtt-1.2.0.tar.gz` & `tmp/hydroqc2mqtt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydroqc2mqtt-1.2.0.tar", last modified: Fri Jan 19 18:57:55 2024, max compression
+gzip compressed data, was "hydroqc2mqtt-1.3.0.tar", last modified: Sat May 11 01:00:43 2024, max compression
```

## Comparing `hydroqc2mqtt-1.2.0.tar` & `hydroqc2mqtt-1.3.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.690767 hydroqc2mqtt-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1946 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    16777 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1255 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    19948 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)       80 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/.pypirc
--rw-rw-rw-   0 root         (0) root         (0)     1918 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    34523 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2625 2024-01-19 18:57:55.690767 hydroqc2mqtt-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1673 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2925 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/config.sample.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.682767 hydroqc2mqtt-1.2.0/hydroqc2mqtt/
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4211 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      275 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    21834 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt/contract_device.py
--rw-rw-rw-   0 root         (0) root         (0)    10820 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt/daemon.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt/error.py
--rw-rw-rw-   0 root         (0) root         (0)    28092 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt/hourly_consump_handler.py
--rw-rw-rw-   0 root         (0) root         (0)    26820 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt/sensors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.690767 hydroqc2mqtt-1.2.0/hydroqc2mqtt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2625 2024-01-19 18:57:55.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1526 2024-01-19 18:57:55.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-19 18:57:55.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-01-19 18:57:55.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      152 2024-01-19 18:57:55.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-01-19 18:57:55.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3199 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/hydroqc2mqtt.svg
--rw-rw-rw-   0 root         (0) root         (0)     1488 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     3398 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/renovate.json5
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/run.sample.sh
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-01-19 18:57:55.690767 hydroqc2mqtt-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.686767 hydroqc2mqtt-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)       37 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/homeassistant/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/homeassistant/sensor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.686767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/
--rw-rw-rw-   0 root         (0) root         (0)      731 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/config
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/account/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/account/state/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.686767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/balance/
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/balance/state
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/contract/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/contract/state/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.686767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/current period epp enabled/
--rw-rw-rw-   0 root         (0) root         (0)        3 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/current period epp enabled/state
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.670767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.686767 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/current billing period current day/
--rw-rw-rw-   0 root         (0) root         (0)        3 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/current billing period current day/state
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 18:57:55.690767 hydroqc2mqtt-1.2.0/tests/input_http_data/
--rw-rw-rw-   0 root         (0) root         (0)      305 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/input_http_data/calculerSommaireContractuel.json
--rw-rw-rw-   0 root         (0) root         (0)     1461 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/input_http_data/contrats.json
--rw-rw-rw-   0 root         (0) root         (0)    11032 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/input_http_data/creditPointeCritique.json
--rw-rw-rw-   0 root         (0) root         (0)     4417 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/input_http_data/infoCompte.json
--rw-rw-rw-   0 root         (0) root         (0)      765 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/input_http_data/outages.json
--rw-rw-rw-   0 root         (0) root         (0)      724 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/input_http_data/relations.json
--rw-rw-rw-   0 root         (0) root         (0)     6133 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/input_http_data/resourceObtenirDonneesConsommationHoraires.json
--rw-rw-rw-   0 root         (0) root         (0)    56115 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/input_http_data/resourceObtenirDonneesPeriodesConsommation.json
--rw-rw-rw-   0 root         (0) root         (0)     6906 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)    12452 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/test_base_sync_comsumption.py
--rw-rw-rw-   0 root         (0) root         (0)    10016 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tests/test_base_sync_comsumption_history.py
--rw-rw-rw-   0 root         (0) root         (0)     2766 2024-01-19 18:57:35.000000 hydroqc2mqtt-1.2.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.578731 hydroqc2mqtt-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)     2468 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/.env.sample
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/.gitlab-ci-local-env.sample
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/.gitlab-ci-local-variables.sample.yml
+-rw-rw-rw-   0 root         (0) root         (0)    18100 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    19948 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/.pypirc
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    34523 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2625 2024-05-11 01:00:43.578731 hydroqc2mqtt-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/config.sample.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.574731 hydroqc2mqtt-1.3.0/hydroqc2mqtt/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4212 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21835 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt/contract_device.py
+-rw-rw-rw-   0 root         (0) root         (0)    10821 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt/daemon.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt/error.py
+-rw-rw-rw-   0 root         (0) root         (0)    28093 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt/hourly_consump_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    29469 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt/sensors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.578731 hydroqc2mqtt-1.3.0/hydroqc2mqtt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2625 2024-05-11 01:00:43.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-05-11 01:00:43.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 01:00:43.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-11 01:00:43.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-11 01:00:43.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-11 01:00:43.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3199 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/hydroqc2mqtt.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     3407 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/renovate.json5
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/run.sample.sh
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-11 01:00:43.578731 hydroqc2mqtt-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.574731 hydroqc2mqtt-1.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.570731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.570731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/homeassistant/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.570731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/homeassistant/sensor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.574731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/
+-rw-rw-rw-   0 root         (0) root         (0)      731 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/config
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.570731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.574731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.570731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/account/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.570731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/account/state/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.570731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.574731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/balance/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/account/state/sensor/balance/state
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.574731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/contract/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.574731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/contract/state/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.574731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.574731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/current period epp enabled/
+-rw-rw-rw-   0 root         (0) root         (0)        3 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/contract/state/binary_sensor/current period epp enabled/state
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.574731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.574731 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/current billing period current day/
+-rw-rw-rw-   0 root         (0) root         (0)        3 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/hydroqc/home/contract/state/sensor/current billing period current day/state
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 01:00:43.578731 hydroqc2mqtt-1.3.0/tests/input_http_data/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/input_http_data/calculerSommaireContractuel.json
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/input_http_data/contrats.json
+-rw-rw-rw-   0 root         (0) root         (0)    11032 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/input_http_data/creditPointeCritique.json
+-rw-rw-rw-   0 root         (0) root         (0)     4417 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/input_http_data/infoCompte.json
+-rw-rw-rw-   0 root         (0) root         (0)      765 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/input_http_data/outages.json
+-rw-rw-rw-   0 root         (0) root         (0)      724 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/input_http_data/relations.json
+-rw-rw-rw-   0 root         (0) root         (0)     6133 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/input_http_data/resourceObtenirDonneesConsommationHoraires.json
+-rw-rw-rw-   0 root         (0) root         (0)    56115 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/input_http_data/resourceObtenirDonneesPeriodesConsommation.json
+-rw-rw-rw-   0 root         (0) root         (0)     6907 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    12453 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/test_base_sync_comsumption.py
+-rw-rw-rw-   0 root         (0) root         (0)    10017 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tests/test_base_sync_comsumption_history.py
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2024-05-11 01:00:34.000000 hydroqc2mqtt-1.3.0/tox.ini
```

### Comparing `hydroqc2mqtt-1.2.0/.gitignore` & `hydroqc2mqtt-1.3.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -119,14 +119,18 @@
 .ropeproject
 
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
+mypy-txt-report/
+mypy-html-report/
+mypy-junit.xml
+tests_result_junit.xml
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 /hydro-env/
 config.yaml
@@ -135,7 +139,10 @@
 # gitlab-ci-local
 .gitlab-ci-local-env
 .gitlab-ci-local/
 .gitlab-ci-local-variables.yml
 
 run.sh
 config.yaml
+
+# vscode
+.vscode/
```

### Comparing `hydroqc2mqtt-1.2.0/.gitlab-ci.yml` & `hydroqc2mqtt-1.3.0/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -52,35 +52,35 @@
     - name: eclipse-mosquitto:2.0.18
       alias: mosquitto
       entrypoint:
         - "/bin/sh"
       command:
         - -c
         - cp mosquitto-no-auth.conf /mosquitto/config/mosquitto.conf && cat /mosquitto/config/mosquitto.conf && /docker-entrypoint.sh mosquitto -c /mosquitto/config/mosquitto.conf
-    - name: homeassistant/home-assistant:2024.1.3
+    - name: homeassistant/home-assistant:2024.5.3
       alias: hass
       entrypoint:
         - bash
       command:
         - -c
         - |
           mkdir -p .storage && (echo ${HASS_AUTH} | base64 -d > .storage/auth) && (hass --script ensure_config -c /config 2>&1) && (echo 'homeassistant:' >> /config/configuration.yaml) && (echo '  time_zone: America/New_York' >> /config/configuration.yaml) && (echo '  latitude: 45.508888' >> /config/configuration.yaml) && (echo '  longitude: -73.561668' >> /config/configuration.yaml) && hass --script auth add admin password && sleep 1 && /init
   tags:
     - hydroqc
   image:
-    name: registry.gitlab.com/hydroqc/hydroqc-base-container/3.11:latest
+    name: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12:latest@sha256:f0eb93bcde1305fc63994808f56adc55951464f04d73a6aedb5f83e420e58a47
   variables:
     MQTT_HOST: mosquitto
     MQTT_PORT: "1883"
   script:
     - cp /usr/share/zoneinfo/America/New_York /etc/localtime
     - echo echo "America/New_York " > /etc/timezone
-    - pip install tox
+    - uv pip install --system --upgrade tox
     - tox --parallel auto
-    - pip install --upgrade setuptools_scm
+    - uv pip install --system --upgrade setuptools_scm
     - echo HYDROQC2MQTT_VERSION=$(python3 -m setuptools_scm) > collected.env
     - echo HYDROQC2MQTT_VERSION_STRIPPED=$(python3 -m setuptools_scm --strip-dev) >> collected.env
   artifacts:
     reports:
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
@@ -126,22 +126,22 @@
       command:
         - -c
         - |
           mkdir -p .storage && (echo ${HASS_AUTH} | base64 -d > .storage/auth) && (hass --script ensure_config -c /config 2>&1) && (echo 'homeassistant:' >> /config/configuration.yaml) && (echo '  time_zone: America/New_York' >> /config/configuration.yaml) && (echo '  latitude: 45.508888' >> /config/configuration.yaml) && (echo '  longitude: -73.561668' >> /config/configuration.yaml) && hass --script auth add admin password && sleep 1 && /init
   tags:
     - hydroqc
   image:
-    name: registry.gitlab.com/hydroqc/hydroqc-base-container/3.11:latest
+    name: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12:latest@sha256:f0eb93bcde1305fc63994808f56adc55951464f04d73a6aedb5f83e420e58a47
   variables:
     MQTT_HOST: mosquitto
     MQTT_PORT: "1883"
   script:
     - cp /usr/share/zoneinfo/America/New_York /etc/localtime
     - echo echo "America/New_York " > /etc/timezone
-    - pip install tox
+    - uv pip install --system --upgrade tox
     - tox --parallel auto
   artifacts:
     reports:
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
       junit: tests_result_junit.xml
@@ -167,18 +167,18 @@
       when: manual
     - when: never
 
 promote2pypi:
   stage: pypi
   tags:
     - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.11:latest
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12:latest@sha256:f0eb93bcde1305fc63994808f56adc55951464f04d73a6aedb5f83e420e58a47
   script:
-    - pip install --upgrade pip
-    - pip install --upgrade build setuptools_scm twine
+    - uv pip install --system --upgrade pip uv
+    - uv pip install --system --upgrade build setuptools_scm twine
     - python3 -m build -o dist
     - python3 -m twine check --strict dist/*
     - twine upload --verbose --non-interactive --repository pypi dist/*
   rules:
     - if: "$CI_SKIP =~ /pypi/"
       when: never
     - if: "$CI_COMMIT_TAG"
@@ -186,34 +186,40 @@
     - when: never
 
 set-version:
   stage: test
   tags:
     - hydroqc
   image:
-    name: registry.gitlab.com/hydroqc/hydroqc-base-container/3.11:latest
+    name: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12:latest@sha256:f0eb93bcde1305fc63994808f56adc55951464f04d73a6aedb5f83e420e58a47
   script:
     - echo HYDROQC2MQTT_VERSION=$(python3 -m setuptools_scm) > collected.env
     - echo HYDROQC2MQTT_VERSION_STRIPPED=$(python3 -m setuptools_scm --strip-dev) >> collected.env
   artifacts:
     reports:
       dotenv: collected.env
     paths:
       - collected.env
   rules:
     # Only run when test-hass-stable is disabled
     - if: "$CI_SKIP =~ /test-hass-stable/"
       when: on_success
+    # Run on renovate branches on changes to dockerfile or gitlab-ci
+    - if: "$CI_COMMIT_REF_NAME =~ /^renovate-/"
+      changes:
+        - Dockerfile
+        - .gitlab-ci.yml
+      when: on_success
     - when: never
 
 .build_generic: &build_generic
   stage: build
-  image: docker:24.0
+  image: docker:26.1
   services:
-    - docker:24.0-dind
+    - docker:26.1-dind
   script:
     - docker version
     - echo ${BUILD-ARG}
     - docker buildx build
       --platform linux/${BUILD_ARCH}
       -t ${CI_REGISTRY_IMAGE}/${ARCH}:${CI_COMMIT_SHORT_SHA}
       -f ./Dockerfile
@@ -235,14 +241,30 @@
         HQ2MQTT_VERSION: ${CI_COMMIT_TAG}
       when: on_success
     # Enabled for main branch
     - if: "$CI_COMMIT_REF_NAME == $CI_DEFAULT_BRANCH"
       variables:
         HQ2MQTT_VERSION: ${HYDROQC2MQTT_VERSION_STRIPPED}+${CI_COMMIT_REF_NAME}
       when: on_success
+    # Build on renovate branches on changes to dockerfile or gitlab-ci
+    - if: "$CI_COMMIT_REF_NAME =~ /^renovate-/"
+      variables:
+        HQ2MQTT_VERSION: ${HYDROQC2MQTT_VERSION_STRIPPED}+${CI_COMMIT_REF_NAME}
+      changes:
+        - Dockerfile
+        - .gitlab-ci.yml
+      when: on_success
+    # Only build renovate MR on changes to dockerfile or gitlab-ci
+    - if: "$CI_MERGE_REQUEST_IID && $CI_COMMIT_REF_NAME =~ /^renovate-/"
+      variables:
+        HQ2MQTT_VERSION: ${HYDROQC2MQTT_VERSION_STRIPPED}+${CI_COMMIT_REF_NAME}
+      changes:
+        - Dockerfile
+        - .gitlab-ci.yml
+      when: on_success
     # Never build renovate MR
     - if: "$CI_MERGE_REQUEST_IID && $CI_COMMIT_REF_NAME =~ /^renovate-/"
       when: never
     # Make it manual for external MR
     - if: "$CI_MERGE_REQUEST_IID && $CI_MERGE_REQUEST_PROJECT_PATH != $CI_MERGE_REQUEST_SOURCE_PROJECT_PATH"
       variables:
         HQ2MQTT_VERSION: ${HYDROQC2MQTT_VERSION_STRIPPED}+${CI_COMMIT_REF_NAME}
@@ -261,56 +283,63 @@
     BUILD_ARCH: amd64
   <<: *build_generic
 build_aarch64:
   variables:
     ARCH: aarch64
     BUILD_ARCH: aarch64
   <<: *build_generic
-  # rules:
-  #   - if: '$CI_COMMIT_TAG'
-  #     variables:
-  #       HQ2MQTT_VERSION: ${CI_COMMIT_TAG}
-  #     when: on_success
-  #   - when: manual
-  #     variables:
-  #       HQ2MQTT_VERSION: ${HYDROQC2MQTT_VERSION_STRIPPED}+${CI_COMMIT_REF_NAME}
-  #     allow_failure: true
+  rules:
+    - if: '$CI_COMMIT_TAG'
+      variables:
+        HQ2MQTT_VERSION: ${CI_COMMIT_TAG}
+      when: on_success
+    - when: manual
+      variables:
+        HQ2MQTT_VERSION: ${HYDROQC2MQTT_VERSION_STRIPPED}+${CI_COMMIT_REF_NAME}
+      allow_failure: true
 
 docker_tag:
   stage: tag
-  image: docker:24.0
+  image: docker:26.1
   services:
-    - docker:24.0-dind
+    - docker:26.1-dind
   script:
     - docker version
     - docker login -u $CI_REGISTRY_USER -p $CI_REGISTRY_PASSWORD $CI_REGISTRY
     - docker manifest create ${CI_REGISTRY_IMAGE}:${IMAGE_TAG}
-      ${CI_REGISTRY_IMAGE}/amd64:${CI_COMMIT_SHORT_SHA} ${CI_REGISTRY_IMAGE}/aarch64:${CI_COMMIT_SHORT_SHA}
-    - docker manifest push ${CI_REGISTRY_IMAGE}:${IMAGE_TAG}
+      ${CI_REGISTRY_IMAGE}/amd64:${CI_COMMIT_SHORT_SHA}
     - docker buildx imagetools inspect ${CI_REGISTRY_IMAGE}:${IMAGE_TAG} --format "{{json .Manifest}}"
-    # - |
-    #     for PLATFORM in aarch64
-    #       do
-    #         echo "docker manifest inspect ${CI_REGISTRY_IMAGE}/${PLATFORM}:${CI_COMMIT_SHORT_SHA}"
-    #         if docker manifest inspect ${CI_REGISTRY_IMAGE}/${PLATFORM}:${CI_COMMIT_SHORT_SHA}; then
-    #           echo "docker manifest create ${CI_REGISTRY_IMAGE}:${IMAGE_TAG} --amend ${CI_REGISTRY_IMAGE}/${PLATFORM}:${CI_COMMIT_SHORT_SHA}"
-    #           docker manifest create ${CI_REGISTRY_IMAGE}:${IMAGE_TAG} --amend ${CI_REGISTRY_IMAGE}/${PLATFORM}:${CI_COMMIT_SHORT_SHA}
-    #         else
-    #             echo "Build for ${PLATFORM} not available for this run."
-    #         fi
-    #     done
-    #- docker buildx imagetools inspect ${CI_REGISTRY_IMAGE}:${IMAGE_TAG} --format "{{json .Manifest}}"
-    #- docker manifest push ${CI_REGISTRY_IMAGE}:${IMAGE_TAG}
+    - |
+        for PLATFORM in aarch64
+          do
+            echo "docker manifest inspect ${CI_REGISTRY_IMAGE}/${PLATFORM}:${CI_COMMIT_SHORT_SHA}"
+            if docker manifest inspect ${CI_REGISTRY_IMAGE}/${PLATFORM}:${CI_COMMIT_SHORT_SHA}; then
+              echo "docker manifest create ${CI_REGISTRY_IMAGE}:${IMAGE_TAG} --amend ${CI_REGISTRY_IMAGE}/${PLATFORM}:${CI_COMMIT_SHORT_SHA}"
+              docker manifest create ${CI_REGISTRY_IMAGE}:${IMAGE_TAG} --amend ${CI_REGISTRY_IMAGE}/${PLATFORM}:${CI_COMMIT_SHORT_SHA}
+            else
+                echo "Build for ${PLATFORM} not available for this run."
+            fi
+        done
+    - docker buildx imagetools inspect ${CI_REGISTRY_IMAGE}:${IMAGE_TAG} --format "{{json .Manifest}}"
+    - docker manifest push ${CI_REGISTRY_IMAGE}:${IMAGE_TAG}
     - |
       if [ "$CI_COMMIT_TAG" ]; then
         docker manifest create ${CI_REGISTRY_IMAGE}:latest ${CI_REGISTRY_IMAGE}/amd64:${CI_COMMIT_SHORT_SHA} ${CI_REGISTRY_IMAGE}/aarch64:${CI_COMMIT_SHORT_SHA}
         docker manifest inspect ${CI_REGISTRY_IMAGE}:latest
         docker manifest push ${CI_REGISTRY_IMAGE}:latest
       fi
   rules:
+    # Only build renovate MR on changes to dockerfile or gitlab-ci
+    - if: "$CI_MERGE_REQUEST_IID && $CI_COMMIT_REF_NAME =~ /^renovate-/"
+      variables:
+        IMAGE_TAG: mr-${CI_COMMIT_REF_NAME}
+      changes:
+        - Dockerfile
+        - .gitlab-ci.yml
+      when: on_success
     # Never tag for renovate MR
     - if: "$CI_MERGE_REQUEST_IID && $CI_COMMIT_REF_NAME =~ /^renovate-/"
       when: never
     # Make it manual for external MR
     - if: "$CI_MERGE_REQUEST_IID && $CI_MERGE_REQUEST_PROJECT_PATH != $CI_MERGE_REQUEST_SOURCE_PROJECT_PATH"
       variables:
         IMAGE_TAG: mr-${CI_COMMIT_REF_NAME}
```

### Comparing `hydroqc2mqtt-1.2.0/.pre-commit-config.yaml` & `hydroqc2mqtt-1.3.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-docstring-first
   - id: check-yaml
   - id: debug-statements
   - id: check-ast
 
 - repo: https://github.com/psf/black
-  rev: 23.12.1
+  rev: 24.4.2
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/PyCQA/flake8/
   rev: 7.0.0
   hooks:
@@ -30,23 +30,22 @@
 
 - repo: https://github.com/PyCQA/doc8
   rev: v1.1.1
   hooks:
   - id: doc8
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.8.0
+  rev: v1.10.0
   hooks:
   - id: mypy
     args: [--strict, --pretty, --show-error-codes]
     additional_dependencies:
-      - "types-PyYAML==6.0.12.12"
+      - "types-PyYAML==6.0.12.20240311"
       - "pytest-stub==1.1.0"
-      - "types-paho-mqtt==1.6.0.20240106"
-      - "homeassistant-stubs==2024.1.3"
-      - "Hydro_Quebec_API_Wrapper==3.1.3"
-      - "mqtt-hass-base==4.2.5"
+      - "types-paho-mqtt==1.6.0.20240321"
+      - "homeassistant-stubs==2024.5.2"
+      - "Hydro_Quebec_API_Wrapper==3.2.0"
+      - "mqtt-hass-base==4.3.0"
       - "aioresponses==0.7.6"
-      - "types-python-dateutil==2.8.19.20240106"
-      - "types-pytz==2023.3.1.1"
+      - "types-python-dateutil==2.9.0.20240316"
+      - "types-pytz==2024.1.0.20240417"
       - "pkce==1.0.3"
-      - "aiomqtt==2.0.0"
```

### Comparing `hydroqc2mqtt-1.2.0/.pylintrc` & `hydroqc2mqtt-1.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/LICENSE` & `hydroqc2mqtt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/PKG-INFO` & `hydroqc2mqtt-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: hydroqc2mqtt
-Version: 1.2.0
+Version: 1.3.0
 Summary: Daemon managing hydroqc sensors through MQTT
 Home-page: https://hydroqc.ca
 Author-email: Hydroqc Team <info@hydroqc.ca>
 License: AGPL-3.0-or-later
 Project-URL: Source Code, https://gitlab.com/hydroqc/hydroqc2mqtt
 Project-URL: Bug Reports, https://gitlab.com/hydroqc/hydroqc2mqtt/-/issues
 Project-URL: Home-page, https://hydroqc.ca
 Keywords: hydro-quebec,mqtt,homeassistant,hydroqc
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.0
+Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mqtt-hass-base==4.2.5
-Requires-Dist: Hydro_Quebec_API_Wrapper==3.1.3
-Requires-Dist: python_dateutil==2.8.2
-Requires-Dist: packaging==23.2
-Requires-Dist: pytz==2023.3.post1
+Requires-Dist: mqtt-hass-base==4.3.0
+Requires-Dist: Hydro_Quebec_API_Wrapper==3.2.0
+Requires-Dist: python_dateutil==2.9.0.post0
+Requires-Dist: packaging==24.0
+Requires-Dist: pytz==2024.1
 Requires-Dist: homeassistant
 Requires-Dist: charset-normalizer==3.3.2
 
 # hydroqc2mqtt
 
 **The full updated project documentation can be found at [https://hydroqc.ca](https://hydroqc.ca)**
```

### Comparing `hydroqc2mqtt-1.2.0/README.md` & `hydroqc2mqtt-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/hydroqc2mqtt/__main__.py` & `hydroqc2mqtt-1.3.0/hydroqc2mqtt/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module defining entrypoint."""
+
 import argparse
 import asyncio
 import os
 
 from hydroqc2mqtt.daemon import Hydroqc2Mqtt
```

### Comparing `hydroqc2mqtt-1.2.0/hydroqc2mqtt/contract_device.py` & `hydroqc2mqtt-1.3.0/hydroqc2mqtt/contract_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module defining HydroQC Contract."""
+
 import datetime
 import logging
 from typing import TypedDict, cast
 
 import aiomqtt as mqtt
 import hydroqc
 import paho.mqtt.client as paho
```

### Comparing `hydroqc2mqtt-1.2.0/hydroqc2mqtt/daemon.py` & `hydroqc2mqtt-1.3.0/hydroqc2mqtt/daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Mqtt Daemon module."""
+
 import asyncio
 import os
 import re
 import sys
 from contextlib import AsyncExitStack
 from datetime import datetime
 from typing import Any, TypedDict
```

### Comparing `hydroqc2mqtt-1.2.0/hydroqc2mqtt/hourly_consump_handler.py` & `hydroqc2mqtt-1.3.0/hydroqc2mqtt/hourly_consump_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module defining HydroQC Contract."""
+
 import asyncio
 import copy
 import datetime
 import json
 import logging
 from collections.abc import Iterator
 from typing import TYPE_CHECKING, TypedDict, cast
```

### Comparing `hydroqc2mqtt-1.2.0/hydroqc2mqtt/sensors.py` & `hydroqc2mqtt-1.3.0/hydroqc2mqtt/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sensor definition list."""
+
 from typing import TypedDict
 
 # TODO: python 3.11 => uncomment Required
 # from typing_extensions import Required
 
 
 # TODO: python 3.11 => uncomment Required
@@ -105,674 +106,674 @@
     "icon": "mdi:lightning-bolt",
     "state_class": "total_increasing",
     "unit": "kWh",
     "sub_mqtt_topic": "contract/state",
 }
 
 
-SENSORS: dict[
-    str, SensorType
-] = {  # pylint: disable=consider-using-namedtuple-or-dataclass
-    # Account
-    "balance": {
-        "name": "Balance",
-        "data_source": "account.balance",
-        "device_class": "monetary",
-        "state_class": "total",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:currency-usd",
-        "unit": "CAD",
-        "sub_mqtt_topic": "account/state",
-        "rates": ["ALL"],
-    },
-    # Contract
-    "outage": {
-        "name": "Next or current outage",
-        "data_source": "contract.next_outage.start_date",
-        "device_class": "timestamp",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:calendar-start",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-        "attributes": {
-            "end_date": "contract.next_outage.end_date",
-            "cause": "contract.next_outage.cause.name",
-            "planned_duration": "contract.next_outage.planned_duration",
-            "code": "contract.next_outage.code.name",
-            "state": "contract.next_outage.status.name",
-            "emergency_level": "contract.next_outage.emergency_level",
-            "is_planned": "contract.next_outage.is_planned",
-        },
-    },
-    "current_billing_period_current_day": {
-        "name": "Current billing period current day",
-        "data_source": "contract.cp_current_day",
-        "device_class": None,
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:calendar-start",
-        "state_class": "measurement",
-        "unit": "days",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    "current_billing_period_duration": {
-        "name": "Current billing period duration",
-        "data_source": "contract.cp_duration",
-        "device_class": None,
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:calendar-expand-horizontal",
-        "state_class": "measurement",
-        "unit": "days",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    "current_billing_period_total_to_date": {
-        "name": "Current billing period total to date",
-        "data_source": "contract.cp_current_bill",
-        "device_class": "monetary",
-        "state_class": "total",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:currency-usd",
-        "unit": "CAD",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    "current_billing_period_projected_bill": {
-        "name": "Current billing period projected bill",
-        "data_source": "contract.cp_projected_bill",
-        "device_class": "monetary",
-        "state_class": "total",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:currency-usd",
-        "unit": "CAD",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    "current_billing_period_daily_bill_mean": {
-        "name": "Current billing period daily bill mean",
-        "data_source": "contract.cp_daily_bill_mean",
-        "device_class": "monetary",
-        "state_class": "total",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:currency-usd",
-        "unit": "CAD",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    "current_billing_period_daily_consumption_mean": {
-        "name": "Current billing period daily consumption mean",
-        "data_source": "contract.cp_daily_consumption_mean",
-        "device_class": "energy",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:home-lightning-bolt",
-        "unit": "kWh",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    "current_billing_period_total_consumption": {
-        "name": "Current billing period total consumption",
-        "data_source": "contract.cp_total_consumption",
-        "device_class": "energy",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:home-lightning-bolt",
-        "state_class": "total_increasing",
-        "unit": "kWh",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    "current_billing_period_projected_total_consumption": {
-        "name": "Current billing period projected total consumption",
-        "data_source": "contract.cp_projected_total_consumption",
-        "device_class": "energy",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:home-lightning-bolt",
-        "unit": "kWh",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    "current_billing_period_average_temperature": {
-        "name": "Current billing period average temperature",
-        "data_source": "contract.cp_average_temperature",
-        "device_class": "temperature",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:thermometer",
-        "state_class": "measurement",
-        "unit": "°C",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    "current_billing_period_kwh_cost_mean": {
-        "name": "Current billing period kwh cost mean",
-        "data_source": "contract.cp_kwh_cost_mean",
-        "device_class": "monetary",
-        "state_class": "total",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:currency-usd",
-        "unit": "CAD/kWh",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    "current_billing_period_rate": {
-        "name": "Current billing period rate",
-        "data_source": "contract.rate",
-        "device_class": None,
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:playlist-check",
-        "state_class": None,
-        "unit": None,
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    "current_billing_period_rate_option": {
-        "name": "Current billing period rate option",
-        "data_source": "contract.rate_option",
-        "device_class": None,
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:playlist-star",
-        "state_class": None,
-        "unit": None,
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    # FlexD and DT (identical for now...)
-    "current_billing_period_higher_price_consumption": {
-        "name": "Current billing period higher price consumption",
-        "data_source": "contract.cp_higher_price_consumption",
-        "device_class": "energy",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:home-lightning-bolt",
-        "unit": "kWh",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["DT", "DPC"],
-    },
-    "current_billing_period_lower_price_consumption": {
-        "name": "Current billing period lower price consumption",
-        "data_source": "contract.cp_lower_price_consumption",
-        "device_class": "energy",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:home-lightning-bolt-outline",
-        "unit": "kWh",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["DT", "DPC"],
-    },
-    "amount_saved_vs_base_rate": {
-        "name": "Net saving/loss vs rate D",
-        "data_source": "contract.amount_saved_vs_base_rate",
-        "device_class": "monetary",
-        "state_class": "total",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:currency-usd",
-        "unit": "CAD",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["DT", "DPC"],
-    },
-    # FlexD
-    "dpc_state": {
-        "name": "Current DPC period detail",
-        "data_source": "contract.peak_handler.current_state",
-        "device_class": None,
-        "expire_after": 0,
-        "force_update": False,
-        "icon": None,
-        "unit": None,
-        "sub_mqtt_topic": "dpc-peak/state",
-        "rates": ["DPC"],
-    },
-    "dpc_next_peak_start": {
-        "name": "Next peak start",
-        "data_source": "contract.peak_handler.next_peak.start_date",
-        "device_class": "timestamp",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:clock-start",
-        "sub_mqtt_topic": "dpc-peak/next/peak",
-        "rates": ["DPC"],
-    },
-    "dpc_next_peak_end": {
-        "name": "Next peak end",
-        "data_source": "contract.peak_handler.next_peak.end_date",
-        "device_class": "timestamp",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:clock-end",
-        "sub_mqtt_topic": "dpc-peak/next/peak",
-        "rates": ["DPC"],
-    },
-    "dpc_next_pre_heat_start": {
-        "name": "Next Pre-heat start",
-        "data_source": "contract.peak_handler.next_peak.preheat.start_date",
-        "device_class": "timestamp",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:clock-start",
-        "sub_mqtt_topic": "dpc-peak/state",
-        "rates": ["DPC"],
-    },
-    "dpc_critical_hours_count": {
-        "name": "Number of critical hours",
-        "data_source": "contract.critical_called_hours",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:clock-alert-outline",
-        "sub_mqtt_topic": "dpc-peak/state",
-        "rates": ["DPC"],
-        "attributes": {
-            "max": "contract.max_critical_called_hours",
-        },
-    },
-    "dpc_winter_days_count": {
-        "name": "Number of winter days",
-        "data_source": "contract.winter_total_days_last_update",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:calendar-range-outline",
-        "sub_mqtt_topic": "dpc-peak/state",
-        "rates": ["DPC"],
-        "attributes": {
-            "max": "contract.winter_total_days",
-        },
-    },
-    # Winter credits
-    "wc_state": {
-        "name": "Current WC period detail",
-        "data_source": "contract.peak_handler.current_state",
-        "device_class": None,
-        "expire_after": 0,
-        "force_update": False,
-        "icon": None,
-        "unit": None,
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_cumulated_credit": {
-        "name": "Cumulated winter credit",
-        "data_source": "contract.peak_handler.cumulated_credit",
-        "device_class": "monetary",
-        "state_class": "total",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:currency-usd",
-        "unit": "CAD",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_projected_cumulated_credit": {
-        "name": "Projected cumulated winter credit",
-        "data_source": "contract.peak_handler.projected_cumulated_credit",
-        "device_class": "monetary",
-        "state_class": "total",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:currency-usd",
-        "unit": "CAD",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_next_anchor_start": {
-        "name": "Next anchor start",
-        "data_source": "contract.peak_handler.next_peak.anchor.start_date",
-        "device_class": "timestamp",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:clock-start",
-        "sub_mqtt_topic": "wintercredits/next/anchor",
-        "rates": ["DCPC"],
-        "attributes": {
-            "critical": "contract.peak_handler.next_peak.is_critical",
-        },
-    },
-    "wc_next_anchor_end": {
-        "name": "Next anchor end",
-        "data_source": "contract.peak_handler.next_peak.anchor.end_date",
-        "device_class": "timestamp",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:clock-end",
-        "sub_mqtt_topic": "wintercredits/next/anchor",
-        "rates": ["DCPC"],
-        "attributes": {
-            "critical": "contract.peak_handler.next_peak.is_critical",
-        },
-    },
-    "wc_next_peak_start": {
-        "name": "Next peak start",
-        "data_source": "contract.peak_handler.next_peak.start_date",
-        "device_class": "timestamp",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:clock-start",
-        "sub_mqtt_topic": "wintercredits/next/peak",
-        "rates": ["DCPC"],
-        "attributes": {
-            "critical": "contract.peak_handler.next_peak.is_critical",
-        },
-    },
-    "wc_next_peak_end": {
-        "name": "Next peak end",
-        "data_source": "contract.peak_handler.next_peak.end_date",
-        "device_class": "timestamp",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:clock-end",
-        "sub_mqtt_topic": "wintercredits/next/peak",
-        "rates": ["DCPC"],
-        "attributes": {
-            "critical": "contract.peak_handler.next_peak.is_critical",
-        },
-    },
-    "wc_next_critical_peak_start": {
-        "name": "Next critical peak start",
-        "data_source": "contract.peak_handler.next_critical_peak.start_date",
-        "device_class": "timestamp",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:clock-start",
-        "sub_mqtt_topic": "wintercredits/next/critical",
-        "rates": ["DCPC"],
-    },
-    "wc_next_critical_peak_end": {
-        "name": "Next critical peak end",
-        "data_source": "contract.peak_handler.next_critical_peak.end_date",
-        "device_class": "timestamp",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:clock-end",
-        "sub_mqtt_topic": "wintercredits/next/critical",
-        "rates": ["DCPC"],
-    },
-    "wc_next_pre_heat_start": {
-        "name": "Next Pre-heat start",
-        "data_source": "contract.peak_handler.next_peak.preheat.start_date",
-        "device_class": "timestamp",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:clock-start",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-        "attributes": {
-            "critical": "contract.peak_handler.next_peak.is_critical",
-        },
-    },
-    # Yesterday
-    "wc_yesterday_morning_peak_credit": {
-        "name": "Yesterday morning peak saved credit",
-        "data_source": "contract.peak_handler.yesterday_morning_peak.credit",
-        "device_class": "monetary",
-        "state_class": "total",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:currency-usd",
-        "unit": "CAD",
-        "sub_mqtt_topic": "wintercredits/yesterday",
-        "rates": ["DCPC"],
-    },
-    "wc_yesterday_morning_peak_actual_consumption": {
-        "name": "Yesterday morning peak actual consumption",
-        "data_source": "contract.peak_handler.yesterday_morning_peak.actual_consumption",
-        "device_class": "energy",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:home-lightning-bolt",
-        "unit": "kWh",
-        "sub_mqtt_topic": "wintercredits/yesterday",
-        "rates": ["DCPC"],
-    },
-    "wc_yesterday_morning_peak_ref_consumption": {
-        "name": "Yesterday morning peak reference consumption",
-        "data_source": "contract.peak_handler.yesterday_morning_peak.ref_consumption",
-        "device_class": "energy",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:home-lightning-bolt",
-        "unit": "kWh",
-        "sub_mqtt_topic": "wintercredits/yesterday",
-        "rates": ["DCPC"],
-    },
-    "wc_yesterday_morning_peak_saved_consumption": {
-        "name": "Yesterday morning peak saved consumption",
-        "data_source": "contract.peak_handler.yesterday_morning_peak.saved_consumption",
-        "device_class": "energy",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:home-lightning-bolt",
-        "unit": "kWh",
-        "sub_mqtt_topic": "wintercredits/yesterday",
-        "rates": ["DCPC"],
-    },
-    "wc_yesterday_evening_peak_credit": {
-        "name": "Yesterday evening peak saved credit",
-        "data_source": "contract.peak_handler.yesterday_evening_peak.credit",
-        "device_class": "monetary",
-        "state_class": "total",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:currency-usd",
-        "unit": "CAD",
-        "sub_mqtt_topic": "wintercredits/yesterday",
-        "rates": ["DCPC"],
-    },
-    "wc_yesterday_evening_peak_actual_consumption": {
-        "name": "Yesterday evening peak actual consumption",
-        "data_source": "contract.peak_handler.yesterday_evening_peak.actual_consumption",
-        "device_class": "energy",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:home-lightning-bolt",
-        "unit": "kWh",
-        "sub_mqtt_topic": "wintercredits/yesterday",
-        "rates": ["DCPC"],
-    },
-    "wc_yesterday_evening_peak_ref_consumption": {
-        "name": "Yesterday evening peak reference consumption",
-        "data_source": "contract.peak_handler.yesterday_evening_peak.ref_consumption",
-        "device_class": "energy",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:home-lightning-bolt",
-        "unit": "kWh",
-        "sub_mqtt_topic": "wintercredits/yesterday",
-        "rates": ["DCPC"],
-    },
-    "wc_yesterday_evening_peak_saved_consumption": {
-        "name": "Yesterday evening peak saved consumption",
-        "data_source": "contract.peak_handler.yesterday_evening_peak.saved_consumption",
-        "device_class": "energy",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:home-lightning-bolt",
-        "unit": "kWh",
-        "sub_mqtt_topic": "wintercredits/yesterday",
-        "rates": ["DCPC"],
-    },
-}
-BINARY_SENSORS: dict[
-    str, BinarySensorType
-] = {  # pylint: disable=consider-using-namedtuple-or-dataclass
-    # HydroQuebec
-    "hydroquebec_website_status": {
-        "name": "HydroQuebec website status",
-        "data_source": "self._hydro_is_up",
-        "device_class": "connectivity",
-        "expire_after": 0,
-        "force_update": False,
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    # Contracts
-    "current_period_epp_enabled": {
-        "name": "Current period epp enabled",
-        "data_source": "contract.cp_epp_enabled",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:code-equal",
-        "sub_mqtt_topic": "contract/state",
-        "rates": ["ALL"],
-    },
-    # Winter credits
-    "wc_critical": {
-        # == wc_next_peak_critical
-        "name": "Critical",
-        "data_source": "contract.peak_handler.next_peak.is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:flash-alert",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_critical_peak_in_progress": {
-        "name": "Critical peak in progress",
-        "data_source": "contract.peak_handler.current_peak_is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:flash-alert",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_pre_heat": {
-        "name": "Pre-heat In Progress",
-        "data_source": "contract.peak_handler.preheat_in_progress",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:flash-alert",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_next_anchor_critical": {
-        "name": "Next Anchor Period Critical",
-        # Est-ce que la période d'ancrage à venir est lié à une pointe critique"
-        "data_source": "contract.peak_handler.next_anchor.is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:flash-alert",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_next_peak_critical": {
-        # == wc_critical
-        # Est-ce que la prochaine période de pointe est critique true/false
-        "name": "Next Peak Period Critical",
-        "data_source": "contract.peak_handler.next_peak.is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:flash-alert",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_upcoming_critical_peak": {
-        # True si au moins un peaks donnés par l'API d'hydroQuebec n'est pas encore terminé
-        "name": "Upcoming Critical Peak",
-        "data_source": "contract.peak_handler.is_any_critical_peak_coming",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:flash-alert",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_critical_morning_peak_today": {
-        "name": "Critical Morning Peak Today",
-        "data_source": "contract.peak_handler.today_morning_peak.is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:message-flash",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_critical_evening_peak_today": {
-        "name": "Critical Evening Peak Today",
-        "data_source": "contract.peak_handler.today_evening_peak.is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:message-flash",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_critical_morning_peak_tomorrow": {
-        "name": "Critical Morning Peak tomorrow",
-        "data_source": "contract.peak_handler.tomorrow_morning_peak.is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:message-flash",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    "wc_critical_evening_peak_tomorrow": {
-        "name": "Critical Evening Peak tomorrow",
-        "data_source": "contract.peak_handler.tomorrow_evening_peak.is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:message-flash",
-        "sub_mqtt_topic": "wintercredits/state",
-        "rates": ["DCPC"],
-    },
-    # DPC
-    "dpc_pre_heat": {
-        "name": "Pre-heat In Progress",
-        "data_source": "contract.peak_handler.preheat_in_progress",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:flash-alert",
-        "sub_mqtt_topic": "dpc-peak/state",
-        "rates": ["DPC"],
-    },
-    "dpc_peak_in_progress": {
-        "name": "Critical peak in progress",
-        "data_source": "contract.peak_handler.peak_in_progress",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:flash-alert",
-        "sub_mqtt_topic": "dpc-peak/state",
-        "rates": ["DPC"],
-    },
-    "dpc_critical_morning_peak_today": {
-        "name": "Critical Morning Peak Today",
-        "data_source": "contract.peak_handler.today_morning_peak.is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:message-flash",
-        "sub_mqtt_topic": "dpc-peak/state",
-        "rates": ["DPC"],
-    },
-    "dpc_critical_evening_peak_today": {
-        "name": "Critical Evening Peak Today",
-        "data_source": "contract.peak_handler.today_evening_peak.is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:message-flash",
-        "sub_mqtt_topic": "dpc-peak/state",
-        "rates": ["DPC"],
-    },
-    "dpc_critical_morning_peak_tomorrow": {
-        "name": "Critical Morning Peak tomorrow",
-        "data_source": "contract.peak_handler.tomorrow_morning_peak.is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:message-flash",
-        "sub_mqtt_topic": "dpc-peak/state",
-        "rates": ["DPC"],
-    },
-    "dpc_critical_evening_peak_tomorrow": {
-        "name": "Critical Evening Peak tomorrow",
-        "data_source": "contract.peak_handler.tomorrow_evening_peak.is_critical",
-        "expire_after": 0,
-        "force_update": False,
-        "icon": "mdi:message-flash",
-        "sub_mqtt_topic": "dpc-peak/state",
-        "rates": ["DPC"],
-    },
-}
+SENSORS: dict[str, SensorType] = (
+    {  # pylint: disable=consider-using-namedtuple-or-dataclass
+        # Account
+        "balance": {
+            "name": "Balance",
+            "data_source": "account.balance",
+            "device_class": "monetary",
+            "state_class": "total",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:currency-usd",
+            "unit": "CAD",
+            "sub_mqtt_topic": "account/state",
+            "rates": ["ALL"],
+        },
+        # Contract
+        "outage": {
+            "name": "Next or current outage",
+            "data_source": "contract.next_outage.start_date",
+            "device_class": "timestamp",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:calendar-start",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+            "attributes": {
+                "end_date": "contract.next_outage.end_date",
+                "cause": "contract.next_outage.cause.name",
+                "planned_duration": "contract.next_outage.planned_duration",
+                "code": "contract.next_outage.code.name",
+                "state": "contract.next_outage.status.name",
+                "emergency_level": "contract.next_outage.emergency_level",
+                "is_planned": "contract.next_outage.is_planned",
+            },
+        },
+        "current_billing_period_current_day": {
+            "name": "Current billing period current day",
+            "data_source": "contract.cp_current_day",
+            "device_class": None,
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:calendar-start",
+            "state_class": "measurement",
+            "unit": "days",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        "current_billing_period_duration": {
+            "name": "Current billing period duration",
+            "data_source": "contract.cp_duration",
+            "device_class": None,
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:calendar-expand-horizontal",
+            "state_class": "measurement",
+            "unit": "days",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        "current_billing_period_total_to_date": {
+            "name": "Current billing period total to date",
+            "data_source": "contract.cp_current_bill",
+            "device_class": "monetary",
+            "state_class": "total",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:currency-usd",
+            "unit": "CAD",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        "current_billing_period_projected_bill": {
+            "name": "Current billing period projected bill",
+            "data_source": "contract.cp_projected_bill",
+            "device_class": "monetary",
+            "state_class": "total",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:currency-usd",
+            "unit": "CAD",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        "current_billing_period_daily_bill_mean": {
+            "name": "Current billing period daily bill mean",
+            "data_source": "contract.cp_daily_bill_mean",
+            "device_class": "monetary",
+            "state_class": "total",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:currency-usd",
+            "unit": "CAD",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        "current_billing_period_daily_consumption_mean": {
+            "name": "Current billing period daily consumption mean",
+            "data_source": "contract.cp_daily_consumption_mean",
+            "device_class": "energy",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:home-lightning-bolt",
+            "unit": "kWh",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        "current_billing_period_total_consumption": {
+            "name": "Current billing period total consumption",
+            "data_source": "contract.cp_total_consumption",
+            "device_class": "energy",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:home-lightning-bolt",
+            "state_class": "total_increasing",
+            "unit": "kWh",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        "current_billing_period_projected_total_consumption": {
+            "name": "Current billing period projected total consumption",
+            "data_source": "contract.cp_projected_total_consumption",
+            "device_class": "energy",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:home-lightning-bolt",
+            "unit": "kWh",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        "current_billing_period_average_temperature": {
+            "name": "Current billing period average temperature",
+            "data_source": "contract.cp_average_temperature",
+            "device_class": "temperature",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:thermometer",
+            "state_class": "measurement",
+            "unit": "°C",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        "current_billing_period_kwh_cost_mean": {
+            "name": "Current billing period kwh cost mean",
+            "data_source": "contract.cp_kwh_cost_mean",
+            "device_class": "monetary",
+            "state_class": "total",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:currency-usd",
+            "unit": "CAD/kWh",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        "current_billing_period_rate": {
+            "name": "Current billing period rate",
+            "data_source": "contract.rate",
+            "device_class": None,
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:playlist-check",
+            "state_class": None,
+            "unit": None,
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        "current_billing_period_rate_option": {
+            "name": "Current billing period rate option",
+            "data_source": "contract.rate_option",
+            "device_class": None,
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:playlist-star",
+            "state_class": None,
+            "unit": None,
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        # FlexD and DT (identical for now...)
+        "current_billing_period_higher_price_consumption": {
+            "name": "Current billing period higher price consumption",
+            "data_source": "contract.cp_higher_price_consumption",
+            "device_class": "energy",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:home-lightning-bolt",
+            "unit": "kWh",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["DT", "DPC"],
+        },
+        "current_billing_period_lower_price_consumption": {
+            "name": "Current billing period lower price consumption",
+            "data_source": "contract.cp_lower_price_consumption",
+            "device_class": "energy",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:home-lightning-bolt-outline",
+            "unit": "kWh",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["DT", "DPC"],
+        },
+        "amount_saved_vs_base_rate": {
+            "name": "Net saving/loss vs rate D",
+            "data_source": "contract.amount_saved_vs_base_rate",
+            "device_class": "monetary",
+            "state_class": "total",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:currency-usd",
+            "unit": "CAD",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["DT", "DPC"],
+        },
+        # FlexD
+        "dpc_state": {
+            "name": "Current DPC period detail",
+            "data_source": "contract.peak_handler.current_state",
+            "device_class": None,
+            "expire_after": 0,
+            "force_update": False,
+            "icon": None,
+            "unit": None,
+            "sub_mqtt_topic": "dpc-peak/state",
+            "rates": ["DPC"],
+        },
+        "dpc_next_peak_start": {
+            "name": "Next peak start",
+            "data_source": "contract.peak_handler.next_peak.start_date",
+            "device_class": "timestamp",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:clock-start",
+            "sub_mqtt_topic": "dpc-peak/next/peak",
+            "rates": ["DPC"],
+        },
+        "dpc_next_peak_end": {
+            "name": "Next peak end",
+            "data_source": "contract.peak_handler.next_peak.end_date",
+            "device_class": "timestamp",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:clock-end",
+            "sub_mqtt_topic": "dpc-peak/next/peak",
+            "rates": ["DPC"],
+        },
+        "dpc_next_pre_heat_start": {
+            "name": "Next Pre-heat start",
+            "data_source": "contract.peak_handler.next_peak.preheat.start_date",
+            "device_class": "timestamp",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:clock-start",
+            "sub_mqtt_topic": "dpc-peak/state",
+            "rates": ["DPC"],
+        },
+        "dpc_critical_hours_count": {
+            "name": "Number of critical hours",
+            "data_source": "contract.critical_called_hours",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:clock-alert-outline",
+            "sub_mqtt_topic": "dpc-peak/state",
+            "rates": ["DPC"],
+            "attributes": {
+                "max": "contract.max_critical_called_hours",
+            },
+        },
+        "dpc_winter_days_count": {
+            "name": "Number of winter days",
+            "data_source": "contract.winter_total_days_last_update",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:calendar-range-outline",
+            "sub_mqtt_topic": "dpc-peak/state",
+            "rates": ["DPC"],
+            "attributes": {
+                "max": "contract.winter_total_days",
+            },
+        },
+        # Winter credits
+        "wc_state": {
+            "name": "Current WC period detail",
+            "data_source": "contract.peak_handler.current_state",
+            "device_class": None,
+            "expire_after": 0,
+            "force_update": False,
+            "icon": None,
+            "unit": None,
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_cumulated_credit": {
+            "name": "Cumulated winter credit",
+            "data_source": "contract.peak_handler.cumulated_credit",
+            "device_class": "monetary",
+            "state_class": "total",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:currency-usd",
+            "unit": "CAD",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_projected_cumulated_credit": {
+            "name": "Projected cumulated winter credit",
+            "data_source": "contract.peak_handler.projected_cumulated_credit",
+            "device_class": "monetary",
+            "state_class": "total",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:currency-usd",
+            "unit": "CAD",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_next_anchor_start": {
+            "name": "Next anchor start",
+            "data_source": "contract.peak_handler.next_peak.anchor.start_date",
+            "device_class": "timestamp",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:clock-start",
+            "sub_mqtt_topic": "wintercredits/next/anchor",
+            "rates": ["DCPC"],
+            "attributes": {
+                "critical": "contract.peak_handler.next_peak.is_critical",
+            },
+        },
+        "wc_next_anchor_end": {
+            "name": "Next anchor end",
+            "data_source": "contract.peak_handler.next_peak.anchor.end_date",
+            "device_class": "timestamp",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:clock-end",
+            "sub_mqtt_topic": "wintercredits/next/anchor",
+            "rates": ["DCPC"],
+            "attributes": {
+                "critical": "contract.peak_handler.next_peak.is_critical",
+            },
+        },
+        "wc_next_peak_start": {
+            "name": "Next peak start",
+            "data_source": "contract.peak_handler.next_peak.start_date",
+            "device_class": "timestamp",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:clock-start",
+            "sub_mqtt_topic": "wintercredits/next/peak",
+            "rates": ["DCPC"],
+            "attributes": {
+                "critical": "contract.peak_handler.next_peak.is_critical",
+            },
+        },
+        "wc_next_peak_end": {
+            "name": "Next peak end",
+            "data_source": "contract.peak_handler.next_peak.end_date",
+            "device_class": "timestamp",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:clock-end",
+            "sub_mqtt_topic": "wintercredits/next/peak",
+            "rates": ["DCPC"],
+            "attributes": {
+                "critical": "contract.peak_handler.next_peak.is_critical",
+            },
+        },
+        "wc_next_critical_peak_start": {
+            "name": "Next critical peak start",
+            "data_source": "contract.peak_handler.next_critical_peak.start_date",
+            "device_class": "timestamp",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:clock-start",
+            "sub_mqtt_topic": "wintercredits/next/critical",
+            "rates": ["DCPC"],
+        },
+        "wc_next_critical_peak_end": {
+            "name": "Next critical peak end",
+            "data_source": "contract.peak_handler.next_critical_peak.end_date",
+            "device_class": "timestamp",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:clock-end",
+            "sub_mqtt_topic": "wintercredits/next/critical",
+            "rates": ["DCPC"],
+        },
+        "wc_next_pre_heat_start": {
+            "name": "Next Pre-heat start",
+            "data_source": "contract.peak_handler.next_peak.preheat.start_date",
+            "device_class": "timestamp",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:clock-start",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+            "attributes": {
+                "critical": "contract.peak_handler.next_peak.is_critical",
+            },
+        },
+        # Yesterday
+        "wc_yesterday_morning_peak_credit": {
+            "name": "Yesterday morning peak saved credit",
+            "data_source": "contract.peak_handler.yesterday_morning_peak.credit",
+            "device_class": "monetary",
+            "state_class": "total",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:currency-usd",
+            "unit": "CAD",
+            "sub_mqtt_topic": "wintercredits/yesterday",
+            "rates": ["DCPC"],
+        },
+        "wc_yesterday_morning_peak_actual_consumption": {
+            "name": "Yesterday morning peak actual consumption",
+            "data_source": "contract.peak_handler.yesterday_morning_peak.actual_consumption",
+            "device_class": "energy",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:home-lightning-bolt",
+            "unit": "kWh",
+            "sub_mqtt_topic": "wintercredits/yesterday",
+            "rates": ["DCPC"],
+        },
+        "wc_yesterday_morning_peak_ref_consumption": {
+            "name": "Yesterday morning peak reference consumption",
+            "data_source": "contract.peak_handler.yesterday_morning_peak.ref_consumption",
+            "device_class": "energy",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:home-lightning-bolt",
+            "unit": "kWh",
+            "sub_mqtt_topic": "wintercredits/yesterday",
+            "rates": ["DCPC"],
+        },
+        "wc_yesterday_morning_peak_saved_consumption": {
+            "name": "Yesterday morning peak saved consumption",
+            "data_source": "contract.peak_handler.yesterday_morning_peak.saved_consumption",
+            "device_class": "energy",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:home-lightning-bolt",
+            "unit": "kWh",
+            "sub_mqtt_topic": "wintercredits/yesterday",
+            "rates": ["DCPC"],
+        },
+        "wc_yesterday_evening_peak_credit": {
+            "name": "Yesterday evening peak saved credit",
+            "data_source": "contract.peak_handler.yesterday_evening_peak.credit",
+            "device_class": "monetary",
+            "state_class": "total",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:currency-usd",
+            "unit": "CAD",
+            "sub_mqtt_topic": "wintercredits/yesterday",
+            "rates": ["DCPC"],
+        },
+        "wc_yesterday_evening_peak_actual_consumption": {
+            "name": "Yesterday evening peak actual consumption",
+            "data_source": "contract.peak_handler.yesterday_evening_peak.actual_consumption",
+            "device_class": "energy",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:home-lightning-bolt",
+            "unit": "kWh",
+            "sub_mqtt_topic": "wintercredits/yesterday",
+            "rates": ["DCPC"],
+        },
+        "wc_yesterday_evening_peak_ref_consumption": {
+            "name": "Yesterday evening peak reference consumption",
+            "data_source": "contract.peak_handler.yesterday_evening_peak.ref_consumption",
+            "device_class": "energy",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:home-lightning-bolt",
+            "unit": "kWh",
+            "sub_mqtt_topic": "wintercredits/yesterday",
+            "rates": ["DCPC"],
+        },
+        "wc_yesterday_evening_peak_saved_consumption": {
+            "name": "Yesterday evening peak saved consumption",
+            "data_source": "contract.peak_handler.yesterday_evening_peak.saved_consumption",
+            "device_class": "energy",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:home-lightning-bolt",
+            "unit": "kWh",
+            "sub_mqtt_topic": "wintercredits/yesterday",
+            "rates": ["DCPC"],
+        },
+    }
+)
+BINARY_SENSORS: dict[str, BinarySensorType] = (
+    {  # pylint: disable=consider-using-namedtuple-or-dataclass
+        # HydroQuebec
+        "hydroquebec_website_status": {
+            "name": "HydroQuebec website status",
+            "data_source": "self._hydro_is_up",
+            "device_class": "connectivity",
+            "expire_after": 0,
+            "force_update": False,
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        # Contracts
+        "current_period_epp_enabled": {
+            "name": "Current period epp enabled",
+            "data_source": "contract.cp_epp_enabled",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:code-equal",
+            "sub_mqtt_topic": "contract/state",
+            "rates": ["ALL"],
+        },
+        # Winter credits
+        "wc_critical": {
+            # == wc_next_peak_critical
+            "name": "Critical",
+            "data_source": "contract.peak_handler.next_peak.is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:flash-alert",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_critical_peak_in_progress": {
+            "name": "Critical peak in progress",
+            "data_source": "contract.peak_handler.current_peak_is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:flash-alert",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_pre_heat": {
+            "name": "Pre-heat In Progress",
+            "data_source": "contract.peak_handler.preheat_in_progress",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:flash-alert",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_next_anchor_critical": {
+            "name": "Next Anchor Period Critical",
+            # Est-ce que la période d'ancrage à venir est lié à une pointe critique"
+            "data_source": "contract.peak_handler.next_anchor.is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:flash-alert",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_next_peak_critical": {
+            # == wc_critical
+            # Est-ce que la prochaine période de pointe est critique true/false
+            "name": "Next Peak Period Critical",
+            "data_source": "contract.peak_handler.next_peak.is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:flash-alert",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_upcoming_critical_peak": {
+            # True si au moins un peaks donnés par l'API d'hydroQuebec n'est pas encore terminé
+            "name": "Upcoming Critical Peak",
+            "data_source": "contract.peak_handler.is_any_critical_peak_coming",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:flash-alert",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_critical_morning_peak_today": {
+            "name": "Critical Morning Peak Today",
+            "data_source": "contract.peak_handler.today_morning_peak.is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:message-flash",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_critical_evening_peak_today": {
+            "name": "Critical Evening Peak Today",
+            "data_source": "contract.peak_handler.today_evening_peak.is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:message-flash",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_critical_morning_peak_tomorrow": {
+            "name": "Critical Morning Peak tomorrow",
+            "data_source": "contract.peak_handler.tomorrow_morning_peak.is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:message-flash",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        "wc_critical_evening_peak_tomorrow": {
+            "name": "Critical Evening Peak tomorrow",
+            "data_source": "contract.peak_handler.tomorrow_evening_peak.is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:message-flash",
+            "sub_mqtt_topic": "wintercredits/state",
+            "rates": ["DCPC"],
+        },
+        # DPC
+        "dpc_pre_heat": {
+            "name": "Pre-heat In Progress",
+            "data_source": "contract.peak_handler.preheat_in_progress",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:flash-alert",
+            "sub_mqtt_topic": "dpc-peak/state",
+            "rates": ["DPC"],
+        },
+        "dpc_peak_in_progress": {
+            "name": "Critical peak in progress",
+            "data_source": "contract.peak_handler.peak_in_progress",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:flash-alert",
+            "sub_mqtt_topic": "dpc-peak/state",
+            "rates": ["DPC"],
+        },
+        "dpc_critical_morning_peak_today": {
+            "name": "Critical Morning Peak Today",
+            "data_source": "contract.peak_handler.today_morning_peak.is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:message-flash",
+            "sub_mqtt_topic": "dpc-peak/state",
+            "rates": ["DPC"],
+        },
+        "dpc_critical_evening_peak_today": {
+            "name": "Critical Evening Peak Today",
+            "data_source": "contract.peak_handler.today_evening_peak.is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:message-flash",
+            "sub_mqtt_topic": "dpc-peak/state",
+            "rates": ["DPC"],
+        },
+        "dpc_critical_morning_peak_tomorrow": {
+            "name": "Critical Morning Peak tomorrow",
+            "data_source": "contract.peak_handler.tomorrow_morning_peak.is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:message-flash",
+            "sub_mqtt_topic": "dpc-peak/state",
+            "rates": ["DPC"],
+        },
+        "dpc_critical_evening_peak_tomorrow": {
+            "name": "Critical Evening Peak tomorrow",
+            "data_source": "contract.peak_handler.tomorrow_evening_peak.is_critical",
+            "expire_after": 0,
+            "force_update": False,
+            "icon": "mdi:message-flash",
+            "sub_mqtt_topic": "dpc-peak/state",
+            "rates": ["DPC"],
+        },
+    }
+)
```

### Comparing `hydroqc2mqtt-1.2.0/hydroqc2mqtt.egg-info/PKG-INFO` & `hydroqc2mqtt-1.3.0/hydroqc2mqtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: hydroqc2mqtt
-Version: 1.2.0
+Version: 1.3.0
 Summary: Daemon managing hydroqc sensors through MQTT
 Home-page: https://hydroqc.ca
 Author-email: Hydroqc Team <info@hydroqc.ca>
 License: AGPL-3.0-or-later
 Project-URL: Source Code, https://gitlab.com/hydroqc/hydroqc2mqtt
 Project-URL: Bug Reports, https://gitlab.com/hydroqc/hydroqc2mqtt/-/issues
 Project-URL: Home-page, https://hydroqc.ca
 Keywords: hydro-quebec,mqtt,homeassistant,hydroqc
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.0
+Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mqtt-hass-base==4.2.5
-Requires-Dist: Hydro_Quebec_API_Wrapper==3.1.3
-Requires-Dist: python_dateutil==2.8.2
-Requires-Dist: packaging==23.2
-Requires-Dist: pytz==2023.3.post1
+Requires-Dist: mqtt-hass-base==4.3.0
+Requires-Dist: Hydro_Quebec_API_Wrapper==3.2.0
+Requires-Dist: python_dateutil==2.9.0.post0
+Requires-Dist: packaging==24.0
+Requires-Dist: pytz==2024.1
 Requires-Dist: homeassistant
 Requires-Dist: charset-normalizer==3.3.2
 
 # hydroqc2mqtt
 
 **The full updated project documentation can be found at [https://hydroqc.ca](https://hydroqc.ca)**
```

### Comparing `hydroqc2mqtt-1.2.0/hydroqc2mqtt.egg-info/SOURCES.txt` & `hydroqc2mqtt-1.3.0/hydroqc2mqtt.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 .dockerignore
+.env.sample
 .flake8
 .gitignore
+.gitlab-ci-local-env.sample
+.gitlab-ci-local-variables.sample.yml
 .gitlab-ci.yml
 .pre-commit-config.yaml
 .pylintrc
 .pypirc
 Dockerfile
 LICENSE
 README.md
```

### Comparing `hydroqc2mqtt-1.2.0/hydroqc2mqtt.svg` & `hydroqc2mqtt-1.3.0/hydroqc2mqtt.svg`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/pyproject.toml` & `hydroqc2mqtt-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-    "setuptools==69.0.3",
-    "setuptools_scm[toml]==8.0.4",
-    "wheel==0.42.0",
+    "setuptools==69.5.1",
+    "setuptools_scm[toml]==8.1.0",
+    "wheel==0.43.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hydroqc2mqtt"
 dynamic = ["version", "dependencies"]
 description = "Daemon managing hydroqc sensors through MQTT"
@@ -18,15 +18,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["hydro-quebec", "mqtt", "homeassistant", "hydroqc"]
 
-requires-python = ">=3.10.0"
+requires-python = ">=3.12.0"
 # https://github.com/renovatebot/renovate/issues/10187
 #dependencies    = [
 #    "mqtt-hass-base==4.0.13",
 #    "Hydro_Quebec_API_Wrapper==0.6.5",
 #    "python_dateutil==2.8.2",
 #    "packaging==21.3",
 ## The following lines should not be there
```

### Comparing `hydroqc2mqtt-1.2.0/renovate.json5` & `hydroqc2mqtt-1.3.0/renovate.json5`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7492559523809523%*

 * *Differences: {"'packageRules'": "{6: {'automergeType': 'branch'}}",*

 * * "'platformAutomerge'": 'True',*

 * * 'delete': "['platform']"}*

```diff
@@ -145,23 +145,23 @@
             ],
             "matchUpdateTypes": [
                 "major"
             ]
         },
         {
             "automerge": true,
-            "automergeType": "pr",
+            "automergeType": "branch",
             "description": "Auto merge container digests",
             "ignoreTests": false,
             "matchDatasources": [
                 "docker"
             ],
             "matchUpdateTypes": [
                 "digest"
             ]
         }
     ],
-    "platform": "gitlab",
+    "platformAutomerge": true,
     "pre-commit": {
         "enabled": true
     }
 }
```

### Comparing `hydroqc2mqtt-1.2.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/config` & `hydroqc2mqtt-1.3.0/tests/expected_mqtt_data/homeassistant/sensor/4444444444-balance/config`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/tests/input_http_data/contrats.json` & `hydroqc2mqtt-1.3.0/tests/input_http_data/contrats.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/tests/input_http_data/creditPointeCritique.json` & `hydroqc2mqtt-1.3.0/tests/input_http_data/creditPointeCritique.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/tests/input_http_data/infoCompte.json` & `hydroqc2mqtt-1.3.0/tests/input_http_data/infoCompte.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/tests/input_http_data/outages.json` & `hydroqc2mqtt-1.3.0/tests/input_http_data/outages.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/tests/input_http_data/relations.json` & `hydroqc2mqtt-1.3.0/tests/input_http_data/relations.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/tests/input_http_data/resourceObtenirDonneesConsommationHoraires.json` & `hydroqc2mqtt-1.3.0/tests/input_http_data/resourceObtenirDonneesConsommationHoraires.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/tests/input_http_data/resourceObtenirDonneesPeriodesConsommation.json` & `hydroqc2mqtt-1.3.0/tests/input_http_data/resourceObtenirDonneesPeriodesConsommation.json`

 * *Files identical despite different names*

### Comparing `hydroqc2mqtt-1.2.0/tests/test_base.py` & `hydroqc2mqtt-1.3.0/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base tests for hydroqc2mqtt."""
+
 import base64
 import json
 import os
 import re
 import sys
 import time
 from typing import Any
```

### Comparing `hydroqc2mqtt-1.2.0/tests/test_base_sync_comsumption.py` & `hydroqc2mqtt-1.3.0/tests/test_base_sync_comsumption.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base tests for hydroqc2mqtt."""
+
 import asyncio
 import base64
 import copy
 import json
 
 # import logging
 import os
```

### Comparing `hydroqc2mqtt-1.2.0/tests/test_base_sync_comsumption_history.py` & `hydroqc2mqtt-1.3.0/tests/test_base_sync_comsumption_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base tests for hydroqc2mqtt."""
+
 import asyncio
 import base64
 import json
 import os
 import re
 import sys
 import time
```

### Comparing `hydroqc2mqtt-1.2.0/tox.ini` & `hydroqc2mqtt-1.3.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = pylint,flake8,pydocstyle,mypy,black,cov-init,py311,cov-report
+envlist = pylint,flake8,pydocstyle,mypy,black,cov-init,py312,cov-report
 skip_missing_interpreters = True
 
 [testenv:pylint]
 basepython = {env:PYTHON3_PATH:python3}
 ignore_errors = True
 deps =
     -r {toxinidir}{/}test_requirements.txt
```

