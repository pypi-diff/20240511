# Comparing `tmp/hikari-tanjun-2.8.1a1.tar.gz` & `tmp/hikari-tanjun-2.9.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari-tanjun-2.8.1a1.tar", last modified: Mon Oct 24 17:34:42 2022, max compression
+gzip compressed data, was "hikari-tanjun-2.9.0a1.tar", last modified: Tue Nov  8 06:49:44 2022, max compression
```

## Comparing `hikari-tanjun-2.8.1a1.tar` & `hikari-tanjun-2.9.0a1.tar`

### file list

```diff
@@ -1,148 +1,149 @@
--rw-r--r--   0        0        0      320 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.codeclimate.yml
--rw-r--r--   0        0        0     1756 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.flake8
--rw-r--r--   0        0        0       14 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.gitattributes
--rw-r--r--   0        0        0       26 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.github/CODEOWNERS
--rw-r--r--   0        0        0       45 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.github/FUNDING.yml
--rw-r--r--   0        0        0      600 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.github/dependabot.yml
--rw-r--r--   0        0        0      524 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.github/pull_request_template.md
--rw-r--r--   0        0        0      628 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.github/workflows/check-dependencies.yml
--rw-r--r--   0        0        0     3457 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.github/workflows/checks.yml
--rw-r--r--   0        0        0     1016 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.github/workflows/publish-docs.yml
--rw-r--r--   0        0        0      758 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      793 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.github/workflows/upgrade-dev-deps.yml
--rw-r--r--   0        0        0     1736 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.gitignore
--rw-r--r--   0        0        0      508 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    40705 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/CHANGELOG.md
--rw-r--r--   0        0        0     5220 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     6399 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1520 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/LICENSE
--rw-r--r--   0        0        0     1324 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/README.md
--rw-r--r--   0        0        0      146 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/docs.in
--rw-r--r--   0        0        0     1726 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/docs.txt
--rw-r--r--   0        0        0     1372 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/flake8.in
--rw-r--r--   0        0        0     3144 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/flake8.txt
--rw-r--r--   0        0        0       36 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/lint.in
--rw-r--r--   0        0        0      346 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/lint.txt
--rw-r--r--   0        0        0       28 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/nox.in
--rw-r--r--   0        0        0      886 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/nox.txt
--rw-r--r--   0        0        0       29 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/publish.in
--rw-r--r--   0        0        0      917 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/publish.txt
--rw-r--r--   0        0        0      146 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/reformat.in
--rw-r--r--   0        0        0      549 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/reformat.txt
--rw-r--r--   0        0        0      137 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/tests.in
--rw-r--r--   0        0        0     1179 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/tests.txt
--rw-r--r--   0        0        0       29 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/type-checking.in
--rw-r--r--   0        0        0      537 2022-10-24 17:34:14.938093 hikari-tanjun-2.8.1a1/dev-requirements/type-checking.txt
--rw-r--r--   0        0        0       24 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/CNAME
--rw-r--r--   0        0        0       17 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/changelog.md
--rw-r--r--   0        0        0       14 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/index.md
--rw-r--r--   0        0        0       29 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/abc.md
--rw-r--r--   0        0        0       45 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/annotations.md
--rw-r--r--   0        0        0       35 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/checks.md
--rw-r--r--   0        0        0       37 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/clients.md
--rw-r--r--   0        0        0      296 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/commands.md
--rw-r--r--   0        0        0       43 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/components.md
--rw-r--r--   0        0        0      372 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/context.md
--rw-r--r--   0        0        0       91 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/conversion.md
--rw-r--r--   0        0        0      667 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/dependencies.md
--rw-r--r--   0        0        0       35 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/errors.md
--rw-r--r--   0        0        0       33 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/hooks.md
--rw-r--r--   0        0        0       21 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/index.md
--rw-r--r--   0        0        0       37 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/parsing.md
--rw-r--r--   0        0        0       45 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/permissions.md
--rw-r--r--   0        0        0       41 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/schedules.md
--rw-r--r--   0        0        0       96 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/reference/utilities.md
--rw-r--r--   0        0        0    35514 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/docs/usage.md
--rw-r--r--   0        0        0     7048 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/LICENSE
--rw-r--r--   0        0        0      583 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/__init__.py
--rw-r--r--   0        0        0     3763 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/checks.py
--rw-r--r--   0        0        0      920 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/config.py
--rw-r--r--   0        0        0     5488 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/error_handling.py
--rw-r--r--   0        0        0     1578 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/impls.py
--rw-r--r--   0        0        0     4901 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/injection.py
--rw-r--r--   0        0        0     2809 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/message_commands.py
--rw-r--r--   0        0        0     1132 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/protos.py
--rw-r--r--   0        0        0     2513 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/run_gateway.py
--rw-r--r--   0        0        0     2821 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/run_rest.py
--rw-r--r--   0        0        0     7296 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/examples/slash_commands.py
--rw-r--r--   0        0        0     1718 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/mkdocs.yml
--rw-r--r--   0        0        0    11990 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/noxfile.py
--rw-r--r--   0        0        0     3546 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/pyproject.toml
--rw-r--r--   0        0        0    11253 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/tanjun/__init__.py
--rw-r--r--   0        0        0    11142 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/tanjun/_internal/__init__.py
--rw-r--r--   0        0        0    11303 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/tanjun/_internal/localisation.py
--rw-r--r--   0        0        0      156 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/tanjun/_internal/vendor/__init__.py
--rw-r--r--   0        0        0   123930 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/tanjun/_internal/vendor/inspect.py
--rw-r--r--   0        0        0    13931 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/tanjun/_internal/vendor/inspect.py.LICENSE
--rw-r--r--   0        0        0    12305 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/tanjun/_internal/vendor/inspect.pyi
--rw-r--r--   0        0        0    12657 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/tanjun/_internal/vendor/inspect.pyi.LICENSE
--rw-r--r--   0        0        0   168491 2022-10-24 17:34:14.942093 hikari-tanjun-2.8.1a1/tanjun/abc.py
--rw-r--r--   0        0        0    47917 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/annotations.py
--rw-r--r--   0        0        0    43134 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/checks.py
--rw-r--r--   0        0        0   117876 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/clients.py
--rw-r--r--   0        0        0     3245 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/commands/__init__.py
--rw-r--r--   0        0        0     4913 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/commands/base.py
--rw-r--r--   0        0        0    23678 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/commands/menu.py
--rw-r--r--   0        0        0    24079 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/commands/message.py
--rw-r--r--   0        0        0   112407 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/commands/slash.py
--rw-r--r--   0        0        0    50681 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/components.py
--rw-r--r--   0        0        0     2027 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/context/__init__.py
--rw-r--r--   0        0        0     8814 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/context/autocomplete.py
--rw-r--r--   0        0        0     6109 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/context/base.py
--rw-r--r--   0        0        0     7613 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/context/menu.py
--rw-r--r--   0        0        0    16348 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/context/message.py
--rw-r--r--   0        0        0    45583 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/context/slash.py
--rw-r--r--   0        0        0    46037 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/conversion.py
--rw-r--r--   0        0        0     4299 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/dependencies/__init__.py
--rw-r--r--   0        0        0    12969 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/dependencies/async_cache.py
--rw-r--r--   0        0        0     2962 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/dependencies/callbacks.py
--rw-r--r--   0        0        0    12259 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/dependencies/data.py
--rw-r--r--   0        0        0    40082 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/dependencies/limiters.py
--rw-r--r--   0        0        0     5819 2022-10-24 17:34:14.946093 hikari-tanjun-2.8.1a1/tanjun/dependencies/locales.py
--rw-r--r--   0        0        0     6992 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tanjun/dependencies/owners.py
--rw-r--r--   0        0        0    22509 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tanjun/dependencies/reloaders.py
--rw-r--r--   0        0        0    18429 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tanjun/errors.py
--rw-r--r--   0        0        0    13945 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tanjun/hooks.py
--rw-r--r--   0        0        0     4048 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tanjun/injecting.py
--rw-r--r--   0        0        0    74739 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tanjun/parsing.py
--rw-r--r--   0        0        0    12480 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tanjun/permissions.py
--rw-r--r--   0        0        0        0 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tanjun/py.typed
--rw-r--r--   0        0        0    41104 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tanjun/schedules.py
--rw-r--r--   0        0        0     2185 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tanjun/utilities.py
--rw-r--r--   0        0        0     1623 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/__init__.py
--rw-r--r--   0        0        0     1623 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/commands/__init__.py
--rw-r--r--   0        0        0     6143 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/commands/test_base.py
--rw-r--r--   0        0        0    22015 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/commands/test_menu.py
--rw-r--r--   0        0        0    35031 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/commands/test_message.py
--rw-r--r--   0        0        0   157979 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/commands/test_slash.py
--rw-r--r--   0        0        0     1623 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/context/__init__.py
--rw-r--r--   0        0        0    17226 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/context/test_autocomplete.py
--rw-r--r--   0        0        0     9593 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/context/test_base.py
--rw-r--r--   0        0        0    11240 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/context/test_menu.py
--rw-r--r--   0        0        0    21951 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/context/test_message.py
--rw-r--r--   0        0        0    49641 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/context/test_slash.py
--rw-r--r--   0        0        0     1623 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/dependencies/__init__.py
--rw-r--r--   0        0        0     2725 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/dependencies/test___init__.py
--rw-r--r--   0        0        0     4958 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/dependencies/test_callbacks.py
--rw-r--r--   0        0        0     9134 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/dependencies/test_data.py
--rw-r--r--   0        0        0   105806 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/dependencies/test_limiters.py
--rw-r--r--   0        0        0     5970 2022-10-24 17:34:14.950093 hikari-tanjun-2.8.1a1/tests/dependencies/test_locales.py
--rw-r--r--   0        0        0    14081 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/dependencies/test_owners.py
--rw-r--r--   0        0        0     2962 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/dependencies/test_reloaders.py
--rw-r--r--   0        0        0     5667 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test__internal.py
--rw-r--r--   0        0        0   172842 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_annotations.py
--rw-r--r--   0        0        0   169852 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_annotations_future_annotations.py
--rw-r--r--   0        0        0   173145 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_checks.py
--rw-r--r--   0        0        0   315953 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_clients.py
--rw-r--r--   0        0        0     7920 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_clients_future_annotations.py
--rw-r--r--   0        0        0    69919 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_components.py
--rw-r--r--   0        0        0     8496 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_components_future_annotations.py
--rw-r--r--   0        0        0    60500 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_conversion.py
--rw-r--r--   0        0        0     8123 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_errors.py
--rw-r--r--   0        0        0    12370 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_hooks.py
--rw-r--r--   0        0        0     2998 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_injecting.py
--rw-r--r--   0        0        0     3222 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_parsing.py
--rw-r--r--   0        0        0     4116 2022-10-24 17:34:14.954093 hikari-tanjun-2.8.1a1/tests/test_permissions.py
--rw-r--r--   0        0        0    73761 2022-10-24 17:34:14.958093 hikari-tanjun-2.8.1a1/tests/test_schedules.py
--rw-r--r--   0        0        0     2556 2022-10-24 17:34:14.958093 hikari-tanjun-2.8.1a1/tests/test_utilities.py
--rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 hikari-tanjun-2.8.1a1/PKG-INFO
+-rw-r--r--   0        0        0      320 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.codeclimate.yml
+-rw-r--r--   0        0        0       14 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.gitattributes
+-rw-r--r--   0        0        0       26 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.github/CODEOWNERS
+-rw-r--r--   0        0        0       45 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      647 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.github/dependabot.yml
+-rw-r--r--   0        0        0      524 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     3457 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     1018 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0      814 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      793 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.github/workflows/upgrade-dev-deps.yml
+-rw-r--r--   0        0        0     1736 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.gitignore
+-rw-r--r--   0        0        0      508 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    41853 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/CHANGELOG.md
+-rw-r--r--   0        0        0     5220 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     6399 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1520 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/LICENSE
+-rw-r--r--   0        0        0     1324 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/README.md
+-rw-r--r--   0        0        0      146 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/docs.in
+-rw-r--r--   0        0        0     1724 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/docs.txt
+-rw-r--r--   0        0        0     1448 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/flake8.in
+-rw-r--r--   0        0        0     3124 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/flake8.txt
+-rw-r--r--   0        0        0       36 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/lint.in
+-rw-r--r--   0        0        0      346 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/lint.txt
+-rw-r--r--   0        0        0       14 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/nox.in
+-rw-r--r--   0        0        0      518 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/nox.txt
+-rw-r--r--   0        0        0       29 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/publish.in
+-rw-r--r--   0        0        0      917 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/publish.txt
+-rw-r--r--   0        0        0      146 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/reformat.in
+-rw-r--r--   0        0        0      590 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/reformat.txt
+-rw-r--r--   0        0        0      139 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/tests.in
+-rw-r--r--   0        0        0     1096 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/tests.txt
+-rw-r--r--   0        0        0       29 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/type-checking.in
+-rw-r--r--   0        0        0      509 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/dev-requirements/type-checking.txt
+-rw-r--r--   0        0        0       24 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/CNAME
+-rw-r--r--   0        0        0       17 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/changelog.md
+-rw-r--r--   0        0        0       14 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/index.md
+-rw-r--r--   0        0        0       29 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/abc.md
+-rw-r--r--   0        0        0       45 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/annotations.md
+-rw-r--r--   0        0        0       35 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/checks.md
+-rw-r--r--   0        0        0       37 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/clients.md
+-rw-r--r--   0        0        0      290 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/commands.md
+-rw-r--r--   0        0        0       43 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/components.md
+-rw-r--r--   0        0        0      364 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/context.md
+-rw-r--r--   0        0        0       89 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/conversion.md
+-rw-r--r--   0        0        0      653 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/dependencies.md
+-rw-r--r--   0        0        0       35 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/errors.md
+-rw-r--r--   0        0        0       33 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/hooks.md
+-rw-r--r--   0        0        0       21 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/index.md
+-rw-r--r--   0        0        0       37 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/parsing.md
+-rw-r--r--   0        0        0       45 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/permissions.md
+-rw-r--r--   0        0        0       41 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/schedules.md
+-rw-r--r--   0        0        0       96 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/reference/utilities.md
+-rw-r--r--   0        0        0    35501 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/docs/usage.md
+-rw-r--r--   0        0        0     7048 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/LICENSE
+-rw-r--r--   0        0        0      583 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/__init__.py
+-rw-r--r--   0        0        0     3763 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/checks.py
+-rw-r--r--   0        0        0      920 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/config.py
+-rw-r--r--   0        0        0     5488 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/error_handling.py
+-rw-r--r--   0        0        0     1578 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/impls.py
+-rw-r--r--   0        0        0     4901 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/injection.py
+-rw-r--r--   0        0        0     2809 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/message_commands.py
+-rw-r--r--   0        0        0     1132 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/protos.py
+-rw-r--r--   0        0        0     2513 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/run_gateway.py
+-rw-r--r--   0        0        0     2294 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/run_rest.py
+-rw-r--r--   0        0        0     7296 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/examples/slash_commands.py
+-rw-r--r--   0        0        0     1695 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/mkdocs.yml
+-rw-r--r--   0        0        0    10083 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/noxfile.py
+-rw-r--r--   0        0        0     5078 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/pyproject.toml
+-rw-r--r--   0        0        0    10348 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/tanjun/__init__.py
+-rw-r--r--   0        0        0    11131 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/tanjun/_internal/__init__.py
+-rw-r--r--   0        0        0     3887 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/tanjun/_internal/cache.py
+-rw-r--r--   0        0        0    11303 2022-11-08 06:49:24.431493 hikari-tanjun-2.9.0a1/tanjun/_internal/localisation.py
+-rw-r--r--   0        0        0      156 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/_internal/vendor/__init__.py
+-rw-r--r--   0        0        0   123930 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/_internal/vendor/inspect.py
+-rw-r--r--   0        0        0    13931 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/_internal/vendor/inspect.py.LICENSE
+-rw-r--r--   0        0        0    12305 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/_internal/vendor/inspect.pyi
+-rw-r--r--   0        0        0    12657 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/_internal/vendor/inspect.pyi.LICENSE
+-rw-r--r--   0        0        0   168223 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/abc.py
+-rw-r--r--   0        0        0    47972 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/annotations.py
+-rw-r--r--   0        0        0    42306 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/checks.py
+-rw-r--r--   0        0        0   118485 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/clients.py
+-rw-r--r--   0        0        0     3245 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/commands/__init__.py
+-rw-r--r--   0        0        0     4913 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/commands/base.py
+-rw-r--r--   0        0        0    23678 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/commands/menu.py
+-rw-r--r--   0        0        0    24079 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/commands/message.py
+-rw-r--r--   0        0        0   112407 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/commands/slash.py
+-rw-r--r--   0        0        0    50681 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/components.py
+-rw-r--r--   0        0        0     2027 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/context/__init__.py
+-rw-r--r--   0        0        0     8814 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/context/autocomplete.py
+-rw-r--r--   0        0        0     6109 2022-11-08 06:49:24.435491 hikari-tanjun-2.9.0a1/tanjun/context/base.py
+-rw-r--r--   0        0        0     7613 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/context/menu.py
+-rw-r--r--   0        0        0    16172 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/context/message.py
+-rw-r--r--   0        0        0    45346 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/context/slash.py
+-rw-r--r--   0        0        0    46365 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/conversion.py
+-rw-r--r--   0        0        0     4299 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/dependencies/__init__.py
+-rw-r--r--   0        0        0    13019 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/dependencies/async_cache.py
+-rw-r--r--   0        0        0     2962 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/dependencies/callbacks.py
+-rw-r--r--   0        0        0    12259 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/dependencies/data.py
+-rw-r--r--   0        0        0    40315 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/dependencies/limiters.py
+-rw-r--r--   0        0        0     5819 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/dependencies/locales.py
+-rw-r--r--   0        0        0     6992 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/dependencies/owners.py
+-rw-r--r--   0        0        0    22509 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/dependencies/reloaders.py
+-rw-r--r--   0        0        0    18429 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/errors.py
+-rw-r--r--   0        0        0    13945 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/hooks.py
+-rw-r--r--   0        0        0     4048 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/injecting.py
+-rw-r--r--   0        0        0    74739 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/parsing.py
+-rw-r--r--   0        0        0    12242 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/permissions.py
+-rw-r--r--   0        0        0        0 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/py.typed
+-rw-r--r--   0        0        0    41104 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/schedules.py
+-rw-r--r--   0        0        0     2185 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tanjun/utilities.py
+-rw-r--r--   0        0        0     1623 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/__init__.py
+-rw-r--r--   0        0        0     1623 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/commands/__init__.py
+-rw-r--r--   0        0        0     6143 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/commands/test_base.py
+-rw-r--r--   0        0        0    22015 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/commands/test_menu.py
+-rw-r--r--   0        0        0    35031 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/commands/test_message.py
+-rw-r--r--   0        0        0   157979 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/commands/test_slash.py
+-rw-r--r--   0        0        0     1623 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/context/__init__.py
+-rw-r--r--   0        0        0    17226 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/context/test_autocomplete.py
+-rw-r--r--   0        0        0     9593 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/context/test_base.py
+-rw-r--r--   0        0        0    11240 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/context/test_menu.py
+-rw-r--r--   0        0        0    21795 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/context/test_message.py
+-rw-r--r--   0        0        0    49559 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/context/test_slash.py
+-rw-r--r--   0        0        0     1623 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/dependencies/__init__.py
+-rw-r--r--   0        0        0     2725 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/dependencies/test___init__.py
+-rw-r--r--   0        0        0     4958 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/dependencies/test_callbacks.py
+-rw-r--r--   0        0        0     9134 2022-11-08 06:49:24.439489 hikari-tanjun-2.9.0a1/tests/dependencies/test_data.py
+-rw-r--r--   0        0        0   110555 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/dependencies/test_limiters.py
+-rw-r--r--   0        0        0     5970 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/dependencies/test_locales.py
+-rw-r--r--   0        0        0    14081 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/dependencies/test_owners.py
+-rw-r--r--   0        0        0     2962 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/dependencies/test_reloaders.py
+-rw-r--r--   0        0        0     1623 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test__internal/__init__.py
+-rw-r--r--   0        0        0    18508 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test__internal/test_cache.py
+-rw-r--r--   0        0        0     5667 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test__internal/test_init.py
+-rw-r--r--   0        0        0   172842 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_annotations.py
+-rw-r--r--   0        0        0   169852 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_annotations_future_annotations.py
+-rw-r--r--   0        0        0   165625 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_checks.py
+-rw-r--r--   0        0        0   316974 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_clients.py
+-rw-r--r--   0        0        0     7920 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_clients_future_annotations.py
+-rw-r--r--   0        0        0    69919 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_components.py
+-rw-r--r--   0        0        0     8496 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_components_future_annotations.py
+-rw-r--r--   0        0        0    66064 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_conversion.py
+-rw-r--r--   0        0        0     8123 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_errors.py
+-rw-r--r--   0        0        0    12370 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_hooks.py
+-rw-r--r--   0        0        0     2998 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_injecting.py
+-rw-r--r--   0        0        0     3222 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_parsing.py
+-rw-r--r--   0        0        0     4116 2022-11-08 06:49:24.443487 hikari-tanjun-2.9.0a1/tests/test_permissions.py
+-rw-r--r--   0        0        0    73761 2022-11-08 06:49:24.447485 hikari-tanjun-2.9.0a1/tests/test_schedules.py
+-rw-r--r--   0        0        0     2556 2022-11-08 06:49:24.447485 hikari-tanjun-2.9.0a1/tests/test_utilities.py
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 hikari-tanjun-2.9.0a1/PKG-INFO
```

### Comparing `hikari-tanjun-2.8.1a1/.github/dependabot.yml` & `hikari-tanjun-2.9.0a1/.github/dependabot.yml`

 * *Files 21% similar despite different names*

```diff
@@ -5,11 +5,12 @@
 
 version: 2
 updates:
   - package-ecosystem: "pip" # See documentation for possible values
     directory: "/" # Location of package manifests
     schedule:
       interval: "weekly"
