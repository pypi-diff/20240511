# Comparing `tmp/lephare-0.1.5.tar.gz` & `tmp/lephare-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lephare-0.1.5.tar", last modified: Mon May  6 23:48:56 2024, max compression
+gzip compressed data, was "lephare-0.1.6.tar", last modified: Fri May 10 23:27:27 2024, max compression
```

## Comparing `lephare-0.1.5.tar` & `lephare-0.1.6.tar`

### file list

```diff
@@ -1,259 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.045221 lephare-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-06 23:48:49.000000 lephare-0.1.5/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-06 23:48:49.000000 lephare-0.1.5/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 23:48:49.000000 lephare-0.1.5/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-06 23:48:49.000000 lephare-0.1.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.005221 lephare-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.005221 lephare-0.1.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.005221 lephare-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/compile-cpp.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-06 23:48:49.000000 lephare-0.1.5/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-06 23:48:49.000000 lephare-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-06 23:48:49.000000 lephare-0.1.5/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-06 23:48:49.000000 lephare-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-06 23:48:49.000000 lephare-0.1.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-06 23:48:49.000000 lephare-0.1.5/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-06 23:48:49.000000 lephare-0.1.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-06 23:48:49.000000 lephare-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-06 23:48:56.045221 lephare-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-06 23:48:49.000000 lephare-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.005221 lephare-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.005221 lephare-0.1.5/docs/doxygen/
--rw-r--r--   0 runner    (1001) docker     (127)   112662 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/doxygen/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/keywords.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/legacy_install.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.009221 lephare-0.1.5/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Building_list_of_onesources.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Data_retrieval.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Example_SED_manipulation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Example_cosmo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Example_full_run.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Example_of_usage_of_magSvc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Minimal_photoz_run.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.009221 lephare-0.1.5/docs/notebooks/data/
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/data/COSMOS.para
--rw-r--r--   0 runner    (1001) docker     (127)    66240 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/data/COSMOS_first100specz.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks/data/output.para
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-06 23:48:49.000000 lephare-0.1.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.009221 lephare-0.1.5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-05-06 23:48:49.000000 lephare-0.1.5/examples/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-05-06 23:48:49.000000 lephare-0.1.5/examples/figuresLPP.py
--rw-r--r--   0 runner    (1001) docker     (127)    31984 2024-05-06 23:48:49.000000 lephare-0.1.5/examples/figuresLPZ.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-06 23:48:49.000000 lephare-0.1.5/examples/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-06 23:48:49.000000 lephare-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 23:48:56.045221 lephare-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-06 23:48:49.000000 lephare-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.001221 lephare-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.013221 lephare-0.1.5/src/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/_flt.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/_photoz.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/filterSvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/magSvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/mag_gal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/sedtolib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lephare/zphota.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.041221 lephare-0.1.5/src/lephare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 23:48:55.000000 lephare-0.1.5/src/lephare.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.017221 lephare-0.1.5/src/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3003 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/PDF.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/PDF.h
--rw-r--r--   0 runner    (1001) docker     (127)    72115 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/SED.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/SED.h
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/SEDLib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/SEDLib.h
--rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/_bindings.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/cosmology.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/cosmology.h
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/ext.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/ext.h
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/ext_curv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/filter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/filter_extinc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20186 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/flt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/flt.h
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/globals.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/globals.h
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/keyword.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/keyword.h
--rw-r--r--   0 runner    (1001) docker     (127)    31598 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/mag.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/mag.h
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/mag_gal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/oneElLambda.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/oneElLambda.h
--rw-r--r--   0 runner    (1001) docker     (127)    80072 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/onesource.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/onesource.h
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/opa.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/opa.h
--rw-r--r--   0 runner    (1001) docker     (127)    61669 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/photoz_lib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/photoz_lib.h
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/sedtolib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-06 23:48:49.000000 lephare-0.1.5/src/lib/zphota.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.017221 lephare-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.021221 lephare-0.1.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/alloutputkeys.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    41606 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/calzetti.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.021221 lephare-0.1.5/tests/data/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/examples/COSMOS.para
--rw-r--r--   0 runner    (1001) docker     (127)    66240 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/examples/COSMOS_first100specz.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/examples/output.para
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.021221 lephare-0.1.5/tests/data/ext/
--rwxr-xr-x   0 runner    (1001) docker     (127)   104052 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/ext/MW_seaton.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)    72411 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/ext/SB_calzetti.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.001221 lephare-0.1.5/tests/data/filt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.021221 lephare-0.1.5/tests/data/filt/subaru/
--rw-r--r--   0 runner    (1001) docker     (127)    25919 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/filt/subaru/IB527.pb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/opa/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/OPACITY.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau00.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau01.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau02.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau03.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau04.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau05.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau06.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau07.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau08.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau09.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau10.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau11.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau12.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau13.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau14.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau15.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau16.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau17.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau18.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau19.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau20.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau21.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau22.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau23.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau24.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau25.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau26.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau27.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau28.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau29.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau30.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau31.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau32.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau33.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau34.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau35.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau36.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau37.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau38.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau39.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau40.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau41.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau42.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau43.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau44.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau45.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau46.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau47.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau48.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau49.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau50.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau51.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau52.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau53.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau54.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau55.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau56.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau57.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau58.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau59.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau60.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau61.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau62.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau63.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau64.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau65.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau66.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau67.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau68.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau69.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau70.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau71.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau72.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau73.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau74.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau75.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau76.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau77.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau78.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau79.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/opa/tau80.out
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/sed/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/sed/GAL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/sed/GAL/BETHERMIN12/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/GAL/BETHERMIN12/BETHERMIN12_MOD.list
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/GAL/BETHERMIN12/sed_z1_MS.dat
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/GAL/ONE_SED.list
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/GAL/o5v.sed.ext
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/sed/QSO/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/QSO/ONE_SED.list
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/QSO/o5v.sed.ext
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.037221 lephare-0.1.5/tests/data/sed/STAR/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/STAR/ONE_SED.list
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/STAR/o5v.sed.ext
--rw-r--r--   0 runner    (1001) docker     (127)    54522 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/WDgd71.sed.ext
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/sed/o5v.sed.ext
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/tau10.out
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/test_data_registry.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/test_file_names.list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.041221 lephare-0.1.5/tests/data/vega/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1592 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/BD+17.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)     3957 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/BD+17o4708.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    24434 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/SunLCB.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    24455 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/VegaLCB.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   100244 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/a0v.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    93156 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/data/vega/a0v_n.sed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:48:56.041221 lephare-0.1.5/tests/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_data_retrieval_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_oneElLambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_onesource.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-06 23:48:49.000000 lephare-0.1.5/tests/lephare/test_sed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.627685 lephare-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-10 23:27:21.000000 lephare-0.1.6/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-10 23:27:21.000000 lephare-0.1.6/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-10 23:27:21.000000 lephare-0.1.6/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-10 23:27:21.000000 lephare-0.1.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.591685 lephare-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.591685 lephare-0.1.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.591685 lephare-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/compile-cpp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-10 23:27:21.000000 lephare-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 23:27:21.000000 lephare-0.1.6/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-10 23:27:21.000000 lephare-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-10 23:27:21.000000 lephare-0.1.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-10 23:27:21.000000 lephare-0.1.6/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-10 23:27:21.000000 lephare-0.1.6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-10 23:27:21.000000 lephare-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-05-10 23:27:27.627685 lephare-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-10 23:27:21.000000 lephare-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.595685 lephare-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.595685 lephare-0.1.6/docs/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (127)   112662 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/doxygen/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/keywords.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/legacy_install.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.595685 lephare-0.1.6/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Building_list_of_onesources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Data_retrieval.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Example_SED_manipulation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Example_cosmo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Example_full_run.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Example_of_usage_of_magSvc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Minimal_photoz_run.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.595685 lephare-0.1.6/docs/notebooks/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/data/COSMOS.para
+-rw-r--r--   0 runner    (1001) docker     (127)    66240 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/data/COSMOS_first100specz.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/data/output.para
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.595685 lephare-0.1.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-05-10 23:27:21.000000 lephare-0.1.6/examples/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-05-10 23:27:21.000000 lephare-0.1.6/examples/figuresLPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31984 2024-05-10 23:27:21.000000 lephare-0.1.6/examples/figuresLPZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-10 23:27:21.000000 lephare-0.1.6/examples/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-10 23:27:21.000000 lephare-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 23:27:27.627685 lephare-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-10 23:27:21.000000 lephare-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.587685 lephare-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.599686 lephare-0.1.6/src/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/_flt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/_photoz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/filterSvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/magSvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/mag_gal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/sedtolib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/zphota.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.627685 lephare-0.1.6/src/lephare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/src/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3003 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/PDF.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/PDF.h
+-rw-r--r--   0 runner    (1001) docker     (127)    72115 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/SED.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/SED.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/SEDLib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/SEDLib.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/_bindings.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/cosmology.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/cosmology.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/ext.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/ext.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/ext_curv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/filter_extinc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20186 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/flt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/flt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/globals.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/globals.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/keyword.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/keyword.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31598 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/mag.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/mag.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/mag_gal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/oneElLambda.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/oneElLambda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    80072 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/onesource.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/onesource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/opa.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/opa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61669 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/photoz_lib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/photoz_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/sedtolib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/zphota.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/alloutputkeys.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41606 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/calzetti.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    84794 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/example.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/tests/data/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/examples/COSMOS.para
+-rw-r--r--   0 runner    (1001) docker     (127)    66240 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/examples/COSMOS_first100specz.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/examples/output.para
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/tests/data/ext/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   104052 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/ext/MW_seaton.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72411 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/ext/SB_calzetti.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.587685 lephare-0.1.6/tests/data/filt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/tests/data/filt/subaru/
+-rw-r--r--   0 runner    (1001) docker     (127)    25919 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/filt/subaru/IB527.pb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/opa/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/OPACITY.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau00.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau01.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau02.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau03.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau04.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau05.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau06.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau07.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau08.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau09.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau10.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau11.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau12.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau13.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau14.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau15.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau16.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau17.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau18.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau19.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau20.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau21.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau22.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau23.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau24.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau25.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau26.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau27.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau28.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau29.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau30.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau31.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau32.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau33.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau34.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau35.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau36.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau37.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau38.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau39.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau40.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau41.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau42.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau43.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau44.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau45.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau46.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau47.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau48.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau49.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau50.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau51.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau52.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau53.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau54.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau55.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau56.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau57.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau58.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau59.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau60.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau61.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau62.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau63.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau64.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau65.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau66.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau67.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau68.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau69.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau70.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau71.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau72.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau73.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau74.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau75.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau76.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau77.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau78.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau79.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau80.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/sed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/sed/GAL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/sed/GAL/BETHERMIN12/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/GAL/BETHERMIN12/BETHERMIN12_MOD.list
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/GAL/BETHERMIN12/sed_z1_MS.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/GAL/ONE_SED.list
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/GAL/o5v.sed.ext
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/sed/QSO/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/QSO/ONE_SED.list
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/QSO/o5v.sed.ext
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/sed/STAR/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/STAR/ONE_SED.list
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/STAR/o5v.sed.ext
+-rw-r--r--   0 runner    (1001) docker     (127)    54522 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/WDgd71.sed.ext
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/o5v.sed.ext
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/tau10.out
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/test_data_registry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/test_file_names.list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.627685 lephare-0.1.6/tests/data/vega/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1592 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/BD+17.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3957 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/BD+17o4708.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24434 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/SunLCB.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24455 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/VegaLCB.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   100244 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/a0v.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    93156 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/a0v_n.sed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.627685 lephare-0.1.6/tests/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_data_retrieval_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_oneElLambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_onesource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_sed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_spec.py
```

### Comparing `lephare-0.1.5/.copier-answers.yml` & `lephare-0.1.6/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.gitattributes` & `lephare-0.1.6/.gitattributes`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.github/ISSUE_TEMPLATE/1-bug_report.md` & `lephare-0.1.6/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.github/ISSUE_TEMPLATE/2-feature_request.md` & `lephare-0.1.6/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.github/pull_request_template.md` & `lephare-0.1.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.github/workflows/build-documentation.yml` & `lephare-0.1.6/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.github/workflows/compile-cpp.yml` & `lephare-0.1.6/.github/workflows/compile-cpp.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.github/workflows/pre-commit-ci.yml` & `lephare-0.1.6/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.github/workflows/publish-to-pypi.yml` & `lephare-0.1.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.github/workflows/smoke-test.yml` & `lephare-0.1.6/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.github/workflows/testing-and-coverage.yml` & `lephare-0.1.6/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.gitignore` & `lephare-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.pre-commit-config.yaml` & `lephare-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.readthedocs.yml` & `lephare-0.1.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/.setup_dev.sh` & `lephare-0.1.6/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/CMakeLists.txt` & `lephare-0.1.6/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/LICENSE` & `lephare-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/PKG-INFO` & `lephare-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lephare
-Version: 0.1.5
+Version: 0.1.6
 Summary: LEPHARE photometric redshift estimator
 Home-page: https://gitlab.lam.fr/Galaxies/LEPHARE
 Author: Johann Cohen-Tanugi
 Author-email: Stéphane Arnouts <stephane.arnouts@lam.fr>, Olivier Ilbert <olivier.ilbert@lam.fr>, Johann Cohen-Tanugi <johann.cohen-tanugi@in2p3.fr>, Raphael Shirley <rshirley@mpe.mpg.de>
 License: MIT License
         
         Copyright (c) 2023 Johann Cohen-Tanugi
@@ -86,15 +86,15 @@
 
 Before installing any dependencies or writing code, it's a great idea to create a
 virtual environment. LINCC-Frameworks engineers primarily use `conda` to manage virtual
 environments. If you have conda installed locally, you can run the following to
 create and activate a new environment.
 
 ```
