# Comparing `tmp/starrailcard-2.1.7.tar.gz` & `tmp/starrailcard-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-2.1.7.tar", last modified: Fri May  3 21:39:14 2024, max compression
+gzip compressed data, was "starrailcard-2.1.8.tar", last modified: Sat May 11 17:12:06 2024, max compression
```

## Comparing `starrailcard-2.1.7.tar` & `starrailcard-2.1.8.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.979988 starrailcard-2.1.7/
--rw-rw-rw-   0        0        0     1721 2024-03-20 15:38:40.000000 starrailcard-2.1.7/LICENSE
--rw-rw-rw-   0        0        0       38 2024-04-29 22:20:14.000000 starrailcard-2.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4744 2024-05-03 21:39:14.978983 starrailcard-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3642 2024-03-18 20:36:48.000000 starrailcard-2.1.7/README.md
--rw-rw-rw-   0        0        0     1106 2024-04-18 21:49:53.000000 starrailcard-2.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 21:39:14.979988 starrailcard-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1544 2024-04-29 22:37:14.000000 starrailcard-2.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.728308 starrailcard-2.1.7/starrailcard/
--rw-rw-rw-   0        0        0     1967 2024-05-03 21:36:05.000000 starrailcard-2.1.7/starrailcard/__init__.py
--rw-rw-rw-   0        0        0    12335 2024-04-29 22:25:47.000000 starrailcard-2.1.7/starrailcard/client.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.701592 starrailcard-2.1.7/starrailcard/src/
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.771493 starrailcard-2.1.7/starrailcard/src/api/
--rw-rw-rw-   0        0        0     2761 2024-04-29 21:42:26.000000 starrailcard-2.1.7/starrailcard/src/api/api.py
--rw-rw-rw-   0        0        0     3487 2024-04-14 22:43:00.000000 starrailcard-2.1.7/starrailcard/src/api/enka.py
--rw-rw-rw-   0        0        0    25187 2024-04-14 22:52:21.000000 starrailcard-2.1.7/starrailcard/src/api/enka_parsed.py
--rw-rw-rw-   0        0        0      487 2024-04-09 16:19:13.000000 starrailcard-2.1.7/starrailcard/src/api/error.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.700592 starrailcard-2.1.7/starrailcard/src/assets/
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.776744 starrailcard-2.1.7/starrailcard/src/assets/font/
--rw-rw-rw-   0        0        0   201292 2023-10-12 08:13:59.000000 starrailcard-2.1.7/starrailcard/src/assets/font/font_hsr.ttf
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.807021 starrailcard-2.1.7/starrailcard/src/data/
--rw-rw-rw-   0        0        0     1751 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/avatar.json
--rw-rw-rw-   0        0        0      252 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/element.json
--rw-rw-rw-   0        0        0       70 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/keys.json
--rw-rw-rw-   0        0        0      293 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/paths.json
--rw-rw-rw-   0        0        0     1915 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/relict_sets.json
--rw-rw-rw-   0        0        0     4947 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/stats.json
--rw-rw-rw-   0        0        0     4738 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/weapons.json
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.822253 starrailcard-2.1.7/starrailcard/src/generator/
--rw-rw-rw-   0        0        0     6662 2024-04-20 04:28:23.000000 starrailcard-2.1.7/starrailcard/src/generator/style_profile_phone.py
--rw-rw-rw-   0        0        0    24567 2024-04-17 16:11:52.000000 starrailcard-2.1.7/starrailcard/src/generator/style_relict_score.py
--rw-rw-rw-   0        0        0    30356 2024-04-17 16:11:41.000000 starrailcard-2.1.7/starrailcard/src/generator/style_ticket.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.853301 starrailcard-2.1.7/starrailcard/src/model/
--rw-rw-rw-   0        0        0     4759 2024-04-13 14:26:08.000000 starrailcard-2.1.7/starrailcard/src/model/StarRailCard.py
--rw-rw-rw-   0        0        0    12254 2024-05-03 18:03:39.000000 starrailcard-2.1.7/starrailcard/src/model/api_mihomo.py
--rw-rw-rw-   0        0        0     4065 2024-03-13 13:47:58.000000 starrailcard-2.1.7/starrailcard/src/model/style.py
--rw-rw-rw-   0        0        0      493 2024-03-13 13:48:02.000000 starrailcard-2.1.7/starrailcard/src/model/ukrainization_model.py
--rw-rw-rw-   0        0        0      845 2024-03-13 13:48:07.000000 starrailcard-2.1.7/starrailcard/src/model/utils_model.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.898082 starrailcard-2.1.7/starrailcard/src/tools/
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.903716 starrailcard-2.1.7/starrailcard/src/tools/calculator/
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.908219 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.928892 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/
--rw-rw-rw-   0        0        0      373 2024-04-06 18:51:59.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/max.json
--rw-rw-rw-   0        0        0       49 2024-04-06 18:52:00.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/relic_id.json
--rw-rw-rw-   0        0        0     3434 2024-04-06 18:52:00.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/rolls.json
--rw-rw-rw-   0        0        0    92881 2024-04-06 18:52:01.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/score.json
--rw-rw-rw-   0        0        0     1959 2024-03-13 13:47:21.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/utils.py
--rw-rw-rw-   0        0        0     5802 2024-05-03 21:15:03.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/stats.py
--rw-rw-rw-   0        0        0     2526 2024-02-22 12:56:12.000000 starrailcard-2.1.7/starrailcard/src/tools/cashe.py
--rw-rw-rw-   0        0        0      709 2024-04-09 17:29:46.000000 starrailcard-2.1.7/starrailcard/src/tools/enums.py
--rw-rw-rw-   0        0        0    10136 2024-02-23 21:20:24.000000 starrailcard-2.1.7/starrailcard/src/tools/git.py
--rw-rw-rw-   0        0        0     9968 2024-04-29 22:09:02.000000 starrailcard-2.1.7/starrailcard/src/tools/http.py
--rw-rw-rw-   0        0        0      938 2024-04-09 16:56:51.000000 starrailcard-2.1.7/starrailcard/src/tools/json_data.py
--rw-rw-rw-   0        0        0     7017 2024-04-29 22:06:20.000000 starrailcard-2.1.7/starrailcard/src/tools/options.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.977480 starrailcard-2.1.7/starrailcard/src/tools/pill/
--rw-rw-rw-   0        0        0      224 2024-05-03 21:37:45.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/__init__.py
--rw-rw-rw-   0        0        0     3854 2024-02-22 12:55:07.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/color.py
--rw-rw-rw-   0        0        0     2330 2024-02-22 13:03:49.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/color_controle.py
--rw-rw-rw-   0        0        0     5367 2024-05-03 18:29:29.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/diagrama.py
--rw-rw-rw-   0        0        0     5518 2024-02-25 12:31:53.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/grandiend_v2.py
--rw-rw-rw-   0        0        0     3284 2024-02-22 12:55:28.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/grandient_v1.py
--rw-rw-rw-   0        0        0     5534 2024-04-29 22:03:56.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/image_controle.py
--rw-rw-rw-   0        0        0     5106 2024-02-22 12:55:59.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/style_editor.py
--rw-rw-rw-   0        0        0     2116 2024-02-22 13:01:14.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/text_controle.py
--rw-rw-rw-   0        0        0     2360 2024-03-13 13:31:40.000000 starrailcard-2.1.7/starrailcard/src/tools/translator.py
--rw-rw-rw-   0        0        0     6585 2024-02-22 12:57:06.000000 starrailcard-2.1.7/starrailcard/src/tools/treePaths.py
--rw-rw-rw-   0        0        0     1748 2024-03-28 18:26:54.000000 starrailcard-2.1.7/starrailcard/src/tools/ukrainization.py
--rw-rw-rw-   0        0        0     6884 2024-03-18 20:19:11.000000 starrailcard-2.1.7/starrailcard/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.977480 starrailcard-2.1.7/starrailcard.egg-info/
--rw-rw-rw-   0        0        0     4744 2024-05-03 21:39:14.000000 starrailcard-2.1.7/starrailcard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2051 2024-05-03 21:39:14.000000 starrailcard-2.1.7/starrailcard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 21:39:14.000000 starrailcard-2.1.7/starrailcard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-05-03 21:39:14.000000 starrailcard-2.1.7/starrailcard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-03 21:39:14.000000 starrailcard-2.1.7/starrailcard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.255601 starrailcard-2.1.8/
+-rw-rw-rw-   0        0        0     1721 2024-03-20 15:38:40.000000 starrailcard-2.1.8/LICENSE
+-rw-rw-rw-   0        0        0       38 2024-04-29 22:20:14.000000 starrailcard-2.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4762 2024-05-11 17:12:06.255601 starrailcard-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3642 2024-03-18 20:36:48.000000 starrailcard-2.1.8/README.md
+-rw-rw-rw-   0        0        0     1106 2024-04-18 21:49:53.000000 starrailcard-2.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 17:12:06.256600 starrailcard-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1571 2024-05-11 16:52:16.000000 starrailcard-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.203391 starrailcard-2.1.8/starrailcard/
+-rw-rw-rw-   0        0        0     1967 2024-05-11 17:11:19.000000 starrailcard-2.1.8/starrailcard/__init__.py
+-rw-rw-rw-   0        0        0    12655 2024-05-11 16:57:10.000000 starrailcard-2.1.8/starrailcard/client.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.193657 starrailcard-2.1.8/starrailcard/src/
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.225144 starrailcard-2.1.8/starrailcard/src/api/
+-rw-rw-rw-   0        0        0     3800 2024-05-10 18:40:10.000000 starrailcard-2.1.8/starrailcard/src/api/api.py
+-rw-rw-rw-   0        0        0     3487 2024-04-14 22:43:00.000000 starrailcard-2.1.8/starrailcard/src/api/enka.py
+-rw-rw-rw-   0        0        0    25187 2024-04-14 22:52:21.000000 starrailcard-2.1.8/starrailcard/src/api/enka_parsed.py
+-rw-rw-rw-   0        0        0      487 2024-04-09 16:19:13.000000 starrailcard-2.1.8/starrailcard/src/api/error.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.192657 starrailcard-2.1.8/starrailcard/src/assets/
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.225144 starrailcard-2.1.8/starrailcard/src/assets/font/
+-rw-rw-rw-   0        0        0   201292 2023-10-12 08:13:59.000000 starrailcard-2.1.8/starrailcard/src/assets/font/font_hsr.ttf
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.232653 starrailcard-2.1.8/starrailcard/src/data/
+-rw-rw-rw-   0        0        0     1751 2024-03-28 18:26:38.000000 starrailcard-2.1.8/starrailcard/src/data/avatar.json
+-rw-rw-rw-   0        0        0      252 2024-03-28 18:26:38.000000 starrailcard-2.1.8/starrailcard/src/data/element.json
+-rw-rw-rw-   0        0        0       70 2024-03-28 18:26:38.000000 starrailcard-2.1.8/starrailcard/src/data/keys.json
+-rw-rw-rw-   0        0        0      293 2024-03-28 18:26:38.000000 starrailcard-2.1.8/starrailcard/src/data/paths.json
+-rw-rw-rw-   0        0        0     1915 2024-03-28 18:26:38.000000 starrailcard-2.1.8/starrailcard/src/data/relict_sets.json
+-rw-rw-rw-   0        0        0     4947 2024-03-28 18:26:38.000000 starrailcard-2.1.8/starrailcard/src/data/stats.json
+-rw-rw-rw-   0        0        0     4738 2024-03-28 18:26:38.000000 starrailcard-2.1.8/starrailcard/src/data/weapons.json
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.235651 starrailcard-2.1.8/starrailcard/src/generator/
+-rw-rw-rw-   0        0        0    26040 2024-05-11 00:13:35.000000 starrailcard-2.1.8/starrailcard/src/generator/style_card.py
+-rw-rw-rw-   0        0        0     6675 2024-05-11 00:13:51.000000 starrailcard-2.1.8/starrailcard/src/generator/style_profile_phone.py
+-rw-rw-rw-   0        0        0    24833 2024-05-10 22:40:14.000000 starrailcard-2.1.8/starrailcard/src/generator/style_relict_score.py
+-rw-rw-rw-   0        0        0    30534 2024-05-10 22:32:55.000000 starrailcard-2.1.8/starrailcard/src/generator/style_ticket.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.237651 starrailcard-2.1.8/starrailcard/src/model/
+-rw-rw-rw-   0        0        0     4208 2024-05-10 18:23:13.000000 starrailcard-2.1.8/starrailcard/src/model/StarRailCard.py
+-rw-rw-rw-   0        0        0    12631 2024-05-10 22:14:10.000000 starrailcard-2.1.8/starrailcard/src/model/api_mihomo.py
+-rw-rw-rw-   0        0        0     8565 2024-05-10 22:49:33.000000 starrailcard-2.1.8/starrailcard/src/model/style.py
+-rw-rw-rw-   0        0        0      493 2024-03-13 13:48:02.000000 starrailcard-2.1.8/starrailcard/src/model/ukrainization_model.py
+-rw-rw-rw-   0        0        0      845 2024-03-13 13:48:07.000000 starrailcard-2.1.8/starrailcard/src/model/utils_model.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.244093 starrailcard-2.1.8/starrailcard/src/tools/
+-rw-rw-rw-   0        0        0     2526 2024-02-22 12:56:12.000000 starrailcard-2.1.8/starrailcard/src/tools/cache.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.245094 starrailcard-2.1.8/starrailcard/src/tools/calculator/
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.245094 starrailcard-2.1.8/starrailcard/src/tools/calculator/src/
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.247597 starrailcard-2.1.8/starrailcard/src/tools/calculator/src/assets/
+-rw-rw-rw-   0        0        0      373 2024-04-06 18:51:59.000000 starrailcard-2.1.8/starrailcard/src/tools/calculator/src/assets/max.json
+-rw-rw-rw-   0        0        0       49 2024-04-06 18:52:00.000000 starrailcard-2.1.8/starrailcard/src/tools/calculator/src/assets/relic_id.json
+-rw-rw-rw-   0        0        0     3434 2024-04-06 18:52:00.000000 starrailcard-2.1.8/starrailcard/src/tools/calculator/src/assets/rolls.json
+-rw-rw-rw-   0        0        0    92881 2024-04-06 18:52:01.000000 starrailcard-2.1.8/starrailcard/src/tools/calculator/src/assets/score.json
+-rw-rw-rw-   0        0        0     1959 2024-03-13 13:47:21.000000 starrailcard-2.1.8/starrailcard/src/tools/calculator/src/utils.py
+-rw-rw-rw-   0        0        0     5802 2024-05-03 21:15:03.000000 starrailcard-2.1.8/starrailcard/src/tools/calculator/stats.py
+-rw-rw-rw-   0        0        0      709 2024-04-09 17:29:46.000000 starrailcard-2.1.8/starrailcard/src/tools/enums.py
+-rw-rw-rw-   0        0        0    12292 2024-05-10 21:23:50.000000 starrailcard-2.1.8/starrailcard/src/tools/git.py
+-rw-rw-rw-   0        0        0     9968 2024-04-29 22:09:02.000000 starrailcard-2.1.8/starrailcard/src/tools/http.py
+-rw-rw-rw-   0        0        0      938 2024-04-09 16:56:51.000000 starrailcard-2.1.8/starrailcard/src/tools/json_data.py
+-rw-rw-rw-   0        0        0     8003 2024-05-11 00:30:12.000000 starrailcard-2.1.8/starrailcard/src/tools/options.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.253602 starrailcard-2.1.8/starrailcard/src/tools/pill/
+-rw-rw-rw-   0        0        0      220 2024-05-10 22:00:17.000000 starrailcard-2.1.8/starrailcard/src/tools/pill/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-05-10 22:00:17.000000 starrailcard-2.1.8/starrailcard/src/tools/pill/color.py
+-rw-rw-rw-   0        0        0     2328 2024-05-10 22:00:17.000000 starrailcard-2.1.8/starrailcard/src/tools/pill/color_control.py
+-rw-rw-rw-   0        0        0     5277 2024-05-10 21:27:12.000000 starrailcard-2.1.8/starrailcard/src/tools/pill/diagrama.py
+-rw-rw-rw-   0        0        0     5517 2024-05-10 21:26:51.000000 starrailcard-2.1.8/starrailcard/src/tools/pill/gradient_v2.py
+-rw-rw-rw-   0        0        0     3279 2024-05-10 22:00:17.000000 starrailcard-2.1.8/starrailcard/src/tools/pill/grandient_v1.py
+-rw-rw-rw-   0        0        0     5479 2024-05-10 21:26:30.000000 starrailcard-2.1.8/starrailcard/src/tools/pill/image_control.py
+-rw-rw-rw-   0        0        0     5717 2024-05-10 21:26:24.000000 starrailcard-2.1.8/starrailcard/src/tools/pill/style_editor.py
+-rw-rw-rw-   0        0        0     2116 2024-05-10 22:00:17.000000 starrailcard-2.1.8/starrailcard/src/tools/pill/text_control.py
+-rw-rw-rw-   0        0        0     2360 2024-03-13 13:31:40.000000 starrailcard-2.1.8/starrailcard/src/tools/translator.py
+-rw-rw-rw-   0        0        0     8286 2024-05-09 19:05:04.000000 starrailcard-2.1.8/starrailcard/src/tools/treePaths.py
+-rw-rw-rw-   0        0        0     1748 2024-03-28 18:26:54.000000 starrailcard-2.1.8/starrailcard/src/tools/ukrainization.py
+-rw-rw-rw-   0        0        0     6884 2024-05-10 22:00:17.000000 starrailcard-2.1.8/starrailcard/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:12:06.254601 starrailcard-2.1.8/starrailcard.egg-info/
+-rw-rw-rw-   0        0        0     4762 2024-05-11 17:12:06.000000 starrailcard-2.1.8/starrailcard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2088 2024-05-11 17:12:06.000000 starrailcard-2.1.8/starrailcard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 17:12:06.000000 starrailcard-2.1.8/starrailcard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-05-11 17:12:06.000000 starrailcard-2.1.8/starrailcard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-11 17:12:06.000000 starrailcard-2.1.8/starrailcard.egg-info/top_level.txt
```

### Comparing `starrailcard-2.1.7/LICENSE` & `starrailcard-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/PKG-INFO` & `starrailcard-2.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.1.7
+Version: 2.1.8
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
-Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai
+Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai,genshin,build,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
```

### Comparing `starrailcard-2.1.7/README.md` & `starrailcard-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/pyproject.toml` & `starrailcard-2.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/setup.py` & `starrailcard-2.1.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 	version=version,
 	author="DeviantUa",
 	author_email="deviantapi@gmail.com",
 	description= "This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.",
 	long_description=open("README.md", "r", encoding="utf-8").read(),
 	long_description_content_type="text/markdown",
 	url="https://github.com/DEViantUA/StarRailCard",
