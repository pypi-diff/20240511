# Comparing `tmp/cyberdrop_dl-5.2.9.tar.gz` & `tmp/cyberdrop_dl-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop_dl-5.2.9.tar", max compression
+gzip compressed data, was "cyberdrop_dl-5.3.1.tar", max compression
```

## Comparing `cyberdrop_dl-5.2.9.tar` & `cyberdrop_dl-5.3.1.tar`

### file list

```diff
@@ -1,97 +1,98 @@
--rw-r--r--   0        0        0    35149 2024-03-19 04:36:14.613205 cyberdrop_dl-5.2.9/LICENSE
--rw-r--r--   0        0        0     2165 2024-03-19 04:36:14.613205 cyberdrop_dl-5.2.9/README.md
--rw-r--r--   0        0        0       21 2024-03-19 04:36:14.613205 cyberdrop_dl-5.2.9/cyberdrop_dl/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.613205 cyberdrop_dl-5.2.9/cyberdrop_dl/clients/__init__.py
--rw-r--r--   0        0        0     6505 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/clients/download_client.py
--rw-r--r--   0        0        0     1980 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/clients/errors.py
--rw-r--r--   0        0        0     7981 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/clients/scraper_client.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0        0        0    21037 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/downloader/downloader.py
--rw-r--r--   0        0        0     6064 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/main.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/managers/__init__.py
--rw-r--r--   0        0        0     2890 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/managers/args_manager.py
--rw-r--r--   0        0        0     1801 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/managers/cache_manager.py
--rw-r--r--   0        0        0     4975 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/managers/client_manager.py
--rw-r--r--   0        0        0    11192 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/managers/config_manager.py
--rw-r--r--   0        0        0     2241 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/managers/db_manager.py
--rw-r--r--   0        0        0     3913 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/managers/download_manager.py
--rw-r--r--   0        0        0     2151 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/managers/log_manager.py
--rw-r--r--   0        0        0     9122 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/managers/manager.py
--rw-r--r--   0        0        0     3150 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/managers/path_manager.py
--rw-r--r--   0        0        0     3138 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/managers/progress_manager.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/__init__.py
--rw-r--r--   0        0        0    10160 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawler.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/__init__.py
--rw-r--r--   0        0        0     8232 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/bunkrr_crawler.py
--rw-r--r--   0        0        0    11970 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/celebforum_crawler.py
--rw-r--r--   0        0        0     6801 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/coomer_crawler.py
--rw-r--r--   0        0        0     3080 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/cyberdrop_crawler.py
--rw-r--r--   0        0        0     7657 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/cyberfile_crawler.py
--rw-r--r--   0        0        0     4118 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/ehentai_crawler.py
--rw-r--r--   0        0        0     3401 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/erome_crawler.py
--rw-r--r--   0        0        0    12595 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/f95zone_crawler.py
--rw-r--r--   0        0        0     3303 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/fapello_crawler.py
--rw-r--r--   0        0        0     6066 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/gofile_crawler.py
--rw-r--r--   0        0        0     2630 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/hotpic_crawler.py
--rw-r--r--   0        0        0     5060 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/imageban_crawler.py
--rw-r--r--   0        0        0     4848 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/imgbb_crawler.py
--rw-r--r--   0        0        0     3024 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/imgbox_crawler.py
--rw-r--r--   0        0        0     4146 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/imgkiwi_crawler.py
--rw-r--r--   0        0        0     4598 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/imgur_crawler.py
--rw-r--r--   0        0        0     6824 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/jpgchurch_crawler.py
--rw-r--r--   0        0        0     7380 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/kemono_crawler.py
--rw-r--r--   0        0        0    12298 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/leakedmodels_crawler.py
--rw-r--r--   0        0        0     3345 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/mediafire_crawler.py
--rw-r--r--   0        0        0    12523 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/nudostar_crawler.py
--rw-r--r--   0        0        0     2522 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/nudostartv_crawler.py
--rw-r--r--   0        0        0     4861 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/omegascans_crawler.py
--rw-r--r--   0        0        0     3518 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/pimpandhost_crawler.py
--rw-r--r--   0        0        0     3479 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/pixeldrain_crawler.py
--rw-r--r--   0        0        0     2827 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/postimg_crawler.py
--rw-r--r--   0        0        0     7569 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/reddit_crawler.py
--rw-r--r--   0        0        0     3950 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/redgifs_crawler.py
--rw-r--r--   0        0        0     3952 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/rule34xxx_crawler.py
--rw-r--r--   0        0        0     4017 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/rule34xyz_crawler.py
--rw-r--r--   0        0        0     1865 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/saint_crawler.py
--rw-r--r--   0        0        0     4162 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/scrolller_crawler.py
--rw-r--r--   0        0        0    12755 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/simpcity_crawler.py
--rw-r--r--   0        0        0    13540 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/socialmediagirls_crawler.py
--rw-r--r--   0        0        0     4240 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/toonily_crawler.py
--rw-r--r--   0        0        0    13019 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/xbunker_crawler.py
--rw-r--r--   0        0        0     2142 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/xbunkr_crawler.py
--rw-r--r--   0        0        0     2513 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/jdownloader.py
--rw-r--r--   0        0        0    20105 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/scraper.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/progress/__init__.py
--rw-r--r--   0        0        0     3014 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/progress/downloads_progress.py
--rw-r--r--   0        0        0     6836 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/progress/file_progress.py
--rw-r--r--   0        0        0     4529 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/progress/scraping_progress.py
--rw-r--r--   0        0        0     3734 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/progress/statistic_progress.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/prompts/__init__.py
--rw-r--r--   0        0        0     5843 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/prompts/general_prompts.py
--rw-r--r--   0        0        0    12292 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/prompts/settings_authentication_prompts.py
--rw-r--r--   0        0        0     7561 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/prompts/settings_global_prompts.py
--rw-r--r--   0        0        0    18451 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/prompts/settings_user_prompts.py
--rw-r--r--   0        0        0      755 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/prompts/url_file_prompts.py
--rw-r--r--   0        0        0     5802 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/ui/ui.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/args/__init__.py
--rw-r--r--   0        0        0     6363 2024-03-19 04:36:14.617205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/args/args.py
--rw-r--r--   0        0        0     2659 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/args/browser_cookie_extraction.py
--rw-r--r--   0        0        0     4331 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/args/config_definitions.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/database/__init__.py
--rw-r--r--   0        0        0     1465 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/database/table_definitions.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/database/tables/__init__.py
--rw-r--r--   0        0        0     9205 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/database/tables/history_table.py
--rw-r--r--   0        0        0     1058 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/database/tables/temp_table.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/dataclasses/__init__.py
--rw-r--r--   0        0        0     2040 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/dataclasses/supported_domains.py
--rw-r--r--   0        0        0     1862 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/dataclasses/url_objects.py
--rw-r--r--   0        0        0     8251 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/sorting.py
--rw-r--r--   0        0        0        0 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/transfer/__init__.py
--rw-r--r--   0        0        0    12785 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/transfer/first_time_setup.py
--rw-r--r--   0        0        0     8301 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/transfer/transfer_v4_config.py
--rw-r--r--   0        0        0     1261 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/transfer/transfer_v4_db.py
--rw-r--r--   0        0        0    10003 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/cyberdrop_dl/utils/utilities.py
--rw-r--r--   0        0        0      963 2024-03-19 04:36:14.621205 cyberdrop_dl-5.2.9/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 cyberdrop_dl-5.2.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/LICENSE
+-rw-r--r--   0        0        0     2165 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/clients/__init__.py
+-rw-r--r--   0        0        0    14901 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/clients/download_client.py
+-rw-r--r--   0        0        0     2245 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/clients/errors.py
+-rw-r--r--   0        0        0     7981 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/clients/scraper_client.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0        0        0    12931 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/downloader/downloader.py
+-rw-r--r--   0        0        0     6672 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/main.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/managers/__init__.py
+-rw-r--r--   0        0        0     4525 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/managers/args_manager.py
+-rw-r--r--   0        0        0     1801 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/managers/cache_manager.py
+-rw-r--r--   0        0        0     5779 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/managers/client_manager.py
+-rw-r--r--   0        0        0    11962 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/managers/config_manager.py
+-rw-r--r--   0        0        0     2241 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/managers/db_manager.py
+-rw-r--r--   0        0        0     3913 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/managers/download_manager.py
+-rw-r--r--   0        0        0     3271 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/managers/log_manager.py
+-rw-r--r--   0        0        0     9122 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/managers/manager.py
+-rw-r--r--   0        0        0     4053 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/managers/path_manager.py
+-rw-r--r--   0        0        0     3138 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/managers/progress_manager.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/__init__.py
+-rw-r--r--   0        0        0    10160 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawler.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/__init__.py
+-rw-r--r--   0        0        0     8410 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/bunkrr_crawler.py
+-rw-r--r--   0        0        0    11970 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/celebforum_crawler.py
+-rw-r--r--   0        0        0     6863 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/coomer_crawler.py
+-rw-r--r--   0        0        0     3080 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/cyberdrop_crawler.py
+-rw-r--r--   0        0        0     7896 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/cyberfile_crawler.py
+-rw-r--r--   0        0        0     4118 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/ehentai_crawler.py
+-rw-r--r--   0        0        0     3401 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/erome_crawler.py
+-rw-r--r--   0        0        0    12595 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/f95zone_crawler.py
+-rw-r--r--   0        0        0     3303 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/fapello_crawler.py
+-rw-r--r--   0        0        0     6169 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/gofile_crawler.py
+-rw-r--r--   0        0        0     2630 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/hotpic_crawler.py
+-rw-r--r--   0        0        0     5060 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/imageban_crawler.py
+-rw-r--r--   0        0        0     4848 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/imgbb_crawler.py
+-rw-r--r--   0        0        0     3237 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/imgbox_crawler.py
+-rw-r--r--   0        0        0     4146 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/imgkiwi_crawler.py
+-rw-r--r--   0        0        0     4598 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/imgur_crawler.py
+-rw-r--r--   0        0        0     6824 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/jpgchurch_crawler.py
+-rw-r--r--   0        0        0     9145 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/kemono_crawler.py
+-rw-r--r--   0        0        0    12298 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/leakedmodels_crawler.py
+-rw-r--r--   0        0        0     3345 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/mediafire_crawler.py
+-rw-r--r--   0        0        0    12523 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/nudostar_crawler.py
+-rw-r--r--   0        0        0     2522 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/nudostartv_crawler.py
+-rw-r--r--   0        0        0     5464 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/omegascans_crawler.py
+-rw-r--r--   0        0        0     3518 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/pimpandhost_crawler.py
+-rw-r--r--   0        0        0     4261 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/pixeldrain_crawler.py
+-rw-r--r--   0        0        0     2827 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/postimg_crawler.py
+-rw-r--r--   0        0        0     3948 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/realbooru_crawler.py
+-rw-r--r--   0        0        0     7569 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/reddit_crawler.py
+-rw-r--r--   0        0        0     3886 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/redgifs_crawler.py
+-rw-r--r--   0        0        0     3952 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/rule34xxx_crawler.py
+-rw-r--r--   0        0        0     4017 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/rule34xyz_crawler.py
+-rw-r--r--   0        0        0     1865 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/saint_crawler.py
+-rw-r--r--   0        0        0     4162 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/scrolller_crawler.py
+-rw-r--r--   0        0        0    12759 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/simpcity_crawler.py
+-rw-r--r--   0        0        0    13535 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/socialmediagirls_crawler.py
+-rw-r--r--   0        0        0     4240 2024-05-10 23:31:44.332192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/toonily_crawler.py
+-rw-r--r--   0        0        0    13019 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/xbunker_crawler.py
+-rw-r--r--   0        0        0     2142 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/xbunkr_crawler.py
+-rw-r--r--   0        0        0     2513 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/jdownloader.py
+-rw-r--r--   0        0        0    20399 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/scraper.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/progress/__init__.py
+-rw-r--r--   0        0        0     3014 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/progress/downloads_progress.py
+-rw-r--r--   0        0        0     6836 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/progress/file_progress.py
+-rw-r--r--   0        0        0     4529 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/progress/scraping_progress.py
+-rw-r--r--   0        0        0     3734 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/progress/statistic_progress.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/prompts/__init__.py
+-rw-r--r--   0        0        0     5887 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/prompts/general_prompts.py
+-rw-r--r--   0        0        0    12292 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/prompts/settings_authentication_prompts.py
+-rw-r--r--   0        0        0     7561 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/prompts/settings_global_prompts.py
+-rw-r--r--   0        0        0    19039 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/prompts/settings_user_prompts.py
+-rw-r--r--   0        0        0      755 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/prompts/url_file_prompts.py
+-rw-r--r--   0        0        0     5996 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/ui/ui.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/args/__init__.py
+-rw-r--r--   0        0        0     7968 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/args/args.py
+-rw-r--r--   0        0        0     2659 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/args/browser_cookie_extraction.py
+-rw-r--r--   0        0        0     4403 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/args/config_definitions.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/database/__init__.py
+-rw-r--r--   0        0        0     1605 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/database/table_definitions.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/database/tables/__init__.py
+-rw-r--r--   0        0        0     9822 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/database/tables/history_table.py
+-rw-r--r--   0        0        0     1058 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/database/tables/temp_table.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/dataclasses/__init__.py
+-rw-r--r--   0        0        0     1852 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/dataclasses/supported_domains.py
+-rw-r--r--   0        0        0     1976 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/dataclasses/url_objects.py
+-rw-r--r--   0        0        0     8403 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/sorting.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/transfer/__init__.py
+-rw-r--r--   0        0        0    12785 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/transfer/first_time_setup.py
+-rw-r--r--   0        0        0     8301 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/transfer/transfer_v4_config.py
+-rw-r--r--   0        0        0     1261 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/transfer/transfer_v4_db.py
+-rw-r--r--   0        0        0    10428 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/cyberdrop_dl/utils/utilities.py
+-rw-r--r--   0        0        0      963 2024-05-10 23:31:44.336192 cyberdrop_dl-5.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 cyberdrop_dl-5.3.1/PKG-INFO
```

### Comparing `cyberdrop_dl-5.2.9/LICENSE` & `cyberdrop_dl-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/README.md` & `cyberdrop_dl-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/clients/errors.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/clients/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 class NoExtensionFailure(Exception):
     """This error will be thrown when no extension is given for a file"""
     def __init__(self, *, message: str = "Extension missing for file"):
         self.message = message
         super().__init__(self.message)
         
 
+class PasswordProtected(Exception):
+    """This error will be thrown when a file is password protected"""
+    def __init__(self, *, message: str = "File/Folder is password protected"):
+        self.message = message
+        super().__init__(self.message)
+        
+
 class DDOSGuardFailure(Exception):
     """This error will be thrown when DDoS-Guard is detected"""
 
     def __init__(self, status: int, message: str = "DDoS-Guard detected"):
         self.status = status
         self.message = message
         super().__init__(self.message)
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/clients/scraper_client.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/clients/scraper_client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/downloader/downloader.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/clients/download_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,395 +1,279 @@
 from __future__ import annotations
 
 import asyncio
 import copy
 import itertools
 import os
-import traceback
-from dataclasses import field, Field
-from functools import wraps
 from http import HTTPStatus
+from functools import wraps, partial
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Tuple
 
+import aiofiles
 import aiohttp
-import filedate
+from aiohttp import ClientSession
 
-from cyberdrop_dl.clients.download_client import is_4xx_client_error
 from cyberdrop_dl.clients.errors import DownloadFailure, InvalidContentTypeFailure
-from cyberdrop_dl.utils.utilities import CustomHTTPStatus, FILE_FORMATS, log
+from cyberdrop_dl.utils.utilities import FILE_FORMATS, log
 
 if TYPE_CHECKING:
