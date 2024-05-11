# Comparing `tmp/pre_commit-3.7.0.tar.gz` & `tmp/pre_commit-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit-3.7.0.tar", last modified: Sun Mar 24 17:37:26 2024, max compression
+gzip compressed data, was "pre_commit-3.7.1.tar", last modified: Sat May 11 01:25:02 2024, max compression
```

## Comparing `pre_commit-3.7.0.tar` & `pre_commit-3.7.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-03-24 17:37:26.316048 pre_commit-3.7.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1092 2022-04-30 16:59:40.000000 pre_commit-3.7.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2024-03-24 17:37:26.316048 pre_commit-3.7.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      480 2022-12-31 16:55:07.000000 pre_commit-3.7.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-03-24 17:37:26.308048 pre_commit-3.7.0/pre_commit/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      127 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1422 2023-07-31 00:01:50.000000 pre_commit-3.7.0/pre_commit/all_languages.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12350 2023-12-09 21:19:28.000000 pre_commit-3.7.0/pre_commit/clientlib.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3219 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/color.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-03-24 17:37:26.308048 pre_commit-3.7.0/pre_commit/commands/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/commands/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7157 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/commands/autoupdate.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      429 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/commands/clean.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2804 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/commands/gc.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9400 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/commands/hook_impl.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1135 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/commands/init_templatedir.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5341 2023-07-31 00:01:50.000000 pre_commit-3.7.0/pre_commit/commands/install_uninstall.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2099 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/commands/migrate_config.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    14151 2024-03-24 17:32:04.000000 pre_commit-3.7.0/pre_commit/commands/run.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      453 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/commands/sample_config.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2578 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/commands/try_repo.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      371 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/commands/validate_config.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      377 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/commands/validate_manifest.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      282 2023-03-17 16:29:01.000000 pre_commit-3.7.0/pre_commit/constants.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1605 2023-10-28 18:17:11.000000 pre_commit-3.7.0/pre_commit/envcontext.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2633 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/error_handler.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/errors.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2378 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/file_lock.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8518 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/git.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1513 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/hook.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5250 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/lang_base.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-03-24 17:37:26.312048 pre_commit-3.7.0/pre_commit/languages/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/languages/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2433 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/conda.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2520 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/coursier.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3130 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/dart.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4840 2024-03-24 17:09:48.000000 pre_commit-3.7.0/pre_commit/languages/docker.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      847 2024-03-24 17:09:48.000000 pre_commit-3.7.0/pre_commit/languages/docker_image.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3487 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/dotnet.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      685 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/fail.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4599 2024-02-18 18:15:24.000000 pre_commit-3.7.0/pre_commit/languages/golang.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1674 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/haskell.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2547 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/lua.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3865 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/node.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1503 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/perl.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3816 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/pygrep.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6820 2023-12-09 21:19:28.000000 pre_commit-3.7.0/pre_commit/languages/python.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5551 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/r.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4648 2023-12-09 19:59:29.000000 pre_commit-3.7.0/pre_commit/languages/ruby.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5495 2023-12-09 21:19:28.000000 pre_commit-3.7.0/pre_commit/languages/rust.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      786 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/script.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1617 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/languages/swift.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      300 2023-02-21 15:20:22.000000 pre_commit-3.7.0/pre_commit/languages/system.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1031 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/logging_handler.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    15564 2024-02-10 18:46:57.000000 pre_commit-3.7.0/pre_commit/main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-03-24 17:37:26.312048 pre_commit-3.7.0/pre_commit/meta_hooks/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/meta_hooks/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1207 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/meta_hooks/check_hooks_apply.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2553 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/meta_hooks/check_useless_excludes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      346 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/meta_hooks/identity.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      911 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/output.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2481 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/parse_shebang.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      495 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/prefix.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7938 2023-12-09 21:19:28.000000 pre_commit-3.7.0/pre_commit/repository.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-03-24 17:37:26.316048 pre_commit-3.7.0/pre_commit/resources/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/resources/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)        2 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_.npmignore
--rw-r--r--   0 asottile  (1000) asottile  (1000)       96 2023-12-09 20:59:15.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_Cargo.toml
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1052 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_LICENSE.renv
--rw-r--r--   0 asottile  (1000) asottile  (1000)      104 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_Makefile.PL
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12037 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_activate.R
--rw-r--r--   0 asottile  (1000) asottile  (1000)      302 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_environment.yml
--rw-r--r--   0 asottile  (1000) asottile  (1000)       43 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_go.mod
--rw-r--r--   0 asottile  (1000) asottile  (1000)       29 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_main.go
--rw-r--r--   0 asottile  (1000) asottile  (1000)       13 2023-12-09 20:59:15.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_main.rs
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_package.json
--rw-r--r--   0 asottile  (1000) asottile  (1000)      212 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_pre-commit-package-dev-1.rockspec
--rw-r--r--   0 asottile  (1000) asottile  (1000)      195 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_pre_commit_placeholder_package.gemspec
--rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_pubspec.yaml
--rw-r--r--   0 asottile  (1000) asottile  (1000)      351 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_renv.lock
--rw-r--r--   0 asottile  (1000) asottile  (1000)       93 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/resources/empty_template_setup.py
--rwxr-xr-x   0 asottile  (1000) asottile  (1000)      528 2022-04-30 16:59:40.000000 pre_commit-3.7.0/pre_commit/resources/hook-tmpl
--rw-r--r--   0 asottile  (1000) asottile  (1000)    32551 2023-04-29 17:03:06.000000 pre_commit-3.7.0/pre_commit/resources/rbenv.tar.gz
--rw-r--r--   0 asottile  (1000) asottile  (1000)    75808 2023-04-29 17:07:26.000000 pre_commit-3.7.0/pre_commit/resources/ruby-build.tar.gz
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5271 2023-04-29 17:03:06.000000 pre_commit-3.7.0/pre_commit/resources/ruby-download.tar.gz
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4191 2024-02-10 19:42:29.000000 pre_commit-3.7.0/pre_commit/staged_files_only.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9275 2023-12-09 20:59:15.000000 pre_commit-3.7.0/pre_commit/store.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6991 2023-12-09 19:59:29.000000 pre_commit-3.7.0/pre_commit/util.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5557 2023-10-28 18:11:21.000000 pre_commit-3.7.0/pre_commit/xargs.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      499 2023-02-20 22:54:27.000000 pre_commit-3.7.0/pre_commit/yaml.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-03-24 17:37:26.308048 pre_commit-3.7.0/pre_commit.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2024-03-24 17:37:26.000000 pre_commit-3.7.0/pre_commit.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2979 2024-03-24 17:37:26.000000 pre_commit-3.7.0/pre_commit.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2024-03-24 17:37:26.000000 pre_commit-3.7.0/pre_commit.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       52 2024-03-24 17:37:26.000000 pre_commit-3.7.0/pre_commit.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       76 2024-03-24 17:37:26.000000 pre_commit-3.7.0/pre_commit.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       11 2024-03-24 17:37:26.000000 pre_commit-3.7.0/pre_commit.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1398 2024-03-24 17:37:26.316048 pre_commit-3.7.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-02-20 22:54:27.000000 pre_commit-3.7.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-05-11 01:25:02.509857 pre_commit-3.7.1/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1092 2022-04-30 16:59:40.000000 pre_commit-3.7.1/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2024-05-11 01:25:02.509857 pre_commit-3.7.1/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      480 2022-12-31 16:55:07.000000 pre_commit-3.7.1/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-05-11 01:25:02.489857 pre_commit-3.7.1/pre_commit/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      127 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1422 2023-07-31 00:01:50.000000 pre_commit-3.7.1/pre_commit/all_languages.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12350 2023-12-09 21:19:28.000000 pre_commit-3.7.1/pre_commit/clientlib.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3219 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/color.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-05-11 01:25:02.497857 pre_commit-3.7.1/pre_commit/commands/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/commands/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7157 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/commands/autoupdate.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      429 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/commands/clean.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2804 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/commands/gc.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9400 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/commands/hook_impl.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1135 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/commands/init_templatedir.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5341 2023-07-31 00:01:50.000000 pre_commit-3.7.1/pre_commit/commands/install_uninstall.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2099 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/commands/migrate_config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    14151 2024-03-24 17:32:04.000000 pre_commit-3.7.1/pre_commit/commands/run.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      453 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/commands/sample_config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2578 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/commands/try_repo.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      371 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/commands/validate_config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      377 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/commands/validate_manifest.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      282 2023-03-17 16:29:01.000000 pre_commit-3.7.1/pre_commit/constants.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1605 2023-10-28 18:17:11.000000 pre_commit-3.7.1/pre_commit/envcontext.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2633 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/error_handler.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/errors.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2378 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/file_lock.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8518 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/git.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1513 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/hook.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5250 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/lang_base.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-05-11 01:25:02.505857 pre_commit-3.7.1/pre_commit/languages/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/languages/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2433 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/conda.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2520 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/coursier.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3130 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/dart.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4840 2024-03-24 17:09:48.000000 pre_commit-3.7.1/pre_commit/languages/docker.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      847 2024-03-24 17:09:48.000000 pre_commit-3.7.1/pre_commit/languages/docker_image.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3487 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/dotnet.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      685 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/fail.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4599 2024-02-18 18:15:24.000000 pre_commit-3.7.1/pre_commit/languages/golang.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1674 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/haskell.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2547 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/lua.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3865 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/node.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1503 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/perl.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3816 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/pygrep.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6820 2023-12-09 21:19:28.000000 pre_commit-3.7.1/pre_commit/languages/python.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5551 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/r.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4648 2023-12-09 19:59:29.000000 pre_commit-3.7.1/pre_commit/languages/ruby.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5504 2024-05-11 01:21:56.000000 pre_commit-3.7.1/pre_commit/languages/rust.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      786 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/script.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1617 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/languages/swift.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      300 2023-02-21 15:20:22.000000 pre_commit-3.7.1/pre_commit/languages/system.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1031 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/logging_handler.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    15564 2024-02-10 18:46:57.000000 pre_commit-3.7.1/pre_commit/main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-05-11 01:25:02.505857 pre_commit-3.7.1/pre_commit/meta_hooks/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/meta_hooks/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1207 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/meta_hooks/check_hooks_apply.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2553 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/meta_hooks/check_useless_excludes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      346 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/meta_hooks/identity.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      911 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/output.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2481 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/parse_shebang.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      495 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/prefix.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7938 2023-12-09 21:19:28.000000 pre_commit-3.7.1/pre_commit/repository.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-05-11 01:25:02.509857 pre_commit-3.7.1/pre_commit/resources/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/resources/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        2 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_.npmignore
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       96 2023-12-09 20:59:15.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_Cargo.toml
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1052 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_LICENSE.renv
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      104 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_Makefile.PL
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12037 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_activate.R
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      302 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_environment.yml
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       43 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_go.mod
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       29 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_main.go
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       13 2023-12-09 20:59:15.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_main.rs
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_package.json
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      212 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_pre-commit-package-dev-1.rockspec
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      195 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_pre_commit_placeholder_package.gemspec
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_pubspec.yaml
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      351 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_renv.lock
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       93 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/resources/empty_template_setup.py
+-rwxr-xr-x   0 asottile  (1000) asottile  (1000)      528 2022-04-30 16:59:40.000000 pre_commit-3.7.1/pre_commit/resources/hook-tmpl
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    32551 2023-04-29 17:03:06.000000 pre_commit-3.7.1/pre_commit/resources/rbenv.tar.gz
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    75808 2023-04-29 17:07:26.000000 pre_commit-3.7.1/pre_commit/resources/ruby-build.tar.gz
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5271 2023-04-29 17:03:06.000000 pre_commit-3.7.1/pre_commit/resources/ruby-download.tar.gz
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4191 2024-02-10 19:42:29.000000 pre_commit-3.7.1/pre_commit/staged_files_only.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9275 2023-12-09 20:59:15.000000 pre_commit-3.7.1/pre_commit/store.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7038 2024-05-11 01:21:56.000000 pre_commit-3.7.1/pre_commit/util.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5557 2023-10-28 18:11:21.000000 pre_commit-3.7.1/pre_commit/xargs.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      499 2023-02-20 22:54:27.000000 pre_commit-3.7.1/pre_commit/yaml.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-05-11 01:25:02.489857 pre_commit-3.7.1/pre_commit.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2024-05-11 01:25:02.000000 pre_commit-3.7.1/pre_commit.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2979 2024-05-11 01:25:02.000000 pre_commit-3.7.1/pre_commit.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2024-05-11 01:25:02.000000 pre_commit-3.7.1/pre_commit.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       52 2024-05-11 01:25:02.000000 pre_commit-3.7.1/pre_commit.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       76 2024-05-11 01:25:02.000000 pre_commit-3.7.1/pre_commit.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       11 2024-05-11 01:25:02.000000 pre_commit-3.7.1/pre_commit.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1398 2024-05-11 01:25:02.509857 pre_commit-3.7.1/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-02-20 22:54:27.000000 pre_commit-3.7.1/setup.py
```

### Comparing `pre_commit-3.7.0/LICENSE` & `pre_commit-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/PKG-INFO` & `pre_commit-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre_commit
-Version: 3.7.0
+Version: 3.7.1
 Summary: A framework for managing and maintaining multi-language pre-commit hooks.
 Home-page: https://github.com/pre-commit/pre-commit
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pre_commit-3.7.0/pre_commit/all_languages.py` & `pre_commit-3.7.1/pre_commit/all_languages.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/clientlib.py` & `pre_commit-3.7.1/pre_commit/clientlib.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/color.py` & `pre_commit-3.7.1/pre_commit/color.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/commands/autoupdate.py` & `pre_commit-3.7.1/pre_commit/commands/autoupdate.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/commands/gc.py` & `pre_commit-3.7.1/pre_commit/commands/gc.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/commands/hook_impl.py` & `pre_commit-3.7.1/pre_commit/commands/hook_impl.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/commands/init_templatedir.py` & `pre_commit-3.7.1/pre_commit/commands/init_templatedir.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/commands/install_uninstall.py` & `pre_commit-3.7.1/pre_commit/commands/install_uninstall.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/commands/migrate_config.py` & `pre_commit-3.7.1/pre_commit/commands/migrate_config.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/commands/run.py` & `pre_commit-3.7.1/pre_commit/commands/run.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/commands/try_repo.py` & `pre_commit-3.7.1/pre_commit/commands/try_repo.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/envcontext.py` & `pre_commit-3.7.1/pre_commit/envcontext.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/error_handler.py` & `pre_commit-3.7.1/pre_commit/error_handler.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/file_lock.py` & `pre_commit-3.7.1/pre_commit/file_lock.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/git.py` & `pre_commit-3.7.1/pre_commit/git.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/hook.py` & `pre_commit-3.7.1/pre_commit/hook.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/lang_base.py` & `pre_commit-3.7.1/pre_commit/lang_base.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/conda.py` & `pre_commit-3.7.1/pre_commit/languages/conda.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/coursier.py` & `pre_commit-3.7.1/pre_commit/languages/coursier.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/dart.py` & `pre_commit-3.7.1/pre_commit/languages/dart.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/docker.py` & `pre_commit-3.7.1/pre_commit/languages/docker.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/docker_image.py` & `pre_commit-3.7.1/pre_commit/languages/docker_image.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/dotnet.py` & `pre_commit-3.7.1/pre_commit/languages/dotnet.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/fail.py` & `pre_commit-3.7.1/pre_commit/languages/fail.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/golang.py` & `pre_commit-3.7.1/pre_commit/languages/golang.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/haskell.py` & `pre_commit-3.7.1/pre_commit/languages/haskell.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/lua.py` & `pre_commit-3.7.1/pre_commit/languages/lua.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/node.py` & `pre_commit-3.7.1/pre_commit/languages/node.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/perl.py` & `pre_commit-3.7.1/pre_commit/languages/perl.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/pygrep.py` & `pre_commit-3.7.1/pre_commit/languages/pygrep.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/python.py` & `pre_commit-3.7.1/pre_commit/languages/python.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/r.py` & `pre_commit-3.7.1/pre_commit/languages/r.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/ruby.py` & `pre_commit-3.7.1/pre_commit/languages/ruby.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/rust.py` & `pre_commit-3.7.1/pre_commit/languages/rust.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 def get_default_version() -> str:
     # If rust is already installed, we can save a bunch of setup time by
     # using the installed version.
     #
     # Just detecting the executable does not suffice, because if rustup is
     # installed but no toolchain is available, then `cargo` exists but
     # cannot be used without installing a toolchain first.
