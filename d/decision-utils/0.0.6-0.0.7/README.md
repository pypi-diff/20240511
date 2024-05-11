# Comparing `tmp/decision_utils-0.0.6.tar.gz` & `tmp/decision_utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decision_utils-0.0.6.tar", last modified: Sat May  4 01:30:17 2024, max compression
+gzip compressed data, was "decision_utils-0.0.7.tar", last modified: Sat May 11 11:37:54 2024, max compression
```

## Comparing `decision_utils-0.0.6.tar` & `decision_utils-0.0.7.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.839624 decision_utils-0.0.6/
--rw-r--r--   0 mv         (501) staff       (20)      832 2024-05-04 01:30:17.839250 decision_utils-0.0.6/PKG-INFO
--rw-r--r--   0 mv         (501) staff       (20)     7388 2024-05-04 01:29:37.000000 decision_utils-0.0.6/README.md
--rw-r--r--   0 mv         (501) staff       (20)     1284 2024-05-04 01:29:37.000000 decision_utils-0.0.6/pyproject.toml
--rw-r--r--   0 mv         (501) staff       (20)       38 2024-05-04 01:30:17.839701 decision_utils-0.0.6/setup.cfg
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.808068 decision_utils-0.0.6/src/
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.812624 decision_utils-0.0.6/src/decision_fetcher/
--rw-r--r--   0 mv         (501) staff       (20)      104 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)     1670 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/__main__.py
--rw-r--r--   0 mv         (501) staff       (20)     2538 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/config.py
--rw-r--r--   0 mv         (501) staff       (20)     7075 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/dissect.py
--rw-r--r--   0 mv         (501) staff       (20)    14966 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/draft.py
--rw-r--r--   0 mv         (501) staff       (20)     4640 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/items.py
--rw-r--r--   0 mv         (501) staff       (20)     1364 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/logger.py
--rw-r--r--   0 mv         (501) staff       (20)     1220 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/sanitize.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.818481 decision_utils-0.0.6/src/decision_fetcher_fields/
--rw-r--r--   0 mv         (501) staff       (20)      597 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)      963 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/citation.py
--rw-r--r--   0 mv         (501) staff       (20)     3057 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/cullables.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.819459 decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/
--rw-r--r--   0 mv         (501) staff       (20)      138 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)      469 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/ordered.py
--rw-r--r--   0 mv         (501) staff       (20)     2492 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/phrases.py
--rw-r--r--   0 mv         (501) staff       (20)     1658 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/wherefore.py
--rw-r--r--   0 mv         (501) staff       (20)      893 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/footnotes.py
--rw-r--r--   0 mv         (501) staff       (20)     1626 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/header.py
--rw-r--r--   0 mv         (501) staff       (20)     1092 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling.py
--rw-r--r--   0 mv         (501) staff       (20)      891 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_cues.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.824996 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/
--rw-r--r--   0 mv         (501) staff       (20)      415 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)      229 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/after_review.py
--rw-r--r--   0 mv         (501) staff       (20)      688 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/court_acts.py
--rw-r--r--   0 mv         (501) staff       (20)     1554 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/court_admin.py
--rw-r--r--   0 mv         (501) staff       (20)     1098 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/granted_denied.py
--rw-r--r--   0 mv         (501) staff       (20)      664 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/hence_this.py
--rw-r--r--   0 mv         (501) staff       (20)     1647 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/issue_errors.py
--rw-r--r--   0 mv         (501) staff       (20)      187 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/issue_resolution.py
--rw-r--r--   0 mv         (501) staff       (20)      874 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/main_issue.py
--rw-r--r--   0 mv         (501) staff       (20)      411 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/merit.py
--rw-r--r--   0 mv         (501) staff       (20)      459 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/resolve_issue.py
--rw-r--r--   0 mv         (501) staff       (20)      270 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/single_issue.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.827545 decision_utils-0.0.6/src/decision_fetcher_fields/tags/
--rw-r--r--   0 mv         (501) staff       (20)      185 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/tags/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)     1450 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/tags/base.py
--rw-r--r--   0 mv         (501) staff       (20)     1452 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/tags/specific.py
--rw-r--r--   0 mv         (501) staff       (20)      987 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/tags/utils.py
--rw-r--r--   0 mv         (501) staff       (20)     3823 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/title_tags.py
--rw-r--r--   0 mv         (501) staff       (20)      183 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/utils.py
--rw-r--r--   0 mv         (501) staff       (20)      825 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/voteline.py
--rw-r--r--   0 mv         (501) staff       (20)     1022 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/writer.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.829731 decision_utils-0.0.6/src/decision_updater/
--rw-r--r--   0 mv         (501) staff       (20)      283 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_updater/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)     1139 2024-02-16 17:00:02.000000 decision_utils-0.0.6/src/decision_updater/__main__.py
--rw-r--r--   0 mv         (501) staff       (20)     3247 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_updater/clean.py
--rw-r--r--   0 mv         (501) staff       (20)      437 2024-02-08 03:12:00.000000 decision_utils-0.0.6/src/decision_updater/dumper.py
--rw-r--r--   0 mv         (501) staff       (20)     1364 2024-02-08 03:12:00.000000 decision_utils-0.0.6/src/decision_updater/logger.py
--rw-r--r--   0 mv         (501) staff       (20)     1164 2024-02-08 08:16:42.000000 decision_utils-0.0.6/src/decision_updater/md.py
--rw-r--r--   0 mv         (501) staff       (20)     4129 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_updater/writer.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.831728 decision_utils-0.0.6/src/decision_utils/
--rw-r--r--   0 mv         (501) staff       (20)      201 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_utils/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)       13 2024-02-08 03:41:37.000000 decision_utils-0.0.6/src/decision_utils/__main__.py
--rw-r--r--   0 mv         (501) staff       (20)     2915 2023-10-13 13:27:11.000000 decision_utils-0.0.6/src/decision_utils/author.py
--rw-r--r--   0 mv         (501) staff       (20)     7698 2024-01-29 02:03:38.000000 decision_utils-0.0.6/src/decision_utils/block.py
--rw-r--r--   0 mv         (501) staff       (20)    10486 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_utils/decision.py
--rw-r--r--   0 mv         (501) staff       (20)    10760 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_utils/opinion.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.836876 decision_utils-0.0.6/src/decision_utils/utils/
--rw-r--r--   0 mv         (501) staff       (20)      259 2023-10-29 05:19:46.000000 decision_utils-0.0.6/src/decision_utils/utils/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)     4624 2023-10-25 02:47:41.000000 decision_utils-0.0.6/src/decision_utils/utils/annex.py
--rw-r--r--   0 mv         (501) staff       (20)      410 2023-10-19 05:38:51.000000 decision_utils-0.0.6/src/decision_utils/utils/casename.py
--rw-r--r--   0 mv         (501) staff       (20)     5184 2023-10-16 09:49:26.000000 decision_utils-0.0.6/src/decision_utils/utils/courts.py
--rw-r--r--   0 mv         (501) staff       (20)      437 2023-10-14 10:37:51.000000 decision_utils-0.0.6/src/decision_utils/utils/dumper.py
--rw-r--r--   0 mv         (501) staff       (20)     2876 2023-10-18 03:38:31.000000 decision_utils-0.0.6/src/decision_utils/utils/fallo.py
--rw-r--r--   0 mv         (501) staff       (20)     3254 2024-02-17 08:40:03.000000 decision_utils-0.0.6/src/decision_utils/utils/formatter.py
--rw-r--r--   0 mv         (501) staff       (20)     1059 2024-02-06 22:04:26.000000 decision_utils-0.0.6/src/decision_utils/utils/md.py
--rw-r--r--   0 mv         (501) staff       (20)     5639 2023-10-24 14:52:02.000000 decision_utils-0.0.6/src/decision_utils/utils/phrase.py
--rw-r--r--   0 mv         (501) staff       (20)      846 2023-10-14 10:38:30.000000 decision_utils-0.0.6/src/decision_utils/utils/regex.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.838132 decision_utils-0.0.6/src/decision_utils.egg-info/
--rw-r--r--   0 mv         (501) staff       (20)      832 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/PKG-INFO
--rw-r--r--   0 mv         (501) staff       (20)     2870 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/SOURCES.txt
--rw-r--r--   0 mv         (501) staff       (20)        1 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/dependency_links.txt
--rw-r--r--   0 mv         (501) staff       (20)      128 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/entry_points.txt
--rw-r--r--   0 mv         (501) staff       (20)      309 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/requires.txt
--rw-r--r--   0 mv         (501) staff       (20)       90 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/top_level.txt
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.837657 decision_utils-0.0.6/src/decision_watcher/
--rw-r--r--   0 mv         (501) staff       (20)       24 2024-02-08 03:40:51.000000 decision_utils-0.0.6/src/decision_watcher/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)     2322 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_watcher/__main__.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.322221 decision_utils-0.0.7/
+-rw-r--r--   0 mv         (501) staff       (20)      832 2024-05-11 11:37:54.321827 decision_utils-0.0.7/PKG-INFO
+-rw-r--r--   0 mv         (501) staff       (20)     8267 2024-05-11 04:05:08.000000 decision_utils-0.0.7/README.md
+-rw-r--r--   0 mv         (501) staff       (20)     1284 2024-05-11 11:36:26.000000 decision_utils-0.0.7/pyproject.toml
+-rw-r--r--   0 mv         (501) staff       (20)       38 2024-05-11 11:37:54.322292 decision_utils-0.0.7/setup.cfg
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.290532 decision_utils-0.0.7/src/
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.296356 decision_utils-0.0.7/src/decision_fetcher/
+-rw-r--r--   0 mv         (501) staff       (20)      104 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     1670 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher/__main__.py
+-rw-r--r--   0 mv         (501) staff       (20)     2538 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher/config.py
+-rw-r--r--   0 mv         (501) staff       (20)     7075 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher/dissect.py
+-rw-r--r--   0 mv         (501) staff       (20)    14966 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher/draft.py
+-rw-r--r--   0 mv         (501) staff       (20)     4710 2024-05-11 02:35:52.000000 decision_utils-0.0.7/src/decision_fetcher/items.py
+-rw-r--r--   0 mv         (501) staff       (20)     1364 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher/logger.py
+-rw-r--r--   0 mv         (501) staff       (20)     1220 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher/sanitize.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.302107 decision_utils-0.0.7/src/decision_fetcher_fields/
+-rw-r--r--   0 mv         (501) staff       (20)      597 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)      963 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/citation.py
+-rw-r--r--   0 mv         (501) staff       (20)     3057 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/cullables.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.303111 decision_utils-0.0.7/src/decision_fetcher_fields/dispositive/
+-rw-r--r--   0 mv         (501) staff       (20)      138 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/dispositive/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)      469 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/dispositive/ordered.py
+-rw-r--r--   0 mv         (501) staff       (20)     2492 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/dispositive/phrases.py
+-rw-r--r--   0 mv         (501) staff       (20)     1658 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/dispositive/wherefore.py
+-rw-r--r--   0 mv         (501) staff       (20)      893 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/footnotes.py
+-rw-r--r--   0 mv         (501) staff       (20)     1626 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/header.py
+-rw-r--r--   0 mv         (501) staff       (20)     1092 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling.py
+-rw-r--r--   0 mv         (501) staff       (20)      891 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_cues.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.307023 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/
+-rw-r--r--   0 mv         (501) staff       (20)      415 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)      229 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/after_review.py
+-rw-r--r--   0 mv         (501) staff       (20)      688 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/court_acts.py
+-rw-r--r--   0 mv         (501) staff       (20)     1554 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/court_admin.py
+-rw-r--r--   0 mv         (501) staff       (20)     1098 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/granted_denied.py
+-rw-r--r--   0 mv         (501) staff       (20)      664 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/hence_this.py
+-rw-r--r--   0 mv         (501) staff       (20)     1647 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/issue_errors.py
+-rw-r--r--   0 mv         (501) staff       (20)      187 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/issue_resolution.py
+-rw-r--r--   0 mv         (501) staff       (20)      874 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/main_issue.py
+-rw-r--r--   0 mv         (501) staff       (20)      411 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/merit.py
+-rw-r--r--   0 mv         (501) staff       (20)      459 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/resolve_issue.py
+-rw-r--r--   0 mv         (501) staff       (20)      270 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/single_issue.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.310116 decision_utils-0.0.7/src/decision_fetcher_fields/tags/
+-rw-r--r--   0 mv         (501) staff       (20)      185 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/tags/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     1450 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/tags/base.py
+-rw-r--r--   0 mv         (501) staff       (20)     1452 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/tags/specific.py
+-rw-r--r--   0 mv         (501) staff       (20)      987 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/tags/utils.py
+-rw-r--r--   0 mv         (501) staff       (20)     3823 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/title_tags.py
+-rw-r--r--   0 mv         (501) staff       (20)      183 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/utils.py
+-rw-r--r--   0 mv         (501) staff       (20)      825 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/voteline.py
+-rw-r--r--   0 mv         (501) staff       (20)     1022 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_fetcher_fields/writer.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.312809 decision_utils-0.0.7/src/decision_updater/
+-rw-r--r--   0 mv         (501) staff       (20)      283 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_updater/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     1139 2024-02-16 17:00:02.000000 decision_utils-0.0.7/src/decision_updater/__main__.py
+-rw-r--r--   0 mv         (501) staff       (20)     3247 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_updater/clean.py
+-rw-r--r--   0 mv         (501) staff       (20)      437 2024-02-08 03:12:00.000000 decision_utils-0.0.7/src/decision_updater/dumper.py
+-rw-r--r--   0 mv         (501) staff       (20)     1364 2024-02-08 03:12:00.000000 decision_utils-0.0.7/src/decision_updater/logger.py
+-rw-r--r--   0 mv         (501) staff       (20)     1164 2024-02-08 08:16:42.000000 decision_utils-0.0.7/src/decision_updater/md.py
+-rw-r--r--   0 mv         (501) staff       (20)     4148 2024-05-11 04:27:25.000000 decision_utils-0.0.7/src/decision_updater/writer.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.314980 decision_utils-0.0.7/src/decision_utils/
+-rw-r--r--   0 mv         (501) staff       (20)      201 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_utils/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)       13 2024-02-08 03:41:37.000000 decision_utils-0.0.7/src/decision_utils/__main__.py
+-rw-r--r--   0 mv         (501) staff       (20)     2915 2023-10-13 13:27:11.000000 decision_utils-0.0.7/src/decision_utils/author.py
+-rw-r--r--   0 mv         (501) staff       (20)     7698 2024-01-29 02:03:38.000000 decision_utils-0.0.7/src/decision_utils/block.py
+-rw-r--r--   0 mv         (501) staff       (20)    10486 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_utils/decision.py
+-rw-r--r--   0 mv         (501) staff       (20)    10760 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_utils/opinion.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.319767 decision_utils-0.0.7/src/decision_utils/utils/
+-rw-r--r--   0 mv         (501) staff       (20)      259 2023-10-29 05:19:46.000000 decision_utils-0.0.7/src/decision_utils/utils/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     4624 2023-10-25 02:47:41.000000 decision_utils-0.0.7/src/decision_utils/utils/annex.py
+-rw-r--r--   0 mv         (501) staff       (20)      410 2023-10-19 05:38:51.000000 decision_utils-0.0.7/src/decision_utils/utils/casename.py
+-rw-r--r--   0 mv         (501) staff       (20)     5184 2023-10-16 09:49:26.000000 decision_utils-0.0.7/src/decision_utils/utils/courts.py
+-rw-r--r--   0 mv         (501) staff       (20)      437 2023-10-14 10:37:51.000000 decision_utils-0.0.7/src/decision_utils/utils/dumper.py
+-rw-r--r--   0 mv         (501) staff       (20)     2876 2023-10-18 03:38:31.000000 decision_utils-0.0.7/src/decision_utils/utils/fallo.py
+-rw-r--r--   0 mv         (501) staff       (20)     3254 2024-02-17 08:40:03.000000 decision_utils-0.0.7/src/decision_utils/utils/formatter.py
+-rw-r--r--   0 mv         (501) staff       (20)     1059 2024-02-06 22:04:26.000000 decision_utils-0.0.7/src/decision_utils/utils/md.py
+-rw-r--r--   0 mv         (501) staff       (20)     5639 2023-10-24 14:52:02.000000 decision_utils-0.0.7/src/decision_utils/utils/phrase.py
+-rw-r--r--   0 mv         (501) staff       (20)      846 2023-10-14 10:38:30.000000 decision_utils-0.0.7/src/decision_utils/utils/regex.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.320803 decision_utils-0.0.7/src/decision_utils.egg-info/
+-rw-r--r--   0 mv         (501) staff       (20)      832 2024-05-11 11:37:54.000000 decision_utils-0.0.7/src/decision_utils.egg-info/PKG-INFO
+-rw-r--r--   0 mv         (501) staff       (20)     2870 2024-05-11 11:37:54.000000 decision_utils-0.0.7/src/decision_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 mv         (501) staff       (20)        1 2024-05-11 11:37:54.000000 decision_utils-0.0.7/src/decision_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 mv         (501) staff       (20)      128 2024-05-11 11:37:54.000000 decision_utils-0.0.7/src/decision_utils.egg-info/entry_points.txt
+-rw-r--r--   0 mv         (501) staff       (20)      309 2024-05-11 11:37:54.000000 decision_utils-0.0.7/src/decision_utils.egg-info/requires.txt
+-rw-r--r--   0 mv         (501) staff       (20)       90 2024-05-11 11:37:54.000000 decision_utils-0.0.7/src/decision_utils.egg-info/top_level.txt
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-11 11:37:54.320386 decision_utils-0.0.7/src/decision_watcher/
+-rw-r--r--   0 mv         (501) staff       (20)       24 2024-02-08 03:40:51.000000 decision_utils-0.0.7/src/decision_watcher/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     2322 2024-05-04 01:29:37.000000 decision_utils-0.0.7/src/decision_watcher/__main__.py
```

### Comparing `decision_utils-0.0.6/PKG-INFO` & `decision_utils-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: decision-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Preprocess frontmatter-ish markdown with Philippine artifacts, statutes, citations.
 Requires-Python: >=3.11
