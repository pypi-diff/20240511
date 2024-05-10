# Comparing `tmp/pkscreener-0.44.20240509.357.tar.gz` & `tmp/pkscreener-0.44.20240510.358.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240509.357.tar", last modified: Thu May  9 21:52:33 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240510.358.tar", last modified: Fri May 10 23:02:03 2024, max compression
```

## Comparing `pkscreener-0.44.20240509.357.tar` & `pkscreener-0.44.20240510.358.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 21:52:33.167768 pkscreener-0.44.20240509.357/
--rw-rw-rw-   0        0        0     1086 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-09 21:52:33.167768 pkscreener-0.44.20240509.357/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 21:52:33.152162 pkscreener-0.44.20240509.357/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 21:52:33.167768 pkscreener-0.44.20240509.357/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    26895 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    10741 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    30554 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11375 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23429 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21859 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18443 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119820 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    53283 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82527 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-09 21:52:22.000000 pkscreener-0.44.20240509.357/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   128576 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/globals.py
--rw-rw-rw-   0        0        0      872 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    49802 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    28594 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-09 21:52:33.152162 pkscreener-0.44.20240509.357/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-09 21:52:33.000000 pkscreener-0.44.20240509.357/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-09 21:52:33.000000 pkscreener-0.44.20240509.357/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 21:52:33.000000 pkscreener-0.44.20240509.357/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-09 21:52:33.000000 pkscreener-0.44.20240509.357/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-09 21:52:33.000000 pkscreener-0.44.20240509.357/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-09 21:52:33.000000 pkscreener-0.44.20240509.357/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-09 21:52:33.167768 pkscreener-0.44.20240509.357/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-09 21:47:47.000000 pkscreener-0.44.20240509.357/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:02:03.347568 pkscreener-0.44.20240510.358/
+-rw-rw-rw-   0        0        0     1086 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-10 23:02:03.363195 pkscreener-0.44.20240510.358/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 23:02:03.331948 pkscreener-0.44.20240510.358/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:02:03.347568 pkscreener-0.44.20240510.358/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26790 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11236 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    30554 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11667 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21948 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18597 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119820 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    55267 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83095 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-10 23:01:53.000000 pkscreener-0.44.20240510.358/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   129897 2024-05-10 22:57:46.000000 pkscreener-0.44.20240510.358/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      884 2024-05-10 22:57:47.000000 pkscreener-0.44.20240510.358/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    51603 2024-05-10 22:57:47.000000 pkscreener-0.44.20240510.358/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    30137 2024-05-10 22:57:47.000000 pkscreener-0.44.20240510.358/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:02:03.347568 pkscreener-0.44.20240510.358/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-10 23:02:03.000000 pkscreener-0.44.20240510.358/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-10 23:02:03.000000 pkscreener-0.44.20240510.358/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 23:02:03.000000 pkscreener-0.44.20240510.358/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-10 23:02:03.000000 pkscreener-0.44.20240510.358/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-10 23:02:03.000000 pkscreener-0.44.20240510.358/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-10 23:02:03.000000 pkscreener-0.44.20240510.358/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-10 23:02:03.363195 pkscreener-0.44.20240510.358/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-10 22:57:47.000000 pkscreener-0.44.20240510.358/setup.py
```

### Comparing `pkscreener-0.44.20240509.357/LICENSE` & `pkscreener-0.44.20240510.358/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/LICENSE-Others` & `pkscreener-0.44.20240510.358/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/PKG-INFO` & `pkscreener-0.44.20240510.358/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240509.357
+Version: 0.44.20240510.358
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240509.357.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240510.358.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.356/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.357/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.356/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.357/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.356/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.357/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240509.357/README.md` & `pkscreener-0.44.20240510.358/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.356/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.357/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.356/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.357/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.356/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.357/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/__init__.py` & `pkscreener-0.44.20240510.358/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/ConfigManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self.logger = None
         self.showPastStrategyData = False
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
         self.maxDashboardWidgetsPerRow = 3
-        self.maxNumResultRowsInMonitor = 2
+        self.maxNumResultRowsInMonitor = 3
         self.calculatersiintraday = False
         self.defaultMonitorOptions = ""#"X:12:9:2.5,|X:0:5:0:40:i 1m,X:12:27,X:12:28,X:12:23,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:2,X:12:24,X:12:12:i 5m,X:12:13:i 1m"
 
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
@@ -151,15 +151,15 @@
             parser.set("config", "shuffle", "y" if self.shuffleEnabled else "n")
             parser.set("config", "cacheStockData", "y" if self.cacheEnabled else "n")
             parser.set("config", "onlyStageTwoStocks", "y" if self.stageTwo else "n")
             parser.set("config", "useEMA", "y" if self.useEMA else "n")
             parser.set(
                 "config", "showunknowntrends", "y" if self.showunknowntrends else "n"
             )
-            parser.set("config", "logsEnabled", "y" if self.logsEnabled else "n")
+            parser.set("config", "logsEnabled", "y" if (self.logsEnabled or "PKDevTools_Default_Log_Level" in os.environ.keys()) else "n")
             parser.set("config", "enablePortfolioCalculations", "y" if self.enablePortfolioCalculations else "n")
             parser.set("config", "showPastStrategyData", "y" if self.showPastStrategyData else "n")
             parser.set("config", "calculatersiintraday", "y" if self.calculatersiintraday else "n")
             parser.set("config", "generalTimeout", str(self.generalTimeout))
             parser.set("config", "defaultIndex", str(self.defaultIndex))
             parser.set("config", "longTimeout", str(self.longTimeout))
             parser.set("config", "maxNetworkRetryCount", str(self.maxNetworkRetryCount))
@@ -167,15 +167,15 @@
             parser.set("config", "maxBacktestWindow", str(self.maxBacktestWindow))
             parser.set("config", "morninganalysiscandlenumber", str(self.morninganalysiscandlenumber))
             parser.set("config", "morninganalysiscandleduration", self.morninganalysiscandleduration)
             parser.set("config", "minimumVolume", str(self.minVolume))
             parser.set("config", "backtestPeriodFactor", str(self.backtestPeriodFactor))
             parser.set("config", "maxDashboardWidgetsPerRow", str(self.maxDashboardWidgetsPerRow))
             parser.set("config", "maxNumResultRowsInMonitor", str(self.maxNumResultRowsInMonitor))