+    versioning-strategy: increase-if-necessary
   - package-ecosystem: "github-actions"
     directory: "/"
     schedule:
       interval: "weekly"
```

### Comparing `hikari-tanjun-2.8.1a1/.github/pull_request_template.md` & `hikari-tanjun-2.9.0a1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/.github/workflows/check-dependencies.yml` & `hikari-tanjun-2.9.0a1/.github/workflows/upgrade-dev-deps.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-name: Check dependencies
+name: Upgrade dev dependencies
 
 on:
-  push:
-    branches: [ master ]
-  pull_request:
-    branches: [ master ]
   schedule:
-    - cron: "0 12 * * 6"
+    - cron: "0 12 1 * *"
   workflow_dispatch:
 
 jobs:
-  check-dependencies:
+  upgrade-dev-deps:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python 3.9
         uses: actions/setup-python@v4
@@ -22,9 +18,16 @@
           python-version: 3.9
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./dev-requirements/nox.txt
 
-      - name: Check dependencies
-        run: python -m nox -s check-dependencies
+      - name: Upgrade dev dependencies
+        run: python -m nox -s upgrade-dev-deps
+
+      - name: Create Pull Request
+        uses: peter-evans/create-pull-request@v4
+        with:
+          branch: task/upgrade-dev-deps
+          commit-message: Upgrade dev dependencies
+          title: Upgrade dev dependencies
```

### Comparing `hikari-tanjun-2.8.1a1/.github/workflows/checks.yml` & `hikari-tanjun-2.9.0a1/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/.github/workflows/publish-docs.yml` & `hikari-tanjun-2.9.0a1/.github/workflows/publish-docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,22 @@
         with:
           python-version: 3.9
 
       - name: Install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./dev-requirements/nox.txt
+
       - name: Build docs
         id: doc_info
         run: |
           mkdir site
           python -m nox -s generate-docs -- -o ./site -j
           echo "::set-output name=GIT_HASH::$(git rev-parse HEAD)"
+
       - name: Push
         uses: s0/git-publish-subdir-action@develop
         env:
           REPO: self
           BRANCH: docs
           FOLDER: ./site
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `hikari-tanjun-2.8.1a1/.gitignore` & `hikari-tanjun-2.9.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/CHANGELOG.md` & `hikari-tanjun-2.9.0a1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [2.9.0a1] - 2022-11-08
+### Added
+- Added `bot_managed` argument to [Client.from_gateway_bot][tanjun.clients.Client.from_gateway_bot]
+  for automatically starting the client when the linked REST bot starts. This defaults to [False][]
+  for backwards compatibility.
+- Thread support (including a `SfCache[hikari.GuildThreadChannel]` concept).
+
+### Changed
+- Bumped the minimum Hikari version to `2.0.0.dev112`.
+- `SfCache[hikari.GuildChannel]` is now `SfCache[hikari.PermissibleGuildChannel]`.
+- Allow [None][] to be passed for `attachment` and `attachments` to edit response methods.
+
+### Fixed
+- The [ToChannel][tanjun.checks.ToChannel]/[to_channel][tanjun.checks.to_channel] converter
+  now correctly uses the registered async channel cache if set.
+
+### Removed
+- The project metadata dunder attributes from [tanjun][].
+  [importlib.metadata][] should be used to get this metadata instead.
+- `replace_attachments` argument from the relevant context edit response methods.
+  For more information see <https://github.com/hikari-py/hikari/releases/tag/2.0.0.dev112>.
 
 ## [2.8.1a1] - 2022-10-24
 ### Changed
 - No longer ignore `delete_after` for ephemeral responses.
 
 ## [2.8.0a1] - 2022-10-16
 ### Added
@@ -718,15 +739,16 @@
   for the slash context and message context to be interchaingable under the right circumstances.
 - Made the callback signatures more generic for commands and converters to allow for implementations to introduce
   features like dependency injection.
 
 ### Removed
 - Removed a lot of impl specific setting and with methods from the abstract interfaces to avoid
 
-[Unreleased]: https://github.com/FasterSpeeding/Tanjun/compare/v2.8.1a1...HEAD
+[Unreleased]: https://github.com/FasterSpeeding/Tanjun/compare/v2.9.0a1...HEAD
+[2.9.0a1]: https://github.com/FasterSpeeding/Tanjun/compare/v2.8.1a1...v2.9.0a1
 [2.8.1a1]: https://github.com/FasterSpeeding/Tanjun/compare/v2.8.0a1...v2.8.1a1
 [2.8.0a1]: https://github.com/FasterSpeeding/Tanjun/compare/v2.7.0a1...v2.8.0a1
 [2.7.0a1]: https://github.com/FasterSpeeding/Tanjun/compare/v2.6.3a1...v2.7.0a1
 [2.6.3a1]: https://github.com/FasterSpeeding/Tanjun/compare/v2.6.2a1...v2.6.3a1
 [2.6.2a1]: https://github.com/FasterSpeeding/Tanjun/compare/v2.6.1a1...v2.6.2a1
 [2.6.1a1]: https://github.com/FasterSpeeding/Tanjun/compare/v2.5.4a1...v2.6.1a1
 [2.5.4a1]: https://github.com/FasterSpeeding/Tanjun/compare/v2.5.3a1...v2.5.4a1
```

### Comparing `hikari-tanjun-2.8.1a1/CODE_OF_CONDUCT.md` & `hikari-tanjun-2.9.0a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/CONTRIBUTING.md` & `hikari-tanjun-2.9.0a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/LICENSE` & `hikari-tanjun-2.9.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/README.md` & `hikari-tanjun-2.9.0a1/README.md`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/dev-requirements/docs.txt` & `hikari-tanjun-2.9.0a1/dev-requirements/docs.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via requests
 charset-normalizer==2.1.1
     # via requests
 click==8.1.3
     # via mkdocs
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.22.2
+griffe==0.23.0
     # via mkdocstrings-python
 idna==3.4
     # via requests
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
@@ -33,37 +33,37 @@
     # via -r dev-requirements/docs.in
 markupsafe==2.1.1
     # via
     #   jinja2
     #   mkdocstrings
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.4.1
+mkdocs==1.4.2
     # via
     #   -r dev-requirements/docs.in
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-material==8.5.7
+mkdocs-material==8.5.8
     # via -r dev-requirements/docs.in
-mkdocs-material-extensions==1.0.3
+mkdocs-material-extensions==1.1
     # via mkdocs-material
 mkdocstrings[python]==0.19.0
     # via
     #   -r dev-requirements/docs.in
     #   mkdocstrings-python
 mkdocstrings-python==0.7.1
     # via mkdocstrings
 packaging==21.3
     # via mkdocs
 pygments==2.13.0
     # via mkdocs-material
-pymdown-extensions==9.6
+pymdown-extensions==9.7
     # via
     #   mkdocs-material
     #   mkdocstrings
 pyparsing==3.0.9
     # via packaging
 python-dateutil==2.8.2
     # via ghp-import
```

### Comparing `hikari-tanjun-2.8.1a1/dev-requirements/flake8.in` & `hikari-tanjun-2.9.0a1/dev-requirements/flake8.in`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-flake8==4.0.1
+flake8==5.0.4
+pyproject-flake8>5.0.0  # These are always pinned to the flake8 ver anyways
 
 # Flake8 plugins
 # Ref: https://github.com/DmytroLitvinov/awesome-flake8-extensions
 
-flake8-bandit==3.0.0             # runs bandit
+flake8-bandit==4.1.1             # runs bandit
 flake8-black==0.3.3              # runs black
 flake8-broken-line==0.6.0          # forbey "\" linebreaks
-flake8-builtins==2.0.0           # builtin shadowing checks
+flake8-builtins==2.0.1           # builtin shadowing checks
 flake8-coding==1.3.2             # coding magic-comment detection
-flake8-comprehensions==3.10.0       # comprehension checks
+flake8-comprehensions==3.10.1       # comprehension checks
 flake8-deprecated==2.0.1           # deprecated call checks
 flake8-docstrings==1.6         # pydocstyle support
 flake8-executable==2.1.2         # shebangs
 flake8-fixme==1.1.1              # "fix me" counter
 flake8-functions==0.0.7          # function linting
 flake8-html==0.4.2               # html output
 flake8-if-statements==1.0.0        # condition linting
```

### Comparing `hikari-tanjun-2.8.1a1/dev-requirements/flake8.txt` & `hikari-tanjun-2.9.0a1/dev-requirements/flake8.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # via flake8-bandit
 black==22.10.0
     # via flake8-black
 click==8.1.3
     # via
     #   black
     #   mr-proper
-flake8==4.0.1
+flake8==5.0.4
     # via
     #   -r dev-requirements/flake8.in
     #   flake8-bandit
     #   flake8-black
     #   flake8-broken-line
     #   flake8-builtins
     #   flake8-coding
@@ -26,29 +26,29 @@
     #   flake8-deprecated
     #   flake8-docstrings
     #   flake8-executable
     #   flake8-html
     #   flake8-isort
     #   flake8-mutable
     #   flake8-pep3101
-    #   flake8-polyfill
     #   flake8-print
     #   flake8-printf-formatting
     #   flake8-raise
-flake8-bandit==3.0.0
+    #   pyproject-flake8
+flake8-bandit==4.1.1
     # via -r dev-requirements/flake8.in
 flake8-black==0.3.3
     # via -r dev-requirements/flake8.in
 flake8-broken-line==0.6.0
     # via -r dev-requirements/flake8.in
-flake8-builtins==2.0.0
+flake8-builtins==2.0.1
     # via -r dev-requirements/flake8.in
 flake8-coding==1.3.2
     # via -r dev-requirements/flake8.in
-flake8-comprehensions==3.10.0
+flake8-comprehensions==3.10.1
     # via -r dev-requirements/flake8.in
 flake8-deprecated==2.0.1
     # via -r dev-requirements/flake8.in
 flake8-docstrings==1.6
     # via -r dev-requirements/flake8.in
 flake8-executable==2.1.2
     # via -r dev-requirements/flake8.in
@@ -66,67 +66,64 @@
     # via -r dev-requirements/flake8.in
 flake8-pep3101==2.0.0
     # via -r dev-requirements/flake8.in
 flake8-plugin-utils==1.3.2
     # via
     #   flake8-if-statements
     #   flake8-pytest-style
-flake8-polyfill==1.0.2
-    # via flake8-bandit
 flake8-print==5.0.0
     # via -r dev-requirements/flake8.in
 flake8-printf-formatting==1.1.2
     # via -r dev-requirements/flake8.in
 flake8-pytest-style==1.6.0
     # via -r dev-requirements/flake8.in
 flake8-raise==0.0.5
     # via -r dev-requirements/flake8.in
 gitdb==4.0.9
     # via gitpython
-gitpython==3.1.27
+gitpython==3.1.29
     # via bandit
 isort==5.10.1
     # via flake8-isort
 jinja2==3.1.2
     # via flake8-html
 markupsafe==2.1.1
     # via jinja2
-mccabe==0.6.1
+mccabe==0.7.0
     # via flake8
 mr-proper==0.0.7
     # via flake8-functions
 mypy-extensions==0.4.3
     # via black
 pathspec==0.10.1
     # via black
-pbr==5.10.0
+pbr==5.11.0
     # via stevedore
 platformdirs==2.5.2
     # via black
-pycodestyle==2.8.0
+pycodestyle==2.9.1
     # via
     #   flake8
-    #   flake8-bandit
     #   flake8-print
 pydocstyle==6.1.1
     # via flake8-docstrings
-pyflakes==2.4.0
+pyflakes==2.5.0
     # via flake8
 pygments==2.13.0
     # via flake8-html
+pyproject-flake8==5.0.4.post1
+    # via -r dev-requirements/flake8.in
 pyyaml==6.0
     # via bandit
 smmap==5.0.0
     # via gitdb
 snowballstemmer==2.2.0
     # via pydocstyle
 stdlib-list==0.8.0
     # via mr-proper
-stevedore==4.0.0
+stevedore==4.1.0
     # via bandit
 tomli==2.0.1
-    # via
-    #   black
-    #   flake8-black
+    # via flake8-black
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `hikari-tanjun-2.8.1a1/dev-requirements/nox.txt` & `hikari-tanjun-2.9.0a1/dev-requirements/nox.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,26 @@
 #
 # This file is autogenerated by pip-compile with python 3.9
 # To update, run:
 #
 #    pip-compile --output-file=dev-requirements/nox.txt dev-requirements/nox.in
 #
-anyio==3.6.1
-    # via httpcore
 argcomplete==2.0.0
     # via nox
-certifi==2022.9.24
-    # via
-    #   httpcore
-    #   httpx
 colorlog==6.7.0
     # via nox
 distlib==0.3.6
     # via virtualenv
 filelock==3.8.0
     # via virtualenv
-h11==0.12.0
-    # via httpcore
-httpcore==0.15.0
-    # via httpx
-httpx==0.23.0
-    # via -r dev-requirements/nox.in
-idna==3.4
-    # via
-    #   anyio
-    #   rfc3986
 nox==2022.8.7
     # via -r dev-requirements/nox.in
 packaging==21.3
     # via nox
 platformdirs==2.5.2
     # via virtualenv
 py==1.11.0
     # via nox
 pyparsing==3.0.9
     # via packaging
-rfc3986[idna2008]==1.5.0
-    # via httpx
-sniffio==1.3.0
-    # via
-    #   anyio
-    #   httpcore
-    #   httpx
-virtualenv==20.16.5
+virtualenv==20.16.6
     # via nox
```

### Comparing `hikari-tanjun-2.8.1a1/dev-requirements/publish.txt` & `hikari-tanjun-2.9.0a1/dev-requirements/publish.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with python 3.9
 # To update, run:
 #
 #    pip-compile --output-file=dev-requirements/publish.txt dev-requirements/publish.in
 #
-build==0.8.0
+build==0.9.0
     # via pip-tools
 certifi==2022.9.24
     # via requests
 charset-normalizer==2.1.1
     # via requests
 click==8.1.3
     # via pip-tools
```

### Comparing `hikari-tanjun-2.8.1a1/dev-requirements/reformat.txt` & `hikari-tanjun-2.9.0a1/dev-requirements/reformat.txt`

 * *Files 17% similar despite different names*

```diff
@@ -14,11 +14,13 @@
     # via black
 pathspec==0.10.1
     # via black
 platformdirs==2.5.2
     # via black
 sort-all==1.2.0
     # via -r dev-requirements/reformat.in
-tokenize-rt==4.2.1
+tokenize-rt==5.0.0
     # via sort-all
 tomli==2.0.1
     # via black
+typing-extensions==4.4.0
+    # via black
```

### Comparing `hikari-tanjun-2.8.1a1/dev-requirements/tests.txt` & `hikari-tanjun-2.9.0a1/dev-requirements/tests.txt`

 * *Files 26% similar despite different names*

```diff
@@ -4,47 +4,42 @@
 #
 #    pip-compile --output-file=dev-requirements/tests.txt dev-requirements/tests.in
 #
 attrs==22.1.0
     # via pytest
 coverage[toml]==6.5.0
     # via pytest-cov
+exceptiongroup==1.0.0
+    # via pytest
 execnet==1.9.0
     # via pytest-xdist
 freezegun==1.2.1
     # via -r dev-requirements/tests.in
 iniconfig==1.1.1
     # via pytest
 packaging==21.3
     # via pytest
 pluggy==1.0.0
     # via pytest
-py==1.11.0
-    # via
-    #   pytest
-    #   pytest-forked
 pyparsing==3.0.9
     # via packaging
-pytest==7.1.3
+pytest==7.2.0
     # via
     #   -r dev-requirements/tests.in
     #   pytest-asyncio
     #   pytest-cov
-    #   pytest-forked
     #   pytest-timeout
     #   pytest-xdist
 pytest-asyncio==0.20.1
     # via -r dev-requirements/tests.in
 pytest-cov==4.0.0
     # via -r dev-requirements/tests.in
-pytest-forked==1.4.0
-    # via pytest-xdist
 pytest-timeout==2.1.0
     # via -r dev-requirements/tests.in
-pytest-xdist==2.5
+pytest-xdist==3.0.2
     # via -r dev-requirements/tests.in
 python-dateutil==2.8.2
     # via freezegun
 six==1.16.0
     # via python-dateutil
 tomli==2.0.1
     # via
```

### Comparing `hikari-tanjun-2.8.1a1/docs/reference/dependencies.md` & `hikari-tanjun-2.9.0a1/docs/reference/dependencies.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # tanjun.dependencies
 
 Default dependency utilities used within Tanjun and their abstract interfaces.
 
 ::: tanjun.dependencies.async_cache
-    rendering:
+    options:
         show_root_heading: true
 
 ::: tanjun.dependencies.callbacks
-    rendering:
+    options:
         show_root_heading: true
 
 ::: tanjun.dependencies.data
-    rendering:
+    options:
         show_root_heading: true
 
 ::: tanjun.dependencies.limiters
-    rendering:
+    options:
         show_root_heading: true
 
 ::: tanjun.dependencies.locales
-    rendering:
+    options:
         show_root_heading: true
 
 ::: tanjun.dependencies.owners
-    rendering:
+    options:
         show_root_heading: true
 
 ::: tanjun.dependencies.reloaders
-    rendering:
+    options:
         show_root_heading: true
```

### Comparing `hikari-tanjun-2.8.1a1/docs/usage.md` & `hikari-tanjun-2.9.0a1/docs/usage.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,24 @@
 `declare_global_commands=True` instructs the client to declare the bot's slash
 commands and context menus on startup and `mention_prefix=True` allows the
 bot's message commands to be triggered by starting a command call with `@bot`.
 
 ```py
 async def main():
     bot = hikari.impl.RESTBot("TOKEN", hikari.TokenType.BOT)
-    client = tanjun.Client.from_rest_bot(bot, declare_global_commands=True)
-
-    await bot.start()
-    async with client:
-        await bot.join()
+    tanjun.Client.from_rest_bot(bot, bot_managed=True, declare_global_commands=True)
+    bot.run()
 ```
 
 And here a Tanjun client is linked to a REST server bot instance to enable
 application command execution.
 
