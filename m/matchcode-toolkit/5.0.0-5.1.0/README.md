# Comparing `tmp/matchcode_toolkit-5.0.0.tar.gz` & `tmp/matchcode_toolkit-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchcode_toolkit-5.0.0.tar", last modified: Wed May  8 21:49:21 2024, max compression
+gzip compressed data, was "matchcode_toolkit-5.1.0.tar", last modified: Sat May 11 00:59:52 2024, max compression
```

## Comparing `matchcode_toolkit-5.0.0.tar` & `matchcode_toolkit-5.1.0.tar`

### file list

```diff
@@ -1,103 +1,107 @@
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.843298 matchcode_toolkit-5.0.0/
--rw-rw-r--   0 jono      (1000) jono      (1000)       89 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/.gitattributes
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.803299 matchcode_toolkit-5.0.0/.github/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.815299 matchcode_toolkit-5.0.0/.github/workflows/
--rw-rw-r--   0 jono      (1000) jono      (1000)      752 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/.github/workflows/docs-ci.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     2023 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/.github/workflows/pypi-release.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)      756 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/.gitignore
--rw-rw-r--   0 jono      (1000) jono      (1000)      525 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/.readthedocs.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)      104 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/AUTHORS.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     1685 2024-05-08 21:46:04.000000 matchcode_toolkit-5.0.0/CHANGELOG.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     3422 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)      217 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/MANIFEST.in
--rw-rw-r--   0 jono      (1000) jono      (1000)     1702 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/Makefile
--rw-rw-r--   0 jono      (1000) jono      (1000)      769 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/NOTICE
--rw-r--r--   0 jono      (1000) jono      (1000)     4107 2024-05-08 21:49:21.843298 matchcode_toolkit-5.0.0/PKG-INFO
--rw-rw-r--   0 jono      (1000) jono      (1000)     2481 2024-05-08 21:47:52.000000 matchcode_toolkit-5.0.0/README.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)    11357 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/apache-2.0.LICENSE
--rw-rw-r--   0 jono      (1000) jono      (1000)      971 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/azure-pipelines.yml
--rwxrwxr-x   0 jono      (1000) jono      (1000)     6328 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/configure
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.815299 matchcode_toolkit-5.0.0/docs/
--rw-rw-r--   0 jono      (1000) jono      (1000)      890 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/Makefile
--rw-rw-r--   0 jono      (1000) jono      (1000)     1071 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/make.bat
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.819299 matchcode_toolkit-5.0.0/docs/scripts/
--rwxrwxr-x   0 jono      (1000) jono      (1000)      131 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/scripts/doc8_style_check.sh
--rw-rw-r--   0 jono      (1000) jono      (1000)      124 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/scripts/sphinx_build_link_check.sh
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.819299 matchcode_toolkit-5.0.0/docs/source/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.819299 matchcode_toolkit-5.0.0/docs/source/_static/
--rw-rw-r--   0 jono      (1000) jono      (1000)      474 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/source/_static/theme_overrides.css
--rw-rw-r--   0 jono      (1000) jono      (1000)     3518 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/source/conf.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.819299 matchcode_toolkit-5.0.0/docs/source/contribute/
--rw-rw-r--   0 jono      (1000) jono      (1000)    10245 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/source/contribute/contrib_doc.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)      274 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/source/index.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     5491 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/docs/source/skeleton-usage.rst
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.807299 matchcode_toolkit-5.0.0/etc/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.823299 matchcode_toolkit-5.0.0/etc/ci/
--rw-rw-r--   0 jono      (1000) jono      (1000)     1700 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/azure-container-deb.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1753 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/azure-container-rpm.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1401 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/etc/ci/azure-posix.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1215 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/azure-win.yml
--rw-rw-r--   0 jono      (1000) jono      (1000)      257 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/install_sudo.sh
--rw-rw-r--   0 jono      (1000) jono      (1000)     8365 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/macports-ci
--rw-rw-r--   0 jono      (1000) jono      (1000)      684 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/macports-ci.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     1022 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/ci/mit.LICENSE
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.831298 matchcode_toolkit-5.0.0/etc/scripts/
--rwxrwxr-x   0 jono      (1000) jono      (1000)     3744 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/README.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     1301 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/check_thirdparty.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     9486 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/fetch_thirdparty.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     9699 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/gen_pypi_simple.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      354 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     2776 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-rw-r--   0 jono      (1000) jono      (1000)     1715 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/gen_requirements.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     2266 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/gen_requirements_dev.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      101 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/requirements.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)     4497 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      504 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     2839 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/test_utils_pypi_supported_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      773 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     6418 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_dejacode.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     6704 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_pip_compatibility_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      494 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     2850 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_pypi_supported_tags.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      741 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)     6152 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_requirements.py
--rw-rw-r--   0 jono      (1000) jono      (1000)    75931 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_thirdparty.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      608 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/etc/scripts/utils_thirdparty.py.ABOUT
--rw-rw-r--   0 jono      (1000) jono      (1000)      867 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/pyproject.toml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1617 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/requirements-dev.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)      314 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/requirements.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)     1492 2024-05-08 21:49:21.843298 matchcode_toolkit-5.0.0/setup.cfg
--rw-rw-r--   0 jono      (1000) jono      (1000)       92 2024-02-24 01:30:19.000000 matchcode_toolkit-5.0.0/setup.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.807299 matchcode_toolkit-5.0.0/src/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.831298 matchcode_toolkit-5.0.0/src/matchcode_toolkit/
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     8251 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/fingerprinting.py
--rw-rw-r--   0 jono      (1000) jono      (1000)    14288 2024-04-16 18:36:22.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/halohash.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.835298 matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     1767 2024-04-16 19:44:23.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     2321 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     1445 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit/plugin_fingerprint.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.839298 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/
--rw-r--r--   0 jono      (1000) jono      (1000)     4107 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 jono      (1000) jono      (1000)     2659 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)      200 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-03-15 00:37:28.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/not-zip-safe
--rw-rw-r--   0 jono      (1000) jono      (1000)      303 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/requires.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)       18 2024-05-08 21:49:21.000000 matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/top_level.txt
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.835298 matchcode_toolkit-5.0.0/tests/
--rw-rw-r--   0 jono      (1000) jono      (1000)     8603 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/test_fingerprinting.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     7866 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/test_halohash.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.807299 matchcode_toolkit-5.0.0/tests/testfiles/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.839298 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/
--rw-rw-r--   0 jono      (1000) jono      (1000)     4793 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
--rw-rw-r--   0 jono      (1000) jono      (1000)    55466 2024-04-16 19:44:23.000000 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate-mod.c
--rw-rw-r--   0 jono      (1000) jono      (1000)    55546 2024-04-16 19:44:23.000000 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate-mod2.c
--rw-rw-r--   0 jono      (1000) jono      (1000)    55519 2024-04-16 19:44:23.000000 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate.c
--rw-rw-r--   0 jono      (1000) jono      (1000)     5962 2024-03-14 23:41:06.000000 matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/test.json
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-08 21:49:21.839298 matchcode_toolkit-5.0.0/tests/testfiles/halohash/
--rw-rw-r--   0 jono      (1000) jono      (1000)      752 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/testfiles/halohash/500-delete-expected-results.csv
--rwxrwxr-x   0 jono      (1000) jono      (1000)      696 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/testfiles/halohash/500-replaced-expected-results.csv
--rwxrwxr-x   0 jono      (1000) jono      (1000)     3051 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/testfiles/halohash/index.js
--rw-rw-r--   0 jono      (1000) jono      (1000)     9425 2024-05-08 21:30:54.000000 matchcode_toolkit-5.0.0/tests/testfiles/halohash/words.txt
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.938300 matchcode_toolkit-5.1.0/
+-rw-rw-r--   0 jono      (1000) jono      (1000)       89 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/.gitattributes
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.918300 matchcode_toolkit-5.1.0/.github/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.922300 matchcode_toolkit-5.1.0/.github/workflows/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      752 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/.github/workflows/docs-ci.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2023 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/.github/workflows/pypi-release.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)      756 2024-05-08 21:30:54.000000 matchcode_toolkit-5.1.0/.gitignore
+-rw-rw-r--   0 jono      (1000) jono      (1000)      525 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/.readthedocs.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)      104 2024-03-14 23:41:06.000000 matchcode_toolkit-5.1.0/AUTHORS.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1802 2024-05-11 00:48:25.000000 matchcode_toolkit-5.1.0/CHANGELOG.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3422 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/CODE_OF_CONDUCT.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)      217 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/MANIFEST.in
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1702 2024-03-14 23:41:06.000000 matchcode_toolkit-5.1.0/Makefile
+-rw-rw-r--   0 jono      (1000) jono      (1000)      769 2024-03-14 23:41:06.000000 matchcode_toolkit-5.1.0/NOTICE
+-rw-r--r--   0 jono      (1000) jono      (1000)     4098 2024-05-11 00:59:52.938300 matchcode_toolkit-5.1.0/PKG-INFO
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2472 2024-05-11 00:53:45.000000 matchcode_toolkit-5.1.0/README.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)    11357 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/apache-2.0.LICENSE
+-rw-rw-r--   0 jono      (1000) jono      (1000)      971 2024-03-14 23:41:06.000000 matchcode_toolkit-5.1.0/azure-pipelines.yml
+-rwxrwxr-x   0 jono      (1000) jono      (1000)     6328 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/configure
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.922300 matchcode_toolkit-5.1.0/docs/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      890 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/docs/Makefile
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1071 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/docs/make.bat
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.922300 matchcode_toolkit-5.1.0/docs/scripts/
+-rwxrwxr-x   0 jono      (1000) jono      (1000)      131 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/docs/scripts/doc8_style_check.sh
+-rw-rw-r--   0 jono      (1000) jono      (1000)      124 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/docs/scripts/sphinx_build_link_check.sh
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.922300 matchcode_toolkit-5.1.0/docs/source/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.922300 matchcode_toolkit-5.1.0/docs/source/_static/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      474 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/docs/source/_static/theme_overrides.css
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3518 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/docs/source/conf.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.922300 matchcode_toolkit-5.1.0/docs/source/contribute/
+-rw-rw-r--   0 jono      (1000) jono      (1000)    10245 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/docs/source/contribute/contrib_doc.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)      274 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/docs/source/index.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     5491 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/docs/source/skeleton-usage.rst
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.918300 matchcode_toolkit-5.1.0/etc/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.926300 matchcode_toolkit-5.1.0/etc/ci/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1700 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/ci/azure-container-deb.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1753 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/ci/azure-container-rpm.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1401 2024-05-08 21:30:54.000000 matchcode_toolkit-5.1.0/etc/ci/azure-posix.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1215 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/ci/azure-win.yml
+-rw-rw-r--   0 jono      (1000) jono      (1000)      257 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/ci/install_sudo.sh
+-rw-rw-r--   0 jono      (1000) jono      (1000)     8365 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/ci/macports-ci
+-rw-rw-r--   0 jono      (1000) jono      (1000)      684 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/ci/macports-ci.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1022 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/ci/mit.LICENSE
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.930300 matchcode_toolkit-5.1.0/etc/scripts/
+-rwxrwxr-x   0 jono      (1000) jono      (1000)     3744 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/README.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1301 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/check_thirdparty.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     9486 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/fetch_thirdparty.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     9699 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/gen_pypi_simple.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      354 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2776 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1715 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/gen_requirements.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2266 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/gen_requirements_dev.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      101 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/requirements.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4497 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      504 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2839 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      773 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     6418 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/utils_dejacode.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     6704 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/utils_pip_compatibility_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      494 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2850 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/utils_pypi_supported_tags.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      741 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)     6152 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/utils_requirements.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)    75931 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/utils_thirdparty.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      608 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/etc/scripts/utils_thirdparty.py.ABOUT
+-rw-rw-r--   0 jono      (1000) jono      (1000)      867 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/pyproject.toml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1617 2024-03-14 23:41:06.000000 matchcode_toolkit-5.1.0/requirements-dev.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)      314 2024-03-14 23:41:06.000000 matchcode_toolkit-5.1.0/requirements.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1494 2024-05-11 00:59:52.938300 matchcode_toolkit-5.1.0/setup.cfg
+-rw-rw-r--   0 jono      (1000) jono      (1000)       92 2024-02-24 01:30:19.000000 matchcode_toolkit-5.1.0/setup.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.930300 matchcode_toolkit-5.1.0/src/
+-rwxr--r--   0 jono      (1000) jono      (1000)     6148 2024-05-10 21:54:34.000000 matchcode_toolkit-5.1.0/src/.DS_Store
+-rwxr--r--   0 jono      (1000) jono      (1000)     4096 2024-05-10 21:54:34.000000 matchcode_toolkit-5.1.0/src/._.DS_Store
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.930300 matchcode_toolkit-5.1.0/src/matchcode_toolkit/
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     8233 2024-05-11 00:48:14.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit/fingerprinting.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)    14288 2024-04-16 18:36:22.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit/halohash.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.930300 matchcode_toolkit-5.1.0/src/matchcode_toolkit/pipelines/
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2024-03-14 23:41:06.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit/pipelines/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1767 2024-04-16 19:44:23.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2321 2024-03-14 23:41:06.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1637 2024-05-11 00:48:14.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit/plugin_fingerprint.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.934300 matchcode_toolkit-5.1.0/src/matchcode_toolkit.egg-info/
+-rw-r--r--   0 jono      (1000) jono      (1000)     4098 2024-05-11 00:59:52.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2770 2024-05-11 00:59:52.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-05-11 00:59:52.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)      202 2024-05-11 00:59:52.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2024-05-11 00:59:52.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit.egg-info/not-zip-safe
+-rw-rw-r--   0 jono      (1000) jono      (1000)      303 2024-05-11 00:59:52.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)       18 2024-05-11 00:59:52.000000 matchcode_toolkit-5.1.0/src/matchcode_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.934300 matchcode_toolkit-5.1.0/tests/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     8603 2024-05-08 21:30:54.000000 matchcode_toolkit-5.1.0/tests/test_fingerprinting.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     7866 2024-05-08 21:30:54.000000 matchcode_toolkit-5.1.0/tests/test_halohash.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1675 2024-05-11 00:48:14.000000 matchcode_toolkit-5.1.0/tests/test_plugin_fingerprinting.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.934300 matchcode_toolkit-5.1.0/tests/testfiles/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.934300 matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4793 2024-03-14 23:41:06.000000 matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
+-rw-rw-r--   0 jono      (1000) jono      (1000)    55466 2024-04-16 19:44:23.000000 matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting/inflate-mod.c
+-rw-rw-r--   0 jono      (1000) jono      (1000)    55546 2024-04-16 19:44:23.000000 matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting/inflate-mod2.c
+-rw-rw-r--   0 jono      (1000) jono      (1000)    55519 2024-04-16 19:44:23.000000 matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting/inflate.c
+-rw-rw-r--   0 jono      (1000) jono      (1000)     5962 2024-03-14 23:41:06.000000 matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting/test.json
+-rw-rw-r--   0 jono      (1000) jono      (1000)     5227 2024-05-11 00:48:14.000000 matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting-expected.json
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2024-05-11 00:59:52.934300 matchcode_toolkit-5.1.0/tests/testfiles/halohash/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      752 2024-05-08 21:30:54.000000 matchcode_toolkit-5.1.0/tests/testfiles/halohash/500-delete-expected-results.csv
+-rwxrwxr-x   0 jono      (1000) jono      (1000)      696 2024-05-08 21:30:54.000000 matchcode_toolkit-5.1.0/tests/testfiles/halohash/500-replaced-expected-results.csv
+-rwxrwxr-x   0 jono      (1000) jono      (1000)     3051 2024-05-08 21:30:54.000000 matchcode_toolkit-5.1.0/tests/testfiles/halohash/index.js
+-rw-rw-r--   0 jono      (1000) jono      (1000)     9425 2024-05-08 21:30:54.000000 matchcode_toolkit-5.1.0/tests/testfiles/halohash/words.txt
```

### Comparing `matchcode_toolkit-5.0.0/.github/workflows/docs-ci.yml` & `matchcode_toolkit-5.1.0/.github/workflows/docs-ci.yml`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/.github/workflows/pypi-release.yml` & `matchcode_toolkit-5.1.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/.gitignore` & `matchcode_toolkit-5.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/.readthedocs.yml` & `matchcode_toolkit-5.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/CHANGELOG.rst` & `matchcode_toolkit-5.1.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 Changelog
 =========
 
+v5.1.0
+------
+
+*2024-05-10* -- Update scancode-toolkit fingerprint plugin to get file fingerprints for text files.
+
 v5.0.0
------
+------
 
 *2024-04-30* -- Update file fingerprint to include number of ngrams hashed in it.
 
 v4.1.0
 ------
 
 *2024-04-15* -- Add new functions to compute fingerprints on text resources for approximate file matching (https://github.com/nexB/matchcode-toolkit/issues/5)
```