-            parser.set("config", "defaultMonitorOptions", "X:12:9:2.5,|X:0:5:0:40:i 1m,X:12:27,X:12:28,X:12:23,X:12:7:3:.01:1,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:2,X:12:24,X:12:12:i 5m,X:12:13:i 1m")
+            parser.set("config", "defaultMonitorOptions", str(self.defaultMonitorOptions))
             try:
                 fp = open("pkscreener.ini", "w")
                 parser.write(fp)
                 fp.close()
                 if showFileCreatedText:
                     OutputControls().printOutput(
                         colorText.BOLD
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/MarketMonitor.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     def __init__(self,monitors=[], maxNumResultsPerRow=3,maxNumColsInEachResult=6,maxNumRowsInEachResult=10,maxNumResultRowsInMonitor=2):
         super(MarketMonitor, self).__init__()
         if monitors is not None and len(monitors) > 0:
             
             self.monitors = monitors[:maxNumResultRowsInMonitor*maxNumResultsPerRow]
             self.monitorIndex = 0
             self.monitorPositions = {}
+            self.monitorResultStocks = {}
             # self.monitorNames = {}
             # We are going to present the dataframes in a 3x3 matrix with limited set of columns
             rowIndex = 0
             colIndex = 0
             self.maxNumResultRowsInMonitor = maxNumResultRowsInMonitor
             self.maxNumRowsInEachResult = maxNumRowsInEachResult
             self.maxNumColsInEachResult = maxNumColsInEachResult
@@ -73,14 +74,23 @@
             self.monitorIndex += 1
             if self.monitorIndex > maxIndex:
                 self.monitorIndex = 0
         except:
             pass
         return option
 
+    def saveMonitorResultStocks(self, results_df):
+        if results_df is None or results_df.empty:
+            prevOutput_results = "NONE"
+        else:
+            prevOutput_results = results_df[~results_df.index.duplicated(keep='first')]
+            prevOutput_results = prevOutput_results.index
+            prevOutput_results = ",".join(prevOutput_results)
+        self.monitorResultStocks[str(self.monitorIndex)] = prevOutput_results
+
     def refresh(self, screen_df:pd.DataFrame=None, screenOptions=None, chosenMenu=None, dbTimestamp="", telegram=False):
         highlightRows = []
         highlightCols = []
         if screen_df is None or screen_df.empty:
             return
 
         screen_monitor_df = screen_df.copy()
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/OtaUpdater.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import subprocess
 import sys
 from datetime import timedelta
 
 from PKDevTools.classes import Archiver
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.log import default_logger
+from PKDevTools.classes.OutputControls import OutputControls
 
 import pkscreener.classes.ConfigManager as ConfigManager
 import pkscreener.classes.Fetcher as Fetcher
 from pkscreener.classes import VERSION
 
 class OTAUpdater:
     developmentVersion = "d"
@@ -182,22 +183,22 @@
                 if float(now_components[2]) < float(version_components[2]):
                     prod_update = True
                 elif float(now_components[2]) == float(version_components[2]):
                     if float(now_components[3]) < float(version_components[3]):
                         prod_update = True
             if prod_update:
                 if skipDownload:
-                    print(
+                    OutputControls().printOutput(
                         colorText.BOLD
                         + colorText.GREEN
                         + f"    [+] A software update (v{tag} [{size} MB]) is available. Check out with the menu option U."
                         + colorText.END
                     )
                     return
-                print(
+                OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
                     + "[+] What's New in this Update?\n"
                     + colorText.END
                     + colorText.GREEN
                     + OTAUpdater.showWhatsNew()
                     + colorText.END
@@ -220,68 +221,68 @@
                             OTAUpdater.updateForWindows(OTAUpdater.checkForUpdate.url)
                         elif "Darwin" in platform.system():
                             OTAUpdater.updateForMac(OTAUpdater.checkForUpdate.url)
                         else:
                             OTAUpdater.updateForLinux(OTAUpdater.checkForUpdate.url)
                     except Exception as e:  # pragma: no cover
                         default_logger().debug(e, exc_info=True)
-                        print(
+                        OutputControls().printOutput(
                             colorText.BOLD
                             + colorText.WARN
                             + "[+] Error occured while updating!"
                             + colorText.END
                         )
                         raise (e)
             elif not prod_update and not skipDownload:
                 if tag.lower() == VERSION.lower():
-                    print(
+                    OutputControls().printOutput(
                         colorText.BOLD
                         + colorText.GREEN
                         + (
                             "[+] No new update available. You have the latest version (v%s) !"
                             % VERSION
                         )
                         + colorText.END
                     )
                 else:
-                    print(
+                    OutputControls().printOutput(
                         colorText.BOLD
                         + colorText.FAIL
                         + (
                             "[+] This version (v%s) is in Development mode and unreleased!"
                             % VERSION
                         )
                         + colorText.END
                     )
                     return OTAUpdater.developmentVersion
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             if OTAUpdater.checkForUpdate.url is not None:
-                print(e)
-                print(
+                OutputControls().printOutput(e)
+                OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.BLUE
                     + (
                         "[+] Download update manually from %s\n"
                         % OTAUpdater.checkForUpdate.url
                     )
                     + colorText.END
                 )
             else:
                 OTAUpdater.checkForUpdate.url = (
                     "[+] No exe/bin/run file as an update available!"
                 )
             if resp is not None and resp.json()["message"] == "Not Found":
-                print(
+                OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.FAIL
                     + OTAUpdater.checkForUpdate.url
                     + colorText.END
                 )
-            print(e)
-            print(
+            OutputControls().printOutput(e)
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] Failure while checking update!"
                 + colorText.END
             )
         return
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 from pkscreener.classes.ScreeningStatistics import ScreeningStatistics
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes import Archiver
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes.PKPickler import PKPicklerDB
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.log import default_logger
+from PKDevTools.classes.OutputControls import OutputControls
+
 STD_ENCODING=sys.stdout.encoding if sys.stdout is not None else 'utf-8'
 
 class PKDailyStockDataDB(SingletonMixin, metaclass=SingletonType):
     def __init__(self,fileName=None):
         super(PKDailyStockDataDB, self).__init__()
         self.pickler = PKPicklerDB(fileName=fileName)
 
@@ -97,21 +99,21 @@
         # Ensure that the intraday_stock_data_<date>.pkl file exists
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=True)
         if not exists:
             savedPeriod = PKMarketOpenCloseAnalyser.configManager.period
             savedDuration = PKMarketOpenCloseAnalyser.configManager.duration
             PKMarketOpenCloseAnalyser.configManager.period = "1d"
             PKMarketOpenCloseAnalyser.configManager.duration = "1m"
-            print(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
-            print(f"[+] {colorText.GREEN}Trying to download {cache_file}{colorText.END}. Please wait ...")
+            OutputControls().printOutput(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
+            OutputControls().printOutput(f"[+] {colorText.GREEN}Trying to download {cache_file}{colorText.END}. Please wait ...")
             Utility.tools.loadStockData({},PKMarketOpenCloseAnalyser.configManager,False,'Y',False,False,None,isIntraday=True)
             exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=True)
             if not exists:
-                print(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
-                print(f"[+] Please run {colorText.FAIL}pkscreener{colorText.END}{colorText.GREEN} -a Y -e -d -i 1m{colorText.END} and then run this menu option again.")
+                OutputControls().printOutput(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
+                OutputControls().printOutput(f"[+] Please run {colorText.FAIL}pkscreener{colorText.END}{colorText.GREEN} -a Y -e -d -i 1m{colorText.END} and then run this menu option again.")
                 input("Press any key to continue...")
             PKMarketOpenCloseAnalyser.configManager.period = savedPeriod
             PKMarketOpenCloseAnalyser.configManager.duration = savedDuration
         copyFilePath = os.path.join(Archiver.get_user_outputs_dir(), f"copy_{cache_file}")
         srcFilePath = os.path.join(Archiver.get_user_outputs_dir(), cache_file)
         try:
             if os.path.exists(copyFilePath) and exists:
@@ -122,23 +124,23 @@
             pass
         return exists, cache_file
 
     def ensureDailyStockDataExists():
         # Ensure that the stock_data_<date>.pkl file exists
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=False)
         if not exists:
-            print(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
+            OutputControls().printOutput(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
         # We should download a fresh copy anyways because we may have altered the existing copy in
         # the previous run. -- !!!! Not required if we saved at the end of last operation !!!!
-            print(f"[+] {colorText.GREEN}Trying to download {cache_file}{colorText.END}. Please wait ...")
+            OutputControls().printOutput(f"[+] {colorText.GREEN}Trying to download {cache_file}{colorText.END}. Please wait ...")
             Utility.tools.loadStockData({},PKMarketOpenCloseAnalyser.configManager,False,'Y',False,False,None,isIntraday=False,forceRedownload=True)
             exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=False)
             if not exists:
-                print(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
-                print(f"[+] Please run {colorText.FAIL}pkscreener{colorText.END}{colorText.GREEN} -a Y -e -d{colorText.END} and then run this menu option again.")
+                OutputControls().printOutput(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
+                OutputControls().printOutput(f"[+] Please run {colorText.FAIL}pkscreener{colorText.END}{colorText.GREEN} -a Y -e -d{colorText.END} and then run this menu option again.")
                 input("Press any key to continue...")
         copyFilePath = os.path.join(Archiver.get_user_outputs_dir(), f"copy_{cache_file}")
         srcFilePath = os.path.join(Archiver.get_user_outputs_dir(), cache_file)
         try:
             if os.path.exists(copyFilePath) and exists:
                 shutil.copy(copyFilePath,srcFilePath) # copy is the saved source of truth
             if not os.path.exists(copyFilePath) and exists: # Let's make a copy of the original one
@@ -211,15 +213,15 @@
                                     "Low":min(df["Low"]),"Close":PKMarketOpenCloseAnalyser.getMorningClose(df),
                                     "Adj Close":df["Adj Close"][-1],"Volume":sum(df["Volume"])}
                     tradingDate = df.index[-1] #PKDateUtilities.tradingDate()
                     timestamp = datetime.datetime.strptime(tradingDate.strftime("%Y-%m-%d %H:%M:%S"),"%Y-%m-%d %H:%M:%S")
                     df = pd.DataFrame([combinedCandle], columns=df.columns, index=[timestamp])
                     morningIntradayCandle[stock] = df.to_dict("split")
             except Exception as e:
-                print(f"{stock}:    {e}")
+                OutputControls().printOutput(f"{stock}:    {e}")
                 continue
         return morningIntradayCandle
 
     def getMorningOpen(df):
         open = df["Open"][0]
         index = 0
         while open is np.nan and index < len(df):
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/PKScanRunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.PKGitFolderDownloader import downloadFolder
 from PKDevTools.classes.PKMultiProcessorClient import PKMultiProcessorClient
 from PKDevTools.classes.multiprocessing_logging import LogQueueReader
 from PKDevTools.classes.SuppressOutput import SuppressOutput
+# from PKDevTools.classes.FunctionTimeouts import exit_after
 
 from pkscreener.classes.StockScreener import StockScreener
 from pkscreener.classes.CandlePatterns import CandlePatterns
 from pkscreener.classes.ConfigManager import parser, tools
 from PKDevTools.classes.OutputControls import OutputControls
 from PKNSETools.PKIntraDay import Intra_Day
 import pkscreener.classes.Fetcher as Fetcher
@@ -319,18 +320,18 @@
                         None,
                         None
                         # (cache_file if (exists and menuOption in ["C"]) else None),
                         # (sec_cache_file if (exists and menuOption in ["C"]) else None),
                     )
                     for _ in range(totalConsumers)
                 ]
-        if executeOption == 29: # Intraday Bid/Ask, for which we need to fetch data from NSE instead of yahoo
-            intradayFetcher = Intra_Day("SBINEQN") # This will initialise the cookies etc.
-            for consumer in consumers:
-                consumer.intradayNSEFetcher = intradayFetcher
+        # if executeOption == 29: # Intraday Bid/Ask, for which we need to fetch data from NSE instead of yahoo
+        intradayFetcher = Intra_Day("SBINEQN") # This will initialise the cookies etc.
+        for consumer in consumers:
+            consumer.intradayNSEFetcher = intradayFetcher
         PKScanRunner.startWorkers(consumers)
         return tasks_queue,results_queue,consumers,logging_queue
 
     def startWorkers(consumers):
         try:
             from pytest_cov.embed import cleanup_on_signal, cleanup_on_sigterm
         except ImportError:
@@ -393,14 +394,15 @@
         PKScanRunner.results_queue = None
         PKScanRunner.scr = None
         PKScanRunner.consumers = None
 
     def shutdown(frame, signum):
         OutputControls().printOutput("Shutting down for test coverage")
 
+    # @exit_after(60)
     def runScan(userPassedArgs,testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df, *otherArgs,resultsReceivedCb=None):
         queueCounter = 0
         counter = 0
         shouldContinue = True
         lastNonNoneResult = None
         while numStocks:
             if counter == 0 and numStocks > 0:
@@ -421,18 +423,19 @@
                             numStocksPerIteration
                             * queueCounter :
                         ],
                         tasks_queue,
                         True,
                         userPassedArgs
                     )
+            numStocks -= 1
             result = results_queue.get()
             if result is not None:
                 lastNonNoneResult = result
-            numStocks -= 1
+            
             if resultsReceivedCb is not None:
                 shouldContinue, backtest_df = resultsReceivedCb(result, numStocks, backtest_df,*otherArgs)
             counter += 1
             # If it's being run under unit testing, let's wrap up if we find at least 1
             # stock or if we've already tried screening through 5% of the list.
             if (not shouldContinue) or (testing and counter >= int(numStocksPerIteration * 0.05)):
                 break
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/Pktalib.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,48 +27,49 @@
 
 import numpy as np
 
 warnings.simplefilter("ignore", DeprecationWarning)
 warnings.simplefilter("ignore", FutureWarning)
 import pandas as pd
 from PKDevTools.classes.ColorText import colorText
+from PKDevTools.classes.OutputControls import OutputControls
 
 from pkscreener import Imports
 
 if Imports["talib"]:
     try:
         import talib
     except:
-        print(
+        OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] 'TA-Lib' library is not installed. For best results, please install 'TA-Lib'! You may wish to follow instructions from\n[+] https://github.com/pkjmesra/PKScreener/"
                 + colorText.END
             )
         try:
             import pandas_ta as talib
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] TA-Lib is not installed. Falling back on pandas_ta.\n[+] For full coverage(candle patterns), you may wish to follow instructions from\n[+] https://github.com/ta-lib/ta-lib-python"
                 + colorText.END
             )
         except:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] pandas_ta is not installed. Falling back on pandas_ta also failed.\n[+] For full coverage(candle patterns), you may wish to follow instructions from\n[+] https://github.com/ta-lib/ta-lib-python"
                 + colorText.END
             )
             pass
         pass
 else:
     try:
         import pandas_ta as talib
