# Comparing `tmp/tkinter-tooltip-3.0.0.tar.gz` & `tmp/tkinter_tooltip-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkinter-tooltip-3.0.0.tar", last modified: Sat Feb  3 18:53:13 2024, max compression
+gzip compressed data, was "tkinter_tooltip-3.1.0.tar", last modified: Sat May 11 17:50:51 2024, max compression
```

## Comparing `tkinter-tooltip-3.0.0.tar` & `tkinter_tooltip-3.1.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.776605 tkinter-tooltip-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.768605 tkinter-tooltip-3.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.768605 tkinter-tooltip-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.768605 tkinter-tooltip-3.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-02-03 18:53:13.776605 tkinter-tooltip-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.764605 tkinter-tooltip-3.0.0/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.768605 tkinter-tooltip-3.0.0/assets/animations/
--rw-r--r--   0 runner    (1001) docker     (127)   249355 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/assets/animations/color-changer.gif
--rw-r--r--   0 runner    (1001) docker     (127)   121443 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/assets/animations/color-changer.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    13488 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/assets/animations/tooltip-delayed.gif
--rw-r--r--   0 runner    (1001) docker     (127)   104213 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/assets/animations/tooltip-tracking.gif
--rw-r--r--   0 runner    (1001) docker     (127)    99322 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/assets/animations/tootip-dark-theme.gif
--rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/assets/animations/tootip-function-refresh.gif
--rw-r--r--   0 runner    (1001) docker     (127)   297660 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/assets/animations/tootip-function.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.772605 tkinter-tooltip-3.0.0/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)    13284 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/assets/images/header.png
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/assets/images/tooltip_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/assets/images/tootil-simple.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.772605 tkinter-tooltip-3.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/features.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.772605 tkinter-tooltip-3.0.0/docs/html_extra/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/html_extra/google3e426562ce42e98f.html
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/html_extra/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/docs/tktooltip.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.772605 tkinter-tooltip-3.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/examples/color_changer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/examples/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/examples/tooltip_destroy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/examples/tooltip_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-02-03 18:53:13.776605 tkinter-tooltip-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.772605 tkinter-tooltip-3.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/test/test_tktooltip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.776605 tkinter-tooltip-3.0.0/tkinter_tooltip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-02-03 18:53:13.000000 tkinter-tooltip-3.0.0/tkinter_tooltip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-03 18:53:13.000000 tkinter-tooltip-3.0.0/tkinter_tooltip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 18:53:13.000000 tkinter-tooltip-3.0.0/tkinter_tooltip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-03 18:53:13.000000 tkinter-tooltip-3.0.0/tkinter_tooltip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-03 18:53:13.000000 tkinter-tooltip-3.0.0/tkinter_tooltip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:53:13.776605 tkinter-tooltip-3.0.0/tktooltip/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/tktooltip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-03 18:53:13.000000 tkinter-tooltip-3.0.0/tktooltip/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/tktooltip/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-03 18:53:03.000000 tkinter-tooltip-3.0.0/tktooltip/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.848919 tkinter_tooltip-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.836919 tkinter_tooltip-3.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.836919 tkinter_tooltip-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.836919 tkinter_tooltip-3.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8031 2024-05-11 17:50:51.848919 tkinter_tooltip-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.832919 tkinter_tooltip-3.1.0/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.840919 tkinter_tooltip-3.1.0/assets/animations/
+-rw-r--r--   0 runner    (1001) docker     (127)   249355 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/assets/animations/color-changer.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   121443 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/assets/animations/color-changer.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    13488 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/assets/animations/tooltip-delayed.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   104213 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/assets/animations/tooltip-tracking.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    99322 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/assets/animations/tootip-dark-theme.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/assets/animations/tootip-function-refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   297660 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/assets/animations/tootip-function.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.840919 tkinter_tooltip-3.1.0/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    13284 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/assets/images/header.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/assets/images/tooltip_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/assets/images/tootil-simple.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.844919 tkinter_tooltip-3.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.844919 tkinter_tooltip-3.1.0/docs/html_extra/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/html_extra/google3e426562ce42e98f.html
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/html_extra/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/docs/tktooltip.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.844919 tkinter_tooltip-3.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/examples/color_changer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/examples/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/examples/tooltip_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/examples/tooltip_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-11 17:50:51.848919 tkinter_tooltip-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.844919 tkinter_tooltip-3.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/test/test_tktooltip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.844919 tkinter_tooltip-3.1.0/tkinter_tooltip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8031 2024-05-11 17:50:51.000000 tkinter_tooltip-3.1.0/tkinter_tooltip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-11 17:50:51.000000 tkinter_tooltip-3.1.0/tkinter_tooltip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 17:50:51.000000 tkinter_tooltip-3.1.0/tkinter_tooltip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-11 17:50:51.000000 tkinter_tooltip-3.1.0/tkinter_tooltip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-11 17:50:51.000000 tkinter_tooltip-3.1.0/tkinter_tooltip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:50:51.844919 tkinter_tooltip-3.1.0/tktooltip/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/tktooltip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-11 17:50:51.000000 tkinter_tooltip-3.1.0/tktooltip/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/tktooltip/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-11 17:50:47.000000 tkinter_tooltip-3.1.0/tktooltip/version.py
```

### Comparing `tkinter-tooltip-3.0.0/.github/FUNDING.yml` & `tkinter_tooltip-3.1.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/.github/workflows/codeql-analysis.yml` & `tkinter_tooltip-3.1.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/.github/workflows/main.yml` & `tkinter_tooltip-3.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/.github/workflows/python-publish.yml` & `tkinter_tooltip-3.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/.pre-commit-config.yaml` & `tkinter_tooltip-3.1.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-added-large-files
         args: ['--maxkb=2000']
 -   repo: https://github.com/PyCQA/flake8
     rev: 7.0.0
     hooks:
     - id: flake8
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.2
     hooks:
     -   id: pyupgrade
 -   repo: https://github.com/pycqa/isort
     rev: 5.13.2
     hooks:
     -   id: isort
         name: isort (python)
 -   repo: https://github.com/psf/black