-Since Hikari's RESTBot doesn't have lifetime events, we have to startup and
-close Tanjun's client around the REST bot ourselves. The bot should always be
-started before Tanjun.
+Unlike when linked to a Gateway bot, `bot_managed=True` must be explicitly
+passed to [Client.from_rest_bot][tanjun.clients.Client.from_rest_bot] to
+have the client automatically start when the Rest bot starts.
 
 ### Client lifetime management
 
 While Hikari's bots provide systems for stating and stopping sub-components,
 these aren't cross-compatible nor Tanjun friendly and Tanjun's client callbacks
 provide a cross-compatible alternative for these (which also supports dependency
 injection).
@@ -352,15 +349,15 @@
 [tanjun.with_annotated_args][tanjun.annotations.with_annotated_args] provides
 a simple way to declare the arguments for both message and slash commands.
 While this feature is cross-compatible, there is one key difference: a
 description must be included for options when annotating for a slash command,
 which is done by passing a string value to [typing.Annotated][] (as shown
 above).
 
-The special generic types offered in [tanjun.annotations] (e.g
+The special generic types offered in [tanjun.annotations][] (e.g
 [Ranged][tanjun.annotations.Ranged] and [Converted][tanjun.annotations.Converted])
 return a [typing.Annotated][] instance from their generic calls and can also be
 passed as arguments to Annotated like `Annotated[Int, Ranged(13, 130)]`, and
 `Annotated[Str, Converted(get_video)]`.
 
 This example doesn't demonstrate every feature of this, and More information on
 how arguments are configured through annotations can be found in
@@ -430,15 +427,15 @@
 @tanjun.as_user_menu("name", "description")
 async def command_2(ctx: tanjun.abc.MenuContext, user: hikari.User) -> None:
     await ctx.create_initial_response("Starting the thing", ephemeral=True)  # private response
     await ctx.respond("meow")  # public response
     await ctx.create_followup("finished the thing", ephemeral=True)  # private response
 ```
 
-Ephemeral responses are a slash command and context menus exclusive feature which
+Ephemeral responses are a slash command and context menu exclusive feature which
 marks a response as private (so that only the command author can see it) and
 temporary. A response can be marked as ephemeral by either passing `ephemeral=True`
 to [AppCommandContext.create_initial_response][tanjun.abc.AppCommandContext.create_initial_response]
 (when initially responding to the slash command) or
 [AppCommandContext.create_followup][tanjun.abc.AppCommandContext.create_followup]
 (for followup responses).
 Alternatively, an ephemeral default can either be set on a client level
@@ -542,15 +539,15 @@
 And here we declare a command callback as taking the client set values for
 `Foo` and `Bar` as keyword arguments using two different approaches.
 Since both arguments don't provide a default, these commands will fail if no
 value for `Foo` or `Bar` has been set using
 [Client.set_type_dependency][tanjun.abc.Client.set_type_dependency].
 
 A more detailed guide on how this works and the full feature set (e.g. optional
-dependencies) can be found [https://alluka.cursed.solutions/usage/](here).
+dependencies) can be found [here](https://alluka.cursed.solutions/usage/).
 [alluka.abc.Client][] is exposed at [Client.injector][tanjun.abc.Client.injector].
 
 ### Standard and special cased injected types.
 
 The following types are registered globally as type dependencies:
 
 * [tanjun.abc.Client][]
@@ -711,15 +708,15 @@
 The return value of an error hook is used with other error hook return values
 to workout whether the error should be re-raised: [True][] acts as a vote
 towards suppressing the error, [False][] acts as a vote towards re-raising the
 error and [None][] acts as no vote. In the case of a tie the error will be
 re-raised.
 
 ```py
-@hooks.add_on_parser_error  # hooks.add_on_parser_error
+@hooks.with_on_parser_error  # hooks.add_on_parser_error
 async def parser_error_hook(ctx: tanjun.abc.Context, error: tanjun.ParserError) -> None:
     ...
 ```
 
 Parser error hooks are called when the argument parsing of a message command
 failed. Parser errors are never re-raised.
```

### Comparing `hikari-tanjun-2.8.1a1/examples/LICENSE` & `hikari-tanjun-2.9.0a1/examples/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/examples/__init__.py` & `hikari-tanjun-2.9.0a1/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/examples/checks.py` & `hikari-tanjun-2.9.0a1/examples/checks.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/examples/config.py` & `hikari-tanjun-2.9.0a1/examples/config.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/examples/error_handling.py` & `hikari-tanjun-2.9.0a1/examples/error_handling.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/examples/impls.py` & `hikari-tanjun-2.9.0a1/examples/impls.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/examples/injection.py` & `hikari-tanjun-2.9.0a1/examples/injection.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/examples/message_commands.py` & `hikari-tanjun-2.9.0a1/examples/message_commands.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/examples/protos.py` & `hikari-tanjun-2.9.0a1/examples/protos.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/examples/run_gateway.py` & `hikari-tanjun-2.9.0a1/examples/run_gateway.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/examples/run_rest.py` & `hikari-tanjun-2.9.0a1/examples/run_rest.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,41 +22,33 @@
 
 async def run() -> None:
     loaded_config = config.ExampleConfig.load()
     # While a BOT token is assumed in this example, a client credentials OAuth2
     # token can also be used with Tanjun but this may limit functionality.
     bot = hikari.RESTBot(loaded_config.bot_token, hikari.TokenType.BOT)
     database = impls.DatabaseImpl()
-    client = (
+    (
         # Passing True for declare_global_commands here instructs the client to
         # declare the slash commands within it which are marked as "global" during
         # the first startup.
         # A guild ID may also be passed here to instruct it to just declare the
         # global commands for that guild, this can be helpful for debug purposes.
-        tanjun.Client.from_rest_bot(bot, declare_global_commands=True)
+        #
+        # `bot_managed=True` must be passed here to indicate that the client should
+        # be automatically started when the REST bot starts.
+        tanjun.Client.from_rest_bot(bot, declare_global_commands=True, bot_managed=True)
         # Unlike a gateway bot bound client, only slash commands will be automatically
         # executed by a client that's bound to a rest bot.
         .load_modules("examples.slash_component")
         .set_type_dependency(config.ExampleConfig, loaded_config)
         .set_type_dependency(protos.DatabaseProto, database)
         # Here we use client callbacks to manage the database, STOPPING can also be used to stop it.
         .add_client_callback(tanjun.ClientCallbackNames.STARTING, database.connect)
     )
-    # Unlike with a gateway bot, for RESTBots hikari has no lifetime event
-    # dispatch which can be used to implicitly startup and close the Tanjun
-    # client. Instead, we must directly startup and close Tanjun.
-    await bot.start()
-
-    # Note that starting a Tanjun client before the relevant bot may lead
-    # to erroneous behaviour as it won't be able to make any requests.
-
-    # While this example uses the client as a context manager to implicitly start
-    # and close it, the `open` and `close` methods can alternatively be used to the same effect.
-    async with client:
-        await bot.join()  # This waits until the bot is closed before closing Tanjun by exiting the context manager.
+    bot.run()
 
 
 def main():
     asyncio.run(run())
 
 
 if __name__ == "__main__":
```

### Comparing `hikari-tanjun-2.8.1a1/examples/slash_commands.py` & `hikari-tanjun-2.9.0a1/examples/slash_commands.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/mkdocs.yml` & `hikari-tanjun-2.9.0a1/mkdocs.yml`

 * *Files 21% similar despite different names*

```diff
@@ -41,27 +41,26 @@
 plugins:
   - autorefs
   - search
   - mkdocstrings:
       default_handler: python
       handlers:
         python:
-          selection:
+          import:
+            - https://docs.python.org/3.9/objects.inv
+            - https://hikari-py.github.io/hikari/objects.inv
+            - https://alluka.cursed.solutions/objects.inv
+            - https://sake.cursed.solutions/objects.inv
+          options:
+            docstring_section_style: spacy
             docstring_style: numpy
             inherited_members: true
-          rendering:
-            docstring_section_style: spacy
             merge_init_into_class: false
+            separate_signature: true
             show_signature_annotations: false
             show_source: false
             show_submodules: false
-            separate_signature: true
-          import:
-            - https://docs.python.org/3.9/objects.inv
-            - https://hikari-py.github.io/hikari/objects.inv
-            - https://alluka.cursed.solutions/objects.inv
-            - https://sake.cursed.solutions/objects.inv
 
 watch:
   - CHANGELOG.md
   - README.md
   - tanjun
```

### Comparing `hikari-tanjun-2.8.1a1/noxfile.py` & `hikari-tanjun-2.9.0a1/noxfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 from __future__ import annotations
 
 import itertools
 import pathlib
 import re
 import shutil
-import tempfile
 from collections import abc as collections
 
 import nox
 
 nox.options.sessions = ["reformat", "flake8", "spell-check", "slot-check", "type-check", "test", "verify-types"]  # type: ignore
 GENERAL_TARGETS = ["./noxfile.py", "./tests"]
 _BLACKLISTED_TARGETS = re.compile("^_internal/vendor/.*\\.py")
@@ -143,15 +142,15 @@
         shutil.copy(path, pathlib.Path(output_directory) / path)
 
 
 @nox.session(reuse_venv=True)
 def flake8(session: nox.Session) -> None:
     """Run this project's modules against the pre-defined flake8 linters."""
     install_requirements(session, *_dev_dep("flake8"))
-    session.run("flake8", *GENERAL_TARGETS)
+    session.run("pflake8", *GENERAL_TARGETS)
 
 
 @nox.session(reuse_venv=True, name="slot-check")
 def slot_check(session: nox.Session) -> None:
     """Check this project's slotted classes for common mistakes."""
     install_requirements(session, ".", *_dev_dep("lint"))
     session.run("slotscheck", "-m", "tanjun")
@@ -185,44 +184,25 @@
     """Build this project using flit."""
     install_requirements(session, *_dev_dep("publish"))
     session.log("Starting build")
     session.run("flit", "build")
 
 
 @nox.session(reuse_venv=True)
-def publish(session: nox.Session, test: bool = False) -> None:
+def publish(session: nox.Session, env: dict[str, str] | None = None) -> None:
     """Publish this project to pypi."""
     install_requirements(session, *_dev_dep("publish"))
     install_requirements(session, ".", first_call=False)
-
-    env: dict[str, str] = {}
-
-    if username := _try_find_option(session, "-u", "--username"):
-        env["FLIT_USERNAME"] = username
-
-    if password := _try_find_option(session, "-p", "--password"):
-        env["FLIT_PASSWORD"] = password
-
-    if index_url := _try_find_option(session, "-i", "--index-url"):
-        env["FLIT_INDEX_URL"] = index_url
-
-    elif test:
-        env["FLIT_INDEX_URL"] = "https://test.pypi.org/legacy/"
-
-    else:
-        env["FLIT_INDEX_URL"] = "https://upload.pypi.org/legacy/"
-
-    session.log("Initiating TestPYPI upload" if test else "Initiating PYPI upload")
     session.run("flit", "publish", env=env)
 
 
 @nox.session(name="test-publish", reuse_venv=True)
 def test_publish(session: nox.Session) -> None:
     """Publish this project to test pypi."""
-    publish(session, test=True)
+    publish(session, env={"FLIT_INDEX_URL": "https://test.pypi.org/legacy/"})
 
 
 @nox.session(reuse_venv=True)
 def reformat(session: nox.Session) -> None:
     """Reformat this project's modules to fit the standard style."""
     install_requirements(session, *_dev_dep("reformat"))  # include_standard_requirements=False
     session.run("black", *GENERAL_TARGETS, "--extend-exclude", "^/tanjun/_internal/vendor/.*$")
@@ -271,39 +251,7 @@
 
 
 @nox.session(name="verify-types", reuse_venv=True)
 def verify_types(session: nox.Session) -> None:
     """Verify the "type completeness" of types exported by the library using Pyright."""
     install_requirements(session, ".", *_dev_dep("type-checking"))
     _run_pyright(session, "--verifytypes", "tanjun", "--ignoreexternal")
-
-
-@nox.session(name="check-dependencies")
-def check_dependencies(session: nox.Session) -> None:
-    """Verify that all the dependencies declared in pyproject.toml are up to date."""
-    import httpx
-
-    # Note: this can be linked to a specific hash by adding it between raw and {file.name} as another route segment.
-    with httpx.Client() as client:
-        requirements = client.get(
-            "https://gist.githubusercontent.com/FasterSpeeding/13e3d871f872fa09cf7bdc4144d62b2b/raw/requirements.json"
-        ).json()
-
-        # Note: this can be linked to a specific hash by adding it between raw and {file.name} as another route segment.
-        code = client.get(
-            "https://gist.githubusercontent.com/FasterSpeeding/13e3d871f872fa09cf7bdc4144d62b2b/raw/check_dependency.py"
-        ).read()
-
-    install_requirements(session, *requirements)
-    # This is saved to a temporary file to avoid the source showing up in any of the output.
-
-    # A try, finally is used to delete the file rather than relying on delete=True behaviour
-    # as on Windows the file cannot be accessed by other processes if delete is True.
-    file = tempfile.NamedTemporaryFile(delete=False)
-    try:
-        with file:
-            file.write(code)
-
-        session.run("python", file.name)
-
-    finally:
-        pathlib.Path(file.name).unlink(missing_ok=False)
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/__init__.py` & `hikari-tanjun-2.9.0a1/tanjun/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -70,27 +70,25 @@
 
 ```py
 bot = hikari.RESTBot("BOT_TOKEN", "Bot")
 
 # declare_global_commands=True instructs the client to set the global commands
 # for the relevant bot on first startup (this will replace any previously
 # declared commands).
-client = tanjun.Client.from_rest_bot(bot, declare_global_commands=True)
+#
+# `bot_managed=True` has to be explicitly passed here to indicate that the client
+# should automatically start when the linked REST bot starts.
+client = tanjun.Client.from_rest_bot(bot, bot_managed=True, declare_global_commands=True)
 
 # This will load components from modules based on loader functions.
 # For more information on this see [tanjun.as_loader][].
 client.load_modules("module.paths")
 
-# Note, unlike a gateway bound bot, the rest bot will not automatically start
-# itself due to the lack of Hikari lifetime events in this environment and
-# will have to be started after the Hikari client.
-async def main() -> None:
-    await bot.start()
-    async with client:
-        await bot.join()
+# Thanks to `bot_managed=True`, this will also start the client.
+bot.run()
 ```
 
 For more extensive examples see the
 [repository's examples](https://github.com/FasterSpeeding/Tanjun/tree/master/examples).
 
 There are also
 [written tutorials](https://patchwork.systems/programming/hikari-discord-bot/index.html)
@@ -130,24 +128,14 @@
     "ParserError",
     "ShlexParser",
     "SlashCommand",
     "SlashCommandGroup",
     "SlashHooks",
     "TanjunError",
     "TooManyArgumentsError",
-    "__author__",
-    "__ci__",
-    "__copyright__",
-    "__coverage__",
-    "__docs__",
-    "__email__",
-    "__issue_tracker__",
-    "__license__",
-    "__url__",
-    "__version__",
     "abc",
     "annotations",
     "as_interval",
     "as_loader",
     "as_message_command",
     "as_message_command_group",
     "as_message_menu",
@@ -217,16 +205,14 @@
     "with_parser",
     "with_role_slash_option",
     "with_sfw_check",
     "with_str_slash_option",
     "with_user_slash_option",
 ]
 
-import typing
-
 from alluka import inject
 from alluka import inject as injected
 
 from . import abc
 from . import annotations
 from . import context
 from . import permissions
@@ -319,18 +305,7 @@
 from .parsing import with_greedy_argument
 from .parsing import with_multi_argument
 from .parsing import with_multi_option
 from .parsing import with_option
 from .parsing import with_parser
 from .schedules import as_interval
 from .schedules import as_time_schedule
-
-__author__: typing.Final[str] = "Faster Speeding"
-__ci__: typing.Final[str] = "https://github.com/FasterSpeeding/Tanjun/actions"
-__copyright__: typing.Final[str] = "© 2020-2022 Faster Speeding"
-__coverage__: typing.Final[str] = "https://codeclimate.com/github/FasterSpeeding/Tanjun"
-__docs__: typing.Final[str] = "https://tanjun.cursed.solutions/"
-__email__: typing.Final[str] = "lucina@lmbyrne.dev"
-__issue_tracker__: typing.Final[str] = "https://github.com/FasterSpeeding/Tanjun/issues"
-__license__: typing.Final[str] = "BSD"
-__url__: typing.Final[str] = "https://github.com/FasterSpeeding/Tanjun"
-__version__: typing.Final[str] = "2.8.1a1"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/_internal/__init__.py` & `hikari-tanjun-2.9.0a1/tanjun/_internal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 import types
 import typing
 from collections import abc as collections
 
 import hikari
 
 from .. import errors
-from .._internal.vendor import inspect
+from .vendor import inspect
 
 if typing.TYPE_CHECKING:
     import typing_extensions
 
     from .. import abc as tanjun
 
     _P = typing_extensions.ParamSpec("_P")
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/_internal/localisation.py` & `hikari-tanjun-2.9.0a1/tanjun/_internal/localisation.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/_internal/vendor/inspect.py` & `hikari-tanjun-2.9.0a1/tanjun/_internal/vendor/inspect.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/_internal/vendor/inspect.py.LICENSE` & `hikari-tanjun-2.9.0a1/tanjun/_internal/vendor/inspect.py.LICENSE`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/_internal/vendor/inspect.pyi` & `hikari-tanjun-2.9.0a1/tanjun/_internal/vendor/inspect.pyi`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/_internal/vendor/inspect.pyi.LICENSE` & `hikari-tanjun-2.9.0a1/tanjun/_internal/vendor/inspect.pyi.LICENSE`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/abc.py` & `hikari-tanjun-2.9.0a1/tanjun/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,21 +439,20 @@
 
     @abc.abstractmethod
     async def edit_initial_response(
         self,
         content: hikari.UndefinedOr[typing.Any] = hikari.UNDEFINED,
         *,
         delete_after: typing.Union[datetime.timedelta, float, int, None] = None,
-        attachment: hikari.UndefinedOr[hikari.Resourceish] = hikari.UNDEFINED,
-        attachments: hikari.UndefinedOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
+        attachment: hikari.UndefinedNoneOr[hikari.Resourceish] = hikari.UNDEFINED,
+        attachments: hikari.UndefinedNoneOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
         component: hikari.UndefinedNoneOr[hikari.api.ComponentBuilder] = hikari.UNDEFINED,
         components: hikari.UndefinedNoneOr[collections.Sequence[hikari.api.ComponentBuilder]] = hikari.UNDEFINED,
         embed: hikari.UndefinedNoneOr[hikari.Embed] = hikari.UNDEFINED,
         embeds: hikari.UndefinedNoneOr[collections.Sequence[hikari.Embed]] = hikari.UNDEFINED,
-        replace_attachments: bool = False,
         mentions_everyone: hikari.UndefinedOr[bool] = hikari.UNDEFINED,
         user_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialUser], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
         role_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialRole], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
@@ -495,16 +494,14 @@
             this message. These components will replace any previously set
             components and passing [None][] or an empty sequence will
             remove all components.
         embed
             An embed to replace the initial response with.
         embeds
             A sequence of embeds to replace the initial response with.
-        replace_attachments
-            Whether to replace the attachments of the response or not.
         mentions_everyone
             If provided, whether the message should parse @everyone/@here
             mentions.
         user_mentions
             If provided, and [True][], all mentions will be parsed.
             If provided, and [False][], no mentions will be parsed.
             Alternatively this may be a collection of
@@ -563,21 +560,20 @@
 
     @abc.abstractmethod
     async def edit_last_response(
         self,
         content: hikari.UndefinedOr[typing.Any] = hikari.UNDEFINED,
         *,
         delete_after: typing.Union[datetime.timedelta, float, int, None] = None,
-        attachment: hikari.UndefinedOr[hikari.Resourceish] = hikari.UNDEFINED,
-        attachments: hikari.UndefinedOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
+        attachment: hikari.UndefinedNoneOr[hikari.Resourceish] = hikari.UNDEFINED,
+        attachments: hikari.UndefinedNoneOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
         component: hikari.UndefinedNoneOr[hikari.api.ComponentBuilder] = hikari.UNDEFINED,
         components: hikari.UndefinedNoneOr[collections.Sequence[hikari.api.ComponentBuilder]] = hikari.UNDEFINED,
         embed: hikari.UndefinedNoneOr[hikari.Embed] = hikari.UNDEFINED,
         embeds: hikari.UndefinedNoneOr[collections.Sequence[hikari.Embed]] = hikari.UNDEFINED,
-        replace_attachments: bool = False,
         mentions_everyone: hikari.UndefinedOr[bool] = hikari.UNDEFINED,
         user_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialUser], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
         role_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialRole], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
@@ -619,16 +615,14 @@
             this message. These components will replace any previously set
             components and passing [None][] or an empty sequence will
             remove all components.
         embed
             An embed to replace the last response with.
         embeds
             A sequence of embeds to replace the last response with.
-        replace_attachments
-            Whether to replace the attachments of the response or not.
         mentions_everyone
             If provided, whether the message should parse @everyone/@here
             mentions.
         user_mentions
             If provided, and [True][], all mentions will be parsed.
             If provided, and [False][], no mentions will be parsed.
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/annotations.py` & `hikari-tanjun-2.9.0a1/tanjun/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,23 +332,23 @@
     Examples
     --------
     ```py
     @with_annotated_args
     @tanjun.as_slash_command("name", "description")
     async def command(
         ctx: tanjun.abc.Context,
-        argument: Annotated[Str, Default(""), "description],
+        argument: Annotated[Str, Default(""), "description"],
         other_argument: Annotated[Default[Str, ""], "description"],
     ) -> None:
         ...
     ```
 
     ```py
     @with_annotated_args
-    @tanjun.as_slash_command("name", "description)
+    @tanjun.as_slash_command("name", "description")
     async def command(
         ctx: tanjun.abc.Context,
         required_argument: Annotated[Default[Str], "description"] = "yeet",
         other_required: Annotated[Int, Default(), "description"] = 123,
     ) -> None:
         ...
     ```
@@ -587,15 +587,15 @@
     ) -> None:
         raise NotImplementedError
     ```
 
     Alternatively, the slice syntax and `range` may be used to set the length
     restraints for a string argument (where the start is inclusive and stop is
     exclusive). These default to a min_length of `0` if the start isn't
-    specified and ignore any specified step.
+    specified and ignores any specified step.
     """
 
     __slots__ = ("_min_length", "_max_length")
 
     @typing.overload
     def __init__(self, max_length: int, /) -> None:
         ...
@@ -849,15 +849,15 @@
     ) -> None:
         raise NotImplementedError
     ```
 
     Alternatively, the slice syntax and `range` may be used to set the range
     for a float or integer argument (where the start is inclusive and stop is
     exclusive). These default to a min_value of `0` if the start isn't
-    specified and ignore any specified step.
+    specified and ignores any specified step.
     """
 
     __slots__ = ("_max_value", "_min_value")
 
     def __init__(self, min_value: typing.Union[int, float], max_value: typing.Union[int, Float], /) -> None:
         """Create an argument range limit.
 
@@ -923,19 +923,19 @@
 class SnowflakeOr(_ConfigIdentifier, metaclass=_SnowflakeOrMeta):
     """Mark an argument as taking an object or its ID.
 
     This allows for the argument to be declared as taking the object for slash
     commands without requiring that the message command equivalent fetch the
     object each time for the following types:
 
-    * [hikari.users.User][]
-    * [hikari.guilds.Role][]
-    * [hikari.guilds.Member][]
-    * [hikari.channels.PartialChannel][]
-    * `hikari.User | hikari.Role`
+    * [User][tanjun.annotations.User]
+    * [Role][tanjun.annotations.Role]
+    * [Member][tanjun.annotations.Member]
+    * [Channel][tanjun.annotations.Channel]
+    * [Mentionable][tanjun.annotations.Mentionable]
 
     Examples
     --------
     ```py
     @with_annotated_args(follow_wrapped=True)
     @tanjun.as_slash_command("meow", "nyaa")
     @tanjun.as_message_command("meow")
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/checks.py` & `hikari-tanjun-2.9.0a1/tanjun/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 import hikari
 
 from . import _internal
 from . import abc as tanjun
 from . import dependencies
 from . import errors
 from . import permissions
+from ._internal import cache
 from ._internal import localisation
 
 if typing.TYPE_CHECKING:
 
     class _AnyCallback(typing.Protocol):
         async def __call__(
             self,
@@ -185,44 +186,19 @@
         ctx: tanjun.Context,
         dependency: alluka.Injected[dependencies.AbstractOwners],
         localiser: alluka.Injected[typing.Optional[dependencies.AbstractLocaliser]] = None,
     ) -> bool:
         return self._handle_result(ctx, await dependency.check_ownership(ctx.client, ctx.author), localiser)
 
 
-_GuildChannelCacheT = typing.Optional[dependencies.SfCache[hikari.GuildChannel]]
-
-
-async def _get_is_nsfw(
-    ctx: tanjun.Context,
-    /,
-    *,
-    dm_default: bool,
-    channel_cache: _GuildChannelCacheT,
-) -> bool:
+async def _get_is_nsfw(ctx: tanjun.Context, /, *, dm_default: bool) -> bool:
     if ctx.guild_id is None:
         return dm_default
 
-    channel: typing.Optional[hikari.PartialChannel] = None
-    if ctx.cache and (channel := ctx.cache.get_guild_channel(ctx.channel_id)):
-        return channel.is_nsfw or False
-
-    if channel_cache:
-        try:
-            return (await channel_cache.get(ctx.channel_id)).is_nsfw or False
-
-        except dependencies.EntryNotFound:
-            raise
-
-        except dependencies.CacheMissError:
-            pass
-
-    channel = await ctx.rest.fetch_channel(ctx.channel_id)
-    assert isinstance(channel, hikari.GuildChannel)
-    return channel.is_nsfw or False
+    return (await cache.get_perm_channel(ctx.client, ctx.channel_id)).is_nsfw or False
 
 
 class NsfwCheck(_Check):
     """Standard NSFW check callback registered by [tanjun.with_nsfw_check][].
 
     This check will only pass if the current channel is NSFW.
     """
@@ -263,20 +239,17 @@
         super().__init__(error, error_message, halt_execution)
 
     async def __call__(
         self,
         ctx: tanjun.Context,
         /,
         *,
-        channel_cache: alluka.Injected[_GuildChannelCacheT] = None,
         localiser: alluka.Injected[typing.Optional[dependencies.AbstractLocaliser]] = None,
     ) -> bool:
-        return self._handle_result(
-            ctx, await _get_is_nsfw(ctx, dm_default=True, channel_cache=channel_cache), localiser
-        )
+        return self._handle_result(ctx, await _get_is_nsfw(ctx, dm_default=True), localiser)
 
 
 class SfwCheck(_Check):
     """Standard SFW check callback registered by [tanjun.with_sfw_check][].
 
     This check will only pass if the current channel is SFW.
     """
@@ -317,20 +290,17 @@
         super().__init__(error, error_message, halt_execution)
 
     async def __call__(
         self,
         ctx: tanjun.Context,
         /,
         *,
-        channel_cache: alluka.Injected[_GuildChannelCacheT] = None,
         localiser: alluka.Injected[typing.Optional[dependencies.AbstractLocaliser]] = None,
     ) -> bool:
-        return self._handle_result(
-            ctx, not await _get_is_nsfw(ctx, dm_default=False, channel_cache=channel_cache), localiser
-        )
+        return self._handle_result(ctx, not await _get_is_nsfw(ctx, dm_default=False), localiser)
 
 
 class DmCheck(_Check):
     """Standard DM check callback registered by [tanjun.with_dm_check][].
 
     This check will only pass if the current channel is a DM channel.
     """
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/clients.py` & `hikari-tanjun-2.9.0a1/tanjun/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,14 +522,17 @@
 class Client(tanjun.Client):
     """Tanjun's standard [tanjun.abc.Client][] implementation.
 
     This implementation supports dependency injection for checks, command
     callbacks, prefix getters and event listeners. For more information on how
     this works see [alluka][].
 
+    When manually managing the lifetime of the client the linked rest app or
+    bot must always be started before the Tanjun client.
+
     !!! note
         By default this client includes a parser error handling hook which will
         by overwritten if you call [tanjun.Client.set_hooks][].
     """
 
     __slots__ = (
         "_auto_defer_after",
@@ -747,16 +750,16 @@
         self._tasks: list[asyncio.Task[typing.Any]] = []
         self._voice = voice
 
         if event_managed:
             if not events:
                 raise ValueError("Client cannot be event managed without an event manager")
 
-            events.subscribe(hikari.StartingEvent, self._on_starting_event)
-            events.subscribe(hikari.StoppingEvent, self._on_stopping_event)
+            events.subscribe(hikari.StartingEvent, self._on_starting)
+            events.subscribe(hikari.StoppingEvent, self._on_stopping)
 
         (
             self.set_type_dependency(tanjun.Client, self)
             .set_type_dependency(Client, self)
             .set_type_dependency(type(self), self)
             .set_type_dependency(hikari.api.RESTClient, rest)
             .set_type_dependency(type(rest), rest)
@@ -955,14 +958,15 @@
 
     @classmethod
     def from_rest_bot(
         cls,
         bot: hikari.RESTBotAware,
         /,
         *,
+        bot_managed: bool = False,
         declare_global_commands: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialGuild], hikari.SnowflakeishOr[hikari.PartialGuild], bool
         ] = False,
         injector: typing.Optional[alluka.abc.Client] = None,
         set_global_commands: typing.Union[hikari.SnowflakeishOr[hikari.PartialGuild], bool] = False,
         command_ids: typing.Optional[collections.Mapping[str, hikari.SnowflakeishOr[hikari.PartialCommand]]] = None,
         message_ids: typing.Optional[collections.Mapping[str, hikari.SnowflakeishOr[hikari.PartialCommand]]] = None,
@@ -985,14 +989,19 @@
             If one or more guild objects/IDs are passed here then the registered
             global commands will be set on the specified guild(s) at startup rather
             than globally.
 
             The endpoint this uses has a strict ratelimit which, as of writing,
             only allows for 2 requests per minute (with that ratelimit either
             being per-guild if targeting a specific guild otherwise globally).
+        bot_managed
+            Whether the client should be managed by the REST bot.
+
+            A REST bot managed client will be automatically started and closed
+            based on the REST bot's startup and shutdown callbacks.
         injector
             The alluka client this should use for dependency injection.
 
             If not provided then the client will initialise its own DI client.
         set_global_commands
             Deprecated as of v2.1.1a1 alias of `declare_global_commands`.
         command_ids
@@ -1013,26 +1022,32 @@
         message_ids
             If provided, a mapping of message context menu command names to the
             IDs of existing commands to update.
         user_ids
             If provided, a mapping of user context menu command names to the IDs
             of existing commands to update.
         """
-        return cls(
+        self = cls(
             rest=bot.rest,
             server=bot.interaction_server,
             declare_global_commands=declare_global_commands,
             injector=injector,
             set_global_commands=set_global_commands,
             command_ids=command_ids,
             message_ids=message_ids,
             user_ids=user_ids,
             _stack_level=1,
         ).set_hikari_trait_injectors(bot)
 
+        if bot_managed:
+            bot.add_startup_callback(self._on_starting)
+            bot.add_shutdown_callback(self._on_stopping)
+
+        return self
+
     async def __aenter__(self) -> Client:
         await self.open()
         return self
 
     async def __aexit__(
         self,
         exc_type: typing.Optional[type[BaseException]],
@@ -1189,18 +1204,18 @@
         return self._shards
 
     @property
     def voice(self) -> typing.Optional[hikari.api.VoiceComponent]:
         # <<inherited docstring from tanjun.abc.Client>>.
         return self._voice
 
-    async def _on_starting_event(self, _: hikari.StartingEvent, /) -> None:
+    async def _on_starting(self, _: typing.Union[hikari.StartingEvent, hikari.RESTBotAware], /) -> None:
         await self.open()
 
-    async def _on_stopping_event(self, _: hikari.StoppingEvent, /) -> None:
+    async def _on_stopping(self, _: typing.Union[hikari.StoppingEvent, hikari.RESTBotAware], /) -> None:
         await self.close()
 
     async def clear_application_commands(
         self,
         *,
         application: typing.Optional[hikari.SnowflakeishOr[hikari.PartialApplication]] = None,
         guild: hikari.UndefinedOr[hikari.SnowflakeishOr[hikari.PartialGuild]] = hikari.UNDEFINED,
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/commands/__init__.py` & `hikari-tanjun-2.9.0a1/tanjun/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/commands/base.py` & `hikari-tanjun-2.9.0a1/tanjun/commands/base.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/commands/menu.py` & `hikari-tanjun-2.9.0a1/tanjun/commands/menu.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/commands/message.py` & `hikari-tanjun-2.9.0a1/tanjun/commands/message.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/commands/slash.py` & `hikari-tanjun-2.9.0a1/tanjun/commands/slash.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/components.py` & `hikari-tanjun-2.9.0a1/tanjun/components.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/context/__init__.py` & `hikari-tanjun-2.9.0a1/tanjun/context/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/context/autocomplete.py` & `hikari-tanjun-2.9.0a1/tanjun/context/autocomplete.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/context/base.py` & `hikari-tanjun-2.9.0a1/tanjun/context/base.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/context/menu.py` & `hikari-tanjun-2.9.0a1/tanjun/context/menu.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/context/message.py` & `hikari-tanjun-2.9.0a1/tanjun/context/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,21 +236,20 @@
         await self._client.rest.delete_message(self._message.channel_id, self._last_response_id)
 
     async def edit_initial_response(
         self,
         content: hikari.UndefinedOr[typing.Any] = hikari.UNDEFINED,
         *,
         delete_after: typing.Union[datetime.timedelta, float, int, None] = None,
-        attachment: hikari.UndefinedOr[hikari.Resourceish] = hikari.UNDEFINED,
-        attachments: hikari.UndefinedOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
+        attachment: hikari.UndefinedNoneOr[hikari.Resourceish] = hikari.UNDEFINED,
+        attachments: hikari.UndefinedNoneOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
         component: hikari.UndefinedNoneOr[hikari.api.ComponentBuilder] = hikari.UNDEFINED,
         components: hikari.UndefinedNoneOr[collections.Sequence[hikari.api.ComponentBuilder]] = hikari.UNDEFINED,
         embed: hikari.UndefinedNoneOr[hikari.Embed] = hikari.UNDEFINED,
         embeds: hikari.UndefinedNoneOr[collections.Sequence[hikari.Embed]] = hikari.UNDEFINED,
-        replace_attachments: bool = False,
         mentions_everyone: hikari.UndefinedOr[bool] = hikari.UNDEFINED,
         user_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialUser], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
         role_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialRole], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
@@ -266,36 +265,34 @@
             content=content,
             attachment=attachment,
             attachments=attachments,
             component=component,
             components=components,
             embed=embed,
             embeds=embeds,
-            replace_attachments=replace_attachments,
             mentions_everyone=mentions_everyone,
             user_mentions=user_mentions,
             role_mentions=role_mentions,
         )
         if delete_after is not None:
             self._register_task(asyncio.create_task(self._delete_after(delete_after, message)))
 
         return message
 
     async def edit_last_response(
         self,
         content: hikari.UndefinedOr[typing.Any] = hikari.UNDEFINED,
         *,
         delete_after: typing.Union[datetime.timedelta, float, int, None] = None,
-        attachment: hikari.UndefinedOr[hikari.Resourceish] = hikari.UNDEFINED,
-        attachments: hikari.UndefinedOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
+        attachment: hikari.UndefinedNoneOr[hikari.Resourceish] = hikari.UNDEFINED,
+        attachments: hikari.UndefinedNoneOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
         component: hikari.UndefinedNoneOr[hikari.api.ComponentBuilder] = hikari.UNDEFINED,
         components: hikari.UndefinedNoneOr[collections.Sequence[hikari.api.ComponentBuilder]] = hikari.UNDEFINED,
         embed: hikari.UndefinedNoneOr[hikari.Embed] = hikari.UNDEFINED,
         embeds: hikari.UndefinedNoneOr[collections.Sequence[hikari.Embed]] = hikari.UNDEFINED,
-        replace_attachments: bool = False,
         mentions_everyone: hikari.UndefinedOr[bool] = hikari.UNDEFINED,
         user_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialUser], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
         role_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialRole], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
@@ -311,15 +308,14 @@
             content=content,
             attachment=attachment,
             attachments=attachments,
             component=component,
             components=components,
             embed=embed,
             embeds=embeds,
-            replace_attachments=replace_attachments,
             mentions_everyone=mentions_everyone,
             user_mentions=user_mentions,
             role_mentions=role_mentions,
         )
 
         if delete_after is not None:
             self._register_task(asyncio.create_task(self._delete_after(delete_after, message)))
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/context/slash.py` & `hikari-tanjun-2.9.0a1/tanjun/context/slash.py`

 * *Files 0% similar despite different names*

```diff
@@ -710,21 +710,20 @@
         await self._interaction.delete_message(self._last_response_id)
 
     async def edit_initial_response(
         self,
         content: hikari.UndefinedOr[typing.Any] = hikari.UNDEFINED,
         *,
         delete_after: typing.Union[datetime.timedelta, float, int, None] = None,
-        attachment: hikari.UndefinedOr[hikari.Resourceish] = hikari.UNDEFINED,
-        attachments: hikari.UndefinedOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
+        attachment: hikari.UndefinedNoneOr[hikari.Resourceish] = hikari.UNDEFINED,
+        attachments: hikari.UndefinedNoneOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
         component: hikari.UndefinedNoneOr[hikari.api.ComponentBuilder] = hikari.UNDEFINED,
         components: hikari.UndefinedNoneOr[collections.Sequence[hikari.api.ComponentBuilder]] = hikari.UNDEFINED,
         embed: hikari.UndefinedNoneOr[hikari.Embed] = hikari.UNDEFINED,
         embeds: hikari.UndefinedNoneOr[collections.Sequence[hikari.Embed]] = hikari.UNDEFINED,
-        replace_attachments: bool = False,
         mentions_everyone: hikari.UndefinedOr[bool] = hikari.UNDEFINED,
         user_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialUser], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
         role_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialRole], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
@@ -735,15 +734,14 @@
             content=content,
             attachment=attachment,
             attachments=attachments,
             component=component,
             components=components,
             embed=embed,
             embeds=embeds,
-            replace_attachments=replace_attachments,
             mentions_everyone=mentions_everyone,
             user_mentions=user_mentions,
             role_mentions=role_mentions,
         )
         # This will be False if the initial response was deferred with this finishing the referral.
         self._has_responded = True
 
@@ -753,21 +751,20 @@
         return message
 
     async def edit_last_response(
         self,
         content: hikari.UndefinedOr[typing.Any] = hikari.UNDEFINED,
         *,
         delete_after: typing.Union[datetime.timedelta, float, int, None] = None,
-        attachment: hikari.UndefinedOr[hikari.Resourceish] = hikari.UNDEFINED,
-        attachments: hikari.UndefinedOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
+        attachment: hikari.UndefinedNoneOr[hikari.Resourceish] = hikari.UNDEFINED,
+        attachments: hikari.UndefinedNoneOr[collections.Sequence[hikari.Resourceish]] = hikari.UNDEFINED,
         component: hikari.UndefinedNoneOr[hikari.api.ComponentBuilder] = hikari.UNDEFINED,
         components: hikari.UndefinedNoneOr[collections.Sequence[hikari.api.ComponentBuilder]] = hikari.UNDEFINED,
         embed: hikari.UndefinedNoneOr[hikari.Embed] = hikari.UNDEFINED,
         embeds: hikari.UndefinedNoneOr[collections.Sequence[hikari.Embed]] = hikari.UNDEFINED,
-        replace_attachments: bool = False,
         mentions_everyone: hikari.UndefinedOr[bool] = hikari.UNDEFINED,
         user_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialUser], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
         role_mentions: typing.Union[
             hikari.SnowflakeishSequence[hikari.PartialRole], bool, hikari.UndefinedType
         ] = hikari.UNDEFINED,
@@ -780,15 +777,14 @@
                 content=content,
                 attachment=attachment,
                 attachments=attachments,
                 component=component,
                 components=components,
                 embed=embed,
                 embeds=embeds,
-                replace_attachments=replace_attachments,
                 mentions_everyone=mentions_everyone,
                 user_mentions=user_mentions,
                 role_mentions=role_mentions,
             )
             if delete_after is not None:
                 self._register_task(asyncio.create_task(self._delete_followup_after(delete_after, message)))
 
@@ -800,15 +796,14 @@
                 content=content,
                 attachment=attachment,
                 attachments=attachments,
                 component=component,
                 components=components,
                 embed=embed,
                 embeds=embeds,
-                replace_attachments=replace_attachments,
                 mentions_everyone=mentions_everyone,
                 user_mentions=user_mentions,
                 role_mentions=role_mentions,
             )
 
         raise LookupError("Context has no previous responses")
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/conversion.py` & `hikari-tanjun-2.9.0a1/tanjun/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,16 @@
             _LOGGER.warning(
                 f"Converter {self!r} registered with {parent_name} may not perform as expected "
                 f"without the following intents: {missing_intents}",
             )
 
 
 _DmCacheT = async_cache.SfCache[hikari.DMChannel]
-_GuildChannelCacheT = async_cache.SfCache[hikari.PartialChannel]
+_GuildChannelCacheT = async_cache.SfCache[hikari.PermissibleGuildChannel]
+_ThreadCacheT = async_cache.SfCache[hikari.GuildThreadChannel]
 
 
 # TODO: GuildChannelConverter
 class ToChannel(BaseConverter):
     """Standard converter for channels mentions/IDs.
 
     For a standard instance of this see [tanjun.conversion.to_channel][].
@@ -226,15 +227,15 @@
             the client doesn't have a registered async cache for DMs.
         """
         self._include_dms = include_dms
 
     @property
     def async_caches(self) -> collections.Sequence[typing.Any]:
         # <<inherited docstring from BaseConverter>>.
-        return (_GuildChannelCacheT, _DmCacheT)
+        return (_GuildChannelCacheT, _DmCacheT, _ThreadCacheT)
 
     @property
     def cache_components(self) -> hikari.api.CacheComponents:
         # <<inherited docstring from BaseConverter>>.
         return hikari.api.CacheComponents.GUILD_CHANNELS
 
     @property
@@ -251,51 +252,59 @@
         self,
         argument: _ArgumentT,
         /,
         ctx: alluka.Injected[tanjun.Context],
         *,
         cache: alluka.Injected[typing.Optional[_GuildChannelCacheT]] = None,
         dm_cache: alluka.Injected[typing.Optional[_DmCacheT]] = None,
+        thread_cache: alluka.Injected[typing.Optional[_ThreadCacheT]] = None,
     ) -> hikari.PartialChannel:
         channel_id = parse_channel_id(argument, message="No valid channel mention or ID found")
         if ctx.cache and (channel_ := ctx.cache.get_guild_channel(channel_id)):
             return channel_
 
-        no_guild_channel = False
+        no_guild_channel = cache and thread_cache and dm_cache
         if cache:
             try:
                 return await cache.get(channel_id)
 
             except async_cache.EntryNotFound:
-                if not self._include_dms:
-                    raise ValueError("Couldn't find channel") from None
-
-                no_guild_channel = True
+                pass
 
             except async_cache.CacheMissError:
+                no_guild_channel = False
+
+        if thread_cache:
+            try:
+                return await thread_cache.get(channel_id)
+
+            except async_cache.EntryNotFound:
                 pass
 
+            except async_cache.CacheMissError:
+                no_guild_channel = False
+
         if dm_cache and self._include_dms:
             try:
                 return await dm_cache.get(channel_id)
 
             except async_cache.EntryNotFound:
-                if no_guild_channel:
-                    raise ValueError("Couldn't find channel") from None
+                pass
 
             except async_cache.CacheMissError:
-                pass
+                no_guild_channel = False
 
-        try:
-            channel = await ctx.rest.fetch_channel(channel_id)
-            if self._include_dms or isinstance(channel, hikari.GuildChannel):
-                return channel
+        if not no_guild_channel:
+            try:
+                channel = await ctx.rest.fetch_channel(channel_id)
+                if self._include_dms or isinstance(channel, hikari.GuildChannel):
+                    return channel
 
-        except hikari.NotFoundError:
-            pass
+            except hikari.NotFoundError:
+                pass
 
         raise ValueError("Couldn't find channel")
 
 
 ChannelConverter = ToChannel
 """Deprecated alias of [tanjun.conversion.ToChannel][]."""
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/dependencies/__init__.py` & `hikari-tanjun-2.9.0a1/tanjun/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/dependencies/async_cache.py` & `hikari-tanjun-2.9.0a1/tanjun/dependencies/async_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
     can be found in [hikari-sake](https://github.com/FasterSpeeding/Sake)
     \>=v1.0.1a1 (exposed by [sake.redis.ResourceClient.add_to_tanjun][]).
 
 Tanjun will use the following type dependencies for these interfaces if they are
 registered with the client:
 
 * `AsyncCache[str, hikari.InviteWithMetadata]`
-* `SfCache[hikari.GuildChannel]`
+* `SfCache[hikari.PermissibleGuildChannel]`
+* `SfCache[hikari.GuildThreadChannel]`
 * `SfCache[hikari.KnownCustomEmoji]`
 * `SfCache[hikari.Guild]`
 * `SfCache[hikari.Role]`
 * `SfCache[hikari.User]`
 * `SfGuildBound[hikari.Member]`
 * `SfGuildBound[hikari.MemberPresence]`
 * `SfGuildBound[hikari.VoiceState]`
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/dependencies/callbacks.py` & `hikari-tanjun-2.9.0a1/tanjun/dependencies/callbacks.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/dependencies/data.py` & `hikari-tanjun-2.9.0a1/tanjun/dependencies/data.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/dependencies/limiters.py` & `hikari-tanjun-2.9.0a1/tanjun/dependencies/limiters.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,20 +208,24 @@
     if type_ is BucketResource.PARENT_CHANNEL:
         if ctx.guild_id is None:
             return ctx.channel_id
 
         if cached_channel := ctx.get_channel():
             return cached_channel.parent_id or ctx.guild_id
 
-        channel_cache = ctx.get_type_dependency(async_cache.SfCache[hikari.GuildChannel])
+        channel_cache = ctx.get_type_dependency(async_cache.SfCache[hikari.PermissibleGuildChannel])
         if channel_cache and (channel_ := await channel_cache.get(ctx.channel_id, default=None)):
             return channel_.parent_id or ctx.guild_id
 
+        thread_cache = ctx.get_type_dependency(async_cache.SfCache[hikari.GuildThreadChannel])
+        if thread_cache and (channel_ := await thread_cache.get(ctx.channel_id, default=None)):
+            return channel_.parent_id
+
         channel = await ctx.fetch_channel()
-        assert isinstance(channel, hikari.TextableGuildChannel)
+        assert isinstance(channel, hikari.GuildChannel)
         return channel.parent_id or ctx.guild_id
 
     # if type_ is BucketResource.CATEGORY:
     #     if ctx.guild_id is None:
     #         return ctx.channel_id
 
     #     # This resource doesn't include threads so we can safely assume that the parent is a category
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/dependencies/locales.py` & `hikari-tanjun-2.9.0a1/tanjun/dependencies/locales.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/dependencies/owners.py` & `hikari-tanjun-2.9.0a1/tanjun/dependencies/owners.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/dependencies/reloaders.py` & `hikari-tanjun-2.9.0a1/tanjun/dependencies/reloaders.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/errors.py` & `hikari-tanjun-2.9.0a1/tanjun/errors.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/hooks.py` & `hikari-tanjun-2.9.0a1/tanjun/hooks.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/injecting.py` & `hikari-tanjun-2.9.0a1/tanjun/injecting.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/parsing.py` & `hikari-tanjun-2.9.0a1/tanjun/parsing.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/permissions.py` & `hikari-tanjun-2.9.0a1/tanjun/permissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Functions used to calculate permissions in Tanjun."""
-
 from __future__ import annotations
 
 __all__: list[str] = [
     "ALL_PERMISSIONS",
     "DM_PERMISSIONS",
     "calculate_everyone_permissions",
     "calculate_permissions",
@@ -43,14 +42,15 @@
 ]
 
 import typing
 from collections import abc as collections
 
 import hikari
 
+from ._internal import cache
 from .dependencies import async_cache
 
 if typing.TYPE_CHECKING:
     from . import abc as tanjun
 
 
 ALL_PERMISSIONS: typing.Final[hikari.Permissions] = hikari.Permissions.all_permissions()
@@ -67,15 +67,15 @@
     | hikari.Permissions.USE_EXTERNAL_STICKERS
     | hikari.Permissions.USE_APPLICATION_COMMANDS
 )
 """Bitfield of the permissions which are accessibly within DM channels."""
 
 
 def _calculate_channel_overwrites(
-    channel: hikari.GuildChannel, member: hikari.Member, permissions: hikari.Permissions
+    channel: hikari.PermissibleGuildChannel, member: hikari.Member, permissions: hikari.Permissions
 ) -> hikari.Permissions:
     if everyone_overwrite := channel.permission_overwrites.get(member.guild_id):
         permissions &= ~everyone_overwrite.deny
         permissions |= everyone_overwrite.allow
 
     deny = hikari.Permissions.NONE
     allow = hikari.Permissions.NONE
@@ -108,15 +108,15 @@
 
 # TODO: implicitly handle more special cases?
 def calculate_permissions(
     member: hikari.Member,
     guild: hikari.Guild,
     roles: collections.Mapping[hikari.Snowflake, hikari.Role],
     *,
-    channel: typing.Optional[hikari.GuildChannel] = None,
+    channel: typing.Optional[hikari.PermissibleGuildChannel] = None,
 ) -> hikari.Permissions:
     """Calculate the permissions a member has within a guild.
 
     Parameters
     ----------
     member
         Object of the member to calculate the permissions for.
@@ -151,65 +151,53 @@
     if not channel:
         return permissions
 
     return _calculate_channel_overwrites(channel, member, permissions)
 
 
 async def _fetch_channel(
-    client: tanjun.Client, channel: hikari.SnowflakeishOr[hikari.PartialChannel]
-) -> hikari.GuildChannel:
-    if isinstance(channel, hikari.GuildChannel):
+    client: tanjun.Client, channel: hikari.SnowflakeishOr[hikari.GuildChannel]
+) -> hikari.PermissibleGuildChannel:
+    if isinstance(channel, hikari.PermissibleGuildChannel):
         return channel
 
-    channel_id = hikari.Snowflake(channel)
-    if client.cache and (found_channel_ := client.cache.get_guild_channel(channel_id)):
-        return found_channel_
-
-    if channel_cache := client.get_type_dependency(_ChannelCacheT):
-        try:
-            return await channel_cache.get(channel_id)
-
-        except async_cache.EntryNotFound:
-            raise
-
-        except async_cache.CacheMissError:
-            pass
+    # If this is a non-permissible guild object then the assumption is that the parent
+    # channel has the perms as this is how it works under the current threads system.
+    if isinstance(channel, hikari.GuildChannel) and channel.parent_id:
+        channel = channel.parent_id
 
-    found_channel = await client.rest.fetch_channel(channel_id)
-    assert isinstance(found_channel, hikari.GuildChannel), "Cannot perform operation on a DM channel."
-    return found_channel
+    return await cache.get_perm_channel(client, hikari.Snowflake(channel))
 
 
-_ChannelCacheT = async_cache.SfCache[hikari.GuildChannel]
 _GuildCacheT = async_cache.SfCache[hikari.Guild]
 _RoleCacheT = async_cache.SfCache[hikari.Role]
 _GuldRoleCacheT = async_cache.SfGuildBound[hikari.Role]
 
 
 async def fetch_permissions(
     client: tanjun.Client,
     member: hikari.Member,
     /,
     *,
-    channel: typing.Optional[hikari.SnowflakeishOr[hikari.PartialChannel]] = None,
+    channel: typing.Optional[hikari.SnowflakeishOr[hikari.GuildChannel]] = None,
 ) -> hikari.Permissions:
     """Calculate the permissions a member has within a guild.
 
     !!! note
         This callback will fallback to REST requests if cache lookups fail or
         are not possible.
 
     Parameters
     ----------
     client
         The Tanjun client to use for lookups.
     member
         The object of the member to calculate the permissions for.
     channel
-        The object of ID of the channel to get their permissions in.
+        The object or ID of the channel to get their permissions in.
         If left as [None][] then this will return their base guild
         permissions.
 
     Returns
     -------
     hikari.Permissions
         The calculated permissions.
@@ -259,15 +247,15 @@
     return _calculate_channel_overwrites(channel, member, permissions)
 
 
 def calculate_everyone_permissions(
     everyone_role: hikari.Role,
     /,
     *,
-    channel: typing.Optional[hikari.GuildChannel] = None,
+    channel: typing.Optional[hikari.PermissibleGuildChannel] = None,
 ) -> hikari.Permissions:
     """Calculate a guild's default permissions within the guild or for a specific channel.
 
     Parameters
     ----------
     everyone_role
         The guild's default @everyone role.
@@ -300,15 +288,15 @@
 
 
 async def fetch_everyone_permissions(
     client: tanjun.Client,
     guild_id: hikari.Snowflake,
     /,
     *,
-    channel: typing.Optional[hikari.SnowflakeishOr[hikari.PartialChannel]] = None,
+    channel: typing.Optional[hikari.SnowflakeishOr[hikari.GuildChannel]] = None,
 ) -> hikari.Permissions:
     """Calculate the permissions a guild's default @everyone role has within a guild or for a specific channel.
 
     !!! note
         This callback will fallback to REST requests if cache lookups fail or
         are not possible.
```

### Comparing `hikari-tanjun-2.8.1a1/tanjun/schedules.py` & `hikari-tanjun-2.9.0a1/tanjun/schedules.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tanjun/utilities.py` & `hikari-tanjun-2.9.0a1/tanjun/utilities.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/__init__.py` & `hikari-tanjun-2.9.0a1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/commands/__init__.py` & `hikari-tanjun-2.9.0a1/tests/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/commands/test_base.py` & `hikari-tanjun-2.9.0a1/tests/commands/test_base.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/commands/test_menu.py` & `hikari-tanjun-2.9.0a1/tests/commands/test_menu.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/commands/test_message.py` & `hikari-tanjun-2.9.0a1/tests/commands/test_message.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/commands/test_slash.py` & `hikari-tanjun-2.9.0a1/tests/commands/test_slash.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/context/__init__.py` & `hikari-tanjun-2.9.0a1/tests/context/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/context/test_autocomplete.py` & `hikari-tanjun-2.9.0a1/tests/context/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/context/test_base.py` & `hikari-tanjun-2.9.0a1/tests/context/test_base.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/context/test_menu.py` & `hikari-tanjun-2.9.0a1/tests/context/test_menu.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/context/test_message.py` & `hikari-tanjun-2.9.0a1/tests/context/test_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,14 @@
                 "hi",
                 attachment=mock_attachment,
                 attachments=mock_attachments,
                 component=mock_component,
                 components=mock_components,
                 embed=mock_embed,
                 embeds=mock_embeds,
-                replace_attachments=True,
                 mentions_everyone=False,
                 user_mentions=[123, 321],
                 role_mentions=[321243],
             )
 
         mock_client.rest.edit_message.assert_awaited_once_with(
             context.message.channel_id,
@@ -286,15 +285,14 @@
             content="hi",
             attachment=mock_attachment,
             attachments=mock_attachments,
             component=mock_component,
             components=mock_components,
             embed=mock_embed,
             embeds=mock_embeds,
-            replace_attachments=True,
             mentions_everyone=False,
             user_mentions=[123, 321],
             role_mentions=[321243],
         )
         create_task.assert_not_called()
         mock_delete_after.assert_not_called()
         mock_register_task.assert_not_called()
@@ -350,15 +348,14 @@
             "hi",
             attachment=mock_attachment,
             attachments=mock_attachments,
             component=mock_component,
             components=mock_components,
             embed=mock_embed,
             embeds=mock_embeds,
-            replace_attachments=True,
             mentions_everyone=False,
             user_mentions=[123, 321],
             role_mentions=[321243],
         )
 
         mock_client.rest.edit_message.assert_awaited_once_with(
             context.message.channel_id,
@@ -366,15 +363,14 @@
             content="hi",
             attachment=mock_attachment,
             attachments=mock_attachments,
             component=mock_component,
             components=mock_components,
             embed=mock_embed,
             embeds=mock_embeds,
-            replace_attachments=True,
             mentions_everyone=False,
             user_mentions=[123, 321],
             role_mentions=[321243],
         )
         mock_register_task.assert_not_called()
         mock_delete_after.assert_not_called()
```

### Comparing `hikari-tanjun-2.8.1a1/tests/context/test_slash.py` & `hikari-tanjun-2.9.0a1/tests/context/test_slash.py`

 * *Files 0% similar despite different names*

```diff
@@ -851,29 +851,27 @@
                 "bye",
                 attachment=mock_attachment,
                 attachments=mock_attachments,
                 component=mock_component,
                 components=mock_components,
                 embed=mock_embed,
                 embeds=mock_embeds,
-                replace_attachments=False,
                 mentions_everyone=True,
                 user_mentions=[123],
                 role_mentions=[444],
             )
 
         mock_interaction.edit_initial_response.assert_awaited_once_with(
             content="bye",
             attachment=mock_attachment,
             attachments=mock_attachments,
             component=mock_component,
             components=mock_components,
             embed=mock_embed,
             embeds=mock_embeds,
-            replace_attachments=False,
             mentions_everyone=True,
             user_mentions=[123],
             role_mentions=[444],
         )
         create_task.assert_not_called()
         assert context.has_responded is True
         mock_register_task.assert_not_called()
```

### Comparing `hikari-tanjun-2.8.1a1/tests/dependencies/__init__.py` & `hikari-tanjun-2.9.0a1/tests/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/dependencies/test___init__.py` & `hikari-tanjun-2.9.0a1/tests/dependencies/test___init__.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/dependencies/test_callbacks.py` & `hikari-tanjun-2.9.0a1/tests/dependencies/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/dependencies/test_data.py` & `hikari-tanjun-2.9.0a1/tests/dependencies/test_data.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/dependencies/test_limiters.py` & `hikari-tanjun-2.9.0a1/tests/dependencies/test_limiters.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,101 +57,197 @@
     ],
 )
 @pytest.mark.asyncio()
 async def test__get_ctx_target(resource_type: tanjun.BucketResource, mock_ctx: tanjun.abc.Context, expected: int):
     assert await tanjun.dependencies.limiters._get_ctx_target(mock_ctx, resource_type) == expected
 
 