-        print(
+        OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + "[+] TA-Lib is not installed. Falling back on pandas_ta.\n[+] For full coverage(candle patterns), you may wish to follow instructions from\n[+] https://github.com/ta-lib/ta-lib-python"
             + colorText.END
         )
         sleep(3)
     except Exception:  # pragma: no cover
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/StockScreener.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,21 +114,67 @@
                 raise StockDataEmptyException(f"Data is None: {data}")
             
             bidGreaterThanAsk = False
             bidAskRatio = 0
             if executeOption == 29:
                 hostRef.intradayNSEFetcher.symbol = stock.upper()
                 priceData = hostRef.intradayNSEFetcher.price_order_info()
-                totalBid = priceData["BidQty"].iloc[0]
-                totalAsk = priceData["AskQty"].iloc[0]
-                if totalBid > totalAsk and \
-                    priceData["LTP"].iloc[0] < float(priceData["UprCP"].iloc[0]) and \
-                    priceData["LTP"].iloc[0] > float(priceData["LwrCP"].iloc[0]):
-                    bidGreaterThanAsk = True
-                    bidAskRatio = round(totalBid/totalAsk,1) if totalAsk > 0 else 0
+                if priceData is not None:
+                    try:
+                        totalBid = priceData["BidQty"].iloc[0]
+                    except:
+                        totalBid = 0
+                        pass
+                    try:
+                        totalAsk = priceData["AskQty"].iloc[0]
+                    except:
+                        totalAsk = 0
+                        pass
+                    try:
+                        lwrCP = float(priceData["LwrCP"].iloc[0])
+                    except:
+                        lwrCP = 0
+                        pass
+                    try:
+                        uprCP = float(priceData["UprCP"].iloc[0])
+                    except:
+                        uprCP = 0
+                        pass
+                    try:
+                        vwap = float(priceData["VWAP"].iloc[0])
+                    except:
+                        vwap = 0
+                        pass
+                    try:
+                        dayVola = float(priceData["DayVola"].iloc[0])
+                    except:
+                        dayVola = 0
+                        pass
+                    try:
+                        delPercent = priceData["Del(%)"].iloc[0]
+                    except:
+                        delPercent = 0
+                        pass
+                    try:
+                        ltp = priceData["LTP"].iloc[0]
+                    except:
+                        ltp = 0
+                        pass
+                    
+                    bidAskSimulate = userArgs is not None and userArgs.simulate is not None and "BidAsk" in userArgs.simulate.keys()
+                    if (totalBid > totalAsk and \
+                        ltp < uprCP and \
+                        ltp > lwrCP) or bidAskSimulate:
+                        bidGreaterThanAsk = True
+                        bidAskRatio = round(totalBid/totalAsk,1) if totalAsk > 0 else (0 if not bidAskSimulate else 3)
+                        bidAskBuildupDict = {"BidQty":totalBid,"AskQty":totalAsk,"LwrCP":lwrCP,"UprCP":uprCP,"VWAP":vwap,"DayVola":dayVola,"Del(%)":delPercent}
+                        screeningDictionary.update(bidAskBuildupDict)
+                        saveDictionary.update(bidAskBuildupDict)
+                    else:
+                        raise ScreeningStatistics.EligibilityConditionNotMet("Bid/Ask Eligibility Not met.")
                 else:
                     raise ScreeningStatistics.EligibilityConditionNotMet("Bid/Ask Eligibility Not met.")
             # hostRef.default_logger.info(f"Will pre-process data:\n{data.tail(10)}")
             fullData, processedData, data = self.getCleanedDataForDuration(backtestDuration, portfolio, screeningDictionary, saveDictionary, configManager, screener, data)
             if "RUNNER" not in os.environ.keys() and backtestDuration == 0 and configManager.calculatersiintraday:
                 if (intraday_data is not None and not intraday_data.empty):
                     intraday_fullData, intraday_processedData = screener.preprocessData(
@@ -185,16 +231,17 @@
                 raise StockDataEmptyException("Empty processedData")
             
             with SuppressOutput(suppress_stderr=(logLevel==logging.NOTSET), suppress_stdout=(not (printCounter or testbuild))):
                 self.updateStock(stock, screeningDictionary, saveDictionary, executeOption, exchangeName)
                 
                 self.performBasicLTPChecks(executeOption, screeningDictionary, saveDictionary, fullData, configManager, screener, exchangeName)
                 hasMinVolumeRatio = self.performBasicVolumeChecks(executeOption, volumeRatio, screeningDictionary, saveDictionary, processedData, configManager, screener)
-                if (bidGreaterThanAsk and not hasMinVolumeRatio) or (bidGreaterThanAsk and bidAskRatio < 2):
-                    raise ScreeningStatistics.EligibilityConditionNotMet("Bid/Ask Eligibility Not met.")
+                if bidGreaterThanAsk:
+                    if not hasMinVolumeRatio or bidAskRatio < 2:
+                        raise ScreeningStatistics.EligibilityConditionNotMet("Bid/Ask Eligibility Not met.")
                 isConfluence = False
                 isInsideBar = 0
                 isMaReversal = 0
                 isIpoBase = False
                 isMaSupport = False
                 isLorentzian = False
                 isVCP = False
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 """
 import sys
 from PKDevTools.classes.ColorText import colorText
+from PKDevTools.classes.OutputControls import OutputControls
 
 import pkscreener.classes.ConfigManager as ConfigManager
 import pkscreener.classes.Utility as Utility
 
 class UserMenuChoicesHandler:
     configManager = ConfigManager.tools()
     configManager.getConfig(ConfigManager.parser)
@@ -39,15 +40,15 @@
         intraday = intradayConfig or argsIntraday
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday)
         if exists:
             shouldReplace = Utility.tools.promptFileExists(
                 cache_file=cache_file, defaultAnswer=defaultAnswer
             )
             if shouldReplace == "N":
-                print(
+                OutputControls().printOutput(
                     cache_file
                     + colorText.END
                     + " already exists. Exiting as user chose not to replace it!"
                 )
                 sys.exit(0)
             else:
                 pattern = f"{'intraday_' if intraday else ''}stock_data_*.pkl"
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/Utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,48 +88,57 @@
     # task = PKTask("Nifty 50 Market Status",MarketStatus().getMarketStatus)
     lngStatus = MarketStatus().marketStatus
     # scheduleTasks(tasksList=[task])
     if lngStatus == "":
         lngStatus = MarketStatus().getMarketStatus(exchangeSymbol="^IXIC" if configManager.defaultIndex == 15 else "^NSEI")
     return (lngStatus +"\n") if lngStatus is not None else "\n"
 
-art = colorText.GREEN + artText + colorText.END + f" | {marketStatus()}"
+art = colorText.GREEN + f"{getArtText()}\nv{VERSION}" + colorText.END + f" | {marketStatus()}"
 
 lastScreened = os.path.join(
     Archiver.get_user_outputs_dir(), "last_screened_results.pkl"
 )
 
 # Class for managing misc and utility methods
 
 class tools:
-    def clearScreen(userArgs=None,clearAlways=False):
+    def clearScreen(userArgs=None,clearAlways=False,forceTop=False):
         if "RUNNER" in os.environ.keys() or (userArgs is not None and userArgs.prodbuild):
             if userArgs is not None and userArgs.v:
                 os.environ["RUNNER"]="LOCAL_RUN_SCANNER"
             return
         elif (userArgs is not None and userArgs.runintradayanalysis):
             return
         if clearAlways or OutputControls().enableMultipleLineOutput:
             if platform.system() == "Windows":
                 try:
                     os.system('color 0f') # sets the background to black with white forerground
                 except:
                     pass
-                os.system("cls")
+                if clearAlways:
+                    os.system("cls")
             elif "Darwin" in platform.system():
-                os.system("clear")
+                if clearAlways:
+                    os.system("clear")
+                # default_logger().debug("Darwin does not work for setting background")
             else:
                 try:
                     os.system('setterm -background black -foreground white -store')
                 except:
                     pass
-                os.system("clear")
+                if clearAlways:
+                    os.system("clear")
+            OutputControls().moveCursorToStartPosition()
         try:
+            if forceTop and OutputControls().lines == 0:
+                OutputControls().lines = 9
+                OutputControls().moveCursorToStartPosition()
+                
             if clearAlways or OutputControls().enableMultipleLineOutput:
-                art = colorText.GREEN + artText + colorText.END + f" | {marketStatus()}"
+                art = colorText.GREEN + f"{getArtText()}\nv{VERSION}" + colorText.END + f" | {marketStatus()}"
                 OutputControls().printOutput(art.encode('utf-8').decode(STD_ENCODING), enableMultipleLineOutput=True)
         except Exception as e:# pragma: no cover
             default_logger().debug(e, exc_info=True)
             pass
 
     # Print about developers and repository
     def showDevInfo(defaultAnswer=None):
@@ -1513,31 +1522,31 @@
         try:
             if os.path.isfile(files[0]) and os.path.isfile(files[1]):
                 pkl = joblib.load(files[1])
                 if Imports["keras"]:
                     try:
                         import keras
                     except:
-                        print("This installation might not work well, especially for NIFTY prediction. Please install 'keras' library on your machine!")
-                        print(
+                        OutputControls().printOutput("This installation might not work well, especially for NIFTY prediction. Please install 'keras' library on your machine!")
+                        OutputControls().printOutput(
                                 colorText.BOLD
                                 + colorText.FAIL
                                 + "[+] 'Keras' library is not installed. You may wish to follow instructions from\n[+] https://github.com/pkjmesra/PKScreener/"
                                 + colorText.END
                             )
                         pass
                 model = keras.models.load_model(files[0]) if Imports["keras"] else None
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             os.remove(files[0])
             os.remove(files[1])
             if not retrial:
                 tools.getNiftyModel(retrial=True)
         if model is None:
-            print(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] 'Keras' library is not installed. Prediction failed! You may wish to follow instructions from\n[+] https://github.com/pkjmesra/PKScreener/"
                 + colorText.END
             )
         return model, pkl
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/WorkflowManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 """
 import os
 from PKDevTools.classes.Telegram import get_secrets
+from PKDevTools.classes.OutputControls import OutputControls
 
 import pkscreener.classes.ConfigManager as ConfigManager
 from pkscreener.classes.Fetcher import screenerStockDataFetcher
 
 configManager = ConfigManager.tools()
 
 
@@ -81,14 +82,14 @@
         "Authorization": f"Bearer {ghp_token}",
         "Content-Type": "application/json",
     }
 
     fetcher = screenerStockDataFetcher(configManager)
     resp = fetcher.postURL(url, data=data, headers=headers)
     if resp.status_code == 204:
