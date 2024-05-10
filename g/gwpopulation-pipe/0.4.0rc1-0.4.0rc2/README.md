# Comparing `tmp/gwpopulation_pipe-0.4.0rc1.tar.gz` & `tmp/gwpopulation_pipe-0.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwpopulation_pipe-0.4.0rc1.tar", last modified: Fri Mar 15 14:59:56 2024, max compression
+gzip compressed data, was "gwpopulation_pipe-0.4.0rc2.tar", last modified: Fri May 10 21:59:47 2024, max compression
```

## Comparing `gwpopulation_pipe-0.4.0rc1.tar` & `gwpopulation_pipe-0.4.0rc2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 colm       (501) staff       (20)        0 2024-03-15 14:59:56.242542 gwpopulation_pipe-0.4.0rc1/
--rw-r--r--   0 colm       (501) staff       (20)     1853 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/.gitignore
--rw-r--r--   0 colm       (501) staff       (20)     3380 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/.gitlab-ci.yml
--rw-r--r--   0 colm       (501) staff       (20)     1035 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 colm       (501) staff       (20)     1068 2021-01-29 16:32:14.000000 gwpopulation_pipe-0.4.0rc1/LICENSE
--rw-r--r--   0 colm       (501) staff       (20)     1421 2024-03-15 14:59:56.242479 gwpopulation_pipe-0.4.0rc1/PKG-INFO
--rw-r--r--   0 colm       (501) staff       (20)      405 2021-11-08 14:38:20.000000 gwpopulation_pipe-0.4.0rc1/README.md
-drwxr-xr-x   0 colm       (501) staff       (20)        0 2024-03-15 14:59:56.236211 gwpopulation_pipe-0.4.0rc1/docs/
--rw-r--r--   0 colm       (501) staff       (20)      605 2021-11-08 14:21:25.000000 gwpopulation_pipe-0.4.0rc1/docs/Makefile
--rw-r--r--   0 colm       (501) staff       (20)     3748 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/docs/conf.py
--rw-r--r--   0 colm       (501) staff       (20)     1533 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/docs/configuration.rst
--rw-r--r--   0 colm       (501) staff       (20)     2381 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/docs/customizing.rst
--rw-r--r--   0 colm       (501) staff       (20)     4111 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/docs/index.rst
--rw-r--r--   0 colm       (501) staff       (20)     1170 2021-11-08 14:21:25.000000 gwpopulation_pipe-0.4.0rc1/docs/prior.rst
--rw-r--r--   0 colm       (501) staff       (20)     3886 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/docs/real-data.rst
--rw-r--r--   0 colm       (501) staff       (20)     1598 2021-11-08 14:21:25.000000 gwpopulation_pipe-0.4.0rc1/docs/simulation.rst
--rw-r--r--   0 colm       (501) staff       (20)     1845 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/docs/specifying-data.rst
--rw-r--r--   0 colm       (501) staff       (20)     1015 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/docs/specifying-models.rst
-drwxr-xr-x   0 colm       (501) staff       (20)        0 2024-03-15 14:59:56.236545 gwpopulation_pipe-0.4.0rc1/docs/templates/
--rw-r--r--   0 colm       (501) staff       (20)      639 2021-11-08 14:21:25.000000 gwpopulation_pipe-0.4.0rc1/docs/templates/custom-class-template.rst
--rw-r--r--   0 colm       (501) staff       (20)     1465 2021-11-08 14:21:25.000000 gwpopulation_pipe-0.4.0rc1/docs/templates/custom-module-template.rst
-drwxr-xr-x   0 colm       (501) staff       (20)        0 2024-03-15 14:59:56.237992 gwpopulation_pipe-0.4.0rc1/example/
--rw-r--r--   0 colm       (501) staff       (20)     2356 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/example/fetch-all-samples.sh
--rw-r--r--   0 colm       (501) staff       (20)      927 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/example/gaussian_models.py
--rw-r--r--   0 colm       (501) staff       (20)      367 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/example/gaussians.prior
--rw-r--r--   0 colm       (501) staff       (20)     2895 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/example/gwtc3-bbh.ini
--rw-r--r--   0 colm       (501) staff       (20)     1898 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/example/gwtc3-bbh.prior
--rw-r--r--   0 colm       (501) staff       (20)     3000 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/example/gwtc3-gaussian.ini
--rw-r--r--   0 colm       (501) staff       (20)      957 2021-11-08 14:21:25.000000 gwpopulation_pipe-0.4.0rc1/example/prior_sample.sh
--rw-r--r--   0 colm       (501) staff       (20)      203 2021-11-08 14:21:25.000000 gwpopulation_pipe-0.4.0rc1/example/samples.json
--rw-r--r--   0 colm       (501) staff       (20)     1281 2021-11-08 14:21:25.000000 gwpopulation_pipe-0.4.0rc1/example/simulations.sh
-drwxr-xr-x   0 colm       (501) staff       (20)        0 2024-03-15 14:59:56.240563 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/
--rw-r--r--   0 colm       (501) staff       (20)       34 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/__init__.py
--rw-r--r--   0 colm       (501) staff       (20)      414 2024-03-15 14:59:56.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/_version.py
--rw-r--r--   0 colm       (501) staff       (20)    13446 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/common_format.py
--rw-r--r--   0 colm       (501) staff       (20)     1098 2021-01-29 21:16:11.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/create_injections.py
--rwxr-xr-x   0 colm       (501) staff       (20)    20365 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/data_analysis.py
--rwxr-xr-x   0 colm       (501) staff       (20)    22247 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/data_collection.py
--rw-r--r--   0 colm       (501) staff       (20)     8180 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/data_simulation.py
--rwxr-xr-x   0 colm       (501) staff       (20)    14445 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/main.py
--rw-r--r--   0 colm       (501) staff       (20)    11333 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/parser.py
--rw-r--r--   0 colm       (501) staff       (20)    10441 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/pesumary_plot.py
--rwxr-xr-x   0 colm       (501) staff       (20)    34949 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/post_plots.py
--rw-r--r--   0 colm       (501) staff       (20)     5189 2021-01-29 21:15:44.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/review.py
--rw-r--r--   0 colm       (501) staff       (20)     4624 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/utils.py
--rwxr-xr-x   0 colm       (501) staff       (20)    11215 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/vt_helper.py
-drwxr-xr-x   0 colm       (501) staff       (20)        0 2024-03-15 14:59:56.241660 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe.egg-info/
--rw-r--r--   0 colm       (501) staff       (20)     1421 2024-03-15 14:59:56.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe.egg-info/PKG-INFO
--rw-r--r--   0 colm       (501) staff       (20)     1295 2024-03-15 14:59:56.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 colm       (501) staff       (20)        1 2024-03-15 14:59:56.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 colm       (501) staff       (20)      687 2024-03-15 14:59:56.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe.egg-info/entry_points.txt
--rw-r--r--   0 colm       (501) staff       (20)      163 2024-03-15 14:59:56.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe.egg-info/requires.txt
--rw-r--r--   0 colm       (501) staff       (20)       18 2024-03-15 14:59:56.000000 gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe.egg-info/top_level.txt
--rw-r--r--   0 colm       (501) staff       (20)      206 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/pyproject.toml
--rw-r--r--   0 colm       (501) staff       (20)     1983 2024-03-15 14:59:56.243068 gwpopulation_pipe-0.4.0rc1/setup.cfg
--rw-r--r--   0 colm       (501) staff       (20)       61 2024-03-15 14:58:25.000000 gwpopulation_pipe-0.4.0rc1/setup.py
+drwxrwxr-x   0 colm.talbot (44246) colm.talbot (44246)        0 2024-05-10 21:59:47.854356 gwpopulation_pipe-0.4.0rc2/
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1853 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/.gitignore
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     3767 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/.gitlab-ci.yml
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1035 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/.pre-commit-config.yaml
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1068 2021-07-29 16:35:45.000000 gwpopulation_pipe-0.4.0rc2/LICENSE
+-rw-r--r--   0 colm.talbot (44246) colm.talbot (44246)     1421 2024-05-10 21:59:47.853356 gwpopulation_pipe-0.4.0rc2/PKG-INFO
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)      405 2022-03-15 19:50:58.000000 gwpopulation_pipe-0.4.0rc2/README.md
+drwxrwxr-x   0 colm.talbot (44246) colm.talbot (44246)        0 2024-05-10 21:59:47.758355 gwpopulation_pipe-0.4.0rc2/docs/
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)      605 2022-03-15 19:50:59.000000 gwpopulation_pipe-0.4.0rc2/docs/Makefile
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     3748 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/docs/conf.py
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1533 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/docs/configuration.rst
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     2381 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/docs/customizing.rst
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     4111 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/docs/index.rst
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1170 2022-03-15 19:50:59.000000 gwpopulation_pipe-0.4.0rc2/docs/prior.rst
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     3886 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/docs/real-data.rst
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1598 2022-03-15 19:50:59.000000 gwpopulation_pipe-0.4.0rc2/docs/simulation.rst
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1845 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/docs/specifying-data.rst
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1015 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/docs/specifying-models.rst
+drwxrwxr-x   0 colm.talbot (44246) colm.talbot (44246)        0 2024-05-10 21:59:47.762355 gwpopulation_pipe-0.4.0rc2/docs/templates/
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)      639 2022-03-15 19:50:59.000000 gwpopulation_pipe-0.4.0rc2/docs/templates/custom-class-template.rst
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1465 2022-03-15 19:50:59.000000 gwpopulation_pipe-0.4.0rc2/docs/templates/custom-module-template.rst
+drwxrwxr-x   0 colm.talbot (44246) colm.talbot (44246)        0 2024-05-10 21:59:47.779355 gwpopulation_pipe-0.4.0rc2/example/
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     2356 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/example/fetch-all-samples.sh
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)      927 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/example/gaussian_models.py
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)      367 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/example/gaussians.prior
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     2895 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/example/gwtc3-bbh.ini
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1898 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/example/gwtc3-bbh.prior
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     3000 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/example/gwtc3-gaussian.ini
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)      957 2022-03-15 19:51:00.000000 gwpopulation_pipe-0.4.0rc2/example/prior_sample.sh
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)      203 2022-03-15 19:51:00.000000 gwpopulation_pipe-0.4.0rc2/example/samples.json
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1281 2022-03-15 19:51:00.000000 gwpopulation_pipe-0.4.0rc2/example/simulations.sh
+drwxrwxr-x   0 colm.talbot (44246) colm.talbot (44246)        0 2024-05-10 21:59:47.835356 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)       34 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/__init__.py
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)      414 2024-05-10 21:59:47.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/_version.py
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)    13447 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/common_format.py
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1098 2021-07-29 16:35:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/create_injections.py
+-rwxrwxr-x   0 colm.talbot (44246) colm.talbot (44246)    20380 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/data_analysis.py
+-rwxrwxr-x   0 colm.talbot (44246) colm.talbot (44246)    21275 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/data_collection.py
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     8180 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/data_simulation.py
+-rwxrwxr-x   0 colm.talbot (44246) colm.talbot (44246)    14445 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/main.py
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)    11315 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/parser.py
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)    10441 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/pesumary_plot.py
+-rwxrwxr-x   0 colm.talbot (44246) colm.talbot (44246)    35108 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/post_plots.py
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     5189 2021-07-29 16:35:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/review.py
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     4624 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/utils.py
+-rwxrwxr-x   0 colm.talbot (44246) colm.talbot (44246)    17829 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/vt_helper.py
+drwxrwxr-x   0 colm.talbot (44246) colm.talbot (44246)        0 2024-05-10 21:59:47.851356 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe.egg-info/
+-rw-r--r--   0 colm.talbot (44246) colm.talbot (44246)     1421 2024-05-10 21:59:47.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe.egg-info/PKG-INFO
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     1295 2024-05-10 21:59:47.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe.egg-info/SOURCES.txt
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)        1 2024-05-10 21:59:47.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe.egg-info/dependency_links.txt
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)      767 2024-05-10 21:59:47.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe.egg-info/entry_points.txt
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)      163 2024-05-10 21:59:47.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe.egg-info/requires.txt
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)       18 2024-05-10 21:59:47.000000 gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe.egg-info/top_level.txt
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)      206 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/pyproject.toml
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)     2064 2024-05-10 21:59:47.856356 gwpopulation_pipe-0.4.0rc2/setup.cfg
+-rw-rw-r--   0 colm.talbot (44246) colm.talbot (44246)       61 2024-05-10 21:57:45.000000 gwpopulation_pipe-0.4.0rc2/setup.py
```

### Comparing `gwpopulation_pipe-0.4.0rc1/.gitignore` & `gwpopulation_pipe-0.4.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/.gitlab-ci.yml` & `gwpopulation_pipe-0.4.0rc2/.gitlab-ci.yml`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,34 @@
 # https://docs.gitlab.com/ee/ci/yaml/#gitlab-ci-yml
 
 # stages is a reserved keyword that defines job dependencies and
 # parallelization. each stage runs in parallel but must complete
 # before the next stage begins
 # This file was copied from bilby_pipe
 
-variables:
-  SETUPTOOLS_SCM_PRETEND_VERSION: "0.0.0"
+workflow:
+  rules:
+    - if: $CI_COMMIT_REF_NAME != $CI_DEFAULT_BRANCH
+      variables:
+        SETUPTOOLS_SCM_PRETEND_VERSION: "0.0.0"
+    - if: $CI_COMMIT_REF_NAME == $CI_DEFAULT_BRANCH
+      variables:
+        SETUPTOOLS_SCM_PRETEND_VERSION: ""
 
 stages:
   - test
   - deploy
 
 .test-python: &test-python
   stage: test
   image: python
   before_script:
     - pip install --upgrade pip
   script:
-    - pip install --pre gwpopulation
-    - pip install --ignore-installed .
+    - pip install .
     - cd ..
     - python -c "import gwpopulation_pipe; print(gwpopulation_pipe.__version__)"
     - python -c "import gwpopulation_pipe.common_format"
     - python -c "import gwpopulation_pipe.create_injections"
     - python -c "import gwpopulation_pipe.data_analysis"
     - python -c "import gwpopulation_pipe.data_collection"
     - python -c "import gwpopulation_pipe.main"
@@ -98,29 +103,41 @@
 gaussian-jax:
   <<: *example-tests
   variables:
     BACKEND: jax
     KIND: gaussian
 
 docs:
-    variables:
-      SETUPTOOLS_SCM_PRETEND_VERSION: ""
     stage: test
     needs: [ "basic-3.10" ]
     image: containers.ligo.org/lscsoft/bilby/v2-bilby-python310
     script:
       - python -m pip install .[pages]
       - cd docs
       - make clean
       - make html
 
     artifacts:
       paths:
         - docs/_build/html/
 
+
+pypi-release:
+  stage: deploy
+  image: containers.ligo.org/lscsoft/bilby/v2-bilby-python310
+  variables:
+    TWINE_USERNAME: $PYPI_USERNAME
+    TWINE_PASSWORD: $PYPI_PASSWORD
+  before_script:
+    - python -m build --sdist --wheel --outdir dist/ .
+  script:
+    - twine upload dist/*
+  only:
+    - tags
+
 pages:
   stage: deploy
   needs: ["docs"]
   script:
     - mkdir public/
     - mv docs/_build/html/* public/
   artifacts:
```