-@pytest.mark.parametrize(
-    ("channel", "result"),
-    [(mock.Mock(parent_id=None, id=123), 123), (mock.Mock(parent_id=54123123, id=123321), 123321)],
-)
 @pytest.mark.asyncio()
-async def test__get_ctx_target_when_parent_channel_and_cache_result(channel: mock.Mock, result: int):
+async def test__get_ctx_target_when_parent_channel_and_cache_result():
     mock_context = mock.Mock()
-    mock_context.get_channel.return_value = channel
+    mock_context.get_channel.return_value = mock.Mock(parent_id=5132, id=123321)
 
     result = await tanjun.dependencies.limiters._get_ctx_target(mock_context, tanjun.BucketResource.PARENT_CHANNEL)
 
-    assert result == result
+    assert result == 5132
     mock_context.get_channel.assert_called_once_with()
     mock_context.fetch_channel.assert_not_called()
     mock_context.get_type_dependency.assert_not_called()
 
 
-@pytest.mark.parametrize(
-    ("channel", "result"),
-    [(mock.Mock(parent_id=None, id=123), 123), (mock.Mock(parent_id=54123123, id=123321), 123321)],
-)
 @pytest.mark.asyncio()
-async def test__get_ctx_target_when_parent_channel_when_async_cache_returns_channel(channel: mock.Mock, result: int):
-    mock_cache = mock.AsyncMock()
-    mock_cache.get.return_value = channel
+async def test__get_ctx_target_when_parent_channel_and_cache_result_has_no_parent():
+    mock_context = mock.Mock()
+    mock_context.get_channel.return_value = mock.Mock(parent_id=None, id=6534234)
+
+    result = await tanjun.dependencies.limiters._get_ctx_target(mock_context, tanjun.BucketResource.PARENT_CHANNEL)
+
+    assert result == mock_context.guild_id
+    mock_context.get_channel.assert_called_once_with()
+    mock_context.fetch_channel.assert_not_called()
+    mock_context.get_type_dependency.assert_not_called()
+
+
+@pytest.mark.asyncio()
+async def test__get_ctx_target_when_parent_channel_when_async_channel_cache_returns():
+    mock_channel_cache = mock.AsyncMock()
+    mock_channel_cache.get.return_value = mock.Mock(parent_id=3421123, id=123321)
     mock_context = mock.Mock(base_context.BaseContext)
     mock_context.get_channel.return_value = None