### Comparing `matchcode_toolkit-5.0.0/CODE_OF_CONDUCT.rst` & `matchcode_toolkit-5.1.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/Makefile` & `matchcode_toolkit-5.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/NOTICE` & `matchcode_toolkit-5.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/PKG-INFO` & `matchcode_toolkit-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchcode-toolkit
-Version: 5.0.0
+Version: 5.1.0
 Summary: matchcode-toolkit
 Home-page: https://github.com/nexB/matchcode-toolkit
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: matchcode,ScanCode.io,open source
 Classifier: Development Status :: 5 - Production/Stable
@@ -76,17 +76,17 @@
   pip install matchcode_toolkit-*-py3-none-any.whl
 
 
 Usage
 -----
 
 MatchCode toolkit provides the ``--fingerprint`` option for ScanCode toolkit.
-This is a post-scan plugin that adds the fields
-``directory_content_fingerprint`` and ``directory_structure_fingerprint`` to
-Resources and computes those values for directories.
+This is a scan plugin that adds the fields
+``directory_content_fingerprint``, ``directory_structure_fingerprint``, and
+``halo1`` to Resources and computes those values.
 ::
 
   scancode --info --fingerprint <scan target location> --json-pp <output location>
 
 
 MatchCode toolkit provides the ``scan_and_fingerprint_package`` and
 ``fingerprint_codebase`` pipelines for ScanCode.io.