### Comparing `gwpopulation_pipe-0.4.0rc1/.pre-commit-config.yaml` & `gwpopulation_pipe-0.4.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/LICENSE` & `gwpopulation_pipe-0.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/PKG-INFO` & `gwpopulation_pipe-0.4.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpopulation_pipe
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: A pipeline population inference
 Home-page: https://git.ligo.org/RatesAndPopulations/gwpopulation_pipe
 Author: Colm Talbot
 Author-email: colm.talbot@ligo.org
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/Makefile` & `gwpopulation_pipe-0.4.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/conf.py` & `gwpopulation_pipe-0.4.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/configuration.rst` & `gwpopulation_pipe-0.4.0rc2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/customizing.rst` & `gwpopulation_pipe-0.4.0rc2/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/index.rst` & `gwpopulation_pipe-0.4.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/prior.rst` & `gwpopulation_pipe-0.4.0rc2/docs/prior.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/real-data.rst` & `gwpopulation_pipe-0.4.0rc2/docs/real-data.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/simulation.rst` & `gwpopulation_pipe-0.4.0rc2/docs/simulation.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/specifying-data.rst` & `gwpopulation_pipe-0.4.0rc2/docs/specifying-data.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/specifying-models.rst` & `gwpopulation_pipe-0.4.0rc2/docs/specifying-models.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/templates/custom-class-template.rst` & `gwpopulation_pipe-0.4.0rc2/docs/templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/docs/templates/custom-module-template.rst` & `gwpopulation_pipe-0.4.0rc2/docs/templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/example/fetch-all-samples.sh` & `gwpopulation_pipe-0.4.0rc2/example/fetch-all-samples.sh`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/example/gaussian_models.py` & `gwpopulation_pipe-0.4.0rc2/example/gaussian_models.py`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/example/gwtc3-bbh.ini` & `gwpopulation_pipe-0.4.0rc2/example/gwtc3-bbh.ini`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/example/gwtc3-bbh.prior` & `gwpopulation_pipe-0.4.0rc2/example/gwtc3-bbh.prior`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/example/gwtc3-gaussian.ini` & `gwpopulation_pipe-0.4.0rc2/example/gwtc3-gaussian.ini`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/example/prior_sample.sh` & `gwpopulation_pipe-0.4.0rc2/example/prior_sample.sh`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/example/simulations.sh` & `gwpopulation_pipe-0.4.0rc2/example/simulations.sh`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/common_format.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/common_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     else:
         logger.info("Generating predicted populations.")
         args.models = result.meta_data["vt_models"]
         vt_data = load_injection_data(
             args.injection_file,
             ifar_threshold=args.vt_ifar_threshold,
             snr_threshold=args.vt_snr_threshold,
-        ).__dict__
+        ).to_dict()
         model = load_model(args)
         synthetic_dataset = resample_injections_per_population_sample(
             posterior=posterior,
             data=vt_data,
             model=model,
             n_draws=n_draws,
         )
```

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/create_injections.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/create_injections.py`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/data_analysis.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/data_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,14 @@
             "Likelihood has no method 'per_event_bayes_factors_and_n_effective'"
             " skipping n_effective calculation."
         )
         return
     all_n_effectives = list()
     for ii in trange(len(posterior), file=sys.stdout):
         parameters = dict(posterior.iloc[ii])
-        parameters, _ = likelihood.conversion_function(parameters)
         likelihood.parameters.update(parameters)
         likelihood.hyper_prior.parameters.update(parameters)
         _, n_effectives = likelihood.per_event_bayes_factors_and_n_effective()
         all_n_effectives.append(float(min(n_effectives)))
     posterior["min_event_n_effective"] = all_n_effectives
     return
 
@@ -360,14 +359,15 @@
         The input samples with the new prior weights in a new `weights` entry.
     reweighted_samples: dict
         The input samples resampled in place according to the new prior weights.
         Note that this will cause samples to be repeated.
     """
     original_samples = likelihood.data
     original_samples["prior"] = likelihood.sampling_prior
+
     reweighted_samples, weights = likelihood.posterior_predictive_resample(
         result.posterior, return_weights=True
     )
     original_samples["weights"] = weights
     original_samples = {
         key: to_numpy(original_samples[key]) for key in original_samples
     }
@@ -450,15 +450,15 @@
     for key in list(hyper_prior.keys()):
         if (
             key not in search_keys
             and key != "rate"
             and not isinstance(hyper_prior[key], Constraint)
         ):
             del hyper_prior[key]
-        elif (isinstance(hyper_prior[key], Constraint)) and (args.backend == "jax"):
+        elif (isinstance(hyper_prior[key], Constraint)) and (args.sampler == "NUTS"):
             del hyper_prior[key]
 
     likelihood = create_likelihood(args, posteriors, model, selection)
     likelihood.parameters.update(hyper_prior.sample())
     likelihood.log_likelihood_ratio()
 
     if args.injection_file is not None:
@@ -550,14 +550,16 @@
             save="hdf5",
             **get_sampler_kwargs(args),
         )
         result.meta_data["models"] = args.models
         result.meta_data["vt_models"] = args.vt_models
         result.meta_data["event_ids"] = event_ids
 
+        result.posterior = likelihood.conversion_function(result.posterior)[0]
+
         logger.info("Computing rate posterior")
         compute_rate_posterior(posterior=result.posterior, selection=selection)
         logger.info("Computing n effectives")
         fill_minimum_n_effective(posterior=result.posterior, likelihood=likelihood)
         logger.info("Generating extra statistics")
         result.posterior = generate_extra_statistics(
             posterior=result.posterior, likelihood=likelihood
```

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/data_collection.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/data_collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from bilby_pipe.utils import convert_string_to_dict
 from gwpopulation.backend import set_backend
 from scipy.interpolate import interp1d
 
 from .data_simulation import simulate_posteriors
 from .parser import create_parser
 from .utils import get_path_or_local
