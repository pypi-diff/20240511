# Comparing `tmp/ytmusicapi-1.7.0.tar.gz` & `tmp/ytmusicapi-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusicapi-1.7.0.tar", last modified: Sat May  4 11:36:37 2024, max compression
+gzip compressed data, was "ytmusicapi-1.7.1.tar", last modified: Sat May 11 16:45:32 2024, max compression
```

## Comparing `ytmusicapi-1.7.0.tar` & `ytmusicapi-1.7.1.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/workflows/docsbuild.yml
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/workflows/pdm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/docs/source/setup/
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/setup/browser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/setup/headers_auth.json.example
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/setup/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/setup/oauth.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)    61554 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/pdm.lock
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.008805 ytmusicapi-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.008805 ytmusicapi-1.7.0/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/auth/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/auth/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.008805 ytmusicapi-1.7.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   226650 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/data/2024_03_get_album.json
--rw-r--r--   0 runner    (1001) docker     (127)  1039226 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/data/2024_03_get_playlist.json
--rw-r--r--   0 runner    (1001) docker     (127)  1004367 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/data/2024_03_get_playlist_public.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.012805 ytmusicapi-1.7.0/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.012805 ytmusicapi-1.7.0/tests/setup/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/setup/setup_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/test.example.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/test_ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.012805 ytmusicapi-1.7.0/ytmusicapi/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/continuations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:36.996805 ytmusicapi-1.7.0/ytmusicapi/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/base.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:36.996805 ytmusicapi-1.7.0/ytmusicapi/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/de/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:36.996805 ytmusicapi-1.7.0/ytmusicapi/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/en/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/en/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:36.996805 ytmusicapi-1.7.0/ytmusicapi/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/es/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/hi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/it/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/nl/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/nl/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/update_mo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/update_po.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/ytmusicapi/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39178 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)    17492 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    20529 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/ytmusicapi/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/albums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/ytmusicapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.624338 ytmusicapi-1.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/workflows/docsbuild.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/workflows/pdm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-11 16:45:32.620338 ytmusicapi-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/docs/source/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/setup/browser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/setup/headers_auth.json.example
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/setup/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/setup/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    61554 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 16:45:32.624338 ytmusicapi-1.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.604338 ytmusicapi-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.604338 ytmusicapi-1.7.1/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/auth/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/auth/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.604338 ytmusicapi-1.7.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   226650 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/data/2024_03_get_album.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1039226 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/data/2024_03_get_playlist.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1004367 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/data/2024_03_get_playlist_public.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.608338 ytmusicapi-1.7.1/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.608338 ytmusicapi-1.7.1/tests/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/setup/setup_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/test.example.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/test_ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.608338 ytmusicapi-1.7.1/ytmusicapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/continuations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.592338 ytmusicapi-1.7.1/ytmusicapi/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ar/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.592338 ytmusicapi-1.7.1/ytmusicapi/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/de/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.592338 ytmusicapi-1.7.1/ytmusicapi/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/en/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/en/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/es/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/es/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/fr/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/hi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/hi/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/it/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/it/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ja/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ko/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/nl/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/nl/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/pt/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ru/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/tr/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/update_mo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/update_po.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ur/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.620338 ytmusicapi-1.7.1/ytmusicapi/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39178 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17492 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20529 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12101 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.620338 ytmusicapi-1.7.1/ytmusicapi/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/albums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.620338 ytmusicapi-1.7.1/ytmusicapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/top_level.txt
```

### Comparing `ytmusicapi-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ytmusicapi-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `ytmusicapi-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/.github/dependabot.yml` & `ytmusicapi-1.7.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/.github/workflows/coverage.yml` & `ytmusicapi-1.7.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/.github/workflows/docsbuild.yml` & `ytmusicapi-1.7.1/.github/workflows/docsbuild.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/.github/workflows/lint.yml` & `ytmusicapi-1.7.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/.github/workflows/pythonpublish.yml` & `ytmusicapi-1.7.1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/CONTRIBUTING.rst` & `ytmusicapi-1.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/LICENSE` & `ytmusicapi-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/PKG-INFO` & `ytmusicapi-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.7.0
+Version: 1.7.1
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ytmusicapi-1.7.0/README.rst` & `ytmusicapi-1.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/docs/Makefile` & `ytmusicapi-1.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/docs/make.bat` & `ytmusicapi-1.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/docs/source/conf.py` & `ytmusicapi-1.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/docs/source/faq.rst` & `ytmusicapi-1.7.1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/docs/source/index.rst` & `ytmusicapi-1.7.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/docs/source/reference.rst` & `ytmusicapi-1.7.1/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/docs/source/setup/browser.rst` & `ytmusicapi-1.7.1/docs/source/setup/browser.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/docs/source/usage.rst` & `ytmusicapi-1.7.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/pdm.lock` & `ytmusicapi-1.7.1/pdm.lock`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/pyproject.toml` & `ytmusicapi-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/README.rst` & `ytmusicapi-1.7.1/tests/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/auth/test_browser.py` & `ytmusicapi-1.7.1/tests/auth/test_browser.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/auth/test_oauth.py` & `ytmusicapi-1.7.1/tests/auth/test_oauth.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/conftest.py` & `ytmusicapi-1.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/data/2024_03_get_album.json` & `ytmusicapi-1.7.1/tests/data/2024_03_get_album.json`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/data/2024_03_get_playlist.json` & `ytmusicapi-1.7.1/tests/data/2024_03_get_playlist.json`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/data/2024_03_get_playlist_public.json` & `ytmusicapi-1.7.1/tests/data/2024_03_get_playlist_public.json`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/mixins/test_browsing.py` & `ytmusicapi-1.7.1/tests/mixins/test_browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/mixins/test_explore.py` & `ytmusicapi-1.7.1/tests/mixins/test_explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/mixins/test_library.py` & `ytmusicapi-1.7.1/tests/mixins/test_library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/mixins/test_playlists.py` & `ytmusicapi-1.7.1/tests/mixins/test_playlists.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,12 +103,13 @@
             source_playlist="OLAK5uy_nvjTE32aFYdFN7HCyMv3cGqD3wqBb4Jow",
             duplicates=True,
         )
         assert response["status"] == "STATUS_SUCCEEDED", "Adding playlist item failed"
         assert len(response["playlistEditResults"]) > 0, "Adding playlist item failed"
         time.sleep(3)
         yt_brand.edit_playlist(playlist_id, addToTop=False)
+        time.sleep(3)
         playlist = yt_brand.get_playlist(playlist_id, related=True)
         assert len(playlist["tracks"]) == 46, "Getting playlist items failed"
         response = yt_brand.remove_playlist_items(playlist_id, playlist["tracks"])
         assert response == "STATUS_SUCCEEDED", "Playlist item removal failed"
         yt_brand.delete_playlist(playlist_id)
```

