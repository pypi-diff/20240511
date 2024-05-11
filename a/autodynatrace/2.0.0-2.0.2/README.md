# Comparing `tmp/autodynatrace-2.0.0.tar.gz` & `tmp/autodynatrace-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodynatrace-2.0.0.tar", last modified: Thu Jun 22 12:29:02 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `autodynatrace-2.0.0.tar` & `autodynatrace-2.0.2.tar`

### file list

```diff
@@ -1,104 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.559888 autodynatrace-2.0.0/
--rw-rw-rw-   0        0        0    13107 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     1185 2023-06-22 12:29:02.559888 autodynatrace-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3124 2023-04-06 14:05:33.000000 autodynatrace-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.494408 autodynatrace-2.0.0/autodynatrace/
--rw-rw-rw-   0        0        0     4062 2023-04-06 14:05:33.000000 autodynatrace-2.0.0/autodynatrace/__init__.py
--rw-rw-rw-   0        0        0      333 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/log.py
--rw-rw-rw-   0        0        0      545 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/sdk.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.494408 autodynatrace-2.0.0/autodynatrace/wrappers/
--rw-rw-rw-   0        0        0        0 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.494408 autodynatrace-2.0.0/autodynatrace/wrappers/aiohttp/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/aiohttp/__init__.py
--rw-rw-rw-   0        0        0      963 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/aiohttp/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/bottle/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/bottle/__init__.py
--rw-rw-rw-   0        0        0     2090 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/bottle/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/celery/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/celery/__init__.py
--rw-rw-rw-   0        0        0     4582 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/celery/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/concurrent/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/concurrent/__init__.py
--rw-rw-rw-   0        0        0     1731 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/concurrent/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/confluent_kafka/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/confluent_kafka/__init__.py
--rw-rw-rw-   0        0        0     3644 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/confluent_kafka/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/custom/
--rw-rw-rw-   0        0        0       46 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/custom/__init__.py
--rw-rw-rw-   0        0        0     2558 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/custom/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/cx_Oracle/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/cx_Oracle/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-06 14:09:35.000000 autodynatrace-2.0.0/autodynatrace/wrappers/cx_Oracle/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/dbapi/
--rw-rw-rw-   0        0        0     2880 2023-06-22 00:20:35.000000 autodynatrace-2.0.0/autodynatrace/wrappers/dbapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.522048 autodynatrace-2.0.0/autodynatrace/wrappers/django/
--rw-rw-rw-   0        0        0      157 2023-03-24 23:29:36.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/__init__.py
--rw-rw-rw-   0        0        0      276 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/apps.py
--rw-rw-rw-   0        0        0     1878 2023-03-24 23:29:36.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/db.py
--rw-rw-rw-   0        0        0     3494 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/middlewares.py
--rw-rw-rw-   0        0        0     1788 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/utils.py
--rw-rw-rw-   0        0        0      889 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.525559 autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/__init__.py
--rw-rw-rw-   0        0        0     2443 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/middleware.py
--rw-rw-rw-   0        0        0     1359 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.525559 autodynatrace-2.0.0/autodynatrace/wrappers/flask/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/flask/__init__.py
--rw-rw-rw-   0        0        0     2612 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/flask/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.525559 autodynatrace-2.0.0/autodynatrace/wrappers/grpc/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/grpc/__init__.py
--rw-rw-rw-   0        0        0     2415 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/grpc/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.525559 autodynatrace-2.0.0/autodynatrace/wrappers/paramiko/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/paramiko/__init__.py
--rw-rw-rw-   0        0        0     1068 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/paramiko/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.535328 autodynatrace-2.0.0/autodynatrace/wrappers/pika/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pika/__init__.py
--rw-rw-rw-   0        0        0     3433 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pika/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.536996 autodynatrace-2.0.0/autodynatrace/wrappers/psycopg2/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/psycopg2/__init__.py
--rw-rw-rw-   0        0        0     2248 2023-06-22 12:06:15.000000 autodynatrace-2.0.0/autodynatrace/wrappers/psycopg2/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.539740 autodynatrace-2.0.0/autodynatrace/wrappers/pymongo/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pymongo/__init__.py
--rw-rw-rw-   0        0        0     2113 2023-04-06 14:09:35.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pymongo/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.541832 autodynatrace-2.0.0/autodynatrace/wrappers/pysnmp/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pysnmp/__init__.py
--rw-rw-rw-   0        0        0     4913 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pysnmp/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.544453 autodynatrace-2.0.0/autodynatrace/wrappers/redis/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/redis/__init__.py
--rw-rw-rw-   0        0        0      747 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/redis/utils.py
--rw-rw-rw-   0        0        0     2111 2023-04-06 14:09:48.000000 autodynatrace-2.0.0/autodynatrace/wrappers/redis/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.546513 autodynatrace-2.0.0/autodynatrace/wrappers/ruxit/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/ruxit/__init__.py
--rw-rw-rw-   0        0        0      475 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/ruxit/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.548057 autodynatrace-2.0.0/autodynatrace/wrappers/sqlalchemy/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/sqlalchemy/__init__.py
--rw-rw-rw-   0        0        0     4496 2023-04-06 14:09:58.000000 autodynatrace-2.0.0/autodynatrace/wrappers/sqlalchemy/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.550140 autodynatrace-2.0.0/autodynatrace/wrappers/starlette/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/starlette/__init__.py
--rw-rw-rw-   0        0        0     1459 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/starlette/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.551168 autodynatrace-2.0.0/autodynatrace/wrappers/subprocess/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/subprocess/__init__.py
--rw-rw-rw-   0        0        0     1401 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/subprocess/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.552903 autodynatrace-2.0.0/autodynatrace/wrappers/suds/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/suds/__init__.py
--rw-rw-rw-   0        0        0      715 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/suds/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.552903 autodynatrace-2.0.0/autodynatrace/wrappers/tornado/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/tornado/__init__.py
--rw-rw-rw-   0        0        0     1744 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/tornado/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.556930 autodynatrace-2.0.0/autodynatrace/wrappers/urllib/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/urllib/__init__.py
--rw-rw-rw-   0        0        0     1563 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/urllib/wrapper.py
--rw-rw-rw-   0        0        0      108 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.494408 autodynatrace-2.0.0/autodynatrace.egg-info/
--rw-rw-rw-   0        0        0     1185 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2781 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       61 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2023-06-22 12:29:02.559888 autodynatrace-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1596 2023-06-21 23:57:15.000000 autodynatrace-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.559888 autodynatrace-2.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     6901 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/tests/test_custom.py
--rw-rw-rw-   0        0        0     1365 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/tests/test_django.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/__about__.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/log.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/sdk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/utils.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/aiohttp/__init__.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/aiohttp/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/bottle/__init__.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/bottle/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/celery/__init__.py
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/celery/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/concurrent/__init__.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/concurrent/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/confluent_kafka/__init__.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/confluent_kafka/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/custom/__init__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/custom/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/cx_Oracle/__init__.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/cx_Oracle/wrapper.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/dbapi/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/django/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/django/apps.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/django/db.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/django/middlewares.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/django/utils.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/django/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/fastapi/__init__.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/fastapi/middleware.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/fastapi/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/flask/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/flask/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/grpc/__init__.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/grpc/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/paramiko/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/paramiko/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/pika/__init__.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/pika/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/psycopg2/__init__.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/psycopg2/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/pymongo/__init__.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/pymongo/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/pysnmp/__init__.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/pysnmp/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/redis/__init__.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/redis/utils.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/redis/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/ruxit/__init__.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/ruxit/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/sqlalchemy/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/starlette/__init__.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/starlette/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/subprocess/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/subprocess/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/suds/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/suds/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/tornado/__init__.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/tornado/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/urllib/__init__.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/autodynatrace/wrappers/urllib/wrapper.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/.gitignore
+-rw-r--r--   0        0        0    13107 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/LICENSE
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/README.md
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 autodynatrace-2.0.2/PKG-INFO
```

