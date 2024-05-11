# Comparing `tmp/QDetective-0.0.2.tar.gz` & `tmp/QDetective-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\QDetective-0.0.2.tar", last modified: Fri Apr  7 06:34:48 2023, max compression
+gzip compressed data, was "QDetective-0.1.0.tar", max compression
```

## Comparing `QDetective-0.0.2.tar` & `QDetective-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,5 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 06:34:48.517797 QDetective-0.0.2/
--rw-rw-rw-   0        0        0      649 2023-04-07 06:34:48.500811 QDetective-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-07 06:34:48.302784 QDetective-0.0.2/QDetective/
--rw-rw-rw-   0        0        0     4720 2023-04-07 03:44:53.000000 QDetective-0.0.2/QDetective/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 06:34:48.445994 QDetective-0.0.2/QDetective.egg-info/
--rw-rw-rw-   0        0        0      649 2023-04-07 06:34:48.000000 QDetective-0.0.2/QDetective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-04-07 06:34:48.000000 QDetective-0.0.2/QDetective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 06:34:48.000000 QDetective-0.0.2/QDetective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-07 06:34:48.000000 QDetective-0.0.2/QDetective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      133 2023-03-30 13:52:44.000000 QDetective-0.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-07 06:34:48.518794 QDetective-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      957 2023-04-07 03:50:24.000000 QDetective-0.0.2/setup.py
+-rwxr-xr-x   0        0        0     1075 2023-04-07 06:32:40.671062 QDetective-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      327 2024-05-11 14:59:37.767132 QDetective-0.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0     5208 2024-05-11 15:00:15.701022 QDetective-0.1.0/qdetective/__init__.py
+-rw-r--r--   0        0        0      525 2024-05-11 15:02:19.705232 QDetective-0.1.0/setup.py
+-rw-r--r--   0        0        0      271 2024-05-11 15:02:19.705363 QDetective-0.1.0/PKG-INFO
```