->> conda create env -n <env_name> python=3.10
+>> conda create -n <env_name> python=3.10
 >> conda activate <env_name>
 ```
 
 Once you have created a new environment, you can install this project for local
 development using the following commands:
 
 ```
```

### Comparing `lephare-0.1.5/README.md` & `lephare-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 Before installing any dependencies or writing code, it's a great idea to create a
 virtual environment. LINCC-Frameworks engineers primarily use `conda` to manage virtual
 environments. If you have conda installed locally, you can run the following to
 create and activate a new environment.
 
 ```
->> conda create env -n <env_name> python=3.10
+>> conda create -n <env_name> python=3.10
 >> conda activate <env_name>
 ```
 
 Once you have created a new environment, you can install this project for local
 development using the following commands:
 
 ```
```

### Comparing `lephare-0.1.5/docs/Makefile` & `lephare-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/conf.py` & `lephare-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/doxygen/Doxyfile` & `lephare-0.1.6/docs/doxygen/Doxyfile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/index.rst` & `lephare-0.1.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/keywords.rst` & `lephare-0.1.6/docs/keywords.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/legacy_install.rst` & `lephare-0.1.6/docs/legacy_install.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/Building_list_of_onesources.ipynb` & `lephare-0.1.6/docs/notebooks/Building_list_of_onesources.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/Data_retrieval.ipynb` & `lephare-0.1.6/docs/notebooks/Data_retrieval.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/Example_SED_manipulation.ipynb` & `lephare-0.1.6/docs/notebooks/Example_SED_manipulation.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/Example_cosmo.ipynb` & `lephare-0.1.6/docs/notebooks/Example_cosmo.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/Example_full_run.ipynb` & `lephare-0.1.6/docs/notebooks/Example_full_run.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/Example_of_usage_of_magSvc.ipynb` & `lephare-0.1.6/docs/notebooks/Example_of_usage_of_magSvc.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/Minimal_photoz_run.ipynb` & `lephare-0.1.6/docs/notebooks/Minimal_photoz_run.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/README.md` & `lephare-0.1.6/docs/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb` & `lephare-0.1.6/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/data/COSMOS.para` & `lephare-0.1.6/docs/notebooks/data/COSMOS.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/data/COSMOS_first100specz.fits` & `lephare-0.1.6/docs/notebooks/data/COSMOS_first100specz.fits`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks/data/output.para` & `lephare-0.1.6/docs/notebooks/data/output.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/docs/notebooks.rst` & `lephare-0.1.6/docs/notebooks.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/examples/color.py` & `lephare-0.1.6/examples/color.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/examples/figuresLPP.py` & `lephare-0.1.6/examples/figuresLPP.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/examples/figuresLPZ.py` & `lephare-0.1.6/examples/figuresLPZ.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/examples/spec.py` & `lephare-0.1.6/examples/spec.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/pyproject.toml` & `lephare-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/setup.py` & `lephare-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/__init__.py` & `lephare-0.1.6/src/lephare/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,9 +24,10 @@
 from .data_retrieval import *
 from .filter import *
 from .filterSvc import *
 from .mag_gal import *
 from .magSvc import *
 from .prepare import *
 from .process import *