-    rev: 24.1.1
+    rev: 24.4.2
     hooks:
     -   id: black
```

### Comparing `tkinter-tooltip-3.0.0/CONTRIBUTING.md` & `tkinter_tooltip-3.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/LICENSE` & `tkinter_tooltip-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/PKG-INFO` & `tkinter_tooltip-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkinter-tooltip
-Version: 3.0.0
+Version: 3.1.0
 Summary: An easy and customisable ToolTip implementation for Tkinter
 Home-page: https://github.com/gnikit/tkinter-tooltip
 Author: Giannis Nikiteas
 Author-email: giannis.nikiteas@gmail.com
 License: MIT
 Project-URL: Documentation, https://gnikit.github.io/tkinter-tooltip
 Project-URL: Repository, https://github.com/gnikit/tkinter-tooltip
@@ -35,22 +35,22 @@
 Provides-Extra: dev
 Requires-Dist: pytest>=5.4.3; extra == "dev"
 Requires-Dist: pytest-cov>=2.12.1; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: sphinx>=4.0.0; extra == "docs"
-Requires-Dist: sphinx-argparse; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
-Requires-Dist: sphinx_design; extra == "docs"
-Requires-Dist: sphinx-copybutton; extra == "docs"
-Requires-Dist: furo; extra == "docs"
-Requires-Dist: myst-parser; extra == "docs"
-Requires-Dist: sphinx-sitemap; extra == "docs"
+Requires-Dist: sphinx>=7.3.7; extra == "docs"
+Requires-Dist: sphinx-argparse>=0.4.0; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints>=2.1.0; extra == "docs"
+Requires-Dist: sphinx_design>=0.5.0; extra == "docs"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "docs"
+Requires-Dist: furo>=2024.5.6; extra == "docs"
+Requires-Dist: myst-parser>=3.0.1; extra == "docs"
+Requires-Dist: sphinx-sitemap>=2.5.1; extra == "docs"
 Provides-Extra: examples
 Requires-Dist: sv-ttk; extra == "examples"
 Requires-Dist: Pillow; extra == "examples"
 
 <div align="center">
 
 [![Downloads](https://pepy.tech/badge/tkinter-tooltip)](https://pepy.tech/project/tkinter-tooltip)
```

### Comparing `tkinter-tooltip-3.0.0/README.md` & `tkinter_tooltip-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/assets/animations/color-changer.gif` & `tkinter_tooltip-3.1.0/assets/animations/color-changer.gif`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/assets/animations/color-changer.mp4` & `tkinter_tooltip-3.1.0/assets/animations/color-changer.mp4`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/assets/animations/tooltip-delayed.gif` & `tkinter_tooltip-3.1.0/assets/animations/tooltip-delayed.gif`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/assets/animations/tooltip-tracking.gif` & `tkinter_tooltip-3.1.0/assets/animations/tooltip-tracking.gif`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/assets/animations/tootip-dark-theme.gif` & `tkinter_tooltip-3.1.0/assets/animations/tootip-dark-theme.gif`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/assets/animations/tootip-function-refresh.gif` & `tkinter_tooltip-3.1.0/assets/animations/tootip-function-refresh.gif`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/assets/animations/tootip-function.gif` & `tkinter_tooltip-3.1.0/assets/animations/tootip-function.gif`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/assets/images/header.png` & `tkinter_tooltip-3.1.0/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/assets/images/tooltip_logo.svg` & `tkinter_tooltip-3.1.0/assets/images/tooltip_logo.svg`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/assets/images/tootil-simple.png` & `tkinter_tooltip-3.1.0/assets/images/tootil-simple.png`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/docs/Makefile` & `tkinter_tooltip-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/docs/conf.py` & `tkinter_tooltip-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/docs/contributing.rst` & `tkinter_tooltip-3.1.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/docs/index.rst` & `tkinter_tooltip-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/docs/make.bat` & `tkinter_tooltip-3.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/examples/color_changer.py` & `tkinter_tooltip-3.1.0/examples/color_changer.py`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/examples/matrix.py` & `tkinter_tooltip-3.1.0/examples/matrix.py`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/examples/tooltip_destroy.py` & `tkinter_tooltip-3.1.0/examples/tooltip_destroy.py`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/examples/tooltip_logo.png` & `tkinter_tooltip-3.1.0/examples/tooltip_logo.png`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/setup.cfg` & `tkinter_tooltip-3.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -54,22 +54,22 @@
 dev = 
 	pytest >= 5.4.3
 	pytest-cov >= 2.12.1
 	black
 	isort
 	pre-commit
 docs = 
-	sphinx >= 4.0.0
-	sphinx-argparse
-	sphinx-autodoc-typehints
-	sphinx_design
-	sphinx-copybutton
-	furo
-	myst-parser
-	sphinx-sitemap
+	sphinx >= 7.3.7
+	sphinx-argparse >= 0.4.0
+	sphinx-autodoc-typehints >= 2.1.0
+	sphinx_design >= 0.5.0
+	sphinx-copybutton >= 0.5.2
+	furo >= 2024.5.6
+	myst-parser >= 3.0.1
+	sphinx-sitemap >= 2.5.1
 examples = 
 	sv-ttk
 	Pillow
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203, E722
```

### Comparing `tkinter-tooltip-3.0.0/test/test_tktooltip.py` & `tkinter_tooltip-3.1.0/test/test_tktooltip.py`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/tkinter_tooltip.egg-info/PKG-INFO` & `tkinter_tooltip-3.1.0/tkinter_tooltip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkinter-tooltip
-Version: 3.0.0
+Version: 3.1.0
 Summary: An easy and customisable ToolTip implementation for Tkinter
 Home-page: https://github.com/gnikit/tkinter-tooltip
 Author: Giannis Nikiteas
 Author-email: giannis.nikiteas@gmail.com
 License: MIT
 Project-URL: Documentation, https://gnikit.github.io/tkinter-tooltip
 Project-URL: Repository, https://github.com/gnikit/tkinter-tooltip
@@ -35,22 +35,22 @@
 Provides-Extra: dev
 Requires-Dist: pytest>=5.4.3; extra == "dev"
 Requires-Dist: pytest-cov>=2.12.1; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: sphinx>=4.0.0; extra == "docs"
-Requires-Dist: sphinx-argparse; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
-Requires-Dist: sphinx_design; extra == "docs"
-Requires-Dist: sphinx-copybutton; extra == "docs"
-Requires-Dist: furo; extra == "docs"
-Requires-Dist: myst-parser; extra == "docs"
-Requires-Dist: sphinx-sitemap; extra == "docs"
+Requires-Dist: sphinx>=7.3.7; extra == "docs"
+Requires-Dist: sphinx-argparse>=0.4.0; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints>=2.1.0; extra == "docs"
+Requires-Dist: sphinx_design>=0.5.0; extra == "docs"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "docs"
+Requires-Dist: furo>=2024.5.6; extra == "docs"
+Requires-Dist: myst-parser>=3.0.1; extra == "docs"
+Requires-Dist: sphinx-sitemap>=2.5.1; extra == "docs"
 Provides-Extra: examples
 Requires-Dist: sv-ttk; extra == "examples"
 Requires-Dist: Pillow; extra == "examples"
 
 <div align="center">
 
 [![Downloads](https://pepy.tech/badge/tkinter-tooltip)](https://pepy.tech/project/tkinter-tooltip)
```

### Comparing `tkinter-tooltip-3.0.0/tkinter_tooltip.egg-info/SOURCES.txt` & `tkinter_tooltip-3.1.0/tkinter_tooltip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tkinter-tooltip-3.0.0/tktooltip/tooltip.py` & `tkinter_tooltip-3.1.0/tktooltip/tooltip.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
         self.refresh = refresh
         self.x_offset = x_offset
         self.y_offset = y_offset
         # visibility status of the ToolTip inside|outside|visible
         self.status = ToolTipStatus.OUTSIDE
         self.last_moved = 0
         # use Message widget to host ToolTip
-        self.message_kwargs: dict = message_kwargs or self.DEFAULT_MESSAGE_KWARGS
+        self.message_kwargs: dict = self.DEFAULT_MESSAGE_KWARGS.copy()
+        self.message_kwargs.update(message_kwargs)
         self.message_widget = tk.Message(
             self,
             textvariable=self.msg_var,
             **self.message_kwargs,
         )
         self.message_widget.grid()
         self.bindigs = self._init_bindings()
```