-    from typing import Tuple
+    from typing import Callable, Coroutine, Any
 
-    from cyberdrop_dl.clients.download_client import DownloadClient
+    from cyberdrop_dl.managers.client_manager import ClientManager
     from cyberdrop_dl.managers.manager import Manager
     from cyberdrop_dl.utils.dataclasses.url_objects import MediaItem
 
 
-def retry(f):
-    """This function is a wrapper that handles retrying for failed downloads"""
-    @wraps(f)
+async def is_4xx_client_error(status_code: int) -> bool:
+    """Checks whether the HTTP status code is 4xx client error"""
+    if isinstance(status_code, str):
+        return True
+    return HTTPStatus.BAD_REQUEST <= status_code < HTTPStatus.INTERNAL_SERVER_ERROR
+
+
+def limiter(func):
+    """Wrapper handles limits for download session"""
+
+    @wraps(func)
     async def wrapper(self, *args, **kwargs):
-        while True:
-            try:
-                return await f(self, *args, **kwargs)
-            except DownloadFailure as e:
-                media_item = args[0]
-                if not isinstance(media_item.download_task_id, Field):
-                    await self.manager.progress_manager.file_progress.remove_file(media_item.download_task_id)
-
-                if e.status != 999:
-                    media_item.current_attempt += 1
-
-                if not self.manager.config_manager.settings_data['Download_Options']['disable_download_attempt_limit']:
-                    if media_item.current_attempt >= self.manager.config_manager.global_settings_data['Rate_Limiting_Options']['download_attempts']:
-                        if hasattr(e, "status"):
-                            await self.manager.progress_manager.download_stats_progress.add_failure(e.status)
-                            if hasattr(e, "message"):
-                                await log(f"Download Failed: {media_item.url} with status {e.status} and message {e.message}", 40)
-                                await self.manager.log_manager.write_download_error_log(media_item.url, f" {e.status} - {e.message}")
-                            else:
-                                await log(f"Download Failed: {media_item.url} with status {e.status}", 40)
-                                await self.manager.log_manager.write_download_error_log(media_item.url, f" {e.status}")
-                        else:
-                            await self.manager.progress_manager.download_stats_progress.add_failure("Unknown")
-                            await self.manager.log_manager.write_download_error_log(media_item.url, " See Log for Details")
-                            await log(f"Download Failed: {media_item.url} with error {e}", 40)
-                        await self.manager.progress_manager.download_progress.add_failed()
-                        break
-
-                if hasattr(e, "status"):
-                    if hasattr(e, "message"):
-                        await log(f"Download Failed: {media_item.url} with status {e.status} and message {e.message}", 40)
-                    else:
-                        await log(f"Download Failed: {media_item.url} with status {e.status}", 40)
-                else:
-                    await log(f"Download Failed: {media_item.url} with error {e}", 40)
-                await log(f"Download Retrying: {media_item.url} with attempt {media_item.current_attempt}", 20)
-            
-            except InvalidContentTypeFailure as e:
-                media_item = args[0]
-                if not isinstance(media_item.download_task_id, Field):
-                    await self.manager.progress_manager.file_progress.remove_file(media_item.download_task_id)
-                await log(f"Download Failed: {media_item.url} received Invalid Content", 40)
-                await log(e.message, 40)
-                await self.manager.progress_manager.download_stats_progress.add_failure("Invalid Content Type")
-                await self.manager.progress_manager.download_progress.add_failed()
-                break
-            
-            except Exception as e:
-                media_item = args[0]
-                await log(f"Download Failed: {media_item.url} with error {e}", 40)
-                if not isinstance(media_item.download_task_id, Field):
-                    await self.manager.progress_manager.file_progress.remove_file(media_item.download_task_id)
-                await log(traceback.format_exc(), 40)
-                await self.manager.progress_manager.download_stats_progress.add_failure("Unknown")
-                await self.manager.progress_manager.download_progress.add_failed()
-                break
+        domain_limiter = await self.client_manager.get_rate_limiter(args[0])
+        await asyncio.sleep(await self.client_manager.get_downloader_spacer(args[0]))
+        await self._global_limiter.acquire()
+        await domain_limiter.acquire()
+
+        async with aiohttp.ClientSession(headers=self._headers, raise_for_status=False,
+                                         cookie_jar=self.client_manager.cookies, timeout=self._timeouts,
+                                         trace_configs=self.trace_configs) as client:
+            kwargs['client_session'] = client
+            return await func(self, *args, **kwargs)
     return wrapper
 
 
-class Downloader:
-    def __init__(self, manager: Manager, domain: str):
-        self.manager: Manager = manager
-        self.domain: str = domain
-
-        self.client: DownloadClient = field(init=False)
-
-        self._file_lock = manager.download_manager.file_lock
-        self._semaphore: asyncio.Semaphore = field(init=False)
-
-        self._additional_headers = {}
-
-        self.processed_items: list = []
-        self.waiting_items = 0
-        self._current_attempt_filesize = {}
-
-    async def startup(self) -> None:
-        """Starts the downloader"""
-        self.client = self.manager.client_manager.downloader_session
-        await self.set_additional_headers()
-        self._semaphore = asyncio.Semaphore(await self.manager.download_manager.get_download_limit(self.domain))
-
-        self.manager.path_manager.download_dir.mkdir(parents=True, exist_ok=True)
-        if self.manager.config_manager.settings_data['Sorting']['sort_downloads']:
-            self.manager.path_manager.sorted_dir.mkdir(parents=True, exist_ok=True)
-
-    async def run(self, media_item: MediaItem) -> None:
-        """Runs the download loop"""
-        self.waiting_items += 1
-        media_item.current_attempt = 0
-
-        await self._semaphore.acquire()
-        self.waiting_items -= 1
-        if media_item.url.path not in self.processed_items:
-            self.processed_items.append(media_item.url.path)
-            await self.manager.progress_manager.download_progress.update_total()
-
-            await log(f"Download Starting: {media_item.url}", 20)
-            async with self.manager.client_manager.download_session_limit:
-                try:
-                    if isinstance(media_item.file_lock_reference_name, Field):
-                        media_item.file_lock_reference_name = media_item.filename
-                    await self._file_lock.check_lock(media_item.file_lock_reference_name)
-                    
-                    await self.download(media_item)
-                except Exception as e:
-                    await log(f"Download Failed: {media_item.url} with error {e}", 40)
-                    await log(traceback.format_exc(), 40)
-                    await self.manager.progress_manager.download_stats_progress.add_failure("Unknown")
-                    await self.manager.progress_manager.download_progress.add_failed()
-                else:
-                    await log(f"Download Finished: {media_item.url}", 20)
-                finally:
-                    await self._file_lock.release_lock(media_item.file_lock_reference_name)
-        self._semaphore.release()
+class DownloadClient:
+    """AIOHTTP operations for downloading"""
+    def __init__(self, manager: Manager, client_manager: ClientManager):
+        self.manager = manager
+        self.client_manager = client_manager
+        
+        self._headers = {"user-agent": client_manager.user_agent}
+        self._timeouts = aiohttp.ClientTimeout(total=client_manager.read_timeout + client_manager.connection_timeout,
+                                               connect=client_manager.connection_timeout)
+        self._global_limiter = self.client_manager.global_rate_limiter
+
+        self.trace_configs = []
+        if os.getenv("PYCHARM_HOSTED") is not None:
+            async def on_request_start(session, trace_config_ctx, params):
+                await log(f"Starting download {params.method} request to {params.url}", 40)
+
+            async def on_request_end(session, trace_config_ctx, params):
+                await log(f"Finishing download {params.method} request to {params.url}", 40)
+                await log(f"Response status for {params.url}: {params.response.status}", 40)
+
+            trace_config = aiohttp.TraceConfig()
+            trace_config.on_request_start.append(on_request_start)
+            trace_config.on_request_end.append(on_request_end)
+            self.trace_configs.append(trace_config)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
-    async def check_file_can_download(self, media_item: MediaItem) -> bool:
-        """Checks if the file can be downloaded"""
-        if not await self.manager.download_manager.check_free_space():
-            await log(f"Download Skip {media_item.url} due to insufficient free space", 10)
-            return False
-        if not await self.manager.download_manager.check_allowed_filetype(media_item):
-            await log(f"Download Skip {media_item.url} due to filetype restrictions", 10)
-            return False
-        if self.manager.config_manager.settings_data['Download_Options']['skip_download_mark_completed']:
-            await log(f"Download Skip {media_item.url} due to mark completed option", 10)
-            await self.mark_incomplete(media_item)
-            await self.mark_completed(media_item)
-            return False
-        return True
+    @limiter
+    async def _download(self, domain: str, manager: Manager, media_item: MediaItem,
+                        save_content: Callable[[aiohttp.StreamReader], Coroutine[Any, Any, None]], client_session: ClientSession) -> None:
+        """Downloads a file"""
+        headers = copy.deepcopy(self._headers)
+        headers['Referer'] = str(media_item.referer)
+        if domain == "pixeldrain":
+            if self.manager.config_manager.authentication_data['PixelDrain']['pixeldrain_api_key']:
+                headers["Authorization"] = await self.manager.download_manager.basic_auth("Cyberdrop-DL", self.manager.config_manager.authentication_data['PixelDrain']['pixeldrain_api_key'])
+        if isinstance(media_item.partial_file, Path):
+            resume_point = media_item.partial_file.stat().st_size if media_item.partial_file.exists() else 0
+            headers['Range'] = f'bytes={resume_point}-'
 
-    async def check_filesize_limits(self, media: MediaItem) -> bool:
-        """Checks if the file size is within the limits"""
-        max_video_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['maximum_video_size']
-        min_video_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['minimum_video_size']
-        max_image_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['maximum_image_size']
-        min_image_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['minimum_image_size']
-        max_other_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['maximum_other_size']
-        min_other_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['minimum_other_size']
+        await asyncio.sleep(self.client_manager.download_delay)
 
-        if media.ext in FILE_FORMATS['Images']:
-            if max_image_filesize and min_image_filesize:
-                if media.filesize < min_image_filesize or media.filesize > max_image_filesize:
-                    return False
-            if media.filesize < min_image_filesize:
-                return False
-            if max_image_filesize and media.filesize > max_image_filesize:
-                return False
-        elif media.ext in FILE_FORMATS['Videos']:
-            if max_video_filesize and min_video_filesize:
-                if media.filesize < min_video_filesize or media.filesize > max_video_filesize:
-                    return False
-            if media.filesize < min_video_filesize:
-                return False
-            if max_video_filesize and media.filesize > max_video_filesize:
-                return False
-        else:
-            if max_other_filesize and min_other_filesize:
-                if media.filesize < min_other_filesize or media.filesize > max_other_filesize:
-                    return False
-            if media.filesize < min_other_filesize:
-                return False
-            if max_other_filesize and media.filesize > max_other_filesize:
-                return False
-        return True
+        async with client_session.get(media_item.url, headers=headers, ssl=self.client_manager.ssl_context,
+                                      proxy=self.client_manager.proxy) as resp:
+            if resp.status == HTTPStatus.REQUESTED_RANGE_NOT_SATISFIABLE:
+                media_item.partial_file.unlink()
+                
+            await self.client_manager.check_http_status(resp, download=True)
+            content_type = resp.headers.get('Content-Type')
+            
+            if not isinstance(media_item.filesize, int):
+                media_item.filesize = int(resp.headers.get('Content-Length', '0'))
+            if not isinstance(media_item.partial_file, Path):
+                proceed, skip = await self.get_final_file_info(media_item, domain)
+                await self.mark_incomplete(media_item, domain)
+                if not proceed:
+                    await log(f"Skipping {media_item.url} as it has already been downloaded", 10)
+                    await self.manager.progress_manager.download_progress.add_previously_completed(False)
+                    await self.mark_completed(media_item, domain)
+                    return
+                if skip:
+                    await self.manager.progress_manager.download_progress.add_skipped()
+                    return
+            
+            ext = Path(media_item.filename).suffix.lower()
+            if content_type and any(s in content_type.lower() for s in ('html', 'text')) and ext not in FILE_FORMATS['Text']:
+                raise InvalidContentTypeFailure(message=f"Received {content_type}, was expecting other")
+
+            if resp.status != HTTPStatus.PARTIAL_CONTENT and media_item.partial_file.is_file():
+                media_item.partial_file.unlink()
+                
+            media_item.task_id = await self.manager.progress_manager.file_progress.add_task(f"({domain.upper()}) {media_item.filename}", media_item.filesize)
+            if media_item.partial_file.is_file():
+                resume_point = media_item.partial_file.stat().st_size
+                await self.manager.progress_manager.file_progress.advance_file(media_item.task_id, resume_point)
+
+            await save_content(resp.content)
+
+    async def _append_content(self, media_item, content: aiohttp.StreamReader, update_progress: partial) -> None:
+        """Appends content to a file"""
+        if not await self.client_manager.manager.download_manager.check_free_space():
+            raise DownloadFailure(status="No Free Space", message="Not enough free space")
+
+        media_item.partial_file.parent.mkdir(parents=True, exist_ok=True)
+        if not media_item.partial_file.is_file():
+            media_item.partial_file.touch()
+        async with aiofiles.open(media_item.partial_file, mode='ab') as f:
+            async for chunk, _ in content.iter_chunks():
+                await asyncio.sleep(0)
+                await f.write(chunk)
+                await update_progress(len(chunk))
+
+    async def download_file(self, manager: Manager, domain: str, media_item: MediaItem) -> None:
+        """Starts a file"""
+        async def save_content(content: aiohttp.StreamReader) -> None:
+            await self._append_content(media_item, content, partial(manager.progress_manager.file_progress.advance_file, media_item.task_id))
+
+        await self._download(domain, manager, media_item, save_content)
+        media_item.partial_file.rename(media_item.complete_file)
+        await self.mark_completed(media_item, domain)
+        
+    """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
+    
+    async def mark_incomplete(self, media_item: MediaItem, domain: str) -> None:
+        """Marks the media item as incomplete in the database"""
+        await self.manager.db_manager.history_table.insert_incompleted(domain, media_item)
 
+    async def mark_completed(self, media_item: MediaItem, domain: str) -> None:
+        """Marks the media item as completed in the database"""
+        await self.manager.db_manager.history_table.mark_complete(domain, media_item)
+    
+    """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
+    
     async def get_download_dir(self, media_item: MediaItem) -> Path:
         """Returns the download directory for the media item"""
         download_folder = media_item.download_folder
         if self.manager.args_manager.retry:
             return download_folder
 
         if self.manager.config_manager.settings_data['Download_Options']['block_download_sub_folders']:
             while download_folder.parent != self.manager.path_manager.download_dir:
                 download_folder = download_folder.parent
             media_item.download_folder = download_folder
         return download_folder
-
-    async def mark_incomplete(self, media_item: MediaItem) -> None:
-        """Marks the media item as incomplete in the database"""
-        await self.manager.db_manager.history_table.insert_incompleted(self.domain, media_item)
-
-    async def mark_completed(self, media_item: MediaItem) -> None:
-        """Marks the media item as completed in the database"""
-        await self.manager.db_manager.history_table.mark_complete(self.domain, media_item)
-
-    async def set_additional_headers(self) -> None:
-        """Sets additional headers for the download session"""
-        if self.domain == "pixeldrain":
-            if self.manager.config_manager.authentication_data['PixelDrain']['pixeldrain_api_key']:
-                self._additional_headers["Authorization"] = await self.manager.download_manager.basic_auth("Cyberdrop-DL", self.manager.config_manager.authentication_data['PixelDrain']['pixeldrain_api_key'])
-
-    async def get_final_file_info(self, complete_file: Path, partial_file: Path,
-                                  media_item: MediaItem) -> tuple[Path, Path, bool, bool]:
+    
+    async def get_final_file_info(self, media_item: MediaItem, domain: str) -> tuple[bool, bool]:
         """Complicated checker for if a file already exists, and was already downloaded"""