+from .runner import *
 from .sedtolib import *
 from .zphota import *
```

### Comparing `lephare-0.1.5/src/lephare/_flt.py` & `lephare-0.1.6/src/lephare/_flt.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/_pdf.py` & `lephare-0.1.6/src/lephare/_pdf.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/_photoz.py` & `lephare-0.1.6/src/lephare/_photoz.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/_spec.py` & `lephare-0.1.6/src/lephare/_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
+__all__ = [
+    "plotspec",
+]
+
 
 def plotspec(filename):
     ### Open .spec file[s] and read the parameters
     fsp = open(filename, "r")  # noqa: SIM115
     print("File:", filename)
 
     bid = fsp.readline()  # header1
```

### Comparing `lephare-0.1.5/src/lephare/_utils.py` & `lephare-0.1.6/src/lephare/_utils.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/data_manager.py` & `lephare-0.1.6/src/lephare/data_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import datetime
 import os
 
 from platformdirs import user_cache_dir
 
+__all__ = [
+    "DataManager",
+]
+
 
 class DataManager:
     def __init__(self):
         self.lephare_dir = os.getenv("LEPHAREDIR", None)
         self.lephare_work_dir = os.getenv("LEPHAREWORK", None)
 
     @property
@@ -80,45 +84,97 @@
             # the lephare work dir env var is set, create subdirectories if needed
             self.create_work_subdirectories(self.lephare_work_dir)
             print(
                 f"""User defined LEPHAREWORK is set. All intermediate files will
                 be written to {self.lephare_work_dir}."""
             )
 