### Comparing `ytmusicapi-1.7.0/tests/mixins/test_podcasts.py` & `ytmusicapi-1.7.1/tests/mixins/test_podcasts.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/mixins/test_search.py` & `ytmusicapi-1.7.1/tests/mixins/test_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,50 @@
 import pytest
 
+from ytmusicapi import YTMusic
+from ytmusicapi.parsers.search import ALL_RESULT_TYPES
+
 
 class TestSearch:
     def test_search_exceptions(self, yt_auth):
         query = "edm playlist"
         with pytest.raises(Exception, match="Invalid filter provided"):
             yt_auth.search(query, filter="song")
         with pytest.raises(Exception, match="Invalid scope provided"):
             yt_auth.search(query, scope="upload")
 
     @pytest.mark.parametrize("query", ["Monekes", "qllwlwl", "heun"])
     def test_search_queries(self, yt, yt_brand, query: str) -> None:
         results = yt_brand.search(query)
         assert ["resultType" in r for r in results] == [True] * len(results)
         assert len(results) >= 10
+        assert not any(
+            artist["name"].lower() in ALL_RESULT_TYPES
+            for result in results
+            if "artists" in result
+            for artist in result["artists"]
+        )
         results = yt.search(query)
         assert len(results) >= 10
+        assert not any(
+            artist["name"].lower() in ALL_RESULT_TYPES
+            for result in results
+            if "artists" in result
+            for artist in result["artists"]
+        )
 
     def test_search_ignore_spelling(self, yt_auth):
         results = yt_auth.search("Martin Stig Andersen - Deteriation", ignore_spelling=True)
         assert len(results) > 0
 