-	keywords = ["honkai", "cards", "generation", "honkaistarraill","raill", "starraill", "builds", "honkairail", "honkai"] ,
+	keywords = ["honkai", "cards", "generation", "honkaistarraill","raill", "starraill", "builds", "honkairail", "honkai", "genshin", "build", "api"] ,
 	packages=setuptools.find_packages(),
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 	],
 	install_requires=[
```

### Comparing `starrailcard-2.1.7/starrailcard/__init__.py` & `starrailcard-2.1.8/starrailcard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 __title__ = 'StarRailCard.py'
 __author__ = 'DeviantUa'
-__version__ = '2.1.7'
+__version__ = '2.1.8'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2024-present DeviantUa'
 
 from .client import *
 from .utils import *
 from .src.tools.enums import *
```

### Comparing `starrailcard-2.1.7/starrailcard/client.py` & `starrailcard-2.1.8/starrailcard/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 
 import anyio
+from typing import Union
 #import asyncio
 
-from .src.tools import http, ukrainization, options, translator, cashe, git
-from .src.generator import style_relict_score, style_ticket, style_profile_phone
+from .src.tools import cache, http, ukrainization, options, translator, git
+from .src.generator import style_relict_score, style_ticket, style_profile_phone, style_card
 from .src.api import api, enka
 from .src.model import StarRailCard,api_mihomo
-from .src.tools.pill import image_controle
+from .src.tools.pill import image_control
 
 
 
 class Card:
     def __init__(self, lang: str = "en", character_art = None, character_id = None, seeleland: bool = False,
                  user_font = None, save: bool = False, asset_save: bool = False, boost_speed: bool = False, remove_logo: bool = False,
-                 cashe = {"maxsize": 150, "ttl": 300}, enka: bool = False, api_data: api_mihomo.MiHoMoApi = None, proxy: str =  None, 
+                 cache = {"maxsize": 150, "ttl": 300}, enka: bool = False, api_data: api_mihomo.MiHoMoApi = None, proxy: str =  None, 
                  user_agent: str = None):
         """Main class for generating cards
 
         Args:
             lang (str, optional): Language in which generation will take place, supported languages: cht, cn, de, en, es, fr, id, jp, kr, pt, ru, th, vi, ua . Defaults to "en".
             character_art (dict, optional): A dictionary that contains a key - character id and link value (If you want to pass several images for 1 character, you can use list in the values). Defaults to None.
             character_id (str, optional): List character ids separated by commas. Defaults to None.
@@ -38,50 +39,49 @@
         self.character_art  = character_art
         self.character_id  = character_id
         self.seeleland = seeleland
         self.user_font = user_font
         self.save = save
         self.asset_save = asset_save
         self.remove_logo = remove_logo
-        self.cashe = cashe
+        self.cache = cache
         self.enka = enka
         self.boost_speed = boost_speed
         self.api_data = api_data
         self.proxy = proxy
         self.user_agent = options.get_user_agent(user_agent)
 
         
     async def __aenter__(self):
-        cashe.Cache.get_cache(maxsize = self.cashe.get("maxsize", 150), ttl = self.cashe.get("ttl", 300))
+        cache.Cache.get_cache(maxsize = self.cache.get("maxsize", 150), ttl = self.cache.get("ttl", 300))
         await http.AioSession.enter(self.proxy)
         
-        await git.ImageCache.set_assets_dowload(self.asset_save)
+        await git.ImageCache.set_assets_download(self.asset_save)
         
         if self.character_id:
             self.character_id = await options.get_charter_id(self.character_id)
         
         if self.character_art:
             if not isinstance(self.character_art, dict):
                 raise TypeError(4,"The character_art parameter must be a dictionary, where the key is the name of the character, and the parameter is an image.\nExample: character_art = {'1235': 'img.png', '1235': ['img.png','http.../img2.png']} or {'123596': 'img.png', '123854': 'http.../img2.png', ...}")
             else:
                 self.character_art = await options.get_character_art(self.character_art)
         
-        
         if not self.lang in translator.SUPPORTED_LANGUAGES:
             self.lang = "en"
         
         if self.lang == "ua":
             await ukrainization.TranslateDataManager().check_update()
         
         self.translateLang = translator.Translator(self.lang)
 
         if self.user_font:
             await git.change_font(font_path = self.user_font)
         
-        image_controle._boost_speed = self.boost_speed
+        image_control._boost_speed = self.boost_speed
 
         
         if self.remove_logo:
             print("""
                 Thank you for using our StarRailCard!
                 By removing the GitHub logo from the generated results, you acknowledge supporting the author through one of the following links:
                 - Patreon: https://www.patreon.com/deviantapi/membership
@@ -107,23 +107,23 @@
             self.lang = lang
         
         if lang == "ua":
             await ukrainization.TranslateDataManager().check_update()
         
         self.translateLang = translator.Translator(lang)
                 
-    async def set_user_font(self, user_font):
+    async def set_user_font(self, user_font: str):
         """Will install a custom font
 
         Args:
             user_font (srt): Font path or font name.
         """
         await git.change_font(font_path = user_font)
-    
-    async def creat_profile(self, uid, style = 1, hide_uid = False, background = None, force_update = False):
+
+    async def create_profile(self, uid: Union[int,str], style: bool = 1, hide_uid: bool = False, background = None, force_update: bool = False):
         """Function for generating a user profile card
 
         Args:
             uid (int): UID of the user in the game.
             style (int, optional): Card style. Defaults to 1.
             hide_uid (bool, optional): Hide UID. Defaults to False.
             background (str, optional): Link to custom card background. Defaults to None.
@@ -164,26 +164,26 @@
             "character_id": [],
         }
         
         if not str(style) in ["1"]:
             style = 1
             
         if style == 1:
-            response["card"] = await style_profile_phone.Creat(data,self.translateLang,self.character_art,hide_uid,uid,background, self.remove_logo).start()
+            response["card"] = await style_profile_phone.Create(data,self.translateLang,self.character_art,hide_uid,uid,background, self.remove_logo).start()
 
         for key in data.characters:
             response["character_id"].append(key.id)
             response["character_name"].append(key.name)
         
         if self.save:
             await options.save_card(uid,response["card"],"profile")
         
         return StarRailCard.StarRail(**response)
         
-    async def creat(self, uid, style = 1, hide_uid = False, force_update = False, style_settings = None):
+    async def create(self, uid: Union[int,str], style: bool = 1, hide_uid: bool = False, force_update: bool = False, style_settings = None, log: bool = False):
         """Function for generating character cards
 
         Args:
             uid (int): UID of the user in the game
             style (int, optional): Card style. Defaults to 1.
             hide_uid (bool, optional): Hide UID. Defaults to False.
             force_update (bool, optional): forced update of user data. Defaults to False.
@@ -204,15 +204,15 @@
                 data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update, user_agent= self.user_agent).get()
         else:
             data = self.api_data
 
         result = []
         
         style, style_settings = await options.style_setting(style, style_settings)