-    def create_new_run(self):
+    def create_new_run(self, descriptive_directory_name=None):
         """Create a timestamped directory to contain the output from the current run.
         The newly created timestamped directory is symlinked to the path defined
-        by the LEPHAREWORK environment variable."""
+        by the LEPHAREWORK environment variable.
+
+        Parameters
+        ----------
+        descriptive_directory_name: str
+            A descriptive name for the new run directory. If None, the directory
+            will be named with the current timestamp.
+
+        Returns
+        -------
+        run_directory : str
+            The path to the newly created run directory.
+        """
 
         lephare_work_dir = os.getenv("LEPHAREWORK", None)
 
         # if the LEPHAREWORK environment variable is not a symlink,
         # then this directory structure is unusual and we cannot create a new run.
         # We'll raise an exception and direct the user to the documentation.
         if not os.path.islink(f"{lephare_work_dir}"):
             # TODO include link to documentation
             raise RuntimeError(
                 """The current directory structure does not support the
                                creation of new runs. Please refer to the documentation for
                                information on how to set up the directory structure."""
             )
 
-        # given that LEPHAREWORK is a symlink, create a new timestamped run directory
-        now = datetime.datetime.now().strftime("%Y%m%dT%H%M%S")
-        run_directory = os.path.realpath(f"{lephare_work_dir}/../{now}")
+        # given that LEPHAREWORK is a symlink, create a new descriptive or
+        # timestamped run directory.
+        if descriptive_directory_name is not None:
+            run_directory = os.path.realpath(f"{lephare_work_dir}/../{descriptive_directory_name}")
+            if os.path.isdir(run_directory):
+                raise FileExistsError(
+                    f"The directory {run_directory} already exists. Please choose another name."
+                )
+        else:
+            now = datetime.datetime.now().strftime("%Y%m%dT%H%M%S")
+            run_directory = os.path.realpath(f"{lephare_work_dir}/../{now}")
+
         print(f"Creating new run directory at {run_directory}.")
         os.makedirs(run_directory, exist_ok=True)
 
         # remove the existing `work` symlink and create a new one
         if os.path.islink(lephare_work_dir):
             os.unlink(lephare_work_dir)
         os.symlink(run_directory, lephare_work_dir)
 
         # create the subdirectories in the new run directory
         self.create_work_subdirectories(run_directory)
 
+        return run_directory
+
     def create_work_subdirectories(self, parent_dir):
         """Creates the required work subdirectories in the parent directory if they
         are not present. No action is taken if the subdirectories already exist."""
         work_sub_directories = ["filt", "lib_bin", "lib_mag", "zphota"]
         for sub_dir in work_sub_directories:
             os.makedirs(os.path.join(parent_dir, sub_dir), exist_ok=True)
+
+    def remove_empty_run_directories(self):
+        """Remove any empty run directories from the cache. If any file exists in
+        any of the subdirectories, the run directory is not considered empty.
+        Note that we generate a new run directory if the work directory is no longer
+        a symlink."""
+        default_os_cache = user_cache_dir("lephare", ensure_exists=True)
+        work_sub_directories = ["filt", "lib_bin", "lib_mag", "zphota"]
+        runs_dir = os.path.join(default_os_cache, "runs")
+        work_dir = os.path.join(default_os_cache, "work")
+        symlink_target = os.readlink(work_dir)
+
+        # Remove empty directories (only if all subdirs are empty)
+        for run_name in os.listdir(runs_dir):
+            run_dir = os.path.join(runs_dir, run_name)
+            empty = True
+            for sub_dir in work_sub_directories:
+                if len(os.listdir(os.path.join(run_dir, sub_dir))) > 0:
+                    empty = False
+                    break
+            if empty:
+                for sub_dir in work_sub_directories:
+                    os.rmdir(os.path.join(run_dir, sub_dir))
+                os.rmdir(run_dir)
+
+        # If we removed the work dir's symlink target, replace with new run dir:
+        if symlink_target not in os.listdir(runs_dir):
+            print("Work directory is no longer a symlink. Creating new run.")
+            self.create_new_run()
```

### Comparing `lephare-0.1.5/src/lephare/data_retrieval.py` & `lephare-0.1.6/src/lephare/data_retrieval.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/filter.py` & `lephare-0.1.6/src/lephare/filter.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/filterSvc.py` & `lephare-0.1.6/src/lephare/filterSvc.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/magSvc.py` & `lephare-0.1.6/src/lephare/magSvc.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/mag_gal.py` & `lephare-0.1.6/src/lephare/mag_gal.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/prepare.py` & `lephare-0.1.6/src/lephare/prepare.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/process.py` & `lephare-0.1.6/src/lephare/process.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/runner.py` & `lephare-0.1.6/src/lephare/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import argparse
 import os
 import time
 
 from lephare._lephare import get_lephare_env, keyword
 
+__all__ = [
+    "Runner",
+]
+
 
 class Runner:
     """Base class holding config values for running all stages.
 
     Parameters
     ----------
     config_keys : `list` or `None`, optional