+    def test_search_localized(self):
+        yt_local = YTMusic(language="it")
+        results = yt_local.search("ABBA")
+        assert all(result["resultType"] in ALL_RESULT_TYPES for result in results)
+
     def test_search_filters(self, yt_auth):
         query = "hip hop playlist"
         results = yt_auth.search(query, filter="songs")
         assert len(results) > 10
         assert all(item["resultType"] == "song" for item in results)
         results = yt_auth.search(query, filter="videos")
         assert len(results) > 10
```

### Comparing `ytmusicapi-1.7.0/tests/mixins/test_watch.py` & `ytmusicapi-1.7.1/tests/mixins/test_watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/setup/setup_account.py` & `ytmusicapi-1.7.1/tests/setup/setup_account.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/tests/test.example.cfg` & `ytmusicapi-1.7.1/tests/test.example.cfg`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/auth/browser.py` & `ytmusicapi-1.7.1/ytmusicapi/auth/browser.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/auth/oauth/credentials.py` & `ytmusicapi-1.7.1/ytmusicapi/auth/oauth/credentials.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/auth/oauth/models.py` & `ytmusicapi-1.7.1/ytmusicapi/auth/oauth/models.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/auth/oauth/token.py` & `ytmusicapi-1.7.1/ytmusicapi/auth/oauth/token.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/auth/types.py` & `ytmusicapi-1.7.1/ytmusicapi/auth/types.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/constants.py` & `ytmusicapi-1.7.1/ytmusicapi/constants.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/continuations.py` & `ytmusicapi-1.7.1/ytmusicapi/continuations.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/helpers.py` & `ytmusicapi-1.7.1/ytmusicapi/helpers.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/README.rst` & `ytmusicapi-1.7.1/ytmusicapi/locales/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/ar/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/ar/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/base.pot` & `ytmusicapi-1.7.1/ytmusicapi/locales/base.pot`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/de/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/de/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/de/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/en/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/en/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/es/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/es/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/es/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/fr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/fr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/hi/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/hi/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/it/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/it/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/it/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/ja/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/ja/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/ko/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/ko/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/nl/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/nl/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/nl/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/nl/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/pt/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/pt/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/ru/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/ru/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/tr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/tr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/ur/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/ur/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po` & `ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/mixins/_protocol.py` & `ytmusicapi-1.7.1/ytmusicapi/mixins/_protocol.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/mixins/_utils.py` & `ytmusicapi-1.7.1/ytmusicapi/mixins/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/mixins/browsing.py` & `ytmusicapi-1.7.1/ytmusicapi/mixins/browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/mixins/explore.py` & `ytmusicapi-1.7.1/ytmusicapi/mixins/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/mixins/library.py` & `ytmusicapi-1.7.1/ytmusicapi/mixins/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/mixins/playlists.py` & `ytmusicapi-1.7.1/ytmusicapi/mixins/playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/mixins/podcasts.py` & `ytmusicapi-1.7.1/ytmusicapi/mixins/podcasts.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/mixins/search.py` & `ytmusicapi-1.7.1/ytmusicapi/mixins/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,55 +188,51 @@
             tab_index = 0 if not scope or filter else scopes.index(scope) + 1
             results = response["contents"]["tabbedSearchResultsRenderer"]["tabs"][tab_index]["tabRenderer"][
                 "content"
             ]
         else:
             results = response["contents"]
 
-        results = nav(results, SECTION_LIST)
+        section_list = nav(results, SECTION_LIST)
 
         # no results
-        if len(results) == 1 and "itemSectionRenderer" in results:
+        if len(section_list) == 1 and "itemSectionRenderer" in section_list:
             return search_results
 
         # set filter for parser
         if filter and "playlists" in filter:
             filter = "playlists"
         elif scope == scopes[1]:
             filter = scopes[1]
 
-        for res in results:
+        for res in section_list:
             if "musicCardShelfRenderer" in res:
                 top_result = parse_top_result(
                     res["musicCardShelfRenderer"], self.parser.get_search_result_types()
                 )
                 search_results.append(top_result)