+        download_dir = await self.get_download_dir(media_item)
+        media_item.complete_file = download_dir / media_item.filename
+        media_item.partial_file = media_item.complete_file.with_suffix(media_item.complete_file.suffix + '.part')
+        
         expected_size = media_item.filesize if isinstance(media_item.filesize, int) else None
         proceed = True
         skip = False
         while True:
-            if not expected_size:
-                media_item.filesize = await self.client.get_filesize(media_item, self._additional_headers)
+            if expected_size:
                 file_size_check = await self.check_filesize_limits(media_item)
                 if not file_size_check:
+                    await log(f"Download Skip {media_item.url} due to filesize restrictions", 10)
                     proceed = False
                     skip = True
-                    return complete_file, partial_file, proceed, skip
+                    return proceed, skip
 
-            if not complete_file.exists() and not partial_file.exists():
+            if not media_item.complete_file.exists() and not media_item.partial_file.exists():
                 break
 
-            if complete_file.exists() and complete_file.stat().st_size == media_item.filesize:
+            if media_item.complete_file.exists() and media_item.complete_file.stat().st_size == media_item.filesize:
                 proceed = False
                 break
 
-            downloaded_filename = await self.manager.db_manager.history_table.get_downloaded_filename(self.domain, media_item)
+            downloaded_filename = await self.manager.db_manager.history_table.get_downloaded_filename(domain, media_item)
             if not downloaded_filename:
-                complete_file, partial_file = await self.iterate_filename(complete_file, media_item)
+                media_item.complete_file, media_item.partial_file = await self.iterate_filename(media_item.complete_file, media_item)
                 break
 
             if media_item.filename == downloaded_filename:
-                if partial_file.exists():
-                    if partial_file.stat().st_size >= media_item.filesize != 0:
-                        partial_file.unlink()
-                    if partial_file.stat().st_size == media_item.filesize:
-                        if complete_file.exists():
-                            new_complete_filename, new_partial_file = await self.iterate_filename(complete_file, media_item)
-                            partial_file.rename(new_complete_filename)
+                if media_item.partial_file.exists():
+                    if media_item.partial_file.stat().st_size >= media_item.filesize != 0:
+                        media_item.partial_file.unlink()
+                    if media_item.partial_file.stat().st_size == media_item.filesize:
+                        if media_item.complete_file.exists():
+                            new_complete_filename, new_partial_file = await self.iterate_filename(media_item.complete_file, media_item)
+                            media_item.partial_file.rename(new_complete_filename)
                             proceed = False
 
-                            complete_file = new_complete_filename
-                            partial_file = new_partial_file
+                            media_item.complete_file = new_complete_filename
+                            media_item.partial_file = new_partial_file
                         else:
                             proceed = False
-                            partial_file.rename(complete_file)
-                elif complete_file.exists():
-                    if complete_file.stat().st_size == media_item.filesize:
+                            media_item.partial_file.rename(media_item.complete_file)
+                elif media_item.complete_file.exists():
+                    if media_item.complete_file.stat().st_size == media_item.filesize:
                         proceed = False
                     else:
-                        complete_file, partial_file = await self.iterate_filename(complete_file, media_item)
+                        media_item.complete_file, media_item.partial_file = await self.iterate_filename(media_item.complete_file, media_item)
                 break
 
             media_item.filename = downloaded_filename
-            complete_file = media_item.download_folder / media_item.filename
-            partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
-
-        media_item.download_filename = complete_file.name
-        return complete_file, partial_file, proceed, skip
+        media_item.download_filename = media_item.complete_file.name
+        return proceed, skip
 
     async def iterate_filename(self, complete_file: Path, media_item: MediaItem) -> Tuple[Path, Path]:
         """Iterates the filename until it is unique"""
         partial_file = None
         for iteration in itertools.count(1):
             filename = f"{complete_file.stem} ({iteration}){media_item.ext}"
             temp_complete_file = media_item.download_folder / filename
             if not temp_complete_file.exists() and not await self.manager.db_manager.history_table.check_filename_exists(filename):
                 media_item.filename = filename
                 complete_file = media_item.download_folder / media_item.filename
                 partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
                 break
         return complete_file, partial_file
+    
+    async def check_filesize_limits(self, media: MediaItem) -> bool:
+        """Checks if the file size is within the limits"""
+        max_video_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['maximum_video_size']
+        min_video_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['minimum_video_size']
+        max_image_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['maximum_image_size']
+        min_image_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['minimum_image_size']
+        max_other_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['maximum_other_size']
+        min_other_filesize = self.manager.config_manager.settings_data['File_Size_Limits']['minimum_other_size']
 
-    async def set_file_datetime(self, media_item: MediaItem, complete_file: Path) -> None:
-        """Sets the file's datetime"""
-        if self.manager.config_manager.settings_data['Download_Options']['disable_file_timestamps']:
-            return
-        if not isinstance(media_item.datetime, Field):
-            file = filedate.File(str(complete_file))
-            file.set(
-                created=media_item.datetime,
-                modified=media_item.datetime,
-                accessed=media_item.datetime,
-            )
-
-    """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
-
-    @retry
-    async def download(self, media_item: MediaItem) -> None:
-        """Downloads the media item"""
-        if not await self.check_file_can_download(media_item):
-            await self.manager.progress_manager.download_progress.add_skipped()
-            return
-
-        download_dir = await self.get_download_dir(media_item)
-
-        partial_file = None
-        complete_file = None
-
-        try:
-            if not isinstance(media_item.current_attempt, int):
-                media_item.current_attempt = 1
-
-            complete_file = download_dir / media_item.filename
-            partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
-
-            complete_file, partial_file, proceed, skip_by_config = await self.get_final_file_info(complete_file, partial_file, media_item)
-            await self.mark_incomplete(media_item)
-
-            if skip_by_config:
-                await self.manager.progress_manager.download_progress.add_skipped()
-                return
-
-            if not proceed:
-                await log(f"Skipping {media_item.url} as it has already been downloaded", 10)
-                await self.manager.progress_manager.download_progress.add_previously_completed(False)
-                await self.mark_completed(media_item)
-                return
-
-            resume_point = partial_file.stat().st_size if partial_file.exists() else 0
-            headers = copy.deepcopy(self._additional_headers)
-            headers['Range'] = f'bytes={resume_point}-'
-
-            media_item.download_task_id = await self.manager.progress_manager.file_progress.add_task(media_item.filename, media_item.filesize)
-            await self.manager.progress_manager.file_progress.advance_file(media_item.download_task_id, resume_point)
-
-            await self.client.download_file(self.manager, self.domain, media_item, partial_file, headers, media_item.download_task_id)
-
-            try:
-                partial_file.rename(complete_file)
-            except FileExistsError:
-                complete_file, _partial_file = await self.iterate_filename(complete_file, media_item)
-                partial_file.rename(complete_file)
-            
-            os.chmod(complete_file, 0o666)
-            
-            await self.set_file_datetime(media_item, complete_file)
-
-            await self.mark_completed(media_item)
-            await self.manager.progress_manager.file_progress.mark_task_completed(media_item.download_task_id)
-            await self.manager.progress_manager.download_progress.add_completed()
-            return
-
-        except (aiohttp.ClientPayloadError, aiohttp.ClientOSError, aiohttp.ClientResponseError, ConnectionResetError,
-                DownloadFailure, FileNotFoundError, PermissionError, aiohttp.ServerDisconnectedError, 
-                asyncio.TimeoutError, aiohttp.ServerTimeoutError) as e:
-            if hasattr(e, "status"):
-                if ((await is_4xx_client_error(e.status) and e.status != HTTPStatus.TOO_MANY_REQUESTS)
-                        or e.status == HTTPStatus.SERVICE_UNAVAILABLE
-                        or e.status == HTTPStatus.BAD_GATEWAY
-                        or e.status == CustomHTTPStatus.WEB_SERVER_IS_DOWN):
-                    await self.manager.progress_manager.download_progress.add_failed()
-                    await self.manager.progress_manager.download_stats_progress.add_failure(e.status)
-                    if not isinstance(media_item.download_task_id, Field):
-                        await self.manager.progress_manager.file_progress.remove_file(media_item.download_task_id)
-                    if hasattr(e, "message"):
-                        if not e.message:
-                            e.message = "Download Failed"
-                        await log(f"Download failed: {media_item.url} with status {e.status} and message {e.message}", 40)
-                        await self.manager.log_manager.write_download_error_log(media_item.url, f" {e.status} - {e.message}")
-                    else:
-                        await log(f"Download Failed: {media_item.url} with status {e.status}", 40)
-                        await self.manager.log_manager.write_download_error_log(media_item.url, f" {e.status}")
-                    return
-
-            if partial_file and partial_file.is_file():
-                size = partial_file.stat().st_size
-                if media_item.filename in self._current_attempt_filesize and self._current_attempt_filesize[media_item.filename] >= size:
-                    raise DownloadFailure(status=getattr(e, "status", type(e).__name__), message="Download failed")
-                self._current_attempt_filesize[media_item.filename] = size
-                media_item.current_attempt = 0
-                raise DownloadFailure(status=999, message="Download timeout reached, retrying")
-
-            raise DownloadFailure(status=getattr(e, "status", type(e).__name__), message=repr(e))
+        if media.ext in FILE_FORMATS['Images']:
+            if max_image_filesize and min_image_filesize:
+                if media.filesize < min_image_filesize or media.filesize > max_image_filesize:
+                    return False
+            if media.filesize < min_image_filesize:
+                return False
+            if max_image_filesize and media.filesize > max_image_filesize:
+                return False
+        elif media.ext in FILE_FORMATS['Videos']:
+            if max_video_filesize and min_video_filesize:
+                if media.filesize < min_video_filesize or media.filesize > max_video_filesize:
+                    return False
+            if media.filesize < min_video_filesize:
+                return False
+            if max_video_filesize and media.filesize > max_video_filesize:
+                return False
+        else:
+            if max_other_filesize and min_other_filesize:
+                if media.filesize < min_other_filesize or media.filesize > max_other_filesize:
+                    return False
+            if media.filesize < min_other_filesize:
+                return False
+            if max_other_filesize and media.filesize > max_other_filesize:
+                return False
+        return True
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/main.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,17 +65,17 @@
         else:
             file_handler_debug = logging.FileHandler("./cyberdrop_dl_debug.log", mode="w")
         file_handler_debug.setLevel(manager.config_manager.settings_data['Runtime_Options']['log_level'])
         formatter = logging.Formatter("%(levelname)-8s : %(asctime)s : %(filename)s:%(lineno)d : %(message)s")
         file_handler_debug.setFormatter(formatter)
         logger_debug.addHandler(file_handler_debug)
 
-        aiosqlite_log = logging.getLogger("aiosqlite")
-        aiosqlite_log.setLevel(manager.config_manager.settings_data['Runtime_Options']['log_level'])
-        aiosqlite_log.addHandler(file_handler_debug)
+        # aiosqlite_log = logging.getLogger("aiosqlite")
+        # aiosqlite_log.setLevel(manager.config_manager.settings_data['Runtime_Options']['log_level'])
+        # aiosqlite_log.addHandler(file_handler_debug)
 
     while True:
         logger = logging.getLogger("cyberdrop_dl")
         if manager.args_manager.all_configs:
             if len(logger.handlers) > 0:
                 await log("Picking new config...", 20)
 
@@ -99,35 +99,44 @@
         file_handler.setFormatter(formatter)
         logger.addHandler(file_handler)
 
         await log("Starting Async Processes...", 20)
         await manager.async_startup()
 
         await log("Starting UI...", 20)
-        try:
-            if not manager.args_manager.no_ui:
-                with Live(manager.progress_manager.layout, refresh_per_second=10):
+        if not manager.args_manager.sort_all_configs:
+            try:
+                if not manager.args_manager.no_ui:
+                    with Live(manager.progress_manager.layout, refresh_per_second=manager.config_manager.settings_data['Runtime_Options']['ui_refresh_rate']):
+                        await runtime(manager)
+                else:
                     await runtime(manager)
-            else:
-                await runtime(manager)
-        except Exception as e:
-            print("\nAn error occurred, please report this to the developer")
-            print(e)
-            print(traceback.format_exc())
-            exit(1)
+            except Exception as e:
+                print("\nAn error occurred, please report this to the developer")
+                print(e)
+                print(traceback.format_exc())
+                exit(1)
 
         clear_screen_proc = await asyncio.create_subprocess_shell('cls' if os.name == 'nt' else 'clear')
         await clear_screen_proc.wait()
 
         await log("Running Post-Download Processes...", 20)
-        if manager.config_manager.settings_data['Sorting']['sort_downloads'] and not manager.args_manager.retry:
+        if isinstance(manager.args_manager.sort_downloads, bool):
+            if manager.args_manager.sort_downloads:
+                sorter = Sorter(manager)
+                await sorter.sort()
+        elif manager.config_manager.settings_data['Sorting']['sort_downloads'] and not manager.args_manager.retry:
             sorter = Sorter(manager)
             await sorter.sort()
         await check_partials_and_empty_folders(manager)
-
+        
+        if manager.config_manager.settings_data['Runtime_Options']['update_last_forum_post']:
+            await log("Updating Last Forum Post...", 20)
+            await manager.log_manager.update_last_forum_post()
+            
         await log("Printing Stats...", 20)
         await manager.progress_manager.print_stats()
 
         await log("Checking for Program End...", 20)
         if not manager.args_manager.all_configs or not list(set(configs) - set(configs_ran)):
             break
         await asyncio.sleep(5)
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/managers/cache_manager.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/managers/cache_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/managers/client_manager.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/managers/client_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import asyncio
 import ssl
 from http import HTTPStatus
 from typing import TYPE_CHECKING
 
 import aiohttp
 import certifi
-from aiohttp import ClientResponse
+from aiohttp import ClientResponse, ContentTypeError
 from aiolimiter import AsyncLimiter
 
 from cyberdrop_dl.clients.download_client import DownloadClient
-from cyberdrop_dl.clients.errors import DownloadFailure, DDOSGuardFailure
+from cyberdrop_dl.clients.errors import DownloadFailure, DDOSGuardFailure, ScrapeFailure
 from cyberdrop_dl.clients.scraper_client import ScraperClient
 from cyberdrop_dl.utils.utilities import CustomHTTPStatus
 
 if TYPE_CHECKING:
     from cyberdrop_dl.managers.manager import Manager
 
 
@@ -41,23 +41,23 @@
             "bunkrr": AsyncLimiter(5, 1),
             "cyberdrop": AsyncLimiter(5, 1),
             "coomer": AsyncLimiter(10, 1),
             "kemono": AsyncLimiter(10, 1),
             "pixeldrain": AsyncLimiter(10, 1),
             "other": AsyncLimiter(25, 1)
         }
-        self.download_spacer = {'bunkr': 0.5, 'bunkrr': 0.5, 'cyberdrop': 0, 'coomer': 0, 'cyberfile': 0, 'kemono': 0,
+        self.download_spacer = {'bunkr': 0.5, 'bunkrr': 0.5, 'cyberdrop': 0, 'coomer': 0.5, 'cyberfile': 0, 'kemono': 0.5,
                                 "pixeldrain": 0}
 
         self.global_rate_limiter = AsyncLimiter(self.rate_limit, 1)
         self.session_limit = asyncio.Semaphore(50)
         self.download_session_limit = asyncio.Semaphore(self.manager.config_manager.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads'])
 
         self.scraper_session = ScraperClient(self)
-        self.downloader_session = DownloadClient(self)
+        self.downloader_session = DownloadClient(manager, self)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     async def get_downloader_spacer(self, key: str) -> float:
         """Returns the download spacer for a domain"""
         if key in self.download_spacer:
             return self.download_spacer[key]
@@ -77,17 +77,35 @@
         headers = response.headers
 
         if download:
             if headers.get('ETag') in ['"eb669b6362e031fa2b0f1215480c4e30"', '"a9e4cee098dc6f1e09ec124299f26b30"']:
                 raise DownloadFailure(status="Bunkr Maintenance", message="Bunkr under maintenance")
             if headers.get('ETag') == '"d835884373f4d6c8f24742ceabe74946"':
                 raise DownloadFailure(status=HTTPStatus.NOT_FOUND, message="Imgur image has been removed")
+            if headers.get('ETag') == '"65b7753c-528a"':
+                raise DownloadFailure(status=HTTPStatus.NOT_FOUND, message="SC Scrape Image")
 
         if HTTPStatus.OK <= status < HTTPStatus.BAD_REQUEST:
             return
+        
+        if "gofile" in response.url.host.lower():
+            try:
+                JSON_Resp = await response.json()
+                if "notFound" in JSON_Resp["status"]:
+                    raise ScrapeFailure(404, "Does Not Exist")
+            except ContentTypeError:
+                pass
+
+        if "imgur" in response.url.host.lower():
+            try:
+                JSON_Resp = await response.json()
+                if "status" in JSON_Resp:
+                    raise ScrapeFailure(JSON_Resp['status'], JSON_Resp['data']['error'])
+            except ContentTypeError:
+                pass
 
         try:
             phrase = HTTPStatus(status).phrase
         except ValueError:
             phrase = "Unknown"
 
         response_text = await response.text()
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/managers/config_manager.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/managers/config_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     with open(file, 'w') as yaml_file:
         yaml.dump(data, yaml_file)
 
 
 def _load_yaml(file: Path) -> Dict:
     """Loads a yaml file and returns it as a dict"""
     with open(file, 'r') as yaml_file:
-        return yaml.load(yaml_file.read(), Loader=yaml.FullLoader)
+        yaml_values = yaml.load(yaml_file.read(), Loader=yaml.FullLoader)
+        return yaml_values if yaml_values else {}
 
 
 class ConfigManager:
     def __init__(self, manager: 'Manager'):
         self.manager = manager
         self.loaded_config: str = field(init=False)
 
@@ -94,14 +95,19 @@
             self.settings_data['Sorting']['sort_folder'] = DOWNLOAD_STORAGE / "Cyberdrop-DL Sorted Downloads"
             self.write_updated_settings_config()
 
     def _verify_authentication_config(self) -> None:
         """Verifies the authentication config file and creates it if it doesn't exist"""
         default_auth_data = copy.deepcopy(authentication_settings)
         existing_auth_data = _load_yaml(self.authentication_settings)