@@ -36,15 +40,15 @@
             self.parse_config_file(config_file)
         if config_keymap is not None:
             # merge the config_file and config_keymap, keeping the config_keymap in case of duplicate
             self.keymap = self.keymap | config_keymap
         if config_keymap is None and config_file is None:
             # this only happens if the code is called as an executed script
             # Consider the keywords given in the line command
-            self.args = self.config_parser(config_keys)
+            self.args = self.config_parser()
             if self.timer:
                 self.start = time.time()
         # set verbosity. check keymap is not set on the commandline.
         if not self.verbose and "VERBOSE" in self.keymap:
             self.verbose = self.keymap["VERBOSE"].split_bool("NO", 1)[0]
 
     # This function take the config file, read it line per linem and output a keyword map
@@ -63,15 +67,15 @@
 
         def config_reader(filename):
             for row in open(filename, "r"):  # noqa: SIM115
                 yield row
 
         config = config_reader(filename)
         for line in config:
-            if line[0] != "#" and line != "\n":
+            if line[0] != "#" and line != "\n" and not line.isspace():
                 splits = line.split()
                 splits[0].lstrip()  # remove leading spaces
                 if splits[0] != "#":
                     try:
                         keymap[splits[0]] = keyword(splits[0], splits[1])
                     except:  # noqa: E722
                         keymap[splits[0]] = keyword(splits[0], "")
@@ -81,22 +85,16 @@
                             **{
                                 splits[0]: splits[1],
                             }
                         )
 
         self.keymap = keymap
 
-    def config_parser(self, config_keys):
-        """Create command line config parser from list of keys
-
-        Parameters
-        ----------
-        config_keys : `list`
-            List of all config keys
-        """
+    def config_parser(self):
+        """Create command line config parser from list of keys"""
         parser = argparse.ArgumentParser(add_help=False)
         # No required positional argument as in the C++ code, though in there
         # absence of the config file results in exiting. Need to understand whether
         # LePhare executables can be run with all keywords provided at the
         # command line
         parser.add_argument("-c", "--config", type=str, default="", help="Path to config file.")
         args, unknown = parser.parse_known_args()
```

### Comparing `lephare-0.1.5/src/lephare/sedtolib.py` & `lephare-0.1.6/src/lephare/sedtolib.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare/zphota.py` & `lephare-0.1.6/src/lephare/zphota.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lephare.egg-info/PKG-INFO` & `lephare-0.1.6/src/lephare.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lephare
-Version: 0.1.5
+Version: 0.1.6
 Summary: LEPHARE photometric redshift estimator
 Home-page: https://gitlab.lam.fr/Galaxies/LEPHARE
 Author: Johann Cohen-Tanugi
 Author-email: Stéphane Arnouts <stephane.arnouts@lam.fr>, Olivier Ilbert <olivier.ilbert@lam.fr>, Johann Cohen-Tanugi <johann.cohen-tanugi@in2p3.fr>, Raphael Shirley <rshirley@mpe.mpg.de>
 License: MIT License
         
         Copyright (c) 2023 Johann Cohen-Tanugi
