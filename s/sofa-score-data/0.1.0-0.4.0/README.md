# Comparing `tmp/sofa_score_data-0.1.0.tar.gz` & `tmp/sofa_score_data-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sofa_score_data-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sofa_score_data-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sofa_score_data-0.1.0.tar` & `sofa_score_data-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0      342 2024-05-11 03:18:47.183236 sofa_score_data-0.1.0/README.md
--rw-r--r--   0        0        0      451 2024-05-11 03:18:47.183236 sofa_score_data-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8959 2024-05-11 03:18:47.183236 sofa_score_data-0.1.0/sofa_score_data/Scraper_Sofascore.py
--rw-r--r--   0        0        0      230 2024-05-11 03:18:47.183236 sofa_score_data-0.1.0/sofa_score_data/__init__.py
--rw-r--r--   0        0        0      521 2024-05-11 03:18:47.183236 sofa_score_data-0.1.0/sofa_score_data/fotmob.py
--rw-r--r--   0        0        0      248 2024-05-11 03:18:47.183236 sofa_score_data-0.1.0/sofa_score_data/match_details_info.py
--rw-r--r--   0        0        0       76 2024-05-11 03:18:47.183236 sofa_score_data-0.1.0/sofa_score_data/transformations.py
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 sofa_score_data-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      196 2024-03-20 03:53:22.984572 sofa_score_data-0.4.0/README.md
+-rw-r--r--   0        0        0      418 2024-03-20 03:53:22.984572 sofa_score_data-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13162 2024-03-20 03:53:22.984572 sofa_score_data-0.4.0/sofa_score_data/Scraper_Sofascore.py
+-rw-r--r--   0        0        0      102 2024-03-20 03:53:22.984572 sofa_score_data-0.4.0/sofa_score_data/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-20 03:53:22.984572 sofa_score_data-0.4.0/sofa_score_data/transformations.py
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 sofa_score_data-0.4.0/PKG-INFO
```