```

### Comparing `matchcode_toolkit-5.0.0/README.rst` & `matchcode_toolkit-5.1.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,17 @@
   pip install matchcode_toolkit-*-py3-none-any.whl
 
 
 Usage
 -----
 
 MatchCode toolkit provides the ``--fingerprint`` option for ScanCode toolkit.
-This is a post-scan plugin that adds the fields
-``directory_content_fingerprint`` and ``directory_structure_fingerprint`` to
-Resources and computes those values for directories.
+This is a scan plugin that adds the fields
+``directory_content_fingerprint``, ``directory_structure_fingerprint``, and
+``halo1`` to Resources and computes those values.
 ::
 
   scancode --info --fingerprint <scan target location> --json-pp <output location>
 
 
 MatchCode toolkit provides the ``scan_and_fingerprint_package`` and
 ``fingerprint_codebase`` pipelines for ScanCode.io.
```

### Comparing `matchcode_toolkit-5.0.0/apache-2.0.LICENSE` & `matchcode_toolkit-5.1.0/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/azure-pipelines.yml` & `matchcode_toolkit-5.1.0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/configure` & `matchcode_toolkit-5.1.0/configure`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/docs/Makefile` & `matchcode_toolkit-5.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/docs/make.bat` & `matchcode_toolkit-5.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/docs/source/conf.py` & `matchcode_toolkit-5.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/docs/source/contribute/contrib_doc.rst` & `matchcode_toolkit-5.1.0/docs/source/contribute/contrib_doc.rst`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/docs/source/skeleton-usage.rst` & `matchcode_toolkit-5.1.0/docs/source/skeleton-usage.rst`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/ci/azure-container-deb.yml` & `matchcode_toolkit-5.1.0/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/ci/azure-container-rpm.yml` & `matchcode_toolkit-5.1.0/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/ci/azure-posix.yml` & `matchcode_toolkit-5.1.0/etc/ci/azure-posix.yml`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/ci/azure-win.yml` & `matchcode_toolkit-5.1.0/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/ci/macports-ci` & `matchcode_toolkit-5.1.0/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/ci/macports-ci.ABOUT` & `matchcode_toolkit-5.1.0/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/ci/mit.LICENSE` & `matchcode_toolkit-5.1.0/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/README.rst` & `matchcode_toolkit-5.1.0/etc/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/check_thirdparty.py` & `matchcode_toolkit-5.1.0/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/fetch_thirdparty.py` & `matchcode_toolkit-5.1.0/etc/scripts/fetch_thirdparty.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/gen_pypi_simple.py` & `matchcode_toolkit-5.1.0/etc/scripts/gen_pypi_simple.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/gen_pypi_simple.py.NOTICE` & `matchcode_toolkit-5.1.0/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/gen_requirements.py` & `matchcode_toolkit-5.1.0/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/gen_requirements_dev.py` & `matchcode_toolkit-5.1.0/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/test_utils_pip_compatibility_tags.py` & `matchcode_toolkit-5.1.0/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/test_utils_pypi_supported_tags.py` & `matchcode_toolkit-5.1.0/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `matchcode_toolkit-5.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/utils_dejacode.py` & `matchcode_toolkit-5.1.0/etc/scripts/utils_dejacode.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/utils_pip_compatibility_tags.py` & `matchcode_toolkit-5.1.0/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/utils_pypi_supported_tags.py` & `matchcode_toolkit-5.1.0/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `matchcode_toolkit-5.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/utils_requirements.py` & `matchcode_toolkit-5.1.0/etc/scripts/utils_requirements.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/utils_thirdparty.py` & `matchcode_toolkit-5.1.0/etc/scripts/utils_thirdparty.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/etc/scripts/utils_thirdparty.py.ABOUT` & `matchcode_toolkit-5.1.0/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/pyproject.toml` & `matchcode_toolkit-5.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/requirements-dev.txt` & `matchcode_toolkit-5.1.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/setup.cfg` & `matchcode_toolkit-5.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 	sphinx-reredirects >= 0.1.2
 	doc8>=0.11.2
 	sphinx-autobuild
 	sphinx-rtd-dark-mode>=1.3.0
 	sphinx-copybutton
 
 [options.entry_points]