-    mock_context.get_type_dependency.return_value = mock_cache
+    mock_context.get_type_dependency.return_value = mock_channel_cache
 
     result = await tanjun.dependencies.limiters._get_ctx_target(mock_context, tanjun.BucketResource.PARENT_CHANNEL)
 
-    assert result == result
+    assert result == 3421123
     mock_context.get_channel.assert_called_once_with()
-    mock_cache.get.assert_awaited_once_with(mock_context.channel_id, default=None)
+    mock_channel_cache.get.assert_awaited_once_with(mock_context.channel_id, default=None)
     mock_context.fetch_channel.assert_not_called()
-    mock_context.get_type_dependency.assert_called_once_with(tanjun.dependencies.SfCache[hikari.GuildChannel])
+    mock_context.get_type_dependency.assert_called_once_with(
+        tanjun.dependencies.SfCache[hikari.PermissibleGuildChannel]
+    )
 
 
-@pytest.mark.parametrize(
-    ("channel", "result"),
-    [
-        (mock.Mock(hikari.TextableGuildChannel, parent_id=None, id=123), 123),
-        (mock.Mock(hikari.TextableGuildChannel, parent_id=54123123, id=123321), 123321),
-    ],
-)
 @pytest.mark.asyncio()
-async def test__get_ctx_target_when_parent_channel_when_async_cache_returns_none_falls_back_to_rest(
-    channel: mock.Mock, result: int
-):
+async def test__get_ctx_target_when_parent_channel_when_async_channel_cache_returns_has_no_parent():
+    mock_channel_cache = mock.AsyncMock()
+    mock_channel_cache.get.return_value = mock.Mock(parent_id=None, id=123)
     mock_context = mock.Mock(base_context.BaseContext)
     mock_context.get_channel.return_value = None