-        print(f"Workflow {workflow_name} Triggered!")
+        OutputControls().printOutput(f"Workflow {workflow_name} Triggered!")
     else:
-        print(f"Something went wrong while triggering {workflow_name}")
+        OutputControls().printOutput(f"Something went wrong while triggering {workflow_name}")
     return resp
 
 
 # resp = run_workflow("B_12_1","-1001785195297","B:12:1")
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/classes/keys.py` & `pkscreener-0.44.20240510.358/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/courbd.ttf` & `pkscreener-0.44.20240510.358/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/pkscreener/globals.py` & `pkscreener-0.44.20240510.358/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,27 +705,27 @@
     # Print Level 1 menu options
     selectedMenu = initExecution(menuOption=menuOption)
     menuOption = selectedMenu.menuKey
     if menuOption in ["M", "D", "I", "L"]:
         launcher = sys.argv[0]
         launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
         if menuOption in ["M"]:
-            print(f"{colorText.GREEN}Launching PKScreener in monitoring mode. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -m 'X'{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit monitoring mode.{colorText.END}")
+            OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener in monitoring mode. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -m 'X'{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit monitoring mode.{colorText.END}")
             sleep(2)
             os.system(f"{launcher} -a Y -m 'X'")
         elif menuOption in ["D"]:
-            print(f"{colorText.GREEN}Launching PKScreener to Download daily OHLC data. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -d{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
+            OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener to Download daily OHLC data. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -d{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
             sleep(2)
             os.system(f"{launcher} -a Y -e -d")
         elif menuOption in ["I"]:
-            print(f"{colorText.GREEN}Launching PKScreener to Download intraday OHLC data. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -d -i 1m{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
+            OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener to Download intraday OHLC data. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -d -i 1m{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
             sleep(2)
             os.system(f"{launcher} -a Y -e -d -i 1m")
         elif menuOption in ["L"]:
-            print(f"{colorText.GREEN}Launching PKScreener to collect logs. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -l{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
+            OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener to collect logs. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -l{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
             sleep(2)
             os.system(f"{launcher} -a Y -l")
         sys.exit(0)
     elif menuOption in ["X", "T", "E", "Y", "U", "H", "C"]:
         # Print Level 2 menu options
         menuOption, indexOption, executeOption, selectedChoice = getScannerMenuChoices(
             testBuild or testing,
@@ -782,16 +782,17 @@
                 userOption = "37"  # NoFilter
                 pass
             except Exception as e:# pragma: no cover
                 default_logger().debug(e, exc_info=True)
                 pass
         userOption = userOption.upper()
         if userOption == "M":
-                # Go back to the caller. It will show the console menu again.
-                return None, None
+            Utility.tools.clearScreen(forceTop=True)
+            # Go back to the caller. It will show the console menu again.
+            return None, None
         elif userOption == "Z":
             handleExitRequest(userOption)
             return None, None
         
         if userOption == "S":
             OutputControls().printOutput(
                 colorText.GREEN
@@ -840,14 +841,15 @@
     else:
         OutputControls().printOutput("Not implemented yet! Try selecting a different option.")
         sleep(3)
         return None, None
 
     handleMenu_XBG(menuOption, indexOption, executeOption)
     if indexOption == "M" or executeOption == "M":
+        Utility.tools.clearScreen(forceTop=True)
         # Go back to the caller. It will show the console menu again.
         return None, None
     listStockCodes = handleRequestForSpecificStocks(options, indexOption)
     handleExitRequest(executeOption)
     if executeOption is None:
         executeOption = 0
     executeOption = int(executeOption)
@@ -1338,15 +1340,15 @@
                             addendum=shareable_strings[1],
                             addendumLabel="NSE Stocks giving bonus:",
                             backtestSummary=shareable_strings[2],
                             backtestDetail="",
                             summaryLabel = "NSE Stocks with corporate action type stock split:",
                             detailLabel = None,
                             )
-                else:
+                elif "|" not in userPassedArgs.options:
                     printNotifySaveScreenedResults(
                         screenResults,
                         saveResults,
                         selectedChoice,
                         menuChoiceHierarchy,
                         testing,
                         user=user,
@@ -1750,14 +1752,15 @@
             menuChoiceHierarchy
             + f'>{level3_X_PopularStocks_MenuDict[selectedChoice["3"]].strip()}'
         )
     intraday = "(Intraday)" if (userPassedArgs is not None and userPassedArgs.intraday) or configManager.isIntradayConfig() else ""
     menuChoiceHierarchy = f"{menuChoiceHierarchy}{intraday}"
     global nValueForMenu
     menuChoiceHierarchy = menuChoiceHierarchy.replace("N-",f"{nValueForMenu}-")
+    Utility.tools.clearScreen()
     OutputControls().printOutput(
         colorText.BOLD
         + colorText.FAIL
         + "[+] You chose: "
         + menuChoiceHierarchy
         + colorText.END
     )
@@ -2158,14 +2161,29 @@
         ]
     for col in saveResults.keys():
         saveResults = saveResults[
             saveResults[col].astype(str).str.contains("Unknown") == False
         ]
     return screenResults, saveResults
 
+# def apply_df_style(x):
+#     red = 'color: red'
+#     noColor = '' 
+#     green = 'color: green'
+#     #compare columns
+#     mask_green_bid = x['BidQty'] > x['AskQty']
+#     mask_red_bid = x['BidQty'] <= x['AskQty']
+#     mask_green_vwap = x['VWAP'] >= x['LTP']
+#     #DataFrame with same index and columns names as original filled empty strings
+#     df1 =  pd.DataFrame(noColor, index=x.index, columns=x.columns)
+#     #modify values of df1 column by boolean mask
+#     df1.loc[mask_green_bid, 'BidQty'] = green
+#     df1.loc[mask_red_bid, 'AskQty'] = red
+#     df1.loc[mask_green_vwap, 'VWAP'] = green
+#     return df1
 
 def runScanners(
     menuOption,
     items,
     tasks_queue,
     results_queue,
     numStocks,
@@ -2221,27 +2239,30 @@
                 progressbar.text(
                     colorText.BOLD
                     + colorText.GREEN
                     + f"{'Remaining' if userPassedArgs.download else ('Found' if menuOption in ['X'] else 'Analysed')} {len(lstscreen) if not userPassedArgs.download else processedCount} {'Stocks' if menuOption in ['X'] else 'Records'}"
                     + colorText.END
                 )
                 if result is not None:
-                    if len(lstscreen) > 0 and userPassedArgs is not None and userPassedArgs.options.split(":")[2] in ["29"]:
+                    if not userPassedArgs.monitor and len(lstscreen) > 0 and userPassedArgs is not None and userPassedArgs.options.split(":")[2] in ["29"]:
                         scr_df = pd.DataFrame(lstscreen)
-                        columns = ["Stock","%Chng","LTP","Volume"]
-                        scr_df = scr_df[columns]
+                        existingColumns = ["Stock","%Chng","LTP","Volume"]
+                        newColumns = ["BidQty","AskQty","LwrCP","UprCP","VWAP","DayVola","Del(%)"]
+                        existingColumns.extend(newColumns)
+                        scr_df = scr_df[existingColumns]
+                        scr_df.sort_values(by=["Volume","BidQty"], ascending=False, inplace=True)
                         tabulated_results = colorText.miniTabulator().tb.tabulate(
                                 scr_df,
                                 headers="keys",
                                 showindex=False,
                                 tablefmt=colorText.No_Pad_GridFormat,
                                 maxcolwidths=Utility.tools.getMaxColumnWidths(scr_df)
                             )
                         tableLength = 2*len(lstscreen)+5
-                        print('\n'+tabulated_results)
+                        OutputControls().printOutput('\n'+tabulated_results)
                         sys.stdout.write(f"\x1b[{tableLength}A")  # cursor up one line
                 if keyboardInterruptEventFired:
                     return False, backtest_df
                 return not ((testing and len(lstscreen) >= 1) or len(lstscreen) >= max_allowed), backtest_df
             otherArgs = (menuOption, backtestPeriod, result, lstscreen, lstsave)
             backtest_df, result =PKScanRunner.runScan(userPassedArgs,testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df,*otherArgs,resultsReceivedCb=processResultsCallback)
 
@@ -2467,19 +2488,21 @@
                 caption = f"{caption.replace('&','n')}"
             send_document(document_filePath, caption, userID=user)
             # Breather for the telegram API to be able to send the document
             sleep(2)
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
     if user is not None:
-        # Send an update to dev channel
-        send_message(
-            "Responded back to userId:{0} with {1}.{2}".format(user, caption, message),
-            userID="-1001785195297",
-        )
+        channel_userID="-1001785195297"
+        if user != channel_userID:
+            # Send an update to dev channel
+            send_message(
+                "Responded back to userId:{0} with {1}.{2}".format(user, caption, message),
+                userID="-1001785195297",
+            )
 
 
 def sendTestStatus(screenResults, label, user=None):
     msg = "<b>SUCCESS</b>" if (screenResults is not None and len(screenResults) >= 1) else "<b>FAIL</b>"
     sendMessageToTelegramChannel(
         message=f"{msg}: Found {len(screenResults) if screenResults is not None else 0} Stocks for {label}", user=user
     )
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240510.358/pkscreener/pkscreener.ini`

 * *Files 2% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 maxnetworkretrycount = 10
 backtestperiod = 120
 maxbacktestwindow = 30
 morninganalysiscandlenumber = 25
 morninganalysiscandleduration = 1m
 minimumvolume = 10000
 backtestperiodfactor = 1
-defaultmonitoroptions = X:12:9:2.5,|X:0:5:0:40:i 1m,X:12:27,X:12:28,X:12:23,X:12:7:3:.01:1,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:2,X:12:24,X:12:12:i 5m,X:12:13:i 1m
+defaultmonitoroptions = X:12:9:2.5,|X:0:5:0:40:i 1m,X:12:27,X:12:28,X:12:23,X:12:7:3:.01:1,|{1}X:0:29:,X:12:6:3,X:12:6:8,X:12:6:7:1,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:2,X:12:24,X:12:12:i 5m,X:12:13:i 1m
 maxDashboardWidgetsPerRow = 3
 maxNumResultRowsInMonitor = 2
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240510.358/pkscreener/pkscreenerbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 from datetime import datetime
 from time import sleep
 from telegram import __version__ as TG_VER
 from telegram.constants import ParseMode
 
 start_time = datetime.now()
 MINUTES_5_IN_SECONDS = 300
+OWNER_USER = "Itsonlypk"
 
 from PKDevTools.classes.Telegram import get_secrets
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.ColorText import colorText
 from pkscreener.classes.MenuOptions import MenuRenderStyle, menu, menus
 from pkscreener.classes.WorkflowManager import run_workflow
 from pkscreener.globals import showSendConfigInfo, showSendHelpInfo
@@ -102,15 +103,15 @@
 ONE, TWO, THREE, FOUR = range(4)
 
 m0 = menus()
 m1 = menus()
 m2 = menus()
 m3 = menus()
 
-TOP_LEVEL_SCANNER_MENUS = ["X", "B", "MI"]
+TOP_LEVEL_SCANNER_MENUS = ["X", "B", "MI","DV"]
 TOP_LEVEL_SCANNER_SKIP_MENUS = ["M", "S", "G", "C", "T", "D", "I", "E", "U", "L", "Z"]
 INDEX_SKIP_MENUS = ["W","E","M","Z","0","2","3","4","6","7","9","10","13"]
 SCANNER_SKIP_MENUS_1_TO_6 = ["0","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_7_TO_12 = ["0","1","2","3","4","5","6","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_13_TO_18 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_19_TO_25 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","22","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_26_TO_31 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","30","42","M","Z"]
@@ -118,15 +119,15 @@
 SCANNER_MENUS_WITH_SUBMENU_SUPPORT = ["6", "7", "21"]
 
 INDEX_COMMANDS_SKIP_MENUS_SCANNER = ["W", "E", "M", "Z"]
 INDEX_COMMANDS_SKIP_MENUS_BACKTEST = ["W", "E", "M", "Z", "N", "0", "15"]
 UNSUPPORTED_COMMAND_MENUS =["22","30","42","M","Z"]
 SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29"]
 
-async def start(update: Update, context: ContextTypes.DEFAULT_TYPE, updatedResults=None, monitorIndex=0) -> int:
+async def start(update: Update, context: ContextTypes.DEFAULT_TYPE, updatedResults=None, monitorIndex=0,chosenBotMenuOption="") -> int:
     """Send message on `/start`."""
     updateCarrier = None
     if update is None:
         return
     else:
         if update.callback_query is not None:
             updateCarrier = update.callback_query
@@ -140,14 +141,17 @@
     # Build InlineKeyboard where each button has a displayed text
     # and a string as callback_data
     # The keyboard is a list of button rows, where each row is in turn
     # a list (hence `[[...]]`).
     mns = m0.renderForMenu(asList=True)
     if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys()) or sys.argv[0].endswith(".py"):
         mns.append(menu().create(f"MI_{monitorIndex}", "Int. Monitor", 2))
+    if user.username == OWNER_USER:
+        mns.append(menu().create(f"DV_0", ("Enbl" if not configManager.logsEnabled else "Dsbl"), 2))
+
     inlineMenus = []
     for mnu in mns:
         if mnu.menuKey[0:2] in TOP_LEVEL_SCANNER_MENUS:
             inlineMenus.append(
                 InlineKeyboardButton(
                     mnu.menuText.split("(")[0],
                     callback_data="C" + str(mnu.menuKey),
@@ -157,22 +161,21 @@
     reply_markup = InlineKeyboardMarkup(keyboard)
     cmds = m0.renderForMenu(
         selectedMenu=None,
         skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
-    chosenBotMenuOption = ""
     if updatedResults is None:
         cmdText = ""
         for cmd in cmds:
             cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
         menuText = f"Welcome {user.first_name}, {(user.username)}! Please choose a menu option by selecting a button from below.\n\nYou can also explore a wide variety of all other scanners by typing in \n{cmdText}\n\n OR just use the buttons below to choose."
     else:
-        chosenBotMenuOption = "Int. Monitor"
+        chosenBotMenuOption = f"{chosenBotMenuOption}\nInt. Monitor. MonitorIndex:{monitorIndex}"
         menuText = updatedResults
     # Send message with text and appended InlineKeyboard
     if update.callback_query is not None:
         await sendUpdatedMenu(
             menuText=menuText, update=update, context=context, reply_markup=reply_markup, replaceWhiteSpaces=(updatedResults is None)
         )
     elif update.message is not None:
@@ -240,14 +243,45 @@
     except Exception as e:
         result_outputs = "Hmm...It looks like you caught us taking a break! Try again later :-)"
         logger.info(f"{launcher} -a Y -m 'X' -p --telegram could not be launched")
         logger.info(e)
         pass
     return result_outputs, filePath
 
+async def XDevModeHandler(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
+    """Show new choice of buttons"""
+    query = update.callback_query
+    data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G").replace("CMI", "MI").replace("CDV","DV")
+    if data[0:2] not in TOP_LEVEL_SCANNER_MENUS:
+        return start(update, context)
+    if data.startswith("DV"):
+        # Dev Mode
+        devModeIndex = int(data.split("_")[1])
+        if devModeIndex == 0:
+            if "PKDevTools_Default_Log_Level" in os.environ.keys():
+                del os.environ['PKDevTools_Default_Log_Level']
+                configManager.maxNumResultRowsInMonitor = 2
+                configManager.logsEnabled = False
+            else:
+                # Switch config file
+                configManager.maxNumResultRowsInMonitor = 3
+                configManager.logsEnabled = True
+                os.environ["PKDevTools_Default_Log_Level"] = str(logging.INFO)
+            configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
+            chosenBotMenuOption = configManager.showConfigFile(defaultAnswer='Y')
+            if monitor_proc is not None:
+                try:
+                    monitor_proc.kill()
+                except:
+                    pass
+            
+            launchIntradayMonitor()
+            await start(update, context,chosenBotMenuOption=chosenBotMenuOption)
+    return START_ROUTES
+
 async def XScanners(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     query = update.callback_query
     data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G").replace("CMI", "MI")
     if data[0:2] not in TOP_LEVEL_SCANNER_MENUS:
         return start(update, context)
     if data.startswith("MI"):
@@ -1066,14 +1100,15 @@
     conv_handler = ConversationHandler(
         entry_points=[CommandHandler("start", start)],
         states={
             START_ROUTES: [
                 CallbackQueryHandler(XScanners, pattern="^" + str("CX") + "$"),
                 CallbackQueryHandler(XScanners, pattern="^" + str("CB") + "$"),
                 CallbackQueryHandler(XScanners, pattern="^" + str("CMI_")),
+                CallbackQueryHandler(XDevModeHandler, pattern="^" + str("CDV_")),
                 # CallbackQueryHandler(XScanners, pattern="^" + str("CG") + "$"),
                 CallbackQueryHandler(Level2, pattern="^" + str("CX_")),
                 CallbackQueryHandler(Level2, pattern="^" + str("CB_")),
                 # CallbackQueryHandler(Level2, pattern="^" + str("CG_")),
                 CallbackQueryHandler(end, pattern="^" + str("CZ") + "$"),
                 CallbackQueryHandler(start, pattern="^"),
             ],
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240510.358/pkscreener/pkscreenercli.py`

 * *Files 4% similar despite different names*

```diff
@@ -384,14 +384,15 @@
         if args.barometer:
             sendGlobalMarketBarometer(userArgs=args)
         else:
             global results, resultStocks, plainResults, dbTimestamp, elapsed_time, start_time
             monitorOption_org = ""
             # args.monitor = configManager.defaultMonitorOptions
             if args.monitor:
+                configManager.getConfig(ConfigManager.parser)
                 args.answerdefault = args.answerdefault or 'Y'
                 if MarketMonitor().monitorIndex == 0:
                     dbTimestamp = PKDateUtilities.currentDateTime().strftime("%H:%M:%S")
                     elapsed_time = 0
                     if start_time is None:
                         start_time = time.time()
                     else:
@@ -408,16 +409,31 @@
                     configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
                 else:
                     # We need to switch to daily scan
                     args.intraday = None
                     configManager.toggleConfig(candleDuration='1d', clearCache=False)
                 if monitorOption.startswith("|"):
                     monitorOption = monitorOption.replace("|","")
+                    monitorOptions = monitorOption.split(":")
+                    if monitorOptions[1] != "0":
+                        monitorOptions[1] = "0"
+                        monitorOption = ":".join(monitorOptions)
                     # We need to pipe the output from previous run into the next one
-                    if resultStocks is not None:
+                    if monitorOption.startswith("{") and "}" in monitorOption:
+                        srcIndex = monitorOption.split("}")[0].split("{")[-1]
+                        monitorOption="".join(monitorOption.split("}")[1:])
+                        try:
+                            srcIndex = int(srcIndex)
+                            # Let's get the previously saved result for the monitor
+                            savedStocks = MarketMonitor().monitorResultStocks[str(srcIndex)]
+                            monitorOption = f"{monitorOption}:{savedStocks}"
+                        except:
+                            # Probably wrong (non-integer) index passed. Let's continue anyway
+                            pass
+                    elif resultStocks is not None:
                         resultStocks = ",".join(resultStocks)
                         monitorOption = f"{monitorOption}:{resultStocks}"
                 args.options = monitorOption.replace("::",":")
                 # (previousCandleDuration != configManager.duration) or 
                 if (MarketMonitor().monitorIndex == 1 and args.options is not None and plainResults is not None):
                     # Load the stock data afresh for each cycle
                     refreshStockData(args.options)
@@ -440,14 +456,16 @@
                 default_logger().debug(e, exc_info=True)
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
                 pass
             if plainResults is not None and not plainResults.empty:
                 plainResults = plainResults[~plainResults.index.duplicated(keep='first')]
                 results = results[~results.index.duplicated(keep='first')]
                 resultStocks = plainResults.index
+            if args.monitor:
+                MarketMonitor().saveMonitorResultStocks(plainResults)
             if results is not None and args.monitor and len(monitorOption_org) > 0:
                 MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy(),dbTimestamp=f"{dbTimestamp} | CycleTime:{elapsed_time}s",telegram=args.telegram)
 
 
 def pipeResults(prevOutput,args):
     nextOnes = args.options.split(";")
     if len(nextOnes) > 1:
@@ -462,14 +480,18 @@
             configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
         else:
             # We need to switch to daily scan
             args.intraday = None
             configManager.toggleConfig(candleDuration='1d', clearCache=False)
         if monitorOption.startswith("|"):
             monitorOption = monitorOption.replace("|","")
+            monitorOptions = monitorOption.split(":")
+            if monitorOptions[1] != "0":
+                monitorOptions[1] = "0"
+                monitorOption = ":".join(monitorOptions)
             # We need to pipe the output from previous run into the next one
             if prevOutput is not None and not prevOutput.empty:
                 prevOutput_results = prevOutput[~prevOutput.index.duplicated(keep='first')]
                 prevOutput_results = prevOutput_results.index
                 prevOutput_results = ",".join(prevOutput_results)
                 monitorOption = f"{monitorOption}:{prevOutput_results}"
         args.options = monitorOption.replace("::",":")
@@ -493,15 +515,19 @@
 
     OutputControls(enableMultipleLineOutput=(args.monitor is None)).printOutput("",end="\r")
         
     configManager.getConfig(ConfigManager.parser)
     # configManager.restartRequestsCache()
     # args.monitor = configManager.defaultMonitorOptions
     if args.monitor is not None:
-        MarketMonitor(monitors=args.monitor.split(",") if len(args.monitor)>5 else configManager.defaultMonitorOptions.split(","),maxNumResultsPerRow=configManager.maxDashboardWidgetsPerRow)
+        MarketMonitor(monitors=args.monitor.split(",") if len(args.monitor)>5 else configManager.defaultMonitorOptions.split(","),
+                      maxNumResultsPerRow=configManager.maxDashboardWidgetsPerRow,
+                      maxNumColsInEachResult=6,
+                      maxNumRowsInEachResult=10,
+                      maxNumResultRowsInMonitor=configManager.maxNumResultRowsInMonitor)
 
     if args.log or configManager.logsEnabled:
         setupLogger(shouldLog=True, trace=args.testbuild)
         if not args.prodbuild and args.answerdefault is None:
             input("Press <Enter> to continue...")
     else:
         if "PKDevTools_Default_Log_Level" in os.environ.keys():
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240510.358/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240509.357
+Version: 0.44.20240510.358
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240509.357.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240510.358.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.356/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.357/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.356/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.357/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.356/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240509.357/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240509.357/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240510.358/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240509.357/setup.py` & `pkscreener-0.44.20240510.358/setup.py`

 * *Files identical despite different names*