-scancode_post_scan = 
-	fingerprint = matchcode_toolkit.plugin_fingerprint:Fingerprint
+scancode_scan = 
+	fingerprint = matchcode_toolkit.plugin_fingerprint:FingerprintScanner
 scancodeio_pipelines = 
 	fingerprint_codebase = matchcode_toolkit.pipelines.fingerprint_codebase:FingerprintCodebase
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `matchcode_toolkit-5.0.0/src/matchcode_toolkit/fingerprinting.py` & `matchcode_toolkit-5.1.0/src/matchcode_toolkit/fingerprinting.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     from typecode.contenttype import get_type
 
     # Do not process `location` if it's not a text file
     ft = get_type(location)
     if not (filetype.is_file(location) and ft.is_text):
         return {}
 
-    with open(location, encoding='utf-8') as f:
+    with open(location) as f:
         content = f.read()
 
     file_fingerprint = create_file_fingerprint(
         content,
         ngram_length=ngram_length
     )
     return dict(
```

### Comparing `matchcode_toolkit-5.0.0/src/matchcode_toolkit/halohash.py` & `matchcode_toolkit-5.1.0/src/matchcode_toolkit/halohash.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py` & `matchcode_toolkit-5.1.0/src/matchcode_toolkit/pipelines/fingerprint_codebase.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py` & `matchcode_toolkit-5.1.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/src/matchcode_toolkit/plugin_fingerprint.py` & `matchcode_toolkit-5.1.0/src/matchcode_toolkit/plugin_fingerprint.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,39 +6,43 @@
 # See https://github.com/nexB/scancode-toolkit for support or download.
 # See https://aboutcode.org for more information about nexB OSS projects.
 #
 
 import attr
 
 from commoncode.cliutils import PluggableCommandLineOption