### Comparing `autodynatrace-2.0.0/LICENSE` & `autodynatrace-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/README.md` & `autodynatrace-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/__init__.py` & `autodynatrace-2.0.2/autodynatrace/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 import os
 import sys
 
 from wrapt.importer import when_imported
 
 from .log import init as log_init, logger
 from .sdk import init as sdk_init
-
-__version__ = 1.082
+from .__about__ import __version__
 
 dt_custom_prop = os.environ.get("DT_CUSTOM_PROP")
 if dt_custom_prop:
-    os.environ["DT_CUSTOM_PROP"] = "{} Autodynatrace={}".format(dt_custom_prop, __version__)
+    os.environ["DT_CUSTOM_PROP"] = "{} Autodynatrace={}".format(dt_custom_prop, reversed)
 else:
     os.environ["DT_CUSTOM_PROP"] = "Autodynatrace={}".format(__version__)
 
 
 log_level_name = os.environ.get("AUTODYNATRACE_LOG_LEVEL", "WARNING")
 log_init(logging.getLevelName(log_level_name))
```

### Comparing `autodynatrace-2.0.0/autodynatrace/sdk.py` & `autodynatrace-2.0.2/autodynatrace/sdk.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/aiohttp/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/aiohttp/wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def instrument():
     @wrapt.patch_function_wrapper("aiohttp.client", "ClientSession._request")
     async def dynatrace_request(wrapped, instance, args, kwargs):
 
         method = args[0]