-from .vt_helper import load_injection_data
+from .vt_helper import dump_injection_data
 
 matplotlib.rcParams["text.usetex"] = False
 
 
 def euclidean_distance_prior(samples):
     r"""
     Evaluate the redshift prior assuming a Euclidean universe.
@@ -143,60 +143,63 @@
                 new[key] = post[key]
             else:
                 new[key] = 0
         new_posts[name] = new
     return new_posts
 
 
-def evaluate_prior(posts, args):
+def evaluate_prior(posts, args, dataset):
     """
     Evaluate the prior distribution for the input posteriors.
 
     Parameters
     ----------
     posts: dict
         Dictionary of `pd.DataFrame` objects containing the posteriors.
     args:
         Input args containing the prior specification.
+    dataset: str
+        The dataset label to evaluate the prior for (i.e. "O4a"). Should be a key in `args.sample_regex`.
 
     Returns
     -------
     posts: dict
         The input dictionary, modified in place.
     """
+
     max_redshift = max(
         args.max_redshift, max([max(posts[key]["redshift"]) for key in posts])
     )
     zs_ = np.linspace(0, max_redshift * 1.01, 1000)
-    if args.distance_prior.lower() == "comoving":
+    if args.distance_prior[dataset].lower() == "comoving":
         logger.info(
             "Using uniform in the comoving source frame distance prior for all events."
         )
         p_z = Planck15.differential_comoving_volume(zs_).value * 4 * np.pi / (1 + zs_)
-    elif args.distance_prior.lower() == "euclidean":
+    elif args.distance_prior[dataset].lower() == "euclidean":
         logger.info("Using Euclidean distance prior for all events.")
         p_z = euclidean_distance_prior(dict(redshift=zs_))
-    elif args.distance_prior.lower() == "none":
+    elif args.distance_prior[dataset].lower() == "none":
         p_z = np.ones(zs_.shape)
     else:
         raise ValueError(f"Redshift prior {args.distance_prior} not recognized")
     p_z /= np.trapz(p_z, zs_)
     interpolated_p_z = interp1d(zs_, p_z)
 
-    if args.mass_prior.lower() == "flat-detector-components":
+    if args.mass_prior[dataset].lower() == "flat-detector-components":
         logger.info("Assuming flat in detector frame mass prior for all events.")
-    elif args.mass_prior.lower() == "flat-detector-chirp-mass-ratio":
+    elif args.mass_prior[dataset].lower() == "flat-detector-chirp-mass-ratio":
         logger.info("Assuming chirp mass prior for all events.")
-    elif args.mass_prior.lower() not in ["flat-source-components", "none"]:
-        raise ValueError(f"Mass prior {args.mass_prior} not recognized.")
+    elif args.mass_prior[dataset].lower() not in ["flat-source-components", "none"]:
+        raise ValueError(f"Mass prior {args.mass_prior[dataset]} not recognized.")
 
-    if args.spin_prior.lower() == "component":
+    if args.spin_prior[dataset].lower() == "component":
         logger.info("Assuming uniform in component spin prior for all events.")
-    elif args.spin_prior.lower() != "none":
-        raise ValueError(f"Spin prior {args.spin_prior} not recognized.")
+    elif args.spin_prior[dataset].lower() != "none":
+        raise ValueError(f"Spin prior {args.spin_prior[dataset]} not recognized.")
 
     if "mass_ratio" in args.parameters:
         logger.info(
             "Model is defined in terms of mass ratio, adjusting prior accordingly."
         )
     if "chirp_mass" in args.parameters:
         logger.info(
@@ -210,29 +213,29 @@
         if "redshift" in post and "redshift" in args.parameters:
             post["prior"] *= interpolated_p_z(post["redshift"])
         else:
             logger.warning(
                 f"No redshift present for {name}, cannot evaluate distance prior weight"
             )
 
-        if args.mass_prior.lower() == "flat-detector-components":
+        if args.mass_prior[dataset].lower() == "flat-detector-components":
             post["prior"] *= (1 + post["redshift"]) ** 2
-        elif args.mass_prior.lower() == "flat-detector-chirp-mass-ratio":
+        elif args.mass_prior[dataset].lower() == "flat-detector-chirp-mass-ratio":
             post["prior"] /= (
                 post["mass_1"]
                 / (1 + post["redshift"])
                 * primary_mass_to_chirp_mass_jacobian(post)
             )
 
         if "mass_ratio" in args.parameters:
             post["prior"] *= post["mass_1"]
         if "chirp_mass" in args.parameters:
             post["prior"] *= primary_mass_to_chirp_mass_jacobian(post)
 
-        if args.spin_prior.lower() == "component":
+        if args.spin_prior[dataset].lower() == "component":
             post["prior"] /= 4
         if "chi_1" in args.parameters:
             post["prior"] *= aligned_spin_prior(post["chi_1"])
         if "chi_2" in args.parameters:
             post["prior"] *= aligned_spin_prior(post["chi_2"])
 
     return posts
@@ -445,20 +448,20 @@
         posts, meta = _load_batch_of_meta_files(
             regex=regex,
             label=label,
             labels=args.preferred_labels,
             keys=args.parameters,
             ignore=ignore,
         )
+        posts = evaluate_prior(posts, args=args, dataset=label)
         posteriors.update(posts)
         meta_data.update(meta)
     if save_meta_data:
         with open(os.path.join(args.run_dir, "data", "event_data.json"), "w") as ff:
             json.dump(meta_data, ff)
-    posteriors = evaluate_prior(posteriors, args=args)
     for key in args.parameters:
         for name in posteriors:
             if key not in posteriors[name]:
                 raise KeyError(f"{key} not found for {name}")
     logger.info(f"Loaded {len(posteriors)} posteriors.")
     return posteriors
 
@@ -543,70 +546,14 @@
     logger.info(f"Downsampling to {n_samples} samples per posterior")
     downsampled_posts = [
         post.sample(n_samples, random_state=args.collection_seed) for post in posts
     ]
     return downsampled_posts, events
 
 
-def dump_injection_data(args):
-    """
-    Dump the injection data to a pickle file to :code:`{args.run_dir}/data/injections.pkl` for easier file transfer.
-
-    This also makes sure the required parameters are present in the data and updates the prior accordingly.
-
-    Parameters
-    ----------
-    args:
-        Command-line arguments
-    """
-    if "*" in args.vt_file:
-        data = reduce(
-            lambda x, y: x + y,
-            [
-                load_injection_data(
-                    vt_file=get_path_or_local(vt_file),
-                    ifar_threshold=args.vt_ifar_threshold,
-                    snr_threshold=args.vt_snr_threshold,
-                )
-                for vt_file in glob.glob(args.vt_file)
-            ],
-        )
-    else:
-        data = load_injection_data(
-            vt_file=get_path_or_local(args.vt_file),
-            ifar_threshold=args.vt_ifar_threshold,
-            snr_threshold=args.vt_snr_threshold,
-        )
-    apply_injection_prior(data, args.parameters)
-    fname = f"{args.run_dir}/data/injections.pkl"
-    with open(fname, "wb") as ff:
-        dill.dump(data, ff)
-    logger.info(f"Written injection data to {fname}")
-
-
-def apply_injection_prior(data, parameters):
-    """
-    We assume the injection prior is uniform in the detector frame primary
-    mass and mass ratio.
-    """
-    if "mass_2" in parameters:
-        data["mass_2"] = data["mass_1"] * data["mass_ratio"]
-        data["prior"] /= data["mass_1"]
-    if "chirp_mass" in parameters:
-        jacobian = primary_mass_to_chirp_mass_jacobian(data)
-        data["chirp_mass"] = data["mass_1"] / jacobian
-        data["prior"] *= jacobian
-    if "chi_1" in parameters:
-        data["chi_1"] = data["a_1"] * data["cos_tilt_1"]
-        data["prior"] *= 2 * aligned_spin_prior(data["chi_1"])
-    if "chi_2" in parameters:
-        data["chi_2"] = data["a_2"] * data["cos_tilt_2"]
-        data["prior"] *= 2 * aligned_spin_prior(data["chi_2"])
-
-
 def resolve_arguments(args):
     """
     - Make sure there are no incompatible arguments.
     - Resolve any deprecated arguments with their corresponding updates if possible.
     - Disable prior terms for parameters that aren't being fit.
     """
     if args.mass_prior.lower() == "flat-detector":
@@ -647,32 +594,60 @@
         "chi_2",
         "chi_eff",
         "chi_p",
     }
     fitted_spins = spin_parameters.intersection(args.parameters)
     if len(fitted_spins) == 0:
         args.spin_prior = "None"
+    args.sample_regex = convert_arg_to_dict(args.sample_regex)
+    prior_dict = {
+        key: vars(args)[key] for key in ["mass_prior", "spin_prior", "distance_prior"]
+    }
+    for param in prior_dict:
+        if "{" not in prior_dict[param]:
+            prior_dict[param] = {
+                dataset: prior_dict[param] for dataset in args.sample_regex
+            }
+        else:
+            prior_dict[param] = convert_arg_to_dict(prior_dict[param])
+    vars(args).update(prior_dict)
+
 
+def convert_arg_to_dict(arg):
+    """
+    Convert a string argument to a dictionary. Not in-place.
+    gwpopulation_pipe strips quotes from the regex string, so we need to add them back in,
+    this assumes that there are no internal braces and spaces after all ':' and ','
+    delimiting entries.
+
+    Parameters
+    ----------
+    arg: str
+        Arg that should be converted to a dictionary.
+
+    Returns
+    -------
+    arg_dict: dict
+        Dictionary representation of the input string.
+    """
     try:
-        regex_str = args.sample_regex
+        regex_str = arg
         if '"' not in regex_str:
-            # gwpopulation_pipe strips quotes from the regex string,
-            # so we need to add them back in, this assumes that there
-            # are no internal braces and spaces after all ':' and ','
-            # delimiting entries.
+
             regex_str = (
                 regex_str.replace("{", '{"')
                 .replace(":", '":"')
                 .replace(", ", '", "')
                 .replace("}", '"}')
                 .replace(" ", "")
             )
-        args.sample_regex = json.loads(regex_str)
+        arg_dict = json.loads(regex_str)
     except json.decoder.JSONDecodeError:
-        args.sample_regex = convert_string_to_dict(args.sample_regex)
+        arg_dict = convert_string_to_dict(arg)
+    return arg_dict
 
 
 def main():
     parser = create_parser()
     args = parser.parse_args()
     resolve_arguments(args)
```

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/data_simulation.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/data_simulation.py`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/main.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/main.py`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/parser.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,50 +167,45 @@
         help="Seed for the downsampling of the posteriors for each event. For reproducibility.",
     )
     collection_parser.add_argument(
         "--data-label", default="posteriors", help="Label for data product."
     )
     collection_parser.add_argument(
         "--distance-prior",
-        default="euclidean",
-        choices=["euclidean", "comoving"],
+        default="comoving",
+        type=str,
         help=(
             "Distance prior format, e.g., euclidean, comoving. 'euclidean' assumes the distance prior goes "
             "like D^2. 'comoving' assumes sources are uniformly distributed in the comoving frame using "
-            "the Planck15 cosmology."
+            "the Planck15 cosmology. Can be in the format of a dict with the same keys as the sample-regex"
         ),
     )
+
     collection_parser.add_argument(
         "--mass-prior",
         default="flat-detector",
-        choices=[
-            "flat-detector-components",
-            "flat-source-components",
-            "flat-detector-chirp-mass-ratio",
-            "flat-detector",
-            "chirp-mass",
-        ],
+        type=str,
         help=(
             "Mass prior used during the initial sampling, must match one of the following options. "
             "\n 'flat-detector': Flat in detector frame primary and secondary masses. "
             "\n 'chirp-mass': Flat in detector frame chirp mass and mass ratio. "
             "\n 'flat-detector-components': Flat in detector frame primary and secondary masses. "
             "This is the default for LVK samples and the same as the deprecated 'flat-detector' option. "
             "\n 'flat-source-components': Flat in source frame primary and secondary masses. "
             "\n 'flat-detector-chirp-mass-ratio': Flat in detector frame chirp mass and mass ratio. "
-            "This is the same as the deprecated 'chirp-mass' option."
+            "This is the same as the deprecated 'chirp-mass' option. Can be in the format of a dict with the same keys as the sample-regex"
         ),
     )
     collection_parser.add_argument(
         "--spin-prior",
         default="component",
-        choices=["component"],
+        type=str,
         help=(
             "Spin prior, the only supported spin prior assumes the spins are isotropically distributed "
-            "with a flat prior on the magnitude. "
+            "with a flat prior on the magnitude. Can be in the format of a dict with the same keys as the sample-regex."
         ),
     )
 
     analysis_parser = parser.add_argument_group(
         title="Arguments describing analysis jobs", description="Analysis arguments"
     )
     analysis_parser.add_argument(
```

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/pesumary_plot.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/pesumary_plot.py`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/post_plots.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/post_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,15 +353,15 @@
                 mass_1, injected_mass_1, color="k", label="True", linestyle="--"
             )
             axs[1].plot(mass_ratio, injected_mass_ratio, color="k", linestyle="--")
 
     axs[0].set_xlim(2, 100)
     axs[0].set_ylim(peak_1 / 100000, peak_1 * 1.1)
     axs[0].set_xlabel("$m_{1}$ [$M_{\\odot}$]")
-    axs[0].legend(loc="best")
+    axs[0].legend(bbox_to_anchor=(0.5, 1.15), loc="upper center")
     if rate:
         ylabel = "$\\frac{d\\mathcal{R}}{dm_{1}}$ [Gpc$^{-3}$yr$^{-1}M_{\\odot}^{-1}$]"
     else:
         ylabel = "$p(m_{1})$ [$M_{\\odot}^{-1}$]"
     axs[0].set_ylabel(ylabel)
 
     axs[1].set_xlim(0.1, 1)
@@ -375,15 +375,15 @@
 
     if len(results) == 1:
         file_name = f"{result.outdir}/{result.label}_mass_spectrum.pdf"
     else:
         file_name = f"{result.outdir}/combined_mass_spectrum.pdf"
     plt.tight_layout()
     if save:
-        plt.savefig(file_name, format="pdf", dpi=600)
+        plt.savefig(file_name, format="pdf", dpi=600, bbox_inches="tight")
         plt.close()
         return ppd
     else:
         return fig
 
 
 def spin_magnitude_spectrum_plot(results, args, rate=False, save=True):
@@ -514,23 +514,22 @@
         axs[ii - 1].set_ylim(0)
         axs[ii - 1].set_xlabel(f"$a_{ii}$")
         if rate:
             ylabel = f"$\\frac{{dN}}{{da_{ii}}}$"
         else:
             ylabel = f"$p(a_{ii})$"
         axs[ii - 1].set_ylabel(ylabel)
-    axs[0].legend(loc="best")
+    axs[0].legend(bbox_to_anchor=(0.5, 1.15), loc="upper center")
 
     if len(results) == 1:
         file_name = f"{result.outdir}/{result.label}_magnitude_spectrum.pdf"
     else:
         file_name = f"{result.outdir}/comparison_magnitude_spectrum.pdf"
-    plt.tight_layout()
     if save:
-        plt.savefig(file_name, format="pdf", dpi=600)
+        plt.savefig(file_name, format="pdf", dpi=600, bbox_inches="tight")
         plt.close()
         return ppd
     else:
         return fig
 
 
 def spin_orientation_spectrum_plot(results, args, rate=False, save=True):
@@ -657,23 +656,22 @@
     else:
         ylabel = "$p(\\cos t_{})$"
     for ii in [1, 2]:
         axs[ii - 1].set_xlim(-1, 1)
         axs[ii - 1].set_ylim(0)
         axs[ii - 1].set_xlabel(f"$\\cos t_{ii}$")
         axs[ii - 1].set_ylabel(ylabel.format(str(ii)))
-    axs[0].legend(loc="best")
+    axs[0].legend(bbox_to_anchor=(0.5, 1.15), loc="upper center")
 
     if len(results) == 1:
         file_name = f"{result.outdir}/{result.label}_orientation_spectrum.pdf"
     else:
         file_name = f"{result.outdir}/comparison_orientation_spectrum.pdf"
-    plt.tight_layout()
     if save:
-        plt.savefig(file_name, format="pdf", dpi=600)
+        plt.savefig(file_name, format="pdf", dpi=600, bbox_inches="tight")
         plt.close()
         return ppd
     else:
         return fig
 
 
 def redshift_spectrum_plot(results, args, rate=True, save=True):
@@ -763,23 +761,22 @@
         ylabel = "$\\mathcal{R}(z)$ [Gpc$^{-3}$yr$^{-1}$]"
     else:
         ylabel = "$\\frac{R(z)}{R(z=0)}$"
     ax.set_xlim(0, 2.3)
     ax.set_yscale("log")
     ax.set_xlabel("$z$")
     ax.set_ylabel(ylabel)
-    ax.legend(loc="best")
+    ax.legend(bbox_to_anchor=(0.5, 1.15), loc="upper center")
 
     if len(results) == 1:
         file_name = f"{result.outdir}/{result.label}_redshift_spectrum.pdf"
     else:
         file_name = f"{result.outdir}/comparison_redshift_spectrum.pdf"
-    plt.tight_layout()
     if save:
-        plt.savefig(file_name, format="pdf", dpi=600)
+        plt.savefig(file_name, format="pdf", dpi=600, bbox_inches="tight")
         plt.close()
         return ppd
     else:
         return fig
 
 
 def reweighted_comparison(data, outdir="outdir"):
```

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/review.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/review.py`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/utils.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/utils.py`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe/vt_helper.py` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe/vt_helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 
+import argparse
+
 import dill
 import h5py
 import numpy as np
 from bilby.core.utils import logger
 
 from gwpopulation.utils import xp
 from gwpopulation.vt import GridVT, ResamplingVT
@@ -77,15 +79,15 @@
     a_2: np.ndarray
     cos_tilt_1: np.ndarray
     cos_tilt_2: np.ndarray
     redshift: np.ndarray
     prior: np.ndarray
     total_generated: int
     analysis_time: float
-    mass_2: np.ndarray = field(default=None, init=False)
+    mass_2: np.ndarray = field(default=None)
 
     def append(self, other):
         self_sample_rate = self.analysis_time / self.total_generated
         other_sample_rate = other.analysis_time / other.total_generated
         self_weight = 2 * self_sample_rate / (self_sample_rate + other_sample_rate)
         other_weight = 2 * other_sample_rate / (self_sample_rate + other_sample_rate)
         for key in self.__dataclass_fields__:
@@ -126,14 +128,19 @@
 
     def items(self):
         return self.__dict__.items()
 
     def get(self, key, alt):
         return self.__dict__.get(key, alt)
 
+    def to_dict(self, keys=None):
+        if keys is None:
+            keys = list(self.__dict__.keys())
+        return {key: getattr(self, key) for key in keys}
+
 
 def load_injection_data(vt_file, ifar_threshold=1, snr_threshold=11):
     """
     Load the injection file in the O3 injection file format.
 
     For mixture files and multiple observing run files we only
     have the full `sampling_pdf`.