-from commoncode.cliutils import POST_SCAN_GROUP
+from commoncode.cliutils import SCAN_GROUP
 from matchcode_toolkit.fingerprinting import compute_codebase_directory_fingerprints
-from plugincode.post_scan import post_scan_impl
-from plugincode.post_scan import PostScanPlugin
+from matchcode_toolkit.fingerprinting import get_file_fingerprint_hashes
+from plugincode.scan import ScanPlugin
+from plugincode.scan import scan_impl
 
 
-@post_scan_impl
-class Fingerprint(PostScanPlugin):
+@scan_impl
+class FingerprintScanner(ScanPlugin):
     resource_attributes = dict(
         directory_content_fingerprint=attr.ib(default=None, repr=False),
         directory_structure_fingerprint=attr.ib(default=None, repr=False),
+        halo1=attr.ib(default=None, repr=False),
     )
     sort_order = 6
-
     options = [
         PluggableCommandLineOption(
             (
                 '--fingerprint',
             ),
             is_flag=True,
             default=False,
-            help='Compute directory fingerprints that are used for matching',
-            help_group=POST_SCAN_GROUP,
+            help='Compute directory and resource fingerprints that are used for matching',
+            help_group=SCAN_GROUP,
             sort_order=20,
         )
     ]
 
     def is_enabled(self, fingerprint, **kwargs):
         return fingerprint
