# Comparing `tmp/countdown-cli-1.0.2.tar.gz` & `tmp/countdown_cli-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countdown-cli-1.0.2.tar", max compression
+gzip compressed data, was "countdown_cli-1.0.3.tar", max compression
```

## Comparing `countdown-cli-1.0.2.tar` & `countdown_cli-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0     1083 2022-02-08 05:29:02.677960 countdown-cli-1.0.2/LICENSE.rst
--rw-r--r--   0        0        0     3982 2022-02-08 05:29:12.894809 countdown-cli-1.0.2/README.rst
--rw-r--r--   0        0        0     1780 2022-02-08 05:29:12.894809 countdown-cli-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      220 2022-02-08 05:29:02.677960 countdown-cli-1.0.2/src/countdown/__init__.py
--rw-r--r--   0        0        0     4073 2022-02-08 05:29:02.677960 countdown-cli-1.0.2/src/countdown/__main__.py
--rw-r--r--   0        0        0        0 2022-02-08 05:29:02.677960 countdown-cli-1.0.2/src/countdown/py.typed
--rw-r--r--   0        0        0     4953 2022-02-08 05:29:14.692326 countdown-cli-1.0.2/setup.py
--rw-r--r--   0        0        0     4873 2022-02-08 05:29:14.692639 countdown-cli-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-05-10 22:46:10.969748 countdown_cli-1.0.3/LICENSE.rst
+-rw-r--r--   0        0        0     3813 2024-05-10 22:46:20.265724 countdown_cli-1.0.3/README.rst
+-rw-r--r--   0        0        0     1795 2024-05-10 22:46:20.265724 countdown_cli-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      220 2024-05-10 22:46:10.969748 countdown_cli-1.0.3/src/countdown/__init__.py
+-rw-r--r--   0        0        0     3968 2024-05-10 22:46:20.265724 countdown_cli-1.0.3/src/countdown/__main__.py
+-rw-r--r--   0        0        0     4695 1970-01-01 00:00:00.000000 countdown_cli-1.0.3/PKG-INFO
```

### Comparing `countdown-cli-1.0.2/LICENSE.rst` & `countdown_cli-1.0.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `countdown-cli-1.0.2/README.rst` & `countdown_cli-1.0.3/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 countdown-cli
 =============
 
 |PyPI| |Status| |Python Version| |License|
 
-|Read the Docs| |Tests| |Codecov|
+|Tests| |Codecov|
 
 |pre-commit| |Black|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/countdown-cli.svg
    :target: https://pypi.org/project/countdown-cli/
    :alt: PyPI
 .. |Status| image:: https://img.shields.io/pypi/status/countdown-cli.svg
@@ -15,17 +15,14 @@
    :alt: Status
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/countdown-cli
    :target: https://pypi.org/project/countdown-cli
    :alt: Python Version
 .. |License| image:: https://img.shields.io/pypi/l/countdown-cli
    :target: https://opensource.org/licenses/MIT
    :alt: License
-.. |Read the Docs| image:: https://img.shields.io/readthedocs/countdown-cli/latest.svg?label=Read%20the%20Docs
-   :target: https://countdown-cli.readthedocs.io/
-   :alt: Read the documentation at https://countdown-cli.readthedocs.io/
 .. |Tests| image:: https://github.com/treyhunner/countdown-cli/workflows/Tests/badge.svg
    :target: https://github.com/treyhunner/countdown-cli/actions?workflow=Tests
    :alt: Tests
 .. |Codecov| image:: https://codecov.io/gh/treyhunner/countdown-cli/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/treyhunner/countdown-cli
    :alt: Codecov
 .. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
@@ -36,35 +33,39 @@
    :alt: Black
 
 This project is based on a `Python Morsels`_ exercise for a command-line countdown timer.
 If you're working on that exercise right now, please **don't look at the source code** for this. 😉
 
 |Logo|
 
-.. |Logo| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/docs/images/python-morsels-logo.png
+.. |Logo| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/images/python-morsels-logo.png
    :target: https://www.pythonmorsels.com
    :width: 400
    :alt: an adorable snake taking a bite out of a cookie with the words Python Morsels next to it (Python Morsels logo)
 
+Wondering how this package works?
+**Don't look at the source code just yet!**
+Instead, try implementing this package with the `Python Morsels "countdown" exercise <https://www.pythonmorsels.com/exercises/fc3be8467c634f978eae0c315f5677d1/>`_!
+
 
 Features
 --------
 
 * Full-screen countdown timer, centered in the terminal window
 * Command-line interface for Linux/Mac/Windows
 
 |32:53|
 
 |14:57|
 
-.. |32:53| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/docs/images/3253.png
+.. |32:53| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/images/3253.png
    :width: 500
    :alt: 32:53 shown in large letters in center of an xterm window (black background with white text)
 