-Requires-Dist: statute-utils>=0.6.11
-Requires-Dist: citation-utils>=0.4.10
+Requires-Dist: statute-utils>=0.6.12
+Requires-Dist: citation-utils>=0.4.11
 Requires-Dist: citation-title>=0.0.1
 Requires-Dist: corpus-judge>=0.1.4
 Requires-Dist: environs>=10.3
-Requires-Dist: markdownify>=0.11.6
+Requires-Dist: markdownify>=0.12.1
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: html-sanitizer>=2.3.0
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: watchdog>=3.0
 Requires-Dist: python-frontmatter>=1.1.0
 Requires-Dist: rich>=13.7
 Provides-Extra: dev
```

### Comparing `decision_utils-0.0.6/README.md` & `decision_utils-0.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,46 @@
 Despite five packages, only `decision-utils` is usable as a third-party package, being a dependency of [citelaws-builder](https://github.com/justmars/citelaws-builder).
 
 ```sh
 just dumpenv # pypi token
 just publish # uses build / twine
 ```
 
+## Todo
+
+> [!WARNING]
+> Issues detected.
+
+- [ ] Changed title position results in missing title: 69232
+- [ ] No way to detect missing separate opinions yet:
+  - [ ] 69232
+  - [ ] 69257
+  - [ ] 69256
+  - [ ] 69115
+- [ ] Debugging unparseable files
+
+### Unparseable files
+
+Detect errors via running `watcher` and editing a target file.
+
+When trying to load a file with frontmatter, I get `yaml.scanner.ScannerError` indicating bad formatting found in the indicated lines. This usually means that the line is too long, e.g.
+
+```yml
+phrases: # bad since second line in the list can't be parsed
+- Consolidated Building Maintenance, Inc. v. Asprec (Asprec), Philippine Pizza, Inc.
+v. Cayetano (Cayetano)__vs__1
+```
+
+I have to edit manually:
+
+```yml
+phrases: # good
+- Consolidated Building Maintenance, Inc. v. Asprec (Asprec), Philippine Pizza, Inc. v. Cayetano (Cayetano)__vs__1
+```
+
 ## `decision-fetcher` + `decision-fetcher-fields`
 
 `decision-fetcher` requires `decision-fetcher-fields` to extract data from sc e-library URL.
 
 Converting the same to markdown files in a local directory.
 
 First create an interim `decision_files.db`:
```

### Comparing `decision_utils-0.0.6/pyproject.toml` & `decision_utils-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "decision-utils"
 description = "Preprocess frontmatter-ish markdown with Philippine artifacts, statutes, citations."
-version = "0.0.6"
+version = "0.0.7"
 requires-python = ">=3.11"
 dependencies = [
-  "statute-utils >= 0.6.11",
-  "citation-utils >= 0.4.10",
+  "statute-utils >= 0.6.12",
+  "citation-utils >= 0.4.11",
   "citation-title >= 0.0.1",
   "corpus-judge >= 0.1.4",
   "environs >= 10.3",             # config
-  "markdownify >= 0.11.6",        # fetcher
+  "markdownify >= 0.12.1",        # fetcher
   "httpx >= 0.27.0",              # fetcher
   "html-sanitizer >= 2.3.0",      # fetcher
   "beautifulsoup4 >= 4.12.3",     # fetcher-fields
   "watchdog >= 3.0",              # updater
   "python-frontmatter >= 1.1.0",  # updater / fetcher
   "rich >= 13.7",                 # updater / watcher
 ]
```

### Comparing `decision_utils-0.0.6/src/decision_fetcher/__main__.py` & `decision_utils-0.0.7/src/decision_fetcher/__main__.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher/config.py` & `decision_utils-0.0.7/src/decision_fetcher/config.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher/dissect.py` & `decision_utils-0.0.7/src/decision_fetcher/dissect.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher/draft.py` & `decision_utils-0.0.7/src/decision_fetcher/draft.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher/items.py` & `decision_utils-0.0.7/src/decision_fetcher/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,15 @@
                     try:
                         item = Item(
                             url=tag("a")[0]["href"].replace(
                                 "showdocs",
                                 "showdocsfriendly",
                             ),  # get the better formatted url
                             docket=tag("strong")[0].text,
+                            # TODO: may not be able to discover title
                             title=tag("small")[0].text.strip(),
                             date=parse(
                                 tag("a")[0]
                                 .find_all(string=True, recursive=False)[-1]
                                 .strip()
                             ).date(),
                         )
```

### Comparing `decision_utils-0.0.6/src/decision_fetcher/logger.py` & `decision_utils-0.0.7/src/decision_fetcher/logger.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher/sanitize.py` & `decision_utils-0.0.7/src/decision_fetcher/sanitize.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/__init__.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/__init__.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/citation.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/citation.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/cullables.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/cullables.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/phrases.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/dispositive/phrases.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/wherefore.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/dispositive/wherefore.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/footnotes.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/footnotes.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/header.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/header.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/ruling.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/ruling.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_cues.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/ruling_cues.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/court_acts.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/court_acts.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/court_admin.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/court_admin.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/granted_denied.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/granted_denied.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/hence_this.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/hence_this.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/issue_errors.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/issue_errors.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/main_issue.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/ruling_patterns/main_issue.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/tags/base.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/tags/base.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/tags/specific.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/tags/specific.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/tags/utils.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/tags/utils.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/title_tags.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/title_tags.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/voteline.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/voteline.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_fetcher_fields/writer.py` & `decision_utils-0.0.7/src/decision_fetcher_fields/writer.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_updater/__main__.py` & `decision_utils-0.0.7/src/decision_updater/__main__.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_updater/clean.py` & `decision_utils-0.0.7/src/decision_updater/clean.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_updater/logger.py` & `decision_utils-0.0.7/src/decision_updater/logger.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_updater/md.py` & `decision_utils-0.0.7/src/decision_updater/md.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_updater/writer.py` & `decision_utils-0.0.7/src/decision_updater/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     if phrase_list:
         data["phrases"] = phrase_list
 
     # clean content
     post = frontmatter.Post(content, **data)  # type: ignore
 
     # save file with updated statutes and citations
-    frontmatter.dump(post=post, fd=str(file))
+    frontmatter.dump(post=post, fd=str(file), Dumper=SafeDumper)
 
     # frontmatter.dump does not include a trailing new line which is
     # a standard for markdown files, a hack is simply to add a new line manually
     # see https://github.com/eyeseast/python-frontmatter/issues/87
     # file.write_text(data=file.read_text() + "\n")
```

### Comparing `decision_utils-0.0.6/src/decision_utils/author.py` & `decision_utils-0.0.7/src/decision_utils/author.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_utils/block.py` & `decision_utils-0.0.7/src/decision_utils/block.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_utils/decision.py` & `decision_utils-0.0.7/src/decision_utils/decision.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_utils/opinion.py` & `decision_utils-0.0.7/src/decision_utils/opinion.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_utils/utils/annex.py` & `decision_utils-0.0.7/src/decision_utils/utils/annex.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_utils/utils/courts.py` & `decision_utils-0.0.7/src/decision_utils/utils/courts.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_utils/utils/fallo.py` & `decision_utils-0.0.7/src/decision_utils/utils/fallo.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_utils/utils/formatter.py` & `decision_utils-0.0.7/src/decision_utils/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_utils/utils/md.py` & `decision_utils-0.0.7/src/decision_utils/utils/md.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_utils/utils/phrase.py` & `decision_utils-0.0.7/src/decision_utils/utils/phrase.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_utils/utils/regex.py` & `decision_utils-0.0.7/src/decision_utils/utils/regex.py`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_utils.egg-info/PKG-INFO` & `decision_utils-0.0.7/src/decision_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: decision-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Preprocess frontmatter-ish markdown with Philippine artifacts, statutes, citations.
 Requires-Python: >=3.11
-Requires-Dist: statute-utils>=0.6.11
-Requires-Dist: citation-utils>=0.4.10
+Requires-Dist: statute-utils>=0.6.12
+Requires-Dist: citation-utils>=0.4.11
 Requires-Dist: citation-title>=0.0.1
 Requires-Dist: corpus-judge>=0.1.4
 Requires-Dist: environs>=10.3
-Requires-Dist: markdownify>=0.11.6
+Requires-Dist: markdownify>=0.12.1
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: html-sanitizer>=2.3.0
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: watchdog>=3.0
 Requires-Dist: python-frontmatter>=1.1.0
 Requires-Dist: rich>=13.7
 Provides-Extra: dev
```

### Comparing `decision_utils-0.0.6/src/decision_utils.egg-info/SOURCES.txt` & `decision_utils-0.0.7/src/decision_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decision_utils-0.0.6/src/decision_watcher/__main__.py` & `decision_utils-0.0.7/src/decision_watcher/__main__.py`

 * *Files identical despite different names*