@@ -86,15 +86,15 @@
 
 Before installing any dependencies or writing code, it's a great idea to create a
 virtual environment. LINCC-Frameworks engineers primarily use `conda` to manage virtual
 environments. If you have conda installed locally, you can run the following to
 create and activate a new environment.
 
 ```
->> conda create env -n <env_name> python=3.10
+>> conda create -n <env_name> python=3.10
 >> conda activate <env_name>
 ```
 
 Once you have created a new environment, you can install this project for local
 development using the following commands:
 
 ```
```

### Comparing `lephare-0.1.5/src/lephare.egg-info/SOURCES.txt` & `lephare-0.1.6/src/lephare.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 src/lib/photoz_lib.cpp
 src/lib/photoz_lib.h
 src/lib/sedtolib.cpp
 src/lib/zphota.cpp
 tests/conftest.py
 tests/data/alloutputkeys.txt
 tests/data/calzetti.dat
+tests/data/example.spec
 tests/data/tau10.out
 tests/data/test_data_registry.txt
 tests/data/test_file_names.list
 tests/data/examples/COSMOS.para
 tests/data/examples/COSMOS_first100specz.fits
 tests/data/examples/output.para
 tests/data/ext/MW_seaton.dat
@@ -223,8 +224,10 @@
 tests/lephare/test_filter.py
 tests/lephare/test_globals.py
 tests/lephare/test_keyword.py
 tests/lephare/test_oneElLambda.py
 tests/lephare/test_onesource.py
 tests/lephare/test_prepare.py
 tests/lephare/test_process.py
-tests/lephare/test_sed.py
+tests/lephare/test_runner.py
+tests/lephare/test_sed.py
+tests/lephare/test_spec.py
```

### Comparing `lephare-0.1.5/src/lib/Makefile` & `lephare-0.1.6/src/lib/Makefile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/PDF.cpp` & `lephare-0.1.6/src/lib/PDF.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/PDF.h` & `lephare-0.1.6/src/lib/PDF.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/SED.cpp` & `lephare-0.1.6/src/lib/SED.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/SED.h` & `lephare-0.1.6/src/lib/SED.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/SEDLib.cpp` & `lephare-0.1.6/src/lib/SEDLib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/SEDLib.h` & `lephare-0.1.6/src/lib/SEDLib.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/_bindings.cc` & `lephare-0.1.6/src/lib/_bindings.cc`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/cosmology.cpp` & `lephare-0.1.6/src/lib/cosmology.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/cosmology.h` & `lephare-0.1.6/src/lib/cosmology.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/ext.cpp` & `lephare-0.1.6/src/lib/ext.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/ext.h` & `lephare-0.1.6/src/lib/ext.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/ext_curv.cpp` & `lephare-0.1.6/src/lib/ext_curv.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/filter.cpp` & `lephare-0.1.6/src/lib/filter.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/filter_extinc.cpp` & `lephare-0.1.6/src/lib/filter_extinc.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/flt.cpp` & `lephare-0.1.6/src/lib/flt.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/flt.h` & `lephare-0.1.6/src/lib/flt.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/globals.cpp` & `lephare-0.1.6/src/lib/globals.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/globals.h` & `lephare-0.1.6/src/lib/globals.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/keyword.cpp` & `lephare-0.1.6/src/lib/keyword.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/keyword.h` & `lephare-0.1.6/src/lib/keyword.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/mag.cpp` & `lephare-0.1.6/src/lib/mag.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/mag.h` & `lephare-0.1.6/src/lib/mag.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/mag_gal.cpp` & `lephare-0.1.6/src/lib/mag_gal.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/oneElLambda.cpp` & `lephare-0.1.6/src/lib/oneElLambda.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/oneElLambda.h` & `lephare-0.1.6/src/lib/oneElLambda.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/onesource.cpp` & `lephare-0.1.6/src/lib/onesource.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/onesource.h` & `lephare-0.1.6/src/lib/onesource.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/opa.cpp` & `lephare-0.1.6/src/lib/opa.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/opa.h` & `lephare-0.1.6/src/lib/opa.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/photoz_lib.cpp` & `lephare-0.1.6/src/lib/photoz_lib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/photoz_lib.h` & `lephare-0.1.6/src/lib/photoz_lib.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/sedtolib.cpp` & `lephare-0.1.6/src/lib/sedtolib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/src/lib/zphota.cpp` & `lephare-0.1.6/src/lib/zphota.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/conftest.py` & `lephare-0.1.6/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,7 +24,14 @@
     return os.path.join(test_data_dir, "test_data_registry.txt")
 
 
 @pytest.fixture
 def unset_env_vars():
     os.environ.pop("LEPHAREDIR", None)
     os.environ.pop("LEPHAREWORK", None)
+
+
+@pytest.fixture
+def set_env_vars():
+    test_dir = os.path.abspath(os.path.dirname(__file__))
+    os.environ["LEPHAREDIR"] = os.path.join(test_dir, "data")
+    os.environ["LEPHAREWORK"] = os.path.join(test_dir, "tmp")
```

