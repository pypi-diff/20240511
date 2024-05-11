# Comparing `tmp/combogenius-0.1.0.tar.gz` & `tmp/combogenius-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\combogenius-0.1.0.tar", last modified: Sun Apr  7 06:53:46 2024, max compression
+gzip compressed data, was "dist\combogenius-0.2.0.tar", last modified: Fri May 10 18:31:07 2024, max compression
```

## Comparing `combogenius-0.1.0.tar` & `combogenius-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 06:53:46.045995 combogenius-0.1.0/
--rw-rw-rw-   0        0        0     1074 2024-04-04 06:12:04.000000 combogenius-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-07 06:27:55.000000 combogenius-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      425 2024-04-07 06:53:46.045995 combogenius-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       29 2024-03-22 14:55:49.000000 combogenius-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 06:53:46.029455 combogenius-0.1.0/combogenius/
--rw-rw-rw-   0        0        0        0 2024-04-07 05:40:29.000000 combogenius-0.1.0/combogenius/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:53:46.037208 combogenius-0.1.0/combogenius/api/
--rw-rw-rw-   0        0        0     2333 2024-04-07 06:09:57.000000 combogenius-0.1.0/combogenius/api/API.py
--rw-rw-rw-   0        0        0        0 2024-04-04 05:47:42.000000 combogenius-0.1.0/combogenius/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:53:46.037208 combogenius-0.1.0/combogenius/database/
--rw-rw-rw-   0        0        0        0 2024-04-06 20:30:18.000000 combogenius-0.1.0/combogenius/database/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:53:46.045995 combogenius-0.1.0/combogenius/database/logger/
--rw-rw-rw-   0        0        0       43 2024-04-06 21:31:02.000000 combogenius-0.1.0/combogenius/database/logger/__init__.py
--rw-rw-rw-   0        0        0     1548 2024-04-06 21:31:02.000000 combogenius-0.1.0/combogenius/database/logger/logger.py
--rw-rw-rw-   0        0        0     1331 2024-04-06 22:20:48.000000 combogenius-0.1.0/combogenius/database/schema.py
--rw-rw-rw-   0        0        0     4452 2024-04-06 21:43:38.000000 combogenius-0.1.0/combogenius/database/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:53:46.045995 combogenius-0.1.0/combogenius/models/
--rw-rw-rw-   0        0        0        0 2024-04-04 05:47:37.000000 combogenius-0.1.0/combogenius/models/__init__.py
--rw-rw-rw-   0        0        0     2634 2024-04-07 05:33:29.000000 combogenius-0.1.0/combogenius/models/make_combos.py
--rw-rw-rw-   0        0        0        0 2024-04-07 05:38:29.000000 combogenius-0.1.0/combogenius/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:53:46.037208 combogenius-0.1.0/combogenius.egg-info/
--rw-rw-rw-   0        0        0      425 2024-04-07 06:53:45.000000 combogenius-0.1.0/combogenius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2024-04-07 06:53:45.000000 combogenius-0.1.0/combogenius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 06:53:45.000000 combogenius-0.1.0/combogenius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-07 06:53:45.000000 combogenius-0.1.0/combogenius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 06:53:46.045995 combogenius-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      454 2024-04-07 06:11:26.000000 combogenius-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 18:31:07.973966 combogenius-0.2.0/
+-rw-rw-rw-   0        0        0     2645 2024-05-10 18:31:07.973966 combogenius-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2025 2024-05-10 17:06:28.000000 combogenius-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 18:31:07.970975 combogenius-0.2.0/combogenius.egg-info/
+-rw-rw-rw-   0        0        0     2645 2024-05-10 18:31:07.000000 combogenius-0.2.0/combogenius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-10 18:31:07.000000 combogenius-0.2.0/combogenius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 18:31:07.000000 combogenius-0.2.0/combogenius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 18:31:07.000000 combogenius-0.2.0/combogenius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 18:31:07.973966 combogenius-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      672 2024-05-10 17:44:51.000000 combogenius-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 18:31:07.972968 combogenius-0.2.0/tests/
+-rw-rw-rw-   0        0        0      472 2024-05-10 17:29:35.000000 combogenius-0.2.0/tests/test_api.py
+-rw-rw-rw-   0        0        0     1447 2024-05-10 17:31:41.000000 combogenius-0.2.0/tests/test_database.py
+-rw-rw-rw-   0        0        0     1748 2024-05-10 17:31:40.000000 combogenius-0.2.0/tests/test_make_combos.py
```