-.. |14:57| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/docs/images/1457.png
+.. |14:57| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/images/1457.png
    :width: 500
    :alt: 14:57 shown in large letters in center of terminal window (light background with darker text)
 
 
 Requirements
 ------------
 
@@ -77,20 +78,14 @@
 You can install *countdown-cli* via pip_ from PyPI_:
 
 .. code:: console
 
    $ python3 -m pip install countdown-cli
 
 
-Usage
------
-
-Please see the `Command-line Reference <Usage_>`_ for details.
-
-
 Contributing
 ------------
 
 Contributions are very welcome.
 To learn more, see the `Contributor Guide`_.
 
 
@@ -119,8 +114,7 @@
 .. _MIT license: https://opensource.org/licenses/MIT
 .. _PyPI: https://pypi.org/project/countdown-cli/
 .. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 .. _file an issue: https://github.com/treyhunner/countdown-cli/issues
 .. _pip: https://pip.pypa.io/
 .. github-only
 .. _Contributor Guide: CONTRIBUTING.rst
-.. _Usage: https://countdown-cli.readthedocs.io/en/latest/usage.html
```

### Comparing `countdown-cli-1.0.2/pyproject.toml` & `countdown_cli-1.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,67 @@
 [tool.poetry]
 name = "countdown-cli"