### Comparing `lephare-0.1.5/tests/data/alloutputkeys.txt` & `lephare-0.1.6/tests/data/alloutputkeys.txt`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/calzetti.dat` & `lephare-0.1.6/tests/data/calzetti.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/examples/COSMOS.para` & `lephare-0.1.6/tests/data/examples/COSMOS.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/examples/COSMOS_first100specz.fits` & `lephare-0.1.6/tests/data/examples/COSMOS_first100specz.fits`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/examples/output.para` & `lephare-0.1.6/tests/data/examples/output.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/ext/MW_seaton.dat` & `lephare-0.1.6/tests/data/ext/MW_seaton.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/ext/SB_calzetti.dat` & `lephare-0.1.6/tests/data/ext/SB_calzetti.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/filt/subaru/IB527.pb` & `lephare-0.1.6/tests/data/filt/subaru/IB527.pb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/OPACITY.dat` & `lephare-0.1.6/tests/data/opa/OPACITY.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau00.out` & `lephare-0.1.6/tests/data/opa/tau00.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau01.out` & `lephare-0.1.6/tests/data/opa/tau01.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau02.out` & `lephare-0.1.6/tests/data/opa/tau02.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau03.out` & `lephare-0.1.6/tests/data/opa/tau03.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau04.out` & `lephare-0.1.6/tests/data/opa/tau04.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau05.out` & `lephare-0.1.6/tests/data/opa/tau05.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau06.out` & `lephare-0.1.6/tests/data/opa/tau06.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau07.out` & `lephare-0.1.6/tests/data/opa/tau07.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau08.out` & `lephare-0.1.6/tests/data/opa/tau08.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau09.out` & `lephare-0.1.6/tests/data/opa/tau09.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau10.out` & `lephare-0.1.6/tests/data/opa/tau10.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau11.out` & `lephare-0.1.6/tests/data/opa/tau11.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau12.out` & `lephare-0.1.6/tests/data/opa/tau12.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau13.out` & `lephare-0.1.6/tests/data/opa/tau13.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau14.out` & `lephare-0.1.6/tests/data/opa/tau14.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau15.out` & `lephare-0.1.6/tests/data/opa/tau15.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau16.out` & `lephare-0.1.6/tests/data/opa/tau16.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau17.out` & `lephare-0.1.6/tests/data/opa/tau17.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau18.out` & `lephare-0.1.6/tests/data/opa/tau18.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau19.out` & `lephare-0.1.6/tests/data/opa/tau19.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau20.out` & `lephare-0.1.6/tests/data/opa/tau20.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau21.out` & `lephare-0.1.6/tests/data/opa/tau21.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau22.out` & `lephare-0.1.6/tests/data/opa/tau22.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau23.out` & `lephare-0.1.6/tests/data/opa/tau23.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau24.out` & `lephare-0.1.6/tests/data/opa/tau24.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau25.out` & `lephare-0.1.6/tests/data/opa/tau25.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau26.out` & `lephare-0.1.6/tests/data/opa/tau26.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau27.out` & `lephare-0.1.6/tests/data/opa/tau27.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau28.out` & `lephare-0.1.6/tests/data/opa/tau28.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau29.out` & `lephare-0.1.6/tests/data/opa/tau29.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau30.out` & `lephare-0.1.6/tests/data/opa/tau30.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau31.out` & `lephare-0.1.6/tests/data/opa/tau31.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau32.out` & `lephare-0.1.6/tests/data/opa/tau32.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau33.out` & `lephare-0.1.6/tests/data/opa/tau33.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau34.out` & `lephare-0.1.6/tests/data/opa/tau34.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau35.out` & `lephare-0.1.6/tests/data/opa/tau35.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau36.out` & `lephare-0.1.6/tests/data/opa/tau36.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau37.out` & `lephare-0.1.6/tests/data/opa/tau37.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau38.out` & `lephare-0.1.6/tests/data/opa/tau38.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau39.out` & `lephare-0.1.6/tests/data/opa/tau39.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau40.out` & `lephare-0.1.6/tests/data/opa/tau40.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau41.out` & `lephare-0.1.6/tests/data/opa/tau41.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau42.out` & `lephare-0.1.6/tests/data/opa/tau42.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau43.out` & `lephare-0.1.6/tests/data/opa/tau43.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau44.out` & `lephare-0.1.6/tests/data/opa/tau44.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau45.out` & `lephare-0.1.6/tests/data/opa/tau45.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau46.out` & `lephare-0.1.6/tests/data/opa/tau46.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau47.out` & `lephare-0.1.6/tests/data/opa/tau47.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau48.out` & `lephare-0.1.6/tests/data/opa/tau48.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau49.out` & `lephare-0.1.6/tests/data/opa/tau49.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau50.out` & `lephare-0.1.6/tests/data/opa/tau50.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau51.out` & `lephare-0.1.6/tests/data/opa/tau51.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau52.out` & `lephare-0.1.6/tests/data/opa/tau52.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau53.out` & `lephare-0.1.6/tests/data/opa/tau53.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau54.out` & `lephare-0.1.6/tests/data/opa/tau54.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau55.out` & `lephare-0.1.6/tests/data/opa/tau55.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau56.out` & `lephare-0.1.6/tests/data/opa/tau56.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau57.out` & `lephare-0.1.6/tests/data/opa/tau57.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau58.out` & `lephare-0.1.6/tests/data/opa/tau58.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau59.out` & `lephare-0.1.6/tests/data/opa/tau59.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau60.out` & `lephare-0.1.6/tests/data/opa/tau60.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau61.out` & `lephare-0.1.6/tests/data/opa/tau61.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau62.out` & `lephare-0.1.6/tests/data/opa/tau62.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau63.out` & `lephare-0.1.6/tests/data/opa/tau63.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau64.out` & `lephare-0.1.6/tests/data/opa/tau64.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau65.out` & `lephare-0.1.6/tests/data/opa/tau65.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau66.out` & `lephare-0.1.6/tests/data/opa/tau66.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau67.out` & `lephare-0.1.6/tests/data/opa/tau67.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau68.out` & `lephare-0.1.6/tests/data/opa/tau68.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau69.out` & `lephare-0.1.6/tests/data/opa/tau69.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau70.out` & `lephare-0.1.6/tests/data/opa/tau70.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau71.out` & `lephare-0.1.6/tests/data/opa/tau71.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau72.out` & `lephare-0.1.6/tests/data/opa/tau72.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau73.out` & `lephare-0.1.6/tests/data/opa/tau73.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau74.out` & `lephare-0.1.6/tests/data/opa/tau74.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau75.out` & `lephare-0.1.6/tests/data/opa/tau75.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau76.out` & `lephare-0.1.6/tests/data/opa/tau76.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau77.out` & `lephare-0.1.6/tests/data/opa/tau77.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau78.out` & `lephare-0.1.6/tests/data/opa/tau78.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau79.out` & `lephare-0.1.6/tests/data/opa/tau79.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/opa/tau80.out` & `lephare-0.1.6/tests/data/opa/tau80.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/sed/GAL/BETHERMIN12/sed_z1_MS.dat` & `lephare-0.1.6/tests/data/sed/GAL/BETHERMIN12/sed_z1_MS.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/sed/GAL/o5v.sed.ext` & `lephare-0.1.6/tests/data/sed/GAL/o5v.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/sed/QSO/o5v.sed.ext` & `lephare-0.1.6/tests/data/sed/QSO/o5v.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/sed/STAR/o5v.sed.ext` & `lephare-0.1.6/tests/data/sed/STAR/o5v.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/sed/WDgd71.sed.ext` & `lephare-0.1.6/tests/data/sed/WDgd71.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/sed/o5v.sed.ext` & `lephare-0.1.6/tests/data/sed/o5v.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/tau10.out` & `lephare-0.1.6/tests/data/tau10.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/vega/BD+17.sed` & `lephare-0.1.6/tests/data/vega/BD+17.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/vega/BD+17o4708.sed` & `lephare-0.1.6/tests/data/vega/BD+17o4708.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/vega/SunLCB.sed` & `lephare-0.1.6/tests/data/vega/SunLCB.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/vega/VegaLCB.sed` & `lephare-0.1.6/tests/data/vega/VegaLCB.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/vega/a0v.sed` & `lephare-0.1.6/tests/data/vega/a0v.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/data/vega/a0v_n.sed` & `lephare-0.1.6/tests/data/vega/a0v_n.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/lephare/test_cosmology.py` & `lephare-0.1.6/tests/lephare/test_cosmology.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/lephare/test_data_retrieval.py` & `lephare-0.1.6/tests/lephare/test_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/lephare/test_data_retrieval_registry.py` & `lephare-0.1.6/tests/lephare/test_data_retrieval_registry.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/lephare/test_filter.py` & `lephare-0.1.6/tests/lephare/test_filter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 import numpy as np
 import pytest
 from lephare import (
+    Filter,
     flt,  # noqa: E402
 )
 from lephare.filterSvc import FilterSvc  # noqa: E402
 
 
 @pytest.fixture
 def filter_file(test_data_dir):