-    mock_context.fetch_channel = mock.AsyncMock(return_value=channel)
-    mock_cache = mock.AsyncMock()
-    mock_cache.get.return_value = None
-    mock_context.get_type_dependency.return_value = mock_cache
+    mock_context.get_type_dependency.return_value = mock_channel_cache
 
     result = await tanjun.dependencies.limiters._get_ctx_target(mock_context, tanjun.BucketResource.PARENT_CHANNEL)
 
-    assert result == result
+    assert result == mock_context.guild_id
+    mock_context.get_channel.assert_called_once_with()
+    mock_channel_cache.get.assert_awaited_once_with(mock_context.channel_id, default=None)
+    mock_context.fetch_channel.assert_not_called()
+    mock_context.get_type_dependency.assert_called_once_with(
+        tanjun.dependencies.SfCache[hikari.PermissibleGuildChannel]
+    )
+
+
+@pytest.mark.asyncio()
+async def test__get_ctx_target_when_parent_channel_when_async_thread_cache_returns():
+    mock_channel_cache = mock.AsyncMock()
+    mock_channel_cache.get.return_value = None
+    mock_thread_cache = mock.AsyncMock()
+    mock_thread_cache.get.return_value = mock.Mock(parent_id=432453, id=123321)
+    mock_context = mock.Mock(base_context.BaseContext)
+    mock_context.get_channel.return_value = None
+    mock_context.get_type_dependency.side_effect = [mock_channel_cache, mock_thread_cache]
+
+    result = await tanjun.dependencies.limiters._get_ctx_target(mock_context, tanjun.BucketResource.PARENT_CHANNEL)
+
+    assert result == 432453
+    mock_context.get_channel.assert_called_once_with()
+    mock_channel_cache.get.assert_awaited_once_with(mock_context.channel_id, default=None)
+    mock_thread_cache.get.assert_awaited_once_with(mock_context.channel_id, default=None)
+    mock_context.fetch_channel.assert_not_called()
+    mock_context.get_type_dependency.assert_has_calls(
+        [
+            mock.call(tanjun.dependencies.SfCache[hikari.PermissibleGuildChannel]),
+            mock.call(tanjun.dependencies.SfCache[hikari.GuildThreadChannel]),
+        ]
+    )
+
+
+@pytest.mark.asyncio()
+async def test__get_ctx_target_when_parent_channel_when_async_caches_returns_none_falls_back_to_rest():
+    mock_context = mock.Mock(base_context.BaseContext)
+    mock_context.get_channel.return_value = None
+    mock_context.fetch_channel = mock.AsyncMock(
+        return_value=mock.Mock(hikari.GuildChannel, parent_id=4365123, id=123321)
+    )
+    mock_channel_cache = mock.AsyncMock()
+    mock_channel_cache.get.return_value = None
+    mock_thread_cache = mock.AsyncMock()
+    mock_thread_cache.get.return_value = None
+    mock_context.get_type_dependency.side_effect = [mock_channel_cache, mock_thread_cache]
+
+    result = await tanjun.dependencies.limiters._get_ctx_target(mock_context, tanjun.BucketResource.PARENT_CHANNEL)
+
+    assert result == 4365123
     mock_context.get_channel.assert_called_once_with()
     mock_context.fetch_channel.assert_awaited_once()
-    mock_context.get_type_dependency.assert_called_once_with(tanjun.dependencies.SfCache[hikari.GuildChannel])
-    mock_cache.get.assert_awaited_once_with(mock_context.channel_id, default=None)
+    mock_context.get_type_dependency.assert_has_calls(
+        [
+            mock.call(tanjun.dependencies.SfCache[hikari.PermissibleGuildChannel]),
+            mock.call(tanjun.dependencies.SfCache[hikari.GuildThreadChannel]),
+        ]
+    )
+    mock_channel_cache.get.assert_awaited_once_with(mock_context.channel_id, default=None)
+    mock_thread_cache.get.assert_awaited_once_with(mock_context.channel_id, default=None)
+
+
+@pytest.mark.asyncio()
+async def test__get_ctx_target_when_parent_channel_when_async_caches_returns_none_falls_back_to_rest_has_no_parent():
+    mock_context = mock.Mock(base_context.BaseContext)
+    mock_context.get_channel.return_value = None
+    mock_context.fetch_channel = mock.AsyncMock(return_value=mock.Mock(hikari.GuildChannel, parent_id=None, id=123))
+    mock_channel_cache = mock.AsyncMock()
+    mock_channel_cache.get.return_value = None
+    mock_thread_cache = mock.AsyncMock()
+    mock_thread_cache.get.return_value = None
+    mock_context.get_type_dependency.side_effect = [mock_channel_cache, mock_thread_cache]
+
+    result = await tanjun.dependencies.limiters._get_ctx_target(mock_context, tanjun.BucketResource.PARENT_CHANNEL)
+
+    assert result == mock_context.guild_id
+    mock_context.get_channel.assert_called_once_with()
+    mock_context.fetch_channel.assert_awaited_once()
+    mock_context.get_type_dependency.assert_has_calls(
+        [
+            mock.call(tanjun.dependencies.SfCache[hikari.PermissibleGuildChannel]),
+            mock.call(tanjun.dependencies.SfCache[hikari.GuildThreadChannel]),
+        ]
+    )
+    mock_channel_cache.get.assert_awaited_once_with(mock_context.channel_id, default=None)
+    mock_thread_cache.get.assert_awaited_once_with(mock_context.channel_id, default=None)
+
+
+@pytest.mark.asyncio()
+async def test__get_ctx_target_when_parent_channel_and_no_async_caches_falls_back_to_rest():
+    mock_context = mock.Mock(base_context.BaseContext)
+    mock_context.get_channel.return_value = None
+    mock_context.fetch_channel = mock.AsyncMock(
+        return_value=mock.Mock(hikari.GuildChannel, parent_id=1235234, id=123321)
+    )
+    mock_context.get_type_dependency.return_value = alluka.abc.UNDEFINED
+
+    result = await tanjun.dependencies.limiters._get_ctx_target(mock_context, tanjun.BucketResource.PARENT_CHANNEL)
+
+    assert result == 1235234
+    mock_context.get_channel.assert_called_once_with()
+    mock_context.fetch_channel.assert_awaited_once()
+    mock_context.get_type_dependency.assert_has_calls(
+        [
+            mock.call(tanjun.dependencies.SfCache[hikari.PermissibleGuildChannel]),
+            mock.call(tanjun.dependencies.SfCache[hikari.GuildThreadChannel]),
+        ]
+    )
 
 
-@pytest.mark.parametrize(
-    ("channel", "result"),
-    [
-        (mock.Mock(hikari.TextableGuildChannel, parent_id=None, id=123), 123),
-        (mock.Mock(hikari.TextableGuildChannel, parent_id=54123123, id=123321), 123321),
-    ],
-)
 @pytest.mark.asyncio()
-async def test__get_ctx_target_when_parent_channel_and_no_async_cache_falls_back_to_rest(
-    channel: mock.Mock, result: int
-):
+async def test__get_ctx_target_when_parent_channel_and_no_async_caches_falls_back_to_rest_has_no_parent():
     mock_context = mock.Mock(base_context.BaseContext)
     mock_context.get_channel.return_value = None
-    mock_context.fetch_channel = mock.AsyncMock(return_value=channel)
+    mock_context.fetch_channel = mock.AsyncMock(return_value=mock.Mock(hikari.GuildChannel, parent_id=None, id=123))
     mock_context.get_type_dependency.return_value = alluka.abc.UNDEFINED
 
     result = await tanjun.dependencies.limiters._get_ctx_target(mock_context, tanjun.BucketResource.PARENT_CHANNEL)
 
-    assert result == result
+    assert result == mock_context.guild_id
     mock_context.get_channel.assert_called_once_with()
     mock_context.fetch_channel.assert_awaited_once()
-    mock_context.get_type_dependency.assert_called_once_with(tanjun.dependencies.SfCache[hikari.GuildChannel])
+    mock_context.get_type_dependency.assert_has_calls(
+        [
+            mock.call(tanjun.dependencies.SfCache[hikari.PermissibleGuildChannel]),
+            mock.call(tanjun.dependencies.SfCache[hikari.GuildThreadChannel]),
+        ]
+    )
 
 
 @pytest.mark.asyncio()
 async def test__get_ctx_target_when_parent_channel_and_dm_bound():
     mock_context = mock.Mock(guild_id=None)
 
     result = await tanjun.dependencies.limiters._get_ctx_target(mock_context, tanjun.BucketResource.PARENT_CHANNEL)
```

### Comparing `hikari-tanjun-2.8.1a1/tests/dependencies/test_locales.py` & `hikari-tanjun-2.9.0a1/tests/dependencies/test_locales.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/dependencies/test_owners.py` & `hikari-tanjun-2.9.0a1/tests/dependencies/test_owners.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/dependencies/test_reloaders.py` & `hikari-tanjun-2.9.0a1/tests/dependencies/test_reloaders.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test__internal.py` & `hikari-tanjun-2.9.0a1/tests/test__internal/test_init.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_annotations.py` & `hikari-tanjun-2.9.0a1/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_annotations_future_annotations.py` & `hikari-tanjun-2.9.0a1/tests/test_annotations_future_annotations.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_checks.py` & `hikari-tanjun-2.9.0a1/tests/test_checks.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from collections import abc as collections
 from unittest import mock
 
 import hikari
 import pytest
 
 import tanjun
+from tanjun._internal import cache
 
 
 @pytest.fixture()
 def command() -> tanjun.abc.ExecutableCommand[typing.Any]:
     command_ = mock.MagicMock(tanjun.abc.ExecutableCommand)
     command_.add_check.return_value = command_
     return command_
@@ -255,254 +256,166 @@
         mock_dependency.check_ownership.assert_awaited_once_with(mock_context.client, mock_context.author)
 
 
 @pytest.mark.asyncio()
 class TestNsfwCheck:
     async def test_when_is_dm(self):
         mock_context = mock.Mock(guild_id=None)
-        mock_cache = mock.AsyncMock()
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.NsfwCheck(error=TypeError, error_message="meep", halt_execution=True)
 
-        result = await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            result = await check(mock_context)
 
         assert result is True
-        mock_context.cache.get_guild_channel.assert_not_called()
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_not_called()
 
     async def test(self):
         mock_context = mock.Mock()
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = True
-        mock_cache = mock.AsyncMock()
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.NsfwCheck(error_message=None)
 
-        result = await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            result = await check(mock_context)
 
         assert result is True
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
-
-    async def test_when_async_cache_raises_not_found(self):
-        mock_context = mock.Mock(cache=None, rest=mock.AsyncMock())
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.EntryNotFound
-        check = tanjun.checks.NsfwCheck(error_message=None)
-
-        with pytest.raises(tanjun.dependencies.EntryNotFound):
-            await check(mock_context, channel_cache=mock_cache)
-
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_called_once_with(mock_context.channel_id)
-
-    async def test_when_not_cache_bound_and_async_cache_hit(self):
-        mock_context = mock.Mock(cache=None, rest=mock.AsyncMock())
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.return_value.is_nsfw = True
-        check = tanjun.checks.NsfwCheck(error_message=None)
-
-        result = await check(mock_context, channel_cache=mock_cache)
-
-        assert result is True
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_called_once_with(mock_context.channel_id)
-
-    async def test_when_not_found_in_cache_and_async_cache_hit(self):
-        mock_context = mock.Mock(rest=mock.AsyncMock())
-        mock_context.cache.get_guild_channel.return_value = None
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.return_value.is_nsfw = None
-        check = tanjun.checks.NsfwCheck(error_message=None)
-
-        result = await check(mock_context, channel_cache=mock_cache)
-
-        assert result is False
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_called_once_with(mock_context.channel_id)
-
-    async def test_when_not_cache_bound(self):
-        mock_context = mock.Mock(cache=None, rest=mock.AsyncMock())
-        mock_context.rest.fetch_channel.return_value = mock.Mock(hikari.GuildChannel, is_nsfw=True)
-        check = tanjun.checks.NsfwCheck(error_message=None)
-
-        result = await check(mock_context, channel_cache=None)
-
-        assert result is True
-        mock_context.rest.fetch_channel.assert_awaited_once_with(mock_context.channel_id)
-
-    async def test_when_not_found_in_cache(self):
-        mock_context = mock.Mock(rest=mock.AsyncMock())
-        mock_context.cache.get_guild_channel.return_value = None
-        mock_context.rest.fetch_channel.return_value = mock.Mock(hikari.GuildChannel, is_nsfw=True)
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
-        check = tanjun.checks.NsfwCheck(error_message=None)
-
-        result = await check(mock_context, channel_cache=mock_cache)
-
-        assert result is True
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_awaited_once_with(mock_context.channel_id)
-        mock_cache.get.assert_awaited_once_with(mock_context.channel_id)
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_false(self):
-        mock_context = mock.Mock()
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = None
+        mock_context = mock.Mock(client=tanjun.Client(mock.AsyncMock(), cache=mock.Mock()))
         check = tanjun.checks.NsfwCheck(error_message=None)
 
-        result = await check(mock_context, channel_cache=None)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=None)) as get_perm_channel:
+            result = await check(mock_context)
 
         assert result is False
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_false_when_error(self):
         class MockException(Exception):
             def __init__(self):
                 ...
 
-        mock_context = mock.Mock()
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = None
+        mock_context = mock.Mock(client=tanjun.Client(mock.AsyncMock(), cache=mock.Mock()))
         check = tanjun.checks.NsfwCheck(error=MockException, error_message="nye")
 
-        with pytest.raises(MockException):
-            await check(mock_context, channel_cache=None)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=None)) as get_perm_channel:
+            with pytest.raises(MockException):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_false_and_error_message(self):
         mock_context = mock.Mock()
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = False
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.NsfwCheck(error_message="meow me")
 
-        with pytest.raises(tanjun.errors.CommandError, match="meow me"):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=False)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="meow me"):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_false_and_error_message_dict(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext)
         mock_context.interaction.locale = hikari.Locale.HU
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = False
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.NsfwCheck(
             error_message={hikari.Locale.DE: "oh", hikari.Locale.HU: "no", hikari.Locale.EN_GB: "meow"}
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="no"):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=False)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="no"):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_false_and_error_message_dict_but_not_app_command(self):
         mock_context = mock.Mock(tanjun.abc.Context)
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = False
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.NsfwCheck(
             error_message={
                 hikari.Locale.DE: "op",
                 "default": "defaulted",
                 hikari.Locale.HU: "no",
                 hikari.Locale.EN_GB: "meow",
             }
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="defaulted"):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=False)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="defaulted"):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_false_and_error_message_dict_defaults(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext)
         mock_context.interaction.locale = hikari.Locale.DA
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = False
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.NsfwCheck(
             error_message={
                 hikari.Locale.DE: "default default default",
                 hikari.Locale.HU: "no",
                 hikari.Locale.EN_GB: "meow",
             }
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="default default default"):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=False)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="default default default"):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_false_and_error_message_dict_explicit_default(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext)
         mock_context.interaction.locale = hikari.Locale.DA
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = False
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.NsfwCheck(
             error_message={
                 hikari.Locale.DE: "default default default",
                 "default": "real default",
                 hikari.Locale.HU: "no",
                 hikari.Locale.EN_GB: "meow",
             }
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="real default"):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=False)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="real default"):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_false_and_error_message_localiser(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext, triggering_name="meow meow")
         mock_context.type = hikari.CommandType.USER
         mock_context.interaction.locale = hikari.Locale.EN_GB
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = False
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.NsfwCheck(
             error_message={
                 hikari.Locale.DE: "default default default",
                 hikari.Locale.HU: "no",
                 hikari.Locale.EN_GB: "meow",
             }
         )
         localiser = tanjun.dependencies.BasicLocaliser().set_variants(
             "user_menu:meow meow:check:tanjun.NsfwCheck",
             {hikari.Locale.CS: "n", hikari.Locale.EN_GB: "override", hikari.Locale.FI: "i'm finished"},
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="override"):
-            await check(mock_context, channel_cache=mock_cache, localiser=localiser)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=False)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="override"):
+                await check(mock_context, localiser=localiser)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_false_and_error_message_localiser_overridden_id(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext, triggering_name="meow meow")
         mock_context.type = hikari.CommandType.USER
         mock_context.interaction.locale = hikari.Locale.EN_GB
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = False
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.NsfwCheck(
             error_message={
                 hikari.Locale.DE: "default default default",
                 hikari.Locale.HU: "no",
                 "id": "cthulhu calls",
                 hikari.Locale.EN_GB: "meow",
             }
@@ -512,28 +425,25 @@
             .set_variants(
                 "user_menu:meow meow:check:tanjun.NsfwCheck",
                 {hikari.Locale.CS: "n", hikari.Locale.EN_GB: "override", hikari.Locale.FI: "i'm finished"},
             )
             .set_variants("cthulhu calls", {hikari.Locale.EN_GB: "wowzer Fred, I'm gay", hikari.Locale.CS: "meow"})
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="wowzer Fred, I'm gay"):
-            await check(mock_context, channel_cache=mock_cache, localiser=localiser)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=False)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="wowzer Fred, I'm gay"):
+                await check(mock_context, localiser=localiser)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_false_and_error_message_localiser_defaults(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext, triggering_name="meow meow")
         mock_context.type = hikari.CommandType.USER
         mock_context.interaction.locale = hikari.Locale.FR
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = False
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.NsfwCheck(
             error_message={
                 hikari.Locale.DE: "default default default",
                 hikari.Locale.HU: "no",
                 hikari.Locale.EN_GB: "meow",
             }
         )