+        
+        if default_auth_data.keys() == existing_auth_data.keys():
+            self.authentication_data = existing_auth_data
+            return
+        
         self.authentication_data = _match_config_dicts(default_auth_data, existing_auth_data)
         _save_yaml(self.authentication_settings, self.authentication_data)
 
     def _verify_settings_config(self) -> None:
         """Verifies the settings config file and creates it if it doesn't exist"""
         default_settings_data = copy.deepcopy(settings)
         existing_settings_data = _load_yaml(self.settings)
@@ -114,36 +120,47 @@
         # change to ints
         self.settings_data['File_Size_Limits']['maximum_image_size'] = int(self.settings_data['File_Size_Limits']['maximum_image_size'])
         self.settings_data['File_Size_Limits']['maximum_video_size'] = int(self.settings_data['File_Size_Limits']['maximum_video_size'])
         self.settings_data['File_Size_Limits']['maximum_other_size'] = int(self.settings_data['File_Size_Limits']['maximum_other_size'])
         self.settings_data['File_Size_Limits']['minimum_image_size'] = int(self.settings_data['File_Size_Limits']['minimum_image_size'])
         self.settings_data['File_Size_Limits']['minimum_video_size'] = int(self.settings_data['File_Size_Limits']['minimum_video_size'])
         self.settings_data['File_Size_Limits']['minimum_other_size'] = int(self.settings_data['File_Size_Limits']['minimum_other_size'])
+        
+        self.settings_data['Runtime_Options']['ui_refresh_rate'] = int(self.settings_data['Runtime_Options']['ui_refresh_rate'])
+        self.settings_data['Runtime_Options']['log_level'] = int(self.settings_data['Runtime_Options']['log_level'])
 
         self.global_settings_data['General']['max_file_name_length'] = int(self.global_settings_data['General']['max_file_name_length'])
         self.global_settings_data['General']['max_folder_name_length'] = int(self.global_settings_data['General']['max_folder_name_length'])
         self.global_settings_data['Rate_Limiting_Options']['connection_timeout'] = int(self.global_settings_data['Rate_Limiting_Options']['connection_timeout'])
         self.global_settings_data['Rate_Limiting_Options']['download_attempts'] = int(self.global_settings_data['Rate_Limiting_Options']['download_attempts'])
         self.global_settings_data['Rate_Limiting_Options']['download_delay'] = int(self.global_settings_data['Rate_Limiting_Options']['download_delay'])
         self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads'] = int(self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads'])
         self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads_per_domain'] = int(self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads_per_domain'])
         self.global_settings_data['Rate_Limiting_Options']['rate_limit'] = int(self.global_settings_data['Rate_Limiting_Options']['rate_limit'])
         self.global_settings_data['Rate_Limiting_Options']['read_timeout'] = int(self.global_settings_data['Rate_Limiting_Options']['read_timeout'])
 
+        if default_settings_data.keys() == existing_settings_data.keys():
+            return
+        
         save_data = copy.deepcopy(self.settings_data)
         save_data['Files']['input_file'] = str(save_data['Files']['input_file'])
         save_data['Files']['download_folder'] = str(save_data['Files']['download_folder'])
         save_data["Logs"]["log_folder"] = str(save_data["Logs"]["log_folder"])
         save_data['Sorting']['sort_folder'] = str(save_data['Sorting']['sort_folder'])
         _save_yaml(self.settings, save_data)
 
     def _verify_global_settings_config(self) -> None:
         """Verifies the global settings config file and creates it if it doesn't exist"""
         default_global_settings_data = copy.deepcopy(global_settings)
         existing_global_settings_data = _load_yaml(self.global_settings)
+        
+        if default_global_settings_data.keys() == existing_global_settings_data.keys():
+            self.global_settings_data = existing_global_settings_data
+            return
+        
         self.global_settings_data = _match_config_dicts(default_global_settings_data, existing_global_settings_data)
         _save_yaml(self.global_settings, self.global_settings_data)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     def create_new_config(self, new_settings: Path, settings_data: Dict) -> None:
         """Creates a new settings config file"""
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/managers/db_manager.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/managers/db_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/managers/download_manager.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/managers/download_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 class DownloadManager:
     def __init__(self, manager: Manager):
         self.manager = manager
         self._download_instances: Dict = {}
 
         self.file_lock = FileLock()
 
-        self.download_limits = {'bunkr': 1, 'bunkrr': 1, 'cyberdrop': 1, 'coomer': 2, 'cyberfile': 2, 'kemono': 2, "pixeldrain": 2}
+        self.download_limits = {'bunkr': 1, 'bunkrr': 1, 'cyberdrop': 1, 'coomer': 2, 'cyberfile': 1, 'kemono': 2, "pixeldrain": 2}
 
     async def get_download_limit(self, key: str) -> int:
         """Returns the download limit for a domain"""
         if key in self.download_limits:
             instances = self.download_limits[key]
         else:
             instances = self.manager.config_manager.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads_per_domain']
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/managers/manager.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/managers/manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/managers/progress_manager.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/managers/progress_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/bunkrr_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/bunkrr_crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     async def fetch(self, scrape_item: ScrapeItem) -> None:
         """Determines where to send the scrape item based on the url"""
         task_id = await self.scraping_progress.add_task(scrape_item.url)
         scrape_item.url = await self.get_stream_link(scrape_item.url)
 
         if scrape_item.url.host.startswith("get"):
             scrape_item.url = await self.reinforced_link(scrape_item.url)
+            if not scrape_item.url:
+                return
             scrape_item.url = await self.get_stream_link(scrape_item.url)
 
         if "a" in scrape_item.url.parts:
             await self.album(scrape_item)
         elif "v" in scrape_item.url.parts:
             await self.video(scrape_item)
         else:
@@ -151,16 +153,19 @@
 
     @error_handling_wrapper
     async def reinforced_link(self, url: URL) -> URL:
         """Gets the download link for a given reinforced URL"""
         """get.bunkr.su"""
         async with self.request_limiter:
             soup = await self.client.get_BS4(self.domain, url)
-
-        link_container = soup.select('a[download*=""]')[-1]
+        
+        try:
+            link_container = soup.select('a[download*=""]')[-1]
+        except IndexError:
+            link_container = soup.select('a[class*=download]')[-1]
         link = URL(link_container.get('href'))
         return link
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     async def get_stream_link(self, url: URL) -> URL:
         """Gets the stream link for a given url"""
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/celebforum_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/celebforum_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/coomer_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/coomer_crawler.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class CoomerCrawler(Crawler):
     def __init__(self, manager: Manager):
         super().__init__(manager, "coomer", "Coomer")
         self.primary_base_domain = URL("https://coomer.su")
         self.ddos_guard_domain = URL("https://*.coomer.su")
         self.api_url = URL("https://coomer.su/api/v1")
-        self.request_limiter = AsyncLimiter(10, 1)
+        self.request_limiter = AsyncLimiter(4, 1)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     async def fetch(self, scrape_item: ScrapeItem) -> None:
         """Determines where to send the scrape item based on the url"""
         task_id = await self.scraping_progress.add_task(scrape_item.url)
 
@@ -92,33 +92,34 @@
 
         for file in post['attachments']:
             await handle_file(file)
 
     @error_handling_wrapper
     async def handle_direct_link(self, scrape_item: ScrapeItem) -> None:
         """Handles a direct link"""
-        filename, ext = await get_filename_and_ext(scrape_item.url.query["f"])
+        try:
+            filename, ext = await get_filename_and_ext(scrape_item.url.query["f"])
+        except KeyError:
+            filename, ext = await get_filename_and_ext(scrape_item.url.name)
         await self.handle_file(scrape_item.url, scrape_item, filename, ext)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     async def parse_datetime(self, date: str) -> int:
         """Parses a datetime string"""
         date = datetime.datetime.strptime(date, "%Y-%m-%d %H:%M:%S")
         return calendar.timegm(date.timetuple())
 
-    @error_handling_wrapper
     async def get_user_str_from_post(self, scrape_item: ScrapeItem) -> str:
         """Gets the user string from a scrape item"""
         async with self.request_limiter:
             soup = await self.client.get_BS4(self.domain, scrape_item.url)
         user = soup.select_one("a[class=post__user-name]").text
         return user
 
-    @error_handling_wrapper
     async def get_user_str_from_profile(self, scrape_item: ScrapeItem) -> str:
         """Gets the user string from a scrape item"""
         async with self.request_limiter:
             soup = await self.client.get_BS4(self.domain, scrape_item.url)
         user = soup.select_one("span[itemprop=name]").text
         return user
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/cyberdrop_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/cyberdrop_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/cyberfile_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/cyberfile_crawler.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import datetime
 from typing import TYPE_CHECKING
 
 from aiolimiter import AsyncLimiter
 from bs4 import BeautifulSoup
 from yarl import URL
 
+from cyberdrop_dl.clients.errors import PasswordProtected
 from cyberdrop_dl.scraper.crawler import Crawler
 from cyberdrop_dl.utils.dataclasses.url_objects import ScrapeItem
 from cyberdrop_dl.utils.utilities import error_handling_wrapper, log, get_filename_and_ext
 
 if TYPE_CHECKING:
     from cyberdrop_dl.managers.manager import Manager
 
@@ -70,15 +71,15 @@
                     await log(f"Couldn't find folder or file id for {scrape_item.url} element", 30)
                     continue
 
                 new_scrape_item = await self.create_scrape_item(scrape_item, link, title, True)
                 self.manager.task_group.create_task(self.run(new_scrape_item))
 
             page += 1
-            if page >= num_pages:
+            if page > num_pages:
                 break
 
     @error_handling_wrapper
     async def shared(self, scrape_item: ScrapeItem) -> None:
         """Scrapes a shared folder"""
         async with self.request_limiter:
             await self.client.get_BS4(self.domain, scrape_item.url)
@@ -141,24 +142,28 @@
     @error_handling_wrapper
     async def handle_content_id(self, scrape_item: ScrapeItem, contentId: int) -> None:
         """Scrapes a file using the content id"""
         data = {"u": contentId}
         async with self.request_limiter:
             ajax_dict = await self.client.post_data(self.domain, self.api_details, data=data)
             ajax_soup = BeautifulSoup(ajax_dict['html'].replace("\\", ""), 'html.parser')
+            
+        if "albumPasswordModel" in ajax_dict['html']:
+            await log(f"Album is password protected: {scrape_item.url}", 30)
+            raise PasswordProtected()
 
         file_menu = ajax_soup.select_one('ul[class="dropdown-menu dropdown-info account-dropdown-resize-menu"] li a')
         file_button = ajax_soup.select_one('div[class="btn-group responsiveMobileMargin"] button')
         if file_menu:
             html_download_text = file_menu.get("onclick")
         else:
             html_download_text = file_button.get("onclick")
         link = URL(html_download_text.split("'")[1])
 
-        file_detail_table = ajax_soup.select_one('table[class="table table-bordered table-striped"]')
+        file_detail_table = ajax_soup.select('table[class="table table-bordered table-striped"]')[-1]
         uploaded_row = file_detail_table.select('tr')[-2]
         uploaded_date = uploaded_row.select_one('td[class=responsiveTable]').text.strip()
         uploaded_date = await self.parse_datetime(uploaded_date)
         scrape_item.possible_datetime = uploaded_date
 
         filename, ext = await get_filename_and_ext(link.name)
         await self.handle_file(link, scrape_item, filename, ext)
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/ehentai_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/ehentai_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/erome_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/erome_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/f95zone_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/f95zone_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/fapello_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/fapello_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/gofile_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/gofile_crawler.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 import re
 from copy import deepcopy
 from typing import TYPE_CHECKING
 
 from aiolimiter import AsyncLimiter
 from yarl import URL
 
-from cyberdrop_dl.clients.errors import ScrapeFailure, DownloadFailure
+from cyberdrop_dl.clients.errors import ScrapeFailure, DownloadFailure, PasswordProtected
 from cyberdrop_dl.scraper.crawler import Crawler
 from cyberdrop_dl.utils.dataclasses.url_objects import ScrapeItem
 from cyberdrop_dl.utils.utilities import get_filename_and_ext, error_handling_wrapper
 
 if TYPE_CHECKING:
     from cyberdrop_dl.clients.scraper_client import ScraperClient
     from cyberdrop_dl.managers.manager import Manager
 
 
 class GoFileCrawler(Crawler):
     def __init__(self, manager: Manager):
         super().__init__(manager, "gofile", "GoFile")
         self.api_address = URL("https://api.gofile.io")
         self.js_address = URL("https://gofile.io/dist/js/alljs.js")
+        self.primary_base_domain = URL("https://gofile.io")
         self.token = ""
         self.websiteToken = ""
         self.headers = {}
         self.request_limiter = AsyncLimiter(10, 1)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