+        
+    def get_scanner(self, **kwargs):
+        return get_file_fingerprint_hashes
 
     def process_codebase(self, codebase, **kwargs):
         codebase = compute_codebase_directory_fingerprints(codebase)
```

### Comparing `matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/PKG-INFO` & `matchcode_toolkit-5.1.0/src/matchcode_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchcode-toolkit
-Version: 5.0.0
+Version: 5.1.0
 Summary: matchcode-toolkit
 Home-page: https://github.com/nexB/matchcode-toolkit
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: matchcode,ScanCode.io,open source
 Classifier: Development Status :: 5 - Production/Stable
@@ -76,17 +76,17 @@
   pip install matchcode_toolkit-*-py3-none-any.whl
 
 
 Usage
 -----
 
 MatchCode toolkit provides the ``--fingerprint`` option for ScanCode toolkit.
-This is a post-scan plugin that adds the fields
-``directory_content_fingerprint`` and ``directory_structure_fingerprint`` to
-Resources and computes those values for directories.
+This is a scan plugin that adds the fields
+``directory_content_fingerprint``, ``directory_structure_fingerprint``, and
+``halo1`` to Resources and computes those values.
 ::
 
   scancode --info --fingerprint <scan target location> --json-pp <output location>
 
 
 MatchCode toolkit provides the ``scan_and_fingerprint_package`` and
 ``fingerprint_codebase`` pipelines for ScanCode.io.
