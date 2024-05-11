# Comparing `tmp/folioflex-1.2.0.tar.gz` & `tmp/folioflex-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folioflex-1.2.0.tar", last modified: Tue May  7 20:18:22 2024, max compression
+gzip compressed data, was "folioflex-1.2.1.tar", last modified: Sat May 11 18:19:36 2024, max compression
```

## Comparing `folioflex-1.2.0.tar` & `folioflex-1.2.1.tar`

### file list

```diff
@@ -1,74 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.867471 folioflex-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 20:18:11.000000 folioflex-1.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-07 20:18:11.000000 folioflex-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-05-07 20:18:22.867471 folioflex-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-07 20:18:11.000000 folioflex-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.855471 folioflex-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.855471 folioflex-1.2.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 20:18:11.000000 folioflex-1.2.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.855471 folioflex-1.2.0/folioflex/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.859470 folioflex-1.2.0/folioflex/budget/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/budget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/budget/budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/budget/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.859470 folioflex-1.2.0/folioflex/chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10679 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/chatbot/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/chatbot/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.859470 folioflex-1.2.0/folioflex/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/budget_personal.ini
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/portfolio_dash.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/portfolio_demo.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/portfolio_personal.ini
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/transactions_dash.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/transactions_demo.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.859470 folioflex-1.2.0/folioflex/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/dashboard_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.863471 folioflex-1.2.0/folioflex/dashboard/pages/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/budget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/ideas.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/personal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/sectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/stocks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.863471 folioflex-1.2.0/folioflex/market/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/market/screener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.863471 folioflex-1.2.0/folioflex/portfolio/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33000 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    68299 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    20733 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.863471 folioflex-1.2.0/folioflex/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/cq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/custom_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/mailer.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.867471 folioflex-1.2.0/folioflex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-07 20:18:11.000000 folioflex-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:18:22.867471 folioflex-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 20:18:11.000000 folioflex-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.867471 folioflex-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-07 20:18:11.000000 folioflex-1.2.0/tests/test_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-07 20:18:11.000000 folioflex-1.2.0/tests/test_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-05-07 20:18:11.000000 folioflex-1.2.0/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 20:18:11.000000 folioflex-1.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-07 20:18:11.000000 folioflex-1.2.0/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.393075 folioflex-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-11 18:19:26.000000 folioflex-1.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-11 18:19:26.000000 folioflex-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-11 18:19:36.393075 folioflex-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-05-11 18:19:26.000000 folioflex-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.381075 folioflex-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.381075 folioflex-1.2.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-11 18:19:26.000000 folioflex-1.2.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.381075 folioflex-1.2.1/folioflex/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.385075 folioflex-1.2.1/folioflex/budget/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/budget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/budget/budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/budget/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.385075 folioflex-1.2.1/folioflex/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10679 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/chatbot/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/chatbot/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.385075 folioflex-1.2.1/folioflex/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/configs/budget_personal.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/configs/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/configs/portfolio_dash.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/configs/portfolio_demo.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/configs/portfolio_personal.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/configs/transactions_dash.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/configs/transactions_demo.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.385075 folioflex-1.2.1/folioflex/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.389075 folioflex-1.2.1/folioflex/dashboard/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/assets/folioflex_logo.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   923499 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/assets/folioflex_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/assets/github-mark-white.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.389075 folioflex-1.2.1/folioflex/dashboard/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/components/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/components/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.389075 folioflex-1.2.1/folioflex/dashboard/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/pages/budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/pages/ideas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/pages/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/pages/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/pages/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/pages/personal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/pages/sectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/pages/stocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.389075 folioflex-1.2.1/folioflex/dashboard/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/dashboard/utils/dashboard_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.389075 folioflex-1.2.1/folioflex/market/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/market/screener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.393075 folioflex-1.2.1/folioflex/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33000 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/portfolio/broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/portfolio/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/portfolio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68299 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/portfolio/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20733 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/portfolio/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.393075 folioflex-1.2.1/folioflex/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/utils/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/utils/cq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/utils/custom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/utils/mailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-11 18:19:26.000000 folioflex-1.2.1/folioflex/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.393075 folioflex-1.2.1/folioflex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-11 18:19:36.000000 folioflex-1.2.1/folioflex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-11 18:19:36.000000 folioflex-1.2.1/folioflex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 18:19:36.000000 folioflex-1.2.1/folioflex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-11 18:19:36.000000 folioflex-1.2.1/folioflex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-11 18:19:36.000000 folioflex-1.2.1/folioflex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-11 18:19:36.000000 folioflex-1.2.1/folioflex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-11 18:19:26.000000 folioflex-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 18:19:36.393075 folioflex-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-11 18:19:26.000000 folioflex-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:19:36.393075 folioflex-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-11 18:19:26.000000 folioflex-1.2.1/tests/test_budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-11 18:19:26.000000 folioflex-1.2.1/tests/test_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-05-11 18:19:26.000000 folioflex-1.2.1/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-11 18:19:26.000000 folioflex-1.2.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-11 18:19:26.000000 folioflex-1.2.1/tests/test_wrappers.py
```

### Comparing `folioflex-1.2.0/LICENSE.md` & `folioflex-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/PKG-INFO` & `folioflex-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folioflex
-Version: 1.2.0
+Version: 1.2.1
 Summary: A collection of portfolio tracking capabilities
 Author-email: John Koestner <johnkoestner@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 John Koestner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,48 +29,49 @@
 Project-URL: repository, https://github.com/jkoestner/folioflex
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ipywidgets>=8.1.0
 Requires-Dist: fredapi>=0.4.3
 Requires-Dist: jupyter-dash>=0.4.2