@@ -55,25 +56,26 @@
                 self.manager.cache_manager.remove("gofile_website_token")
                 await self.get_website_token(self.js_address, self.client)
                 async with self.request_limiter:
                     JSON_Resp = await self.client.get_json(self.domain, (self.api_address / "contents" / content_id).with_query({"wt": self.websiteToken}), headers_inc=self.headers)
             else:
                 raise ScrapeFailure(e.status, e.message)
 
-        if JSON_Resp["status"] != "ok":
-            raise ScrapeFailure(404, "Does Not Exist")
-
         JSON_Resp = JSON_Resp['data']
+        
+        if "password" in JSON_Resp:
+            raise PasswordProtected()
+        
         title = await self.create_title(JSON_Resp["name"], content_id, None)
 
         contents = JSON_Resp["children"]
         for content_id in contents:
             content = contents[content_id]
             if content["type"] == "folder":
-                new_scrape_item = await self.create_scrape_item(scrape_item, URL(content["name"]), title, True)
+                new_scrape_item = await self.create_scrape_item(scrape_item, self.primary_base_domain / "d" / content["code"], title, True)
                 self.manager.task_group.create_task(self.run(new_scrape_item))
                 continue
             if content["link"] == "overloaded":
                 link = URL(content["directLink"])
             else:
                 link = URL(content["link"])
             filename, ext = await get_filename_and_ext(link.name)
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/hotpic_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/hotpic_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/imageban_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/imageban_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/imgbb_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/imgbb_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/imgbox_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/imgbox_crawler.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,28 @@
 if TYPE_CHECKING:
     from cyberdrop_dl.managers.manager import Manager
 
 
 class ImgBoxCrawler(Crawler):
     def __init__(self, manager: Manager):
         super().__init__(manager, "imgbox", "ImgBox")
+        self.primary_base_domain = URL("https://imgbox.com")
         self.request_limiter = AsyncLimiter(10, 1)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     async def fetch(self, scrape_item: ScrapeItem) -> None:
         """Determines where to send the scrape item based on the url"""
         task_id = await self.scraping_progress.add_task(scrape_item.url)
 
         if "t" in scrape_item.url.host or "_" in scrape_item.url.name:
-            scrape_item.url = URL("https://imgbox.com") / scrape_item.url.name.split("_")[0]
+            scrape_item.url = self.primary_base_domain / scrape_item.url.name.split("_")[0]
+            
+        if "gallery/edit" in str(scrape_item.url):
+            scrape_item.url = self.primary_base_domain / "g" / scrape_item.url.parts[-2]
 
         if "g" in scrape_item.url.parts:
             await self.album(scrape_item)
         else:
             await self.image(scrape_item)
 
         await self.scraping_progress.remove_task(task_id)
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/imgkiwi_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/imgkiwi_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/imgur_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/imgur_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/jpgchurch_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/jpgchurch_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/kemono_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/kemono_crawler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 import calendar
 import datetime
+import re
 from typing import TYPE_CHECKING, Tuple, Dict
 
 from aiolimiter import AsyncLimiter
 from yarl import URL
 
+from cyberdrop_dl.clients.errors import NoExtensionFailure
 from cyberdrop_dl.scraper.crawler import Crawler
 from cyberdrop_dl.utils.dataclasses.url_objects import ScrapeItem
 from cyberdrop_dl.utils.utilities import get_filename_and_ext, error_handling_wrapper
 
 if TYPE_CHECKING:
     from cyberdrop_dl.managers.manager import Manager
 
@@ -50,15 +52,15 @@
         """Scrapes a profile"""
         offset = 0
         service, user = await self.get_service_and_user(scrape_item)
         user_str = await self.get_user_str_from_profile(scrape_item)
         api_call = self.api_url / service / "user" / user
         while True:
             async with self.request_limiter:
-                JSON_Resp = await self.client.get_json("kemono", api_call.with_query({"o": offset}))
+                JSON_Resp = await self.client.get_json(self.domain, api_call.with_query({"o": offset}))
                 offset += 50
                 if not JSON_Resp:
                     break
 
             for post in JSON_Resp:
                 await self.handle_post_content(scrape_item, post, user, user_str)
 
@@ -66,54 +68,91 @@
     async def discord(self, scrape_item: ScrapeItem) -> None:
         """Scrapes a profile"""
         offset = 0
         channel = scrape_item.url.raw_fragment
         api_call = self.api_url / "discord/channel" / channel
         while True:
             async with self.request_limiter:
-                JSON_Resp = await self.client.get_json("kemono", api_call.with_query({"o": offset}))
+                JSON_Resp = await self.client.get_json(self.domain, api_call.with_query({"o": offset}))
                 offset += 150
                 if not JSON_Resp:
                     break
 
             for post in JSON_Resp:
                 await self.handle_post_content(scrape_item, post, channel, channel)
 
     @error_handling_wrapper
     async def post(self, scrape_item: ScrapeItem) -> None:
         """Scrapes a post"""
         service, user, post_id = await self.get_service_user_and_post(scrape_item)
         user_str = await self.get_user_str_from_post(scrape_item)
         api_call = self.api_url / service / "user" / user / "post" / post_id
         async with self.request_limiter:
-            post = await self.client.get_json("kemono", api_call)
+            post = await self.client.get_json(self.domain, api_call)
         await self.handle_post_content(scrape_item, post, user, user_str)
 
     @error_handling_wrapper
     async def handle_post_content(self, scrape_item: ScrapeItem, post: Dict, user: str, user_str: str) -> None:
         """Handles the content of a post"""
         date = post["published"].replace("T", " ")
         post_id = post["id"]
         post_title = post.get("title", "")
 
+        await self.get_content_links(scrape_item, post, user_str)
+
         async def handle_file(file_obj):
             link = self.primary_base_domain / ("data" + file_obj['path'])
             link = link.with_query({"f": file_obj['name']})
             await self.create_new_scrape_item(link, scrape_item, user_str, post_title, post_id, date)
 
         if post.get('file'):
             await handle_file(post['file'])
 
         for file in post['attachments']:
             await handle_file(file)
 
+    async def get_content_links(self, scrape_item: ScrapeItem, post: Dict, user: str) -> None:
+        """Gets links out of content in post"""
+        content = post.get("content", "")
+        if not content:
+            return
+
+        date = post["published"].replace("T", " ")
+        post_id = post["id"]
+        title = post.get("title", "")
+
+        post_title = None
+        if self.manager.config_manager.settings_data['Download_Options']['separate_posts']:
+            post_title = f"{date} - {title}"
+            if self.manager.config_manager.settings_data['Download_Options']['include_album_id_in_folder_name']:
+                post_title = post_id + " - " + post_title
+
+        new_title = await self.create_title(user, None, None)
+        scrape_item = await self.create_scrape_item(scrape_item, scrape_item.url, new_title, True, None, await self.parse_datetime(date))
+        await scrape_item.add_to_parent_title(post_title)
+        await scrape_item.add_to_parent_title("Loose Files")
+
+        yarl_links = []
+        all_links = [x.group().replace(".md.", ".") for x in re.finditer(r"(?:http.*?)(?=($|\n|\r\n|\r|\s|\"|\[/URL]|']\[|]\[|\[/img]|</a>|</p>))", content)]
+        for link in all_links:
+            yarl_links.append(URL(link))
+
+        for link in yarl_links:
+            if "kemono" in link.host:
+                continue
+            scrape_item = await self.create_scrape_item(scrape_item, link, "")
+            await self.handle_external_links(scrape_item)
+
     @error_handling_wrapper
     async def handle_direct_link(self, scrape_item: ScrapeItem) -> None:
         """Handles a direct link"""
-        filename, ext = await get_filename_and_ext(scrape_item.url.query["f"])
+        try:
+            filename, ext = await get_filename_and_ext(scrape_item.url.query["f"])
+        except NoExtensionFailure:
+            filename, ext = await get_filename_and_ext(scrape_item.url.name)
         await self.handle_file(scrape_item.url, scrape_item, filename, ext)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     async def parse_datetime(self, date: str) -> int:
         """Parses a datetime string into a unix timestamp"""
         date = datetime.datetime.strptime(date, "%Y-%m-%d %H:%M:%S")
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/leakedmodels_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/leakedmodels_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/mediafire_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/mediafire_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/nudostar_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/nudostar_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/nudostartv_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/nudostartv_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/omegascans_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/omegascans_crawler.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     from cyberdrop_dl.managers.manager import Manager
 
 
 class OmegaScansCrawler(Crawler):
     def __init__(self, manager: Manager):
         super().__init__(manager, "omegascans", "OmegaScans")
         self.primary_base_domain = URL("https://omegascans.org")
+        self.api_url = "https://api.omegascans.org/chapter/query?page={}&perPage={}&series_id={}"
         self.request_limiter = AsyncLimiter(10, 1)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     async def fetch(self, scrape_item: ScrapeItem) -> None:
         """Determines where to send the scrape item based on the url"""
         task_id = await self.scraping_progress.add_task(scrape_item.url)
@@ -39,23 +40,37 @@
 
     @error_handling_wrapper
     async def series(self, scrape_item: ScrapeItem) -> None:
         """Scrapes an album"""
         async with self.request_limiter:
             soup = await self.client.get_BS4(self.domain, scrape_item.url)
 
-        chapters = soup.select("a[class*=text-gray-50]")
-        for chapter in chapters:
-            chapter_path = chapter.get("href")
-            if chapter_path.startswith("/"):
-                chapter_path = self.primary_base_domain / chapter_path[1:]
-            else:
-                chapter_path = URL(chapter_path)
-            new_scrape_item = await self.create_scrape_item(scrape_item, chapter_path, "", True)
-            self.manager.task_group.create_task(self.run(new_scrape_item))
+        scripts = soup.select("script")
+        for script in scripts:
+            if "series_id" in script.get_text():
+                series_id = script.get_text().split('series_id\\":')[1].split(",")[0]
+                break
+
+        page_number = 1
+        number_per_page = 30
+        while True:
+            api_url = URL(self.api_url.format(page_number, number_per_page, series_id))
+            async with self.request_limiter:
+                JSON_Obj = await self.client.get_json(self.domain, api_url)
+            if not JSON_Obj:
+                break
+
+            for chapter in JSON_Obj['data']:
+                chapter_url = scrape_item.url / chapter['chapter_slug']
+                new_scrape_item = await self.create_scrape_item(scrape_item, chapter_url, "", True)
+                self.manager.task_group.create_task(self.run(new_scrape_item))
+
+            if JSON_Obj['meta']['current_page'] == JSON_Obj['meta']['last_page']:
+                break
+            page_number += 1
 
     @error_handling_wrapper
     async def chapter(self, scrape_item: ScrapeItem) -> None:
         """Scrapes an image"""
         async with self.request_limiter:
             soup = await self.client.get_BS4(self.domain, scrape_item.url)
 
@@ -66,15 +81,15 @@
         title_parts = soup.select_one("title").get_text().split(" - ")
         series_name = title_parts[0]
         chapter_title = title_parts[1]
         series_title = await self.create_title(series_name, None, None)
         await scrape_item.add_to_parent_title(series_title)
         await scrape_item.add_to_parent_title(chapter_title)
 
-        date = soup.select_one('h2[class="font-semibold font-sans text-gray-400 text-xs"]').get_text()
+        date = soup.select('h2[class="font-semibold font-sans text-muted-foreground text-xs"]')[-1].get_text()
         try:
             date = await self.parse_datetime_standard(date)
         except ValueError:
             scripts = soup.select("script")
             for script in scripts:
                 if "created" in script.get_text():
                     date = script.get_text().split("created_at\\\":\\\"")[1].split(".")[0]
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/pimpandhost_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/pimpandhost_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/pixeldrain_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/redgifs_crawler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,95 @@
 from __future__ import annotations
 
-import calendar
-import datetime
 from typing import TYPE_CHECKING
 
 from aiolimiter import AsyncLimiter
 from yarl import URL
 
 from cyberdrop_dl.scraper.crawler import Crawler
 from cyberdrop_dl.utils.dataclasses.url_objects import ScrapeItem
 from cyberdrop_dl.utils.utilities import error_handling_wrapper, get_filename_and_ext
 
 if TYPE_CHECKING:
     from cyberdrop_dl.managers.manager import Manager
 
 
-class PixelDrainCrawler(Crawler):
+class RedGifsCrawler(Crawler):
     def __init__(self, manager: Manager):
-        super().__init__(manager, "pixeldrain", "PixelDrain")
-        self.api_address = URL('https://pixeldrain.com/api/')
+        super().__init__(manager, "redgifs", "RedGifs")
+        self.redgifs_api = URL("https://api.redgifs.com/")
+        self.token = ""
+        self.headers = {}
         self.request_limiter = AsyncLimiter(10, 1)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     async def fetch(self, scrape_item: ScrapeItem) -> None:
         """Determines where to send the scrape item based on the url"""
         task_id = await self.scraping_progress.add_task(scrape_item.url)
 
-        if "l" in scrape_item.url.parts:
-            await self.folder(scrape_item)
-        else:
-            await self.file(scrape_item)
+        if not self.token:
+            await self.manage_token(self.redgifs_api / "v2/auth/temporary")
+
+        if self.token:
+            if "users" in scrape_item.url.parts:
+                await self.user(scrape_item)
+            else:
+                await self.post(scrape_item)
 
         await self.scraping_progress.remove_task(task_id)
 
     @error_handling_wrapper
-    async def folder(self, scrape_item: ScrapeItem) -> None:
-        """Scrapes a folder"""
-        album_id = scrape_item.url.parts[2]
-        results = await self.get_album_results(album_id)
-        
-        async with self.request_limiter:
-            JSON_Resp = await self.client.get_json(self.domain, self.api_address / "list" / scrape_item.url.parts[-1])
+    async def user(self, scrape_item: ScrapeItem) -> None:
+        """Scrapes a users page"""
+        user_id = scrape_item.url.parts[-1].split(".")[0]
+
+        page = 1
+        total_pages = 1
+        while page <= total_pages:
+            async with self.request_limiter:
+                JSON_Resp = await self.client.get_json(self.domain, (self.redgifs_api / "v2/users" / user_id / "search").with_query(f"order=new&count=40&page={page}"), headers_inc=self.headers)
+            total_pages = JSON_Resp["pages"]
+            gifs = JSON_Resp["gifs"]
+            for gif in gifs:
+                links = gif["urls"]
+                date = gif["createDate"]
+                title = await self.create_title(user_id, None, None)
+
+                try:
+                    link = URL(links["hd"])
+                except (KeyError, TypeError):
+                    link = URL(links["sd"])
 
-        title = await self.create_title(JSON_Resp['title'], scrape_item.url.parts[2], None)
-
-        for file in JSON_Resp['files']:
-            link = await self.create_download_link(file['id'])
-            date = await self.parse_datetime(file['date_upload'].replace("T", " ").split(".")[0].strip("Z"))
-            filename, ext = await get_filename_and_ext(file['name'])
-            new_scrape_item = await self.create_scrape_item(scrape_item, link, title, True, None, date)
-            if not await self.check_album_results(link, results):
+                filename, ext = await get_filename_and_ext(link.name)
+                new_scrape_item = await self.create_scrape_item(scrape_item, link, title, True, date)
                 await self.handle_file(link, new_scrape_item, filename, ext)
+            page += 1
 
     @error_handling_wrapper
-    async def file(self, scrape_item: ScrapeItem) -> None:
-        """Scrapes a file"""
+    async def post(self, scrape_item: ScrapeItem) -> None:
+        """Scrapes a post"""
+        post_id = scrape_item.url.parts[-1].split(".")[0]
+
         async with self.request_limiter:
-            JSON_Resp = await self.client.get_json(self.domain, self.api_address / "file" / scrape_item.url.parts[-1] / "info")
+            JSON_Resp = await self.client.get_json(self.domain, self.redgifs_api / "v2/gifs" / post_id, headers_inc=self.headers)
 
