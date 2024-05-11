# Comparing `tmp/pyke_build-0.1.0.tar.gz` & `tmp/pyke_build-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyke_build-0.1.0.tar", last modified: Sun Apr 28 23:08:04 2024, max compression
+gzip compressed data, was "pyke_build-0.2.0.tar", last modified: Sat May 11 01:15:04 2024, max compression
```

## Comparing `pyke_build-0.1.0.tar` & `pyke_build-0.2.0.tar`

### file list

```diff
@@ -1,127 +1,137 @@
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.494148 pyke_build-0.1.0/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     3090 2024-04-28 22:39:41.000000 pyke_build-0.1.0/.gitignore
--rw-r--r--   0 schrock   (1000) schrock   (1000)       28 2024-02-24 20:10:29.000000 pyke_build-0.1.0/.nvimrc
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     1071 2024-02-19 23:49:32.000000 pyke_build-0.1.0/LICENSE
--rw-r--r--   0 schrock   (1000) schrock   (1000)       76 2024-02-21 01:08:06.000000 pyke_build-0.1.0/MANIFEST.in
--rw-r--r--   0 schrock   (1000) schrock   (1000)    56578 2024-04-28 23:08:04.494148 pyke_build-0.1.0/PKG-INFO
--rw-rw-r--   0 schrock   (1000) schrock   (1000)    55745 2024-04-28 21:58:20.000000 pyke_build-0.1.0/README.md
--rw-r--r--   0 schrock   (1000) schrock   (1000)       28 2024-02-20 00:01:00.000000 pyke_build-0.1.0/compile_flags.txt
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.482148 pyke_build-0.1.0/demos/
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/custom_phase/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     3670 2024-04-17 22:20:01.000000 pyke_build-0.1.0/demos/custom_phase/custom.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/custom_phase/include/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       99 2024-03-22 00:09:45.000000 pyke_build-0.1.0/demos/custom_phase/include/abc.h
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      642 2024-04-17 19:41:06.000000 pyke_build-0.1.0/demos/custom_phase/make.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/custom_phase/src/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-03-21 22:29:05.000000 pyke_build-0.1.0/demos/custom_phase/src/a.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-03-21 22:29:05.000000 pyke_build-0.1.0/demos/custom_phase/src/b.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-03-21 22:49:03.000000 pyke_build-0.1.0/demos/custom_phase/src/c.c
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/custom_phase/src/gen/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-03-22 01:36:40.000000 pyke_build-0.1.0/demos/custom_phase/src/gen/d.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       46 2024-03-22 01:36:40.000000 pyke_build-0.1.0/demos/custom_phase/src/gen/e.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      106 2024-04-13 00:18:00.000000 pyke_build-0.1.0/demos/custom_phase/src/main.c
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/diamond_deps/
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/diamond_deps/include/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       99 2024-04-10 18:49:58.000000 pyke_build-0.1.0/demos/diamond_deps/include/abc.h
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      808 2024-04-17 19:41:06.000000 pyke_build-0.1.0/demos/diamond_deps/make.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/diamond_deps/src/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-04-10 18:49:58.000000 pyke_build-0.1.0/demos/diamond_deps/src/a.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-04-10 18:49:58.000000 pyke_build-0.1.0/demos/diamond_deps/src/b.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-04-10 18:49:58.000000 pyke_build-0.1.0/demos/diamond_deps/src/c.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-04-10 18:49:58.000000 pyke_build-0.1.0/demos/diamond_deps/src/d.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       46 2024-04-10 18:49:58.000000 pyke_build-0.1.0/demos/diamond_deps/src/e.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      106 2024-04-13 22:48:17.000000 pyke_build-0.1.0/demos/diamond_deps/src/main.c
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/multi_make/
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/multi_make/exp/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       47 2024-03-12 23:07:29.000000 pyke_build-0.1.0/demos/multi_make/exp/a.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       48 2024-03-12 23:07:29.000000 pyke_build-0.1.0/demos/multi_make/exp/b.c
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/multi_make/include/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      101 2024-03-12 23:07:29.000000 pyke_build-0.1.0/demos/multi_make/include/abc.h
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      671 2024-04-17 19:41:06.000000 pyke_build-0.1.0/demos/multi_make/simple_0.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      564 2024-04-17 19:41:06.000000 pyke_build-0.1.0/demos/multi_make/simple_1.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/multi_make/src/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-03-12 23:07:29.000000 pyke_build-0.1.0/demos/multi_make/src/a.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-03-12 23:07:29.000000 pyke_build-0.1.0/demos/multi_make/src/b.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-03-12 23:07:29.000000 pyke_build-0.1.0/demos/multi_make/src/c.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      108 2024-04-13 00:19:14.000000 pyke_build-0.1.0/demos/multi_make/src/main.c
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/multi_shared_objects/
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/demos/multi_shared_objects/include/
--rw-r--r--   0 schrock   (1000) schrock   (1000)       89 2024-04-11 20:49:07.000000 pyke_build-0.1.0/demos/multi_shared_objects/include/multi.h
--rw-r--r--   0 schrock   (1000) schrock   (1000)      699 2024-04-17 19:41:06.000000 pyke_build-0.1.0/demos/multi_shared_objects/make.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/demos/multi_shared_objects/src/
--rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.1.0/demos/multi_shared_objects/src/aaa.c
--rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.1.0/demos/multi_shared_objects/src/aas.c
--rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.1.0/demos/multi_shared_objects/src/asa.c
--rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.1.0/demos/multi_shared_objects/src/ass.c
--rw-r--r--   0 schrock   (1000) schrock   (1000)      151 2024-04-11 20:51:53.000000 pyke_build-0.1.0/demos/multi_shared_objects/src/main.c
--rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.1.0/demos/multi_shared_objects/src/saa.c
--rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.1.0/demos/multi_shared_objects/src/sas.c
--rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.1.0/demos/multi_shared_objects/src/ssa.c
--rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.1.0/demos/multi_shared_objects/src/sss.c
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/demos/simple_app/
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/demos/simple_app/include/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      101 2024-03-12 23:07:29.000000 pyke_build-0.1.0/demos/simple_app/include/abc.h
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      178 2024-04-17 19:41:06.000000 pyke_build-0.1.0/demos/simple_app/make.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/demos/simple_app/src/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-03-12 23:07:29.000000 pyke_build-0.1.0/demos/simple_app/src/a.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-03-12 23:07:29.000000 pyke_build-0.1.0/demos/simple_app/src/b.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-03-12 23:07:29.000000 pyke_build-0.1.0/demos/simple_app/src/c.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       94 2024-04-13 00:19:40.000000 pyke_build-0.1.0/demos/simple_app/src/main.c
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/demos/simple_lib/
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/demos/simple_lib/include/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      101 2024-03-27 16:52:36.000000 pyke_build-0.1.0/demos/simple_lib/include/abc.h
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      305 2024-04-17 19:41:06.000000 pyke_build-0.1.0/demos/simple_lib/make.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/demos/simple_lib/src/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-03-27 16:52:36.000000 pyke_build-0.1.0/demos/simple_lib/src/a.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-03-27 16:52:36.000000 pyke_build-0.1.0/demos/simple_lib/src/b.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-03-27 16:52:36.000000 pyke_build-0.1.0/demos/simple_lib/src/c.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       94 2024-04-13 00:19:53.000000 pyke_build-0.1.0/demos/simple_lib/src/main.c
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/demos/simple_so/
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/demos/simple_so/include/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      101 2024-04-10 18:49:58.000000 pyke_build-0.1.0/demos/simple_so/include/abc.h
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      374 2024-04-17 19:41:06.000000 pyke_build-0.1.0/demos/simple_so/make.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/demos/simple_so/src/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-04-10 18:49:58.000000 pyke_build-0.1.0/demos/simple_so/src/a.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-04-10 18:49:58.000000 pyke_build-0.1.0/demos/simple_so/src/b.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-04-10 18:49:58.000000 pyke_build-0.1.0/demos/simple_so/src/c.c
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       94 2024-04-13 00:20:06.000000 pyke_build-0.1.0/demos/simple_so/src/main.c
--rw-r--r--   0 schrock   (1000) schrock   (1000)     1102 2024-04-28 23:02:53.000000 pyke_build-0.1.0/pyproject.toml
--rw-r--r--   0 schrock   (1000) schrock   (1000)       65 2024-02-24 09:02:19.000000 pyke_build-0.1.0/pyrightconfig.json
--rw-r--r--   0 schrock   (1000) schrock   (1000)     1282 2024-04-17 05:09:15.000000 pyke_build-0.1.0/readme_helper.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       25 2024-02-22 18:33:58.000000 pyke_build-0.1.0/requierments.txt
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       38 2024-04-28 23:08:04.494148 pyke_build-0.1.0/setup.cfg
--rw-r--r--   0 schrock   (1000) schrock   (1000)       38 2024-02-25 02:40:53.000000 pyke_build-0.1.0/setup.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.486148 pyke_build-0.1.0/src/
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/src/pyke/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      707 2024-04-28 22:15:09.000000 pyke_build-0.1.0/src/pyke/__init__.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      411 2024-04-28 23:08:04.000000 pyke_build-0.1.0/src/pyke/_version.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     7529 2024-04-16 22:00:51.000000 pyke_build-0.1.0/src/pyke/action.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     1603 2024-04-18 18:40:09.000000 pyke_build-0.1.0/src/pyke/ansi.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)    10494 2024-04-19 20:39:48.000000 pyke_build-0.1.0/src/pyke/options.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)    15856 2024-04-15 21:56:08.000000 pyke_build-0.1.0/src/pyke/options_parser.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.490148 pyke_build-0.1.0/src/pyke/phases/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      539 2024-04-18 22:32:08.000000 pyke_build-0.1.0/src/pyke/phases/__init__.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     1746 2024-04-19 17:49:42.000000 pyke_build-0.1.0/src/pyke/phases/archive.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)    31451 2024-04-21 22:06:18.000000 pyke_build-0.1.0/src/pyke/phases/c_family_build.py
--rw-r--r--   0 schrock   (1000) schrock   (1000)     2867 2024-04-21 23:07:55.000000 pyke_build-0.1.0/src/pyke/phases/command_phase.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     2671 2024-04-19 01:38:09.000000 pyke_build-0.1.0/src/pyke/phases/compile.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     3915 2024-04-17 04:24:10.000000 pyke_build-0.1.0/src/pyke/phases/compile_and_archive.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     4137 2024-04-19 17:47:27.000000 pyke_build-0.1.0/src/pyke/phases/compile_and_link_to_exe.py
--rw-r--r--   0 schrock   (1000) schrock   (1000)     4295 2024-04-17 04:24:32.000000 pyke_build-0.1.0/src/pyke/phases/compile_and_link_to_so.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     2096 2024-04-22 19:22:28.000000 pyke_build-0.1.0/src/pyke/phases/link_to_exe.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     2896 2024-04-17 04:24:57.000000 pyke_build-0.1.0/src/pyke/phases/link_to_shared_object.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)    26622 2024-04-23 20:44:01.000000 pyke_build-0.1.0/src/pyke/phases/phase.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      390 2024-04-16 18:57:49.000000 pyke_build-0.1.0/src/pyke/phases/project.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)    18049 2024-04-28 22:14:15.000000 pyke_build-0.1.0/src/pyke/pyke.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)    10858 2024-04-21 22:50:52.000000 pyke_build-0.1.0/src/pyke/utilities.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.494148 pyke_build-0.1.0/src/pyke_build.egg-info/
--rw-r--r--   0 schrock   (1000) schrock   (1000)    56578 2024-04-28 23:08:04.000000 pyke_build-0.1.0/src/pyke_build.egg-info/PKG-INFO
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     2605 2024-04-28 23:08:04.000000 pyke_build-0.1.0/src/pyke_build.egg-info/SOURCES.txt
--rw-rw-r--   0 schrock   (1000) schrock   (1000)        1 2024-04-28 23:08:04.000000 pyke_build-0.1.0/src/pyke_build.egg-info/dependency_links.txt
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       40 2024-04-28 23:08:04.000000 pyke_build-0.1.0/src/pyke_build.egg-info/entry_points.txt
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       25 2024-04-28 23:08:04.000000 pyke_build-0.1.0/src/pyke_build.egg-info/requires.txt
--rw-rw-r--   0 schrock   (1000) schrock   (1000)        5 2024-04-28 23:08:04.000000 pyke_build-0.1.0/src/pyke_build.egg-info/top_level.txt
--rwxrwxr-x   0 schrock   (1000) schrock   (1000)      890 2024-04-18 19:49:50.000000 pyke_build-0.1.0/test.sh
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-28 23:08:04.494148 pyke_build-0.1.0/tests/
--rw-r--r--   0 schrock   (1000) schrock   (1000)    14791 2024-04-19 20:39:34.000000 pyke_build-0.1.0/tests/test_options.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)    35023 2024-04-19 20:15:33.000000 pyke_build-0.1.0/tests/test_options_parser.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.242777 pyke_build-0.2.0/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     3090 2024-04-28 22:39:41.000000 pyke_build-0.2.0/.gitignore
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       28 2024-02-24 20:10:29.000000 pyke_build-0.2.0/.nvimrc
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     1071 2024-02-19 23:49:32.000000 pyke_build-0.2.0/LICENSE
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       76 2024-02-21 01:08:06.000000 pyke_build-0.2.0/MANIFEST.in
+-rw-r--r--   0 schrock   (1000) schrock   (1000)    58742 2024-05-11 01:15:04.242777 pyke_build-0.2.0/PKG-INFO
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)    57909 2024-05-11 01:07:39.000000 pyke_build-0.2.0/README.md
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       28 2024-02-20 00:01:00.000000 pyke_build-0.2.0/compile_flags.txt
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.234777 pyke_build-0.2.0/demos/
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.234777 pyke_build-0.2.0/demos/custom_phase/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     3670 2024-04-17 22:20:01.000000 pyke_build-0.2.0/demos/custom_phase/custom.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.234777 pyke_build-0.2.0/demos/custom_phase/include/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       99 2024-03-22 00:09:45.000000 pyke_build-0.2.0/demos/custom_phase/include/abc.h
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      642 2024-04-17 19:41:06.000000 pyke_build-0.2.0/demos/custom_phase/make.py
+-rw-r--r--   0 schrock   (1000) schrock   (1000)      125 2024-05-09 22:29:07.000000 pyke_build-0.2.0/demos/custom_phase/pyke-config.json
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       50 2024-05-09 22:28:30.000000 pyke_build-0.2.0/demos/custom_phase/pyke-subconfig.json
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.234777 pyke_build-0.2.0/demos/custom_phase/src/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-03-21 22:29:05.000000 pyke_build-0.2.0/demos/custom_phase/src/a.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-03-21 22:29:05.000000 pyke_build-0.2.0/demos/custom_phase/src/b.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-03-21 22:49:03.000000 pyke_build-0.2.0/demos/custom_phase/src/c.c
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.234777 pyke_build-0.2.0/demos/custom_phase/src/gen/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-03-22 01:36:40.000000 pyke_build-0.2.0/demos/custom_phase/src/gen/d.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       46 2024-03-22 01:36:40.000000 pyke_build-0.2.0/demos/custom_phase/src/gen/e.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      106 2024-04-13 00:18:00.000000 pyke_build-0.2.0/demos/custom_phase/src/main.c
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.234777 pyke_build-0.2.0/demos/diamond_deps/
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.234777 pyke_build-0.2.0/demos/diamond_deps/include/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       99 2024-04-10 18:49:58.000000 pyke_build-0.2.0/demos/diamond_deps/include/abc.h
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      808 2024-04-17 19:41:06.000000 pyke_build-0.2.0/demos/diamond_deps/make.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/diamond_deps/src/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-04-10 18:49:58.000000 pyke_build-0.2.0/demos/diamond_deps/src/a.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-04-10 18:49:58.000000 pyke_build-0.2.0/demos/diamond_deps/src/b.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-04-10 18:49:58.000000 pyke_build-0.2.0/demos/diamond_deps/src/c.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-04-10 18:49:58.000000 pyke_build-0.2.0/demos/diamond_deps/src/d.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       46 2024-04-10 18:49:58.000000 pyke_build-0.2.0/demos/diamond_deps/src/e.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      106 2024-04-13 22:48:17.000000 pyke_build-0.2.0/demos/diamond_deps/src/main.c
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/multi_make/
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/multi_make/exp/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       47 2024-03-12 23:07:29.000000 pyke_build-0.2.0/demos/multi_make/exp/a.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       48 2024-03-12 23:07:29.000000 pyke_build-0.2.0/demos/multi_make/exp/b.c
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/multi_make/include/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      101 2024-03-12 23:07:29.000000 pyke_build-0.2.0/demos/multi_make/include/abc.h
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      671 2024-04-17 19:41:06.000000 pyke_build-0.2.0/demos/multi_make/simple_0.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      564 2024-04-17 19:41:06.000000 pyke_build-0.2.0/demos/multi_make/simple_1.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/multi_make/src/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-03-12 23:07:29.000000 pyke_build-0.2.0/demos/multi_make/src/a.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-03-12 23:07:29.000000 pyke_build-0.2.0/demos/multi_make/src/b.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-03-12 23:07:29.000000 pyke_build-0.2.0/demos/multi_make/src/c.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      108 2024-04-13 00:19:14.000000 pyke_build-0.2.0/demos/multi_make/src/main.c
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/multi_shared_objects/
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/multi_shared_objects/a-star/
+-rw-r--r--   0 schrock   (1000) schrock   (1000)      330 2024-05-09 23:09:44.000000 pyke_build-0.2.0/demos/multi_shared_objects/a-star/make.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/multi_shared_objects/a-star/src/
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.2.0/demos/multi_shared_objects/a-star/src/aaa.c
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.2.0/demos/multi_shared_objects/a-star/src/aas.c
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.2.0/demos/multi_shared_objects/a-star/src/asa.c
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.2.0/demos/multi_shared_objects/a-star/src/ass.c
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/multi_shared_objects/include/
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       89 2024-04-11 20:49:07.000000 pyke_build-0.2.0/demos/multi_shared_objects/include/multi.h
+-rw-r--r--   0 schrock   (1000) schrock   (1000)      433 2024-05-10 19:17:55.000000 pyke_build-0.2.0/demos/multi_shared_objects/make.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/multi_shared_objects/s-star/
+-rw-r--r--   0 schrock   (1000) schrock   (1000)      341 2024-05-09 23:01:46.000000 pyke_build-0.2.0/demos/multi_shared_objects/s-star/make.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/multi_shared_objects/s-star/src/
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.2.0/demos/multi_shared_objects/s-star/src/saa.c
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.2.0/demos/multi_shared_objects/s-star/src/sas.c
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.2.0/demos/multi_shared_objects/s-star/src/ssa.c
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       49 2024-04-11 20:47:02.000000 pyke_build-0.2.0/demos/multi_shared_objects/s-star/src/sss.c
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/multi_shared_objects/src/
+-rw-r--r--   0 schrock   (1000) schrock   (1000)      151 2024-04-11 20:51:53.000000 pyke_build-0.2.0/demos/multi_shared_objects/src/main.c
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/simple_app/
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/simple_app/include/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      101 2024-03-12 23:07:29.000000 pyke_build-0.2.0/demos/simple_app/include/abc.h
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      178 2024-04-17 19:41:06.000000 pyke_build-0.2.0/demos/simple_app/make.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/simple_app/src/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-03-12 23:07:29.000000 pyke_build-0.2.0/demos/simple_app/src/a.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-03-12 23:07:29.000000 pyke_build-0.2.0/demos/simple_app/src/b.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-03-12 23:07:29.000000 pyke_build-0.2.0/demos/simple_app/src/c.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       94 2024-04-13 00:19:40.000000 pyke_build-0.2.0/demos/simple_app/src/main.c
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/simple_lib/
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/simple_lib/include/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      101 2024-03-27 16:52:36.000000 pyke_build-0.2.0/demos/simple_lib/include/abc.h
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      305 2024-04-17 19:41:06.000000 pyke_build-0.2.0/demos/simple_lib/make.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/simple_lib/src/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-03-27 16:52:36.000000 pyke_build-0.2.0/demos/simple_lib/src/a.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-03-27 16:52:36.000000 pyke_build-0.2.0/demos/simple_lib/src/b.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-03-27 16:52:36.000000 pyke_build-0.2.0/demos/simple_lib/src/c.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       94 2024-04-13 00:19:53.000000 pyke_build-0.2.0/demos/simple_lib/src/main.c
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/simple_so/
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/simple_so/include/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      101 2024-04-10 18:49:58.000000 pyke_build-0.2.0/demos/simple_so/include/abc.h
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      374 2024-04-17 19:41:06.000000 pyke_build-0.2.0/demos/simple_so/make.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.238777 pyke_build-0.2.0/demos/simple_so/src/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       42 2024-04-10 18:49:58.000000 pyke_build-0.2.0/demos/simple_so/src/a.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       44 2024-04-10 18:49:58.000000 pyke_build-0.2.0/demos/simple_so/src/b.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       45 2024-04-10 18:49:58.000000 pyke_build-0.2.0/demos/simple_so/src/c.c
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       94 2024-04-13 00:20:06.000000 pyke_build-0.2.0/demos/simple_so/src/main.c
+-rw-r--r--   0 schrock   (1000) schrock   (1000)     1102 2024-04-28 23:02:53.000000 pyke_build-0.2.0/pyproject.toml
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       65 2024-02-24 09:02:19.000000 pyke_build-0.2.0/pyrightconfig.json
+-rw-r--r--   0 schrock   (1000) schrock   (1000)     1282 2024-04-17 05:09:15.000000 pyke_build-0.2.0/readme_helper.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       25 2024-02-22 18:33:58.000000 pyke_build-0.2.0/requierments.txt
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       38 2024-05-11 01:15:04.242777 pyke_build-0.2.0/setup.cfg
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       38 2024-02-25 02:40:53.000000 pyke_build-0.2.0/setup.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.234777 pyke_build-0.2.0/src/
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.242777 pyke_build-0.2.0/src/pyke/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      721 2024-05-09 18:46:22.000000 pyke_build-0.2.0/src/pyke/__init__.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      411 2024-05-11 01:15:04.000000 pyke_build-0.2.0/src/pyke/_version.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     7529 2024-04-16 22:00:51.000000 pyke_build-0.2.0/src/pyke/action.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     1603 2024-04-18 18:40:09.000000 pyke_build-0.2.0/src/pyke/ansi.py
+-rw-r--r--   0 schrock   (1000) schrock   (1000)     5372 2024-05-09 22:31:06.000000 pyke_build-0.2.0/src/pyke/config.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)    10494 2024-04-19 20:39:48.000000 pyke_build-0.2.0/src/pyke/options.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)    16384 2024-05-07 22:16:05.000000 pyke_build-0.2.0/src/pyke/options_parser.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.242777 pyke_build-0.2.0/src/pyke/phases/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      539 2024-04-18 22:32:08.000000 pyke_build-0.2.0/src/pyke/phases/__init__.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     1746 2024-04-19 17:49:42.000000 pyke_build-0.2.0/src/pyke/phases/archive.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)    31416 2024-05-07 23:41:21.000000 pyke_build-0.2.0/src/pyke/phases/c_family_build.py
+-rw-r--r--   0 schrock   (1000) schrock   (1000)     2867 2024-04-21 23:07:55.000000 pyke_build-0.2.0/src/pyke/phases/command_phase.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     2671 2024-04-19 01:38:09.000000 pyke_build-0.2.0/src/pyke/phases/compile.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     3915 2024-04-17 04:24:10.000000 pyke_build-0.2.0/src/pyke/phases/compile_and_archive.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     4137 2024-04-19 17:47:27.000000 pyke_build-0.2.0/src/pyke/phases/compile_and_link_to_exe.py
+-rw-r--r--   0 schrock   (1000) schrock   (1000)     4289 2024-05-10 00:34:07.000000 pyke_build-0.2.0/src/pyke/phases/compile_and_link_to_so.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     2096 2024-04-22 19:22:28.000000 pyke_build-0.2.0/src/pyke/phases/link_to_exe.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     2890 2024-05-10 00:34:07.000000 pyke_build-0.2.0/src/pyke/phases/link_to_shared_object.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)    26332 2024-05-10 00:40:42.000000 pyke_build-0.2.0/src/pyke/phases/phase.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      390 2024-04-16 18:57:49.000000 pyke_build-0.2.0/src/pyke/phases/project.py
+-rw-r--r--   0 schrock   (1000) schrock   (1000)     1536 2024-05-09 21:39:33.000000 pyke_build-0.2.0/src/pyke/pyke-config.json
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)    15343 2024-05-10 00:34:07.000000 pyke_build-0.2.0/src/pyke/pyke.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)    11052 2024-05-10 00:44:49.000000 pyke_build-0.2.0/src/pyke/utilities.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.242777 pyke_build-0.2.0/src/pyke_build.egg-info/
+-rw-r--r--   0 schrock   (1000) schrock   (1000)    58742 2024-05-11 01:15:04.000000 pyke_build-0.2.0/src/pyke_build.egg-info/PKG-INFO
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     2865 2024-05-11 01:15:04.000000 pyke_build-0.2.0/src/pyke_build.egg-info/SOURCES.txt
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)        1 2024-05-11 01:15:04.000000 pyke_build-0.2.0/src/pyke_build.egg-info/dependency_links.txt
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       40 2024-05-11 01:15:04.000000 pyke_build-0.2.0/src/pyke_build.egg-info/entry_points.txt
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       25 2024-05-11 01:15:04.000000 pyke_build-0.2.0/src/pyke_build.egg-info/requires.txt
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)        5 2024-05-11 01:15:04.000000 pyke_build-0.2.0/src/pyke_build.egg-info/top_level.txt
+-rwxrwxr-x   0 schrock   (1000) schrock   (1000)      890 2024-04-18 19:49:50.000000 pyke_build-0.2.0/test.sh
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-11 01:15:04.242777 pyke_build-0.2.0/tests/
+-rw-r--r--   0 schrock   (1000) schrock   (1000)    14791 2024-04-19 20:39:34.000000 pyke_build-0.2.0/tests/test_options.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)    35023 2024-04-19 20:15:33.000000 pyke_build-0.2.0/tests/test_options_parser.py
```

### Comparing `pyke_build-0.1.0/.gitignore` & `pyke_build-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/LICENSE` & `pyke_build-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/PKG-INFO` & `pyke_build-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyke-build
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python-based build system for automating build and deployment tasks.
 Author-email: Trevor Schrock <spacemeat@gmail.com>
 Maintainer-email: Trevor Schrock <spacemeat@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/spacemeat/pyke.git
 Keywords: C,C++,build
 Classifier: Development Status :: 3 - Alpha