-                if results := nav(res, ["musicCardShelfRenderer", "contents"], True):
-                    category = None
-                    # category "more from youtube" is missing sometimes
-                    if "messageRenderer" in results[0]:
-                        category = nav(results.pop(0), ["messageRenderer", *TEXT_RUN_TEXT])
-                    type = None
-                else:
+                if not (shelf_contents := nav(res, ["musicCardShelfRenderer", "contents"], True)):
                     continue
+                type = category = None
+                # if "more from youtube" is present, remove it - it's not parseable
+                if "messageRenderer" in shelf_contents[0]:
+                    category = nav(shelf_contents.pop(0), ["messageRenderer", *TEXT_RUN_TEXT])
 
             elif "musicShelfRenderer" in res:
-                results = res["musicShelfRenderer"]["contents"]
-                type_filter = filter
+                shelf_contents = res["musicShelfRenderer"]["contents"]
                 category = nav(res, MUSIC_SHELF + TITLE_TEXT, True)
-                if not type_filter and scope == scopes[0]:
-                    type_filter = category
+                type_filter = filter or category
 
                 type = type_filter[:-1].lower() if type_filter else None
 
             else:
                 continue
 
             search_result_types = self.parser.get_search_result_types()
-            search_results.extend(parse_search_results(results, search_result_types, type, category))
+            search_results.extend(parse_search_results(shelf_contents, search_result_types, type, category))
 
             if filter:  # if filter is set, there are continuations
 
                 def request_func(additionalParams):
                     return self._send_request(endpoint, body, additionalParams)
 
                 def parse_func(contents):
```

### Comparing `ytmusicapi-1.7.0/ytmusicapi/mixins/uploads.py` & `ytmusicapi-1.7.1/ytmusicapi/mixins/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/mixins/watch.py` & `ytmusicapi-1.7.1/ytmusicapi/mixins/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/navigation.py` & `ytmusicapi-1.7.1/ytmusicapi/navigation.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/_utils.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,16 @@
     except ValueError:
         index = len(runs)
 
     return index
 
 
 def parse_duration(duration):
-    if duration is None:
+    # duration may be falsy or a single space: ' '
+    if not duration or not duration.strip():
         return duration
     mapped_increments = zip([1, 60, 3600], reversed(duration.split(":")))
     seconds = sum(multiplier * int(time) for multiplier, time in mapped_increments)
     return seconds
 
 
 def i18n(method):