-        link = await self.create_download_link(JSON_Resp['id'])
-        date = await self.parse_datetime(JSON_Resp['date_upload'].replace("T", " ").split(".")[0])
-        filename, ext = await get_filename_and_ext(JSON_Resp['name'])
-        new_scrape_item = await self.create_scrape_item(scrape_item, link, "", False, None, date)
+        title_part = JSON_Resp["gif"].get("title", "Loose Files")
+        title = await self.create_title(title_part, None, None)
+        links = JSON_Resp["gif"]["urls"]
+        date = JSON_Resp["gif"]["createDate"]
+
+        link = URL(links["hd"] if "hd" in links else links["sd"])
+
+        filename, ext = await get_filename_and_ext(link.name)
+        new_scrape_item = await self.create_scrape_item(scrape_item, link, title, True, date)
         await self.handle_file(link, new_scrape_item, filename, ext)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
-    async def parse_datetime(self, date: str) -> int:
-        """Parses a datetime string into a unix timestamp"""
-        date = datetime.datetime.strptime(date, "%Y-%m-%d %H:%M:%S")
-        return calendar.timegm(date.timetuple())
-
-    async def create_download_link(self, file_id: str) -> URL:
-        """Creates a download link for a file"""
-        link = (self.api_address / "file" / file_id).with_query('download')
-        return link
+    @error_handling_wrapper
+    async def manage_token(self, token_url: URL) -> None:
+        """Gets/Sets the redgifs token and header"""
+        async with self.request_limiter:
+            json_obj = await self.client.get_json(self.domain, token_url)
+        self.token = json_obj["token"]
+        self.headers = {"Authorization": f"Bearer {self.token}"}
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/postimg_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/postimg_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/reddit_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/reddit_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/redgifs_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/rule34xyz_crawler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,96 @@
 from __future__ import annotations
 
+import calendar
+import datetime
 from typing import TYPE_CHECKING
 
 from aiolimiter import AsyncLimiter
 from yarl import URL
 
 from cyberdrop_dl.scraper.crawler import Crawler
 from cyberdrop_dl.utils.dataclasses.url_objects import ScrapeItem
-from cyberdrop_dl.utils.utilities import error_handling_wrapper, get_filename_and_ext
+from cyberdrop_dl.utils.utilities import get_filename_and_ext, error_handling_wrapper
 
 if TYPE_CHECKING:
     from cyberdrop_dl.managers.manager import Manager
 
 
-class RedGifsCrawler(Crawler):
+class Rule34XYZCrawler(Crawler):
     def __init__(self, manager: Manager):
-        super().__init__(manager, "redgifs", "RedGifs")
-        self.redgifs_api = URL("https://api.redgifs.com/")
-        self.token = ""
-        self.headers = {}
+        super().__init__(manager, "rule34.xyz", "Rule34XYZ")
+        self.primary_base_url = URL("https://rule34.xyz")
         self.request_limiter = AsyncLimiter(10, 1)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     async def fetch(self, scrape_item: ScrapeItem) -> None:
         """Determines where to send the scrape item based on the url"""
         task_id = await self.scraping_progress.add_task(scrape_item.url)
 
-        if not self.token:
-            await self.manage_token(self.redgifs_api / "v2/auth/temporary")
-
-        if self.token:
-            if "users" in scrape_item.url.parts:
-                await self.user(scrape_item)
-            else:
-                await self.post(scrape_item)
+        if "post" in scrape_item.url.parts:
+            await self.file(scrape_item)
+        else:
+            await self.tag(scrape_item)
 
         await self.scraping_progress.remove_task(task_id)
 
     @error_handling_wrapper
-    async def user(self, scrape_item: ScrapeItem) -> None:
-        """Scrapes a users page"""
-        user_id = scrape_item.url.parts[-1].split(".")[0]
-
-        page = 1
-        total_pages = 1
-        while page <= total_pages:
-            async with self.request_limiter:
-                JSON_Resp = await self.client.get_json(self.domain, (self.redgifs_api / "v2/users" / user_id / "search").with_query(f"order=new&count=40&page={page}"), headers_inc=self.headers)
-            total_pages = JSON_Resp["pages"]
-            gifs = JSON_Resp["gifs"]
-            for gif in gifs:
-                links = gif["urls"]
-                date = gif["createDate"]
-                title_part = gif.get("title", "Loose Files")
-                title = await self.create_title(title_part, None, None)
-
-                try:
-                    link = URL(links["hd"])
-                except (KeyError, TypeError):
-                    link = URL(links["sd"])
-
-                filename, ext = await get_filename_and_ext(link.name)
-                new_scrape_item = await self.create_scrape_item(scrape_item, link, title, True, date)
-                await self.handle_file(link, new_scrape_item, filename, ext)
-            page += 1
+    async def tag(self, scrape_item: ScrapeItem) -> None:
+        """Scrapes an album"""
+        async with self.request_limiter:
+            soup = await self.client.get_BS4(self.domain, scrape_item.url)
 
-    @error_handling_wrapper
-    async def post(self, scrape_item: ScrapeItem) -> None:
-        """Scrapes a post"""
-        post_id = scrape_item.url.parts[-1].split(".")[0]
+        title = await self.create_title(scrape_item.url.parts[1], None, None)
+
+        content_block = soup.select_one('div[class="box-grid ng-star-inserted"]')
+        content = content_block.select("a[class=boxInner]")
+        for file_page in content:
+            link = file_page.get('href')
+            if link.startswith("/"):
+                link = f"{self.primary_base_url}{link}"
+            link = URL(link)
+            new_scrape_item = await self.create_scrape_item(scrape_item, link, title, True)
+            self.manager.task_group.create_task(self.run(new_scrape_item))
+        if not content:
+            return
+
+        if len(scrape_item.url.parts) > 2:
+            page = int(scrape_item.url.parts[-1])
+            next_page = scrape_item.url.with_path(f"/{scrape_item.url.parts[1]}/page/{page + 1}")
+        else:
+            next_page = scrape_item.url.with_path(f"/{scrape_item.url.parts[1]}/page/2")
+        new_scrape_item = await self.create_scrape_item(scrape_item, next_page, "")
+        self.manager.task_group.create_task(self.run(new_scrape_item))
 
+    @error_handling_wrapper
+    async def file(self, scrape_item: ScrapeItem) -> None:
+        """Scrapes an image"""
         async with self.request_limiter:
-            JSON_Resp = await self.client.get_json(self.domain, self.redgifs_api / "v2/gifs" / post_id, headers_inc=self.headers)
+            soup = await self.client.get_BS4(self.domain, scrape_item.url)
+
+        date = await self.parse_datetime(soup.select_one('div[class="posted ng-star-inserted"]').text.split("(")[1].split(")")[0])
+        scrape_item.date = date
 
-        title_part = JSON_Resp["gif"].get("title", "Loose Files")
-        title = await self.create_title(title_part, None, None)
-        links = JSON_Resp["gif"]["urls"]
-        date = JSON_Resp["gif"]["createDate"]
-
-        link = URL(links["hd"] if "hd" in links else links["sd"])
-
-        filename, ext = await get_filename_and_ext(link.name)
-        new_scrape_item = await self.create_scrape_item(scrape_item, link, title, True, date)
-        await self.handle_file(link, new_scrape_item, filename, ext)
+        image = soup.select_one('img[class*="img shadow-base"]')
+        if image:
+            link = image.get('src')
+            if link.startswith("/"):
+                link = f"{self.primary_base_url}{link}"
+            link = URL(link)
+            filename, ext = await get_filename_and_ext(link.name)
+            await self.handle_file(link, scrape_item, filename, ext)
+        video = soup.select_one("video source")
+        if video:
+            link = video.get('src')
+            if link.startswith("/"):
+                link = f"{self.primary_base_url}{link}"
+            link = URL(link)
+            filename, ext = await get_filename_and_ext(link.name)
+            await self.handle_file(link, scrape_item, filename, ext)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
-    @error_handling_wrapper
-    async def manage_token(self, token_url: URL) -> None:
-        """Gets/Sets the redgifs token and header"""
-        async with self.request_limiter:
-            json_obj = await self.client.get_json(self.domain, token_url)
-        self.token = json_obj["token"]
-        self.headers = {"Authorization": f"Bearer {self.token}"}
+    async def parse_datetime(self, date: str) -> int:
+        """Parses a datetime string into a unix timestamp"""
+        date = datetime.datetime.strptime(date, "%b %d, %Y, %I:%M:%S %p")
+        return calendar.timegm(date.timetuple())
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/rule34xxx_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/rule34xxx_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/rule34xyz_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/pixeldrain_crawler.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,94 +3,92 @@
 import calendar
 import datetime
 from typing import TYPE_CHECKING
 
 from aiolimiter import AsyncLimiter
 from yarl import URL
 
+from cyberdrop_dl.clients.errors import NoExtensionFailure
 from cyberdrop_dl.scraper.crawler import Crawler
 from cyberdrop_dl.utils.dataclasses.url_objects import ScrapeItem
-from cyberdrop_dl.utils.utilities import get_filename_and_ext, error_handling_wrapper
+from cyberdrop_dl.utils.utilities import error_handling_wrapper, get_filename_and_ext
 
 if TYPE_CHECKING:
     from cyberdrop_dl.managers.manager import Manager
 
 
-class Rule34XYZCrawler(Crawler):
+class PixelDrainCrawler(Crawler):
     def __init__(self, manager: Manager):
-        super().__init__(manager, "rule34.xyz", "Rule34XYZ")
-        self.primary_base_url = URL("https://rule34.xyz")
+        super().__init__(manager, "pixeldrain", "PixelDrain")
+        self.api_address = URL('https://pixeldrain.com/api/')
         self.request_limiter = AsyncLimiter(10, 1)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     async def fetch(self, scrape_item: ScrapeItem) -> None:
         """Determines where to send the scrape item based on the url"""
         task_id = await self.scraping_progress.add_task(scrape_item.url)
 
-        if "post" in scrape_item.url.parts:
-            await self.file(scrape_item)
+        if "l" in scrape_item.url.parts:
+            await self.folder(scrape_item)
         else:
-            await self.tag(scrape_item)
+            await self.file(scrape_item)
 
         await self.scraping_progress.remove_task(task_id)
 
     @error_handling_wrapper
-    async def tag(self, scrape_item: ScrapeItem) -> None:
-        """Scrapes an album"""
+    async def folder(self, scrape_item: ScrapeItem) -> None:
+        """Scrapes a folder"""
+        album_id = scrape_item.url.parts[2]
+        results = await self.get_album_results(album_id)
+        
         async with self.request_limiter:
-            soup = await self.client.get_BS4(self.domain, scrape_item.url)
+            JSON_Resp = await self.client.get_json(self.domain, self.api_address / "list" / scrape_item.url.parts[-1])
 
-        title = await self.create_title(scrape_item.url.parts[1], None, None)
+        title = await self.create_title(JSON_Resp['title'], scrape_item.url.parts[2], None)
 
-        content_block = soup.select_one('div[class="box-grid ng-star-inserted"]')
-        content = content_block.select("a[class=boxInner]")
-        for file_page in content:
-            link = file_page.get('href')
-            if link.startswith("/"):
-                link = f"{self.primary_base_url}{link}"
-            link = URL(link)
-            new_scrape_item = await self.create_scrape_item(scrape_item, link, title, True)
-            self.manager.task_group.create_task(self.run(new_scrape_item))
-        if not content:
-            return
-
-        if len(scrape_item.url.parts) > 2:
-            page = int(scrape_item.url.parts[-1])
-            next_page = scrape_item.url.with_path(f"/{scrape_item.url.parts[1]}/page/{page + 1}")
-        else:
-            next_page = scrape_item.url.with_path(f"/{scrape_item.url.parts[1]}/page/2")
-        new_scrape_item = await self.create_scrape_item(scrape_item, next_page, "")
-        self.manager.task_group.create_task(self.run(new_scrape_item))
+        for file in JSON_Resp['files']:
+            link = await self.create_download_link(file['id'])
+            date = await self.parse_datetime(file['date_upload'].replace("T", " ").split(".")[0].strip("Z"))
+            try:
+                filename, ext = await get_filename_and_ext(file['name'])
+            except NoExtensionFailure:
+                if "image" or "video" in file["mime_type"]:
+                    filename, ext = await get_filename_and_ext(file['name'] + "." + file["mime_type"].split("/")[-1])
+                else:
+                    raise NoExtensionFailure()
+            new_scrape_item = await self.create_scrape_item(scrape_item, link, title, True, None, date)
+            if not await self.check_album_results(link, results):
+                await self.handle_file(link, new_scrape_item, filename, ext)
 
     @error_handling_wrapper
     async def file(self, scrape_item: ScrapeItem) -> None:
-        """Scrapes an image"""
+        """Scrapes a file"""
         async with self.request_limiter:
-            soup = await self.client.get_BS4(self.domain, scrape_item.url)
+            JSON_Resp = await self.client.get_json(self.domain, self.api_address / "file" / scrape_item.url.parts[-1] / "info")
 
-        date = await self.parse_datetime(soup.select_one('div[class="posted ng-star-inserted"]').text.split("(")[1].split(")")[0])
-        scrape_item.date = date
-
-        image = soup.select_one('img[class*="img shadow-base"]')
-        if image:
-            link = image.get('src')
-            if link.startswith("/"):
-                link = f"{self.primary_base_url}{link}"
-            link = URL(link)
-            filename, ext = await get_filename_and_ext(link.name)
-            await self.handle_file(link, scrape_item, filename, ext)
-        video = soup.select_one("video source")
-        if video:
-            link = video.get('src')
-            if link.startswith("/"):
-                link = f"{self.primary_base_url}{link}"
-            link = URL(link)
-            filename, ext = await get_filename_and_ext(link.name)
-            await self.handle_file(link, scrape_item, filename, ext)
+        link = await self.create_download_link(JSON_Resp['id'])
+        date = await self.parse_datetime(JSON_Resp['date_upload'].replace("T", " ").split(".")[0])
+        try:
+            filename, ext = await get_filename_and_ext(JSON_Resp['name'])
+        except NoExtensionFailure:
+            if "image" or "video" in JSON_Resp["mime_type"]:
+                filename, ext = await get_filename_and_ext(JSON_Resp['name'] + "." + JSON_Resp["mime_type"].split("/")[-1])
+            else:
+                raise NoExtensionFailure()
+        new_scrape_item = await self.create_scrape_item(scrape_item, link, "", False, None, date)
+        await self.handle_file(link, new_scrape_item, filename, ext)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     async def parse_datetime(self, date: str) -> int:
         """Parses a datetime string into a unix timestamp"""
-        date = datetime.datetime.strptime(date, "%b %d, %Y, %I:%M:%S %p")
+        try:
+            date = datetime.datetime.strptime(date, "%Y-%m-%d %H:%M:%S")
+        except ValueError:
+            date = datetime.datetime.strptime(date, "%Y-%m-%d %H:%M:%SZ")
         return calendar.timegm(date.timetuple())
+
+    async def create_download_link(self, file_id: str) -> URL:
+        """Creates a download link for a file"""
+        link = (self.api_address / "file" / file_id).with_query('download')
+        return link
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/saint_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/saint_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/scrolller_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/scrolller_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/simpcity_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/simpcity_crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,16 @@
                 current_post_number = int(post.select_one(self.posts_number_selector).get(self.posts_number_attribute).split('/')[-1].split('post-')[-1])
                 scrape_post, continue_scraping = await self.check_post_number(post_number, current_post_number)
 
                 if scrape_post:
                     date = int(post.select_one(self.post_date_selector).get(self.post_date_attribute))
                     new_scrape_item = await self.create_scrape_item(scrape_item, thread_url, title, False, None, date)
 