-Requires-Dist: jupyterlab>=4.0.5
-Requires-Dist: jupyterlab-code-formatter>=2.2.1
+Requires-Dist: jupyterlab>=4.0.10
 Requires-Dist: kaleido<0.2.0,>=0.1.0
 Requires-Dist: numpy>=1.22.3
 Requires-Dist: openpyxl>=3.0.7
 Requires-Dist: pandas>=0.25.0
 Requires-Dist: pandas-market-calendars>=4.1.4
 Requires-Dist: pyxirr>=0.7.2
 Requires-Dist: sqlalchemy>=2.0.23
 Requires-Dist: yfinance>=0.2.32
 Requires-Dist: dash>=1.0.2
+Requires-Dist: dash_bootstrap_components>=1.6.0
 Requires-Dist: dash-core-components>=1.0.0
 Requires-Dist: dash-html-components>=1.0.0
 Requires-Dist: dash-renderer>=1.0.0
 Requires-Dist: dash-table>=4.0.2
 Requires-Dist: Flask>=1.1.1
 Requires-Dist: Flask-Compress>=1.4.0
+Requires-Dist: Flask-Login>=0.6.3
 Requires-Dist: gunicorn>=19.9.0
 Requires-Dist: celery>=5.3.1
 Requires-Dist: flower>=2.0.0
 Requires-Dist: redis>=3.3.8
 Requires-Dist: g4f==0.2.4.1
 Requires-Dist: hugchat>=0.3.8
 Requires-Dist: openai>=1.3.7
 Requires-Dist: seleniumbase>=4.22.0
-Provides-Extra: budget
-Requires-Dist: emoji>=2.9.0; extra == "budget"
-Requires-Dist: gensim>=4.3.2; extra == "budget"
-Requires-Dist: scikit-learn>=1.3.2; extra == "budget"
-Requires-Dist: scipy==1.10.1; extra == "budget"
-Requires-Dist: psycopg2-binary; extra == "budget"
+Requires-Dist: emoji>=2.9.0
+Requires-Dist: gensim>=4.3.2
+Requires-Dist: scikit-learn>=1.3.2
+Requires-Dist: scipy==1.10.1
+Requires-Dist: psycopg2-binary
 Provides-Extra: dev
 Requires-Dist: black>=23.7.0; extra == "dev"
 Requires-Dist: isort>=5.13.2; extra == "dev"
+Requires-Dist: jupyterlab-code-formatter>=2.2.1; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: ruff>=0.1.5; extra == "dev"
 Requires-Dist: sphinx<7.2,>=6.0; extra == "dev"
 Requires-Dist: sphinx_rtd_theme>=1.2.2; extra == "dev"
 
 <div align="center">
