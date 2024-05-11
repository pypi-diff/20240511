# Comparing `tmp/anabih_python_test-6.0.0.tar.gz` & `tmp/anabih_python_test-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anabih_python_test-6.0.0.tar", last modified: Thu May  9 14:40:45 2024, max compression
+gzip compressed data, was "anabih_python_test-7.0.0.tar", last modified: Sat May 11 20:13:37 2024, max compression
```

## Comparing `anabih_python_test-6.0.0.tar` & `anabih_python_test-7.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 14:40:45.662454 anabih_python_test-6.0.0/
--rw-rw-rw-   0        0        0      431 2024-05-09 14:40:45.660619 anabih_python_test-6.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       19 2024-05-09 00:01:05.000000 anabih_python_test-6.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 14:40:45.659620 anabih_python_test-6.0.0/anabih_python_test.egg-info/
--rw-rw-rw-   0        0        0      431 2024-05-09 14:40:45.000000 anabih_python_test-6.0.0/anabih_python_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-05-09 14:40:45.000000 anabih_python_test-6.0.0/anabih_python_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 14:40:45.000000 anabih_python_test-6.0.0/anabih_python_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 14:40:45.000000 anabih_python_test-6.0.0/anabih_python_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 14:40:45.658620 anabih_python_test-6.0.0/my_package/
--rw-rw-rw-   0        0        0        0 2024-05-09 03:08:34.000000 anabih_python_test-6.0.0/my_package/__init__.py
--rw-rw-rw-   0        0        0       62 2024-05-09 14:40:29.000000 anabih_python_test-6.0.0/my_package/greetings.py
--rw-rw-rw-   0        0        0       42 2024-05-09 14:40:45.662454 anabih_python_test-6.0.0/setup.cfg
--rw-rw-rw-   0        0        0      657 2024-05-09 14:40:41.000000 anabih_python_test-6.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 20:13:37.944333 anabih_python_test-7.0.0/
+-rw-rw-rw-   0        0        0      537 2024-05-11 20:13:37.943333 anabih_python_test-7.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2024-05-09 00:01:05.000000 anabih_python_test-7.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 20:13:37.942333 anabih_python_test-7.0.0/anabih_python_test.egg-info/
+-rw-rw-rw-   0        0        0      537 2024-05-11 20:13:37.000000 anabih_python_test-7.0.0/anabih_python_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-11 20:13:37.000000 anabih_python_test-7.0.0/anabih_python_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 20:13:37.000000 anabih_python_test-7.0.0/anabih_python_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-11 20:13:37.000000 anabih_python_test-7.0.0/anabih_python_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 20:13:37.000000 anabih_python_test-7.0.0/anabih_python_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 20:13:37.941333 anabih_python_test-7.0.0/my_package/
+-rw-rw-rw-   0        0        0        0 2024-05-09 03:08:34.000000 anabih_python_test-7.0.0/my_package/__init__.py
+-rw-rw-rw-   0        0        0      468 2024-05-11 20:09:15.000000 anabih_python_test-7.0.0/my_package/greetings.py
+-rw-rw-rw-   0        0        0      715 2024-05-11 20:13:25.000000 anabih_python_test-7.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 20:13:37.945334 anabih_python_test-7.0.0/setup.cfg
```