-                    for elem in post.find_all(self.quotes_selector):
-                        elem.decompose()
+                    # for elem in post.find_all(self.quotes_selector):
+                    #     elem.decompose()
                     post_content = post.select_one(self.posts_content_selector)
                     await self.post(new_scrape_item, post_content, current_post_number)
 
                 if not continue_scraping:
                     break
 
             next_page = soup.select_one(self.next_page_selector)
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/socialmediagirls_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/socialmediagirls_crawler.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.posts_content_selector = "div[class=bbWrapper]"
         self.next_page_selector = "a[class*=pageNav-jump--next]"
         self.next_page_attribute = "href"
         self.links_selector = "a"
         self.links_attribute = "href"
         self.attachment_url_part = "attachments"
         self.images_selector = "img[class*=bbImage]"
-        self.images_attribute = "data-src"
+        self.images_attribute = "src"
         self.videos_selector = "video source"
         self.iframe_selector = "iframe[class=saint-iframe]"
         self.videos_attribute = "src"
         self.embeds_selector = "span[data-s9e-mediaembed-iframe]"
         self.embeds_attribute = "data-s9e-mediaembed-iframe"
         self.attachments_block_selector = "section[class=message-attachments]"
         self.attachments_selector = "a"
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/toonily_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/toonily_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/xbunker_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/xbunker_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/crawlers/xbunkr_crawler.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/crawlers/xbunkr_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/jdownloader.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/jdownloader.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/scraper/scraper.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/scraper/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
                         "imgur": self.imgur, "img.kiwi": self.imgwiki, "jpg.church": self.jpgchurch,
                         "jpg.homes": self.jpgchurch, "jpg.fish": self.jpgchurch, "jpg.fishing": self.jpgchurch,
                         "jpg.pet": self.jpgchurch, "jpeg.pet": self.jpgchurch, "jpg1.su": self.jpgchurch,
                         "jpg2.su": self.jpgchurch, "jpg3.su": self.jpgchurch, "jpg4.su": self.jpgchurch,
                         "host.church": self.jpgchurch, "kemono": self.kemono, "leakedmodels": self.leakedmodels,
                         "mediafire": self.mediafire, "nudostar.com": self.nudostar, "nudostar.tv": self.nudostartv,
                         "omegascans": self.omegascans, "pimpandhost": self.pimpandhost, "pixeldrain": self.pixeldrain,
-                        "postimg": self.postimg, "reddit": self.reddit, "redd.it": self.reddit, "redgifs": self.redgifs,
-                        "rule34.xxx": self.rule34xxx, "rule34.xyz": self.rule34xyz, "saint": self.saint,
-                        "scrolller": self.scrolller, "simpcity": self.simpcity,
-                        "socialmediagirls": self.socialmediagirls, "toonily": self.toonily, "xbunker": self.xbunker,
-                        "xbunkr": self.xbunkr, "bunkr": self.bunkrr}
+                        "postimg": self.postimg, "realbooru": self.realbooru, "reddit": self.reddit, 
+                        "redd.it": self.reddit, "redgifs": self.redgifs, "rule34.xxx": self.rule34xxx, 
+                        "rule34.xyz": self.rule34xyz, "saint": self.saint, "scrolller": self.scrolller, 
+                        "simpcity": self.simpcity, "socialmediagirls": self.socialmediagirls, "toonily": self.toonily, 
+                        "xbunker": self.xbunker, "xbunkr": self.xbunkr, "bunkr": self.bunkrr}
         self.existing_crawlers = {}
         self.no_crawler_downloader = Downloader(self.manager, "no_crawler")
         self.jdownloader = JDownloader(self.manager)
 
     async def bunkrr(self) -> None:
         """Creates a Bunkr Crawler instance"""
         from cyberdrop_dl.scraper.crawlers.bunkrr_crawler import BunkrrCrawler
@@ -180,14 +180,19 @@
         from cyberdrop_dl.scraper.crawlers.pixeldrain_crawler import PixelDrainCrawler
         self.existing_crawlers['pixeldrain'] = PixelDrainCrawler(self.manager)
 
     async def postimg(self) -> None:
         """Creates a PostImg Crawler instance"""
         from cyberdrop_dl.scraper.crawlers.postimg_crawler import PostImgCrawler
         self.existing_crawlers['postimg'] = PostImgCrawler(self.manager)
+        
+    async def realbooru(self) -> None:
+        """Creates a RealBooru Crawler instance"""
+        from cyberdrop_dl.scraper.crawlers.realbooru_crawler import RealBooruCrawler
+        self.existing_crawlers['realbooru'] = RealBooruCrawler(self.manager)
 
     async def reddit(self) -> None:
         """Creates a Reddit Crawler instance"""
         from cyberdrop_dl.scraper.crawlers.reddit_crawler import RedditCrawler
         self.existing_crawlers['reddit'] = RedditCrawler(self.manager)
         self.existing_crawlers['redd.it'] = self.existing_crawlers['reddit']
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/ui/progress/downloads_progress.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/ui/progress/downloads_progress.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/ui/progress/file_progress.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/ui/progress/file_progress.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/ui/progress/scraping_progress.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/ui/progress/scraping_progress.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/ui/progress/statistic_progress.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/ui/progress/statistic_progress.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/ui/prompts/general_prompts.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/ui/prompts/general_prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,23 +25,24 @@
     """Main prompt for the program"""
     action = inquirer.select(
         message="What would you like to do?",
         choices=[
             Choice(1, "Download"),
             Choice(2, "Download (All Configs)"),
             Choice(3, "Retry Failed Downloads"),
-            Choice(4, "Edit URLs File"),
+            Choice(4, "Sort All Configs"),
+            Choice(5, "Edit URLs File"),
             Separator(),
-            Choice(5, f"Select Config (Current: {manager.config_manager.loaded_config})"),
-            Choice(6, "Change URLs.txt file and Download Location"),
-            Choice(7, "Manage Configs"),
+            Choice(6, f"Select Config (Current: {manager.config_manager.loaded_config})"),
+            Choice(7, "Change URLs.txt file and Download Location"),
+            Choice(8, "Manage Configs"),
             Separator(),
-            Choice(8, "Import Cyberdrop_V4 Items"),
-            Choice(9, "Donate"),
-            Choice(10, "Exit"),
+            Choice(9, "Import Cyberdrop_V4 Items"),
+            Choice(10, "Donate"),
+            Choice(11, "Exit"),
         ], long_instruction="ARROW KEYS: Navigate | ENTER: Select",
         vi_mode=manager.vi_mode,
     ).execute()
 
     return action
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/ui/prompts/settings_authentication_prompts.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/ui/prompts/settings_authentication_prompts.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/ui/prompts/settings_global_prompts.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/ui/prompts/settings_global_prompts.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/ui/prompts/settings_user_prompts.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/ui/prompts/settings_user_prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,33 +341,46 @@
                    enabled=config["Runtime_Options"]["skip_check_for_empty_folders"]),
             Choice(value="delete_partial_files",
                    name="Delete partial files in the download folder",
                    enabled=config["Runtime_Options"]["delete_partial_files"]),
             Choice(value="send_unsupported_to_jdownloader",
                    name="Send unsupported urls to JDownloader to download",
                    enabled=config["Runtime_Options"]["send_unsupported_to_jdownloader"]),
+            Choice(value="update_last_forum_post",
+                   name="Update the last forum post after scraping",
+                   enabled=config["Runtime_Options"]["update_last_forum_post"]),
         ], long_instruction="ARROW KEYS: Move | TAB: Select | ENTER: Confirm",
         vi_mode=manager.vi_mode,
     ).execute()
 
     log_level = inquirer.number(
         message="Enter the log level:",
         default=int(config['Runtime_Options']['log_level']),
         validate=NumberValidator(),
         long_instruction="10 is the default (uses pythons logging numerical levels)",
         vi_mode=manager.vi_mode,
     ).execute()
 
+    ui_refresh_rate = inquirer.number(
+        message="Enter the desired UI refresh rate:",
+        default=int(config['Runtime_Options']['ui_refresh_rate']),
+        min_allowed=1,
+        validate=NumberValidator(),
+        long_instruction="10 is the default",
+        vi_mode=manager.vi_mode,
+    ).execute()
+
     for key in config["Runtime_Options"]:
         config["Runtime_Options"][key] = False
 
     for key in action:
         config["Runtime_Options"][key] = True
 
     config['Runtime_Options']['log_level'] = int(log_level)
+    config['Runtime_Options']['ui_refresh_rate'] = int(ui_refresh_rate)
 
 
 def edit_sort_options_prompt(manager: Manager, config: Dict) -> None:
     """Edit the sort options"""
     console.clear()
     console.print("Editing Sort Options")
     config["Sorting"]["sort_downloads"] = False
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/ui/prompts/url_file_prompts.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/ui/prompts/url_file_prompts.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/ui/ui.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/ui/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,33 @@
             manager.args_manager.all_configs = True
             break
 
         # Retry Failed Downloads
         elif action == 3:
             manager.args_manager.retry = True
             break
+            
+        # Sort All Configs
+        elif action == 4:
+            manager.args_manager.sort_all_configs = True
+            manager.args_manager.all_configs = True
+            break
 
         # Edit URLs
-        elif action == 4:
+        elif action == 5:
             input_file = manager.config_manager.settings_data['Files']['input_file'] if not manager.args_manager.input_file else manager.args_manager.input_file
             edit_urls_prompt(input_file, manager.vi_mode)
 
         # Select Config
-        elif action == 5:
+        elif action == 6:
             configs = manager.config_manager.get_configs()
             selected_config = select_config_prompt(manager, configs)
             manager.config_manager.change_config(selected_config)
 
-        elif action == 6:
+        elif action == 7:
             console.clear()
             console.print("Editing Input / Output File Paths")
             input_file = inquirer.filepath(
                 message="Enter the input file path:",
                 default=str(manager.config_manager.settings_data['Files']['input_file']),
                 validate=PathValidator(is_file=True, message="Input is not a file"),
                 vi_mode=manager.vi_mode,
@@ -75,15 +81,15 @@
             ).execute()
 
             manager.config_manager.settings_data['Files']['input_file'] = Path(input_file)
             manager.config_manager.settings_data['Files']['download_folder'] = Path(download_folder)
             manager.config_manager.write_updated_settings_config()
 
         # Manage Configs
-        elif action == 7:
+        elif action == 8:
             while True:
                 console.clear()
                 console.print("[bold]Manage Configs[/bold]")
                 console.print(f"[bold]Current Config:[/bold] {manager.config_manager.loaded_config}")
 
                 action = manage_configs_prompt(manager)
 
@@ -130,17 +136,17 @@
                     edit_global_settings_prompt(manager)
 
                 # Done
                 elif action == 7:
                     break
 
         # Import Cyberdrop_V4 Items
-        elif action == 8:
+        elif action == 9:
             import_cyberdrop_v4_items_prompt(manager)
 
         # Donate
-        elif action == 9:
+        elif action == 10:
             donations_prompt(manager)
 
         # Exit
-        elif action == 10:
+        elif action == 11:
             exit(0)
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/args/args.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/args/args.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,34 +11,42 @@
     general.add_argument("-V", "--version", action="version", version=f"%(prog)s {VERSION}")
     general.add_argument("--config", type=str, help="name of config to load", default="")
     general.add_argument("--proxy", type=str, help="manually specify proxy string", default="")
     general.add_argument("--flaresolverr", type=str, help="IP:PORT for flaresolverr", default="")
     general.add_argument("--no-ui", action="store_true", help="Disables the UI/Progress view entirely", default=False)
     general.add_argument("--download", action="store_true", help="Skip the UI and go straight to downloading", default=False)
     general.add_argument("--download-all-configs", action="store_true", help="Skip the UI and go straight to downloading (runs all configs sequentially)", default=False)
+    general.add_argument("--sort-all-configs", action="store_true", help="Sort all configs sequentially", default=False)
     general.add_argument("--retry-failed", action="store_true", help="retry failed downloads", default=False)
     general.add_argument("--vi-mode", action="store_true", help="enable VIM keybindings for UI", default=None)
 
     # File Paths
     file_paths = parser.add_argument_group("File_Paths")
     file_paths.add_argument("-i", "--input-file", type=str, help="path to txt file containing urls to download", default="")
     file_paths.add_argument("-d", "--output-folder", type=str, help="path to download folder", default="")
     file_paths.add_argument("--config-file", type=str, help="path to the CDL settings.yaml file to load", default="")
     file_paths.add_argument("--appdata-folder", type=str, help="path to where you want CDL to store it's AppData folder", default="")
     file_paths.add_argument("--log-folder", type=str, help="path to where you want CDL to store it's log files", default="")
+    file_paths.add_argument("--main-log-filename", type=str, help="filename for the main log file", default="")
+    file_paths.add_argument("--last-forum-post-filename", type=str, help="filename for the last forum post log file", default="")
+    file_paths.add_argument("--unsupported-urls-filename", type=str, help="filename for the unsupported urls log file", default="")
+    file_paths.add_argument("--download-error-urls-filename", type=str, help="filename for the download error urls log file", default="")
+    file_paths.add_argument("--scrape-error-urls-filename", type=str, help="filename for the scrape error urls log file", default="")
 
     # Settings
     download_options = parser.add_argument_group("Download_Options")
     download_options.add_argument("--block-download-sub-folders", action="store_true", help="block sub folder creation", default=False)
     download_options.add_argument("--disable-download-attempt-limit", action="store_true", help="disable download attempt limit", default=False)
     download_options.add_argument("--disable-file-timestamps", action="store_true", help="disable file timestamps", default=False)
     download_options.add_argument("--include-album-id-in-folder-name", action="store_true", help="include album id in folder name", default=False)
     download_options.add_argument("--include-thread-id-in-folder-name", action="store_true", help="include thread id in folder name", default=False)
     download_options.add_argument("--remove-domains-from-folder-names", action="store_true", help="remove website domains from folder names", default=False)
     download_options.add_argument("--remove-generated-id-from-filenames", action="store_true", help="remove site generated id from filenames", default=False)
+    download_options.add_argument("--scrape-single-forum-post", action="store_true", help="scrape single forum post", default=False)
+    download_options.add_argument("--separate-posts", action="store_true", help="separate posts into folders", default=False)
     download_options.add_argument("--skip-download-mark-completed", action="store_true", help="skip download and mark as completed in history", default=False)
 
     file_size_limits = parser.add_argument_group("File_Size_Limits")
     file_size_limits.add_argument("--maximum-image-size", type=int, help="maximum image size in bytes (default: %(default)s)", default=0)
     file_size_limits.add_argument("--maximum-video-size", type=int, help="maximum video size in bytes (default: %(default)s)", default=0)
     file_size_limits.add_argument("--maximum-other-size", type=int, help="maximum other size in bytes (default: %(default)s)", default=0)
     file_size_limits.add_argument("--minimum-image-size", type=int, help="minimum image size in bytes (default: %(default)s)", default=0)
@@ -57,11 +65,17 @@
     runtime_options = parser.add_argument_group("Runtime_Options")
     runtime_options.add_argument("--ignore-history", action="store_true", help="ignore history when scraping", default=False)
     runtime_options.add_argument("--log-level", type=int, help="set the log level (default: %(default)s)", default=10)
     runtime_options.add_argument("--skip-check-for-partial-files", action="store_true", help="skip check for partial downloads", default=False)
     runtime_options.add_argument("--skip-check-for-empty-folders", action="store_true", help="skip check (and removal) for empty folders", default=False)
     runtime_options.add_argument("--delete-partial-files", action="store_true", help="delete partial downloads", default=False)
     runtime_options.add_argument("--send-unsupported-to-jdownloader", action="store_true", help="send unsupported urls to jdownloader", default=False)