-version = "1.0.2"
+version = "1.0.3"
 description = "Terminal program to display countdown timer"
 authors = ["Trey Hunner <trey@treyhunner.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/treyhunner/countdown-cli"
 repository = "https://github.com/treyhunner/countdown-cli"
-documentation = "https://countdown-cli.readthedocs.io"
 packages = [
     { include = "countdown", from = "src" },
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/treyhunner/countdown-cli/releases"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 click = "^8.0.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0.0"
-coverage = {extras = ["toml"], version = "^6.2"}
-safety = "^1.10.3"
-mypy = "^0.931"
-typeguard = "^2.13.3"
-xdoctest = {extras = ["colors"], version = "^0.15.10"}
-sphinx = "^4.3.2"
-sphinx-autobuild = ">=2021.3.14"
+pytest = "^8.2.0"
+coverage = {extras = ["toml"], version = "^7.5.1"}
 pre-commit = "^2.16.0"
-flake8 = "^4.0.1"
-black = ">=21.10b0"
-flake8-bandit = "^2.1.2"
-flake8-bugbear = "^22.1.11"
-flake8-docstrings = "^1.6.0"
-flake8-rst-docstrings = "^0.2.5"
-pep8-naming = "^0.12.1"
-darglint = "^1.8.1"
-reorder-python-imports = "^2.6.0"
-pre-commit-hooks = "^4.1.0"
-sphinx-click = "^3.0.2"
-Pygments = "^2.11.2"
-pyupgrade = "^2.31.0"
-furo = ">=2021.11.12"
+flake8 = "^7.0.0"
+black = "^24.4.2"
+flake8-bandit = "^4.1.1"
+flake8-bugbear = "^24.4.26"
+flake8-docstrings = "^1.7.0"
+flake8-rst-docstrings = "^0.3.0"
+pep8-naming = "^0.13.3"
+reorder-python-imports = "^3.12.0"
+pre-commit-hooks = "^4.6.0"
+docutils = { version = "!=0.21.post1", optional = true }
 
 [tool.poetry.scripts]
 countdown = "countdown.__main__:main"
 
+[tool.poetry.group.dev.dependencies]
+tomli = "^2.0.1"
+
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
 source = ["countdown", "tests"]
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 100
+fail_under = 96
 
 [tool.mypy]
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
```

### Comparing `countdown-cli-1.0.2/src/countdown/__main__.py` & `countdown_cli-1.0.3/src/countdown/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Command-line interface."""
-from __future__ import annotations
 
 import re
 import shutil
 import sys
 import time
 
 import click
@@ -42,36 +41,36 @@
     "8": " ████ \n██  ██\n ████ \n██  ██\n ████ ",
     "9": "██████\n██  ██\n██████\n    ██\n █████",
     ":": "  \n██\n  \n██\n  ",
 }
 CLEAR = "\033[H\033[J"
 
 
-def duration(string: str) -> int:
+def duration(string):
     """Convert given XmXs string to seconds (as an integer)."""
     match = DURATION_RE.search(string)
     if not match:
         raise ValueError(f"Invalid duration: {string}")
     minutes, seconds = match.groups()
     return int(minutes or 0) * 60 + int(seconds or 0)
 
 
 @click.command()
 @click.version_option(package_name="countdown-cli")
 @click.argument("duration", type=duration)
-def main(duration: int) -> None:
+def main(duration):
     """Countdown from the given duration to 0.
 
     DURATION should be a number followed by m or s for minutes or seconds.
 
     Examples of DURATION:
 
     \b
     - 5m (5 minutes)
-    - 45s (30 seconds)
+    - 45s (45 seconds)
     - 2m30s (2 minutes and 30 seconds)
     """  # noqa: D301
     enable_ansi_escape_codes()
     print(ENABLE_ALT_BUFFER + HIDE_CURSOR, end="")
     try:
         for n in range(duration, -1, -1):
             lines = get_number_lines(n)
@@ -79,15 +78,15 @@
             time.sleep(1)
     except KeyboardInterrupt:
         pass
     finally:
         print(SHOW_CURSOR + DISABLE_ALT_BUFFER, end="")
 
 
-def enable_ansi_escape_codes() -> None:
+def enable_ansi_escape_codes():
     """If running on Windows, enable ANSI escape codes."""
     if sys.platform == "win32":  # pragma: no cover
         from ctypes import windll
 
         k = windll.kernel32
         stdout = -11
         enable_processed_output = 0x0001
@@ -97,25 +96,25 @@
             k.GetStdHandle(stdout),
             enable_processed_output
             | enable_wrap_at_eol_output
             | enable_virtual_terminal_processing,
         )
 
 
-def print_full_screen(lines: list[str]) -> None:
+def print_full_screen(lines):
     """Print the given lines centered in the middle of the terminal window."""
     width, height = shutil.get_terminal_size()
     width -= max(len(line) for line in lines)
     height -= len(lines) + 2
     vertical_pad = "\n" * (height // 2)
     padded_text = "\n".join(" " * (width // 2) + line for line in lines)
     print(CLEAR + vertical_pad + padded_text, flush=True)
 
 
-def get_number_lines(seconds: int) -> list[str]:
+def get_number_lines(seconds):
     """Return list of lines which make large MM:SS glyphs for given seconds."""
     lines = [""] * 5
     minutes, seconds = divmod(seconds, 60)
     time = f"{minutes:02d}:{seconds:02d}"
     for char in time:
         char_lines = CHARS[char].splitlines()
         for i, line in enumerate(char_lines):
```

### Comparing `countdown-cli-1.0.2/setup.py` & `countdown_cli-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,143 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: countdown-cli
+Version: 1.0.3
+Summary: Terminal program to display countdown timer
+Home-page: https://github.com/treyhunner/countdown-cli
+License: MIT
+Author: Trey Hunner
+Author-email: trey@treyhunner.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: click (>=8.0.1,<9.0.0)
+Project-URL: Changelog, https://github.com/treyhunner/countdown-cli/releases
+Project-URL: Repository, https://github.com/treyhunner/countdown-cli
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+countdown-cli
+=============
 
-packages = \
-['countdown']
+|PyPI| |Status| |Python Version| |License|
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.0.1,<9.0.0']
-
-entry_points = \
-{'console_scripts': ['countdown = countdown.__main__:main']}
-
-setup_kwargs = {
-    'name': 'countdown-cli',
-    'version': '1.0.2',
-    'description': 'Terminal program to display countdown timer',
-    'long_description': "countdown-cli\n=============\n\n|PyPI| |Status| |Python Version| |License|\n\n|Read the Docs| |Tests| |Codecov|\n\n|pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/countdown-cli.svg\n   :target: https://pypi.org/project/countdown-cli/\n   :alt: PyPI\n.. |Status| image:: https://img.shields.io/pypi/status/countdown-cli.svg\n   :target: https://pypi.org/project/countdown-cli/\n   :alt: Status\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/countdown-cli\n   :target: https://pypi.org/project/countdown-cli\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/countdown-cli\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/countdown-cli/latest.svg?label=Read%20the%20Docs\n   :target: https://countdown-cli.readthedocs.io/\n   :alt: Read the documentation at https://countdown-cli.readthedocs.io/\n.. |Tests| image:: https://github.com/treyhunner/countdown-cli/workflows/Tests/badge.svg\n   :target: https://github.com/treyhunner/countdown-cli/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/treyhunner/countdown-cli/branch/main/graph/badge.svg\n   :target: https://codecov.io/gh/treyhunner/countdown-cli\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\nThis project is based on a `Python Morsels`_ exercise for a command-line countdown timer.\nIf you're working on that exercise right now, please **don't look at the source code** for this. 😉\n\n|Logo|\n\n.. |Logo| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/docs/images/python-morsels-logo.png\n   :target: https://www.pythonmorsels.com\n   :width: 400\n   :alt: an adorable snake taking a bite out of a cookie with the words Python Morsels next to it (Python Morsels logo)\n\n\nFeatures\n--------\n\n* Full-screen countdown timer, centered in the terminal window\n* Command-line interface for Linux/Mac/Windows\n\n|32:53|\n\n|14:57|\n\n.. |32:53| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/docs/images/3253.png\n   :width: 500\n   :alt: 32:53 shown in large letters in center of an xterm window (black background with white text)\n\n.. |14:57| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/docs/images/1457.png\n   :width: 500\n   :alt: 14:57 shown in large letters in center of terminal window (light background with darker text)\n\n\nRequirements\n------------\n\n* Python 3.7+\n\n\nInstallation\n------------\n\nYou can install *countdown-cli* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ python3 -m pip install countdown-cli\n\n\nUsage\n-----\n\nPlease see the `Command-line Reference <Usage_>`_ for details.\n\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_.\n\n\nLicense\n-------\n\nDistributed under the terms of the `MIT license`_,\n*countdown-cli* is free and open source software.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue`_ along with a detailed description.\n\n\nCredits\n-------\n\nThis project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.\n\n.. _Python Morsels: https://www.pythonmorsels.com\n.. _@cjolowicz: https://github.com/cjolowicz\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _MIT license: https://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/project/countdown-cli/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _file an issue: https://github.com/treyhunner/countdown-cli/issues\n.. _pip: https://pip.pypa.io/\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Usage: https://countdown-cli.readthedocs.io/en/latest/usage.html\n",
-    'author': 'Trey Hunner',
-    'author_email': 'trey@treyhunner.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/treyhunner/countdown-cli',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+|Tests| |Codecov|
 
+|pre-commit| |Black|
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/countdown-cli.svg
+   :target: https://pypi.org/project/countdown-cli/
+   :alt: PyPI
+.. |Status| image:: https://img.shields.io/pypi/status/countdown-cli.svg
+   :target: https://pypi.org/project/countdown-cli/
+   :alt: Status
+.. |Python Version| image:: https://img.shields.io/pypi/pyversions/countdown-cli
+   :target: https://pypi.org/project/countdown-cli
+   :alt: Python Version
+.. |License| image:: https://img.shields.io/pypi/l/countdown-cli
+   :target: https://opensource.org/licenses/MIT
+   :alt: License
+.. |Tests| image:: https://github.com/treyhunner/countdown-cli/workflows/Tests/badge.svg
+   :target: https://github.com/treyhunner/countdown-cli/actions?workflow=Tests
+   :alt: Tests
+.. |Codecov| image:: https://codecov.io/gh/treyhunner/countdown-cli/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/treyhunner/countdown-cli
+   :alt: Codecov
+.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Black
+
+This project is based on a `Python Morsels`_ exercise for a command-line countdown timer.
+If you're working on that exercise right now, please **don't look at the source code** for this. 😉
+
+|Logo|
+
+.. |Logo| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/images/python-morsels-logo.png
+   :target: https://www.pythonmorsels.com
+   :width: 400
+   :alt: an adorable snake taking a bite out of a cookie with the words Python Morsels next to it (Python Morsels logo)
+
+Wondering how this package works?
+**Don't look at the source code just yet!**
+Instead, try implementing this package with the `Python Morsels "countdown" exercise <https://www.pythonmorsels.com/exercises/fc3be8467c634f978eae0c315f5677d1/>`_!
+
+
+Features
+--------
+
+* Full-screen countdown timer, centered in the terminal window
+* Command-line interface for Linux/Mac/Windows
+
+|32:53|
+
+|14:57|
+
+.. |32:53| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/images/3253.png
+   :width: 500
+   :alt: 32:53 shown in large letters in center of an xterm window (black background with white text)
+
+.. |14:57| image:: https://raw.githubusercontent.com/treyhunner/countdown-cli/main/images/1457.png
+   :width: 500
+   :alt: 14:57 shown in large letters in center of terminal window (light background with darker text)
+
+
+Requirements
+------------
+
+* Python 3.7+
+
+
+Installation
+------------
+
+You can install *countdown-cli* via pip_ from PyPI_:
+
+.. code:: console
+
+   $ python3 -m pip install countdown-cli
+
+
+Contributing
+------------
+
+Contributions are very welcome.
+To learn more, see the `Contributor Guide`_.
+
+
+License
+-------
+
+Distributed under the terms of the `MIT license`_,
+*countdown-cli* is free and open source software.
+
+
+Issues
+------
+
+If you encounter any problems,
+please `file an issue`_ along with a detailed description.
+
+
+Credits
+-------
+
+This project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.
+
+.. _Python Morsels: https://www.pythonmorsels.com
+.. _@cjolowicz: https://github.com/cjolowicz
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _MIT license: https://opensource.org/licenses/MIT
+.. _PyPI: https://pypi.org/project/countdown-cli/
+.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+.. _file an issue: https://github.com/treyhunner/countdown-cli/issues
+.. _pip: https://pip.pypa.io/
+.. github-only
+.. _Contributor Guide: CONTRIBUTING.rst
 
-setup(**setup_kwargs)
```