@@ -84,46 +85,48 @@
 [![license badge](https://img.shields.io/github/license/jkoestner/folioflex)](https://github.com/jkoestner/folioflex/blob/main/LICENSE.md)
 [![codecov](https://codecov.io/gh/jkoestner/folioflex/branch/main/graph/badge.svg?token=K4RS9LX4UG)](https://codecov.io/gh/jkoestner/folioflex)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Static Badge](https://img.shields.io/badge/docs-available-green?labelColor=green&color=gray&link=https%3A%2F%2Fjkoestner.github.io%2Ffolioflex%2F)](https://jkoestner.github.io/folioflex/)
 
 
 ## Table of Contents
-- [Overview](#overview)
-- [Installation](#installation)
-  - [Local Install](#local-install)
-  - [Docker Install](#docker-install)
-- [Usage](#usage)
-  - [CLI](#cli)
-  - [Python](#python)
-  - [Web Dashboard](#web-dashboard---invest)
-  - [Plaid Dashboard](#plaid-dashboard)
-- [Other Tools](#other-tools)
-  - [Jupyter Lab Usage](#jupyter-lab-usage)
-  - [Logging](#logging)
-  - [Coverage](#coverage)
+- [Portfolio](#portfolio)
+  - [Table of Contents](#table-of-contents)
+  - [Overview](#overview)
+  - [Installation](#installation)
+    - [Local Install](#local-install)
+    - [Docker Install](#docker-install)
+  - [Usage](#usage)
+    - [CLI](#cli)
+    - [Python](#python)
+    - [Web Dashboard - Invest](#web-dashboard---invest)
+    - [Plaid Dashboard](#plaid-dashboard)
+  - [Other Tools](#other-tools)
+    - [Jupyter Lab Usage](#jupyter-lab-usage)
+    - [Logging](#logging)
+    - [Coverage](#coverage)
 
 ## Overview
 
 **🚀 Welcome to FolioFlex! 🚀**
 
 **📖 Description:**
 
 - FolioFlex is your go-to toolkit for portfolio management and market analysis! Dive into the world of stocks, bonds, and more with our user-friendly tools. 📈📊
 
 **🔧 Features:**
 
 - **Market Screener**: Filter and find trending stocks. 🔍
-![screener](assets/screenshots/screener.png)
-![heatmap](assets/screenshots/heatmap.png)
+![screener](docs/screenshots/screener.png)
+![heatmap](docs/screenshots/heatmap.png)
 - **Portfolio Management**: Organize and track, your investments. 💼
-![portfolio](assets/screenshots/portfolio.png)
+![portfolio](docs/screenshots/portfolio.png)
 - **Budget Tool**: Create and monitor a budget. 💰
-![budget](assets/screenshots/budget.png)
-![budget_compare](assets/screenshots/budget_compare.png)
+![budget](docs/screenshots/budget.png)
+![budget_compare](docs/screenshots/budget_compare.png)
 
 **📚 Documentation:**
 
 - [Installation Guide](https://jkoestner.github.io/folioflex/installation.html): Get started with FolioFlex in no time! 🛠️
 
 **🎥 See It In Action:**
 
@@ -153,19 +156,16 @@
 ```
 pip install folioflex
 ```
 
 Other options can be installed if using more functionality
 
 ```
-pip install folioflex[budget] # if using the budget modules
+pip install folioflex
 pip install folioflex[dev]    # if needing to develop or lint
-pip install folioflex[gpt]    # if using the mailer or gpt code
-pip install folioflex[web]    # if using the web dashboard
-pip install folioflex[worker] # if using the web dashboard
 ``````
 
 Or could be done using GitHub.
 
 ```
 pip install git+https://github.com/jkoestner/folioflex.git
 ```
```

### Comparing `folioflex-1.2.0/README.md` & `folioflex-1.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,46 +9,48 @@
 [![license badge](https://img.shields.io/github/license/jkoestner/folioflex)](https://github.com/jkoestner/folioflex/blob/main/LICENSE.md)
 [![codecov](https://codecov.io/gh/jkoestner/folioflex/branch/main/graph/badge.svg?token=K4RS9LX4UG)](https://codecov.io/gh/jkoestner/folioflex)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Static Badge](https://img.shields.io/badge/docs-available-green?labelColor=green&color=gray&link=https%3A%2F%2Fjkoestner.github.io%2Ffolioflex%2F)](https://jkoestner.github.io/folioflex/)
 
 
 ## Table of Contents
-- [Overview](#overview)
-- [Installation](#installation)
-  - [Local Install](#local-install)
-  - [Docker Install](#docker-install)
-- [Usage](#usage)
-  - [CLI](#cli)
-  - [Python](#python)
-  - [Web Dashboard](#web-dashboard---invest)
-  - [Plaid Dashboard](#plaid-dashboard)
-- [Other Tools](#other-tools)
-  - [Jupyter Lab Usage](#jupyter-lab-usage)
-  - [Logging](#logging)
-  - [Coverage](#coverage)
+- [Portfolio](#portfolio)
+  - [Table of Contents](#table-of-contents)
+  - [Overview](#overview)
+  - [Installation](#installation)
+    - [Local Install](#local-install)
+    - [Docker Install](#docker-install)
+  - [Usage](#usage)
+    - [CLI](#cli)
+    - [Python](#python)
+    - [Web Dashboard - Invest](#web-dashboard---invest)
+    - [Plaid Dashboard](#plaid-dashboard)
+  - [Other Tools](#other-tools)
+    - [Jupyter Lab Usage](#jupyter-lab-usage)
+    - [Logging](#logging)
+    - [Coverage](#coverage)
 
 ## Overview
 
 **🚀 Welcome to FolioFlex! 🚀**
 
 **📖 Description:**
 
 - FolioFlex is your go-to toolkit for portfolio management and market analysis! Dive into the world of stocks, bonds, and more with our user-friendly tools. 📈📊
 
 **🔧 Features:**
 
 - **Market Screener**: Filter and find trending stocks. 🔍
-![screener](assets/screenshots/screener.png)
-![heatmap](assets/screenshots/heatmap.png)
+![screener](docs/screenshots/screener.png)
+![heatmap](docs/screenshots/heatmap.png)
 - **Portfolio Management**: Organize and track, your investments. 💼
-![portfolio](assets/screenshots/portfolio.png)
+![portfolio](docs/screenshots/portfolio.png)
 - **Budget Tool**: Create and monitor a budget. 💰
-![budget](assets/screenshots/budget.png)
-![budget_compare](assets/screenshots/budget_compare.png)
+![budget](docs/screenshots/budget.png)
+![budget_compare](docs/screenshots/budget_compare.png)
 
 **📚 Documentation:**
 
 - [Installation Guide](https://jkoestner.github.io/folioflex/installation.html): Get started with FolioFlex in no time! 🛠️
 
 **🎥 See It In Action:**
 
@@ -78,19 +80,16 @@
 ```
 pip install folioflex
 ```
 
 Other options can be installed if using more functionality
 
 ```
-pip install folioflex[budget] # if using the budget modules
+pip install folioflex
 pip install folioflex[dev]    # if needing to develop or lint
-pip install folioflex[gpt]    # if using the mailer or gpt code
-pip install folioflex[web]    # if using the web dashboard
-pip install folioflex[worker] # if using the web dashboard
 ``````
 
 Or could be done using GitHub.
 
 ```
 pip install git+https://github.com/jkoestner/folioflex.git
 ```
```

### Comparing `folioflex-1.2.0/docs/source/conf.py` & `folioflex-1.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/budget/budget.py` & `folioflex-1.2.1/folioflex/budget/budget.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/budget/models.py` & `folioflex-1.2.1/folioflex/budget/models.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/chatbot/providers.py` & `folioflex-1.2.1/folioflex/chatbot/providers.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/chatbot/scraper.py` & `folioflex-1.2.1/folioflex/chatbot/scraper.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/configs/budget_personal.ini` & `folioflex-1.2.1/folioflex/configs/budget_personal.ini`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/configs/config.ini` & `folioflex-1.2.1/folioflex/configs/config.ini`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/configs/portfolio_dash.ini` & `folioflex-1.2.1/folioflex/configs/portfolio_dash.ini`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/configs/portfolio_demo.ini` & `folioflex-1.2.1/folioflex/configs/portfolio_demo.ini`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/configs/portfolio_personal.ini` & `folioflex-1.2.1/folioflex/configs/portfolio_personal.ini`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/configs/transactions_dash.csv` & `folioflex-1.2.1/folioflex/configs/transactions_dash.csv`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/configs/transactions_demo.csv` & `folioflex-1.2.1/folioflex/configs/transactions_demo.csv`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/dashboard/dashboard_helper.py` & `folioflex-1.2.1/folioflex/dashboard/utils/dashboard_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,52 +8,14 @@
 
 import pandas as pd
 import plotly.graph_objs as go
 from dash import dcc, html
 from dateutil.relativedelta import relativedelta
 
 
-def get_menu():
-    """Provide menu for pages."""
-    menu = html.Div(
-        [
-            dcc.Link(
-                "Stocks   ",
-                href="/stocks",
-            ),
-            dcc.Link(
-                "Sectors   ",
-                href="/sectors",
-                style={"padding": 10},
-            ),
-            dcc.Link(
-                "Ideas   ",
-                href="/ideas",
-                style={"padding": 10},
-            ),
-            dcc.Link(
-                "Macro   ",
-                href="/macro",
-                style={"padding": 10},
-            ),
-            dcc.Link(
-                "Personal   ",
-                href="/personal",
-                style={"padding": 10},
-            ),
-            dcc.Link(
-                "Budget   ",
-                href="/budget",
-                style={"padding": 10},
-            ),
-        ]
-    )
-    return menu
-
-
 def get_defaults():
     """Provide default initializations for pages."""
     # TODO
     # These are needed so that the variable can be none. With some work
     # this could probably be removed and put in individual pages.
     defaults = (
         html.Div(id="task-status", children="none", style={"display": "none"}),
```

### Comparing `folioflex-1.2.0/folioflex/dashboard/layouts.py` & `folioflex-1.2.1/folioflex/dashboard/components/layouts.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/dashboard/pages/macro.py` & `folioflex-1.2.1/folioflex/dashboard/pages/macro.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 """Macro dashboard."""
 
+import dash
 from dash import dash_table, dcc, html
 
-from folioflex.dashboard import dashboard_helper
+from folioflex.dashboard.utils import dashboard_helper
 from folioflex.portfolio.wrappers import BLS, Fred, TradingView
+from folioflex.utils import custom_logger
 
-# Creating the dash app
+logger = custom_logger.setup_logging(__name__)
 
+dash.register_page(__name__, path="/macro", title="folioflex - Macro", order=2)
 
-def layout(login_status, login_alert):
+#   _                            _
+#  | |    __ _ _   _  ___  _   _| |_
+#  | |   / _` | | | |/ _ \| | | | __|
+#  | |__| (_| | |_| | (_) | |_| | |_
+#  |_____\__,_|\__, |\___/ \__,_|\__|
+#              |___/
+
+
+def layout():
     """Macro layout."""
     # getting data from wrappers
     fred_summary = Fred().get_summary()
     bls_cpi = BLS().get_cpi()
     economic_calendar = TradingView().get_economic_calendar()
 
     # creating html table for items
@@ -71,89 +82,69 @@
         markdown_options={"link_target": "_blank"},
     )
 
     return html.Div(
         [
             # adding variables needed that are used in callbacks.
             *dashboard_helper.get_defaults(),
-            dcc.Store(id="login-status", data=login_status),
-            html.Div(id="login-alert", children=login_alert, style={"display": "none"}),
             # ---------------------------------------------------------------
-            # menu section
-            html.Div(
-                [
-                    dashboard_helper.get_menu(),
-                    dcc.Markdown(
-                        """
+            dcc.Markdown(
+                """
                         Macro indicators
                         """
-                    ),
-                    html.P(),
-                ],
-                className="row",
             ),
+            html.P(),
             # key indicators section
             html.Div(
-                [
-                    html.Div(
-                        indicators_table,
-                        className="four columns",
-                    ),
-                ],
-                className="row",
+                indicators_table,
+                className="four columns",
             ),
             # economic calendar section
             html.Div(
                 [
-                    html.Div(
-                        [
-                            # creating economic calendar
-                            html.A(
-                                "Economic Calendar",
-                                href="https://www.tradingview.com/economic-calendar/",
-                                target="_blank",
-                            ),
-                            dash_table.DataTable(
-                                id="economic-calendar",
-                                columns=[
-                                    {"name": i, "id": i}
-                                    for i in economic_calendar.columns
-                                ],
-                                data=economic_calendar.to_dict("records"),
-                                style_cell={
-                                    "whiteSpace": "normal",
-                                    "height": "auto",
-                                    "textAlign": "left",
-                                },
-                                style_cell_conditional=[
-                                    # Apply a default width to all columns
-                                    {
-                                        "if": {"column_id": c},
-                                        "minWidth": "50px",
-                                        "width": "150px",
-                                        "maxWidth": "180px",
-                                    }
-                                    for c in economic_calendar.columns
-                                    if c != "comment"
-                                ]
-                                + [
-                                    # Specifically targeting the 'comment'
-                                    # column to have a larger width
-                                    {
-                                        "if": {"column_id": "comment"},
-                                        "minWidth": "150px",
-                                        "width": "2400px",
-                                        "maxWidth": "2450px",
-                                    },
-                                ],
-                                style_table={"overflowX": "auto"},
-                                page_action="none",
-                                style_data={"overflow": "hidden"},
-                            ),
+                    # creating economic calendar
+                    html.A(
+                        "Economic Calendar",
+                        href="https://www.tradingview.com/economic-calendar/",
+                        target="_blank",
+                    ),
+                    dash_table.DataTable(
+                        id="economic-calendar",
+                        columns=[
+                            {"name": i, "id": i} for i in economic_calendar.columns
+                        ],
+                        data=economic_calendar.to_dict("records"),
+                        style_cell={
+                            "whiteSpace": "normal",
+                            "height": "auto",
+                            "textAlign": "left",
+                        },
+                        style_cell_conditional=[
+                            # Apply a default width to all columns
+                            {
+                                "if": {"column_id": c},
+                                "minWidth": "50px",
+                                "width": "150px",
+                                "maxWidth": "180px",
+                            }
+                            for c in economic_calendar.columns
+                            if c != "comment"
+                        ]
+                        + [
+                            # Specifically targeting the 'comment'
+                            # column to have a larger width
+                            {
+                                "if": {"column_id": "comment"},
+                                "minWidth": "150px",
+                                "width": "2400px",
+                                "maxWidth": "2450px",
+                            },
                         ],
-                        className="ten columns",
+                        style_table={"overflowX": "auto"},
+                        page_action="none",
+                        style_data={"overflow": "hidden"},
                     ),
                 ],
-                className="row",
+                className="ten columns",
             ),
         ]
     )
```

### Comparing `folioflex-1.2.0/folioflex/portfolio/broker.py` & `folioflex-1.2.1/folioflex/portfolio/broker.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/portfolio/heatmap.py` & `folioflex-1.2.1/folioflex/portfolio/heatmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     lookback : int (optional)
         number of days to lookback
 
     Returns
     -------
     fig : Figure
        heatmap figure
+
     """
     if portfolio is None:
         returns = Finviz().get_heatmap_data()
         color = "return_pct"
     else:
         if config_path is None:
             raise ValueError(
```

### Comparing `folioflex-1.2.0/folioflex/portfolio/helper.py` & `folioflex-1.2.1/folioflex/portfolio/helper.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/portfolio/portfolio.py` & `folioflex-1.2.1/folioflex/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/portfolio/wrappers.py` & `folioflex-1.2.1/folioflex/portfolio/wrappers.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/utils/cli.py` & `folioflex-1.2.1/folioflex/utils/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Provide cli for folioflex."""
 
 import argparse
 import ast
 from argparse import ArgumentDefaultsHelpFormatter
 
+from folioflex.dashboard import app
 from folioflex.portfolio.portfolio import Manager, Portfolio
 from folioflex.utils import mailer
 
 
 def _parse_input_to_list(input_str):
     """
     Parse the input string.
@@ -208,14 +209,17 @@
         "-p",
         "--proxy",
         type=str,
         default=None,
         help=("The proxy to use for the chatbot - user:password@ip:port"),
     )
 
+    # subparser: dashboard
+    _dash_parser = _subparsers.add_parser("dash", help="dashboard command")
+
     return _parser
 
 
 parser = _create_argparser()
 
 
 def cli():
@@ -244,10 +248,13 @@
             heatmap_portfolio=args.heatmap_portfolio,
             manager_performance=args.manager_performance,
             portfolio_performance=args.portfolio_performance,
             chatbot=args.chatbot,
         )
         print(f"status sent: {email_status}")
 
+    elif args.command == "dash":
+        app.app.run_server(debug=True)
+
 
 if __name__ == "__main__":
     cli()
```

### Comparing `folioflex-1.2.0/folioflex/utils/config_helper.py` & `folioflex-1.2.1/folioflex/utils/config_helper.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex/utils/cq.py` & `folioflex-1.2.1/folioflex/utils/cq.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 """
 
 from datetime import datetime
 
 import yfinance as yf
 from celery import Celery
 
-from folioflex.dashboard import layouts
+from folioflex.dashboard.components import layouts
 from folioflex.portfolio import portfolio
 from folioflex.utils import config_helper
 
 celery_app = Celery(
     "tasks",
     broker=config_helper.REDIS_URL,
     backend=config_helper.REDIS_URL,
```

### Comparing `folioflex-1.2.0/folioflex/utils/custom_logger.py` & `folioflex-1.2.1/folioflex/utils/custom_logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """
 Custom logger with color formatter.
 
 inspired by:
 https://gist.github.com/joshbode/58fac7ababc700f51e2a9ecdebe563ad
+
+The Jupyter formatter exists due to issues with getting a colored output.
+The following issue describes why the formatter doesn't work.
+https://github.com/seleniumbase/SeleniumBase/issues/2592
 """
 
 import logging
 import sys
 
 from colorama import Back, Fore, Style
 from IPython.display import HTML, display
@@ -135,35 +139,62 @@
     # folioflex logger
     folioflex_logger = logging.getLogger(name)
     folioflex_logger.setLevel(logging.INFO)
 
     return folioflex_logger
 
 
-def set_log_level(new_level):
+def set_log_level(new_level, module_prefix="folioflex"):
     """
     Set the log level.
 
     Parameters
     ----------
     new_level : int
         the new log level
+    module_prefix : str
+        the module logger prefix to set the log level for
 
     """
     options = ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
     if new_level not in options:
         raise ValueError(f"Log level must be one of {options}")
     # update the log level for all project loggers
     for logger_name, logger in logging.Logger.manager.loggerDict.items():
         # Check if the logger's name starts with the specified prefix
-        if logger_name.startswith("folioflex"):
+        if logger_name.startswith(module_prefix):
             if isinstance(logger, logging.Logger):
                 logger.setLevel(new_level)
 
 
+def get_log_level(module_prefix="folioflex"):
+    """
+    Get the log level.
+
+    Parameters
+    ----------
+    module_prefix : str
+        the module logger prefix to get the log level for
+
+    Returns
+    -------
+    str
+        the log level
+
+    """
+    log_level = None
+    for logger_name, logger in logging.Logger.manager.loggerDict.items():
+        # Check if the logger's name starts with the specified prefix
+        if logger_name.startswith(module_prefix):
+            if isinstance(logger, logging.Logger):
+                log_level = logging.getLevelName(logger.getEffectiveLevel())
+                break
+    return log_level
+
+
 def test_logger(level="DEBUG"):
     """Test the logger."""
     logger = setup_logging(__name__)
     set_log_level(level)
     logger.debug("debug message")
     logger.info("info message")
     logger.warning("warning message")
```

### Comparing `folioflex-1.2.0/folioflex/utils/mailer.py` & `folioflex-1.2.1/folioflex/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/folioflex.egg-info/PKG-INFO` & `folioflex-1.2.1/folioflex.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folioflex
-Version: 1.2.0
+Version: 1.2.1
 Summary: A collection of portfolio tracking capabilities
 Author-email: John Koestner <johnkoestner@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 John Koestner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,48 +29,49 @@
 Project-URL: repository, https://github.com/jkoestner/folioflex
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ipywidgets>=8.1.0
 Requires-Dist: fredapi>=0.4.3
 Requires-Dist: jupyter-dash>=0.4.2
-Requires-Dist: jupyterlab>=4.0.5
-Requires-Dist: jupyterlab-code-formatter>=2.2.1
+Requires-Dist: jupyterlab>=4.0.10
 Requires-Dist: kaleido<0.2.0,>=0.1.0
 Requires-Dist: numpy>=1.22.3
 Requires-Dist: openpyxl>=3.0.7
 Requires-Dist: pandas>=0.25.0
 Requires-Dist: pandas-market-calendars>=4.1.4
 Requires-Dist: pyxirr>=0.7.2
 Requires-Dist: sqlalchemy>=2.0.23
 Requires-Dist: yfinance>=0.2.32
 Requires-Dist: dash>=1.0.2
+Requires-Dist: dash_bootstrap_components>=1.6.0
 Requires-Dist: dash-core-components>=1.0.0
 Requires-Dist: dash-html-components>=1.0.0
 Requires-Dist: dash-renderer>=1.0.0
 Requires-Dist: dash-table>=4.0.2
 Requires-Dist: Flask>=1.1.1
 Requires-Dist: Flask-Compress>=1.4.0
+Requires-Dist: Flask-Login>=0.6.3
 Requires-Dist: gunicorn>=19.9.0
 Requires-Dist: celery>=5.3.1
 Requires-Dist: flower>=2.0.0
 Requires-Dist: redis>=3.3.8
 Requires-Dist: g4f==0.2.4.1
 Requires-Dist: hugchat>=0.3.8
 Requires-Dist: openai>=1.3.7
 Requires-Dist: seleniumbase>=4.22.0
-Provides-Extra: budget
-Requires-Dist: emoji>=2.9.0; extra == "budget"
-Requires-Dist: gensim>=4.3.2; extra == "budget"
-Requires-Dist: scikit-learn>=1.3.2; extra == "budget"
-Requires-Dist: scipy==1.10.1; extra == "budget"
-Requires-Dist: psycopg2-binary; extra == "budget"
+Requires-Dist: emoji>=2.9.0
+Requires-Dist: gensim>=4.3.2
+Requires-Dist: scikit-learn>=1.3.2
+Requires-Dist: scipy==1.10.1
+Requires-Dist: psycopg2-binary
 Provides-Extra: dev
 Requires-Dist: black>=23.7.0; extra == "dev"
 Requires-Dist: isort>=5.13.2; extra == "dev"
+Requires-Dist: jupyterlab-code-formatter>=2.2.1; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: ruff>=0.1.5; extra == "dev"
 Requires-Dist: sphinx<7.2,>=6.0; extra == "dev"
 Requires-Dist: sphinx_rtd_theme>=1.2.2; extra == "dev"
 
 <div align="center">
@@ -84,46 +85,48 @@
 [![license badge](https://img.shields.io/github/license/jkoestner/folioflex)](https://github.com/jkoestner/folioflex/blob/main/LICENSE.md)
 [![codecov](https://codecov.io/gh/jkoestner/folioflex/branch/main/graph/badge.svg?token=K4RS9LX4UG)](https://codecov.io/gh/jkoestner/folioflex)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Static Badge](https://img.shields.io/badge/docs-available-green?labelColor=green&color=gray&link=https%3A%2F%2Fjkoestner.github.io%2Ffolioflex%2F)](https://jkoestner.github.io/folioflex/)
 
 
 ## Table of Contents
-- [Overview](#overview)
-- [Installation](#installation)
-  - [Local Install](#local-install)
-  - [Docker Install](#docker-install)
-- [Usage](#usage)
-  - [CLI](#cli)
-  - [Python](#python)
-  - [Web Dashboard](#web-dashboard---invest)
-  - [Plaid Dashboard](#plaid-dashboard)
-- [Other Tools](#other-tools)
-  - [Jupyter Lab Usage](#jupyter-lab-usage)
-  - [Logging](#logging)
-  - [Coverage](#coverage)
+- [Portfolio](#portfolio)
+  - [Table of Contents](#table-of-contents)
+  - [Overview](#overview)
+  - [Installation](#installation)
+    - [Local Install](#local-install)
+    - [Docker Install](#docker-install)
+  - [Usage](#usage)
+    - [CLI](#cli)
+    - [Python](#python)
+    - [Web Dashboard - Invest](#web-dashboard---invest)
+    - [Plaid Dashboard](#plaid-dashboard)
+  - [Other Tools](#other-tools)
+    - [Jupyter Lab Usage](#jupyter-lab-usage)
+    - [Logging](#logging)
+    - [Coverage](#coverage)
 
 ## Overview
 
 **🚀 Welcome to FolioFlex! 🚀**
 
 **📖 Description:**
 
 - FolioFlex is your go-to toolkit for portfolio management and market analysis! Dive into the world of stocks, bonds, and more with our user-friendly tools. 📈📊
 
 **🔧 Features:**
 
 - **Market Screener**: Filter and find trending stocks. 🔍
-![screener](assets/screenshots/screener.png)
-![heatmap](assets/screenshots/heatmap.png)
+![screener](docs/screenshots/screener.png)
+![heatmap](docs/screenshots/heatmap.png)
 - **Portfolio Management**: Organize and track, your investments. 💼
-![portfolio](assets/screenshots/portfolio.png)
+![portfolio](docs/screenshots/portfolio.png)
 - **Budget Tool**: Create and monitor a budget. 💰
-![budget](assets/screenshots/budget.png)
-![budget_compare](assets/screenshots/budget_compare.png)
+![budget](docs/screenshots/budget.png)
+![budget_compare](docs/screenshots/budget_compare.png)
 
 **📚 Documentation:**
 
 - [Installation Guide](https://jkoestner.github.io/folioflex/installation.html): Get started with FolioFlex in no time! 🛠️
 
 **🎥 See It In Action:**
 
@@ -153,19 +156,16 @@
 ```
 pip install folioflex
 ```
 
 Other options can be installed if using more functionality
 
 ```
-pip install folioflex[budget] # if using the budget modules
+pip install folioflex
 pip install folioflex[dev]    # if needing to develop or lint
-pip install folioflex[gpt]    # if using the mailer or gpt code
-pip install folioflex[web]    # if using the web dashboard
-pip install folioflex[worker] # if using the web dashboard
 ``````
 
 Or could be done using GitHub.
 
 ```
 pip install git+https://github.com/jkoestner/folioflex.git
 ```
```

### Comparing `folioflex-1.2.0/folioflex.egg-info/SOURCES.txt` & `folioflex-1.2.1/folioflex.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,24 +23,32 @@
 folioflex/configs/config.ini
 folioflex/configs/portfolio_dash.ini
 folioflex/configs/portfolio_demo.ini
 folioflex/configs/portfolio_personal.ini
 folioflex/configs/transactions_dash.csv
 folioflex/configs/transactions_demo.csv
 folioflex/dashboard/__init__.py
-folioflex/dashboard/dashboard_helper.py
-folioflex/dashboard/layouts.py
+folioflex/dashboard/app.py
+folioflex/dashboard/assets/folioflex_logo.ico
+folioflex/dashboard/assets/folioflex_logo.png
+folioflex/dashboard/assets/github-mark-white.png
+folioflex/dashboard/components/__init__.py
+folioflex/dashboard/components/auth.py
+folioflex/dashboard/components/layouts.py
 folioflex/dashboard/pages/__init__.py
 folioflex/dashboard/pages/budget.py
 folioflex/dashboard/pages/ideas.py
 folioflex/dashboard/pages/login.py
+folioflex/dashboard/pages/logout.py
 folioflex/dashboard/pages/macro.py
 folioflex/dashboard/pages/personal.py
 folioflex/dashboard/pages/sectors.py
 folioflex/dashboard/pages/stocks.py
+folioflex/dashboard/utils/__init__.py
+folioflex/dashboard/utils/dashboard_helper.py
 folioflex/market/__init__.py
 folioflex/market/screener.py
 folioflex/portfolio/__init__.py
 folioflex/portfolio/broker.py
 folioflex/portfolio/heatmap.py
 folioflex/portfolio/helper.py
 folioflex/portfolio/portfolio.py
```

### Comparing `folioflex-1.2.0/folioflex.egg-info/requires.txt` & `folioflex-1.2.1/folioflex.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 ipywidgets>=8.1.0
 fredapi>=0.4.3
 jupyter-dash>=0.4.2
-jupyterlab>=4.0.5
-jupyterlab-code-formatter>=2.2.1
+jupyterlab>=4.0.10
 kaleido<0.2.0,>=0.1.0
 numpy>=1.22.3
 openpyxl>=3.0.7
 pandas>=0.25.0
 pandas-market-calendars>=4.1.4
 pyxirr>=0.7.2
 sqlalchemy>=2.0.23
 yfinance>=0.2.32
 dash>=1.0.2
+dash_bootstrap_components>=1.6.0
 dash-core-components>=1.0.0
 dash-html-components>=1.0.0
 dash-renderer>=1.0.0
 dash-table>=4.0.2
 Flask>=1.1.1
 Flask-Compress>=1.4.0
+Flask-Login>=0.6.3
 gunicorn>=19.9.0
 celery>=5.3.1
 flower>=2.0.0
 redis>=3.3.8
 g4f==0.2.4.1
 hugchat>=0.3.8
 openai>=1.3.7
 seleniumbase>=4.22.0
-
-[budget]
 emoji>=2.9.0
 gensim>=4.3.2
 scikit-learn>=1.3.2
 scipy==1.10.1
 psycopg2-binary
 
 [dev]
 black>=23.7.0
 isort>=5.13.2
+jupyterlab-code-formatter>=2.2.1
 pytest>=7.4.0
 pytest-cov>=4.1.0
 ruff>=0.1.5
 sphinx<7.2,>=6.0
 sphinx_rtd_theme>=1.2.2
```

### Comparing `folioflex-1.2.0/pyproject.toml` & `folioflex-1.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,63 +11,64 @@
 license = { file = 'LICENSE.md' }
 requires-python = '>=3.8'
 
 dependencies = [
     "ipywidgets>=8.1.0",
     "fredapi>=0.4.3",
     "jupyter-dash>=0.4.2",
-    "jupyterlab>=4.0.5",
-    "jupyterlab-code-formatter>=2.2.1",
-    "kaleido>=0.1.0,<0.2.0",            # as of Kaleido 0.2.1, the image processig is too slow.
+    "jupyterlab>=4.0.10",
+    "kaleido>=0.1.0,<0.2.0",          # as of Kaleido 0.2.1, the image processig is too slow.
     "numpy>=1.22.3",
     "openpyxl>=3.0.7",
     "pandas>=0.25.0",
     "pandas-market-calendars>=4.1.4",
     "pyxirr>=0.7.2",
     "sqlalchemy>=2.0.23",
     "yfinance>=0.2.32",
 
     # web
     "dash>=1.0.2",
+    "dash_bootstrap_components>=1.6.0",
     "dash-core-components>=1.0.0",
     "dash-html-components>=1.0.0",
     "dash-renderer>=1.0.0",
     "dash-table>=4.0.2",
     "Flask>=1.1.1",
     "Flask-Compress>=1.4.0",
+    "Flask-Login>=0.6.3",
     "gunicorn>=19.9.0",
 
     # worker
     "celery>=5.3.1",
     "flower>=2.0.0",
     "redis>=3.3.8",
 
     # gpt
     "g4f==0.2.4.1",         # this package has loose testing support
     "hugchat>=0.3.8",
     "openai>=1.3.7",
     "seleniumbase>=4.22.0",
-]
 
-[project.optional-dependencies]
-budget = [
+    # budget
     "emoji>=2.9.0",
     "gensim>=4.3.2",
     "scikit-learn>=1.3.2",
     "scipy==1.10.1",       # gensim needs to update to newest scipy 
     "psycopg2-binary",
 ]
 
+[project.optional-dependencies]
 dev = [
     "black>=23.7.0",
     "isort>=5.13.2",
+    "jupyterlab-code-formatter>=2.2.1",
     "pytest>=7.4.0",
     "pytest-cov>=4.1.0",
     "ruff>=0.1.5",
-    "sphinx>=6.0, <7.2",       # 7.2 breaks the docs build
+    "sphinx>=6.0, <7.2",                # 7.2 breaks the docs build
     "sphinx_rtd_theme>=1.2.2",
 ]
 
 [project.scripts]
 ffx = "folioflex.utils.cli:cli" # the entry points provide console scripts at command line
 
 [project.urls]
```

### Comparing `folioflex-1.2.0/tests/test_budget.py` & `folioflex-1.2.1/tests/test_budget.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/tests/test_chatbot.py` & `folioflex-1.2.1/tests/test_chatbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tests the chatbot."""
 
 import os
 
 import g4f
 import openai
+import pytest
 from hugchat import hugchat
 
 from folioflex.chatbot import providers
 
 
 def test_g4f():
     """Checks g4f initialize."""
@@ -16,29 +17,30 @@
         chatbot.provider, providers.G4FProvider
     ), "Default provider - G4F - not initialized correctly."
     assert chatbot.chatbot["model"] == g4f.models.default, "Default model not set."
     assert chatbot.chatbot["provider"] == g4f.Provider.Bing, "Default provider not set."
     assert chatbot.chatbot["auth"] == False, "Default auth not set."
     assert chatbot.chatbot["access_token"] is None, "Default access token not set."
     response = chatbot.chat("return back 'test' for test purpose")
-    assert response == "test", "Response not as expected."
+    assert isinstance(response, str), "Response not a string."
 
 
 # openai has billing so not testing unless needed
 # def test_openai():
 #     """Checks openai initialize."""
 #     chatbot = providers.GPTchat(provider="openai")
 #     assert isinstance(
 #         chatbot.provider, providers.OpenaiProvider
 #     ), "Default provider - OpenAI - not initialized correctly."
 #     assert isinstance(chatbot.chatbot, openai.OpenAI), "Default model not set."
 #     response = chatbot.chat("return back 'test' for test purpose")
 #     assert response == "test", "Response not as expected."
 
 
+@pytest.mark.xfail
 # hugchat needs api key to be set in environment variable to login
 def test_hugchat():
     """Checks hugchat initialize."""
     # Access credentials from environment variables
     hugchat_login = os.environ.get("HUGCHAT_LOGIN")
     hugchat_password = os.environ.get("HUGCHAT_PASSWORD")
```

### Comparing `folioflex-1.2.0/tests/test_portfolio.py` & `folioflex-1.2.1/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.2.0/tests/test_utils.py` & `folioflex-1.2.1/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Tests the utilities."""
 
 from datetime import datetime
 
-from folioflex.dashboard import dashboard_helper
+from folioflex.dashboard.utils import dashboard_helper
 from folioflex.utils import config_helper
 
 config_path = config_helper.ROOT_PATH / "tests" / "files" / "test_portfolio.ini"
 config_dict = config_helper.get_config_options(config_path, "test")
 
 
 def test_config_load():
```

### Comparing `folioflex-1.2.0/tests/test_wrappers.py` & `folioflex-1.2.1/tests/test_wrappers.py`

 * *Files identical despite different names*