-        
+                
         try:
             player = data.player.model_dump()
         except:
             player = data.player
         
         response = {
             "settings": {
@@ -242,17 +242,19 @@
                                 return  
                         
                         art = None
                         if self.character_art:
                             if str(key.id) in self.character_art:
                                 art = self.character_art[str(key.id)]
                         if style == 1:
-                            result.append(await style_relict_score.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
+                            result.append(await style_relict_score.Create(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
                         elif style == 2:
-                            result.append(await style_ticket.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
+                            result.append(await style_ticket.Create(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
+                        elif style == 3:
+                            result.append(await style_card.Create(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
                     except Exception as e:
                         print(f"Error in get_result for character {key.id}: {e}")
                         
                 tasks.start_soon(get_result, key)
                     
         response["card"] = result
```

### Comparing `starrailcard-2.1.7/starrailcard/src/api/api.py` & `starrailcard-2.1.8/starrailcard/src/api/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ..tools import http, translator, ukrainization, options
 from ..model import api_mihomo
 from .error import StarRailCardError
 from ..tools.json_data import JsonManager
 from ..tools.enums import PathData
 
 _API_MIHOMO: str = "https://api.mihomo.me/sr_info_parsed/{uid}"
+_API_MIHOMO_NAKED: str = "https://api.mihomo.me/sr_info/{uid}"
 
 
 
 class ApiMiHoMo:
     """Class for interacting with the MiHoMo API."""
 
     def __init__(self, uid: str, lang: str = "en", v: int = 2, force_update: bool = False, user_agent: str = None, proxy = None) -> None:
@@ -25,27 +26,30 @@
         api_mihomo.UA_LANG = False
         if lang == "ua":
             self.ua_lang = True
             api_mihomo.UA_LANG = True
             
         self.v = v
 
+    async def recollect(self, data):
+        
+        pass
+    
     async def get(self) -> Optional[api_mihomo.MiHoMoApi]:
         """Get data from the MiHoMo API."""
         try:
             params = {
                 'lang': self.lang,
                 'is_force_update': str(self.force_update),
                 'version': f"v{self.v}"
             }
             
             headers = {
                 "User-Agent": self.user_agent
             }
-            
             data = await http.AioSession.get(_API_MIHOMO.format(uid=self.uid), headers = headers, params=params, proxy= self.proxy)
             
             if data is None:
                 raise StarRailCardError(4, "Failed to get data from API, please try again")
             
             if 'detail' in data:
                 detail = data['detail']
@@ -59,11 +63,28 @@
                     raise StarRailCardError(0, detail)
                 
         except aiohttp.ClientConnectionError:
             raise StarRailCardError(1, "Server is not responding")
         except aiohttp.ClientResponseError as e:
             raise StarRailCardError(e.status, f"Server returned status code {e.status}")
         
+        if data["player"]["space_info"].get("book_count") is None:
+            self.dop_info = await http.AioSession.get(_API_MIHOMO_NAKED.format(uid=self.uid), headers = headers, params=params, proxy= self.proxy)
+            data = await self.add_info(data)
+        
         if self.ua_lang:
             await ukrainization.TranslateDataManager().load_translate_data()
         
-        return api_mihomo.MiHoMoApi(player=data["player"], characters=data["characters"], dont_update_link= False)
+        return api_mihomo.MiHoMoApi(player=data["player"], characters=data["characters"], dont_update_link= False)
+    
+    async def add_info(self, data):
+        info = self.dop_info["detailInfo"]["recordInfo"]
+        
+        data["player"]["space_info"]["relicCount"] = info.get("relicCount", 0)
+        data["player"]["space_info"]["musicCount"] = info.get("musicCount", 0)
+        data["player"]["space_info"]["bookCount"] = info.get("bookCount", 0)
+        
+        memory_data = info.get("challengeInfo", {})
+        data["player"]["space_info"]["memory_data"]["abyssStarCount"] = memory_data.get("abyssStarCount")
+        data["player"]["space_info"]["memory_data"]["abyssLevel"] = memory_data.get("abyssLevel")
+        
+        return data
```

### Comparing `starrailcard-2.1.7/starrailcard/src/api/enka.py` & `starrailcard-2.1.8/starrailcard/src/api/enka.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/api/enka_parsed.py` & `starrailcard-2.1.8/starrailcard/src/api/enka_parsed.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/assets/font/font_hsr.ttf` & `starrailcard-2.1.8/starrailcard/src/assets/font/font_hsr.ttf`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/data/avatar.json` & `starrailcard-2.1.8/starrailcard/src/data/avatar.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/data/relict_sets.json` & `starrailcard-2.1.8/starrailcard/src/data/relict_sets.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/data/stats.json` & `starrailcard-2.1.8/starrailcard/src/data/stats.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/data/weapons.json` & `starrailcard-2.1.8/starrailcard/src/data/weapons.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/generator/style_profile_phone.py` & `starrailcard-2.1.8/starrailcard/src/generator/style_profile_phone.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,42 +5,42 @@
 import asyncio
 import random
 from PIL import ImageDraw,Image,ImageChops
 from ..tools import pill, git, options
 
 _of = git.ImageCache()
 
-class Creat:
+class Create:
     def __init__(self,profile,lang,img,hide,uid,background, remove_logo) -> None:
         self.remove_logo = remove_logo
         self.profile = profile
         self.lang = lang
         self.img = img
         self.hide = hide
         self.uid = uid
         self.background = background
     
-    async def creat_background(self):
+    async def create_background(self):
         self.background_profile = Image.new("RGBA", (828, 1078), (0,0,0,0))
         
-        maska,frame = await asyncio.gather(_of.maska_prof_bg,_of.menu)
+        mask,frame = await asyncio.gather(_of.maska_prof_bg,_of.menu)
         if self.background is None:
             background_image = random.choice([await _of.bg_1, await  _of.bg_2, await  _of.bg_3, await  _of.bg_5])
             background_shadow = Image.new("RGBA", (828, 1078), (0,0,0,100))
         else:
-            background_image = await pill.get_dowload_img(self.background)
-            background_image = await pill.get_centr_size((828,1078),background_image)
+            background_image = await pill.get_download_img(self.background)
+            background_image = await pill.get_center_size((828,1078),background_image)
             background_shadow = Image.new("RGBA", (828, 1078), (0,0,0,150))
         background_image = background_image.convert("RGBA")
         background_image.alpha_composite(background_shadow)
-        self.background_profile.paste(background_image,(0,0),maska.convert("L"))
+        self.background_profile.paste(background_image,(0,0),mask.convert("L"))
         self.background_profile.alpha_composite(frame)
         
 
-    async def creat_charter(self,key):
+    async def create_charter(self,key):
         if key.rarity == 5:
             charter_profile = await _of.avatar_five
         else:
             charter_profile = await _of.avatar_four
         
         charter_profile = charter_profile.copy()
         
@@ -48,37 +48,37 @@
             if str(key.id) in self.img:
                 url_id = self.img[str(key.id)]
             else:
                 url_id = f'https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/icon/avatar/{key.id}.png'
         else:
             url_id = f'https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/icon/avatar/{key.id}.png'
             
-        splash,mask = await asyncio.gather(pill.get_dowload_img(url_id),_of.maska_character)
-        splash = await pill.get_centr_size((109,109),splash)
+        splash,mask = await asyncio.gather(pill.get_download_img(url_id),_of.maska_character)
+        splash = await pill.get_center_size((109,109),splash)
         charter_profile.paste(splash,(16,28),mask.convert("L"))
         name = await pill.create_image_with_text(key.name,16, max_width=123, color=(255, 255, 255, 255)) 
         
         charter_profile.alpha_composite(name,(136,int(49-name.size[1]/2)))       
 
         max_level = options.max_lvl(key.promotion)
         level = f"{self.lang.lvl}: {key.level}/{max_level}"
         
-        element_icon = await pill.get_dowload_img(key.element.icon, size=(28,28))
-        path_icon = await pill.get_dowload_img(key.path.icon, size=(28,28))
+        element_icon = await pill.get_download_img(key.element.icon, size=(28,28))
+        path_icon = await pill.get_download_img(key.path.icon, size=(28,28))
         
         charter_profile.alpha_composite(path_icon,(263,28))
         charter_profile.alpha_composite(element_icon,(293,28))
         
         
         d = ImageDraw.Draw(charter_profile)
         d.text((19,7), level, font= self.font_charter, fill=(255,255,255,255))
         
         
         if not key.light_cone is None:
-            icon = await pill.get_dowload_img(key.light_cone.icon, size = (66,66))
+            icon = await pill.get_download_img(key.light_cone.icon, size = (66,66))
             charter_profile.alpha_composite(icon,(136,70))
             d.text((201,95), f"{self.lang.lvl}: {key.light_cone.level}/{options.max_lvl(key.light_cone.promotion)}", font=self.font_charter, fill=(255, 255, 255, 255))
             starts = await options.get_stars(key.light_cone.rarity)
             charter_profile.alpha_composite(starts.resize((85,18)),(224,114))
             
             background = await _of.light_cone_ups
             background = background.copy()
@@ -92,23 +92,23 @@
             charter_profile.alpha_composite(background.resize((17,17)), (202,114))
             
         return charter_profile
     
     async def get_charter(self):
         task = []
         for key in self.profile.characters:
-            task.append(self.creat_charter(key))
+            task.append(self.create_charter(key))
             
         self.charter = await asyncio.gather(*task)
     
-    async def creat_avatar(self):
+    async def create_avatar(self):
         self.background_profile_avatar = Image.new("RGBA", (625, 254), (0,0,0,0))
         avatar = self.profile.player.avatar.icon
             
-        avatar,font_20,desc_frame = await asyncio.gather(pill.get_dowload_img(avatar, size= (134,134)),pill.get_font(18),_of.desc_frame)
+        avatar,font_20,desc_frame = await asyncio.gather(pill.get_download_img(avatar, size= (134,134)),pill.get_font(18),_of.desc_frame)
             
         self.background_profile_avatar.alpha_composite(avatar)
         
         d = ImageDraw.Draw(self.background_profile_avatar)
         
         level = f"{self.lang.lvl}: {self.profile.player.level}"
         Wlevel = f"{self.lang.WL}: {self.profile.player.world_level}"
@@ -143,11 +143,11 @@
             self.background_profile.alpha_composite(logo,(752,0))
                 
     async def start(self):
         
         _of.set_mapping(3)
         self.font_charter = await pill.get_font(13)
         
-        await asyncio.gather(self.creat_background(), self.get_charter(), self.creat_avatar())
+        await asyncio.gather(self.create_background(), self.get_charter(), self.create_avatar())
         await self.build()        
         
         return self.background_profile
```

### Comparing `starrailcard-2.1.7/starrailcard/src/generator/style_relict_score.py` & `starrailcard-2.1.8/starrailcard/src/generator/style_relict_score.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,57 +25,57 @@
     if x == 5:
         return await _of.light_cone_frame_five
     elif x == 4:
         return await _of.light_cone_frame_four
     else:
         return await _of.light_cone_frame_three
 
-class Creat:
+class Create:
     def __init__(self, data, lang, art, hide_uid, uid, seeleland,remove_logo) -> None:
         self.remove_logo = remove_logo
         self.data = data
         self.lang = lang
-        self.art = art #Image.open("modified_exampl.gif")#art
+        self.art = art
         self.hide_uid = hide_uid
         self.uid = uid
         
         self.gif = False
         self.GIFT_BG = []
         
         self.seeleland = seeleland
-        self.totall_eff = 0
+        self.total_eff = 0
         self.element_color = self.data.element.color.rgba
     
-    async def creat_bacground(self):
-        self.background = Image.new(RelictScore.RGBA, RelictScore.bacground_size, (0,0,0,0))
-        background_dark = Image.new(RelictScore.RGBA, RelictScore.bacground_size, (0,0,0,100))
-        background_art = Image.new(RelictScore.RGBA, RelictScore.bacground_size, (0,0,0,0))
-        background_blur = Image.new(RelictScore.RGBA, RelictScore.bacground_size, (0,0,0,0))
+    async def create_bacground(self):
+        self.background = Image.new(RelictScore.RGBA, RelictScore.background_size, (0,0,0,0))
+        background_dark = Image.new(RelictScore.RGBA, RelictScore.background_size, (0,0,0,100))
+        background_art = Image.new(RelictScore.RGBA, RelictScore.background_size, (0,0,0,0))
+        background_blur = Image.new(RelictScore.RGBA, RelictScore.background_size, (0,0,0,0))
         lines = await _of.background_line
         logo = await _of.LOGO_GIT
         shadow = await _of.background_shadow
         maska_art = await _of.background_maska_art
         background_overlay = await _of.background_overlay
         background_maska_blur = await _of.background_maska_blur
         background_default = await _of.background_default
                 
         if self.art:
-            user_image = await pill.get_centr_size(RelictScore.art_size, self.art)
-            bg = await pill.GradientGenerator(user_image).generate(1,RelictScore.bacground_size[1])       
-            bg = bg.resize(RelictScore.bacground_size)
+            user_image = await pill.get_center_size(RelictScore.art_size, self.art)
+            bg = await pill.GradientGenerator(user_image).generate(1,RelictScore.background_size[1])       
+            bg = bg.resize(RelictScore.background_size)
             user_image_op = await pill.apply_opacity(user_image, opacity = RelictScore.opacity_art)
 
             background_blur.alpha_composite(bg.convert("RGBA"))
             background_blur.alpha_composite(user_image_op)
             
             background_blur = background_blur.filter(ImageFilter.GaussianBlur(RelictScore.blur_art))
             line,self.element_color = await pill.recolor_image(lines, self.element_color[:3], light = True)            
         else:
             bg = background_default.copy() 
-            user_image = await pill.get_centr_scale(RelictScore.splash_size, await pill.get_dowload_img(self.data.portrait))
+            user_image = await pill.get_center_scale(RelictScore.splash_size, await pill.get_download_img(self.data.portrait))
             user_image_op = await pill.apply_opacity(user_image, opacity = RelictScore.opacity_splash)
             background_blur.alpha_composite(bg.convert("RGBA"))
             background_blur.alpha_composite(user_image_op)
             background_blur = background_blur.filter(ImageFilter.GaussianBlur(RelictScore.blur_splashart))
             line = await pill.recolor_image(lines, self.element_color[:3])
             
         background_blur.alpha_composite(background_dark)
@@ -88,28 +88,28 @@
         self.background.paste(background_art,(0,0),maska_art.convert("L"))
         self.background.alpha_composite(shadow)
         self.background.alpha_composite(line, (RelictScore.position_line))
         if not self.remove_logo:
             self.background.alpha_composite(logo)
         
         if not self.hide_uid:
-            uid = Image.new(RelictScore.RGBA, RelictScore.bacground_size, (0,0,0,0))
+            uid = Image.new(RelictScore.RGBA, RelictScore.background_size, (0,0,0,0))
             d = ImageDraw.Draw(uid)
             
             font_10 = await pill.get_font(RelictScore.font_uid)
             d.text((0,0), f"UID: {self.uid}", font=font_10, fill=(255, 255, 255, 75))
             self.background.alpha_composite(uid,RelictScore.position_uid)
     
-    async def creat_light_cone(self):
+    async def create_light_cone(self):
         self.background_light_cones = Image.new(RelictScore.RGBA, (330, 190), (0, 0, 0, 0))
         if self.data.light_cone is None:
             return
         
         background = Image.new(RelictScore.RGBA, (139, 190), (0, 0, 0, 0))
-        image = await pill.get_dowload_img(self.data.light_cone.portrait, size=(118, 169))
+        image = await pill.get_download_img(self.data.light_cone.portrait, size=(118, 169))
         background.alpha_composite(image,(9,9))
         light_cone_frame_stars = await get_cone_frame(self.data.light_cone.rarity)
         background.alpha_composite(light_cone_frame_stars)
         light_cone_frame = await _of.light_cone_frame
         background.alpha_composite(light_cone_frame)
         
         self.background_light_cones.alpha_composite(background)
@@ -142,15 +142,15 @@
         names = await pill.create_image_with_text(self.data.light_cone.name, 18, max_width=180, color=(255, 255, 255, 255))
         line = Image.new("RGBA", (1,48), options.color_lc_line.get(str(self.data.light_cone.rarity), (150, 202, 255, 255)))
         
         
         self.background_light_cones.alpha_composite(line,(140,9))
         self.background_light_cones.alpha_composite(names,(146,int(34-names.size[1]/2)))   
     
-    async def creat_stats(self):
+    async def create_stats(self):
         self.background_stats = Image.new(RelictScore.RGBA, (563, 290), (0, 0, 0, 0))
 
         combined_attributes = {}
         dop = {}
 
         for attribute in self.data.attributes + self.data.additions:
             field = attribute.field
@@ -161,26 +161,26 @@
                 dop[field] = {"main": attribute.display, "dop": 0}
                 combined_attributes[field] = attribute
 
         dop = {key: value for key, value in dop.items() if value['dop'] != 0}
         
         xp,y = 0,0
 
-        async for i, background in pill.creat_stats(combined_attributes, dop, 
+        async for i, background in pill.create_stats(combined_attributes, dop, 
                       RelictScore.stat_font_dop,RelictScore.stat_font,
                       RelictScore.stat_line_size, RelictScore.stat_name_size, RelictScore.stat_max_width, RelictScore.stat_icon_size,
                       RelictScore.stat_icon_position, RelictScore.stat_name_position, RelictScore.stat_x_position,
                       self.element_color, RelictScore.stat_value_font):
             self.background_stats.alpha_composite(background,(xp,y))
             y += 45
             if i == 5:
                 xp = 290
                 y = 0
  
-    async def creat_name(self):
+    async def create_name(self):
         self.background_name = Image.new(RelictScore.RGBA, RelictScore.name_size, (0, 0, 0, 0))
         d = ImageDraw.Draw(self.background_name)
         names = await pill.create_image_with_text(self.data.name, RelictScore.font_name_size , max_width=RelictScore.name_with, color= RelictScore.name_color)
         if names.size[1] <= RelictScore.name_h_max:
             self.background_name.alpha_composite(names,(RelictScore.name_position,int(RelictScore.name_h_max-names.size[1]/2)))
         else:
             self.background_name.alpha_composite(names,(RelictScore.name_position,int(RelictScore.name_h_min-names.size[1]/2)))
@@ -188,93 +188,93 @@
         font_17 = await pill.get_font(RelictScore.font_name_level)
         max_level = options.max_lvl(self.data.promotion)
         level = f"{self.lang.lvl}: {self.data.level}/{max_level}"
         d.text(RelictScore.position_name_level, level, font=font_17, fill= RelictScore.color_name_level)
         starts = await options.get_stars(self.data.rarity)
         self.background_name.alpha_composite(starts,RelictScore.position_name_star)
        
-    async def creat_constant(self):
+    async def create_constant(self):
         self.background_skills = Image.new(RelictScore.RGBA, RelictScore.constant_size_background, (0, 0, 0, 0))
         x = 0
         rank = self.data.rank
         for key in self.data.rank_icons[:rank]:
             bg = Image.new(RelictScore.RGBA, RelictScore.constant_size, (0, 0, 0, 0))
-            icon = await pill.get_dowload_img(key, size=RelictScore.constant_size_icon)
+            icon = await pill.get_download_img(key, size=RelictScore.constant_size_icon)
             icon_blur = icon.filter(ImageFilter.GaussianBlur(RelictScore.constant_blur))
             icon_blur = await pill.recolor_image(icon_blur, self.element_color[:3])
             bg.alpha_composite(icon_blur,RelictScore.constant_icon_position)
             bg.alpha_composite(icon,RelictScore.constant_icon_position)
             self.background_skills.alpha_composite(bg,(x,0))
             x += 68
 
         for key in self.data.rank_icons[rank:]:
             bg = Image.new(RelictScore.RGBA, RelictScore.constant_size, (0, 0, 0, 0))
-            icon = await pill.get_dowload_img(key, size= RelictScore.constant_size_icon)
+            icon = await pill.get_download_img(key, size= RelictScore.constant_size_icon)
             icon = await pill.apply_opacity(icon, opacity=RelictScore.constant_size_icon_opacity)
             bg.alpha_composite(icon,RelictScore.constant_icon_position)
             self.background_skills.alpha_composite(bg,(x,0))
             x += 68
      
-    async def creat_relict_sets(self):
+    async def create_relict_sets(self):
         rel_set = options.calculator_relict_sets(self.data.relic_sets)
 
         self.background_sets = Image.new(RelictScore.RGBA, RelictScore.sets_background, (0,0,0,0))
         
-        font = await pill.get_font(RelictScore.setst_font)
+        font = await pill.get_font(RelictScore.sets_font)
         
         line_items = []
         i = 0
         for key in rel_set:
             sets = rel_set[key]
-            holst_line = Image.new(RelictScore.RGBA, RelictScore.setst_line_size, (0,0,0,0))
+            holst_line = Image.new(RelictScore.RGBA, RelictScore.sets_line_size, (0,0,0,0))
             background_count = await _of.relict_count_sets
             background_count = background_count.copy()
             d = ImageDraw.Draw(background_count)
-            d.text(RelictScore.setst_count_position, str(sets["num"]), font=font, fill= RelictScore.setst_name_color)
+            d.text(RelictScore.sets_count_position, str(sets["num"]), font=font, fill= RelictScore.sets_name_color)
             d = ImageDraw.Draw(holst_line)
             sets_name_font,size = await pill.get_text_size_frame(sets["name"],15,492)
             if key[:1] == "1":
                 holst_line.alpha_composite(background_count)
-                d.text((36, 4), sets["name"], font=sets_name_font, fill=RelictScore.setst_name_color)
+                d.text((36, 4), sets["name"], font=sets_name_font, fill=RelictScore.sets_name_color)
                 line_items.append({"setap": i, "line": holst_line})
                 i += 1
             else:
-                holst_line.alpha_composite(background_count,(532,0))
-                d.text((int(521-size), 4), sets["name"], font=sets_name_font, fill=RelictScore.setst_name_color)
+                holst_line.alpha_composite(background_count,(530 - background_count.size[0],0))
+                d.text((int(521 - background_count.size[0] -size), 4), sets["name"], font=sets_name_font, fill=RelictScore.sets_name_color)
                 line_items.append({"setap": 1, "line": holst_line})
                 
         for key in line_items:
             if key["setap"] == 1:
                 self.background_sets.alpha_composite(key["line"],(0,29))
             elif key["setap"] == 2:
                 self.background_sets.alpha_composite(key["line"],(0,29))
             else:
                 self.background_sets.alpha_composite(key["line"],(0,0))
     
-    async def creat_relict(self,relict):
+    async def create_relict(self,relict):
         background_main = Image.new(RelictScore.RGBA,RelictScore.relict_size, (0,0,0,0))
         background = Image.new(RelictScore.RGBA,RelictScore.relict_size, (0,0,0,0))
         background_image = Image.new("RGBA",RelictScore.relict_size, (0,0,0,0))
         relict_frame = await _of.relict_frame
         relict_maska = await _of.relict_maska
         relict_score_frame = await _of.relict_score_frame
         relict_line = await _of.relict_line
         
         background_main.alpha_composite(relict_frame)
         
-        image = await pill.get_dowload_img(relict.icon, size= RelictScore.relict_icon_size)
+        image = await pill.get_download_img(relict.icon, size= RelictScore.relict_icon_size)
         background_image.alpha_composite(image,RelictScore.relict_icon_position)
         background.paste(background_image,(0,0),relict_maska.convert("L"))
         
         background_main.alpha_composite(relict_score_frame,(8,0))
         background_main.alpha_composite(background)
         background_main.alpha_composite(relict_line)
         score = self.score_info["score"].get(str(relict.id),_DEFAULT_SCORE)
         
-        main_stat_icon = await pill.get_dowload_img(relict.main_affix.icon, size= RelictScore.relict_main_stat_icon_size)
+        main_stat_icon = await pill.get_download_img(relict.main_affix.icon, size= RelictScore.relict_main_stat_icon_size)
         color = options.color_element.get(relict.main_affix.type, None)
         if not color is None:
             main_stat_icon = await pill.recolor_image(main_stat_icon, color[:3])
         stars = await options.get_stars(relict.rarity, type = 1)
         
         background_main.alpha_composite(stars,RelictScore.relict_position_star)
         background_main.alpha_composite(main_stat_icon,RelictScore.relict_main_stat_icon_position)
@@ -293,15 +293,15 @@
         y_icon = 21
         y_roll = 30
         y_text = 27
                 
         eff = 0
         
         for k in relict.sub_affix:
-            icon = await pill.get_dowload_img(k.icon, size=RelictScore.relict_sub_icon_size)
+            icon = await pill.get_download_img(k.icon, size=RelictScore.relict_sub_icon_size)
             background_main.alpha_composite(icon,(142,y_icon))
             scoreR = score["rolls"].get(k.type,0)
             if k.type in self.score_info["bad"]:
                 d.text((173, y_text), str(k.display), font=font_18, fill= (255,255,255,255))
             else:
                 eff += 1
                 d.text((173, y_text), str(k.display), font=font_18, fill= options.color_scoreR.get(scoreR,(255,255,255,255)))
@@ -315,25 +315,25 @@
         
         d.text((105, 4), "Rank:", font=font_14, fill = (255,255,255,255))
         d.text((149, 4), str(score["rank"]["name"]), font=font_14, fill = score["rank"]["color"])
         
         d.text((187, 4), "Eff Stat:", font=font_14, fill = (255,255,255,255))
         d.text((247, 4), str(eff), font=font_14, fill = options.color_scoreR.get(eff,(255,255,255,255)))
         
-        self.totall_eff += eff
+        self.total_eff += eff
         
         line_f = await _of.relict_frame_line
         line_f = line_f.copy()
         line_f = await pill.recolor_image(line_f, self.element_color[:3])
         background_main.alpha_composite(line_f,(0,21))
         
         return {"position": str(relict.id)[-1:] , "img": background_main}
     
     async def get_path(self):
-        self.background_path = await pill.creat_path(self.data)
+        self.background_path = await pill.create_path(self.data)
     
     async def get_score(self):
         self.score_info = await stats.Calculator(self.data).start()
         
     async def build_relict(self):
         self.background_relict = Image.new(RelictScore.RGBA, (1131,297), (0,0,0,0))
         none_relict = await _of.none_relict
@@ -355,15 +355,15 @@
         for key in map:
             if map[key] is None:
                 self.background_relict.alpha_composite(none_relict, position.get(key))
 
         self.background_relict.alpha_composite(self.background_score,(0,112))
         self.background_relict.alpha_composite(self.background_sets,(0,45))
     
-    async def creat_seeleland(self):
+    async def create_seeleland(self):
         self.seelelen = Image.new("RGBA",(1,1), (0,0,0,0))
         
         if self.seeleland:
             self.seelelen = await _of.seeleland_v2
             self.seelelen = self.seelelen.copy()
             font = await pill.get_font(15)
             data = await options.get_seeleland(self.uid, self.data.id)
@@ -374,15 +374,15 @@
                 self.seelelen = Image.new("RGBA",(1,1), (0,0,0,0))
                 return None
             draw = ImageDraw.Draw(self.seelelen)
             draw.text((143, 7), str(data["sc"]), font=font, fill=(255, 255, 255, 255))
             draw.text((136, 24), f'{data["rank"][:-2]}..', font=font, fill=(255, 255, 255, 255))
             draw.text((127, 42), data["percrank"].replace("top ", ""), font=font, fill=(255, 255, 255, 255))
     
-    async def creat_score_total(self):
+    async def create_score_total(self):
         self.background_score = Image.new("RGBA",(559,43), (0,0,0,0))
         
         sclor_bg = await _of.relict_backgroundl_score_line
         sclor_bg = sclor_bg.copy()
         sclor_bg_color = await _of.relict_full_score_line
         sclor_bg_color = sclor_bg_color.copy()
         sclor_bg_color = await pill.recolor_image(sclor_bg_color, self.element_color[:3])
@@ -412,25 +412,25 @@
         d.text((249, -2), "Score:", font=font_21, fill = (255,255,255,255))
         d.text((320, -2), str(self.score_info["total_score"]['count']), font=font_21, fill = self.score_info["total_score"]["rank"]["color"])
         
         d.text((17, -2), "Summary Rank:", font=font_21, fill = (255,255,255,255))
         d.text((189, -2), str(self.score_info["total_score"]["rank"]["name"]), font=font_21, fill = self.score_info["total_score"]["rank"]["color"])
         
         d.text((393, -2), "Eff Stat:", font=font_21, fill = (255,255,255,255))
-        d.text((497, -2), str(self.totall_eff), font=font_21, fill = options.color_scoreR.get(self.totall_eff,(255,255,255,255)))   
+        d.text((497, -2), str(self.total_eff), font=font_21, fill = options.color_scoreR.get(self.total_eff,(255,255,255,255)))   
     
     async def build(self):
-        bg = Image.new(RelictScore.RGBA, RelictScore.bacground_size, (0,0,0,0))
-        bg.alpha_composite(self.background_light_cones,(782,16))
-        bg.alpha_composite(self.background_stats,(781,220))
-        bg.alpha_composite(self.background_name,(6,654))
-        bg.alpha_composite(self.background_skills.resize((320,47)),(1033,134))
-        bg.alpha_composite(self.background_path.resize((488,428)),(1409,16))
-        bg.alpha_composite(self.background_relict,(781,473))
-        bg.alpha_composite(self.seelelen,(1120,35))
+        bg = Image.new(RelictScore.RGBA, RelictScore.background_size, (0,0,0,0))
+        bg.alpha_composite(self.background_light_cones,RelictScore.build_lc_position)
+        bg.alpha_composite(self.background_stats,RelictScore.build_stats_position)
+        bg.alpha_composite(self.background_name,RelictScore.build_name_position)
+        bg.alpha_composite(self.background_skills.resize(RelictScore.build_constant_size),RelictScore.build_constant_position)
+        bg.alpha_composite(self.background_path.resize(RelictScore.build_skill_size),RelictScore.build_skill_position)
+        bg.alpha_composite(self.background_relict,RelictScore.build_relict_position)
+        bg.alpha_composite(self.seelelen,RelictScore.build_seelelen_position)
         
         if self.gif:
             self.background = []
             for key in self.GIFT_BG:
                 key.alpha_composite(bg)
                 self.background.append(key.convert("RGB"))
         else:
@@ -454,59 +454,61 @@
                     if color:
                         self.element_color = await pill.get_colors(frame.convert("RGBA"), 15, common=True, radius=5, quality=800)
                         color = False
                     if frame_count >= 50:
                         break
                     if frame_count % n != 0:
                         self.art = frame.convert("RGBA")
-                        await self.creat_bacground()
+                        await self.create_bacground()
                         self.GIFT_BG.append(self.background.copy())
                     frame_count += 1            
         else:
             if self.art:
                 self.element_color = await pill.get_colors(self.art, 15, common=True, radius=5, quality=800)
             
-            await self.creat_bacground()
+            await self.create_bacground()
+        
+        
         
         async with anyio.create_task_group() as tasks:
-            tasks.start_soon(self.creat_light_cone)
-            tasks.start_soon(self.creat_stats)
-            tasks.start_soon(self.creat_name)
-            tasks.start_soon(self.creat_constant)
-            tasks.start_soon(self.creat_relict_sets)
+            tasks.start_soon(self.create_light_cone)
+            tasks.start_soon(self.create_stats)
+            tasks.start_soon(self.create_name)
+            tasks.start_soon(self.create_constant)
+            tasks.start_soon(self.create_relict_sets)
             tasks.start_soon(self.get_score)
             tasks.start_soon(self.get_path)
-            tasks.start_soon(self.creat_seeleland)
+            tasks.start_soon(self.create_seeleland)
         
         async def wait_all(*funcs):
             results = [None] * len(funcs)
             
             async with anyio.create_task_group() as tasks:
                 async def process(func, i):
                     results[i] = await func()
                 
                 for i, func in enumerate(funcs):
                     tasks.start_soon(process, func, i)
             
             return results
-        
+
         self.relict = await wait_all(*[
-            functools.partial(self.creat_relict, key)
+            functools.partial(self.create_relict, key)
             for key in self.data.relics
         ])
                 
-        await self.creat_score_total()
+        await self.create_score_total()
         
         await self.build_relict()
         await self.build()
         
         data = {
             "id": self.data.id,
             "animation":  self.gif,
             "name": self.data.name,
             "rarity": self.data.rarity,
             "card": self.background,
-            "size": RelictScore.bacground_size,
+            "size": RelictScore.background_size,
             "color": self.element_color
         }
         
         return data
```

### Comparing `starrailcard-2.1.7/starrailcard/src/generator/style_ticket.py` & `starrailcard-2.1.8/starrailcard/src/generator/style_ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,96 +20,93 @@
                     }
 }
 
 _of = git.ImageCache()
 _of.set_mapping(2)
 
 
-class Creat:
+class Create:
     def __init__(self, data, lang, art, hide_uid, uid, seeleland, remove_logo) -> None:
         self.data = data
         self.remove_logo = remove_logo
         self.lang = lang
         self.art = art
         self.hide_uid = hide_uid
         self.uid = uid
         self.seeleland = seeleland
-        self.totall_eff = 0
-        self.seeleland = seeleland
+        self.total_eff = 0
         self.element_color = self.data.element.color.rgba
         self.gif = False
         self.GIFT_BG = []
         
-    async def creat_bacground(self):
-        self.background = Image.new(Ticket.RGBA, Ticket.bacground_size, (0,0,0,0))
-        background_splash = Image.new(Ticket.RGBA, Ticket.background_splash_size, Ticket.bacground_default_color)
+    async def create_background(self):
+        self.background = Image.new(Ticket.RGBA, Ticket.background_size, (0,0,0,0))
+        background_splash = Image.new(Ticket.RGBA, Ticket.background_splash_size, Ticket.background_default_color)
         background_dark = Image.new(Ticket.RGBA, Ticket.background_splash_size, (0,0,0,100))       
         
         line = await _of.background_line
         logo = await _of.LOGO_GIT_INV
         shadow = await _of.background_shadow
         splash = True
         background_overlay = await _of.background_overlay
         
         if self.art:
-            user_image = await pill.get_centr_size(Ticket.art_size, self.art)
-            self.background = pill.grandiend_v2.GrandientBackground(user_image,(1,Ticket.bacground_size[1])).start(left= True,overlay_add = False)
+            user_image = await pill.get_center_size(Ticket.art_size, self.art)
+            self.background = pill.gradient_v2.GradientBackground(user_image,(1,Ticket.background_size[1])).start(left= True,overlay_add = False)
             line,self.element_color = await pill.recolor_image(line, self.element_color[:3], light = True)
             
                 
-            self.background = self.background.resize(Ticket.bacground_size)
+            self.background = self.background.resize(Ticket.background_size)
             position_art = Ticket.position_art
             splash = False
             self.background = ImageChops.soft_light(self.background, background_overlay.convert(Ticket.RGBA))
             ll = await pill.light_level(self.element_color)
             if ll > 0.6:
                 self.background.alpha_composite(background_dark)
         else:
-            self.background = Image.new(Ticket.RGBA, Ticket.bacground_size, Ticket.bacground_default_color)
-            user_image = await pill.get_centr_scale(Ticket.splash_size, await pill.get_dowload_img(self.data.portrait))
+            self.background = Image.new(Ticket.RGBA, Ticket.background_size, Ticket.background_default_color)
+            user_image = await pill.get_center_scale(Ticket.splash_size, await pill.get_download_img(self.data.portrait))
             position_art = Ticket.position_splash_art
-            
-        
-        
+
         self.background.alpha_composite(user_image.convert(Ticket.RGBA),position_art)
         if splash:
             self.background.alpha_composite(background_splash)
         self.background.alpha_composite(line,Ticket.position_line)
         self.background.alpha_composite(shadow,Ticket.position_shadow)
         if not self.remove_logo:
             self.background.alpha_composite(logo,(1845,0))
         
         if not self.hide_uid:
-            uid = Image.new(Ticket.RGBA, Ticket.bacground_size, (0,0,0,0))
+            uid = Image.new(Ticket.RGBA, Ticket.background_size, (0,0,0,0))
             d = ImageDraw.Draw(uid)
             
             font_10 = await pill.get_font(Ticket.font_uid)
             d.text((0,0), f"UID: {self.uid}", font=font_10, fill=(255, 255, 255, 100))
             self.background.alpha_composite(uid,Ticket.position_uid)
     
-    async def creat_light_cone(self):
+    async def create_light_cone(self):
         if self.data.light_cone is None:
             self.light_cone_background = Image.new("RGBA", (447, 255), (0, 0, 0, 0))
             return 
         
-        maska = await _of.maska_light_cones
+        mask = await _of.maska_light_cones
         frame_light_cones = await _of.frame_light_cones
         blic_light_cones = await _of.blic_light_cones
         
-        light_cone_holst = Image.new(Ticket.RGBA, Ticket.lc_bacgrount_size, (0, 0, 0, 0))
-        light_cone_holst_image = Image.new(Ticket.RGBA, Ticket.lc_bacgrount_size, (0, 0, 0, 0))
+        light_cone_holst = Image.new(Ticket.RGBA, Ticket.lc_background_size, (0, 0, 0, 0))
+        light_cone_holst_image = Image.new(Ticket.RGBA, Ticket.lc_background_size, (0, 0, 0, 0))
 
-        image = await pill.get_dowload_img(self.data.light_cone.portrait, size=Ticket.lc_image_size)
+        image = await pill.get_download_img(self.data.light_cone.portrait, size=Ticket.lc_image_size)
         light_cone_holst_image.alpha_composite(image, Ticket.lc_image_position)
 
-        light_cone_holst.paste(light_cone_holst_image, (0, 0), maska.convert("L"))
+        light_cone_holst.paste(light_cone_holst_image, (0, 0), mask.convert("L"))
 
-        light_cone_holst_image = Image.new(Ticket.RGBA, Ticket.lc_bacgrount_size, (0, 0, 0, 0))
+        light_cone_holst_image = Image.new(Ticket.RGBA, Ticket.lc_background_size, (0, 0, 0, 0))
         
-        shadow, frame, self.color = await pill.get_resurs_light_cones(self.data.light_cone.rarity)
+        shadow, frame, self.color = await pill.get_resource_light_cones(self.data.light_cone.rarity)
         
         light_cone_holst_image.alpha_composite(shadow)
         light_cone_holst_image.alpha_composite(frame, Ticket.lc_frame_position)
         light_cone_holst_image.alpha_composite(light_cone_holst)
         light_cone_holst_image.alpha_composite(frame_light_cones)
         light_cone_holst_image.alpha_composite(blic_light_cones)
         light_cone_holst_image.alpha_composite(frame)
@@ -148,15 +145,15 @@
         self.light_cone_background.alpha_composite(line, (191, 19))
         self.light_cone_background.alpha_composite(name_light_cone, (200, 23))
         
         y = int(22 + line.size[1])
 
         self.light_cone_background.alpha_composite(background_stat, (188, y))
     
-    async def creat_relict(self,relict):
+    async def create_relict(self,relict):
         
         font_15 = await pill.get_font(15)
         font_26 = await pill.get_font(26)
         font_14 = await pill.get_font(14)
         font_17 = await pill.get_font(17)
         
         background = Image.new(Ticket.RGBA, (394,115), (0,0,0,0))
@@ -165,25 +162,25 @@
         relict_background = relict_background.copy()
         
         count = await _of.relict_count_lvl
         relict_maska = await _of.relict_maska
         relict_score_frame = await _of.relict_score_frame
         
         relict_background_icon = Image.new(Ticket.RGBA, (387,88), (0,0,0,0))
-        image = await pill.get_dowload_img(relict.icon, size= (108,108))
+        image = await pill.get_download_img(relict.icon, size= (108,108))
         relict_background_icon.alpha_composite(image,(-6,-10))
         
         line = Image.new(Ticket.RGBA, (1,81), (255,255,255,255))
         
         relict_background.paste(relict_background_icon,(0,0),relict_maska.convert("L"))
         relict_background.alpha_composite(line,(117,4))
         relict_background.alpha_composite(line,(251,4))
         
         score = self.score_info["score"].get(str(relict.id),_DEFAULT_SCORE)
-        main_stat_icon = await pill.get_dowload_img(relict.main_affix.icon, size= Ticket.relict_main_stat_icon_size)
+        main_stat_icon = await pill.get_download_img(relict.main_affix.icon, size= Ticket.relict_main_stat_icon_size)
         color = options.color_element.get(relict.main_affix.type, None)
         if not color is None:
             main_stat_icon = await pill.recolor_image(main_stat_icon, color[:3])
         
         stars = await options.get_stars(relict.rarity, type = 3)
         stars = stars.resize((25,82))
         
@@ -208,15 +205,15 @@
         p_roll_x = 222
         p_roll_y = 15
         
         eff = 0
         
         for i, k in enumerate(relict.sub_affix):
             count_draw  = count.copy()
-            icon = await pill.get_dowload_img(k.icon, size=Ticket.relict_sub_icon_size)
+            icon = await pill.get_download_img(k.icon, size=Ticket.relict_sub_icon_size)
             relict_background.alpha_composite(icon,(x_icon,y_icon))
             scoreR = score["rolls"].get(k.type,0)
             x = x_text - int(font_17.getlength(str(k.display)))
             
             if k.type in self.score_info["bad"]:
                 d.text((x, y_text), str(k.display), font=font_17, fill= (255,255,255,255))
             else:
@@ -254,57 +251,57 @@
         
         d.text((136, 1), "Rank:", font=font_14, fill = (255,255,255,255))
         d.text((178, 1), str(score["rank"]["name"]), font=font_14, fill = score["rank"]["color"])
         
         d.text((239, 1), "Eff Stat:", font=font_14, fill = (255,255,255,255))
         d.text((301, 1), str(eff), font=font_14, fill = options.color_scoreR.get(eff,(255,255,255,255)))
         
-        self.totall_eff += eff
+        self.total_eff += eff
                 
         return {"position": str(relict.id)[-1:] , "img": background}        
 
     
-    async def creat_relict_sets(self):
+    async def create_relict_sets(self):
         rel_set = options.calculator_relict_sets(self.data.relic_sets)
 
         self.background_sets = Image.new(Ticket.RGBA, Ticket.sets_background, (0,0,0,0))
         icons_sets = await _of.relict_icon_sets
         background_counts = await _of.relict_count_sets
-        font = await pill.get_font(Ticket.setst_font)
+        font = await pill.get_font(Ticket.sets_font)
         
         line_items = []
         i = 0
         for key in rel_set:
             sets = rel_set[key]
-            holst_line = Image.new(Ticket.RGBA, Ticket.setst_line_size, (0,0,0,0))
-            icon = await pill.get_dowload_img(sets["icon"], size = (33,33))
+            holst_line = Image.new(Ticket.RGBA, Ticket.sets_line_size, (0,0,0,0))
+            icon = await pill.get_download_img(sets["icon"], size = (33,33))
             icons_sets.alpha_composite(icon, (3,3))
             
             background_count = background_counts.copy()
             d = ImageDraw.Draw(background_count)
-            d.text(Ticket.setst_count_position, str(sets["num"]), font=font, fill= Ticket.setst_name_color)
+            d.text(Ticket.sets_count_position, str(sets["num"]), font=font, fill= Ticket.sets_name_color)
             
             d = ImageDraw.Draw(holst_line)
             sets_name_font,size = await pill.get_text_size_frame(sets["name"],15,280)
             if key[:1] == "1":
                 if i != 0:
                     holst_line.alpha_composite(icons_sets, (356,0))
                     holst_line.alpha_composite(background_count,(0,10))
-                    d.text((int(185-size/2), 12), sets["name"], font=sets_name_font, fill=Ticket.setst_name_color)
+                    d.text((int(185-size/2), 12), sets["name"], font=sets_name_font, fill=Ticket.sets_name_color)
                     line_items.append({"setap": i, "line": holst_line})
                 else:
                     holst_line.alpha_composite(icons_sets, (0,0))
                     holst_line.alpha_composite(background_count,(370,10))
-                    d.text((int(185-size/2), 12), sets["name"], font=sets_name_font, fill=Ticket.setst_name_color)
+                    d.text((int(185-size/2), 12), sets["name"], font=sets_name_font, fill=Ticket.sets_name_color)
                     line_items.append({"setap": i, "line": holst_line})
                 i += 1
             else:
                 holst_line.alpha_composite(icons_sets, (0,0))
                 holst_line.alpha_composite(background_count,(370,10))
-                d.text((int(185-size/2), 12), sets["name"], font=sets_name_font, fill=Ticket.setst_name_color)
+                d.text((int(185-size/2), 12), sets["name"], font=sets_name_font, fill=Ticket.sets_name_color)
                 line_items.append({"setap": 3, "line": holst_line})
         
         
         
         for key in line_items:
             if key["setap"] == 0:
                 self.background_sets.alpha_composite(key["line"],(0,0))
@@ -312,15 +309,15 @@
                 self.background_sets.alpha_composite(key["line"],(413,507))
             else:
                 self.background_sets.alpha_composite(key["line"],(0,45))
                 
     async def get_score(self):
         self.score_info = await stats.Calculator(self.data).start()
     
-    async def creat_stats(self):
+    async def create_stats(self):
         self.background_stats = Image.new(Ticket.RGBA, (434, 692), (0, 0, 0, 0))
 
         combined_attributes = {}
         dop = {}
         
         for attribute in self.data.attributes + self.data.additions:
             field = attribute.field
@@ -331,15 +328,15 @@
                 dop[field] = {"main": attribute.display, "dop": 0}
                 combined_attributes[field] = attribute
 
         dop = {key: value for key, value in dop.items() if value['dop'] != 0}
         
         result = []
                 
-        async for i, background in pill.creat_stats(combined_attributes, dop, 
+        async for i, background in pill.create_stats(combined_attributes, dop, 
                       Ticket.stat_font_dop,Ticket.stat_font,
                       Ticket.stat_line_size, Ticket.stat_name_size, Ticket.stat_max_width, Ticket.stat_icon_size,
                       Ticket.stat_icon_position, Ticket.stat_name_position, Ticket.stat_x_position,
                       self.element_color,Ticket.stat_value_font
                       ,Ticket.stat_y_no_dop,Ticket.stat_y_yes_dop,Ticket.stat_y_dop):
             result.append(background)
                 
@@ -348,15 +345,15 @@
         
         x = int(692 / (len(result)))
         position_line = 0
         for key in result:
             self.background_stats.alpha_composite(key, (0, position_line))
             position_line += x
                    
-    async def creat_path(self):
+    async def create_path(self):
         font = await pill.get_font(11)
         font_13 = await pill.get_font(13)
 
         self.main_bg =  Image.new("RGBA", (282,58), (0, 0, 0, 0))
         position_main = 0
 
         self.dop_bg = Image.new("RGBA", (399,124), (0, 0, 0, 0))
@@ -381,17 +378,17 @@
         )
         
         i = 0
         for key in self.data.skill_trees:
             if key.max_level == 1:
 
                 if key.anchor in ["Point05","Point06","Point07","Point08"]:
-                    icon = await pill.get_dowload_img(key.icon, size=(38,38))
+                    icon = await pill.get_download_img(key.icon, size=(38,38))
                 else:
-                    icon = await pill.get_dowload_img(key.icon, size=(30,30))
+                    icon = await pill.get_download_img(key.icon, size=(30,30))
                     
                 if key.level == 0:
                     if key.anchor in ["Point05","Point06","Point07","Point08"]:
                         bg = await _of.dop
                         bg = bg.copy()
                         bg.alpha_composite(icon,(7,10))
                         closed_main = await _of.closed_main
@@ -410,15 +407,15 @@
                         bg = await _of.open_trees
                         bg = await pill.recolor_image(bg.copy(), self.element_color[:3])
                         icon = await pill.recolor_image(icon, (0, 0, 0))
                         bg.alpha_composite(icon, (0,0))
                 self.dop_bg.alpha_composite(bg, position_dop[i])
                 i += 1
             else:
-                icon = await pill.get_dowload_img(key.icon, size=(43, 43))
+                icon = await pill.get_download_img(key.icon, size=(43, 43))
                 bg = await _of.bg_main
                 frame_bg = await _of.frame_main
                 bg = bg.copy()
                 frame_bg = await pill.recolor_image(frame_bg.copy(),self.element_color[:3])
                 bg.alpha_composite(frame_bg)
                 
                 count = await _of.count_tree
@@ -438,15 +435,15 @@
                 else:
                     draw.text((18-x,0), f"{key.level}/{key.max_level}", font=font_13, fill=(255, 255, 255, 255))
                 bg.alpha_composite(count,(4,44))
                 self.main_bg.alpha_composite(bg,(position_main,0))
                 position_main += 77
 
 
-    async def creat_name(self):
+    async def create_name(self):
         self.background_name = Image.new(Ticket.RGBA, Ticket.name_size, (0, 0, 0, 0))
         d = ImageDraw.Draw(self.background_name)
         names = await pill.create_image_with_text(self.data.name, Ticket.font_name_size , max_width=Ticket.name_with, color= Ticket.name_color)
         names_dark = await pill.recolor_image(names,(0,0,0))
         if names_dark.size[1] <= Ticket.name_h_max:
             self.background_name.alpha_composite(names_dark,(Ticket.name_position - 1,int(Ticket.name_h_max-names.size[1]/2)))
         else:
@@ -462,41 +459,41 @@
         max_level = options.max_lvl(self.data.promotion)
         level = f"{self.lang.lvl}: {self.data.level}/{max_level}"
         d.text((Ticket.position_name_level[0]-1, Ticket.position_name_level[1]), level, font=font_17, fill= (0,0,0,255))
         d.text(Ticket.position_name_level, level, font=font_17, fill= Ticket.color_name_level)
         starts = await options.get_stars(self.data.rarity)
         self.background_name.alpha_composite(starts,Ticket.position_name_star)   
     
-    async def creat_constant(self):
+    async def create_constant(self):
         self.background_skills = Image.new(Ticket.RGBA, (381, 54), (0, 0, 0, 0))
         x = 0
         rank = self.data.rank
         closed = await _of.CLOSED_const
         closed = closed.resize((54,54))
         closed = await pill.recolor_image(closed.copy(), self.element_color[:3])
         for key in self.data.rank_icons[:rank]:
             bg = await _of.ON_const
             bg = await pill.recolor_image(bg.resize((54,54)).copy(),self.element_color[:3])
-            icon = await pill.get_dowload_img(key, size=(43,43))
+            icon = await pill.get_download_img(key, size=(43,43))
             icon = await pill.recolor_image(icon, self.element_color[:3])
             bg.alpha_composite(icon,(5,5))
             self.background_skills.alpha_composite(bg,(x,0))
             x += 65
         for key in self.data.rank_icons[rank:]:
             bg = await _of.OFF_const
             bg = bg.resize((54,54)).copy()
-            icon = await pill.get_dowload_img(key, size=(43,43))
+            icon = await pill.get_download_img(key, size=(43,43))
             icon = await pill.apply_opacity(icon, 0.3)
             bg.alpha_composite(icon,(5,5))
             bg.alpha_composite(closed,(0,0))
             self.background_skills.alpha_composite(bg,(x,0))
             x += 65
    
     
-    async def creat_score_total(self):
+    async def create_score_total(self):
         self.background_score = Image.new("RGBA",(442,37), (0,0,0,0))
         
         sclor_bg = await _of.relict_backgroundl_score_line
         sclor_bg = sclor_bg.copy()
         sclor_bg_color = await _of.relict_full_score_line
         sclor_bg_color = sclor_bg_color.copy()
         sclor_bg_color = await pill.recolor_image(sclor_bg_color, self.element_color[:3])
@@ -526,15 +523,15 @@
         d.text((178, -2), "Score:", font=font_16, fill = (255,255,255,255))
         d.text((233, -2), str(self.score_info["total_score"]['count']), font=font_16, fill = self.score_info["total_score"]["rank"]["color"])
         
         d.text((0, -2), "Summary Rank:", font=font_16, fill = (255,255,255,255))
         d.text((132, -2), str(self.score_info["total_score"]["rank"]["name"]), font=font_16, fill = self.score_info["total_score"]["rank"]["color"])
         
         d.text((287, -2), "Eff Stat:", font=font_16, fill = (255,255,255,255))
-        d.text((366, -2), str(self.totall_eff), font=font_16, fill = options.color_scoreR.get(self.totall_eff,(255,255,255,255)))
+        d.text((366, -2), str(self.total_eff), font=font_16, fill = options.color_scoreR.get(self.total_eff,(255,255,255,255)))
     
     
     async def build_relict(self):
         self.background_relict = Image.new(Ticket.RGBA, (807,457), (0,0,0,0))
         none_relict = await _of.none_relict
         position = {
             "1": (0,0),
@@ -552,15 +549,15 @@
             map[key["position"]] = 0
         
         for key in map:
             if map[key] is None:
                 self.background_relict.alpha_composite(none_relict, position.get(key))
     
     
-    async def creat_seeleland(self):
+    async def create_seeleland(self):
         self.seelelen = Image.new("RGBA",(1,1), (0,0,0,0))
         
         if self.seeleland:
             self.seelelen = await _of.seeleland_v2
             self.seelelen = self.seelelen.copy()
             font = await pill.get_font(15)
             data = await options.get_seeleland(self.uid, self.data.id)
@@ -572,26 +569,26 @@
                 return None
             draw = ImageDraw.Draw(self.seelelen)
             draw.text((143, 7), str(data["sc"]), font=font, fill=(255, 255, 255, 255))
             draw.text((136, 24), f'{data["rank"][:-2]}..', font=font, fill=(255, 255, 255, 255))
             draw.text((127, 42), data["percrank"].replace("top ", ""), font=font, fill=(255, 255, 255, 255))
     
     async def build(self):
-        bg = Image.new(Ticket.RGBA, Ticket.bacground_size, (0,0,0,0))
+        bg = Image.new(Ticket.RGBA, Ticket.background_size, (0,0,0,0))
         
-        bg.alpha_composite(self.light_cone_background.resize((302,182)),(29,35))
-        bg.alpha_composite(self.background_relict,(29,310)) 
-        bg.alpha_composite(self.background_sets,(29,222))
-        bg.alpha_composite(self.background_stats,(884,56))
-        bg.alpha_composite(self.main_bg,(500,68))
-        bg.alpha_composite(self.dop_bg,(446,165))
-        bg.alpha_composite(self.background_skills,(455,327))
-        bg.alpha_composite(self.background_name,(1350,691))
-        bg.alpha_composite(self.background_score,(442,436))
-        bg.alpha_composite(self.seelelen,(1688,718)) 
+        bg.alpha_composite(self.light_cone_background.resize(Ticket.build_lc_size),Ticket.build_lc_position)
+        bg.alpha_composite(self.background_relict,Ticket.build_relict_position) 
+        bg.alpha_composite(self.background_sets,Ticket.build_sets_position)
+        bg.alpha_composite(self.background_stats,Ticket.build_stats_position)
+        bg.alpha_composite(self.main_bg,Ticket.build_skill_position_main)
+        bg.alpha_composite(self.dop_bg,Ticket.build_skill_position_dop)
+        bg.alpha_composite(self.background_skills,Ticket.build_constant_position)
+        bg.alpha_composite(self.background_name,Ticket.build_name_position)
+        bg.alpha_composite(self.background_score,Ticket.build_score_position)
+        bg.alpha_composite(self.seelelen,Ticket.build_seelelen_position) 
         
         if self.gif:
             self.background = []
             for key in self.GIFT_BG:
                 key.alpha_composite(bg)
                 self.background.append(key.convert("RGB"))
         else:
@@ -611,64 +608,64 @@
                     self.art = Image.open(f)
                     for frame in ImageSequence.Iterator(self.art):
                         self.element_color = await pill.get_colors(frame.convert("RGBA"), 15, common=True, radius=5, quality=800)
                         if frame_count >= 50:
                             break
                         if frame_count % n != 0:
                             self.art = frame.convert("RGBA")
-                            await self.creat_bacground()
+                            await self.create_background()
                             self.GIFT_BG.append(self.background.copy())
                         frame_count += 1
             else:
                 self.element_color = await pill.get_colors(self.art, 15, common=True, radius=5, quality=800)
-                await self.creat_bacground()
+                await self.create_background()
         else:
             self.element_color = (255,213,167,255)
-            await self.creat_bacground()
+            await self.create_background()
         
         async with anyio.create_task_group() as tasks:
-            tasks.start_soon(self.creat_light_cone)
-            tasks.start_soon(self.creat_stats)
-            tasks.start_soon(self.creat_name)
-            tasks.start_soon(self.creat_constant)
-            tasks.start_soon(self.creat_relict_sets)
+            tasks.start_soon(self.create_light_cone)
+            tasks.start_soon(self.create_stats)
+            tasks.start_soon(self.create_name)
+            tasks.start_soon(self.create_constant)
+            tasks.start_soon(self.create_relict_sets)
             tasks.start_soon(self.get_score)
-            tasks.start_soon(self.creat_path)
-            tasks.start_soon(self.creat_seeleland)
+            tasks.start_soon(self.create_path)
+            tasks.start_soon(self.create_seeleland)
         
         async def wait_all(*funcs):
             results = [None] * len(funcs)
             
             async with anyio.create_task_group() as tasks:
                 async def process(func, i):
                     results[i] = await func()
                 
                 for i, func in enumerate(funcs):
                     tasks.start_soon(process, func, i)
             
             return results
         
         self.relict = await wait_all(*[
-            functools.partial(self.creat_relict, key)
+            functools.partial(self.create_relict, key)
             for key in self.data.relics
         ])
 
 
             #self.relict = await asyncio.gather(*relic_tasks)
         
         
         
-        await self.creat_score_total()
+        await self.create_score_total()
         await self.build_relict()
         await self.build()
         
         data = {
                 "id": self.data.id,
                 "name": self.data.name,
                 "animation": self.gif,
                 "rarity": self.data.rarity,
                 "card": self.background,
-                "size": Ticket.bacground_size,
+                "size": Ticket.background_size,
                 "color": self.element_color,
             }
             
         return data
```

### Comparing `starrailcard-2.1.7/starrailcard/src/model/StarRailCard.py` & `starrailcard-2.1.8/starrailcard/src/model/StarRailCard.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,53 +11,33 @@
 except:
     pass
 
 import numpy as np
 
 from ..tools.ukrainization import TranslateDataManager
 from ..tools.http import AioSession
+from .api_mihomo import Player
 
 UA_LANG = False
 MAIN_LINK: Final[str] = "https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{icon}"
 
-class MemoryInfo(BaseModel):
-    level: Optional[int]
-    chaos_id: Optional[int]
-    chaos_level: Optional[int]
-    
-class SpaceInfo(BaseModel):
-    memory_data: Optional[MemoryInfo]
-    universe_level: Optional[int]
-    light_cone_count: Optional[int]
-    avatar_count: Optional[int]
-    achievement_count: Optional[int]
+
 
 class Avatar(BaseModel):
     id: str
     name: str
     icon: str
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         #self.icon = MAIN_LINK.format(icon = self.icon)
     
         if UA_LANG:
             self.name = TranslateDataManager._data.avatar.get(self.id, self.name)
 
-class Player(BaseModel):
-    uid: Optional[str]
-    nickname: Optional[str]
-    level: int
-    world_level: int
-    friend_count: int
-    avatar: Avatar
-    signature: Optional[str]
-    is_display: bool
-    space_info: Optional[SpaceInfo]
-
 class Card(BaseModel):
     id: int
     name: Optional[str]
     rarity: int
     card: Union[Image.Image,list]
     animation: bool
     size: Optional[tuple]
```

### Comparing `starrailcard-2.1.7/starrailcard/src/model/api_mihomo.py` & `starrailcard-2.1.8/starrailcard/src/model/api_mihomo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from typing import List, Optional,Final
 
 from ..tools.ukrainization import TranslateDataManager
 
 UA_LANG = False
 MAIN_LINK: Final[str] = "https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{icon}"
 
@@ -21,22 +21,33 @@
     
     return red, green, blue, alpha
 
 class MemoryInfo(BaseModel):
     level: Optional[int]
     chaos_id: Optional[int]
     chaos_level: Optional[int]
+    abyss_level: Optional[int] =  Field(0, alias= "abyssLevel")
+    abyss_star_count: Optional[int] =  Field(0, alias= "abyssStarCount")
+    
+    class Config:
+        populate_by_name = True
     
 class SpaceInfo(BaseModel):
+    relic_count: Optional[int] =  Field(0, alias= "relicCount")
+    music_count: Optional[int] =  Field(0, alias= "musicCount")
+    book_count: Optional[int] =  Field(0, alias= "bookCount")
     memory_data: Optional[MemoryInfo]
     universe_level: Optional[int]
     light_cone_count: Optional[int]
     avatar_count: Optional[int]
     achievement_count: Optional[int]
 
+    class Config:
+        populate_by_name = True
+        
 class Avatar(BaseModel):
     id: str
     name: str
     icon: str
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -308,15 +319,14 @@
     player: Player
     characters: List[Character]
     dont_update_link: Optional[bool] = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if not self.dont_update_link:
-            # Формирование новых ссылок на иконки
             self.player.avatar.icon = MAIN_LINK.format(icon = self.player.avatar.icon)
             for character in self.characters:
                 character.icon = MAIN_LINK.format(icon=character.icon)
                 character.preview = MAIN_LINK.format(icon=character.preview)
                 character.portrait = MAIN_LINK.format(icon=character.portrait)
                 character.rank_icons = [MAIN_LINK.format(icon=icon) for icon in character.rank_icons]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `starrailcard-2.1.7/starrailcard/src/model/utils_model.py` & `starrailcard-2.1.8/starrailcard/src/model/utils_model.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/rolls.json` & `starrailcard-2.1.8/starrailcard/src/tools/calculator/src/assets/rolls.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/score.json` & `starrailcard-2.1.8/starrailcard/src/tools/calculator/src/assets/score.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/calculator/src/utils.py` & `starrailcard-2.1.8/starrailcard/src/tools/calculator/src/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/calculator/stats.py` & `starrailcard-2.1.8/starrailcard/src/tools/calculator/stats.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/cashe.py` & `starrailcard-2.1.8/starrailcard/src/tools/cache.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/enums.py` & `starrailcard-2.1.8/starrailcard/src/tools/enums.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/git.py` & `starrailcard-2.1.8/starrailcard/src/tools/git.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from PIL import Image
 import os
 import threading
 from pathlib import Path
 from io import BytesIO
 
 from .http import AioSession
-from .cashe import Cache
+from .cache import Cache
 
 lock = threading.Lock()
 
 _caches = Cache.get_cache()
 
 assets = Path(__file__).parent.parent / 'assets'
 
@@ -82,14 +82,54 @@
     'light_cone_ups': 'teample_two_new/light_cone/ups.png',
     
     'LOGO_GIT': 'teample_two_new/LOGO.png',
     'LOGO_GIT_INV': 'three/LOGO.png',
     'seeleland_v2': "seeleland_v2.png"
 }
 
+
+card_style = {
+    'background_overlay': 'style_card/background/overlay.png',
+    'background_shadow': 'style_card/background/shadow.png',
+    'background_maska': 'style_card/background/maska.png',
+    'background_maska_art': 'style_card/background/maska_art.png',
+    
+    'shadow_3_light_cone': 'three/light_cones/3_shadow_lc.png',
+    'star_3_frame_light_cone': 'three/light_cones/3_star_frame_lc.png',
+    'shadow_4_light_cone': 'three/light_cones/4_shadow_lc.png',
+    'star_4_frame_light_cone': 'three/light_cones/4_star_frame_lc.png',
+    'shadow_5_light_cone': 'three/light_cones/5_shadow_lc.png',
+    'star_5_frame_light_cone': 'three/light_cones/5_star_frame_lc.png',
+    'blic_light_cones': 'three/light_cones/blic.png',
+    'frame_light_cones': 'three/light_cones/frame_lc.png',
+    'maska_light_cones': 'three/light_cones/maska_lc.png',
+    'stats_light_cones': 'three/light_cones/stats.png',
+    'none_relict': 'teample_two_new/relict/none_relict.png',
+    
+    'relict_backgroundl_score_line': 'teample_two_new/relict/backgroundl_score_line.png',
+    'relict_full_score_line': 'teample_two_new/relict/full_score_line.png',
+    'relict_count_sets': 'teample_two_new/relict/count_sets.png',
+    'relict_frame_line': 'teample_two_new/relict/frame_line.png',    
+    'relict_line': 'teample_two_new/relict/line.png',
+    'relict_frame': 'teample_two_new/relict/relict_frame.png',
+    'relict_maska': 'teample_two_new/relict/relict_maska.png',
+    'relict_score_frame': 'teample_two_new/relict/score_frame.png',
+    'none_relict': 'teample_two_new/relict/none_relict.png',
+    
+    'talants_adaptationt_frame': 'style_card/talants/adaptationt_frame.png',
+    'talants_background': 'style_card/talants/background.png',
+    'talants_count': 'style_card/talants/count.png',
+    'talants_default_frame': 'style_card/talants/default_frame.png',
+    'talants_line': 'style_card/talants/line.png',
+    'talants_mini_stats': 'style_card/talants/mini_stats.png',
+    'talants_main_stats': 'style_card/talants/main_stats.png',
+    
+    
+}
+
 relict_score = {
     'background_default': 'teample_two_new/background/background_default.png',
     'background_line': 'teample_two_new/background/line.png',
     'background_maska_art': 'teample_two_new/background/maska_art.png',
     'background_maska_blur': 'teample_two_new/background/maska_blur.png',
     'background_overlay': 'teample_two_new/background/overlay.png',
     'background_shadow': 'teample_two_new/background/shadow.png',
@@ -167,31 +207,35 @@
     "maska_prof_bg": 'profile_phone/maska_prof_bg.png',
     "menu": 'profile_phone/menu.png',
     "avatar_four": 'profile_phone/avatar_four.png',
     "avatar_five": 'profile_phone/avatar_five.png',
     'maska_character': 'profile_phone/maska_charter.png'
 }
 
+
+
 class ImageCache:
     
-    _assets_dowload = False
+    _assets_download = False
     _mapping = {}
             
     @classmethod
-    async def set_assets_dowload(cls, dowload = False):
-        cls._assets_dowload = dowload
+    async def set_assets_download(cls, download = False):
+        cls._assets_download = download
     
     @classmethod
     def set_mapping(cls,style):
         if style == 1:
             cls._mapping = relict_score
         elif style == 2:
             cls._mapping = ticket
         elif style == 3:
             cls._mapping = profile_phone
+        elif style == 4:
+            cls._mapping = card_style
         
     @classmethod
     async def _load_image(cls, name):
         
         try:
             image = _caches[name]
         except KeyError:
@@ -211,15 +255,15 @@
         if url in _caches:
             return _caches[name]
         else:
             image_data = await AioSession.get(url, response_format= "bytes")
             image = Image.open(BytesIO(image_data))
             _caches[name] = image
         
-        if cls._assets_dowload:
+        if cls._assets_download:
             file_path = assets / name
             file_path.parent.mkdir(parents=True, exist_ok=True)
             image.save(str(assets / name))
         
         return image
 
     async def __getattr__(cls, name):
```

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/http.py` & `starrailcard-2.1.8/starrailcard/src/tools/http.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/json_data.py` & `starrailcard-2.1.8/starrailcard/src/tools/json_data.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/options.py` & `starrailcard-2.1.8/starrailcard/src/tools/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,34 @@
     4: (255, 250, 141, 255),
     3: (252, 209, 124, 255),
     2: (234, 207, 153, 255),  # Было (184, 157, 103, 255)
     1: (220, 195, 148, 255),  # Было (170, 145, 98, 255)
     0: (255, 255, 255, 255)   # Было (255, 255, 255, 255)
 }
 
+color_element_stat = {
+    'physical_dmg': (255, 255, 255, 255),
+    'fire_dmg': (248, 79, 54, 255),
+    'ice_dmg': (71, 199, 253, 255),
+    'lightning_dmg': (136, 114, 241, 255),
+    'wind_dmg': (0, 255, 156, 255),
+    'quantum_dmg': (28, 41, 186, 255),
+    'imaginary_dmg': (244, 210, 88, 255),
+}
+
+color_element_talant = {
+    'physical': (255, 255, 255, 255),
+    'fire': (248, 79, 54, 255),
+    'ice': (71, 199, 253, 255),
+    'lightning': (136, 114, 241, 255),
+    'thunder': (136, 114, 241, 255),
+    'wind': (0, 255, 156, 255),
+    'quantum': (28, 41, 186, 255),
+    'imaginary': (244, 210, 88, 255),
+}
 
 color_element = {
     'PhysicalAddedRatio': (255, 255, 255, 255),
     'PhysicalResistance': (255, 255, 255, 255),
     'FireAddedRatio': (248, 79, 54, 255),
     'FireResistance': (248, 79, 54, 255),
     'IceAddedRatio': (71, 199, 253, 255),
@@ -85,15 +105,15 @@
     data = [value for value in data if value.isdigit()]
     
     if data == []:
         return None
     return data
 
 async def style_setting(style, settings):
-    if str(style) in ["1","2"]:
+    if str(style) in ["1","2","3"]:
         return style, settings
     
     return 1, {}
 
 
 def ups(x):
     if x == 5:
@@ -125,22 +145,35 @@
         max = 70
     else:
         max = 80
     
     return max
 
 
-async def get_character_art(character_art):
+
+async def get_character_art(character_art, style=None):
     processed_dict = {}
     for key, value in character_art.items():
         if isinstance(value, list):
-            processed_dict[key] = random.choice(value)
+            if isinstance(value[0], dict):
+                if style is not None:
+                    matching_art = [v['art'] for v in value if v['style'] == style]
+                    if matching_art:
+                        processed_dict[key] = random.choice(matching_art)
+                else:
+                    processed_dict[key] = random.choice([v['art'] for v in value])
+            else:
+                processed_dict[key] = random.choice(value)
+        elif isinstance(value, dict):
+            if 'style' in value and value['style'] == style:
+                processed_dict[key] = value['art']
         else:
             processed_dict[key] = value
 
+    
     return processed_dict
 
 async def get_stars(x, type = 1):
     if type == 1:
         if x == 5:
             return await _git.g_five
         elif x == 4:
@@ -210,30 +243,25 @@
     url = f"https://seeleland.azurewebsites.net/api/get_player_data?uid={uid}"
     data = await AioSession.get(url, response_format= "json")
     if data is None:
         return None
     for key in data:
         if key["k"] == str(charter_id):
             data = key.get("lb")
-    
-    if data != {} and data is not None:
-        if type(data) == list:
-            for key in data:
-                if "lb" in key:
-                    if "tutorial" in key["lb"]:
-                        return key["lb"]["tutorial"]
-                    else:
-                        '''for keys in key["lb"]:
-                            return key["lb"][keys]'''
-                        return None
-        else:
-            for key in data:
-                return data[key]
-    else:
+
+    if data == {} or data is None:
         return None
+    if type(data) == list:
+        for key in data:
+            if "lb" in key:
+                return key["lb"]["tutorial"] if "tutorial" in key["lb"] else None
+    else:
+        for key in data:
+            return data[key]
+
 
 async def save_card(uid, image_data, name):
     data = datetime.datetime.now().strftime("%d_%m_%Y %H_%M")
     path = os.getcwd()
     
     try:
         os.makedirs(f'{path}/RailCardImg/{uid}', exist_ok=True)
```

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/pill/color.py` & `starrailcard-2.1.8/starrailcard/src/tools/pill/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # All rights reserved.
 
 from PIL import Image,ImageFilter
 from more_itertools import chunked
 
 import numpy as np
 
-from .color_controle import light_level, _get_light_pixel_color, _get_dark_pixel_color
+from .color_control import light_level, get_light_pixel_color, _get_dark_pixel_color
 
 async def get_average_color(image):
     if image.mode != 'RGBA':
         image = image.convert('RGBA')
     
     channels = image.split()
     
@@ -121,13 +121,13 @@
             / 255
         ), 'L'))
     
     color_palette = await get_dominant_colors(filtered_image, number, common=common)
     color_palette = color_palette[0][1]
     ll = await light_level(color_palette)
     if ll < 0.15:
-        color_palette = await _get_light_pixel_color(color_palette)
+        color_palette = await get_light_pixel_color(color_palette)
     elif ll > 0.80:
         color_palette = await _get_dark_pixel_color(color_palette)
         
         
     return color_palette
```

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/pill/color_controle.py` & `starrailcard-2.1.8/starrailcard/src/tools/pill/color_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 import colorsys
-from .. import cashe 
+from .. import cache 
 
-_caches = cashe.Cache.get_cache()
+_caches = cache.Cache.get_cache()
 
 async def apply_opacity(image, opacity=0.2):
     result_image = image.copy()
     alpha = result_image.split()[3]
     alpha = alpha.point(lambda p: int(p * opacity))
     result_image.putalpha(alpha)
 
@@ -39,15 +39,15 @@
     return image
 
 
 async def recolor_image(image, target_color, light = False):
     if light:
         ll = await light_level(target_color)
         if ll < 45:
-            target_color = await _get_light_pixel_color(target_color,up = True)
+            target_color = await get_light_pixel_color(target_color,up = True)
     if image.mode != 'RGBA':
         image = image.convert('RGBA')
 
     image = image.copy()
 
     pixels = image.load()
     for i in range(image.width):
@@ -55,15 +55,15 @@
             r, g, b, a = pixels[i, j]
             if a != 0:
                 pixels[i, j] = target_color + (a,)
     if light:
         return image, target_color
     return image
 
-async def _get_light_pixel_color(pixel_color, up = False):
+async def get_light_pixel_color(pixel_color, up = False):
     h, l, s = colorsys.rgb_to_hls(*(x / 255 for x in pixel_color[:3]))
     if up:
         l = min(max(0.6, l), 0.9)
     else:
         l = min(max(0.3, l), 0.8)
     return tuple(round(x * 255) for x in colorsys.hls_to_rgb(h, l, s))
```

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/pill/diagrama.py` & `starrailcard-2.1.8/starrailcard/src/tools/pill/diagrama.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright 2023 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
+
 from PIL import Image
-from .. import pill
 import io
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import font_manager
 from pathlib import Path
 import warnings
-import random
+
 
 warnings.filterwarnings("ignore")
 
 assets = assets = Path(__file__).parent.parent.parent / 'assets'
 
 font_path = str(assets / 'font' / 'font_hsr.ttf')
 
@@ -46,15 +46,15 @@
     @staticmethod
     def _reorder_data_by_indices(lst):
         normalized_indices = [i % len(lst) for i in indices if i < len(lst)]
         return [lst[i] for i in normalized_indices]
 
     async def create_normalized_radial_chart(self):
 
-        rgb = self.rgb#pill.element_color_text.get(self.rgb, (149, 107, 5, 255))
+        rgb = self.rgb
         params = [item['name'] for item in self.data]
         values = [item['value'] for item in self.data]
 
         max_values = {item['name']: item['value'] for item in self.data_rect}
 
         num_vars = len(params)
         normalized_values = []
```

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/pill/grandiend_v2.py` & `starrailcard-2.1.8/starrailcard/src/tools/pill/gradient_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 
 from PIL import Image, ImageDraw, ImageChops
 import numpy as np
 import colorsys
 
-class GrandientBackground:
+class GradientBackground:
     def __init__(self, image, size, overlay = None, size_art = None):
         self.image = image
         self.overlay = overlay
         self.size_art = size_art
         self.width = size[0]
         self.height = size[1]
```

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/pill/grandient_v1.py` & `starrailcard-2.1.8/starrailcard/src/tools/pill/grandient_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 
 from PIL import Image
 
-from .color_controle import light_level, _get_light_pixel_color, _get_dark_pixel_color
+from .color_control import light_level, get_light_pixel_color, _get_dark_pixel_color
 
 class GradientGenerator:
     def __init__(self, source_img_path):
         self.source_img = source_img_path
         self.frame = ()
         self.source_width, self.source_height = self.source_img.size
 
@@ -28,30 +28,30 @@
         bottom_2 = top_height + center_height - 1
         top_3 = top_height + center_height + 1
         bottom_3 = height - 2
 
         top_color = await self._get_pixel_color(left, top_1, right, bottom_1)
         ll = await light_level(top_color)
         if ll < 45:
-            top_color = await _get_light_pixel_color(top_color)
+            top_color = await get_light_pixel_color(top_color)
         elif ll > 200:
             top_color = await _get_dark_pixel_color(top_color)
 
         center_color = await self._get_pixel_color(left, top_2, right, bottom_2)
         
         ll = await light_level(center_color)
         if ll < 45:
-            center_color = await _get_light_pixel_color(center_color)
+            center_color = await get_light_pixel_color(center_color)
         elif ll > 200:
             center_color = await _get_dark_pixel_color(center_color)
 
         bottom_color = await self._get_pixel_color(left, top_3, right, bottom_3)
         ll = await light_level(bottom_color)
         if ll < 45:
-            bottom_color = await _get_light_pixel_color(bottom_color)
+            bottom_color = await get_light_pixel_color(bottom_color)
         elif ll > 200:
             bottom_color = await _get_dark_pixel_color(bottom_color)
 
         for y in range(top_height):
             for x in range(width):
                 ratio = y / (top_height - 1)
                 gradient_color = self._get_interpolated_color(top_color, center_color, ratio)
```

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/pill/image_controle.py` & `starrailcard-2.1.8/starrailcard/src/tools/pill/image_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 import os
 import re
 import json
 
 from PIL import Image
 from io import BytesIO
 from ..git import assets
-from .. import cashe, http
+from .. import cache, http
 
-_caches = cashe.Cache.get_cache()
+_caches = cache.Cache.get_cache()
 _boost_speed = False
 
 
 async def resize_image(image, scale):
     width, height = image.size
     new_width = int(width * scale)
     new_height = int(height * scale)
     resized_image = image.resize((new_width, new_height))
     return resized_image
 
 
-async def get_centr_size(size, file_name): #get_centr_honkai_art
+async def get_center_size(size, file_name): #get_centr_honkai_art
     background_image = Image.new('RGBA', size, color=(0, 0, 0, 0))
     foreground_image = file_name.convert("RGBA")
 
     scale = max(size[0] / foreground_image.size[0], size[1] / foreground_image.size[1])
     foreground_image = foreground_image.resize((int(foreground_image.size[0] * scale), int(foreground_image.size[1] * scale)))
 
     background_size = background_image.size
@@ -41,15 +41,15 @@
         y = background_size[1] // 2 - foreground_size[1] // 2
 
     background_image.alpha_composite(foreground_image, (x, y))
 
     return background_image
 
 
-async def get_centr_scale(size, file_name):
+async def get_center_scale(size, file_name):
     
     background_image = Image.new('RGBA', size, color=(0, 0, 0, 0))
     foreground_image = file_name.convert("RGBA")
     
     scale = 0.65
     foreground_image = await resize_image(foreground_image, scale)
 
@@ -68,15 +68,15 @@
     path = f"/boost_speed/{link.split('master')[1]}"
     full_path = os.path.join(assets, path.lstrip('/'))
 
     if os.path.exists(full_path):
         try:
             return Image.open(full_path).convert("RGBA")
         except Exception as e:
-            raise IOError(f"Error reading image file: {e}")  # Прекращаем выполнение функции
+            raise IOError(f"Error reading image file: {e}")
     else:
         return None
 
 async def download_image(link, headers=None):
     try:
         image = await http.AioSession.get(link, headers=headers, response_format="bytes")
         return image
@@ -93,15 +93,15 @@
 
 async def open_image(image_data):
     try:
         return Image.open(BytesIO(image_data)).convert("RGBA")
     except Exception as e:
         raise TypeError(f"Error Open image: {e}")
 
-async def get_dowload_img(link, size=None, thumbnail_size=None, gif=False):
+async def get_download_img(link, size=None, thumbnail_size=None, gif=False):
     cache_key = json.dumps((link, size, thumbnail_size), sort_keys=True)
     image_boost = None
     
     if _boost_speed:
         if "StarRailRes" in link:
             image_boost = await get_image_from_boost_speed(link)
 
@@ -162,18 +162,18 @@
     if type(img) != str:
         img = img
     elif type(img) == str:
         linkImg = re.search("(?P<url>https?://[^\s]+)", img)
         if linkImg:
             try:
                 if "gif" in linkImg.group():
-                    img = await get_dowload_img(linkImg.group(), gif = True)
+                    img = await get_download_img(linkImg.group(), gif = True)
                     return img
                 else:
-                    img = await get_dowload_img(linkImg.group())
+                    img = await get_download_img(linkImg.group())
             except:
                 return None
         else:
             img = Image.open(img)
     else:
         return None
     return img.convert("RGBA")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/pill/style_editor.py` & `starrailcard-2.1.8/starrailcard/src/tools/pill/style_editor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 
 from PIL import Image,ImageDraw
 from .. import git, options, treePaths
-from .text_controle import get_font, create_image_with_text
-from .image_controle import get_dowload_img
-from .color_controle import  recolor_image, apply_opacity
+from .text_control import get_font, create_image_with_text
+from .image_control import get_download_img
+from .color_control import  recolor_image, apply_opacity
 
 
 
-async def creat_stats(combined_attributes, dop, 
+async def create_stats(combined_attributes, dop, 
                       font_dop,font,
                       line_size, name_size, max_width, icon_size,
                       icon_position, name_position, x_position,
                       color_font, stat_value_font,
-                      stat_y_no_dop = 13, stat_y_yes_dop = 6, stat_y_dop = 25):
+                      stat_y_no_dop = 13, stat_y_yes_dop = 6, stat_y_dop = 25, line = False):
     
     font = await get_font(font)
     font_dop = await get_font(font_dop)
     stat_value_font = await get_font(stat_value_font)
     
     for i, attribute in enumerate(combined_attributes):
         stat = combined_attributes[attribute]
-        icon = await get_dowload_img(stat.icon, size= icon_size)
+        icon = await get_download_img(stat.icon, size= icon_size)
+        if attribute in ["physical_dmg","fire_dmg","ice_dmg","lightning_dmg","wind_dmg","quantum_dmg", "imaginary_dmg"]:
+            icon = await recolor_image(icon.copy(), options.color_element_stat.get(attribute, (255,255,255,255))[:3])
         background = Image.new("RGBA", line_size, (0, 0, 0, 0))
         d = ImageDraw.Draw(background)
         value = "{:.1f}%".format(stat.value * 100) if stat.percent else round(stat.value)
         name_text = await create_image_with_text(stat.name, name_size, max_width=max_width, color=(255, 255, 255, 255)) #max_height=45,
         background.alpha_composite(name_text, (name_position[0],(int(name_position[1]-name_text.size[1]/2))))
-        background.alpha_composite(icon,icon_position)
-        
+        background.alpha_composite(icon,icon_position)        
         if attribute in dop: 
             x = x_position - int(stat_value_font.getlength(str(value)))
             d.text((x, stat_y_yes_dop), str(value), font=stat_value_font, fill=(255, 255, 255, 255))
 
             x = x_position - int(font_dop.getlength(dop[attribute]["dop"]))
             d.text((x, stat_y_dop), dop[attribute]["dop"], font=font_dop, fill= color_font)
 
             x = x - int(font_dop.getlength(dop[attribute]["main"])) - 5
             d.text((x, stat_y_dop), dop[attribute]["main"], font=font_dop, fill=(255, 255, 255, 255))
         else:
             x = x_position - int(stat_value_font.getlength(str(value)))
             d.text((x, stat_y_no_dop), str(value), font=stat_value_font, fill=(255, 255, 255, 255))
 
+        if line:
+            x = line_size[0] - (int(stat_value_font.getlength(str(value))) + name_position[0] + name_text.size[0] + 10 * 3)   
+            line_stat = Image.new("RGBA", (x,2), (255,255,255,50))
+            background.alpha_composite(line_stat,(name_text.size[0]+icon_size[0] + 15, int(line_size[1]/2)))
+            
+            
         yield i, background
         
 
-async def creat_path(character):
+async def create_path(character):
     background_path = await options.get_background_path(character.path.id)
     path = treePaths.map_new.get(character.path.id)
     font_15 = await get_font(15) 
     for key in character.skill_trees:
         if key.anchor in ['Point01','Point02','Point03','Point04','Point05']:
-            icon = await get_dowload_img(key.icon, size=(47,47))
+            icon = await get_download_img(key.icon, size=(47,47))
             icon = await recolor_image(icon, (255,212,173))
             count = await git.ImageCache().path_count
             count = count.copy()
             d = ImageDraw.Draw(count)
             if key.anchor == 'Point01':
                 if key.max_level > 6:
                     key.level += 1
@@ -65,25 +72,25 @@
                     key.level += 2
                 
             x = 29 - int(font_15.getlength(f"{key.level}/{key.max_level}")/2)
             d.text((x, 1), f"{key.level}/{key.max_level}", font=font_15, fill = (255,255,255,255))
             background_path.alpha_composite(icon, path[key.anchor]["icon"])
             background_path.alpha_composite(count, path[key.anchor]["count"])
         elif key.anchor in ['Point06','Point07','Point08']:
-            icon = await get_dowload_img(key.icon, size=(47,47))
+            icon = await get_download_img(key.icon, size=(47,47))
             icon = await recolor_image(icon, (0,0,0))
             if key.level == key.max_level:
                 background_path.alpha_composite(icon, path[key.anchor]["icon"])
             else:
                 icon = await apply_opacity(icon, opacity=0.5)
                 closed = await git.ImageCache().path_closed_main
                 background_path.alpha_composite(icon, path[key.anchor]["icon"])
                 background_path.alpha_composite(closed, path[key.anchor]["closed"])
         else:
-            icon = await get_dowload_img(key.icon, size=(35,35))
+            icon = await get_download_img(key.icon, size=(35,35))
             icon = await recolor_image(icon, (0,0,0))
             if key.level == key.max_level:
                 background_path.alpha_composite(icon, path[key.anchor]["icon"])
             else:
                 icon = await apply_opacity(icon, opacity=0.5)
                 closed = await git.ImageCache().path_closed_dop
                 background_path.alpha_composite(icon, path[key.anchor]["icon"])
@@ -91,15 +98,15 @@
                 
     return background_path
 
 
 _of = git.ImageCache()
 _of.set_mapping(2)
 
-async def get_resurs_light_cones(x):
+async def get_resource_light_cones(x):
     if x == 3:
         return await _of.shadow_3_light_cone, await _of.star_3_frame_light_cone, (150, 202, 255, 255)
     elif x == 4:
         return await _of.shadow_4_light_cone, await _of.star_4_frame_light_cone, (217, 150, 255, 255)
     else:
         return await _of.shadow_5_light_cone, await _of.star_5_frame_light_cone, (255, 199, 150, 255)
```

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/pill/text_controle.py` & `starrailcard-2.1.8/starrailcard/src/tools/pill/text_control.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 import json
 from PIL import ImageFont,Image,ImageDraw
-from .. import git, cashe
+from .. import cache, git
 
-_caches = cashe.Cache.get_cache()
+_caches = cache.Cache.get_cache()
 
 async def get_font(size):
     return ImageFont.truetype(git.font, size)
 
 async def get_text_size_frame(text,font_size,frame_width):    
     font = await get_font(font_size)
```

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/translator.py` & `starrailcard-2.1.8/starrailcard/src/tools/translator.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/src/tools/ukrainization.py` & `starrailcard-2.1.8/starrailcard/src/tools/ukrainization.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.7/starrailcard/utils.py` & `starrailcard-2.1.8/starrailcard/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 
 async def get_character(lang = "en"):
     url = f"https://hsr.yatta.top/{lang}/archive/avatar"
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as response:
             return await response.json()
 
-async def get_name(characrer_id = None, lang = "en"):
+async def get_name(character_id = None, lang = "en"):
     avatar_data = await get_character(lang)
     if avatar_data.get("response") != 200:
         print("An error occurred while receiving data")
         return 
     data = {}
     for key in avatar_data.get("data", {}).get("items", {}):
-        if not characrer_id is None:
-            if int(key) == int(characrer_id):
+        if not character_id is None:
+            if int(key) == int(character_id):
                 return {key: avatar_data["data"]["items"][key].get("name")}
         data[key] = avatar_data["data"]["items"][key].get("name")
 
     return data
 
 async def get_character_id(name = None, lang = "en"):
```

### Comparing `starrailcard-2.1.7/starrailcard.egg-info/PKG-INFO` & `starrailcard-2.1.8/starrailcard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.1.7
+Version: 2.1.8
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
-Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai
+Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai,genshin,build,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
```

### Comparing `starrailcard-2.1.7/starrailcard.egg-info/SOURCES.txt` & `starrailcard-2.1.8/starrailcard.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,24 @@
 starrailcard/src/data/avatar.json
 starrailcard/src/data/element.json
 starrailcard/src/data/keys.json
 starrailcard/src/data/paths.json
 starrailcard/src/data/relict_sets.json
 starrailcard/src/data/stats.json
 starrailcard/src/data/weapons.json
+starrailcard/src/generator/style_card.py
 starrailcard/src/generator/style_profile_phone.py
 starrailcard/src/generator/style_relict_score.py
 starrailcard/src/generator/style_ticket.py
 starrailcard/src/model/StarRailCard.py
 starrailcard/src/model/api_mihomo.py
 starrailcard/src/model/style.py
 starrailcard/src/model/ukrainization_model.py
 starrailcard/src/model/utils_model.py
-starrailcard/src/tools/cashe.py
+starrailcard/src/tools/cache.py
 starrailcard/src/tools/enums.py
 starrailcard/src/tools/git.py
 starrailcard/src/tools/http.py
 starrailcard/src/tools/json_data.py
 starrailcard/src/tools/options.py
 starrailcard/src/tools/translator.py
 starrailcard/src/tools/treePaths.py
@@ -44,14 +45,14 @@
 starrailcard/src/tools/calculator/src/utils.py
 starrailcard/src/tools/calculator/src/assets/max.json
 starrailcard/src/tools/calculator/src/assets/relic_id.json
 starrailcard/src/tools/calculator/src/assets/rolls.json
 starrailcard/src/tools/calculator/src/assets/score.json
 starrailcard/src/tools/pill/__init__.py
 starrailcard/src/tools/pill/color.py
-starrailcard/src/tools/pill/color_controle.py
+starrailcard/src/tools/pill/color_control.py
 starrailcard/src/tools/pill/diagrama.py
-starrailcard/src/tools/pill/grandiend_v2.py
+starrailcard/src/tools/pill/gradient_v2.py
 starrailcard/src/tools/pill/grandient_v1.py
-starrailcard/src/tools/pill/image_controle.py
+starrailcard/src/tools/pill/image_control.py
 starrailcard/src/tools/pill/style_editor.py
-starrailcard/src/tools/pill/text_controle.py
+starrailcard/src/tools/pill/text_control.py
```