-    if cmd_output_b('cargo', '--version', check=False)[0] == 0:
+    if cmd_output_b('cargo', '--version', check=False, cwd='/')[0] == 0:
         return 'system'
     else:
         return C.DEFAULT
 
 
 def _rust_toolchain(language_version: str) -> str:
     """Transform the language version into a rust toolchain version."""
```

### Comparing `pre_commit-3.7.0/pre_commit/languages/script.py` & `pre_commit-3.7.1/pre_commit/languages/script.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/languages/swift.py` & `pre_commit-3.7.1/pre_commit/languages/swift.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/logging_handler.py` & `pre_commit-3.7.1/pre_commit/logging_handler.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/main.py` & `pre_commit-3.7.1/pre_commit/main.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/meta_hooks/check_hooks_apply.py` & `pre_commit-3.7.1/pre_commit/meta_hooks/check_hooks_apply.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/meta_hooks/check_useless_excludes.py` & `pre_commit-3.7.1/pre_commit/meta_hooks/check_useless_excludes.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/output.py` & `pre_commit-3.7.1/pre_commit/output.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/parse_shebang.py` & `pre_commit-3.7.1/pre_commit/parse_shebang.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/repository.py` & `pre_commit-3.7.1/pre_commit/repository.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/resources/empty_template_LICENSE.renv` & `pre_commit-3.7.1/pre_commit/resources/empty_template_LICENSE.renv`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/resources/empty_template_activate.R` & `pre_commit-3.7.1/pre_commit/resources/empty_template_activate.R`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/resources/hook-tmpl` & `pre_commit-3.7.1/pre_commit/resources/hook-tmpl`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/resources/rbenv.tar.gz` & `pre_commit-3.7.1/pre_commit/resources/rbenv.tar.gz`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/resources/ruby-build.tar.gz` & `pre_commit-3.7.1/pre_commit/resources/ruby-build.tar.gz`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/resources/ruby-download.tar.gz` & `pre_commit-3.7.1/pre_commit/resources/ruby-download.tar.gz`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/staged_files_only.py` & `pre_commit-3.7.1/pre_commit/staged_files_only.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/store.py` & `pre_commit-3.7.1/pre_commit/store.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit/util.py` & `pre_commit-3.7.1/pre_commit/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,32 +201,33 @@
 else:  # pragma: no cover
     cmd_output_p = cmd_output_b
 
 
 def _handle_readonly(
         func: Callable[[str], object],
         path: str,
-        exc: OSError,
+        exc: Exception,
 ) -> None:
     if (
             func in (os.rmdir, os.remove, os.unlink) and
+            isinstance(exc, OSError) and
             exc.errno in {errno.EACCES, errno.EPERM}
     ):
         for p in (path, os.path.dirname(path)):
             os.chmod(p, os.stat(p).st_mode | stat.S_IWUSR)
         func(path)
     else:
         raise
 
 
 if sys.version_info < (3, 12):  # pragma: <3.12 cover
     def _handle_readonly_old(
         func: Callable[[str], object],
         path: str,
-        excinfo: tuple[type[OSError], OSError, TracebackType],
+        excinfo: tuple[type[Exception], Exception, TracebackType],
     ) -> None:
         return _handle_readonly(func, path, excinfo[1])
 
     def rmtree(path: str) -> None:
         shutil.rmtree(path, ignore_errors=False, onerror=_handle_readonly_old)
 else:  # pragma: >=3.12 cover
     def rmtree(path: str) -> None:
```

### Comparing `pre_commit-3.7.0/pre_commit/xargs.py` & `pre_commit-3.7.1/pre_commit/xargs.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/pre_commit.egg-info/PKG-INFO` & `pre_commit-3.7.1/pre_commit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre-commit
-Version: 3.7.0
+Version: 3.7.1
 Summary: A framework for managing and maintaining multi-language pre-commit hooks.
 Home-page: https://github.com/pre-commit/pre-commit
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pre_commit-3.7.0/pre_commit.egg-info/SOURCES.txt` & `pre_commit-3.7.1/pre_commit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pre_commit-3.7.0/setup.cfg` & `pre_commit-3.7.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pre_commit
-version = 3.7.0
+version = 3.7.1
 description = A framework for managing and maintaining multi-language pre-commit hooks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pre-commit/pre-commit
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