+    runtime_options.add_argument("--ui-refresh-rate", type=int, help="set the UI refresh rate (default: %(default)s)", default=10)
+    runtime_options.add_argument("--update-last-forum-post", action="store_true", help="update the last forum post", default=False)
+
+    sorting_options = parser.add_argument_group("Sorting")
+    sorting_options.add_argument("--sort-downloads", action="store_true", help="sort downloads into folders", default=False)
+    sorting_options.add_argument("--sort_folder", type=str, help="path to where you want CDL to store it's log files", default="")
 
     # Links
     parser.add_argument("links", metavar="link", nargs="*", help="link to content to download (passing multiple links is supported)", default=[])
     return parser.parse_args()
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/args/browser_cookie_extraction.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/args/browser_cookie_extraction.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/args/config_definitions.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/args/config_definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,16 @@
     "Runtime_Options": {
         "ignore_history": False,
         "log_level": 10,
         "skip_check_for_partial_files": False,
         "skip_check_for_empty_folders": False,
         "delete_partial_files": False,
         "send_unsupported_to_jdownloader": False,
+        "ui_refresh_rate": 10,
+        "update_last_forum_post": False,
     },
     "Sorting": {
         "sort_downloads": False,
         "sort_folder": str(DOWNLOAD_STORAGE / "Cyberdrop-DL Sorted Downloads"),
         "sort_incremementer_format": " ({i})",
         "sorted_audio": "{sort_dir}/{base_dir}/Audio/{filename}{ext}",
         "sorted_image": "{sort_dir}/{base_dir}/Images/{filename}{ext}",
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/database/table_definitions.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/database/table_definitions.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
                                                url_path TEXT,
                                                referer TEXT,
                                                album_id TEXT,
                                                download_path TEXT,
                                                download_filename TEXT,
                                                original_filename TEXT,
                                                completed INTEGER NOT NULL,
+                                               created_at TIMESTAMP,
+                                               completed_at TIMESTAMP,
                                                PRIMARY KEY (domain, url_path, original_filename)
                                                );"""
 
 create_fixed_history = """CREATE TABLE IF NOT EXISTS media_copy (domain TEXT,
                                                url_path TEXT,
                                                referer TEXT,
                                                album_id TEXT,
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/database/tables/history_table.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/database/tables/history_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from sqlite3 import Row
+from sqlite3 import Row, IntegrityError
 
 import aiosqlite
 from typing import TYPE_CHECKING, Iterable, Any
 from yarl import URL
 
 from cyberdrop_dl.utils.database.table_definitions import create_history, create_fixed_history
 
@@ -96,27 +96,30 @@
         return sql_file_check and sql_file_check[0] != 0
 
     async def insert_incompleted(self, domain: str, media_item: MediaItem) -> None:
         """Inserts an uncompleted file into the database"""
         domain = await get_db_domain(domain)
         url_path = await get_db_path(media_item.url, str(media_item.referer))
         download_filename = media_item.download_filename if isinstance(media_item.download_filename, str) else ""
-        await self.db_conn.execute("""UPDATE media SET domain = ?, album_id = ? WHERE domain = 'no_crawler' and url_path = ? and referer = ?""", 
-                                   (domain, media_item.album_id, url_path, str(media_item.referer)))
-        await self.db_conn.execute("""INSERT OR IGNORE INTO media (domain, url_path, referer, album_id, download_path, download_filename, original_filename, completed) VALUES (?, ?, ?, ?, ?, ?, ?, ?)""",
+        try:
+            await self.db_conn.execute("""UPDATE media SET domain = ?, album_id = ? WHERE domain = 'no_crawler' and url_path = ? and referer = ?""", 
+                                       (domain, media_item.album_id, url_path, str(media_item.referer)))
+        except IntegrityError:
+            await self.db_conn.execute("""DELETE FROM media WHERE domain = 'no_crawler' and url_path = ?""", (url_path,))
+        await self.db_conn.execute("""INSERT OR IGNORE INTO media (domain, url_path, referer, album_id, download_path, download_filename, original_filename, completed, created_at) VALUES (?, ?, ?, ?, ?, ?, ?, ?, CURRENT_TIMESTAMP)""",
                                    (domain, url_path, str(media_item.referer), media_item.album_id, str(media_item.download_folder), download_filename, media_item.original_filename, 0))
         await self.db_conn.execute("""UPDATE media SET download_filename = ? WHERE domain = ? and url_path = ?""",
                                    (download_filename, domain, url_path))
         await self.db_conn.commit()
 
     async def mark_complete(self, domain: str, media_item: MediaItem) -> None:
         """Mark a download as completed in the database"""
         domain = await get_db_domain(domain)
         url_path = await get_db_path(media_item.url, str(media_item.referer))
-        await self.db_conn.execute("""UPDATE media SET completed = 1 WHERE domain = ? and url_path = ?""",
+        await self.db_conn.execute("""UPDATE media SET completed = 1, completed_at = CURRENT_TIMESTAMP WHERE domain = ? and url_path = ?""",
                                    (domain, url_path))
         await self.db_conn.commit()
 
     async def check_filename_exists(self, filename: str) -> bool:
         """Checks whether a downloaded filename exists in the database"""
         cursor = await self.db_conn.cursor()
         result = await cursor.execute("""SELECT EXISTS(SELECT 1 FROM media WHERE download_filename = ?)""", (filename,))
@@ -147,15 +150,15 @@
         cursor = await self.db_conn.cursor()
         result = await cursor.execute("""SELECT * from media WHERE domain = 'bunkr' and completed = 1""")
         bunkr_entries = await result.fetchall()
 
         for entry in bunkr_entries:
             entry = list(entry)
             entry[0] = "bunkrr"
-            await self.db_conn.execute("""INSERT or REPLACE INTO media VALUES (?, ?, ?, ?, ?, ?, ?, ?)""", entry)
+            await self.db_conn.execute("""INSERT or REPLACE INTO media VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?)""", entry)
         await self.db_conn.commit()
 
         await self.db_conn.execute("""DELETE FROM media WHERE domain = 'bunkr'""")
         await self.db_conn.commit()
 
     async def fix_primary_keys(self) -> None:
         cursor = await self.db_conn.cursor()
@@ -170,17 +173,25 @@
             await self.db_conn.commit()
 
             await self.db_conn.execute("""DROP TABLE media""")
             await self.db_conn.commit()
 
             await self.db_conn.execute("""ALTER TABLE media_copy RENAME TO media""")
             await self.db_conn.commit()
-            
+
     async def add_columns(self) -> None:
         cursor = await self.db_conn.cursor()
         result = await cursor.execute("""pragma table_info(media)""")
         result = await result.fetchall()
         current_cols = [col[1] for col in result]
         
         if "album_id" not in current_cols:
             await self.db_conn.execute("""ALTER TABLE media ADD COLUMN album_id TEXT""")
             await self.db_conn.commit()
+
+        if "created_at" not in current_cols:
+            await self.db_conn.execute("""ALTER TABLE media ADD COLUMN created_at TIMESTAMP""")
+            await self.db_conn.commit()
+
+        if "completed_at" not in current_cols:
+            await self.db_conn.execute("""ALTER TABLE media ADD COLUMN completed_at TIMESTAMP""")
+            await self.db_conn.commit()
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/database/tables/temp_table.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/database/tables/temp_table.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/dataclasses/supported_domains.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/dataclasses/supported_domains.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,22 +7,19 @@
     """The allows options for domains to skip when scraping and mappings"""
     supported_hosts: ClassVar[Tuple[str, ...]] = ("bunkr", "bunkrr", "celebforum", "coomer", "cyberdrop", "cyberfile",
                                                   "e-hentai", "erome", "fapello", "f95zone", "gofile", "hotpic",
                                                   "ibb.co", "imageban", "imgbox", "imgur", "img.kiwi", "jpg.church",
                                                   "jpg.homes", "jpg.fish", "jpg.fishing", "jpg.pet", "jpeg.pet",
                                                   "jpg1.su", "jpg2.su", "jpg3.su", "jpg4.su", "host.church", "kemono",
                                                   "leakedmodels", "mediafire", "nudostar.com", "nudostar.tv",
-                                                  "omegascans", "pimpandhost", "pixeldrain", "postimg", "reddit",
-                                                  "redd.it", "redgifs", "rule34.xxx", "rule34.xyz", "saint",
+                                                  "omegascans", "pimpandhost", "pixeldrain", "postimg", "realbooru", 
+                                                  "reddit", "redd.it", "redgifs", "rule34.xxx", "rule34.xyz", "saint",
                                                   "scrolller", "simpcity", "socialmediagirls", "toonily", "xbunker",
                                                   "xbunkr")
 
     supported_forums: ClassVar[Tuple[str, ...]] = ("celebforum.to", "f95zone.to", "leakedmodels.com", "nudostar.com",
                                                    "simpcity.su", "forums.socialmediagirls.com", "xbunker.nu")
     supported_forums_map = {"celebforum.to": "celebforum", "f95zone.to": "f95zone", "leakedmodels.com": "leakedmodels",
                             "nudostar.com": "nudostar", "simpcity.su": "simpcity",
                             "forums.socialmediagirls.com": "socialmediagirls", "xbunker.nu": "xbunker"}
 
-    supported_ddos_guard: ClassVar[Tuple[str, ...]] = (".bunkrr.su", ".coomer.su", ".kemono.su")
-    supported_ddos_guard_map = {".bunkrr.su": "bunkrr", ".coomer.su": "coomer", ".kemono.su": "kemono"}
-
     sites: List[str]
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/dataclasses/url_objects.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/dataclasses/url_objects.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,17 +17,21 @@
         self.download_folder: Path = download_folder
         self.filename: str = filename
         self.ext: str = ext
         self.download_filename: str = field(init=False)
         self.original_filename: str = original_filename
         self.file_lock_reference_name: str = field(init=False)
         self.datetime: str = field(init=False)
+        
         self.filesize: int = field(init=False)
         self.current_attempt: int = field(init=False)
-        self.download_task_id: TaskID = field(init=False)
+        
+        self.partial_file: Path = field(init=False)
+        self.complete_file: Path = field(init=False)
+        self.task_id: TaskID = field(init=False)
 
 
 class ScrapeItem:
     def __init__(self, url: "URL", parent_title: str, part_of_album: bool = False, album_id: Union[str, None] = None, possible_datetime: int = None,
                  retry: bool = False, retry_path: Path = None):
         self.url: URL = url
         self.parent_title: str = parent_title
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/sorting.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/sorting.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
     async def sort(self) -> None:
         """Sorts the files in the download directory into their respective folders"""
         await log_with_color("\nSorting Downloads: Please Wait", "cyan", 20)
 
         if await self.check_dir_parents():
             return
+        
+        if not self.download_dir.is_dir():
+            await log_with_color("Download Directory does not exist", "red", 40)
+            return
 
         for folder in self.download_dir.iterdir():
             if not folder.is_dir():
                 continue
 
             files = await self.find_files_in_dir(folder)
             for file in files:
```

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/transfer/first_time_setup.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/transfer/first_time_setup.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/transfer/transfer_v4_config.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/transfer/transfer_v4_config.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/transfer/transfer_v4_db.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/transfer/transfer_v4_db.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.2.9/cyberdrop_dl/utils/utilities.py` & `cyberdrop_dl-5.3.1/cyberdrop_dl/utils/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from functools import wraps
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import rich
 from yarl import URL
 
-from cyberdrop_dl.clients.errors import NoExtensionFailure, FailedLoginFailure, InvalidContentTypeFailure
+from cyberdrop_dl.clients.errors import NoExtensionFailure, FailedLoginFailure, InvalidContentTypeFailure, \
+    PasswordProtected
 
 if TYPE_CHECKING:
     from typing import Tuple
 
     from cyberdrop_dl.managers.manager import Manager
     from cyberdrop_dl.utils.dataclasses.url_objects import ScrapeItem
 
@@ -60,14 +61,18 @@
 
         try:
             return await func(self, *args, **kwargs)
         except NoExtensionFailure:
             await log(f"Scrape Failed: {link} (No File Extension)", 40)
             await self.manager.log_manager.write_scrape_error_log(link, " No File Extension")
             await self.manager.progress_manager.scrape_stats_progress.add_failure("No File Extension")
+        except PasswordProtected:
+            await log(f"Scrape Failed: {link} (Password Protected)", 40)
+            await self.manager.log_manager.write_unsupported_urls_log(link)
+            await self.manager.progress_manager.scrape_stats_progress.add_failure("Password Protected")
         except FailedLoginFailure:
             await log(f"Scrape Failed: {link} (Failed Login)", 40)
             await self.manager.log_manager.write_scrape_error_log(link, " Failed Login")
             await self.manager.progress_manager.scrape_stats_progress.add_failure("Failed Login")
         except InvalidContentTypeFailure:
             await log(f"Scrape Failed: {link} (Invalid Content Type Received)", 40)
             await self.manager.log_manager.write_scrape_error_log(link, " Invalid Content Type Received")
@@ -99,15 +104,15 @@
     if DEBUG_VAR:
         logger_debug.log(level, message)
 
 
 async def log_debug(message: [str, Exception], level: int) -> None:
     """Simple logging function"""
     if DEBUG_VAR:
-        logger_debug.log(level, message)
+        logger_debug.log(level, message.encode('ascii', 'ignore').decode('ascii'))
 
 
 async def log_with_color(message: str, style: str, level: int) -> None:
     """Simple logging function with color"""
     logger.log(level, message)
     if DEBUG_VAR:
         logger_debug.log(level, message)
@@ -153,14 +158,16 @@
 async def get_filename_and_ext(filename: str, forum: bool = False) -> Tuple[str, str]:
     """Returns the filename and extension of a given file, throws NoExtensionFailure if there is no extension"""
     filename_parts = filename.rsplit('.', 1)
     if len(filename_parts) == 1:
         raise NoExtensionFailure()
     if filename_parts[-1].isnumeric() and forum:
         filename_parts = filename_parts[0].rsplit('-', 1)
+    if len(filename_parts[-1]) > 5:
+        raise NoExtensionFailure()
     ext = "." + filename_parts[-1].lower()
     filename = filename_parts[0][:MAX_NAME_LENGTHS['FILE']] if len(filename_parts[0]) > MAX_NAME_LENGTHS['FILE'] else filename_parts[0]
     filename = filename.strip()
     filename = filename.rstrip(".")
     filename = await sanitize(filename + ext)
     return filename, ext
```

### Comparing `cyberdrop_dl-5.2.9/pyproject.toml` & `cyberdrop_dl-5.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyberdrop-dl"
-version = "5.2.9"
+version = "5.3.1"
 description = "Bulk downloader for multiple file hosts"
 authors = ["Jules Winnfield <juleswinnfieldII@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Jules-WinnfieldX/CyberDropDownloader"
 documentation = "https://jules-winnfieldx.gitbook.io/cyberdrop-dl/"
 packages = [{include = "cyberdrop_dl"}]
```

### Comparing `cyberdrop_dl-5.2.9/PKG-INFO` & `cyberdrop_dl-5.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 5.2.9
+Version: 5.3.1
 Summary: Bulk downloader for multiple file hosts
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules Winnfield
 Author-email: juleswinnfieldII@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 5.2.9 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 5.3.1 Summary: Bulk
 downloader for multiple file hosts Home-page: https://github.com/Jules-
 WinnfieldX/CyberDropDownloader Author: Jules Winnfield Author-email:
 juleswinnfieldII@protonmail.com Requires-Python: >=3.11,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-Dist:
 aiofiles (==0.8.0) Requires-Dist: aiohttp (>=3.9.1,<4.0.0) Requires-Dist:
 aiolimiter (>=1.1.0,<2.0.0) Requires-Dist: aiosqlite (==0.17.0) Requires-Dist:
```