```

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/albums.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/albums.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/browsing.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/explore.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/i18n.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/i18n.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/library.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/playlists.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/podcasts.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/podcasts.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/search.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/search.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from ._utils import *
 from .songs import *
 
+UNIQUE_RESULT_TYPES = ["artist", "playlist", "song", "video", "station", "profile", "podcast", "episode"]
+ALL_RESULT_TYPES = ["album", *UNIQUE_RESULT_TYPES]
+
 
 def get_search_result_type(result_type_local, result_types_local):
     if not result_type_local:
         return None
-    result_types = ["artist", "playlist", "song", "video", "station", "profile", "podcast", "episode"]
     result_type_local = result_type_local.lower()
     # default to album since it's labeled with multiple values ('Single', 'EP', etc.)
     if result_type_local not in result_types_local:
         result_type = "album"
     else:
-        result_type = result_types[result_types_local.index(result_type_local)]
+        result_type = UNIQUE_RESULT_TYPES[result_types_local.index(result_type_local)]
 
     return result_type
 
 
 def parse_top_result(data, search_result_types):
     result_type = get_search_result_type(nav(data, SUBTITLE), search_result_types)
     search_result = {"category": nav(data, CARD_SHELF_TITLE), "resultType": result_type}
@@ -35,15 +37,15 @@
 
     if result_type in ["song", "video", "album"]:
         search_result["videoId"] = nav(data, ["onTap", *WATCH_VIDEO_ID], True)
         search_result["videoType"] = nav(data, ["onTap", *NAVIGATION_VIDEO_TYPE], True)
 
         search_result["title"] = nav(data, TITLE_TEXT)
         runs = nav(data, ["subtitle", "runs"])
-        song_info = parse_song_runs(runs)
+        song_info = parse_song_runs(runs[2:])
         search_result.update(song_info)
 
     if result_type in ["album"]:
         search_result["browseId"] = nav(data, TITLE + NAVIGATION_BROWSE_ID, True)
 
     if result_type in ["playlist"]:
         search_result["playlistId"] = nav(data, MENU_PLAYLIST_ID)
@@ -54,22 +56,37 @@
     return search_result
 
 
 def parse_search_result(data, search_result_types, result_type, category):
     default_offset = (not result_type or result_type == "album") * 2
     search_result = {"category": category}
     video_type = nav(data, [*PLAY_BUTTON, "playNavigationEndpoint", *NAVIGATION_VIDEO_TYPE], True)
-    if not result_type and video_type:
-        result_type = "song" if video_type == "MUSIC_VIDEO_TYPE_ATV" else "video"
 
-    result_type = (
-        get_search_result_type(get_item_text(data, 1), search_result_types)
-        if not result_type
-        else result_type
-    )
+    # try to determine the result type based on the first run
+    if result_type not in ALL_RESULT_TYPES:  # i.e. localized result_type
+        result_type = get_search_result_type(get_item_text(data, 1), search_result_types)
+
+    # determine result type based on browseId
+    #  if there was no category title (i.e. for extra results in Top Result)
+    if not result_type:
+        if browse_id := nav(data, NAVIGATION_BROWSE_ID, True):
+            mapping = {
+                "VMPL": "playlist",
+                "RD": "playlist",
+                "MPLA": "artist",
+                "MPRE": "album",
+                "MPSP": "podcast",
+                "MPED": "episode",
+            }
+            result_type = next(
+                iter(type for prefix, type in mapping.items() if browse_id.startswith(prefix)), None
+            )
+        else:
+            result_type = "song" if video_type == "MUSIC_VIDEO_TYPE_ATV" else "video"
+
     search_result["resultType"] = result_type
 
     if result_type != "artist":
         search_result["title"] = get_item_text(data, 0)
 
     if result_type == "artist":
         search_result["artist"] = get_item_text(data, 0)
@@ -130,15 +147,16 @@
         search_result["videoType"] = video_type
 
     if result_type in ["song", "video", "album"]:
         search_result["duration"] = None
         search_result["year"] = None
         flex_item = get_flex_column_item(data, 1)
         runs = flex_item["text"]["runs"]
-        song_info = parse_song_runs(runs)
+        runs_offset = (len(runs[0]) == 1) * 2  # ignore the first run if it is a type specifier (like "Song")
+        song_info = parse_song_runs(runs[runs_offset:])
         search_result.update(song_info)
 
     if result_type in ["artist", "album", "playlist", "profile", "podcast"]:
         search_result["browseId"] = nav(data, NAVIGATION_BROWSE_ID, True)
 
     if result_type in ["song", "album"]:
         search_result["isExplicit"] = nav(data, BADGE_LABEL, True) is not None
```

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/songs.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/songs.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/uploads.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/uploads.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,17 @@
             ],
         )
         videoId = nav(data, [*MENU_ITEMS, 0, *MENU_SERVICE])["queueAddEndpoint"]["queueTarget"]["videoId"]
 
         title = get_item_text(data, 0)
         like = nav(data, MENU_LIKE_STATUS)
         thumbnails = nav(data, THUMBNAILS) if "thumbnail" in data else None
-        duration = get_fixed_column_item(data, 0)["text"]["runs"][0]["text"]
+        duration = None
+        if "fixedColumns" in data:
+            duration = get_fixed_column_item(data, 0)["text"]["runs"][0]["text"]
         song = {
             "entityId": entityId,
             "videoId": videoId,
             "title": title,
             "duration": duration,
             "duration_seconds": parse_duration(duration),
             "artists": parse_song_artists(data, 1),
```

### Comparing `ytmusicapi-1.7.0/ytmusicapi/parsers/watch.py` & `ytmusicapi-1.7.1/ytmusicapi/parsers/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/setup.py` & `ytmusicapi-1.7.1/ytmusicapi/setup.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi/ytmusic.py` & `ytmusicapi-1.7.1/ytmusicapi/ytmusic.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.0/ytmusicapi.egg-info/PKG-INFO` & `ytmusicapi-1.7.1/ytmusicapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.7.0
+Version: 1.7.1
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ytmusicapi-1.7.0/ytmusicapi.egg-info/SOURCES.txt` & `ytmusicapi-1.7.1/ytmusicapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

