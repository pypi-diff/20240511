# Comparing `tmp/cdflib-1.2.5.tar.gz` & `tmp/cdflib-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdflib-1.2.5.tar", last modified: Sat Mar  2 00:08:07 2024, max compression
+gzip compressed data, was "cdflib-1.2.6.tar", last modified: Tue Mar  5 22:07:13 2024, max compression
```

## Comparing `cdflib-1.2.5.tar` & `cdflib-1.2.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.310876 cdflib-1.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.298876 cdflib-1.2.5/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-02 00:07:58.000000 cdflib-1.2.5/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-02 00:07:58.000000 cdflib-1.2.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.294876 cdflib-1.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.298876 cdflib-1.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-02 00:07:58.000000 cdflib-1.2.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-02 00:07:58.000000 cdflib-1.2.5/.github/workflows/pypi-build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-02 00:07:58.000000 cdflib-1.2.5/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-02 00:07:58.000000 cdflib-1.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-02 00:07:58.000000 cdflib-1.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-02 00:07:58.000000 cdflib-1.2.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-02 00:07:58.000000 cdflib-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-02 00:07:58.000000 cdflib-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-02 00:08:07.310876 cdflib-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-02 00:07:58.000000 cdflib-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.298876 cdflib-1.2.5/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-02 00:07:58.000000 cdflib-1.2.5/archive/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-03-02 00:07:58.000000 cdflib-1.2.5/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.298876 cdflib-1.2.5/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 00:07:58.000000 cdflib-1.2.5/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-02 00:07:58.000000 cdflib-1.2.5/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.302876 cdflib-1.2.5/cdflib/
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/CDFLeapSeconds.txt
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/_gzip_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-02 00:08:07.000000 cdflib-1.2.5/cdflib/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    84441 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/cdfread.py
--rw-r--r--   0 runner    (1001) docker     (127)   106046 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/cdfwrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)    65533 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/epochs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/epochs_astropy.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.302876 cdflib-1.2.5/cdflib/xarray/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38101 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/xarray/cdf_to_xarray.py
--rw-r--r--   0 runner    (1001) docker     (127)    38007 2024-03-02 00:07:58.000000 cdflib-1.2.5/cdflib/xarray/xarray_to_cdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.310876 cdflib-1.2.5/cdflib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-02 00:08:07.000000 cdflib-1.2.5/cdflib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-02 00:08:07.000000 cdflib-1.2.5/cdflib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 00:08:07.000000 cdflib-1.2.5/cdflib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-02 00:08:07.000000 cdflib-1.2.5/cdflib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-02 00:08:07.000000 cdflib-1.2.5/cdflib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-02 00:07:58.000000 cdflib-1.2.5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.306876 cdflib-1.2.5/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.306876 cdflib-1.2.5/doc/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/modules/cdfepoch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/modules/cdfread.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/modules/cdfwrite.rst
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/modules/dataclasses.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/modules/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-02 00:07:58.000000 cdflib-1.2.5/doc/modules/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-02 00:07:58.000000 cdflib-1.2.5/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-02 00:07:58.000000 cdflib-1.2.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-02 00:07:58.000000 cdflib-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-02 00:08:07.310876 cdflib-1.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.306876 cdflib-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-02 00:07:58.000000 cdflib-1.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-03-02 00:07:58.000000 cdflib-1.2.5/tests/test_astropy_epochs.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-02 00:07:58.000000 cdflib-1.2.5/tests/test_cdfread.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-02 00:07:58.000000 cdflib-1.2.5/tests/test_cdfread_rle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18059 2024-03-02 00:07:58.000000 cdflib-1.2.5/tests/test_cdfwrite.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9647 2024-03-02 00:07:58.000000 cdflib-1.2.5/tests/test_epochs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20738 2024-03-02 00:07:58.000000 cdflib-1.2.5/tests/test_xarray_reader_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:08:07.310876 cdflib-1.2.5/tests/testfiles/
--rw-r--r--   0 runner    (1001) docker     (127)   125566 2024-03-02 00:07:58.000000 cdflib-1.2.5/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (127)    67164 2024-03-02 00:07:58.000000 cdflib-1.2.5/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (127)    70003 2024-03-02 00:07:58.000000 cdflib-1.2.5/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-02 00:07:58.000000 cdflib-1.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.011916 cdflib-1.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.003916 cdflib-1.2.6/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-05 22:06:55.000000 cdflib-1.2.6/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-05 22:06:55.000000 cdflib-1.2.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:12.999916 cdflib-1.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.003916 cdflib-1.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-05 22:06:55.000000 cdflib-1.2.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-05 22:06:55.000000 cdflib-1.2.6/.github/workflows/pypi-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-05 22:06:55.000000 cdflib-1.2.6/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-05 22:06:55.000000 cdflib-1.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-05 22:06:55.000000 cdflib-1.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-05 22:06:55.000000 cdflib-1.2.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-05 22:06:55.000000 cdflib-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-05 22:06:55.000000 cdflib-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-05 22:07:13.011916 cdflib-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-05 22:06:55.000000 cdflib-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.003916 cdflib-1.2.6/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-05 22:06:55.000000 cdflib-1.2.6/archive/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-03-05 22:06:55.000000 cdflib-1.2.6/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.003916 cdflib-1.2.6/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 22:06:55.000000 cdflib-1.2.6/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-05 22:06:55.000000 cdflib-1.2.6/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.007916 cdflib-1.2.6/cdflib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/CDFLeapSeconds.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/_gzip_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-05 22:07:12.000000 cdflib-1.2.6/cdflib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84441 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106046 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/cdfwrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65533 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/epochs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/epochs_astropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.007916 cdflib-1.2.6/cdflib/xarray/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38137 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/xarray/cdf_to_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38007 2024-03-05 22:06:55.000000 cdflib-1.2.6/cdflib/xarray/xarray_to_cdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.011916 cdflib-1.2.6/cdflib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-05 22:07:12.000000 cdflib-1.2.6/cdflib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-05 22:07:12.000000 cdflib-1.2.6/cdflib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 22:07:12.000000 cdflib-1.2.6/cdflib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-05 22:07:12.000000 cdflib-1.2.6/cdflib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-05 22:07:12.000000 cdflib-1.2.6/cdflib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-05 22:06:55.000000 cdflib-1.2.6/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.007916 cdflib-1.2.6/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.011916 cdflib-1.2.6/doc/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/modules/cdfepoch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/modules/cdfread.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/modules/cdfwrite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/modules/dataclasses.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/modules/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-05 22:06:55.000000 cdflib-1.2.6/doc/modules/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-05 22:06:55.000000 cdflib-1.2.6/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-05 22:06:55.000000 cdflib-1.2.6/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-05 22:06:55.000000 cdflib-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-05 22:07:13.011916 cdflib-1.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.011916 cdflib-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-05 22:06:55.000000 cdflib-1.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-03-05 22:06:55.000000 cdflib-1.2.6/tests/test_astropy_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-05 22:06:55.000000 cdflib-1.2.6/tests/test_cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-05 22:06:55.000000 cdflib-1.2.6/tests/test_cdfread_rle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18059 2024-03-05 22:06:55.000000 cdflib-1.2.6/tests/test_cdfwrite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9647 2024-03-05 22:06:55.000000 cdflib-1.2.6/tests/test_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20738 2024-03-05 22:06:55.000000 cdflib-1.2.6/tests/test_xarray_reader_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:07:13.011916 cdflib-1.2.6/tests/testfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)   125566 2024-03-05 22:06:55.000000 cdflib-1.2.6/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (127)    67164 2024-03-05 22:06:55.000000 cdflib-1.2.6/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (127)    70003 2024-03-05 22:06:55.000000 cdflib-1.2.6/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-05 22:06:55.000000 cdflib-1.2.6/tox.ini
```

### Comparing `cdflib-1.2.5/.circleci/config.yml` & `cdflib-1.2.6/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/.github/workflows/ci.yml` & `cdflib-1.2.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/.github/workflows/pypi-build.yaml` & `cdflib-1.2.6/.github/workflows/pypi-build.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/.pre-commit-config.yaml` & `cdflib-1.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/.readthedocs.yml` & `cdflib-1.2.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/LICENSE` & `cdflib-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/PKG-INFO` & `cdflib-1.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.2.5
+Version: 1.2.6
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.2.5/README.md` & `cdflib-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/asv.conf.json` & `cdflib-1.2.6/asv.conf.json`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/benchmarks/benchmarks.py` & `cdflib-1.2.6/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/cdflib/CDFLeapSeconds.txt` & `cdflib-1.2.6/cdflib/CDFLeapSeconds.txt`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/cdflib/cdfread.py` & `cdflib-1.2.6/cdflib/cdfread.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/cdflib/cdfwrite.py` & `cdflib-1.2.6/cdflib/cdfwrite.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/cdflib/dataclasses.py` & `cdflib-1.2.6/cdflib/dataclasses.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/cdflib/epochs.py` & `cdflib-1.2.6/cdflib/epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/cdflib/epochs_astropy.py` & `cdflib-1.2.6/cdflib/epochs_astropy.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/cdflib/s3.py` & `cdflib-1.2.6/cdflib/s3.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/cdflib/utils.py` & `cdflib-1.2.6/cdflib/utils.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/cdflib/xarray/cdf_to_xarray.py` & `cdflib-1.2.6/cdflib/xarray/cdf_to_xarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,18 +303,18 @@
     var_props: VDRInfo,
     depend_variables: List[str],
     all_variable_data: Dict[str, npt.NDArray],
     all_variable_properties: Dict[str, VDRInfo],
     created_unlimited_dims: Dict[str, int],
 ) -> Tuple[str, bool, bool]:
     """
-    Determines the name of the
+    Determines the name of the dimensions that the variables span
     """
 