@@ -542,260 +452,179 @@
             .set_variants(
                 "user_menu:meow meow:check:tanjun.NsfwCheck",
                 {hikari.Locale.CS: "n", hikari.Locale.EN_GB: "override", hikari.Locale.FI: "i'm finished"},
             )
             .set_variants("cthulhu calls", {hikari.Locale.EN_GB: "wowzer Fred, I'm gay", hikari.Locale.CS: "meow"})
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="default default default"):
-            await check(mock_context, channel_cache=mock_cache, localiser=localiser)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=False)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="default default default"):
+                await check(mock_context, localiser=localiser)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_false_and_halt_execution(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
-        mock_context.cache.get_guild_channel.return_value = None
-        mock_context.rest.fetch_channel.return_value = mock.Mock(hikari.GuildChannel, is_nsfw=False)
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.NsfwCheck(error_message="yeet", halt_execution=True)
 
-        with pytest.raises(tanjun.errors.HaltExecution):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=False)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.HaltExecution):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_awaited_once_with(mock_context.channel_id)
-        mock_cache.get.assert_awaited_once_with(mock_context.channel_id)
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
 
 @pytest.mark.asyncio()
 class TestSfwCheck:
     async def test_when_is_dm(self):
         mock_context = mock.Mock(guild_id=None)
-        mock_cache = mock.AsyncMock()
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.SfwCheck(error=ValueError, error_message="lll", halt_execution=True)
 
-        result = await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            result = await check(mock_context)
 
         assert result is True
-        mock_context.cache.get_guild_channel.assert_not_called()
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_not_called()
 
     async def test(self):
         mock_context = mock.Mock()
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = False
-        mock_cache = mock.AsyncMock()
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.SfwCheck(error_message=None)
 
-        result = await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=False)) as get_perm_channel:
+            result = await check(mock_context)
 
         assert result is True
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
-
-    async def test_when_not_cache_bound_and_async_cache_hit(self):
-        mock_context = mock.Mock(cache=None, rest=mock.AsyncMock())
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.return_value.is_nsfw = False
-        check = tanjun.checks.SfwCheck(error_message=None)
-
-        result = await check(mock_context, channel_cache=mock_cache)
-
-        assert result is True
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_called_once_with(mock_context.channel_id)
-
-    async def test_when_not_found_in_cache_and_async_cache_hit(self):
-        mock_context = mock.Mock(rest=mock.AsyncMock())
-        mock_context.cache.get_guild_channel.return_value = None
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.return_value.is_nsfw = None
-        check = tanjun.checks.SfwCheck(error_message=None)
-
-        result = await check(mock_context, channel_cache=mock_cache)
-
-        assert result is True
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_called_once_with(mock_context.channel_id)
-
-    async def test_when_not_cache_bound(self):
-        mock_context = mock.Mock(cache=None, rest=mock.AsyncMock())
-        mock_context.rest.fetch_channel.return_value = mock.Mock(hikari.GuildChannel, is_nsfw=True)
-        check = tanjun.checks.SfwCheck(error_message=None)
-
-        result = await check(mock_context, channel_cache=None)
-
-        assert result is False
-        mock_context.rest.fetch_channel.assert_awaited_once_with(mock_context.channel_id)
-
-    async def test_when_not_found_in_cache(self):
-        mock_context = mock.Mock(rest=mock.AsyncMock())
-        mock_context.cache.get_guild_channel.return_value = None
-        mock_context.rest.fetch_channel.return_value = mock.Mock(hikari.GuildChannel, is_nsfw=True)
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
-        check = tanjun.checks.SfwCheck(error_message=None)
-
-        result = await check(mock_context, channel_cache=mock_cache)
-
-        assert result is False
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_awaited_once_with(mock_context.channel_id)
-        mock_cache.get.assert_awaited_once_with(mock_context.channel_id)
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_is_nsfw(self):
-        mock_context = mock.Mock()
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = True
+        mock_context = mock.Mock(client=tanjun.Client(mock.AsyncMock(), cache=mock.Mock()))
         check = tanjun.checks.SfwCheck(error_message=None)
 
-        result = await check(mock_context, channel_cache=None)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            result = await check(mock_context)
 
         assert result is False
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_is_nsfw_and_error(self):
         class MockException(Exception):
             def __init__(self):
                 ...
 
-        mock_context = mock.Mock()
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = True
+        mock_context = mock.Mock(client=tanjun.Client(mock.AsyncMock(), cache=mock.Mock()))
         check = tanjun.checks.SfwCheck(error=MockException, error_message="bye")
 
-        with pytest.raises(MockException):
-            await check(mock_context, channel_cache=None)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            with pytest.raises(MockException):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_is_nsfw_and_error_message(self):
         mock_context = mock.Mock()
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = True
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.SfwCheck(error_message="meow me")
 
-        with pytest.raises(tanjun.errors.CommandError, match="meow me"):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="meow me"):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_is_nsfw_and_error_message_dict(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext)
         mock_context.interaction.locale = hikari.Locale.DA
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = True
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.SfwCheck(
             error_message={hikari.Locale.BG: "oooooo", hikari.Locale.DA: "moooo", hikari.Locale.EN_GB: "pussy cat"}
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="moooo"):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="moooo"):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_is_nsfw_and_error_message_dict_but_not_app_command(self):
         mock_context = mock.Mock(tanjun.abc.Context)
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = True
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.SfwCheck(
             error_message={
                 hikari.Locale.BG: "oooooo",
                 "default": "bye bye",
                 hikari.Locale.DA: "moooo",
                 hikari.Locale.EN_GB: "pussy cat",
             }
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="bye bye"):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="bye bye"):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_is_nsfw_and_error_message_dict_defaults(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext)
         mock_context.interaction.locale = hikari.Locale.FR
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = True
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.SfwCheck(
             error_message={hikari.Locale.BG: "oooooo", hikari.Locale.DA: "moooo", hikari.Locale.EN_GB: "pussy cat"}
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="oooooo"):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="oooooo"):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_is_nsfw_and_error_message_dict_explicit_default(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext)
         mock_context.interaction.locale = hikari.Locale.FR
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = True
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.SfwCheck(
             error_message={
                 hikari.Locale.BG: "oooooo",
                 hikari.Locale.DA: "moooo",
                 hikari.Locale.EN_GB: "pussy cat",
                 "default": "oh no",
             }
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="oh no"):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="oh no"):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_is_nsfw_and_error_message_localiser(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext, triggering_name="oh no girl")
         mock_context.type = hikari.CommandType.USER
         mock_context.interaction.locale = hikari.Locale.DA
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = True
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.SfwCheck(
             error_message={hikari.Locale.BG: "oooooo", hikari.Locale.DA: "moooo", hikari.Locale.EN_GB: "pussy cat"}
         )
         localiser = tanjun.dependencies.BasicLocaliser().set_variants(
             "user_menu:oh no girl:check:tanjun.SfwCheck", {hikari.Locale.DA: "real value", hikari.Locale.BG: "op"}
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="real value"):
-            await check(mock_context, channel_cache=mock_cache, localiser=localiser)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="real value"):
+                await check(mock_context, localiser=localiser)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_is_nsfw_and_error_message_localiser_overridden_id(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext, triggering_name="oh no girl")
         mock_context.type = hikari.CommandType.USER
         mock_context.interaction.locale = hikari.Locale.EN_GB
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = True
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.SfwCheck(
             error_message={
                 hikari.Locale.BG: "oooooo",
                 hikari.Locale.DA: "moooo",
                 "id": "meow meow meow meow",
                 hikari.Locale.EN_GB: "pussy cat",
             }
@@ -814,28 +643,25 @@
                 {
                     hikari.Locale.EN_GB: "Passing you like a summer breeze",
                     hikari.Locale.EN_US: "You feel life has no other reason to be",
                 },
             )
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="Passing you like a summer breeze"):
-            await check(mock_context, channel_cache=mock_cache, localiser=localiser)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="Passing you like a summer breeze"):
+                await check(mock_context, localiser=localiser)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_is_nsfw_and_error_message_localiser_defaults(self):
         mock_context = mock.Mock(tanjun.abc.AppCommandContext, triggering_name="oh no girl")
         mock_context.type = hikari.CommandType.USER
         mock_context.interaction.locale = hikari.Locale.DE
-        mock_context.cache.get_guild_channel.return_value.is_nsfw = True
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.SfwCheck(
             error_message={
                 hikari.Locale.JA: "years of meows",
                 hikari.Locale.DA: "moooo",
                 "id": "meow meow meow meow",
                 hikari.Locale.EN_GB: "pussy cat",
             }
@@ -854,35 +680,30 @@
                 {
                     hikari.Locale.EN_GB: "Passing you like a summer breeze",
                     hikari.Locale.EN_US: "You feel life has no other reason to be",
                 },
             )
         )
 