@@ -38,34 +38,36 @@
 Usually, a declarative syntax is desireable for systems like this. But even CMake is a sort of language, and pyke files are too--just, in python. Very basic python is all you need to know to use it fully, and when you need that convenience of a full language, it's very nice to have. Sane defaults and a simple object structure help keep things fairly minimal for a basic project.
 
 - **Extensibility**
 Pyke comes with some basic classes (called `Phase`s) which can manage basic tasks. But you may have special needs in your project tha require a specific tool to be run, or files to be moved around, or secret keys to be managed, etc. If it's not in the basic set of classes, build your own. It's a reasonable interface to design new functionality for.
 
 ## Installing pyke
 
-Pyke is very nearly ready for its first submission to PyPI. Until then, clone this repo and install locally:
-
-```
-$ git clone git@github.com:spacemeat/pyke
-$ cd pyke
-$ pip install .
-```
-<!--
 Couldn't be easier. You need to be running python3.10 at least, and have pip installed. To install it globally:
 
 ```
-$ pip install pyke
+$ python3 -m pip install pyke-build
 ```
+
 or,
+
 ```
-$ pip install --user pyke
+$ python3 -m pip install --user pyke-build
 ```
--->
+
 You can optionally put it in a virtual environment, which may be the better idea.
 
+Alternatively, you can clone this repo and install locally:
+
+```
+$ git clone https://github.com/spacemeat/pyke
+$ cd pyke
+$ python3 -m pip install .
+```
+
 ## Using pyke
 
 We'll do a simple example. We have a C project laid out like this:
 
 ```
 simple_app
 ├── include
@@ -219,15 +221,15 @@
 * They cannot be cyclical. The dependency graph must not contain loops, though diamond relationships are fine.
 * Option overrides and actions that are specified to multiple phases in a dependency tree happen in reverse depth-first order. The deepest dependency phases act first; this way, dependencies that build objects will happen before those that depend on them to build libraries, etc. When setting actions and overrides from the command line, the default is to set them to all phases, so whole dependency graphs can be levered at once.
 
 If your project has multiple steps to build static libraries or shared objects (dynamic libraries) which are then used by other binaries in the build, you can make them dependencies of the built binary phases that use them. The appropriate directories and file references will automatically be resolved. Further, depnding on the properties of the project, appropriate dynamic lookup options will be inserted as well (like `-rpath` options for UNIX-like systems).
 
 ## Actions
 
-Pyke is not just good for building. There are other standard actions it can perform, with more forthcoming. Actually, it's more correct to say that `Phase` objects perform actions. Any string passed as an action on the command line will be applied as an action to the appropriate phases which implement the action. If no phase supports the action, it is quietly ignored.
+Pyke is not just good for building. There are other standard actions it can perform, with more forthcoming. Actually, it's more correct to say that `Phase` objects perform actions. Any string passed as an action on the command line will be applied to the appropriate phases which implement the action. If no phase supports the action, it is quietly ignored.
 
 There is a default action (`report_actions`) which displays the available actions in each phase of a project. This default can be overridden in a config file, either in a project or under $HOME (see [configuring pyke](#configuring-pyke)), to make the default action something different.
 
 ### Built-in actions
 
 Currently, the supported actions in each built-in phase are:
 
@@ -459,19 +461,19 @@
 You can also explicitly override after phase creation:
 
 ```python
 from pyke import CompileAndLinkToExePhase, Op, get_main_phase
 
 phase = CompileAndLinkToExePhase('simple_experiemtal', {
     'sources': ['a.cpp', 'b.cpp', 'c.cpp', 'main.cpp'],
-    'include_dirs': Op('+=', 'include/exp')        # appending to include_dirs
+    'include_dirs': Op('+=', 'include/exp')                 # appending to include_dirs
 })
 