```

### Comparing `matchcode_toolkit-5.0.0/src/matchcode_toolkit.egg-info/SOURCES.txt` & `matchcode_toolkit-5.1.0/src/matchcode_toolkit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 etc/scripts/utils_pip_compatibility_tags.py
 etc/scripts/utils_pip_compatibility_tags.py.ABOUT
 etc/scripts/utils_pypi_supported_tags.py
 etc/scripts/utils_pypi_supported_tags.py.ABOUT
 etc/scripts/utils_requirements.py
 etc/scripts/utils_thirdparty.py
 etc/scripts/utils_thirdparty.py.ABOUT
+src/.DS_Store
+src/._.DS_Store
 src/matchcode_toolkit/__init__.py
 src/matchcode_toolkit/fingerprinting.py
 src/matchcode_toolkit/halohash.py
 src/matchcode_toolkit/plugin_fingerprint.py
 src/matchcode_toolkit.egg-info/PKG-INFO
 src/matchcode_toolkit.egg-info/SOURCES.txt
 src/matchcode_toolkit.egg-info/dependency_links.txt
@@ -68,14 +70,16 @@
 src/matchcode_toolkit.egg-info/requires.txt
 src/matchcode_toolkit.egg-info/top_level.txt
 src/matchcode_toolkit/pipelines/__init__.py
 src/matchcode_toolkit/pipelines/fingerprint_codebase.py
 src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
 tests/test_fingerprinting.py
 tests/test_halohash.py
+tests/test_plugin_fingerprinting.py
+tests/testfiles/fingerprinting-expected.json
 tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
 tests/testfiles/fingerprinting/inflate-mod.c
 tests/testfiles/fingerprinting/inflate-mod2.c
 tests/testfiles/fingerprinting/inflate.c
 tests/testfiles/fingerprinting/test.json
 tests/testfiles/halohash/500-delete-expected-results.csv
 tests/testfiles/halohash/500-replaced-expected-results.csv
```

### Comparing `matchcode_toolkit-5.0.0/tests/test_fingerprinting.py` & `matchcode_toolkit-5.1.0/tests/test_fingerprinting.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/tests/test_halohash.py` & `matchcode_toolkit-5.1.0/tests/test_halohash.py`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json` & `matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate-mod.c` & `matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting/inflate-mod.c`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate-mod2.c` & `matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting/inflate-mod2.c`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/inflate.c` & `matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting/inflate.c`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/tests/testfiles/fingerprinting/test.json` & `matchcode_toolkit-5.1.0/tests/testfiles/fingerprinting/test.json`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/tests/testfiles/halohash/500-delete-expected-results.csv` & `matchcode_toolkit-5.1.0/tests/testfiles/halohash/500-delete-expected-results.csv`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/tests/testfiles/halohash/500-replaced-expected-results.csv` & `matchcode_toolkit-5.1.0/tests/testfiles/halohash/500-replaced-expected-results.csv`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/tests/testfiles/halohash/index.js` & `matchcode_toolkit-5.1.0/tests/testfiles/halohash/index.js`

 * *Files identical despite different names*

### Comparing `matchcode_toolkit-5.0.0/tests/testfiles/halohash/words.txt` & `matchcode_toolkit-5.1.0/tests/testfiles/halohash/words.txt`

 * *Files identical despite different names*