-        with pytest.raises(tanjun.errors.CommandError, match="years of meows"):
-            await check(mock_context, channel_cache=mock_cache, localiser=localiser)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.CommandError, match="years of meows"):
+                await check(mock_context, localiser=localiser)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
     async def test_when_is_nsfw_and_halt_execution(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
-        mock_context.cache.get_guild_channel.return_value = None
-        mock_context.rest.fetch_channel.return_value = mock.Mock(hikari.GuildChannel, is_nsfw=True)
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_context.client = tanjun.Client(mock.AsyncMock(), cache=mock.Mock())
         check = tanjun.checks.SfwCheck(error_message="yeet", halt_execution=True)
 
-        with pytest.raises(tanjun.errors.HaltExecution):
-            await check(mock_context, channel_cache=mock_cache)
+        with mock.patch.object(cache, "get_perm_channel", return_value=mock.Mock(is_nsfw=True)) as get_perm_channel:
+            with pytest.raises(tanjun.errors.HaltExecution):
+                await check(mock_context)
 
-        mock_context.cache.get_guild_channel.assert_called_once_with(mock_context.channel_id)
-        mock_context.rest.fetch_channel.assert_awaited_once_with(mock_context.channel_id)
-        mock_cache.get.assert_awaited_once_with(mock_context.channel_id)
+        get_perm_channel.assert_awaited_once_with(mock_context.client, mock_context.channel_id)
 
 
 class TestDmCheck:
     def test_for_dm(self):
         check = tanjun.checks.DmCheck(error=ValueError, error_message="meow", halt_execution=True)
         assert check(mock.Mock(guild_id=None)) is True
```

### Comparing `hikari-tanjun-2.8.1a1/tests/test_clients.py` & `hikari-tanjun-2.9.0a1/tests/test_clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,17 +276,61 @@
 
 class TestClient:
     @pytest.mark.skip(reason="TODO")
     def test___init__(self):
         ...
 
     @pytest.mark.skip(reason="TODO")
+    def test_from_gateway_bot(self):
+        ...
+
+    @pytest.mark.skip(reason="TODO")
+    def test_from_rest_bot(self):
+        ...
+
+    def test_from_rest_bot_when_bot_managed(self):
+        mock_bot = mock.Mock()
+
+        client = tanjun.Client.from_rest_bot(mock_bot, bot_managed=True)
+
+        mock_bot.add_startup_callback.assert_called_once_with(client._on_starting)
+        mock_bot.add_shutdown_callback.assert_called_once_with(client._on_stopping)
+
+    @pytest.mark.skip(reason="TODO")
     def test___repr__(self):
         ...
 
+    @pytest.mark.asyncio()
+    async def test__on_starting(self):
+        mock_open = mock.AsyncMock()
+        mock_rest = mock.AsyncMock()
+
+        class TestClient(tanjun.Client):
+            open = mock_open
+
+        client = TestClient(mock_rest)
+
+        await client._on_starting(mock.Mock())
+
+        mock_open.assert_awaited_once_with()
+
+    @pytest.mark.asyncio()
+    async def test__on_stopping(self):
+        mock_close = mock.AsyncMock()
+        mock_rest = mock.AsyncMock()
+
+        class TestClient(tanjun.Client):
+            close = mock_close
+
+        client = TestClient(mock_rest)
+
+        await client._on_stopping(mock.Mock())
+
+        mock_close.assert_awaited_once_with()
+
     @pytest.mark.skip(reason="TODO")
     def test__schedule_startup_registers(self):
         ...
 
     @pytest.mark.asyncio()
     async def test__add_task(self):
         mock_task_1 = mock.Mock()
@@ -329,22 +373,14 @@
         await asyncio.sleep(0)
 
         client = tanjun.Client(mock.AsyncMock())
 
         client._add_task(mock_task)
         assert client._tasks == []
 
-    @pytest.mark.skip(reason="TODO")
-    def test_from_gateway_bot(self):
-        ...
-
-    @pytest.mark.skip(reason="TODO")
-    def test_from_rest_bot(self):
-        ...
-
     @pytest.mark.asyncio()
     async def test_context_manager(self):
         open_ = mock.AsyncMock()
         close_ = mock.AsyncMock()
 
         class MockClient(tanjun.Client):
             open = open_
```

### Comparing `hikari-tanjun-2.8.1a1/tests/test_clients_future_annotations.py` & `hikari-tanjun-2.9.0a1/tests/test_clients_future_annotations.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_components.py` & `hikari-tanjun-2.9.0a1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_components_future_annotations.py` & `hikari-tanjun-2.9.0a1/tests/test_components_future_annotations.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_conversion.py` & `hikari-tanjun-2.9.0a1/tests/test_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,248 +107,375 @@
         assert obj.requires_cache is expected
 
 
 class TestChannelConverter:
     @pytest.mark.asyncio()
     async def test___call___when_cached(self):
         mock_context = mock.Mock()
-        mock_cache = mock.AsyncMock()
+        mock_channel_cache = mock.AsyncMock()
         mock_dm_cache = mock.AsyncMock()
+        mock_thread_cache = mock.AsyncMock()
 
-        result = await tanjun.to_channel("123321", mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+        result = await tanjun.to_channel(
+            "123321", mock_context, cache=mock_channel_cache, dm_cache=mock_dm_cache, thread_cache=mock_thread_cache
+        )
 
         assert result is mock_context.cache.get_guild_channel.return_value
         mock_context.cache.get_guild_channel.assert_called_once_with(123321)
         mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_not_called()
+        mock_channel_cache.get.assert_not_called()
         mock_dm_cache.get.assert_not_called()
+        mock_thread_cache.get.assert_not_called()
 
     @pytest.mark.asyncio()
     async def test___call___when_not_cached_and_no_async_cache(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache.get_guild_channel.return_value = None
 
-        result = await tanjun.to_channel("<#12222>", mock_context, cache=None, dm_cache=None)
+        result = await tanjun.to_channel("<#12222>", mock_context)
 
         assert result is mock_context.rest.fetch_channel.return_value
         mock_context.cache.get_guild_channel.assert_called_once_with(12222)
         mock_context.rest.fetch_channel.assert_awaited_once_with(12222)
 
     @pytest.mark.asyncio()
     async def test___call___when_cacheless_and_no_async_cache(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache = None
 
-        result = await tanjun.to_channel(222, mock_context, cache=None, dm_cache=None)
+        result = await tanjun.to_channel(222, mock_context)
 
         assert result is mock_context.rest.fetch_channel.return_value
         mock_context.rest.fetch_channel.assert_awaited_once_with(222)
 
     @pytest.mark.asyncio()
     async def test___call___when_not_cached_and_async_channel_cache_hit(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache.get_guild_channel.return_value = None
-        mock_cache = mock.AsyncMock()
+        mock_channel_cache = mock.AsyncMock()
         mock_dm_cache = mock.AsyncMock()
+        mock_thread_cache = mock.AsyncMock()
 
-        result = await tanjun.to_channel("<#12222>", mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+        result = await tanjun.to_channel(
+            "<#12222>", mock_context, cache=mock_channel_cache, dm_cache=mock_dm_cache, thread_cache=mock_thread_cache
+        )
 
-        assert result is mock_cache.get.return_value
+        assert result is mock_channel_cache.get.return_value
         mock_context.cache.get_guild_channel.assert_called_once_with(12222)
         mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_awaited_once_with(12222)
+        mock_channel_cache.get.assert_awaited_once_with(12222)
         mock_dm_cache.get.assert_not_called()
+        mock_thread_cache.get.assert_not_called()
+
+    @pytest.mark.parametrize("side_effect", [tanjun.dependencies.CacheMissError, tanjun.dependencies.EntryNotFound])
+    @pytest.mark.asyncio()
+    async def test___call___when_not_cached_and_async_thread_cache_hit(self, side_effect: type[Exception]):
+        mock_context = mock.Mock(rest=mock.AsyncMock())
+        mock_context.cache.get_guild_channel.return_value = None
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = side_effect
+        mock_dm_cache = mock.AsyncMock()
+        mock_thread_cache = mock.AsyncMock()
+
+        result = await tanjun.to_channel(
+            "<#12222>", mock_context, cache=mock_channel_cache, dm_cache=mock_dm_cache, thread_cache=mock_thread_cache
+        )
+
+        assert result is mock_thread_cache.get.return_value
+        mock_context.cache.get_guild_channel.assert_called_once_with(12222)
+        mock_context.rest.fetch_channel.assert_not_called()
+        mock_channel_cache.get.assert_awaited_once_with(12222)
+        mock_dm_cache.get.assert_not_called()
+        mock_thread_cache.get.assert_awaited_once_with(12222)
 
     @pytest.mark.parametrize("side_effect", [tanjun.dependencies.CacheMissError, tanjun.dependencies.EntryNotFound])
     @pytest.mark.asyncio()
     async def test___call___when_not_cached_and_async_dm_cache_hit(self, side_effect: type[Exception]):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache.get_guild_channel.return_value = None
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = side_effect
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = side_effect
         mock_dm_cache = mock.AsyncMock()
+        mock_thread_cache = mock.AsyncMock()
+        mock_thread_cache.get.side_effect = side_effect
 
-        result = await tanjun.to_channel("<#12222>", mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+        result = await tanjun.to_channel(
+            "<#12222>", mock_context, cache=mock_channel_cache, dm_cache=mock_dm_cache, thread_cache=mock_thread_cache
+        )
 
         assert result is mock_dm_cache.get.return_value
         mock_context.cache.get_guild_channel.assert_called_once_with(12222)
         mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_awaited_once_with(12222)
+        mock_channel_cache.get.assert_awaited_once_with(12222)
         mock_dm_cache.get.assert_awaited_once_with(12222)
+        mock_thread_cache.get.assert_awaited_once_with(12222)
 
     @pytest.mark.asyncio()
     async def test___call___when_not_cached_async_cache_raises_not_found_and_not_including_dms(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache.get_guild_channel.return_value = None
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.EntryNotFound
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = tanjun.dependencies.EntryNotFound
         mock_dm_cache = mock.AsyncMock()
+        mock_thread_cache = mock.AsyncMock()
+        mock_thread_cache.get.side_effect = tanjun.dependencies.EntryNotFound
         converter = tanjun.conversion.ChannelConverter(include_dms=False)
 
         with pytest.raises(ValueError, match="Couldn't find channel"):
-            await converter("<#12222>", mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+            await converter(
+                "<#12222>",
+                mock_context,
+                cache=mock_channel_cache,
+                dm_cache=mock_dm_cache,
+                thread_cache=mock_thread_cache,
+            )
 
         mock_context.cache.get_guild_channel.assert_called_once_with(12222)
         mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_awaited_once_with(12222)
+        mock_channel_cache.get.assert_awaited_once_with(12222)
         mock_dm_cache.get.assert_not_called()
+        mock_thread_cache.get.assert_awaited_once_with(12222)
 
     @pytest.mark.asyncio()
     async def test___call___when_cacheless_and_async_channel_cache_hit(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache = None
-        mock_cache = mock.AsyncMock()
+        mock_channel_cache = mock.AsyncMock()
         mock_dm_cache = mock.AsyncMock()
+        mock_thread_cache = mock.AsyncMock()
 
-        result = await tanjun.to_channel(222, mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+        result = await tanjun.to_channel(
+            222, mock_context, cache=mock_channel_cache, dm_cache=mock_dm_cache, thread_cache=mock_thread_cache
+        )
 
-        assert result is mock_cache.get.return_value
+        assert result is mock_channel_cache.get.return_value
         mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_awaited_once_with(222)
+        mock_channel_cache.get.assert_awaited_once_with(222)
         mock_dm_cache.get.assert_not_called()
+        mock_thread_cache.get.assert_not_called()
+
+    @pytest.mark.parametrize("side_effect", [tanjun.dependencies.CacheMissError, tanjun.dependencies.EntryNotFound])
+    @pytest.mark.asyncio()
+    async def test___call___when_cacheless_and_async_thread_cache_hit(self, side_effect: type[Exception]):
+        mock_context = mock.Mock(rest=mock.AsyncMock())
+        mock_context.cache = None
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = side_effect
+        mock_dm_cache = mock.AsyncMock()
+        mock_thread_cache = mock.AsyncMock()
+
+        result = await tanjun.to_channel(
+            222, mock_context, cache=mock_channel_cache, dm_cache=mock_dm_cache, thread_cache=mock_thread_cache
+        )
+
+        assert result is mock_thread_cache.get.return_value
+        mock_context.rest.fetch_channel.assert_not_called()
+        mock_channel_cache.get.assert_awaited_once_with(222)
+        mock_dm_cache.get.assert_not_called()
+        mock_thread_cache.get.assert_awaited_once_with(222)
 
     @pytest.mark.parametrize("side_effect", [tanjun.dependencies.CacheMissError, tanjun.dependencies.EntryNotFound])
     @pytest.mark.asyncio()
     async def test___call___when_cacheless_and_async_dm_cache_hit(selff, side_effect: type[Exception]):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache = None
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = side_effect
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = side_effect
         mock_dm_cache = mock.AsyncMock()
+        mock_thread_cache = mock.AsyncMock()
+        mock_thread_cache.get.side_effect = side_effect
 
-        result = await tanjun.to_channel(222, mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+        result = await tanjun.to_channel(
+            222, mock_context, cache=mock_channel_cache, dm_cache=mock_dm_cache, thread_cache=mock_thread_cache
+        )
 
         assert result is mock_dm_cache.get.return_value
         mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_awaited_once_with(222)
+        mock_channel_cache.get.assert_awaited_once_with(222)
         mock_dm_cache.get.assert_awaited_once_with(222)
+        mock_thread_cache.get.assert_awaited_once_with(222)
 
     @pytest.mark.asyncio()
     async def test___call___when_not_cached_and_async_channel_caches_raise_not_found_and_not_including_dms(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache.get_guild_channel.return_value = None
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.EntryNotFound
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = tanjun.dependencies.EntryNotFound
         mock_dm_cache = mock.AsyncMock()
+        mock_thread_cache = mock.AsyncMock()
+        mock_thread_cache.get.side_effect = tanjun.dependencies.EntryNotFound
         converter = tanjun.conversion.ChannelConverter(include_dms=False)
 
         with pytest.raises(ValueError, match="Couldn't find channel"):
-            await converter("<#12222>", mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+            await converter(
+                "<#12222>",
+                mock_context,
+                cache=mock_channel_cache,
+                dm_cache=mock_dm_cache,
+                thread_cache=mock_thread_cache,
+            )
 
         mock_context.cache.get_guild_channel.assert_called_once_with(12222)
         mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_awaited_once_with(12222)
+        mock_channel_cache.get.assert_awaited_once_with(12222)
         mock_dm_cache.get.assert_not_called()
+        mock_thread_cache.get.assert_awaited_once_with(12222)
 
     @pytest.mark.asyncio()
-    async def test___call___when_not_cached_and_both_async_caches_raise_not_found(self):
+    async def test___call___when_not_cached_and_all_async_caches_raise_not_found(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache.get_guild_channel.return_value = None
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.EntryNotFound
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = tanjun.dependencies.EntryNotFound
         mock_dm_cache = mock.AsyncMock()
         mock_dm_cache.get.side_effect = tanjun.dependencies.EntryNotFound
+        mock_thread_cache = mock.AsyncMock()
+        mock_thread_cache.get.side_effect = tanjun.dependencies.EntryNotFound
 
         with pytest.raises(ValueError, match="Couldn't find channel"):
-            await tanjun.to_channel("<#12222>", mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+            await tanjun.to_channel(
+                "<#12222>",
+                mock_context,
+                cache=mock_channel_cache,
+                dm_cache=mock_dm_cache,
+                thread_cache=mock_thread_cache,
+            )
 
         mock_context.cache.get_guild_channel.assert_called_once_with(12222)
         mock_context.rest.fetch_channel.assert_not_called()
-        mock_cache.get.assert_awaited_once_with(12222)
+        mock_channel_cache.get.assert_awaited_once_with(12222)
         mock_dm_cache.get.assert_awaited_once_with(12222)
+        mock_thread_cache.get.assert_awaited_once_with(12222)
 
     @pytest.mark.asyncio()
-    async def test___call___when_not_cached_and_async_caches_both_raise_cache_miss_error(self):
+    async def test___call___when_not_cached_and_async_caches_all_raise_cache_miss_error(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache.get_guild_channel.return_value = None
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = tanjun.dependencies.CacheMissError
         mock_dm_cache = mock.AsyncMock()
         mock_dm_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_thread_cache = mock.AsyncMock()
+        mock_thread_cache.get.side_effect = tanjun.dependencies.CacheMissError
 
-        result = await tanjun.to_channel("<#12222>", mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+        result = await tanjun.to_channel(
+            "<#12222>", mock_context, cache=mock_channel_cache, dm_cache=mock_dm_cache, thread_cache=mock_thread_cache
+        )
 
         assert result is mock_context.rest.fetch_channel.return_value
         mock_context.cache.get_guild_channel.assert_called_once_with(12222)
         mock_context.rest.fetch_channel.assert_awaited_once_with(12222)
-        mock_cache.get.assert_awaited_once_with(12222)
+        mock_channel_cache.get.assert_awaited_once_with(12222)
         mock_dm_cache.get.assert_awaited_once_with(12222)
+        mock_thread_cache.get.assert_awaited_once_with(12222)
 
     @pytest.mark.asyncio()
     async def test___call___when_not_including_dms(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.rest.fetch_channel.return_value = mock.Mock(hikari.GuildChannel)
         mock_context.cache.get_guild_channel.return_value = None
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = tanjun.dependencies.CacheMissError
         mock_dm_cache = mock.AsyncMock()
+        mock_thread_cache = mock.AsyncMock()
+        mock_thread_cache.get.side_effect = tanjun.dependencies.CacheMissError
         converter = tanjun.conversion.ChannelConverter(include_dms=False)
 
-        result = await converter("<#12222>", mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+        result = await converter(
+            "<#12222>", mock_context, cache=mock_channel_cache, dm_cache=mock_dm_cache, thread_cache=mock_thread_cache
+        )
 
         assert result is mock_context.rest.fetch_channel.return_value
         mock_context.cache.get_guild_channel.assert_called_once_with(12222)
         mock_context.rest.fetch_channel.assert_awaited_once_with(12222)
-        mock_cache.get.assert_awaited_once_with(12222)
+        mock_channel_cache.get.assert_awaited_once_with(12222)
         mock_dm_cache.get.assert_not_called()
+        mock_thread_cache.get.assert_awaited_once_with(12222)
 
     @pytest.mark.asyncio()
     async def test___call___when_not_including_dms_and_rest_returns_dm_channel(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.rest.fetch_channel.return_value = mock.Mock(hikari.DMChannel)
         mock_context.cache.get_guild_channel.return_value = None
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = tanjun.dependencies.CacheMissError
         mock_dm_cache = mock.AsyncMock()
+        mock_thread_cache = mock.AsyncMock()
+        mock_thread_cache.get.side_effect = tanjun.dependencies.CacheMissError
         converter = tanjun.conversion.ChannelConverter(include_dms=False)
 
         with pytest.raises(ValueError, match="Couldn't find channel"):
-            await converter("<#12222>", mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+            await converter(
+                "<#12222>",
+                mock_context,
+                cache=mock_channel_cache,
+                dm_cache=mock_dm_cache,
+                thread_cache=mock_thread_cache,
+            )
 
         mock_context.cache.get_guild_channel.assert_called_once_with(12222)
         mock_context.rest.fetch_channel.assert_awaited_once_with(12222)
-        mock_cache.get.assert_awaited_once_with(12222)
+        mock_channel_cache.get.assert_awaited_once_with(12222)
         mock_dm_cache.get.assert_not_called()
+        mock_thread_cache.get.assert_awaited_once_with(12222)
 
     @pytest.mark.asyncio()
     async def test___call___when_not_found_and_not_including_dms(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache.get_guild_channel.return_value = None
         mock_context.rest.fetch_channel.side_effect = hikari.NotFoundError(url="gey", headers={}, raw_body="")
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = tanjun.dependencies.CacheMissError
         mock_dm_cache = mock.AsyncMock()
         mock_dm_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_thread_cache = mock.AsyncMock()
+        mock_thread_cache.get.side_effect = tanjun.dependencies.CacheMissError
         converter = tanjun.conversion.ChannelConverter(include_dms=False)
 
         with pytest.raises(ValueError, match="Couldn't find channel"):
-            await converter("<#12222>", mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+            await converter(
+                "<#12222>",
+                mock_context,
+                cache=mock_channel_cache,
+                dm_cache=mock_dm_cache,
+                thread_cache=mock_thread_cache,
+            )
 
         mock_context.cache.get_guild_channel.assert_called_once_with(12222)
         mock_context.rest.fetch_channel.assert_awaited_once_with(12222)
-        mock_cache.get.assert_awaited_once_with(12222)
+        mock_channel_cache.get.assert_awaited_once_with(12222)
         mock_dm_cache.get.assert_not_called()
+        mock_thread_cache.get.assert_awaited_once_with(12222)
 
     @pytest.mark.asyncio()
     async def test___call___when_not_found(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache.get_guild_channel.return_value = None
         mock_context.rest.fetch_channel.side_effect = hikari.NotFoundError(url="gey", headers={}, raw_body="")
-        mock_cache = mock.AsyncMock()
-        mock_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_channel_cache = mock.AsyncMock()
+        mock_channel_cache.get.side_effect = tanjun.dependencies.CacheMissError
         mock_dm_cache = mock.AsyncMock()
         mock_dm_cache.get.side_effect = tanjun.dependencies.CacheMissError
+        mock_thread_cache = mock.AsyncMock()
+        mock_thread_cache.get.side_effect = tanjun.dependencies.CacheMissError
 
         with pytest.raises(ValueError, match="Couldn't find channel"):
-            await tanjun.to_channel("<#12222>", mock_context, cache=mock_cache, dm_cache=mock_dm_cache)
+            await tanjun.to_channel(
+                "<#12222>",
+                mock_context,
+                cache=mock_channel_cache,
+                dm_cache=mock_dm_cache,
+                thread_cache=mock_thread_cache,
+            )
 
         mock_context.cache.get_guild_channel.assert_called_once_with(12222)
         mock_context.rest.fetch_channel.assert_awaited_once_with(12222)
-        mock_cache.get.assert_awaited_once_with(12222)
+        mock_channel_cache.get.assert_awaited_once_with(12222)
         mock_dm_cache.get.assert_awaited_once_with(12222)
+        mock_thread_cache.get.assert_awaited_once_with(12222)
 
 
 class TestEmojiConverter:
     @pytest.mark.asyncio()
     async def test___call___when_cached(self):
         mock_context = mock.Mock()
         mock_cache = mock.AsyncMock()
@@ -388,15 +515,18 @@
         mock_cache.get.assert_awaited_once_with(54123)
 
     @pytest.mark.asyncio()
     async def test___call___when_cacheless(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache = None
 
-        result = await tanjun.to_emoji("<a:name:7623421>", mock_context, cache=None)
+        result = await tanjun.to_emoji(
+            "<a:name:7623421>",
+            mock_context,
+        )
 
         assert result is mock_context.rest.fetch_emoji.return_value
         mock_context.rest.fetch_emoji.assert_awaited_once_with(mock_context.guild_id, 7623421)
 
     @pytest.mark.asyncio()
     async def test___call___when_rest_async_cache_not_found(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
@@ -482,15 +612,15 @@
         mock_cache.get.assert_awaited_once_with(54234)
 
     @pytest.mark.asyncio()
     async def test___call___when_cacheless(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache = None
 
-        result = await tanjun.to_guild(2222, mock_context, cache=None)
+        result = await tanjun.to_guild(2222, mock_context)
 
         assert result is mock_context.rest.fetch_guild.return_value
         mock_context.rest.fetch_guild.assert_awaited_once_with(2222)
 
     @pytest.mark.asyncio()
     async def test___call___when_async_not_found(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
@@ -562,15 +692,15 @@
         mock_cache.get.assert_awaited_once_with("fffff")
 
     @pytest.mark.asyncio()
     async def test___call___when_cacheless(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache = None
 
-        result = await tanjun.to_invite("123321", mock_context, cache=None)
+        result = await tanjun.to_invite("123321", mock_context)
 
         assert result is mock_context.rest.fetch_invite.return_value
         mock_context.rest.fetch_invite.assert_awaited_once_with("123321")
 
     @pytest.mark.asyncio()
     async def test___call___when_async_cache_not_found(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
@@ -624,15 +754,15 @@
         assert result is mock_cache.get.return_value
         mock_context.cache.get_invite.assert_called_once_with("asdbasd")
         mock_cache.get.assert_awaited_once_with("asdbasd")
 
     @pytest.mark.asyncio()
     async def test___call___when_not_str(self):
         with pytest.raises(ValueError, match="`432123` is not a valid invite code"):
-            await tanjun.to_invite_with_metadata(432123, mock.Mock(), cache=None)
+            await tanjun.to_invite_with_metadata(432123, mock.Mock())
 
     @pytest.mark.asyncio()
     async def test___call___when_not_cached(self):
         mock_context = mock.Mock()
         mock_context.cache.get_invite.return_value = None
         mock_cache = mock.AsyncMock()
         mock_cache.get.return_value = None
@@ -644,15 +774,15 @@
         mock_cache.get.assert_called_once_with("dsds")
 
     @pytest.mark.asyncio()
     async def test___call___when_cacheless(self):
         mock_context = mock.Mock(cache=None)
 
         with pytest.raises(ValueError, match="Couldn't find invite"):
-            await tanjun.to_invite_with_metadata("asdbasd", mock_context, cache=None)
+            await tanjun.to_invite_with_metadata("asdbasd", mock_context)
 
 
 class TestMemberConverter:
     @pytest.mark.asyncio()
     async def test___call___when_in_a_dm(self):
         mock_context = mock.Mock(guild_id=None)
         mock_cache = mock.AsyncMock()
@@ -750,15 +880,15 @@
         mock_cache.get_from_guild.assert_awaited_once_with(mock_context.guild_id, 5123123)
 
     @pytest.mark.asyncio()
     async def test___call___when_cacheless(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache = None
 
-        result = await tanjun.to_member("5123123", mock_context, cache=None)
+        result = await tanjun.to_member("5123123", mock_context)
 
         assert result is mock_context.rest.fetch_member.return_value
         mock_context.rest.fetch_member.assert_awaited_once_with(mock_context.guild_id, 5123123)
         mock_context.rest.search_members.assert_not_called()
 
     @pytest.mark.asyncio()
     async def test___call___when_mock_cache_raises_not_found(self):
@@ -778,15 +908,15 @@
     @pytest.mark.asyncio()
     async def test___call___when_rest_raises_not_found(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache.get_member.return_value = None
         mock_context.rest.fetch_member.side_effect = hikari.NotFoundError(url="grey", headers={}, raw_body="")
 
         with pytest.raises(ValueError, match="Couldn't find member in this guild"):
-            await tanjun.to_member("5123123", mock_context, cache=None)
+            await tanjun.to_member("5123123", mock_context)
 
         mock_context.cache.get_member.assert_called_once_with(mock_context.guild_id, 5123123)
         mock_context.rest.fetch_member.assert_awaited_once_with(mock_context.guild_id, 5123123)
         mock_context.rest.search_members.assert_not_called()
 
 
 class TestPresenceConverter:
@@ -849,15 +979,15 @@
 
     @pytest.mark.asyncio()
     async def test___call___when_cacheless(self):
         mock_context = mock.Mock()
         mock_context.cache = None
 
         with pytest.raises(ValueError, match="Couldn't find presence in current guild"):
-            await tanjun.to_presence("<@543123>", mock_context, cache=None)
+            await tanjun.to_presence("<@543123>", mock_context)
 
 
 class TestUserConverter:
     @pytest.mark.asyncio()
     async def test___call___when_cached(self):
         mock_context = mock.Mock()
         mock_cache = mock.AsyncMock()
@@ -897,15 +1027,15 @@
         mock_cache.get.assert_awaited_once_with(55)
 
     @pytest.mark.asyncio()
     async def test___call___when_cacheless(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache = None
 
-        result = await tanjun.to_user("12343", mock_context, cache=None)
+        result = await tanjun.to_user("12343", mock_context)
 
         assert result is mock_context.rest.fetch_user.return_value
         mock_context.rest.fetch_user.assert_awaited_once_with(12343)
 
     @pytest.mark.asyncio()
     async def test___call___when_not_found(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
@@ -977,15 +1107,15 @@
         mock_cache.get.assert_awaited_once_with(55)
 
     @pytest.mark.asyncio()
     async def test___call___when_cacheless(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
         mock_context.cache = None
 
-        result = await tanjun.to_message("@me/12/34", mock_context, cache=None)
+        result = await tanjun.to_message("@me/12/34", mock_context)
 
         assert result is mock_context.rest.fetch_message.return_value
         mock_context.rest.fetch_message.assert_awaited_once_with(12, 34)
 
     @pytest.mark.asyncio()
     async def test___call___when_not_found(self):
         mock_context = mock.Mock(rest=mock.AsyncMock())
@@ -1074,22 +1204,22 @@
         mock_cache.get_from_guild.assert_awaited_once_with(mock_context.guild_id, 65234, default=None)
 
     @pytest.mark.asyncio()
     async def test___call___when_cacheless_and_no_async_cache(self):
         mock_context = mock.Mock(cache=None)
 
         with pytest.raises(ValueError, match="Voice state couldn't be found for current guild"):
-            await tanjun.to_voice_state(65234, mock_context, cache=None)
+            await tanjun.to_voice_state(65234, mock_context)
 
     @pytest.mark.asyncio()
     async def test___call___when_in_a_dm(self):
         mock_context = mock.Mock(guild_id=None)
 
         with pytest.raises(ValueError, match="Cannot get a voice state from a DM channel"):
-            await tanjun.to_voice_state(65234, mock_context, cache=None)
+            await tanjun.to_voice_state(65234, mock_context)
 
 
 TOO_LARGE_SF = hikari.Snowflake.max() + 1
 TOO_SMALL_SF = hikari.Snowflake.min() - 50
 
 
 @pytest.mark.parametrize(
```

### Comparing `hikari-tanjun-2.8.1a1/tests/test_errors.py` & `hikari-tanjun-2.9.0a1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_hooks.py` & `hikari-tanjun-2.9.0a1/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_injecting.py` & `hikari-tanjun-2.9.0a1/tests/test_injecting.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_parsing.py` & `hikari-tanjun-2.9.0a1/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_permissions.py` & `hikari-tanjun-2.9.0a1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_schedules.py` & `hikari-tanjun-2.9.0a1/tests/test_schedules.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/tests/test_utilities.py` & `hikari-tanjun-2.9.0a1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hikari-tanjun-2.8.1a1/PKG-INFO` & `hikari-tanjun-2.9.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-tanjun
-Version: 2.8.1a1
+Version: 2.9.0a1
 Summary: A flexible command framework designed to extend Hikari.
 Keywords: hikari
 Author-email: Faster Speeding <lucina@lmbyrne.dev>
 Requires-Python: >=3.9.0,<3.12
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -18,19 +18,19 @@
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: alluka~=0.1.2
-Requires-Dist: hikari~=2.0.0.dev111
-Project-URL: changelog, https://github.com/FasterSpeeding/tanjun/blob/master/CHANGELOG.md
-Project-URL: documentation, https://tanjun.cursed.solutions/
-Project-URL: homepage, https://github.com/FasterSpeeding/Tanjun
-Project-URL: repository, https://github.com/FasterSpeeding/Tanjun
+Requires-Dist: hikari~=2.0.0.dev112
+Project-URL: Changelog, https://github.com/FasterSpeeding/tanjun/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://tanjun.cursed.solutions/
+Project-URL: Homepage, https://github.com/FasterSpeeding/Tanjun
+Project-URL: Repository, https://github.com/FasterSpeeding/Tanjun
 
 # Tanjun
 
 A flexible command framework designed to extend Hikari.
 
 # Installation
```