-    if var_props.Rec_Vary and var_props.Last_Rec > 0:
+    if var_props.Rec_Vary and var_props.Last_Rec >= 0:
         # Check if this variable is itself the dimension
         if var_name in depend_variables and (len(var_props.Dim_Sizes) == 0 or var_props.Last_Rec >= 0):
             if not (len(var_props.Dim_Sizes) > 0 and var_props.Last_Rec > 0):
                 return var_name, True, False
             # There might be dimensions listed, but they might not vary
             if len(var_props.Dim_Sizes) > 0:
                 for i in range(0, len(var_props.Dim_Sizes)):
```

### Comparing `cdflib-1.2.5/cdflib/xarray/xarray_to_cdf.py` & `cdflib-1.2.6/cdflib/xarray/xarray_to_cdf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/cdflib.egg-info/PKG-INFO` & `cdflib-1.2.6/cdflib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.2.5
+Version: 1.2.6
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.2.5/cdflib.egg-info/SOURCES.txt` & `cdflib-1.2.6/cdflib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/doc/Makefile` & `cdflib-1.2.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/doc/changelog.rst` & `cdflib-1.2.6/doc/changelog.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/doc/conf.py` & `cdflib-1.2.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/doc/index.rst` & `cdflib-1.2.6/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/doc/make.bat` & `cdflib-1.2.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/doc/modules/cdfepoch.rst` & `cdflib-1.2.6/doc/modules/cdfepoch.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/doc/modules/cdfread.rst` & `cdflib-1.2.6/doc/modules/cdfread.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/doc/modules/cdfwrite.rst` & `cdflib-1.2.6/doc/modules/cdfwrite.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/meta.yaml` & `cdflib-1.2.6/meta.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/mypy.ini` & `cdflib-1.2.6/mypy.ini`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/setup.cfg` & `cdflib-1.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/tests/test_astropy_epochs.py` & `cdflib-1.2.6/tests/test_astropy_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/tests/test_cdfread.py` & `cdflib-1.2.6/tests/test_cdfread.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/tests/test_cdfwrite.py` & `cdflib-1.2.6/tests/test_cdfwrite.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/tests/test_epochs.py` & `cdflib-1.2.6/tests/test_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/tests/test_xarray_reader_writer.py` & `cdflib-1.2.6/tests/test_xarray_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf` & `cdflib-1.2.6/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf` & `cdflib-1.2.6/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.2.5/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf` & `cdflib-1.2.6/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf`

 * *Files identical despite different names*