-        url = args[1]
+        url = str(args[1])
         headers = dict(kwargs.get("headers", {}))
 
         with sdk.trace_outgoing_web_request(url, method, headers) as tracer:
             tag = tracer.outgoing_dynatrace_string_tag.decode()
             logger.debug("dynatrace - tracing {} '{}' with tag '{}'".format(method, url, tag))
             headers.update({DYNATRACE_HTTP_HEADER_NAME: tag})
             kwargs["headers"] = headers
```

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/bottle/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/bottle/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/celery/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/celery/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/concurrent/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/concurrent/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/confluent_kafka/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/confluent_kafka/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/custom/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/custom/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/cx_Oracle/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/cx_Oracle/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/dbapi/__init__.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/dbapi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ...sdk import sdk
 from ..utils import normalize_vendor
 
 
 class TracedCursor(wrapt.ObjectProxy):
     def __init__(self, cursor, db_info):
         super(TracedCursor, self).__init__(cursor)
-        self.db_info = f"{db_info}"
+        self.db_info = db_info
         self._self_last_execute_operation = None
         self._original_cursor = cursor
 
     def _trace_method(self, method, query, *args, **kwargs):
 
         # It could be psycopg2.sql.Composable, but we don't want to import that here
         if not isinstance(query, str):
```

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/django/db.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/django/db.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/django/middlewares.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/django/middlewares.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/django/utils.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/django/utils.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/django/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/django/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/middleware.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/fastapi/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/flask/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/flask/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/grpc/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/grpc/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/paramiko/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/paramiko/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/pika/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/pika/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/psycopg2/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/psycopg2/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ...sdk import sdk
 
 
 def instrument():
     def parse_dsn(dsn):
         return {c.split("=")[0]: c.split("=")[1] for c in dsn.split() if "=" in c}
 
-    class DynatraceCursor(psycopg2.extra.DictCursorBase):
+    class DynatraceCursor(psycopg2.extensions.cursor):
         def __init__(self, *args, **kwargs):
             self._dynatrace_db_info = kwargs.pop("dynatrace_db_info", None)
             super(DynatraceCursor, self).__init__(*args, **kwargs)
 
         def execute(self, query, vars=None):
             if hasattr(self, "_dynatrace_db_info") and self._dynatrace_db_info is not None:
                 with sdk.trace_sql_database_request(self._dynatrace_db_info, "{}".format(query)) as tracer:
```

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/pymongo/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/pymongo/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/pysnmp/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/pysnmp/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/redis/utils.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/redis/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/redis/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/sqlalchemy/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/sqlalchemy/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/starlette/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/starlette/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/subprocess/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/subprocess/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/suds/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/suds/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/tornado/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/tornado/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/autodynatrace/wrappers/urllib/wrapper.py` & `autodynatrace-2.0.2/autodynatrace/wrappers/urllib/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.0.0/setup.py` & `autodynatrace-2.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,48 @@
-from setuptools import setup, find_packages
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
-setup(
-    name="autodynatrace",
-    version="2.0.0",
-    packages=find_packages(),
-    package_data={"autodynatrace": ["wrappers/*"]},
-    install_requires=["wrapt>=1.11.2", "oneagent-sdk>=1.3.0", "six>=1.10.0", "autowrapt>=1.0"],
-    tests_require=["pytest", "mock", "tox", "django"],
-    entry_points={"autodynatrace": ["string = autodynatrace:load"]},
-    python_requires=">=3.6",
-    author="David Lopes",
-    author_email="david.lopes@dynatrace.com",
-    description="Auto instrumentation for the OneAgent SDK",
-    long_description="The autodynatrace package will auto instrument your python apps",
-    url="https://github.com/dlopes7/autodynatrace",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved",
-        "License :: OSI Approved :: Apache Software License",  # 2.0
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Operating System :: POSIX :: Linux",
-        "Operating System :: Microsoft :: Windows",
-        "Topic :: System :: Monitoring",
-    ],
-    project_urls={"Issue Tracker": "https://github.com/dlopes7/autodynatrace/issues"},
-)
+[project]
+name = "autodynatrace"
+dynamic = ["version"]
+description = "Auto instrumentation for the OneAgent SDK"
+readme = "README.md"
+license = ""
+requires-python = ">=3.6"
+authors = [
+    { name = "David Lopes", email = "david.lopes@dynatrace.com" },
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Topic :: System :: Monitoring",
+]
+dependencies = [
+    "autowrapt>=1.0",
+    "oneagent-sdk>=1.3.0",
+    "six>=1.10.0",
+    "wrapt>=1.11.2",
+]
+
+[project.entry-points.autodynatrace]
+string = "autodynatrace:load"
+
+[project.urls]
+Homepage = "https://github.com/dlopes7/autodynatrace"
+"Issue Tracker" = "https://github.com/dlopes7/autodynatrace/issues"
+
+[tool.hatch.version]
+path = "autodynatrace/__about__.py"
+
+[tool.hatch.build.targets.sdist]
+include = [
+    "/autodynatrace",
+]
```