-phase.push_opts({                                           # appending to sources
-    'sources': Op('*=', [f'exp/{src}' for src in [
+phase.push_opts({
+    'sources': Op('*=', [f'exp/{src}' for src in [          # extending sources
              'try_this.cpp', 'maybe.cpp', 'what_if.cpp']])
 })
 
 get_main_phase().depend_on(phase)
 ```
 
 Note the use of the `Op` class, which signals that the override is an operational modifier, not merely a replacement. The operator is expressed as a string. Overriding with a value directly instead of with `Op` implies a replacement ('=').
@@ -489,23 +491,25 @@
 As seen previously, overrides can be specified on the command line as well with `-o [phases:][option[op value]`. This can look similar to overrides in code (though you may need to enquote it):
 
 ```
 $ pyke -ocolors=none build
 $ pyke -o "compile:sources *= [exp/try_this.c, exp/maybe.c, exp/what_if.c]" opts
 ```
 
-String values can be in quotes if they need to be disambiguated from punctuation. The usual escapements work with '\'. Overrides you specify with `[]` are treated as lists, `()` as tuples, `{}` as sets, and `{:}` as dicts. Since option keys must only contain letters, numbers, and underscores, you can differentiate a single-valued set from an interpolation by inserting a comma, or specifically enquoting the string:
+String values can be in quotes if they need to be disambiguated from punctuation or shell interpolation. The usual escapements work with '\\'. Overrides you specify with `[]` are treated as lists, `()` as tuples, `{}` as sets, and `{:}` as dicts. Since option keys must only contain letters, numbers, and underscores, you can differentiate a single-valued set from an interpolation by inserting a comma, or specifically enquoting the string:
 
 ```
 $ pyke -o "my_set_of_one={foo,}" ...
 $ pyke -o "my_set_of_one={'foo'}" ...
 ```
 
 Python's built-in literals True, False, and None are defined as options, and can be interpolated as {true}, {false}, and {none}.
 
+Much like older-style subshell invocation, you can enquote a shell command in \`backtick\`s, and the command will be executed, with its output inserted in place. This is most useful in config files, since they're not executed in a shell context.
+
 There is more to say about how value overrides are parsed. Smartly using quotes, commas, or spaces to differentiate strings from interpolators will usually get you where you want. Generally, though, setting options in the makefile will probably be preferred.
 
 ### Base pyke options
 
 There are a few options that are uiversal to pyke, regardless of the type of project it is running. Here are the options you can set to adjust its behavior:
 
 |option|default|usage
@@ -637,29 +641,61 @@
 exe_anchor = {build_detail_anchor}/{exe_dir}
 exe_path = {exe_anchor}/{exe_file}
 ```
 You are encouraged to change `exe_dir` to set a base directory for executable files, and `exe_basename` to set the name of the executable. Pyke will only reference `exe_path` directly.
 
 Similar options are defined for static archives and shared objects. Of course, you can change any of these, or make your own constructed paths.
 
+### Recursive makefiles
+
+You can run another makefile within a makefile:
+
+```python
+# shaper/libs/make.py:
+import pyke as p
+shape_lib = p.CompileAndLinkToArchive()
+s = shape_lib.clone({'name': 'sphere',      'sources': ['shapes/sphere.cpp']})
+c = shape_lib.clone({'name': 'cube',        'sources': ['shapes/cube.cpp']})
+i = shape_lib.clone({'name': 'icosohedron', 'sources': ['shapes/icosohedron.cpp']})
+p.get_main_phase().depend_on([s, c, i])
+```
+```python
+# shaper/exe/make.py:
+import pyke as p
+
+base = p.run_makefile('../libs')   # tries to load '../libs/make.py'
+libs = [base.find_dep(lib) for lib in ('sphere', 'cube', 'icosohedron')]
+exe = p.CompileAndLinkToExePhase({'sources': ['main.c']}, libs)
+p.get_main_phase().depend_on(exe)
+```
+
+Here, the makefile `../libs/make.py` is run. Its ProjectPhase is returned as `base`, and the phases it loaded can be found in its dependency tree. The `project_anchor` and `gen_anchor` options are preserved for each makefile, though you can change them manually. Each makefile will also load its cohabiting `pyke-config.json` file as well, unless you suppress it with a parameter:
+
+```python
+...
+base = p.run_makefile('../libs', False)  # does not load libs/pyke-config.py, even if it exists.
+...
+```
+
 ## The CLI
 
 The general form of a pyke command is:
 
 ```
 pyke [-v | -h | [-c]? [-m makefile]? ]? [[-p [phase[,phase]*]]* | [-o [phase[,phase]*:]key[op_value]]* | [phase[,phase]*:][action]* ]*
 ```
 
 Notably, -o and action arguments are processed in command-line order. You can set the phases to use with each, setting some option overrides, performing actions, setting different options, perform more actions, etc. If no phases are specified, the overrides and actions apply to all phases, in reverse depth-first dependency order.
 
 The command line arguments are:
 * `-v`, `--version`: Prints the version information for pyke, and exits.
 * `-h`, `--help`: Prints a help document.
-* `-c`, `--cache_makefile`: Allows the makefile's __cache__ to be generated. This might speed up complex builds, but they'd hvae to be really complex. Must precede any arguments that are not -v, -h, or -m.
-* `-m`, `--module`: Specifies the module (pyke file), or its directory if the pyke file is called 'make.py', to be run. Must precede any arguments that are not -v, -h, or -c. If no -m argument is given, pyke will look for and run ./make.py.
+* `-m`, `--makefile`: Specifies the module (pyke file), or its directory if the pyke file is called 'make.py', to be run. Must precede any arguments that are not -v, -h, or -c. If no -m argument is given, pyke will look for and run ./make.py.
+* `-n`, `--noconfig`: Specifies that the `pyke-config.json` file adjacent to the makefile should not be loaded.
+* `-c`, `--report-config`: Prints the full combined configuration from all loaded config files, and exits.
 * `-p`, `--phases`: Specifies a subset of phases on which to apply subsequent overrides or actions, if such arguments do not provide their own. Each `-p` encountered resets the subgroup. Option and action arguments that provide their own phases overrule `-p` for that argument, but do not reset it.
 * `-o`, `--override`: Specifies an option override to apply to some or all phases for subsequenet actions. If the option is given as a key-op-value, the override is pushed; if it is only a key (with no operator-value pair) the override is popped.
 * `action`: Arguments given without switches specify actions to be taken on the indicated phases. Any action on any phase which doesn't support it is quietly ignored.
 
 ### Referencing phases
 
 Phases have names (`short name`s), as seen, but also have `full name`s, given as "group.name". For each phase, if the group name is not explicitly set, it is overridden *after the makefile is run* to be the short name of the closest dependency *project phase*. Project phases are thereafter given the short name `project`. This naming scheme allows for subprojects to be referenced by the group name on the CLI. We'll see some examples.
@@ -731,14 +767,15 @@
 * ~/.config/pyke/pyke-config.json
 * <makefile's directory>/pyke-config.json
 
 An example config might look like this:
 
 ```json
 {
+    "include": ["../pyke-config.json"],
     "argument_aliases": {
         "-noc": "-ocolors=none",
         "-bdb": "dbadmin:build",
         "-rdb": [
             "-odbadmin:run_args=\"-logging=TRUE -username=$DBADMIN_UNAME -password=$DBADMIN_PASSWD\"",
             "dbadmin:run"
         ]
@@ -746,20 +783,25 @@
     "action_aliases": {
         "pf": "package_flatpak",
         "vac": "verify_appchecker"
     },
     "default_action": "build",
     "default_arguments": [
         "-v2"
-    ]
+    ],
+    "cache_makefile_module": "true"
 }
 ```
 
 Each can contain the following sections:
 
+### Include files
+
+These are paths to other JSON files which contribute to the configuration. They are loaded before the rest of this file's contents, which can add to or override as described below. Useful if you have distinct configuration for work projects vs. personal projects, or lots of pyke projects which all use the same options. Paths that start with '/' are absolute; otherwise, they are relative to this file's path.
+
 ### Argument aliases
 
 These are convenient shorthands for complex overrides, override-action pairs, or whatever you like. Their values cannot contain other argument alias names, but *can* contain action aliases, and are otherwise exactly as you'd type them on the CLI (except you don't need to enquote things that the shell might interpret). Multiple values must be housed in a list. Each config file adds to the list of argument aliases.
 
 ### Action aliases
 
 Actions can be aliased. These are one-for-one word replacements, and the action values must not be other action aliases, though you *can* have more than one alias for any given action. Each config file adds to the list of action aliases.
@@ -768,14 +810,18 @@
 
 The default action is taken when no action is specified on a CLI. By default, this is set to `report_actions`. The value must not be an alias. Each config file overrides a set default action.
 
 ### Default arguments
 
 Ccontains a list of strings, each of which is a separate command line argument. These can be full names or aliases. They are placed consecutively directly after the -m argument, but before any -o or action arguments, on every invocation of pyke. It is a convenient way to customize the way pyke always works on your project or machine. Each config file appends to the list of default arguments.
 
+### Cache makefile module
+
+Allows the makefile's __cache__ to be generated by python. This might speed up complex builds, but they'd hvae to be really complex.
+
 ## Advanced Topics
 
 ### Adding new phases
 
 Of course, a benefit of a programmatic build system is extension. Building your own Phase classes shold be straightforward. You likely won't have to often.
 
 Say you need a code generator. It must make .c files your project compiles and links with extant source. You can write a custom Phase-derived class to do just this. This gets you into the weeds of `Step` and `Result` classes, and action steps. More help will be provided in the future, but for now, let's just look at the code in demos/custom_phase/custom.py:
@@ -862,15 +908,15 @@
         for file_op in self.files.get_operations('generate'):
             for out in file_op.output_files:
                 source_code = get_source_code(out.path)
                 self.do_step_generate_source(action, dirs[out.path.parent],
                                              source_code, origin_path, out.path)
 ```
 
-There's a bit going on, but it's not terrible. This uses some facilities available in `CFamilyBuildPhase` to clean generated source and the generation directory, as well as making directories for the build. The main work is in generating the source files in an appropriate generation directory.
+There's a bit going on, but it's not terrible. Actions already implemented in `CFamilyBuildPhase` can clean generated source and the generation directory, as well as make directories for the build. The main work here is in generating the source files in an appropriate generation directory.
 
 Integrating this custom phase into your makefile is as simple as making a new instance of the new phase, and setting it as a dependency of the build phase:
 
 ```python
 'Bsic project with custom code generation phase'
 
 # pylint: disable=wrong-import-position
@@ -916,33 +962,34 @@
 
 And that's it. Now the `build` action will first generate the files in the right place if needed, and then build them if needed. The `clean` action will delete the generated files, and the `clean_build_directory` action will not only remove the build, but also the generated source directory.
 
 > A few notes: The above will only generate the source files if they don't exist, or are older than the makefile (which has the source text in it). Also, the gen diretory is based on `gen_anchor` (by way of `build_anchor`), which is necessary for any generated files to be built in the right place if you change `gen_anchor`'s value.
 
 #### Adding new actions
 
-To add a new action to a custom phase, simply add a method to the phase class. For example, to add an action called "deploy", write a method like so:
+To add a new action to a custom phase, simply add a method to the phase class. For example, to add an action called "deploy", write a phase method like so:
 
 ```python
+    ...
     def do_action_deploy(self, action: Action) -> ResultCode:
         ...
 ```
 (You'll want to import Action and ResultCode from pyke if you want the annotations.) That's all you need to do for the method to be called on an action, since actions' names are just strings, and pyke reflects on method names to find a phase that can handle the action. Of course, implmenting actions is more involved, as you can see above.
 
 ### Adding new build kinds
 
-Adding new build kinds is straightforward if you're just trying to customize the system build commands. There are currently three that depend on the build kind: `debug_level`; `optimization`; and `flags`. For POSIX tools, these correspond to the `-g{debug_level}`, `-O{optimization}`, and `{flags}` of any definition. If you wanted a custom kind called "smallest", imply provide the following overrides, with perhaps these values:
+Adding new build kinds is straightforward if you're just trying to customize the system build commands. There are currently three that depend on the build kind: `debug_level`; `optimization`; and `flags`. For POSIX tools, these correspond to the `-g{debug_level}`, `-O{optimization}`, and `{flags}` of any definition. If you wanted a custom kind called "smallest", simply provide the following overrides, with perhaps these values:
 
 ```
 'gnuclang_smallest_debug_level': '0',
 'gnuclang_smallest_optimization': 's',
 'gnuclang_smallest_flags': ['-DNDEBUG'],
 ```
 
-When selecting the build kind with `-o kind=smallest`, these overrides should be selected for the build.
+When selecting the build kind with `-o kind=smallest`, these overrides will be selected for the build.
 
 ### Setting colors
 
 The colorful output can be helpful, but not if you're on an incapable terminal, or just don't like them or want them at all. You can select a color palette:
 
 ```
 pyke -o colors=none build
```

### Comparing `pyke_build-0.1.0/README.md` & `pyke_build-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,34 +16,36 @@
 Usually, a declarative syntax is desireable for systems like this. But even CMake is a sort of language, and pyke files are too--just, in python. Very basic python is all you need to know to use it fully, and when you need that convenience of a full language, it's very nice to have. Sane defaults and a simple object structure help keep things fairly minimal for a basic project.
 
 - **Extensibility**
 Pyke comes with some basic classes (called `Phase`s) which can manage basic tasks. But you may have special needs in your project tha require a specific tool to be run, or files to be moved around, or secret keys to be managed, etc. If it's not in the basic set of classes, build your own. It's a reasonable interface to design new functionality for.
 
 ## Installing pyke
 
-Pyke is very nearly ready for its first submission to PyPI. Until then, clone this repo and install locally:
-
-```
-$ git clone git@github.com:spacemeat/pyke
-$ cd pyke
-$ pip install .
-```
-<!--
 Couldn't be easier. You need to be running python3.10 at least, and have pip installed. To install it globally:
 
 ```
-$ pip install pyke
+$ python3 -m pip install pyke-build
 ```
+
 or,
+
 ```
-$ pip install --user pyke
+$ python3 -m pip install --user pyke-build
 ```
--->
+
 You can optionally put it in a virtual environment, which may be the better idea.
 
+Alternatively, you can clone this repo and install locally:
+
+```
+$ git clone https://github.com/spacemeat/pyke
+$ cd pyke
+$ python3 -m pip install .
+```
+
 ## Using pyke
 
 We'll do a simple example. We have a C project laid out like this:
 
 ```
 simple_app
 ├── include
@@ -197,15 +199,15 @@
 * They cannot be cyclical. The dependency graph must not contain loops, though diamond relationships are fine.
 * Option overrides and actions that are specified to multiple phases in a dependency tree happen in reverse depth-first order. The deepest dependency phases act first; this way, dependencies that build objects will happen before those that depend on them to build libraries, etc. When setting actions and overrides from the command line, the default is to set them to all phases, so whole dependency graphs can be levered at once.
 
 If your project has multiple steps to build static libraries or shared objects (dynamic libraries) which are then used by other binaries in the build, you can make them dependencies of the built binary phases that use them. The appropriate directories and file references will automatically be resolved. Further, depnding on the properties of the project, appropriate dynamic lookup options will be inserted as well (like `-rpath` options for UNIX-like systems).
 
 ## Actions
 
-Pyke is not just good for building. There are other standard actions it can perform, with more forthcoming. Actually, it's more correct to say that `Phase` objects perform actions. Any string passed as an action on the command line will be applied as an action to the appropriate phases which implement the action. If no phase supports the action, it is quietly ignored.
+Pyke is not just good for building. There are other standard actions it can perform, with more forthcoming. Actually, it's more correct to say that `Phase` objects perform actions. Any string passed as an action on the command line will be applied to the appropriate phases which implement the action. If no phase supports the action, it is quietly ignored.
 
 There is a default action (`report_actions`) which displays the available actions in each phase of a project. This default can be overridden in a config file, either in a project or under $HOME (see [configuring pyke](#configuring-pyke)), to make the default action something different.
 
 ### Built-in actions
 
 Currently, the supported actions in each built-in phase are:
 
@@ -437,19 +439,19 @@
 You can also explicitly override after phase creation:
 
 ```python
 from pyke import CompileAndLinkToExePhase, Op, get_main_phase
 
 phase = CompileAndLinkToExePhase('simple_experiemtal', {
     'sources': ['a.cpp', 'b.cpp', 'c.cpp', 'main.cpp'],
-    'include_dirs': Op('+=', 'include/exp')        # appending to include_dirs
+    'include_dirs': Op('+=', 'include/exp')                 # appending to include_dirs
 })
 
-phase.push_opts({                                           # appending to sources
-    'sources': Op('*=', [f'exp/{src}' for src in [
+phase.push_opts({
+    'sources': Op('*=', [f'exp/{src}' for src in [          # extending sources
              'try_this.cpp', 'maybe.cpp', 'what_if.cpp']])
 })
 
 get_main_phase().depend_on(phase)
 ```
 
 Note the use of the `Op` class, which signals that the override is an operational modifier, not merely a replacement. The operator is expressed as a string. Overriding with a value directly instead of with `Op` implies a replacement ('=').
@@ -467,23 +469,25 @@
 As seen previously, overrides can be specified on the command line as well with `-o [phases:][option[op value]`. This can look similar to overrides in code (though you may need to enquote it):
 
 ```
 $ pyke -ocolors=none build
 $ pyke -o "compile:sources *= [exp/try_this.c, exp/maybe.c, exp/what_if.c]" opts
 ```
 
-String values can be in quotes if they need to be disambiguated from punctuation. The usual escapements work with '\'. Overrides you specify with `[]` are treated as lists, `()` as tuples, `{}` as sets, and `{:}` as dicts. Since option keys must only contain letters, numbers, and underscores, you can differentiate a single-valued set from an interpolation by inserting a comma, or specifically enquoting the string:
+String values can be in quotes if they need to be disambiguated from punctuation or shell interpolation. The usual escapements work with '\\'. Overrides you specify with `[]` are treated as lists, `()` as tuples, `{}` as sets, and `{:}` as dicts. Since option keys must only contain letters, numbers, and underscores, you can differentiate a single-valued set from an interpolation by inserting a comma, or specifically enquoting the string:
 
 ```
 $ pyke -o "my_set_of_one={foo,}" ...
 $ pyke -o "my_set_of_one={'foo'}" ...
 ```
 
 Python's built-in literals True, False, and None are defined as options, and can be interpolated as {true}, {false}, and {none}.
 
+Much like older-style subshell invocation, you can enquote a shell command in \`backtick\`s, and the command will be executed, with its output inserted in place. This is most useful in config files, since they're not executed in a shell context.
+
 There is more to say about how value overrides are parsed. Smartly using quotes, commas, or spaces to differentiate strings from interpolators will usually get you where you want. Generally, though, setting options in the makefile will probably be preferred.
 
 ### Base pyke options
 
 There are a few options that are uiversal to pyke, regardless of the type of project it is running. Here are the options you can set to adjust its behavior:
 
 |option|default|usage
@@ -615,29 +619,61 @@
 exe_anchor = {build_detail_anchor}/{exe_dir}
 exe_path = {exe_anchor}/{exe_file}
 ```
 You are encouraged to change `exe_dir` to set a base directory for executable files, and `exe_basename` to set the name of the executable. Pyke will only reference `exe_path` directly.
 
 Similar options are defined for static archives and shared objects. Of course, you can change any of these, or make your own constructed paths.
 
+### Recursive makefiles
+
+You can run another makefile within a makefile:
+
+```python
+# shaper/libs/make.py:
+import pyke as p
+shape_lib = p.CompileAndLinkToArchive()
+s = shape_lib.clone({'name': 'sphere',      'sources': ['shapes/sphere.cpp']})
+c = shape_lib.clone({'name': 'cube',        'sources': ['shapes/cube.cpp']})
+i = shape_lib.clone({'name': 'icosohedron', 'sources': ['shapes/icosohedron.cpp']})
+p.get_main_phase().depend_on([s, c, i])
+```
+```python
+# shaper/exe/make.py:
+import pyke as p
+
+base = p.run_makefile('../libs')   # tries to load '../libs/make.py'
+libs = [base.find_dep(lib) for lib in ('sphere', 'cube', 'icosohedron')]
+exe = p.CompileAndLinkToExePhase({'sources': ['main.c']}, libs)
+p.get_main_phase().depend_on(exe)
+```
+
+Here, the makefile `../libs/make.py` is run. Its ProjectPhase is returned as `base`, and the phases it loaded can be found in its dependency tree. The `project_anchor` and `gen_anchor` options are preserved for each makefile, though you can change them manually. Each makefile will also load its cohabiting `pyke-config.json` file as well, unless you suppress it with a parameter:
+
+```python
+...
+base = p.run_makefile('../libs', False)  # does not load libs/pyke-config.py, even if it exists.
+...
+```
+
 ## The CLI
 
 The general form of a pyke command is:
 
 ```
 pyke [-v | -h | [-c]? [-m makefile]? ]? [[-p [phase[,phase]*]]* | [-o [phase[,phase]*:]key[op_value]]* | [phase[,phase]*:][action]* ]*
 ```
 
 Notably, -o and action arguments are processed in command-line order. You can set the phases to use with each, setting some option overrides, performing actions, setting different options, perform more actions, etc. If no phases are specified, the overrides and actions apply to all phases, in reverse depth-first dependency order.
 
 The command line arguments are:
 * `-v`, `--version`: Prints the version information for pyke, and exits.
 * `-h`, `--help`: Prints a help document.
-* `-c`, `--cache_makefile`: Allows the makefile's __cache__ to be generated. This might speed up complex builds, but they'd hvae to be really complex. Must precede any arguments that are not -v, -h, or -m.
-* `-m`, `--module`: Specifies the module (pyke file), or its directory if the pyke file is called 'make.py', to be run. Must precede any arguments that are not -v, -h, or -c. If no -m argument is given, pyke will look for and run ./make.py.
+* `-m`, `--makefile`: Specifies the module (pyke file), or its directory if the pyke file is called 'make.py', to be run. Must precede any arguments that are not -v, -h, or -c. If no -m argument is given, pyke will look for and run ./make.py.
+* `-n`, `--noconfig`: Specifies that the `pyke-config.json` file adjacent to the makefile should not be loaded.
+* `-c`, `--report-config`: Prints the full combined configuration from all loaded config files, and exits.
 * `-p`, `--phases`: Specifies a subset of phases on which to apply subsequent overrides or actions, if such arguments do not provide their own. Each `-p` encountered resets the subgroup. Option and action arguments that provide their own phases overrule `-p` for that argument, but do not reset it.
 * `-o`, `--override`: Specifies an option override to apply to some or all phases for subsequenet actions. If the option is given as a key-op-value, the override is pushed; if it is only a key (with no operator-value pair) the override is popped.
 * `action`: Arguments given without switches specify actions to be taken on the indicated phases. Any action on any phase which doesn't support it is quietly ignored.
 
 ### Referencing phases
 
 Phases have names (`short name`s), as seen, but also have `full name`s, given as "group.name". For each phase, if the group name is not explicitly set, it is overridden *after the makefile is run* to be the short name of the closest dependency *project phase*. Project phases are thereafter given the short name `project`. This naming scheme allows for subprojects to be referenced by the group name on the CLI. We'll see some examples.
@@ -709,14 +745,15 @@
 * ~/.config/pyke/pyke-config.json
 * <makefile's directory>/pyke-config.json
 
 An example config might look like this:
 
 ```json
 {
+    "include": ["../pyke-config.json"],
     "argument_aliases": {
         "-noc": "-ocolors=none",
         "-bdb": "dbadmin:build",
         "-rdb": [
             "-odbadmin:run_args=\"-logging=TRUE -username=$DBADMIN_UNAME -password=$DBADMIN_PASSWD\"",
             "dbadmin:run"
         ]
@@ -724,20 +761,25 @@
     "action_aliases": {
         "pf": "package_flatpak",
         "vac": "verify_appchecker"
     },
     "default_action": "build",
     "default_arguments": [
         "-v2"
-    ]
+    ],
+    "cache_makefile_module": "true"
 }
 ```
 
 Each can contain the following sections:
 
+### Include files
+
+These are paths to other JSON files which contribute to the configuration. They are loaded before the rest of this file's contents, which can add to or override as described below. Useful if you have distinct configuration for work projects vs. personal projects, or lots of pyke projects which all use the same options. Paths that start with '/' are absolute; otherwise, they are relative to this file's path.
+
 ### Argument aliases
 
 These are convenient shorthands for complex overrides, override-action pairs, or whatever you like. Their values cannot contain other argument alias names, but *can* contain action aliases, and are otherwise exactly as you'd type them on the CLI (except you don't need to enquote things that the shell might interpret). Multiple values must be housed in a list. Each config file adds to the list of argument aliases.
 
 ### Action aliases
 
 Actions can be aliased. These are one-for-one word replacements, and the action values must not be other action aliases, though you *can* have more than one alias for any given action. Each config file adds to the list of action aliases.
@@ -746,14 +788,18 @@
 
 The default action is taken when no action is specified on a CLI. By default, this is set to `report_actions`. The value must not be an alias. Each config file overrides a set default action.
 
 ### Default arguments
 
 Ccontains a list of strings, each of which is a separate command line argument. These can be full names or aliases. They are placed consecutively directly after the -m argument, but before any -o or action arguments, on every invocation of pyke. It is a convenient way to customize the way pyke always works on your project or machine. Each config file appends to the list of default arguments.
 
+### Cache makefile module
+
+Allows the makefile's __cache__ to be generated by python. This might speed up complex builds, but they'd hvae to be really complex.
+
 ## Advanced Topics
 
 ### Adding new phases
 
 Of course, a benefit of a programmatic build system is extension. Building your own Phase classes shold be straightforward. You likely won't have to often.
 
 Say you need a code generator. It must make .c files your project compiles and links with extant source. You can write a custom Phase-derived class to do just this. This gets you into the weeds of `Step` and `Result` classes, and action steps. More help will be provided in the future, but for now, let's just look at the code in demos/custom_phase/custom.py:
@@ -840,15 +886,15 @@
         for file_op in self.files.get_operations('generate'):
             for out in file_op.output_files:
                 source_code = get_source_code(out.path)
                 self.do_step_generate_source(action, dirs[out.path.parent],
                                              source_code, origin_path, out.path)
 ```
 
-There's a bit going on, but it's not terrible. This uses some facilities available in `CFamilyBuildPhase` to clean generated source and the generation directory, as well as making directories for the build. The main work is in generating the source files in an appropriate generation directory.
+There's a bit going on, but it's not terrible. Actions already implemented in `CFamilyBuildPhase` can clean generated source and the generation directory, as well as make directories for the build. The main work here is in generating the source files in an appropriate generation directory.
 
 Integrating this custom phase into your makefile is as simple as making a new instance of the new phase, and setting it as a dependency of the build phase:
 
 ```python
 'Bsic project with custom code generation phase'
 
 # pylint: disable=wrong-import-position
@@ -894,33 +940,34 @@
 
 And that's it. Now the `build` action will first generate the files in the right place if needed, and then build them if needed. The `clean` action will delete the generated files, and the `clean_build_directory` action will not only remove the build, but also the generated source directory.
 
 > A few notes: The above will only generate the source files if they don't exist, or are older than the makefile (which has the source text in it). Also, the gen diretory is based on `gen_anchor` (by way of `build_anchor`), which is necessary for any generated files to be built in the right place if you change `gen_anchor`'s value.
 
 #### Adding new actions
 
-To add a new action to a custom phase, simply add a method to the phase class. For example, to add an action called "deploy", write a method like so:
+To add a new action to a custom phase, simply add a method to the phase class. For example, to add an action called "deploy", write a phase method like so:
 
 ```python
+    ...
     def do_action_deploy(self, action: Action) -> ResultCode:
         ...
 ```
 (You'll want to import Action and ResultCode from pyke if you want the annotations.) That's all you need to do for the method to be called on an action, since actions' names are just strings, and pyke reflects on method names to find a phase that can handle the action. Of course, implmenting actions is more involved, as you can see above.
 
 ### Adding new build kinds
 
-Adding new build kinds is straightforward if you're just trying to customize the system build commands. There are currently three that depend on the build kind: `debug_level`; `optimization`; and `flags`. For POSIX tools, these correspond to the `-g{debug_level}`, `-O{optimization}`, and `{flags}` of any definition. If you wanted a custom kind called "smallest", imply provide the following overrides, with perhaps these values:
+Adding new build kinds is straightforward if you're just trying to customize the system build commands. There are currently three that depend on the build kind: `debug_level`; `optimization`; and `flags`. For POSIX tools, these correspond to the `-g{debug_level}`, `-O{optimization}`, and `{flags}` of any definition. If you wanted a custom kind called "smallest", simply provide the following overrides, with perhaps these values:
 
 ```
 'gnuclang_smallest_debug_level': '0',
 'gnuclang_smallest_optimization': 's',
 'gnuclang_smallest_flags': ['-DNDEBUG'],
 ```
 
-When selecting the build kind with `-o kind=smallest`, these overrides should be selected for the build.
+When selecting the build kind with `-o kind=smallest`, these overrides will be selected for the build.
 
 ### Setting colors
 
 The colorful output can be helpful, but not if you're on an incapable terminal, or just don't like them or want them at all. You can select a color palette:
 
 ```
 pyke -o colors=none build
```

### Comparing `pyke_build-0.1.0/demos/custom_phase/custom.py` & `pyke_build-0.2.0/demos/custom_phase/custom.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/demos/custom_phase/make.py` & `pyke_build-0.2.0/demos/custom_phase/make.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/demos/diamond_deps/make.py` & `pyke_build-0.2.0/demos/diamond_deps/make.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/demos/multi_make/simple_0.py` & `pyke_build-0.2.0/demos/multi_make/simple_0.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/demos/multi_make/simple_1.py` & `pyke_build-0.2.0/demos/multi_make/simple_1.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/pyproject.toml` & `pyke_build-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/readme_helper.py` & `pyke_build-0.2.0/readme_helper.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/src/pyke/__init__.py` & `pyke_build-0.2.0/src/pyke/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 try:
     from ._version import version as __version__
     from ._version import version_tuple
 except ImportError:
     __version__ = '(unknown version)'
     version_tuple = (0, 0, '(unknown version)')
 
+from .action import Action, ResultCode, Step, Result, FileData
 from .options import Options, OptionOp, Op
 from .phases import (Phase, CommandPhase, CFamilyBuildPhase, CompilePhase, ArchivePhase,
                      LinkToExePhase, LinkToSharedObjectPhase, CompileAndArchivePhase,
                      CompileAndLinkToExePhase, CompileAndLinkToSharedObjectPhase, ProjectPhase)
-from .pyke import get_main_phase
-from .action import Action, ResultCode, Step, Result, FileData
+from .pyke import get_main_phase, run_makefile
 from .utilities import input_path_is_newer, do_shell_command
```

### Comparing `pyke_build-0.1.0/src/pyke/action.py` & `pyke_build-0.2.0/src/pyke/action.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/src/pyke/ansi.py` & `pyke_build-0.2.0/src/pyke/ansi.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/src/pyke/options.py` & `pyke_build-0.2.0/src/pyke/options.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/src/pyke/options_parser.py` & `pyke_build-0.2.0/src/pyke/options_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 ''' Bits for parsing stringized options, like one gets from a command line.'''
 
 from dataclasses import dataclass
 from enum import Enum
 import re
 from typing import Any, Callable
-from .utilities import InvalidOptionValue
+from .utilities import InvalidOptionValue, do_shell_command
 
 class Token(Enum):
     ''' Encodes tokens found in override values parsed from a string. '''
     QSTRING = '\''
     DQSTRING = '"'
+    BQSTRING = '`'
     LPAREN = '('
     RPAREN = ')'
     LBRACKET = '['
     RBRACKET = ']'
     LBRACE = '{'
     RBRACE = '}'
     COLON = ':'
@@ -78,19 +79,21 @@
 
         if self.value == '':
             self.toks.append(TokenObj(Token.STRING, '', depth))
         else:
             while idx < len(self.value):
                 cur = self.value[idx]
                 match cur:
-                    case '\'' | '"':
+                    case '\'' | '"' | '`':
                         if cur == '\'':
                             self.toks.append(TokenObj(Token.QSTRING, '', depth))
-                        else:
+                        elif cur == '"':
                             self.toks.append(TokenObj(Token.DQSTRING, '', depth))
+                        else:
+                            self.toks.append(TokenObj(Token.BQSTRING, '', depth))
                         sidx = idx + 1
                         while sidx < len(self.value):
                             scur = self.value[sidx]
                             if scur == '\\':
                                 sidx += 1
                                 if sidx < len(self.value):
                                     scur = self.value[sidx]
@@ -315,17 +318,23 @@
         def recur(toks: list) -> Any:
             tok_idx = 0
 
             def get_unit_obj(tok: TokenObj) -> Any:
                 match tok.token:
                     case Token.INT: return int(tok.value, 0)
                     case Token.FLOAT: return float(tok.value)
+                    case Token.STRING: return tok.value
                     case Token.QSTRING: return tok.value
                     case Token.DQSTRING: return tok.value
-                    case Token.STRING: return tok.value
+                    case Token.BQSTRING:
+                        ret, out, err = do_shell_command(tok.value)
+                        if ret != 0:
+                            raise InvalidOptionValue(f'Shell-command option {tok.value} '
+                                                     f'returned "{err}" ({ret}).')
+                        return out.strip()
                 return tok
 
             while tok_idx < len(toks):
                 tok = toks[tok_idx]
                 if isinstance(tok, list):
                     return recur(tok)
```

### Comparing `pyke_build-0.1.0/src/pyke/phases/__init__.py` & `pyke_build-0.2.0/src/pyke/phases/__init__.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/src/pyke/phases/archive.py` & `pyke_build-0.2.0/src/pyke/phases/archive.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/src/pyke/phases/c_family_build.py` & `pyke_build-0.2.0/src/pyke/phases/c_family_build.py`

 * *Files identical despite different names*

```diff
@@ -464,15 +464,15 @@
         ''' Get all the headers used by the given src_path, including system headers.'''
         if not src_path.exists():
             return []
         cmd = self.make_cmd_compile_src_to_object(src_path, obj_path, True)
         ret, _, err = do_shell_command(cmd)
         if ret == 0:
             return self.parse_include_report(err)
-        raise ValueError('Header discovery failed.')
+        return []
 
     def do_step_create_directory(self, action: Action, depends_on: Steps, new_dir: Path) -> Step:
         '''
         Performs a directory creation operation as an action step.
         '''
         def act(cmd: str, new_dir: Path):
             step_result = ResultCode.SUCCEEDED
```

### Comparing `pyke_build-0.1.0/src/pyke/phases/command_phase.py` & `pyke_build-0.2.0/src/pyke/phases/command_phase.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/src/pyke/phases/compile.py` & `pyke_build-0.2.0/src/pyke/phases/compile.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/src/pyke/phases/compile_and_archive.py` & `pyke_build-0.2.0/src/pyke/phases/compile_and_archive.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/src/pyke/phases/compile_and_link_to_exe.py` & `pyke_build-0.2.0/src/pyke/phases/compile_and_link_to_exe.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/src/pyke/phases/compile_and_link_to_so.py` & `pyke_build-0.2.0/src/pyke/phases/compile_and_link_to_so.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             'target_path': '{shared_object_path}',
             'relocatable_code': True,
         }
         self.options |= (options or {})
 
     def patch_options(self):
         ''' Fixups run before file operations.'''
-        for dep in self.enumerate_dependencies():
+        for dep in self.iterate_dep_tree():
             dep.push_opts({'relocatable_code': True}, True, True)
 
     def compute_file_operations(self):
         ''' Implelent this in any phase that uses input files or generates output files.'''
         so_path = Path(self.opt_str('shared_object_path'))
 
         prebuilt_objs = [FileData(prebuilt_obj_path, 'object', None)
```

### Comparing `pyke_build-0.1.0/src/pyke/phases/link_to_exe.py` & `pyke_build-0.2.0/src/pyke/phases/link_to_exe.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/src/pyke/phases/link_to_shared_object.py` & `pyke_build-0.2.0/src/pyke/phases/link_to_shared_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             'name': 'link_to_shared_object',
             'target_path': '{shared_object_path}',
         }
         self.options |= (options or {})
 
     def patch_options(self):
         ''' Fixups run before file operations.'''
-        for dep in self.enumerate_dependencies():
+        for dep in self.iterate_dep_tree():
             dep.push_opts({'relocatable_code': True}, True, True)
 
     def compute_file_operations(self):
         ''' Implelent this in any phase that uses input files or generates output files.'''
 
         so_path = Path(self.opt_str('shared_object_path'))
```

### Comparing `pyke_build-0.1.0/src/pyke/phases/phase.py` & `pyke_build-0.2.0/src/pyke/phases/phase.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,45 +123,40 @@
             self.depend_on(dep)
 
         self.files: PhaseFiles
 
     def __repr__(self):
         return self.name
 
-    def enumerate_dependencies(self):
+    def iterate_dep_tree(self):
         ''' Enumerates all the dependencies in depth-first order.'''
         for dep in self.dependencies:
-            yield from dep.enumerate_dependencies()
+            yield from dep.iterate_dep_tree()
         yield self
 
-    def find_dependency_by_name(self, name: str):
+    def find_dep(self, name: str):
         ''' Finds the dependency (including self) by name.'''
-        for dep in self.enumerate_dependencies():
-            if dep.opt_str('name') == name:
+        for dep in self.iterate_dep_tree():
+            if name in (dep.name, dep.full_name):
                 return dep
         return None
 
-    def find_in_dependency_tree(self, dep_to_find: Self):
-        ''' Returns whether dep_to_find is in the dependency tree for this phase. '''
-        try:
-            idx = self.dependencies.index(dep_to_find)
-            return self.dependencies[idx]
-        except ValueError:
-            for dep in self.dependencies:
-                phase = dep.find_in_dependency_tree(dep_to_find)
-                if phase is not None:
-                    return phase
-            return None
+    def find_dep_object(self, dep_to_match: Self):
+        ''' Finds the dependency (including self) by name.'''
+        for dep in self.iterate_dep_tree():
+            if dep == dep_to_match:
+                return dep
+        return None
 
     def depend_on(self, new_deps: Self | list[Self]):
         ''' Sets a dependency phase for this phase. Must not be a phase which does not
         depend on this phase already (no circular references allowed). '''
         new_deps = ensure_list(new_deps)
         for new_dep in new_deps:
-            if new_dep.find_in_dependency_tree(self) is not None:
+            if new_dep.find_dep_object(self) is not None:
                 raise CircularDependencyError(
                     f'Attempt to set a circular dependency {new_dep.opt_str("name")} '
                     f'to phase {self.name}. Not cool.')
             self.dependencies.append(new_dep)
 
     def clone(self, options: dict | None = None,
               dependencies = None):
@@ -183,23 +178,23 @@
         else:
             group_name = self.opt_str('group')
         for phase in self.dependencies:
             phase.propagate_group_names(group_name)
 
     def patch_options_in_dependencies(self):
         ''' Opportunity for phases to fix up options before running file operations.'''
-        for dep in list(self.enumerate_dependencies()):
+        for dep in list(self.iterate_dep_tree()):
             dep.patch_options()
 
     def patch_options(self):
         ''' Fixups run before file operations.'''
 
     def compute_file_operations_in_dependencies(self):
         ''' Compute file operations dwon the dependency hierarchy.'''
-        for dep in list(self.enumerate_dependencies()):
+        for dep in list(self.iterate_dep_tree()):
             dep.files = PhaseFiles()
             dep.compute_file_operations()
 
     def compute_file_operations(self):
         ''' Implelent this in any phase that uses input files or generates output files.'''
 
     def record_file_operation(self, input_files: list[FileData] | FileData | None,
```

### Comparing `pyke_build-0.1.0/src/pyke/pyke.py` & `pyke_build-0.2.0/src/pyke/pyke.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,83 +8,64 @@
 
 from enum import Enum
 import importlib.util
 import importlib.machinery
 import os
 from pathlib import Path
 import sys
-import json
 import traceback
 
 from . import __version__
 from .action import Action
+from .config import Configurator
 from .options import OptionOp, Op
 from .options_parser import parse_value
 from .phases.phase import Phase
 from .phases.project import ProjectPhase
-from .utilities import WorkingSet, MalformedConfigError, ensure_list
+from .utilities import PhaseNotFoundError, WorkingSet, ensure_list
 
-def get_main_phase():
+def get_main_phase() -> Phase:
     ''' Returns the main project created for the makefile.'''
+    if not WorkingSet.main_phase:
+        raise PhaseNotFoundError('No main phase found. Seems unlikely, but there it is.')
     return WorkingSet.main_phase
 
 class ReturnCode(Enum):
     ''' Encoded return code for program exit.'''
     SUCCEEDED = 0
     MAKEFILE_NOT_FOUND = 1
     MAKEFILE_DID_NOT_LOAD = 2
     INVALID_ARGS = 3
     ACTION_FAILED = 4
 
-def run_make_file(pyke_path, cache_make):
-    ''' Loads and runs the user-created make file.'''
-    if pyke_path.exists():
-        try:
-            sys.dont_write_bytecode = not cache_make
-            spec = importlib.util.spec_from_file_location('pyke', pyke_path)
-            if spec:
-                module = importlib.util.module_from_spec(spec)
-                loader = spec.loader
-                if loader:
-                    loader.exec_module(module)
-                    sys.dont_write_bytecode = cache_make
-                    return
-        except Exception:
-            print (f'"{pyke_path}" could not be loaded.')
-            traceback.print_exc()
-            sys.exit(ReturnCode.MAKEFILE_DID_NOT_LOAD.value)
-    else:
-        print (f'"{pyke_path}" was not found.')
-        sys.exit(ReturnCode.MAKEFILE_NOT_FOUND.value)
-
-
 def print_version():
     ''' Print the version.'''
     print (f'pyke version {__version__}')
 
 
 def print_help():
     ''' Send help.'''
     print (
-    ''' Pyke - a Python-powered build system
+''' Pyke - a Python-powered build system
 
 Usage:
 pyke [invocations]* [phases | overrides | actions]*
 
 invocations:
 -v, --version: Prints the version information for pyke, and exits.
 -h, --help: Prints a help document.
--c, --cache_makefile: Allows the makefile's __cache__ to be generated. This
-    might speed up complex builds, but they'd hvae to be really complex to
-    make a noticeable difference.
 -m, --makefile: Specifies the makefile (pyke file) to be run. Actions are
     performed relative to the makefile's directory, unless an option override
     (-o gen_anchor=dir/to/gen) is given, in which case they are performed
     relative to the given anchor directory. If no -m argument is given, pyke
     will look for and run ./make.py.
+-n, --noconfig: Specifies that the pyke-config.json file adjacent to the
+    makefile should not be loaded.
+-c, --report-config: Prints the full configuration combined from all loaded
+    config files, and exits.
 
 phases:
 -p, --phases: Specifies one or more phases to set as active phases for the
     subsequent overrides and actions, providing they do not specify their own.
     The format is:
     -p phases
     'phases' is a comma-separated list of names of phase objects defined in
@@ -163,116 +144,86 @@
 
 Looks for ./make.py && loads && overrides the 'colors' option && runs the
 'clean', 'build", and 'run' actions successively, given the success of each
 previous action.
 $ pyke -ocolors={colors_none} clean build run
 ''')
 
-def load_config():
-    ''' Loads aliases from ~/.config/pyke/pyke-config.json or <project-root>/pyke-config.json,
-    overriding in that order. '''
-    def process_config(config):
-        if not isinstance(config, dict):
-            raise MalformedConfigError(f'Config file {file}: Must be a JSON dictonary.')
-
-        def read_block(config, subblock, keyname) -> dict[str, list[str]]:
-            rets = {}
-            if aliases := config.get(subblock):
-                if not isinstance(aliases, dict):
-                    raise MalformedConfigError(
-                        f'Config file {file}: "{subblock}" must be a dictionary.')
-                for alias, values in aliases.items():
-                    if not isinstance(alias, str):
-                        raise MalformedConfigError(
-                            f'Config file {file}: "{config}/{keyname}" key must be a string.')
-                    if isinstance(values, str):
-                        values = [values]
-                    if (not isinstance(values, list) or
-                        any(not isinstance(value, str) for value in values)):
-                        raise MalformedConfigError(
-                            f'Config file {file}: "{config}/{keyname}" value must be a string '
-                            'or a list of strings.')
-                    rets[alias] = values
-            return rets
-
-        WorkingSet.argument_aliases |= read_block(config, 'argument_aliases', 'argument')
-        WorkingSet.action_aliases |= read_block(config, 'action_aliases', 'action')
-        if default_action := config.get('default_action'):
-            if not isinstance(default_action, str):
-                raise MalformedConfigError(
-                    f'Config file {file}: "default_action" must be a string.')
-            WorkingSet.default_action = default_action
-        if default_arguments := config.get('default_arguments'):
-            if not isinstance(default_arguments, list):
-                raise MalformedConfigError(
-                    f' Config file {file}: "default_arguments" must be a list of strings.')
-            WorkingSet.default_arguments.extend(default_arguments)
-
-    def set_default_config():
-        default_config = '''
-{
-    "argument_aliases": {
-        "-v0": "-overbosity=0",
-        "-v1": "-overbosity=1",
-        "-v2": "-overbosity=2",
-        "-rv0": "-oreport_verbosity=0",
-        "-rv1": "-oreport_verbosity=1",
-        "-rv2": "-oreport_verbosity=2",
-        "-release": "-okind=release",
-        "-versioned_sos": ["-oposix_shared_object_file={posix_so_real_name}",
-                           "-ogenerate_versioned_sonames=True"],
-        "vsos": ["-oposix_shared_object_file={posix_so_real_name}",
-                 "-ogenerate_versioned_sonames=True"],
-
-        "-deploy_install": ["-orpath_deps=False",
-                            "-omoveable_binaries=False",
-                            "-oposix_shared_object_file={posix_so_real_name}",
-                            "-ogenerate_versioned_sonames=true",
-                            "-okind=release"],
-        "-deploy_moveable": ["-orpath_deps=True",
-                             "-omoveable_binaries=True",
-                             "-oposix_shared_object_file={posix_so_linker_name}",
-                             "-ogenerate_versioned_sonames=false",
-                             "-okind=release"]
-    },
-    "action_aliases": {
-        "opts": "report_options",
-        "files": "report_files",
-        "actions": "report_actions",
-        "c": "clean",
-        "cbd": "clean_build_directory",
-        "b": "build"
-    },
-    "default_action": "report_actions",
-    "default_arguments": []
-} '''
-        config = json.loads(default_config)
-        process_config(config)
-
-    set_default_config()
-
-    for direc in list(dict.fromkeys([
-            Path.home() / '.config' / 'pyke',
-            WorkingSet.makefile_dir])):
-        file = Path(direc) / 'pyke-config.json'
+def _run_makefile(pyke_path):
+    ''' Loads and runs the user-created make file.'''
+    cache_make = Configurator.cache_makefile_module
+    if pyke_path.exists():
         try:
-            with open(file, 'r', encoding='utf-8') as fi:
-                config = json.load(fi)
-                process_config(config)
-        except (FileNotFoundError, MalformedConfigError):
-            pass
+            old_dont_write_bytecode = sys.dont_write_bytecode
+            sys.dont_write_bytecode = not cache_make
+            spec = importlib.util.spec_from_file_location('pyke', pyke_path)
+            if spec:
+                module = importlib.util.module_from_spec(spec)
+                loader = spec.loader
+                if loader:
+                    loader.exec_module(module)
+                    sys.dont_write_bytecode = old_dont_write_bytecode
+                    return
+        except Exception:
+            print (f'"{pyke_path}" could not be loaded.')
+            traceback.print_exc()
+            sys.exit(ReturnCode.MAKEFILE_DID_NOT_LOAD.value)
+    else:
+        print (f'"{pyke_path}" was not found.')
+        sys.exit(ReturnCode.MAKEFILE_NOT_FOUND.value)
+
+def run_makefile(make_file: str, load_makefile_config: bool = True):
+    ''' Load and run a makefile by relative path to the makefile directory.'''
+    old_makefile_dir = WorkingSet.makefile_dir
+    old_main_phase = WorkingSet.main_phase
+
+    if make_file.startswith('/'):
+        make_path = Path(make_file)
+    else:
+        make_path = old_makefile_dir / make_file
+    if not make_file.endswith('.py'):
+        make_path = make_path / 'make.py'
+
+    makefile_dir = make_path.parent
+    if proj := WorkingSet.loaded_makefiles.get(make_path):
+        return proj
+
+    if load_makefile_config:
+        Configurator.load_from_makefile_dir(makefile_dir)
+
+    WorkingSet.makefile_dir = makefile_dir
+
+    project_phase_name = (make_path.parent.name if
+        make_path.name == 'make.py'
+        else make_path.stem)
+    main_phase = ProjectPhase({
+        'name': project_phase_name})
+
+    WorkingSet.loaded_makefiles[make_path] = main_phase
+    WorkingSet.all_phases.add(main_phase)
+    WorkingSet.main_phase = main_phase
+
+    _run_makefile(make_path)
+
+    WorkingSet.makefile_dir = old_makefile_dir
+    WorkingSet.main_phase = old_main_phase
+    return main_phase
 
 def propagate_group_names():
     ''' Cascades project names to group names in dependency phases.'''
-    WorkingSet.main_phase.propagate_group_names('')
+    if WorkingSet.main_phase:
+        WorkingSet.main_phase.propagate_group_names('')
 
 def uniquify_phase_names():
     ''' Ensure phase names are unique within groups.'''
+    if not WorkingSet.main_phase:
+        return
+
     names = {}
-    for phase in WorkingSet.main_phase.enumerate_dependencies():
+    for phase in WorkingSet.main_phase.iterate_dep_tree():
         fullname = phase.full_name
         if fullname in names:
             c, lp = names[fullname]
             lp.append(phase)
             names[fullname] = (c + 1, lp)
         else:
             names[fullname] = (1, [phase])
@@ -298,109 +249,108 @@
     '.foo' specifies a phase with main group set, whose name is 'foo'
     '.@' specifies all phases with main group set, with any name
     '@.foo' specifies all phases in any group (or none), whose name is 'foo'
     'bar.@' specifies all phases in group 'bar'
     'bar.foo' specifies a phase in group 'bar' named 'foo'
     '@.@' specifies all phases
     '''
+    if not WorkingSet.main_phase:
+        return []
+
     phases = []
     labels = ensure_list(labels)
     for label in labels:
         if '.' not in label:
             label = f'{WorkingSet.main_phase.name}.{label}'
         if label.startswith('.'):
             label = f'{WorkingSet.main_phase.name}{label}'
         group_phase_label = label.split('.', 1)
         grouplabel, namelabel = group_phase_label
-        for phase in WorkingSet.main_phase.enumerate_dependencies():
+        for phase in WorkingSet.main_phase.iterate_dep_tree():
             if grouplabel in ['@', phase.group]:
                 if namelabel in ['@', phase.name]:
                     phases.append(phase)
     return phases
 
 def main():
     '''Entrypoint for pyke.'''
     current_dir = os.getcwd()
     make_file = 'make.py'
-    cache_make = False
+    load_makefile_config = True
 
     idx = 1
     while idx < len(sys.argv):
         arg = sys.argv[idx]
 
         if arg in ['-v', '--version']:
             print_version()
             return ReturnCode.SUCCEEDED.value
 
         if arg in ['-h', '--help']:
             print_help()
             return ReturnCode.SUCCEEDED.value
 
-        if arg in ['-c', '--cache_makefile']:
-            cache_make = True
-            idx += 1
-            continue
-
-        if arg.startswith('-m') or arg == '--module':
+        if arg.startswith('-m') or arg == '--makefile':
             make_file = ''
             if len(arg) > 2:
                 make_file = sys.argv[idx][2:]
             else:
                 idx += 1
                 make_file = sys.argv[idx]
             idx += 1
             continue
 
-        break
+        if arg in ['-n', '--noconfig']:
+            load_makefile_config = False
+            idx += 1
+            continue
 
-    make_path = Path(current_dir) / make_file
-    if not make_file.endswith('.py'):
-        make_path = make_path / 'make.py'
+        break
 
-    WorkingSet.makefile_dir = str(make_path.parent)
+    WorkingSet.makefile_dir = Path(current_dir)
 
-    load_config()
+    Configurator.load_from_default_config()
+    Configurator.load_from_home_config()
 
-    project_phase_name = (make_path.parent.name if
-        make_path.name == 'make.py'
-        else make_path.stem)
-    WorkingSet.main_phase = ProjectPhase({
-        'name': project_phase_name})
-    WorkingSet.all_phases.add(WorkingSet.main_phase)
+    main_phase = run_makefile(make_file, load_makefile_config)
+    WorkingSet.main_phase = main_phase
 
-    run_make_file(make_path, cache_make)
     propagate_group_names()
     uniquify_phase_names()
-    WorkingSet.main_phase.patch_options_in_dependencies()
+    main_phase.patch_options_in_dependencies()
 
     actions_done = []
     file_operations_are_dirty = True
 
     args = []
-    for arg in [*WorkingSet.default_arguments, *sys.argv[idx:]]:
-        args.extend(WorkingSet.argument_aliases.get(arg, [arg]))
+    for arg in [*Configurator.default_arguments, *sys.argv[idx:]]:
+        args.extend(Configurator.argument_aliases.get(arg, [arg]))
 
     affected_phases = get_phases('@.@')
 
     idx = 0
     while idx < len(args):
         arg = args[idx]
 
+        if arg in ['--makefile', '-n', '--noconfig'] or arg.startswith('-m'):
+            print (f'{arg} must precede any of -p (--phase), -o (--override), '
+                   '-c (--report_config), or any action arguments.')
+            return ReturnCode.INVALID_ARGS.value
+
         if arg in ['-v', '--version']:
             print_version()
             return ReturnCode.SUCCEEDED.value
 
         if arg in ['-h', '--help']:
             print_help()
             return ReturnCode.SUCCEEDED.value
 
-        if arg in ['-c', '--cache_makefile', '--module'] or arg.startswith('-m'):
-            print (f'{arg} must precede any of -p (--phase), -o (--override), '
-                   'or any action arguments.')
-            return ReturnCode.INVALID_ARGS.value
+        if arg in ['-c', '--report_config']:
+            print(Configurator.report())
+            return ReturnCode.SUCCEEDED.value
 
         if arg.startswith('-p') or arg == '--phases':
             if len(arg) > 2:
                 phases = arg[2:]
             else:
                 idx += 1
                 phases = args[idx]
@@ -448,39 +398,39 @@
 
             file_operations_are_dirty = True
 
         else:
             arg_affected_phases = []
 
             if file_operations_are_dirty:
-                WorkingSet.main_phase.compute_file_operations_in_dependencies()
+                main_phase.compute_file_operations_in_dependencies()
                 file_operations_are_dirty = False
 
             if ':' in arg:
                 phase_labels, arg = arg.split(':', 1)
                 arg_affected_phases = get_phases(phase_labels)
             else:
                 arg_affected_phases = affected_phases
 
-            arg = WorkingSet.action_aliases.get(arg, [arg])[0]
+            arg = Configurator.action_aliases.get(arg, [arg])[0]
             action = Action(arg)
             for active_phase in arg_affected_phases:
                 active_phase.do(action)
 
             res = action.run()
             if res.failed():
                 return ReturnCode.ACTION_FAILED.value
 
             actions_done.append(action.name)
 
         idx += 1
 
     if len(actions_done) == 0:
-        WorkingSet.main_phase.compute_file_operations_in_dependencies()
-        action = Action(WorkingSet.default_action)
+        main_phase.compute_file_operations_in_dependencies()
+        action = Action(Configurator.default_action)
         for active_phase in affected_phases:
             active_phase.do(action)
 
         res = action.run()
         if res.failed():
             return ReturnCode.ACTION_FAILED.value
```

### Comparing `pyke_build-0.1.0/src/pyke/utilities.py` & `pyke_build-0.2.0/src/pyke/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,23 +93,27 @@
         raise ValueError(f'Input file "{in_path}" does not exist; cannot compare m-times.')
 
     outm = out_path.stat().st_mtime if out_path.exists() else 0
     inm = in_path.stat().st_mtime
     return inm > outm
 
 def any_input_paths_are_newer(in_paths: list[Path], out_paths: list[Path]):
+    ''' Compares the modified times of each file in in_paths to each in out_paths. If any in
+    in_paths are newer than any in out_paths, or any in out_paths don't actually exist, then
+    return True.'''
     if any(not in_path.exists() for in_path in in_paths):
         raise ValueError('Input files do not exist; cannot compare m-times.')
 
     if len(in_paths) == 0 or len(out_paths) == 0:
         return True
 
+    max_mtime = 32536799999
     outm = functools.reduce(min,
                [out_path.stat().st_mtime if out_path.exists() else 0 for out_path in out_paths],
-               32536799999)
+               max_mtime)
     inm = functools.reduce(max,
                  [in_path.stat().st_mtime for in_path in in_paths], 0)
     return inm > outm
 
 def do_shell_command(cmd):
     ''' Reports, and then performs the given shell command as a subprocess. It is run in its
     own shell instance, each with its own environment. '''
@@ -134,20 +138,17 @@
     if ret == 0 and out == '16':
         return 'named'
 
     return 'none'
 
 class WorkingSet:
     ''' Keeps track of globally-available values.'''
-    makefile_dir = ''
-    argument_aliases = {}
-    action_aliases = {}
-    default_action = ''
-    default_arguments = []
-    main_phase: Phase
+    makefile_dir = Path()
+    loaded_makefiles: dict[Path, Phase] = {}
+    main_phase: Phase | None = None
     all_phases: set[Phase] = set()
 
 ansi_colors = {
     'colors_24bit': {
         'off':              {'form': 'off' },
         'success':          {'form': 'b24', 'fg': (0x33, 0xaf, 0x55) },
         'fail':             {'form': 'b24', 'fg': (0xff, 0x33, 0x33) },
```

### Comparing `pyke_build-0.1.0/src/pyke_build.egg-info/PKG-INFO` & `pyke_build-0.2.0/src/pyke_build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyke-build
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python-based build system for automating build and deployment tasks.
 Author-email: Trevor Schrock <spacemeat@gmail.com>
 Maintainer-email: Trevor Schrock <spacemeat@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/spacemeat/pyke.git
 Keywords: C,C++,build
 Classifier: Development Status :: 3 - Alpha
@@ -38,34 +38,36 @@
 Usually, a declarative syntax is desireable for systems like this. But even CMake is a sort of language, and pyke files are too--just, in python. Very basic python is all you need to know to use it fully, and when you need that convenience of a full language, it's very nice to have. Sane defaults and a simple object structure help keep things fairly minimal for a basic project.
 
 - **Extensibility**
 Pyke comes with some basic classes (called `Phase`s) which can manage basic tasks. But you may have special needs in your project tha require a specific tool to be run, or files to be moved around, or secret keys to be managed, etc. If it's not in the basic set of classes, build your own. It's a reasonable interface to design new functionality for.
 
 ## Installing pyke
 
-Pyke is very nearly ready for its first submission to PyPI. Until then, clone this repo and install locally:
-
-```
-$ git clone git@github.com:spacemeat/pyke
-$ cd pyke
-$ pip install .
-```
-<!--
 Couldn't be easier. You need to be running python3.10 at least, and have pip installed. To install it globally:
 
 ```
-$ pip install pyke
+$ python3 -m pip install pyke-build
 ```
+
 or,
+
 ```
-$ pip install --user pyke
+$ python3 -m pip install --user pyke-build
 ```
--->
+
 You can optionally put it in a virtual environment, which may be the better idea.
 
+Alternatively, you can clone this repo and install locally:
+
+```
+$ git clone https://github.com/spacemeat/pyke
+$ cd pyke
+$ python3 -m pip install .
+```
+
 ## Using pyke
 
 We'll do a simple example. We have a C project laid out like this:
 
 ```
 simple_app
 ├── include
@@ -219,15 +221,15 @@
 * They cannot be cyclical. The dependency graph must not contain loops, though diamond relationships are fine.
 * Option overrides and actions that are specified to multiple phases in a dependency tree happen in reverse depth-first order. The deepest dependency phases act first; this way, dependencies that build objects will happen before those that depend on them to build libraries, etc. When setting actions and overrides from the command line, the default is to set them to all phases, so whole dependency graphs can be levered at once.
 
 If your project has multiple steps to build static libraries or shared objects (dynamic libraries) which are then used by other binaries in the build, you can make them dependencies of the built binary phases that use them. The appropriate directories and file references will automatically be resolved. Further, depnding on the properties of the project, appropriate dynamic lookup options will be inserted as well (like `-rpath` options for UNIX-like systems).
 
 ## Actions
 
-Pyke is not just good for building. There are other standard actions it can perform, with more forthcoming. Actually, it's more correct to say that `Phase` objects perform actions. Any string passed as an action on the command line will be applied as an action to the appropriate phases which implement the action. If no phase supports the action, it is quietly ignored.
+Pyke is not just good for building. There are other standard actions it can perform, with more forthcoming. Actually, it's more correct to say that `Phase` objects perform actions. Any string passed as an action on the command line will be applied to the appropriate phases which implement the action. If no phase supports the action, it is quietly ignored.
 
 There is a default action (`report_actions`) which displays the available actions in each phase of a project. This default can be overridden in a config file, either in a project or under $HOME (see [configuring pyke](#configuring-pyke)), to make the default action something different.
 
 ### Built-in actions
 
 Currently, the supported actions in each built-in phase are:
 
@@ -459,19 +461,19 @@
 You can also explicitly override after phase creation:
 
 ```python
 from pyke import CompileAndLinkToExePhase, Op, get_main_phase
 
 phase = CompileAndLinkToExePhase('simple_experiemtal', {
     'sources': ['a.cpp', 'b.cpp', 'c.cpp', 'main.cpp'],
-    'include_dirs': Op('+=', 'include/exp')        # appending to include_dirs
+    'include_dirs': Op('+=', 'include/exp')                 # appending to include_dirs
 })
 
-phase.push_opts({                                           # appending to sources
-    'sources': Op('*=', [f'exp/{src}' for src in [
+phase.push_opts({
+    'sources': Op('*=', [f'exp/{src}' for src in [          # extending sources
              'try_this.cpp', 'maybe.cpp', 'what_if.cpp']])
 })
 
 get_main_phase().depend_on(phase)
 ```
 
 Note the use of the `Op` class, which signals that the override is an operational modifier, not merely a replacement. The operator is expressed as a string. Overriding with a value directly instead of with `Op` implies a replacement ('=').
@@ -489,23 +491,25 @@
 As seen previously, overrides can be specified on the command line as well with `-o [phases:][option[op value]`. This can look similar to overrides in code (though you may need to enquote it):
 
 ```
 $ pyke -ocolors=none build
 $ pyke -o "compile:sources *= [exp/try_this.c, exp/maybe.c, exp/what_if.c]" opts
 ```
 
-String values can be in quotes if they need to be disambiguated from punctuation. The usual escapements work with '\'. Overrides you specify with `[]` are treated as lists, `()` as tuples, `{}` as sets, and `{:}` as dicts. Since option keys must only contain letters, numbers, and underscores, you can differentiate a single-valued set from an interpolation by inserting a comma, or specifically enquoting the string:
+String values can be in quotes if they need to be disambiguated from punctuation or shell interpolation. The usual escapements work with '\\'. Overrides you specify with `[]` are treated as lists, `()` as tuples, `{}` as sets, and `{:}` as dicts. Since option keys must only contain letters, numbers, and underscores, you can differentiate a single-valued set from an interpolation by inserting a comma, or specifically enquoting the string:
 
 ```
 $ pyke -o "my_set_of_one={foo,}" ...
 $ pyke -o "my_set_of_one={'foo'}" ...
 ```
 
 Python's built-in literals True, False, and None are defined as options, and can be interpolated as {true}, {false}, and {none}.
 
+Much like older-style subshell invocation, you can enquote a shell command in \`backtick\`s, and the command will be executed, with its output inserted in place. This is most useful in config files, since they're not executed in a shell context.
+
 There is more to say about how value overrides are parsed. Smartly using quotes, commas, or spaces to differentiate strings from interpolators will usually get you where you want. Generally, though, setting options in the makefile will probably be preferred.
 
 ### Base pyke options
 
 There are a few options that are uiversal to pyke, regardless of the type of project it is running. Here are the options you can set to adjust its behavior:
 
 |option|default|usage
@@ -637,29 +641,61 @@
 exe_anchor = {build_detail_anchor}/{exe_dir}
 exe_path = {exe_anchor}/{exe_file}
 ```
 You are encouraged to change `exe_dir` to set a base directory for executable files, and `exe_basename` to set the name of the executable. Pyke will only reference `exe_path` directly.
 
 Similar options are defined for static archives and shared objects. Of course, you can change any of these, or make your own constructed paths.
 
+### Recursive makefiles
+
+You can run another makefile within a makefile:
+
+```python
+# shaper/libs/make.py:
+import pyke as p
+shape_lib = p.CompileAndLinkToArchive()
+s = shape_lib.clone({'name': 'sphere',      'sources': ['shapes/sphere.cpp']})
+c = shape_lib.clone({'name': 'cube',        'sources': ['shapes/cube.cpp']})
+i = shape_lib.clone({'name': 'icosohedron', 'sources': ['shapes/icosohedron.cpp']})
+p.get_main_phase().depend_on([s, c, i])
+```
+```python
+# shaper/exe/make.py:
+import pyke as p
+
+base = p.run_makefile('../libs')   # tries to load '../libs/make.py'
+libs = [base.find_dep(lib) for lib in ('sphere', 'cube', 'icosohedron')]
+exe = p.CompileAndLinkToExePhase({'sources': ['main.c']}, libs)
+p.get_main_phase().depend_on(exe)
+```
+
+Here, the makefile `../libs/make.py` is run. Its ProjectPhase is returned as `base`, and the phases it loaded can be found in its dependency tree. The `project_anchor` and `gen_anchor` options are preserved for each makefile, though you can change them manually. Each makefile will also load its cohabiting `pyke-config.json` file as well, unless you suppress it with a parameter:
+
+```python
+...
+base = p.run_makefile('../libs', False)  # does not load libs/pyke-config.py, even if it exists.
+...
+```
+
 ## The CLI
 
 The general form of a pyke command is:
 
 ```
 pyke [-v | -h | [-c]? [-m makefile]? ]? [[-p [phase[,phase]*]]* | [-o [phase[,phase]*:]key[op_value]]* | [phase[,phase]*:][action]* ]*
 ```
 
 Notably, -o and action arguments are processed in command-line order. You can set the phases to use with each, setting some option overrides, performing actions, setting different options, perform more actions, etc. If no phases are specified, the overrides and actions apply to all phases, in reverse depth-first dependency order.
 
 The command line arguments are:
 * `-v`, `--version`: Prints the version information for pyke, and exits.
 * `-h`, `--help`: Prints a help document.
-* `-c`, `--cache_makefile`: Allows the makefile's __cache__ to be generated. This might speed up complex builds, but they'd hvae to be really complex. Must precede any arguments that are not -v, -h, or -m.
-* `-m`, `--module`: Specifies the module (pyke file), or its directory if the pyke file is called 'make.py', to be run. Must precede any arguments that are not -v, -h, or -c. If no -m argument is given, pyke will look for and run ./make.py.
+* `-m`, `--makefile`: Specifies the module (pyke file), or its directory if the pyke file is called 'make.py', to be run. Must precede any arguments that are not -v, -h, or -c. If no -m argument is given, pyke will look for and run ./make.py.
+* `-n`, `--noconfig`: Specifies that the `pyke-config.json` file adjacent to the makefile should not be loaded.
+* `-c`, `--report-config`: Prints the full combined configuration from all loaded config files, and exits.
 * `-p`, `--phases`: Specifies a subset of phases on which to apply subsequent overrides or actions, if such arguments do not provide their own. Each `-p` encountered resets the subgroup. Option and action arguments that provide their own phases overrule `-p` for that argument, but do not reset it.
 * `-o`, `--override`: Specifies an option override to apply to some or all phases for subsequenet actions. If the option is given as a key-op-value, the override is pushed; if it is only a key (with no operator-value pair) the override is popped.
 * `action`: Arguments given without switches specify actions to be taken on the indicated phases. Any action on any phase which doesn't support it is quietly ignored.
 
 ### Referencing phases
 
 Phases have names (`short name`s), as seen, but also have `full name`s, given as "group.name". For each phase, if the group name is not explicitly set, it is overridden *after the makefile is run* to be the short name of the closest dependency *project phase*. Project phases are thereafter given the short name `project`. This naming scheme allows for subprojects to be referenced by the group name on the CLI. We'll see some examples.
@@ -731,14 +767,15 @@
 * ~/.config/pyke/pyke-config.json
 * <makefile's directory>/pyke-config.json
 
 An example config might look like this:
 
 ```json
 {
+    "include": ["../pyke-config.json"],
     "argument_aliases": {
         "-noc": "-ocolors=none",
         "-bdb": "dbadmin:build",
         "-rdb": [
             "-odbadmin:run_args=\"-logging=TRUE -username=$DBADMIN_UNAME -password=$DBADMIN_PASSWD\"",
             "dbadmin:run"
         ]
@@ -746,20 +783,25 @@
     "action_aliases": {
         "pf": "package_flatpak",
         "vac": "verify_appchecker"
     },
     "default_action": "build",
     "default_arguments": [
         "-v2"
-    ]
+    ],
+    "cache_makefile_module": "true"
 }
 ```
 
 Each can contain the following sections:
 
+### Include files
+
+These are paths to other JSON files which contribute to the configuration. They are loaded before the rest of this file's contents, which can add to or override as described below. Useful if you have distinct configuration for work projects vs. personal projects, or lots of pyke projects which all use the same options. Paths that start with '/' are absolute; otherwise, they are relative to this file's path.
+
 ### Argument aliases
 
 These are convenient shorthands for complex overrides, override-action pairs, or whatever you like. Their values cannot contain other argument alias names, but *can* contain action aliases, and are otherwise exactly as you'd type them on the CLI (except you don't need to enquote things that the shell might interpret). Multiple values must be housed in a list. Each config file adds to the list of argument aliases.
 
 ### Action aliases
 
 Actions can be aliased. These are one-for-one word replacements, and the action values must not be other action aliases, though you *can* have more than one alias for any given action. Each config file adds to the list of action aliases.
@@ -768,14 +810,18 @@
 
 The default action is taken when no action is specified on a CLI. By default, this is set to `report_actions`. The value must not be an alias. Each config file overrides a set default action.
 
 ### Default arguments
 
 Ccontains a list of strings, each of which is a separate command line argument. These can be full names or aliases. They are placed consecutively directly after the -m argument, but before any -o or action arguments, on every invocation of pyke. It is a convenient way to customize the way pyke always works on your project or machine. Each config file appends to the list of default arguments.
 
+### Cache makefile module
+
+Allows the makefile's __cache__ to be generated by python. This might speed up complex builds, but they'd hvae to be really complex.
+
 ## Advanced Topics
 
 ### Adding new phases
 
 Of course, a benefit of a programmatic build system is extension. Building your own Phase classes shold be straightforward. You likely won't have to often.
 
 Say you need a code generator. It must make .c files your project compiles and links with extant source. You can write a custom Phase-derived class to do just this. This gets you into the weeds of `Step` and `Result` classes, and action steps. More help will be provided in the future, but for now, let's just look at the code in demos/custom_phase/custom.py:
@@ -862,15 +908,15 @@
         for file_op in self.files.get_operations('generate'):
             for out in file_op.output_files:
                 source_code = get_source_code(out.path)
                 self.do_step_generate_source(action, dirs[out.path.parent],
                                              source_code, origin_path, out.path)
 ```
 
-There's a bit going on, but it's not terrible. This uses some facilities available in `CFamilyBuildPhase` to clean generated source and the generation directory, as well as making directories for the build. The main work is in generating the source files in an appropriate generation directory.
+There's a bit going on, but it's not terrible. Actions already implemented in `CFamilyBuildPhase` can clean generated source and the generation directory, as well as make directories for the build. The main work here is in generating the source files in an appropriate generation directory.
 
 Integrating this custom phase into your makefile is as simple as making a new instance of the new phase, and setting it as a dependency of the build phase:
 
 ```python
 'Bsic project with custom code generation phase'
 
 # pylint: disable=wrong-import-position
@@ -916,33 +962,34 @@
 
 And that's it. Now the `build` action will first generate the files in the right place if needed, and then build them if needed. The `clean` action will delete the generated files, and the `clean_build_directory` action will not only remove the build, but also the generated source directory.
 
 > A few notes: The above will only generate the source files if they don't exist, or are older than the makefile (which has the source text in it). Also, the gen diretory is based on `gen_anchor` (by way of `build_anchor`), which is necessary for any generated files to be built in the right place if you change `gen_anchor`'s value.
 
 #### Adding new actions
 
-To add a new action to a custom phase, simply add a method to the phase class. For example, to add an action called "deploy", write a method like so:
+To add a new action to a custom phase, simply add a method to the phase class. For example, to add an action called "deploy", write a phase method like so:
 
 ```python
+    ...
     def do_action_deploy(self, action: Action) -> ResultCode:
         ...
 ```
 (You'll want to import Action and ResultCode from pyke if you want the annotations.) That's all you need to do for the method to be called on an action, since actions' names are just strings, and pyke reflects on method names to find a phase that can handle the action. Of course, implmenting actions is more involved, as you can see above.
 
 ### Adding new build kinds
 
-Adding new build kinds is straightforward if you're just trying to customize the system build commands. There are currently three that depend on the build kind: `debug_level`; `optimization`; and `flags`. For POSIX tools, these correspond to the `-g{debug_level}`, `-O{optimization}`, and `{flags}` of any definition. If you wanted a custom kind called "smallest", imply provide the following overrides, with perhaps these values:
+Adding new build kinds is straightforward if you're just trying to customize the system build commands. There are currently three that depend on the build kind: `debug_level`; `optimization`; and `flags`. For POSIX tools, these correspond to the `-g{debug_level}`, `-O{optimization}`, and `{flags}` of any definition. If you wanted a custom kind called "smallest", simply provide the following overrides, with perhaps these values:
 
 ```
 'gnuclang_smallest_debug_level': '0',
 'gnuclang_smallest_optimization': 's',
 'gnuclang_smallest_flags': ['-DNDEBUG'],
 ```
 
-When selecting the build kind with `-o kind=smallest`, these overrides should be selected for the build.
+When selecting the build kind with `-o kind=smallest`, these overrides will be selected for the build.
 
 ### Setting colors
 
 The colorful output can be helpful, but not if you're on an incapable terminal, or just don't like them or want them at all. You can select a color palette:
 
 ```
 pyke -o colors=none build
```

### Comparing `pyke_build-0.1.0/src/pyke_build.egg-info/SOURCES.txt` & `pyke_build-0.2.0/src/pyke_build.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 pyrightconfig.json
 readme_helper.py
 requierments.txt
 setup.py
 test.sh
 demos/custom_phase/custom.py
 demos/custom_phase/make.py
+demos/custom_phase/pyke-config.json
+demos/custom_phase/pyke-subconfig.json
 demos/custom_phase/include/abc.h
 demos/custom_phase/src/a.c
 demos/custom_phase/src/b.c
 demos/custom_phase/src/c.c
 demos/custom_phase/src/main.c
 demos/custom_phase/src/gen/d.c
 demos/custom_phase/src/gen/e.c
@@ -33,24 +35,26 @@
 demos/multi_make/exp/b.c
 demos/multi_make/include/abc.h
 demos/multi_make/src/a.c
 demos/multi_make/src/b.c
 demos/multi_make/src/c.c
 demos/multi_make/src/main.c
 demos/multi_shared_objects/make.py
+demos/multi_shared_objects/a-star/make.py
+demos/multi_shared_objects/a-star/src/aaa.c
+demos/multi_shared_objects/a-star/src/aas.c
+demos/multi_shared_objects/a-star/src/asa.c
+demos/multi_shared_objects/a-star/src/ass.c
 demos/multi_shared_objects/include/multi.h
-demos/multi_shared_objects/src/aaa.c
-demos/multi_shared_objects/src/aas.c
-demos/multi_shared_objects/src/asa.c
-demos/multi_shared_objects/src/ass.c
+demos/multi_shared_objects/s-star/make.py
+demos/multi_shared_objects/s-star/src/saa.c
+demos/multi_shared_objects/s-star/src/sas.c
+demos/multi_shared_objects/s-star/src/ssa.c
+demos/multi_shared_objects/s-star/src/sss.c
 demos/multi_shared_objects/src/main.c
-demos/multi_shared_objects/src/saa.c
-demos/multi_shared_objects/src/sas.c
-demos/multi_shared_objects/src/ssa.c
-demos/multi_shared_objects/src/sss.c
 demos/simple_app/make.py
 demos/simple_app/include/abc.h
 demos/simple_app/src/a.c
 demos/simple_app/src/b.c
 demos/simple_app/src/c.c
 demos/simple_app/src/main.c
 demos/simple_lib/make.py
@@ -65,16 +69,18 @@
 demos/simple_so/src/b.c
 demos/simple_so/src/c.c
 demos/simple_so/src/main.c
 src/pyke/__init__.py
 src/pyke/_version.py
 src/pyke/action.py
 src/pyke/ansi.py
+src/pyke/config.py
 src/pyke/options.py
 src/pyke/options_parser.py
+src/pyke/pyke-config.json
 src/pyke/pyke.py
 src/pyke/utilities.py
 src/pyke/phases/__init__.py
 src/pyke/phases/archive.py
 src/pyke/phases/c_family_build.py
 src/pyke/phases/command_phase.py
 src/pyke/phases/compile.py
```

### Comparing `pyke_build-0.1.0/test.sh` & `pyke_build-0.2.0/test.sh`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/tests/test_options.py` & `pyke_build-0.2.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pyke_build-0.1.0/tests/test_options_parser.py` & `pyke_build-0.2.0/tests/test_options_parser.py`

 * *Files identical despite different names*