@@ -33,7 +34,27 @@
     if g is not None:
         assert np.allclose(f.data()[1], g.data()[1])
     else:
         print("SVO not tested due to exception raised : server not reachable?")
     # filters in COSMOS.para not available to the unit tests
     fltvec = FilterSvc.from_config(os.path.join(test_data_dir, "examples/COSMOS.para"))
     assert len(fltvec) == 1
+
+
+def test_filter_base_class(test_data_dir, set_env_vars):
+    """Simple test to ensure that we can create an instance of a Filter object."""
+    config_file_path = os.path.join(test_data_dir, "examples/COSMOS.para")
+    filter = Filter(config_file=config_file_path)
+    filter.run()
+    assert len(filter.keymap)
+
+
+def test_filter_with_kwargs(test_data_dir, set_env_vars):
+    """Simple test to ensure that we can create an instance of a Filter object
+    and that we can pass kwargs when instantiating the object."""
+    config_file_path = os.path.join(test_data_dir, "examples/COSMOS.para")
+    input_args = {"verbose": True, "TRANS_TYPE": 42}
+    filter = Filter(config_file=config_file_path)
+    filter.run(**input_args)
+    assert len(filter.keymap)
+    assert filter.verbose
+    assert filter.keymap["TRANS_TYPE"].value == "42"
```

### Comparing `lephare-0.1.5/tests/lephare/test_keyword.py` & `lephare-0.1.6/tests/lephare/test_keyword.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/lephare/test_oneElLambda.py` & `lephare-0.1.6/tests/lephare/test_oneElLambda.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/lephare/test_onesource.py` & `lephare-0.1.6/tests/lephare/test_onesource.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/lephare/test_process.py` & `lephare-0.1.6/tests/lephare/test_process.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.5/tests/lephare/test_sed.py` & `lephare-0.1.6/tests/lephare/test_sed.py`

 * *Files identical despite different names*