@@ -170,28 +177,33 @@
     logger.info(f"Loading VT data from {vt_file}.")
     if vt_file.endswith(".pkl"):
         with open(vt_file, "rb") as ff:
             data = dill.load(ff)
         for key, value in data.items():
             if isinstance(value, np.ndarray):
                 data[key] = xp.asarray(value)
-        return data
+        return VTData(**data)
 
     with h5py.File(vt_file, "r") as ff:
         if "injections" in ff:
             data = ff["injections"]
             total_generated = int(data.attrs["total_generated"][()])
             analysis_time = data.attrs["analysis_time_s"][()] / 365.25 / 24 / 60 / 60
         elif "events" in ff:
             import pandas as pd
 
             data = pd.DataFrame(ff["events"][()]).to_dict(orient="list")
             data = {key: np.array(value) for key, value in data.items()}
             total_generated = int(ff.attrs["total_generated"][()])
-            analysis_time = ff.attrs["total_analysis_time"][()] / 365.25 / 24 / 60 / 60
+            try:
+                analysis_time = (
+                    ff.attrs["total_analysis_time"][()] / 365.25 / 24 / 60 / 60
+                )
+            except KeyError:
+                analysis_time = ff.attrs["analysis_time"][()] / 365.25 / 24 / 60 / 60
             if analysis_time == 0:
                 analysis_time = 1 / 12
         else:
             raise KeyError(f"Unable to identify injections from {ff.keys()}")
 
         if "mass1_source" in data:
             mass_1_key = "mass1_source"
@@ -199,15 +211,16 @@
         else:
             mass_1_key = "mass_1_source"
             mass_2_key = "mass_2_source"
         if "redshift" in data:
             redshift_key = "redshift"
         else:
             redshift_key = "z"
-        found = get_found_injections(data, ifar_threshold, snr_threshold)
+        found_shape = data[mass_1_key][()].shape
+        found = get_found_injections(data, found_shape, ifar_threshold, snr_threshold)
         n_found = sum(found)
         if n_found == 0:
             raise ValueError("No sensitivity injections pass threshold.")
         gwpop_data = dict(
             mass_1=xp.asarray(data[mass_1_key][()][found]),
             mass_ratio=xp.asarray(
                 data[mass_2_key][()][found] / data[mass_1_key][()][found]
@@ -224,22 +237,38 @@
                     + data[f"spin{ii}z"][()][found] ** 2
                 )
                 ** 0.5
             )
             gwpop_data[f"cos_tilt_{ii}"] = (
                 xp.asarray(data[f"spin{ii}z"][()][found]) / gwpop_data[f"a_{ii}"]
             )
-        if "sampling_pdf" in data:
+        if (
+            "sampling_pdf" in data
+        ):  # O1+O2+O3 mixture and endO3 injections (https://dcc.ligo.org/LIGO-T2100377, https://dcc.ligo.org/LIGO-T2100113)
             gwpop_data["prior"] = (
                 xp.asarray(data["sampling_pdf"][()][found])
                 * xp.asarray(data[mass_1_key][()][found])
                 * (2 * np.pi * gwpop_data["a_1"] ** 2)
                 * (2 * np.pi * gwpop_data["a_2"] ** 2)
             )
-        else:
+        elif (
+            "lnpdraw_mass1_source_mass2_source_redshift_spin1x_spin1y_spin1z_spin2x_spin2y_spin2z"
+            in data
+        ):  # O1+O2+O3+O4a mixture (https://dcc.ligo.org/LIGO-T2400110)
+            gwpop_data["prior"] = xp.exp(
+                xp.asarray(
+                    data[
+                        "lnpdraw_mass1_source_mass2_source_redshift_spin1x_spin1y_spin1z_spin2x_spin2y_spin2z"
+                    ][()][found]
+                )
+                + xp.log(xp.asarray(data[mass_1_key][()][found]))
+                + xp.log(2 * np.pi * gwpop_data["a_1"] ** 2)
+                + xp.log(2 * np.pi * gwpop_data["a_2"] ** 2)
+            )
+        else:  # O4a sensitivity injections (https://dcc.ligo.org/LIGO-T2400073)
             gwpop_data["prior"] = xp.exp(
                 xp.sum(
                     [
                         xp.asarray(data[f"lnpdraw_{key}"][()][found])
                         for key in [
                             "mass1_source",
                             "mass2_source_GIVEN_mass1_source",
@@ -252,41 +281,121 @@
                     ],
                     axis=0,
                 )
             )
             gwpop_data["prior"] /= xp.sin(xp.arccos(gwpop_data["cos_tilt_1"]))
             gwpop_data["prior"] /= xp.sin(xp.arccos(gwpop_data["cos_tilt_2"]))
             gwpop_data["prior"] *= gwpop_data["mass_1"]
+
+        weights = 1
         if "v1_1ifo" in vt_file:
-            gwpop_data["prior"] /= data["weights_1ifo"][()][found]
+            weights *= data["weights_1ifo"][()][found]
+        elif "weights" in data:
+            weights *= data["weights"][()][found]
+        gwpop_data["prior"] /= weights
     return VTData(**gwpop_data)
 
 
-def get_found_injections(data, ifar_threshold=1, snr_threshold=11):
-    found = np.zeros_like(data["mass_1"], dtype=bool)
-    if ifar_threshold is not None and "ifar" in any(
-        [key.lower() for key in data.keys()]
+def get_found_injections(data, shape, ifar_threshold=1, snr_threshold=11):
+    found = np.zeros(shape, dtype=bool)
+    has_ifar = any(["ifar" in key.lower() for key in data.keys()])
+    if not has_ifar and any(
+        [key for key in data.keys() if key.lower().startswith("far_")]
     ):
+        far_keys = [key for key in data.keys() if key.lower().startswith("far_")]
+        for far_key in far_keys:
+            data[f"i{far_key}"] = 1 / data[far_key][()]
+        has_ifar = True
+    if ifar_threshold is None:
+        ifar_threshold = 1e300
+    if has_ifar:
         for key in data:
             if "ifar" in key.lower():
-                found = found | (data[key] > ifar_threshold)
+                found |= data[key][()] > ifar_threshold
             if "name" in data.keys():
-                gwtc1 = (data["name"] == b"o1") | (data["name"] == b"o2")
-                found = found | (gwtc1 & (data["optimal_snr_net"] > snr_threshold))
+                gwtc1 = (data["name"][()] == b"o1") | (data["name"][()] == b"o2")
+                found |= gwtc1 & (data["optimal_snr_net"][()] > snr_threshold)
+        if "semianalytic_observed_phase_maximized_snr_net" in data.keys():
+            found |= (
+                data["semianalytic_observed_phase_maximized_snr_net"][()]
+                > snr_threshold
+            )
         return found
     elif snr_threshold is not None:
         if "observed_phase_maximized_snr_net" in data.keys():
-            found = found | (data["observed_phase_maximized_snr_net"] > snr_threshold)
+            found |= data["observed_phase_maximized_snr_net"][()] > snr_threshold
         elif "observed_snr_net" in data.keys():
-            found = found | (data["observed_snr_net"] > snr_threshold)
+            found |= data["observed_snr_net"][()] > snr_threshold
         return found
     else:
         raise ValueError("Cannot find keys to filter sensitivity injections.")
 
 
+def apply_injection_prior(data, parameters):
+    """
+    We assume the injection prior is uniform in the detector frame primary
+    mass and mass ratio.
+    """
+    if "mass_2" in parameters:
+        data["mass_2"] = data["mass_1"] * data["mass_ratio"]
+        data["prior"] /= data["mass_1"]
+    if "chirp_mass" in parameters:
+        jacobian = primary_mass_to_chirp_mass_jacobian(data)
+        data["chirp_mass"] = data["mass_1"] / jacobian
+        data["prior"] *= jacobian
+    if "chi_1" in parameters:
+        data["chi_1"] = data["a_1"] * data["cos_tilt_1"]
+        data["prior"] *= 2 * aligned_spin_prior(data["chi_1"])
+    if "chi_2" in parameters:
+        data["chi_2"] = data["a_2"] * data["cos_tilt_2"]
+        data["prior"] *= 2 * aligned_spin_prior(data["chi_2"])
+
+
+def dump_injection_data(args, save_filename=None):
+    """
+    Dump the injection data to a pickle file to :code:`{args.run_dir}/data/injections.pkl` for easier file transfer.
+
+    This also makes sure the required parameters are present in the data and updates the prior accordingly.
+
+    Parameters
+    ----------
+    args:
+        Command-line arguments
+    save_filename:
+        The filename to save the data to. If None, it will save the data to args.run_dir/data/injections.pkl.
+    """
+    if "*" in args.vt_file:
+        data = reduce(
+            lambda x, y: x + y,
+            [
+                load_injection_data(
+                    vt_file=get_path_or_local(vt_file),
+                    ifar_threshold=args.vt_ifar_threshold,
+                    snr_threshold=args.vt_snr_threshold,
+                )
+                for vt_file in glob.glob(args.vt_file)
+            ],
+        )
+    else:
+        data = load_injection_data(
+            vt_file=get_path_or_local(args.vt_file),
+            ifar_threshold=args.vt_ifar_threshold,
+            snr_threshold=args.vt_snr_threshold,
+        )
+    apply_injection_prior(data, args.parameters)
+    if save_filename is None:
+        fname = f"{args.run_dir}/data/injections.pkl"
+    else:
+        fname = save_filename
+    data_dict = data.to_dict()
+    with open(fname, "wb") as ff:
+        dill.dump(data_dict, ff)
+    logger.info(f"Written injection data to {fname}")
+
+
 def injection_resampling_vt(vt_file, model, ifar_threshold=1, snr_threshold=11):
     import glob
 
     if "*" in vt_file:
         vt_files = glob.glob(vt_file)
         data = sum(
             [
@@ -314,7 +423,76 @@
 
     data = load_injection_data(
         vt_file=vt_file, ifar_threshold=ifar_threshold, snr_threshold=snr_threshold
     )
     data["prior"] = data["mass_1"] ** (-2.35 + 1) * data["mass_ratio"] ** 2
 
     return ResamplingVT(model=model, data=data, n_events=N_EVENTS)
+
+
+def create_injection_parser():
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "vt_file",
+        type=str,
+        help="File to load VT data from or a glob string matching multiple files to combine.",
+    )
+
+    parser.add_argument(
+        "--vt-ifar-threshold",
+        type=float,
+        default=1,
+        help="IFAR threshold for resampling injections",
+    )
+    parser.add_argument(
+        "--vt-snr-threshold",
+        type=float,
+        default=11,
+        help="SNR threshold for resampling injections. "
+        "This is only used for O1/O2 injections",
+    )
+    parser.add_argument(
+        "--vt-function",
+        type=str,
+        default="injection_resampling_vt",
+        help="Function to generate selection function from.",
+    )
+
+    parser.add_argument(
+        "--parameters",
+        "-p",
+        action="append",
+        help=(
+            "Parameters that are fit with the model. "
+            "These are the parameters that will be extracted from the injections "
+            "and should follow Bilby naming conventions with the exception that all masses "
+            "are assumed to be in the source frame. Here is a list of parameters for which "
+            "prior factors will be properly accounted. "
+            "mass_1: source frame primary mass, mass_2: source frame secondary mass, "
+            "chirp_mass: source frame chirp mass, mass_ratio: mass ratio, redshift: redshift, "
+            "a_1: primary spin magnitude, a_2: secondary spin magnitude, cos_tilt_1: "
+            "cosine primary spin tilt, cos_tilt_2: cosine secondary spin tilt, "
+            "chi_1: aligned primary spin, chi_2: aligned secondary spin."
+            "Any other parameters will be assumed to have a flat prior."
+            "These parameters are also used to set the fiducial prior values. "
+            "No redundancy checks are performed so users should be careful to not "
+            "include unused parameters as that may have unintended consequences."
+        ),
+    )
+
+    parser.add_argument(
+        "--save_as",
+        "-s",
+        type=str,
+        default="injections.pkl",
+        help="name of pickle file to save the injections",
+    )
+
+    return parser
+
+
+def read_injections():
+    parser = create_injection_parser()
+    args = parser.parse_args()
+    save_file = args.save_as
+    save_file = save_file.split(".pkl")[0] + ".pkl"
+    dump_injection_data(args, save_file)
```

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe.egg-info/PKG-INFO` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpopulation_pipe
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: A pipeline population inference
 Home-page: https://git.ligo.org/RatesAndPopulations/gwpopulation_pipe
 Author: Colm Talbot
 Author-email: colm.talbot@ligo.org
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe.egg-info/SOURCES.txt` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwpopulation_pipe-0.4.0rc1/gwpopulation_pipe.egg-info/entry_points.txt` & `gwpopulation_pipe-0.4.0rc2/gwpopulation_pipe.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [console_scripts]
 gwpopulation_pipe = gwpopulation_pipe.main:main
 gwpopulation_pipe_analysis = gwpopulation_pipe.data_analysis:main
 gwpopulation_pipe_collection = gwpopulation_pipe.data_collection:main
 gwpopulation_pipe_plot = gwpopulation_pipe.post_plots:main
 gwpopulation_pipe_pp_test = gwpopulation_pipe.review:setup_pp_test
+gwpopulation_pipe_read_injections = gwpopulation_pipe.vt_helper:read_injections
 gwpopulation_pipe_simulate_posteriors = gwpopulation_pipe.data_simulation:main
 gwpopulation_pipe_to_common_format = gwpopulation_pipe.common_format:main
 
 [gwpopulation.xp]
 format = gwpopulation_pipe.common_format
 plot = gwpopulation_pipe.post_plots
 simulate = gwpopulation_pipe.data_simulation
```

### Comparing `gwpopulation_pipe-0.4.0rc1/setup.cfg` & `gwpopulation_pipe-0.4.0rc2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 	gwpopulation_pipe = gwpopulation_pipe.main:main
 	gwpopulation_pipe_analysis = gwpopulation_pipe.data_analysis:main
 	gwpopulation_pipe_collection = gwpopulation_pipe.data_collection:main
 	gwpopulation_pipe_plot = gwpopulation_pipe.post_plots:main
 	gwpopulation_pipe_pp_test = gwpopulation_pipe.review:setup_pp_test
 	gwpopulation_pipe_simulate_posteriors = gwpopulation_pipe.data_simulation:main
 	gwpopulation_pipe_to_common_format = gwpopulation_pipe.common_format:main
+	gwpopulation_pipe_read_injections = gwpopulation_pipe.vt_helper:read_injections
 gwpopulation.xp = 
 	format = gwpopulation_pipe.common_format
 	simulate = gwpopulation_pipe.data_simulation
 	plot = gwpopulation_pipe.post_plots
 	utils = gwpopulation_pipe.utils
 	vt = gwpopulation_pipe.vt_helper
```

