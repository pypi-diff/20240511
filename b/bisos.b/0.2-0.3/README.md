# Comparing `tmp/bisos.b-0.2.tar.gz` & `tmp/bisos.b-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bisos.b-0.2.tar", last modified: Wed Feb 21 23:58:31 2024, max compression
+gzip compressed data, was "bisos.b-0.3.tar", last modified: Sat May 11 04:59:57 2024, max compression
```

## Comparing `bisos.b-0.2.tar` & `bisos.b-0.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-21 23:58:31.889732 bisos.b-0.2/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2022-06-29 18:37:11.000000 bisos.b-0.2/MANIFEST.in
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1451 2024-02-21 23:58:31.889732 bisos.b-0.2/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      588 2024-02-21 23:58:31.000000 bisos.b-0.2/README.rst
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      149 2022-06-29 18:37:11.000000 bisos.b-0.2/TITLE.txt
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-21 23:58:31.885733 bisos.b-0.2/bin/
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    19819 2022-09-05 19:26:17.000000 bisos.b-0.2/bin/csExamples.cs
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-21 23:58:31.885733 bisos.b-0.2/bisos/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2022-06-29 18:37:11.000000 bisos.b-0.2/bisos/__init__.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-21 23:58:31.889732 bisos.b-0.2/bisos/b/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1737 2024-01-31 20:57:45.000000 bisos.b-0.2/bisos/b/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    21226 2022-09-25 07:34:23.000000 bisos.b-0.2/bisos/b/ast.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-21 23:58:31.889732 bisos.b-0.2/bisos/b/b_io/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      937 2022-09-24 22:01:52.000000 bisos.b-0.2/bisos/b/b_io/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     6660 2024-02-10 04:42:43.000000 bisos.b-0.2/bisos/b/b_io/ann.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    20147 2022-09-25 23:54:49.000000 bisos.b-0.2/bisos/b/b_io/eh.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     5690 2022-09-24 22:01:52.000000 bisos.b-0.2/bisos/b/b_io/io.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    19072 2022-09-25 22:24:52.000000 bisos.b-0.2/bisos/b/b_io/k1-eh.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    18680 2022-09-29 22:51:34.000000 bisos.b-0.2/bisos/b/b_io/log.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     6469 2022-09-24 22:01:52.000000 bisos.b-0.2/bisos/b/b_io/out.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     5458 2022-09-24 22:01:52.000000 bisos.b-0.2/bisos/b/b_io/stderr.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     5484 2022-09-24 22:01:52.000000 bisos.b-0.2/bisos/b/b_io/stdin.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     5164 2024-02-10 04:42:43.000000 bisos.b-0.2/bisos/b/b_io/stdout.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     7392 2022-09-25 22:17:29.000000 bisos.b-0.2/bisos/b/b_io/tm.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    14148 2022-09-24 22:27:10.000000 bisos.b-0.2/bisos/b/clsMethod_csu.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     4866 2022-09-27 05:11:31.000000 bisos.b-0.2/bisos/b/comment.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-21 23:58:31.889732 bisos.b-0.2/bisos/b/cs/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      810 2022-09-24 22:06:28.000000 bisos.b-0.2/bisos/b/cs/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    15312 2022-09-24 22:06:28.000000 bisos.b-0.2/bisos/b/cs/arg.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    78494 2024-02-08 06:22:30.000000 bisos.b-0.2/bisos/b/cs/cs.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    28633 2024-02-03 20:08:13.000000 bisos.b-0.2/bisos/b/cs/examples.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    12803 2024-01-22 02:29:29.000000 bisos.b-0.2/bisos/b/cs/globalContext.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    41249 2022-09-24 22:06:28.000000 bisos.b-0.2/bisos/b/cs/inCmnd.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    73247 2024-02-09 01:54:18.000000 bisos.b-0.2/bisos/b/cs/k1-ro.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    11210 2022-11-26 05:16:19.000000 bisos.b-0.2/bisos/b/cs/main.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    21551 2022-09-24 22:06:28.000000 bisos.b-0.2/bisos/b/cs/param.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    73950 2024-02-10 01:09:33.000000 bisos.b-0.2/bisos/b/cs/ro.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     9270 2024-01-22 22:24:25.000000 bisos.b-0.2/bisos/b/cs/rpyc.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    12903 2022-09-24 22:06:28.000000 bisos.b-0.2/bisos/b/cs/rtInvoker.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    12636 2022-09-24 22:06:28.000000 bisos.b-0.2/bisos/b/cs/runArgs.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    17615 2022-09-25 17:31:18.000000 bisos.b-0.2/bisos/b/cs/track.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    11057 2022-09-24 22:27:10.000000 bisos.b-0.2/bisos/b/dir.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     7470 2022-09-24 22:27:10.000000 bisos.b-0.2/bisos/b/exception.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    42680 2024-02-01 19:53:47.000000 bisos.b-0.2/bisos/b/fp.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    53827 2024-02-04 06:46:27.000000 bisos.b-0.2/bisos/b/fpCls.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     8338 2022-10-04 19:54:17.000000 bisos.b-0.2/bisos/b/fpath.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    10387 2024-02-04 06:51:44.000000 bisos.b-0.2/bisos/b/fto.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     8464 2022-09-24 22:27:10.000000 bisos.b-0.2/bisos/b/fv.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     6672 2022-10-02 20:47:08.000000 bisos.b-0.2/bisos/b/importFile.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     9887 2022-09-29 19:54:59.000000 bisos.b-0.2/bisos/b/niche.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    15908 2024-01-31 20:59:15.000000 bisos.b-0.2/bisos/b/op.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    15728 2022-12-07 20:03:07.000000 bisos.b-0.2/bisos/b/pyRunAs.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    22794 2024-01-19 18:26:36.000000 bisos.b-0.2/bisos/b/subProc.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     7242 2022-09-24 22:27:10.000000 bisos.b-0.2/bisos/b/types.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-21 23:58:31.885733 bisos.b-0.2/bisos.b.egg-info/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1451 2024-02-21 23:58:31.000000 bisos.b-0.2/bisos.b.egg-info/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1147 2024-02-21 23:58:31.000000 bisos.b-0.2/bisos.b.egg-info/SOURCES.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-02-21 23:58:31.000000 bisos.b-0.2/bisos.b.egg-info/dependency_links.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-02-21 23:58:31.000000 bisos.b-0.2/bisos.b.egg-info/namespace_packages.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-02-21 23:58:31.000000 bisos.b-0.2/bisos.b.egg-info/not-zip-safe
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2024-02-21 23:58:31.000000 bisos.b-0.2/bisos.b.egg-info/requires.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-02-21 23:58:31.000000 bisos.b-0.2/bisos.b.egg-info/top_level.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-02-21 23:58:31.000000 bisos.b-0.2/lh-agpl3-LICENSE.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-02-21 23:58:31.889732 bisos.b-0.2/setup.cfg
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1882 2024-02-21 23:57:29.000000 bisos.b-0.2/setup.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:59:57.487445 bisos.b-0.3/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2022-06-29 18:37:11.000000 bisos.b-0.3/MANIFEST.in
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1451 2024-05-11 04:59:57.487445 bisos.b-0.3/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      588 2024-05-11 04:59:56.000000 bisos.b-0.3/README.rst
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      149 2022-06-29 18:37:11.000000 bisos.b-0.3/TITLE.txt
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:59:57.475445 bisos.b-0.3/bin/
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    19819 2022-09-05 19:26:17.000000 bisos.b-0.3/bin/csExamples.cs
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:59:57.479445 bisos.b-0.3/bisos/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2022-06-29 18:37:11.000000 bisos.b-0.3/bisos/__init__.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:59:57.483445 bisos.b-0.3/bisos/b/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1737 2024-01-31 20:57:45.000000 bisos.b-0.3/bisos/b/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    21226 2022-09-25 07:34:23.000000 bisos.b-0.3/bisos/b/ast.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:59:57.483445 bisos.b-0.3/bisos/b/b_io/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      937 2022-09-24 22:01:52.000000 bisos.b-0.3/bisos/b/b_io/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     6660 2024-02-10 04:42:43.000000 bisos.b-0.3/bisos/b/b_io/ann.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    20187 2024-05-11 04:58:53.000000 bisos.b-0.3/bisos/b/b_io/eh.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5690 2022-09-24 22:01:52.000000 bisos.b-0.3/bisos/b/b_io/io.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    19072 2022-09-25 22:24:52.000000 bisos.b-0.3/bisos/b/b_io/k1-eh.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    18680 2022-09-29 22:51:34.000000 bisos.b-0.3/bisos/b/b_io/log.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     6469 2022-09-24 22:01:52.000000 bisos.b-0.3/bisos/b/b_io/out.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5458 2022-09-24 22:01:52.000000 bisos.b-0.3/bisos/b/b_io/stderr.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5484 2022-09-24 22:01:52.000000 bisos.b-0.3/bisos/b/b_io/stdin.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     5164 2024-02-10 04:42:43.000000 bisos.b-0.3/bisos/b/b_io/stdout.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7392 2022-09-25 22:17:29.000000 bisos.b-0.3/bisos/b/b_io/tm.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    14148 2022-09-24 22:27:10.000000 bisos.b-0.3/bisos/b/clsMethod_csu.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     4866 2022-09-27 05:11:31.000000 bisos.b-0.3/bisos/b/comment.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:59:57.487445 bisos.b-0.3/bisos/b/cs/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      810 2022-09-24 22:06:28.000000 bisos.b-0.3/bisos/b/cs/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    15312 2022-09-24 22:06:28.000000 bisos.b-0.3/bisos/b/cs/arg.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    81313 2024-05-11 04:58:53.000000 bisos.b-0.3/bisos/b/cs/cs.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    29593 2024-05-11 04:58:53.000000 bisos.b-0.3/bisos/b/cs/examples.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    12803 2024-01-22 02:29:29.000000 bisos.b-0.3/bisos/b/cs/globalContext.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    41249 2022-09-24 22:06:28.000000 bisos.b-0.3/bisos/b/cs/inCmnd.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    73247 2024-02-09 01:54:18.000000 bisos.b-0.3/bisos/b/cs/k1-ro.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    11210 2022-11-26 05:16:19.000000 bisos.b-0.3/bisos/b/cs/main.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    21929 2024-05-11 04:58:53.000000 bisos.b-0.3/bisos/b/cs/param.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    97094 2024-05-11 04:58:53.000000 bisos.b-0.3/bisos/b/cs/ro.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     9270 2024-01-22 22:24:25.000000 bisos.b-0.3/bisos/b/cs/rpyc.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    12903 2022-09-24 22:06:28.000000 bisos.b-0.3/bisos/b/cs/rtInvoker.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    12636 2022-09-24 22:06:28.000000 bisos.b-0.3/bisos/b/cs/runArgs.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    17615 2022-09-25 17:31:18.000000 bisos.b-0.3/bisos/b/cs/track.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    11057 2022-09-24 22:27:10.000000 bisos.b-0.3/bisos/b/dir.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7470 2022-09-24 22:27:10.000000 bisos.b-0.3/bisos/b/exception.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    42680 2024-02-01 19:53:47.000000 bisos.b-0.3/bisos/b/fp.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    54004 2024-05-11 04:58:53.000000 bisos.b-0.3/bisos/b/fpCls.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     8338 2022-10-04 19:54:17.000000 bisos.b-0.3/bisos/b/fpath.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    10387 2024-02-04 06:51:44.000000 bisos.b-0.3/bisos/b/fto.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     8464 2022-09-24 22:27:10.000000 bisos.b-0.3/bisos/b/fv.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     6672 2022-10-02 20:47:08.000000 bisos.b-0.3/bisos/b/importFile.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     9887 2022-09-29 19:54:59.000000 bisos.b-0.3/bisos/b/niche.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    15955 2024-05-11 04:58:53.000000 bisos.b-0.3/bisos/b/op.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    15728 2022-12-07 20:03:07.000000 bisos.b-0.3/bisos/b/pyRunAs.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    22794 2024-01-19 18:26:36.000000 bisos.b-0.3/bisos/b/subProc.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     7242 2022-09-24 22:27:10.000000 bisos.b-0.3/bisos/b/types.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:59:57.479445 bisos.b-0.3/bisos.b.egg-info/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1451 2024-05-11 04:59:57.000000 bisos.b-0.3/bisos.b.egg-info/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1147 2024-05-11 04:59:57.000000 bisos.b-0.3/bisos.b.egg-info/SOURCES.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:59:57.000000 bisos.b-0.3/bisos.b.egg-info/dependency_links.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-11 04:59:57.000000 bisos.b-0.3/bisos.b.egg-info/namespace_packages.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:59:57.000000 bisos.b-0.3/bisos.b.egg-info/not-zip-safe
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       25 2024-05-11 04:59:57.000000 bisos.b-0.3/bisos.b.egg-info/requires.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-11 04:59:57.000000 bisos.b-0.3/bisos.b.egg-info/top_level.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-11 04:59:56.000000 bisos.b-0.3/lh-agpl3-LICENSE.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-11 04:59:57.487445 bisos.b-0.3/setup.cfg
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1916 2024-05-11 04:58:53.000000 bisos.b-0.3/setup.py
```

### Comparing `bisos.b-0.2/PKG-INFO` & `bisos.b-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.b
-Version: 0.2
+Version: 0.3
 Summary: bisos.bx-bases: python scripts (Interactive Command Modules -- ICM) are used for bootstrapping the BISOS (ByStar Internet Services OS) environment.
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
```

### Comparing `bisos.b-0.2/README.rst` & `bisos.b-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bin/csExamples.cs` & `bisos.b-0.3/bin/csExamples.cs`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/__init__.py` & `bisos.b-0.3/bisos/b/__init__.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/ast.py` & `bisos.b-0.3/bisos/b/ast.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/b_io/__init__.py` & `bisos.b-0.3/bisos/b/b_io/__init__.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/b_io/ann.py` & `bisos.b-0.3/bisos/b/b_io/ann.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/b_io/eh.py` & `bisos.b-0.3/bisos/b/b_io/eh.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,22 +456,21 @@
 ####+END:
         outcome,
 ):
     """ #+begin_org
 ** [[elisp:(org-cycle)][| *DocStr | ]
     #+end_org """
 
-    print((
-        "io.eh.badOutcome: InvokedBy {invokerName}, Operation Failed: Stdcmnd={stdcmnd} Error={status} -- {errInfo}".
-        format(invokerName=outcome.invokerName,
+    print("io.eh.badOutcome: InvokedBy {invokerName}, Operation Failed: Stdcmnd={stdcmnd} Error={status} -- {errInfo}".
+           format(invokerName=outcome.invokerName,
                stdcmnd=outcome.stdcmnd,
                status=outcome.error,
                errInfo=outcome.errInfo,
-        )))
-    print(('io.eh.: ' + ' -- ' + b.ast.stackFrameInfoGet(2) ))
+                  ),  file=sys.stderr)   
+    print(('io.eh.: ' + ' -- ' + b.ast.stackFrameInfoGet(2) ), file=sys.stderr)
 
     return outcome
 
 ####+BEGIN: b:py3:cs:func/typing :funcName "badLastOutcome" :funcType "extTyped" :deco ""
 """ #+begin_org
 *  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-extTyped [[elisp:(outline-show-subtree+toggle)][||]] /badLastOutcome/   [[elisp:(org-cycle)][| ]]
 #+end_org """
```

### Comparing `bisos.b-0.2/bisos/b/b_io/io.py` & `bisos.b-0.3/bisos/b/b_io/io.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/b_io/k1-eh.py` & `bisos.b-0.3/bisos/b/b_io/k1-eh.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/b_io/log.py` & `bisos.b-0.3/bisos/b/b_io/log.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/b_io/out.py` & `bisos.b-0.3/bisos/b/b_io/out.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/b_io/stderr.py` & `bisos.b-0.3/bisos/b/b_io/stderr.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/b_io/stdin.py` & `bisos.b-0.3/bisos/b/b_io/stdin.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/b_io/stdout.py` & `bisos.b-0.3/bisos/b/b_io/stdout.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/b_io/tm.py` & `bisos.b-0.3/bisos/b/b_io/tm.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/clsMethod_csu.py` & `bisos.b-0.3/bisos/b/clsMethod_csu.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/comment.py` & `bisos.b-0.3/bisos/b/comment.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/cs/__init__.py` & `bisos.b-0.3/bisos/b/cs/__init__.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/cs/arg.py` & `bisos.b-0.3/bisos/b/cs/arg.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/cs/cs.py` & `bisos.b-0.3/bisos/b/cs/cs.py`

 * *Files 2% similar despite different names*

```diff
@@ -754,14 +754,91 @@
             cmndOutcome=cmndOutcome,
             **kwArgs,
         )
 
         return outcome
 
 
+####+BEGIN: b:py3:cs:method/typing :methodName "pyRoCmnd" :methodType "eType"  :deco "default"
+    """ #+begin_org
+**  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  Mtd-T-eType [[elisp:(outline-show-subtree+toggle)][||]] /pyRoCmnd/  deco=default  [[elisp:(org-cycle)][| ]]
+    #+end_org """
+    @cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+    def pyRoCmnd(
+####+END:
+            self,
+            rtInv=None,
+            cmndOutcome=None,
+            roSapPath=None,
+            rosmu=None,
+            perfName=None,
+            svcName=None,
+            **kwArgs,
+    )  -> b.op.Outcome:
+        """ #+begin_org
+** [[elisp:(org-cycle)][| DocStr| ]]  Calls Cmnd, Returns Outcome
+pyCmnd invokactions are non-interactive
+        #+end_org """
+
+        if rtInv is None:
+            rtInv = cs.RtInvoker.new_py()
+        if cmndOutcome is None:
+            cmndOutcome = b.op.Outcome()
+
+        cmndClass = self.__class__
+
+        if roSapPath is None:
+            roSapPath = cs.ro.SapBase_FPs.perfNameToRoSapPath(perfName, rosmu=rosmu, svcName=svcName)
+
+        print(roSapPath)
+        rpycInvResult =  cs.ro.roInvokeCmndAtSap(
+            roSapPath,
+            rtInv,
+            cmndOutcome,
+            cmndClass,
+            ** kwArgs,
+        )
+
+        return cmndOutcome
+
+####+BEGIN: b:py3:cs:method/typing :methodName "pyRoWCmnd" :methodType "eType"  :deco "default"
+    """ #+begin_org
+**  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  Mtd-T-eType [[elisp:(outline-show-subtree+toggle)][||]] /pyRoWCmnd/  deco=default  [[elisp:(org-cycle)][| ]]
+    #+end_org """
+    @cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+    def pyRoWCmnd(
+####+END:
+            self,
+            cmndOutcome,
+            roSapPath=None,
+            rosmu=None,
+            perfName=None,
+            svcName=None,
+            **kwArgs,
+    )  -> b.op.Outcome:
+        """ #+begin_org
+** [[elisp:(org-cycle)][| DocStr| ]]  A Wrapped Cmnd, Calls Cmnd, Returns Outcome
+pyCmnd invokactions are non-interactive
+        #+end_org """
+
+        rtInv = cs.RtInvoker.new_py()
+
+        outcome = self.pyRoCmnd(
+            rtInv=rtInv,
+            cmndOutcome=cmndOutcome,
+            roSapPath=roSapPath,
+            rosmu=rosmu,
+            perfName=perfName,
+            svcName=svcName,
+            **kwArgs,
+        )
+
+        return outcome
+
+
 
 
 ####+BEGIN: blee:bxPanel:foldingSection :outLevel 0 :sep nil :title "CS Output" :anchor ""  :extraInfo "Perhaps It Belongs In The IO Package"
 """ #+begin_org
 *  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*     [[elisp:(outline-show-subtree+toggle)][| _CS Output_: |]]  Perhaps It Belongs In The IO Package  [[elisp:(org-shifttab)][<)]] E|
 #+end_org """
 ####+END:
@@ -1437,14 +1514,18 @@
     #+end_org """
 
     # print(G.__class__._outcomeReportCmnd)
 
     if G.__class__._outcomeReportCmnd == False:
         return
 
+    if cmndOutcome is  None:
+        sys.stderr.write("Bad Cmnd Return -- No cmndOutcome\n")
+        return
+
     if cmndOutcome.results is not  None:
         sys.stdout.write(f"{cmndOutcome.results}\n")
     else:
         sys.stderr.write("Cmnd -- No Results\n")
 
 
 ####+BEGIN: b:py3:cs:func/typing :funcName "invOutcomeReportRo" :funcType "extTyped" :deco ""
```

### Comparing `bisos.b-0.2/bisos/b/cs/examples.py` & `bisos.b-0.3/bisos/b/cs/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,23 +143,46 @@
 
     print(( G_myName + " -i commonExamples" + "    # Help, Model, icmOptionsExample"))
     print(( G_myName + " -i describe" + " |" + " emlVisit"))
     print(( G_myName + " -i examples" + " |" + " icmToEmlVisit"))
     print(( G_myName + " -i visit"))
     print(( """emlVisit -v -n showRun -i gotoPanel """ + G_myFullName))
 
-    menuChapter('/Remote Operations -- Performer And Invoker/')
+    if cs.ro.csMuIsDirect() is True:
+        menuChapter('/Remote Operations -- Performer And Invoker/')
 
-    print(f"""csRo-manage.cs --perfName="localhost" --rosmu="{G_myName}"  -i ro_sapCreate""")
-    print(f"""{G_myName} --perfName="localhost" -i csPerformer  & # in background Start rpyc CS Service""")
-    print(f"""csRo-manage.cs --perfName="localhost" --rosmu="{G_myName}"  -i ro_fps list""")
-    print(f"""{G_myName}  --perfName="localhost" -i examples""")
+        # print(f"""csRo-manage.cs --perfName="localhost" --rosmu="{G_myName}"  -i ro_sapCreate""")
+        # print(f"""{G_myName} --perfName="localhost" -i csPerformer  & # in background Start rpyc CS Service""")
+        # print(f"""csRo-manage.cs --perfName="localhost" --rosmu="{G_myName}"  -i ro_fps list""")
+        # print(f"""{G_myName}  --perfName="localhost" -i examples""")
+
+        print(( G_myName + " -i roEnable" + "    # Create Symlinks For roPerf- and roInv-"))
+        print(( "roPerf-" + G_myName + "    # Remote Operations Performer"))
+        print(( "roInv-" + G_myName  + "    # Remote Operations Invoker"))
+
+    elif cs.ro.csMuIsPerformer() is True:
+        menuChapter('/Direct Commands and roInvoker/')
+        directName = cs.ro.csMuDirectName()
+        invokerName = cs.ro.csMuInvokerName()
+        print(( directName + "    # Direct Commands"))
+        print(( invokerName + "   # Remote Operations Invoker"))
+
+    elif cs.ro.csMuIsInvoker() is True:
+        menuChapter('/Direct Commands and roInvoker/')
+        directName = cs.ro.csMuDirectName()
+        performerName = cs.ro.csMuPerformerName()
+        print(( directName + "    # Direct Commands"))
+        print(( performerName + "   # Remote Operations Performer"))
 
-    menuChapter('*ICM Blee Player Invokations*')
-    b_io.ann.write("icmPlayer.sh -h -v -n showRun -i grouped {G_myName}".format(G_myName=G_myName))
+    else:
+        oops()
+
+
+    # menuChapter('*ICM Blee Player Invokations*')
+    # b_io.ann.write("icmPlayer.sh -h -v -n showRun -i grouped {G_myName}".format(G_myName=G_myName))
 
 ####+BEGIN: b:py3:cs:func/typing :funcName "devExamples" :funcType "extTyped" :deco "track"
 """ #+begin_org
 *  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-extTyped [[elisp:(outline-show-subtree+toggle)][||]] /devExamples/  deco=track  [[elisp:(org-cycle)][| ]]
 #+end_org """
 @cs.track(fnLoc=True, fnEntry=True, fnExit=True)
 def devExamples(
@@ -479,15 +502,15 @@
 def cmndEnter(
 ####+END:
         name: str,
         pars: collections.OrderedDict[str, str]=collections.OrderedDict(),
         args: str="",
         verb: list[str]=[],
         comment: str='none',
-        csWrapper: str='',
+        wrapper: str='',
         csName: str='',
 ) -> None:
     """ #+begin_org
 ** [[elisp:(org-cycle)][| *DocStr | ] Constructs cmndLine based on positional args and specific other args. Calls ~menuItemInsert~.
     For services, it looks at invModel and roSap.
     #+end_org """
 
@@ -514,15 +537,15 @@
         verb = ['none']
 
     for eachVerbosity in verb:
         menuItemInsert(
             commandLine=cmndLine,
             verbosity=eachVerbosity,
             comment=comment,
-            icmWrapper=csWrapper,
+            icmWrapper=wrapper,
             icmName=csName,
         )
 
 
 
 
 ####+BEGIN: b:py3:cs:func/typing :funcName "cmndInsert" :funcType "extTyped" :deco "track"
```

### Comparing `bisos.b-0.2/bisos/b/cs/globalContext.py` & `bisos.b-0.3/bisos/b/cs/globalContext.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/cs/inCmnd.py` & `bisos.b-0.3/bisos/b/cs/inCmnd.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/cs/k1-ro.py` & `bisos.b-0.3/bisos/b/cs/k1-ro.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/cs/main.py` & `bisos.b-0.3/bisos/b/cs/main.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/cs/param.py` & `bisos.b-0.3/bisos/b/cs/param.py`

 * *Files 1% similar despite different names*

```diff
@@ -468,14 +468,27 @@
         parScope=CmndParamScope.TargetParam,
         #argparseShortOpt='-v',
         argparseLongOpt='--logFile',
         )
 
     icmParams.parDictAdd(
         parAction='store',
+        parName='sectionTitle',
+        parDescription='For use as section title of examples',
+        parDataType=None,
+        parDefault=None,
+        parMetavar='ARG',
+        parChoices=[],
+        parScope=CmndParamScope.TargetParam,
+        #argparseShortOpt='-v',
+        argparseLongOpt='--sectionTitle',
+        )
+
+    icmParams.parDictAdd(
+        parAction='store',
         parName='logFileLevel',
         parDescription='Specifies destination LogFile for this run',
         parDataType=None,
         parDefault=None,
         parMetavar='ARG',
         parChoices=[],
         parScope=CmndParamScope.TargetParam,
```

### Comparing `bisos.b-0.2/bisos/b/cs/ro.py` & `bisos.b-0.3/bisos/b/cs/ro.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """ #+begin_org
 * [[elisp:(org-cycle)][| /Control Parameters Of This File/ |]] :: dblk ctrls classifications=cs-u
 #+BEGIN_SRC emacs-lisp
 (setq-local b:dblockControls t) ; (setq-local b:dblockControls nil)
 (put 'b:dblockControls 'py3:cs:Classification "cs-u") ; one of cs-mu, cs-u, cs-lib, b-lib, pyLibPure
 #+END_SRC
 #+RESULTS:
-: cs-mu
+: cs-u
 #+end_org """
 ####+END:
 
 ####+BEGIN: b:prog:file/proclamations :outLevel 1
 """ #+begin_org
 * *[[elisp:(org-cycle)][| Proclamations |]]* :: Libre-Halaal Software --- Part Of Blee ---  Poly-COMEEGA Format.
 ** This is Libre-Halaal Software. © Libre-Halaal Foundation. Subject to AGPL.
@@ -77,14 +77,15 @@
 ####+BEGIN: b:py3:cs:framework/imports :basedOn "classification"
 """ #+begin_org
 ** Imports Based On Classification=cs-u
 #+end_org """
 from bisos import b
 from bisos.b import cs
 from bisos.b import b_io
+from bisos.common import csParam
 
 import collections
 ####+END:
 
 import pathlib
 import __main__
 import os
@@ -1116,45 +1117,145 @@
             #parScope=icm.ICM_ParamScope.TargetParam,  # type: ignore
             argparseShortOpt=None,
             argparseLongOpt='--accessControl',
         )
 
         return icmParams
 
+
 ####+BEGIN: b:py3:cs:method/typing :methodName "svcNameToRoSapPath" :deco "staticmethod"
     """ #+begin_org
 **  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  Mtd-T-     [[elisp:(outline-show-subtree+toggle)][||]] /svcNameToRoSapPath/  deco=staticmethod  [[elisp:(org-cycle)][| ]]
     #+end_org """
     @staticmethod
     def svcNameToRoSapPath(
 ####+END:
             svcName,
             rosmu=None,
             rosmuSel=None,
+            perfName=None,
             perfModel=None,
     ):
         """."""
 
         if rosmu == None:
             rosmu=cs.G.icmMyName()
 
         if rosmuSel == None:
             rosmuSel="default"
 
         if perfModel == None:
             perfModel="rpyc"
 
-        perfName = svcName
+        if perfName is None:
+            perfNames = __class__.fromRosmuSapPathGetPerfNames(rosmu)
+            perfName = perfNames[0].name
 
         sapBaseFps = b.pattern.sameInstance(SapBase_FPs, rosmu=rosmu, svcName=svcName, perfName=perfName, perfModel=perfModel, rosmuSel=rosmuSel)
 
         roSapPath = sapBaseFps.fps_absBasePath()
 
         return roSapPath
 
+
+####+BEGIN: b:py3:cs:method/typing :methodName "perfNameToRoSapPath" :deco "staticmethod"
+    """ #+begin_org
+**  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  Mtd-T-     [[elisp:(outline-show-subtree+toggle)][||]] /perfNameToRoSapPath/  deco=staticmethod  [[elisp:(org-cycle)][| ]]
+    #+end_org """
+    @staticmethod
+    def perfNameToRoSapPath(
+####+END:
+            perfName,
+            svcName=None,
+            rosmu=None,
+            rosmuSel=None,
+            perfModel=None,
+    ):
+        """."""
+
+        if rosmu == None:
+            rosmu=cs.G.icmMyName()
+
+        if rosmuSel == None:
+            rosmuSel="default"
+
+        if perfModel == None:
+            perfModel="rpyc"
+
+        if svcName is None:
+            svcNames = __class__.fromRosmuSapPathGetSvcNames(rosmu)
+            svcName = svcNames[0].name
+
+        sapBaseFps = b.pattern.sameInstance(SapBase_FPs, rosmu=rosmu, svcName=svcName, perfName=perfName, perfModel=perfModel, rosmuSel=rosmuSel)
+        roSapPath = sapBaseFps.fps_absBasePath()
+
+        return roSapPath
+
+####+BEGIN: b:py3:cs:method/typing :methodName "rosmuSapPath_obtain" :deco "staticmethod"
+    """ #+begin_org
+**  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  Mtd-T-     [[elisp:(outline-show-subtree+toggle)][||]] /rosmuSapPath_obtain/  deco=staticmethod  [[elisp:(org-cycle)][| ]]
+    #+end_org """
+    @staticmethod
+    def rosmuSapPath_obtain(
+####+END:
+            rosmu=None,
+    ) -> pathlib.Path:
+
+        if rosmu == None:
+            rosmu=cs.G.icmMyName()
+
+        return (
+            pathlib.Path(
+                os.path.join(
+                    "/bisos/var/cs/ro/sap",
+                    rosmu,
+                )
+            )
+        )
+
+####+BEGIN: b:py3:cs:method/typing :methodName "fromRosmuSapPathGetPerfNames" :deco "staticmethod"
+    """ #+begin_org
+**  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  Mtd-T-     [[elisp:(outline-show-subtree+toggle)][||]] /fromRosmuSapPathGetPerfNames/  deco=staticmethod  [[elisp:(org-cycle)][| ]]
+    #+end_org """
+    @staticmethod
+    def fromRosmuSapPathGetPerfNames(
+####+END:
+            rosmu=None,
+    ) -> list[pathlib.Path]:
+
+        if rosmu == None:
+            rosmu=cs.G.icmMyName()
+
+        rosmuPath = __class__.rosmuSapPath_obtain(rosmu)
+        perfNames = rosmuPath.iterdir()
+        return  list(perfNames)
+
+####+BEGIN: b:py3:cs:method/typing :methodName "fromRosmuSapPathGetSvcNames" :deco "staticmethod"
+    """ #+begin_org
+**  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  Mtd-T-     [[elisp:(outline-show-subtree+toggle)][||]] /fromRosmuSapPathGetSvcNames/  deco=staticmethod  [[elisp:(org-cycle)][| ]]
+    #+end_org """
+    @staticmethod
+    def fromRosmuSapPathGetSvcNames(
+####+END:
+            rosmu=None,
+    ) -> list[pathlib.Path]:
+
+        if rosmu == None:
+            rosmu=cs.G.icmMyName()
+
+        perfNames = __class__.fromRosmuSapPathGetPerfNames(rosmu)
+
+        svcNames = []
+
+        for eachPerfName in perfNames:
+            theseSvcNames = eachPerfName.iterdir()
+            svcNames = svcNames + list(theseSvcNames)
+
+        return list(svcNames)
+
 ####+BEGIN: b:py3:cs:method/typing :methodName "fps_manifestDict" :deco ""
     """ #+begin_org
 **  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  Mtd-T-     [[elisp:(outline-show-subtree+toggle)][||]] /fps_manifestDict/ deco=    [[elisp:(org-cycle)][| ]]
     #+end_org """
     def fps_manifestDictBuild(
 ####+END:
             self,
@@ -1238,17 +1339,17 @@
            self,
     ) -> pathlib.Path:
         return (
             pathlib.Path(
                 os.path.join(
                     "/bisos/var/cs/ro/sap",
                     self.rosmu,
+                    self.perfName,
                     self.svcName,
                     self.perfModel,
-                    self.rosmuSel,
                 )
             )
         )
 
 
 ####+BEGIN: b:py3:cs:method/typing :methodName "basePath_update" :deco "default"
     """ #+begin_org
@@ -1284,19 +1385,19 @@
 
 ####+BEGIN: bx:cs:py3:section :title "CS ro_sap Cmnds"
 """ #+begin_org
 *  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  /Section/    [[elisp:(outline-show-subtree+toggle)][||]] *CS ro_sap Cmnds*  [[elisp:(org-cycle)][| ]]
 #+end_org """
 ####+END:
 
-####+BEGINNOT: b:py3:cs:cmnd/classHead :cmndName "ro_sapCreate" :ro "noCli" :comment "" :parsMand "perfName rosmu" :parsOpt "perfModel rosmuSel" :argsMin 0 :argsMax 0
+####+BEGINNOT: b:py3:cs:cmnd/classHead :cmndName "ro_sapCreateOld" :ro "noCli" :comment "" :parsMand "perfName rosmu" :parsOpt "perfModel rosmuSel" :argsMin 0 :argsMax 0
 """ #+begin_org
 *  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  CmndSvc-   [[elisp:(outline-show-subtree+toggle)][||]] <<ro_sapCreate>>parsMand=perfName rosmu parsOpt=perfModel rosmuSel argsMin=0 argsMax=0 ro=noCli pyInv=
 #+end_org """
-class ro_sapCreate(cs.Cmnd):
+class ro_sapCreateOld(cs.Cmnd):
     cmndParamsMandatory = [ 'perfName', 'rosmu', ]
     cmndParamsOptional = [ 'perfModel', 'rosmuSel', ]
     cmndArgsLen = {'Min': 0, 'Max': 0,}
     rtInvConstraints = cs.rtInvoker.RtInvoker.new_noRo() # NO RO From CLI
 
     @cs.track(fnLoc=True, fnEntry=True, fnExit=True)
     def cmnd(self,
@@ -1337,14 +1438,100 @@
         sapBaseFps.fps_setParam('perfName', perfName)
         sapBaseFps.fps_setParam('perfModel', perfModel)
         sapBaseFps.fps_setParam('rosmu', rosmu)
         sapBaseFps.fps_setParam('rosmuSel', rosmuSel)
 
         return(cmndOutcome)
 
+
+####+BEGIN: b:py3:cs:cmnd/classHead :cmndName "ro_sapCreate" :ro "noCli" :comment "" :parsMand "perfName rosmu svcName" :parsOpt "perfPortNu perfIpAddr perfModel rosmuSel rosmuControl accessControl" :argsMin 0 :argsMax 0
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  CmndSvc-   [[elisp:(outline-show-subtree+toggle)][||]] <<ro_sapCreate>>  =verify= parsMand=perfName rosmu svcName parsOpt=perfPortNu perfIpAddr perfModel rosmuSel rosmuControl accessControl ro=noCli   [[elisp:(org-cycle)][| ]]
+#+end_org """
+class ro_sapCreate(cs.Cmnd):
+    cmndParamsMandatory = [ 'perfName', 'rosmu', 'svcName', ]
+    cmndParamsOptional = [ 'perfPortNu', 'perfIpAddr', 'perfModel', 'rosmuSel', 'rosmuControl', 'accessControl', ]
+    cmndArgsLen = {'Min': 0, 'Max': 0,}
+    rtInvConstraints = cs.rtInvoker.RtInvoker.new_noRo() # NO RO From CLI
+
+    @cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+    def cmnd(self,
+             rtInv: cs.RtInvoker,
+             cmndOutcome: b.op.Outcome,
+             perfName: typing.Optional[str]=None,  # Cs Mandatory Param
+             rosmu: typing.Optional[str]=None,  # Cs Mandatory Param
+             svcName: typing.Optional[str]=None,  # Cs Mandatory Param
+             perfPortNu: typing.Optional[str]=None,  # Cs Optional Param
+             perfIpAddr: typing.Optional[str]=None,  # Cs Optional Param
+             perfModel: typing.Optional[str]=None,  # Cs Optional Param
+             rosmuSel: typing.Optional[str]=None,  # Cs Optional Param
+             rosmuControl: typing.Optional[str]=None,  # Cs Optional Param
+             accessControl: typing.Optional[str]=None,  # Cs Optional Param
+    ) -> b.op.Outcome:
+
+        failed = b_io.eh.badOutcome
+        callParamsDict = {'perfName': perfName, 'rosmu': rosmu, 'svcName': svcName, 'perfPortNu': perfPortNu, 'perfIpAddr': perfIpAddr, 'perfModel': perfModel, 'rosmuSel': rosmuSel, 'rosmuControl': rosmuControl, 'accessControl': accessControl, }
+        if self.invocationValidate(rtInv, cmndOutcome, callParamsDict, None).isProblematic():
+            return failed(cmndOutcome)
+        perfName = csParam.mappedValue('perfName', perfName)
+        rosmu = csParam.mappedValue('rosmu', rosmu)
+        svcName = csParam.mappedValue('svcName', svcName)
+        perfPortNu = csParam.mappedValue('perfPortNu', perfPortNu)
+        perfIpAddr = csParam.mappedValue('perfIpAddr', perfIpAddr)
+        perfModel = csParam.mappedValue('perfModel', perfModel)
+        rosmuSel = csParam.mappedValue('rosmuSel', rosmuSel)
+        rosmuControl = csParam.mappedValue('rosmuControl', rosmuControl)
+        accessControl = csParam.mappedValue('accessControl', accessControl)
+####+END:
+        """\
+***** [[elisp:(org-cycle)][| *CmndDesc:* | ]] Creates path for ro_sap and updates FPs
+        """
+
+        if rosmuSel is None:
+            rosmuSel = 'default'
+
+        if perfModel is None:
+            perfModel = 'rpyc'
+
+        if rosmuControl is None:
+            rosmuControl  = 'bisos'
+
+        if accessControl is None:
+            accessControl  = 'placeholder'
+
+        # NOTYET
+        from bisos.banna import bannaPortNu
+
+        if perfPortNu is None:
+            if (perfPortsList := bannaPortNu.bannaPortNuOf().pyWCmnd(
+                    cmndOutcome,
+                    argsList=[svcName]
+            ).results) is None : return failed(cmndOutcome)
+            perfPortNu = perfPortsList[0]
+
+        if perfIpAddr is None:
+            perfIpAddr = 'localhost'
+
+        sapBaseFps = b.pattern.sameInstance(SapBase_FPs, rosmu=rosmu, svcName=svcName, perfName=perfName, perfModel=perfModel, rosmuSel=rosmuSel)
+
+        sapBaseFps.fps_setParam('perfIpAddr', perfIpAddr)
+        sapBaseFps.fps_setParam('svcName', svcName)
+        sapBaseFps.fps_setParam('perfPortNu', perfPortNu)
+        sapBaseFps.fps_setParam('accessControl', accessControl)
+        sapBaseFps.fps_setParam('rosmuControl', rosmuControl)
+        sapBaseFps.fps_setParam('perfName', perfName)
+        sapBaseFps.fps_setParam('perfModel', perfModel)
+        sapBaseFps.fps_setParam('rosmu', rosmu)
+        sapBaseFps.fps_setParam('rosmuSel', rosmuSel)
+
+        sapPath = sapBaseFps.basePath_obtain()
+
+        return cmndOutcome.set(opResults=sapPath,)
+
+
 ####+BEGIN: bx:cs:py3:section :title "CS Performer"
 """ #+begin_org
 *  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  /Section/    [[elisp:(outline-show-subtree+toggle)][||]] *CS Performer*  [[elisp:(org-cycle)][| ]]
 #+end_org """
 ####+END:
 
 ####+BEGINNOT: b:py3:cs:cmnd/classHead :cmndName "csPerformer" :comment "" :parsMand "" :parsOpt "roSapPath svcName" :argsMin 0 :argsMax 0 :pyInv ""
@@ -1503,14 +1690,16 @@
             argChoices=[],
             argDescription="Rest of args for use by action"
         )
 
         return cmndArgsSpecDict
 
 
+
+
 ####+BEGIN: b:py3:cs:func/typing :funcName "roInvokeCmndAtSap" :comment "~Name of Box File Params~"  :funcType "eType" :deco "track"
 """ #+begin_org
 *  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-eType  [[elisp:(outline-show-subtree+toggle)][||]] /roInvokeCmndAtSap/  ~Name of Box File Params~ deco=track  [[elisp:(org-cycle)][| ]]
 #+end_org """
 @cs.track(fnLoc=True, fnEntry=True, fnExit=True)
 def roInvokeCmndAtSap(
 ####+END:
@@ -1533,18 +1722,347 @@
     rpycInvResult = cs.rpyc.csInvoke(
         ipAddr.parValueGet(),
         portNu.parValueGet(),
         cmndClass,
         **cmndKwArgs,
     )
     opResult = cmndKwArgs['cmndOutcome']
-    print(f"roOutcomeOf {cmndClass.__name__}::  {opResult.results}", file=sys.stderr)
+    resultsLen = len(opResult.results)
+    resultsType = type(opResult.results)
+    print(f"roOutcomeOf {cmndClass.__name__}::  opResult.results type = {resultsType} :: opResult.results length = {resultsLen}", file=sys.stderr)
     return rpycInvResult
 
 
+####+BEGIN: b:py3:cs:cmnd/classHead :cmndName "roEnable" :comment "" :parsMand "" :parsOpt "" :argsMin 0 :argsMax 0 :pyInv ""
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  CmndSvc-   [[elisp:(outline-show-subtree+toggle)][||]] <<roEnable>>  =verify= ro=cli   [[elisp:(org-cycle)][| ]]
+#+end_org """
+class roEnable(cs.Cmnd):
+    cmndParamsMandatory = [ ]
+    cmndParamsOptional = [ ]
+    cmndArgsLen = {'Min': 0, 'Max': 0,}
+
+    @cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+    def cmnd(self,
+             rtInv: cs.RtInvoker,
+             cmndOutcome: b.op.Outcome,
+    ) -> b.op.Outcome:
+
+        failed = b_io.eh.badOutcome
+        callParamsDict = {}
+        if self.invocationValidate(rtInv, cmndOutcome, callParamsDict, None).isProblematic():
+            return failed(cmndOutcome)
+####+END:
+
+        self.cmndDocStr(f""" #+begin_org
+** [[elisp:(org-cycle)][| *CmndDesc:* | ]]
+        #+end_org """)
+
+        self.captureRunStr(""" #+begin_org
+#+begin_src sh :results output :session shared
+  csExamples.cs -i roEnable
+#+end_src
+#+RESULTS:
+:
+        #+end_org """)
+        if self.justCaptureP(): return cmndOutcome
+
+        title = "NOTYET -- Should create roInv- and roPerf- symlinks."
+
+        return cmndOutcome.set(opResults=f"{title}",)
+
+
+
+####+BEGIN: b:py3:cs:func/typing :funcName "csMuIsPerformer" :comment "~Based on G_name~"  :funcType "eType" :deco "track"
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-eType  [[elisp:(outline-show-subtree+toggle)][||]] /csMuIsPerformer/  ~Based on G_name~ deco=track  [[elisp:(org-cycle)][| ]]
+#+end_org """
+@cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+def csMuIsPerformer(
+####+END:
+) -> bool:
+    """ #+begin_org
+** [[elisp:(org-cycle)][| *DocStr | ]
+    #+end_org """
+
+    csMuName = cs.G.icmMyName()
+    if "roPerf-" in csMuName:
+        return True
+    else:
+        return False
+
+####+BEGIN: b:py3:cs:func/typing :funcName "csMuIsInvoker" :comment "~Based on G_name~"  :funcType "eType" :deco "track"
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-eType  [[elisp:(outline-show-subtree+toggle)][||]] /csMuIsInvoker/  ~Based on G_name~ deco=track  [[elisp:(org-cycle)][| ]]
+#+end_org """
+@cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+def csMuIsInvoker(
+####+END:
+) -> bool:
+    """ #+begin_org
+** [[elisp:(org-cycle)][| *DocStr | ]
+    #+end_org """
+
+    csMuName = cs.G.icmMyName()
+    if "roInv-" in csMuName:
+        return True
+    else:
+        return False
+
+
+####+BEGIN: b:py3:cs:func/typing :funcName "csMuIsDirect" :comment "~Based on G_name~"  :funcType "eType" :deco "track"
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-eType  [[elisp:(outline-show-subtree+toggle)][||]] /csMuIsDirect/  ~Based on G_name~ deco=track  [[elisp:(org-cycle)][| ]]
+#+end_org """
+@cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+def csMuIsDirect(
+####+END:
+) -> bool:
+    """ #+begin_org
+** [[elisp:(org-cycle)][| *DocStr | ]
+    #+end_org """
+
+    csMuName = cs.G.icmMyName()
+    if "roInv-" in csMuName:
+        return False
+    elif "roPerf-" in csMuName:
+        return False
+    else:
+        return True
+
+####+BEGIN: b:py3:cs:func/typing :funcName "csMuDirectName" :comment "~Based on G_name~"  :funcType "eType" :deco "track"
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-eType  [[elisp:(outline-show-subtree+toggle)][||]] /csMuDirectName/  ~Based on G_name~ deco=track  [[elisp:(org-cycle)][| ]]
+#+end_org """
+@cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+def csMuDirectName(
+####+END:
+) -> bool:
+    """ #+begin_org
+** [[elisp:(org-cycle)][| *DocStr | ]
+    #+end_org """
+
+    csMuName = cs.G.icmMyName()
+    if "roInv-" in csMuName:
+        return csMuName.replace("roInv-", "")
+    elif "roPerf-" in csMuName:
+        return csMuName.replace("roPerf-", "")
+    else:
+        return csMuName
+
+####+BEGIN: b:py3:cs:func/typing :funcName "csMuInvokerName" :comment "~Based on G_name~"  :funcType "eType" :deco "track"
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-eType  [[elisp:(outline-show-subtree+toggle)][||]] /csMuInvokerName/  ~Based on G_name~ deco=track  [[elisp:(org-cycle)][| ]]
+#+end_org """
+@cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+def csMuInvokerName(
+####+END:
+) -> bool:
+    """ #+begin_org
+** [[elisp:(org-cycle)][| *DocStr | ]
+    #+end_org """
+
+    csMuName = cs.G.icmMyName()
+    if "roInv-" in csMuName:
+        return csMuName
+    elif "roPerf-" in csMuName:
+        return csMuName.replace("roPerf-", "roInv-")
+    else:
+        return ("roInv-" + csMuName)
+
+####+BEGIN: b:py3:cs:func/typing :funcName "csMuPerformerName" :comment "~Based on G_name~"  :funcType "eType" :deco "track"
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-eType  [[elisp:(outline-show-subtree+toggle)][||]] /csMuPerformerName/  ~Based on G_name~ deco=track  [[elisp:(org-cycle)][| ]]
+#+end_org """
+@cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+def csMuPerformerName(
+####+END:
+) -> bool:
+    """ #+begin_org
+** [[elisp:(org-cycle)][| *DocStr | ]
+    #+end_org """
+
+    csMuName = cs.G.icmMyName()
+    if "roInv-" in csMuName:
+        return csMuName.replace("roInv-", "roPerf-")
+    elif "roPerf-" in csMuName:
+        return csMuName
+    else:
+        return ("roPerf-" + csMuName)
+
+####+BEGIN: b:py3:cs:func/typing :funcName "roPerf_examples" :comment "~Based on G_name~"  :funcType "eType" :deco "track"
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-eType  [[elisp:(outline-show-subtree+toggle)][||]] /roPerf_examples/  ~Based on G_name~ deco=track  [[elisp:(org-cycle)][| ]]
+#+end_org """
+@cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+def roPerf_examples(
+####+END:
+        rosmu,
+        svcName,
+        perfName,
+        sectionTitle='default',
+        cmndOutcome=None,
+):
+    """ #+begin_org
+** [[elisp:(org-cycle)][| *DocStr | ]
+    #+end_org """
+
+    od = collections.OrderedDict
+    cmnd = cs.examples.cmndEnter
+    literal = cs.examples.execInsert
+
+    if sectionTitle == 'default': cs.examples.menuChapter('*Remote Operations -- Performer SAP Create and Manage*')
+
+    cmnd('perf_sapCreate', pars=od([('svcName', svcName), ('perfName', perfName), ('rosmu', rosmu)]))
+    literal(f"""csRo-manage.cs --svcName={svcName} --rosmu={rosmu}  -i ro_fps list""")
+    cmnd('csPerformer', pars=od([('svcName', svcName)]), comment="&  #  in background Start rpyc CS Service" )
+
+
+####+BEGIN: b:py3:cs:cmnd/classHead :cmndName "perf_sapCreate" :ro "noCli" :comment "" :parsMand "svcName perfName rosmu" :parsOpt "rosmuControl" :argsMin 0 :argsMax 0
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  CmndSvc-   [[elisp:(outline-show-subtree+toggle)][||]] <<perf_sapCreate>>  =verify= parsMand=svcName perfName rosmu parsOpt=rosmuControl ro=noCli   [[elisp:(org-cycle)][| ]]
+#+end_org """
+class perf_sapCreate(cs.Cmnd):
+    cmndParamsMandatory = [ 'svcName', 'perfName', 'rosmu', ]
+    cmndParamsOptional = [ 'rosmuControl', ]
+    cmndArgsLen = {'Min': 0, 'Max': 0,}
+    rtInvConstraints = cs.rtInvoker.RtInvoker.new_noRo() # NO RO From CLI
+
+    @cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+    def cmnd(self,
+             rtInv: cs.RtInvoker,
+             cmndOutcome: b.op.Outcome,
+             svcName: typing.Optional[str]=None,  # Cs Mandatory Param
+             perfName: typing.Optional[str]=None,  # Cs Mandatory Param
+             rosmu: typing.Optional[str]=None,  # Cs Mandatory Param
+             rosmuControl: typing.Optional[str]=None,  # Cs Optional Param
+    ) -> b.op.Outcome:
+
+        failed = b_io.eh.badOutcome
+        callParamsDict = {'svcName': svcName, 'perfName': perfName, 'rosmu': rosmu, 'rosmuControl': rosmuControl, }
+        if self.invocationValidate(rtInv, cmndOutcome, callParamsDict, None).isProblematic():
+            return failed(cmndOutcome)
+        svcName = csParam.mappedValue('svcName', svcName)
+        perfName = csParam.mappedValue('perfName', perfName)
+        rosmu = csParam.mappedValue('rosmu', rosmu)
+        rosmuControl = csParam.mappedValue('rosmuControl', rosmuControl)
+####+END:
+        """\
+***** [[elisp:(org-cycle)][| *CmndDesc:* | ]] Invoked both by invoker and performer. Creates path for ro_sap and updates FPs
+        """
+        self.captureRunStr(""" #+begin_org
+#+begin_src sh :results output :session shared
+  example.cs -i perf_sapCreate
+#+end_src
+#+RESULTS:
+:
+        #+end_org """)
+        if self.justCaptureP(): return cmndOutcome
+
+        if (sapPath := cs.ro.ro_sapCreate().pyWCmnd(
+                cmndOutcome,
+                rosmu=rosmu,
+                svcName=svcName,
+                perfName=perfName
+        ).results) is None : return failed(cmndOutcome)
+
+        return cmndOutcome.set(opResults=sapPath,)
+
+
+####+BEGIN: b:py3:cs:func/typing :funcName "roInv_examples" :comment "~Based on G_name~"  :funcType "eType" :deco "track"
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-eType  [[elisp:(outline-show-subtree+toggle)][||]] /roInv_examples/  ~Based on G_name~ deco=track  [[elisp:(org-cycle)][| ]]
+#+end_org """
+@cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+def roInv_examples(
+####+END:
+        rosmu,
+        svcName,
+        perfName,
+        perfIpAddr,
+        sectionTitle='default',
+        cmndOutcome=None,
+):
+    """ #+begin_org
+** [[elisp:(org-cycle)][| *DocStr | ]
+    #+end_org """
+
+    od = collections.OrderedDict
+    cmnd = cs.examples.cmndEnter
+    literal = cs.examples.execInsert
+
+    if sectionTitle == 'default': cs.examples.menuChapter('*Remote Operations --Invoker Management*')
+
+    cmnd('inv_sapCreate', pars=od([('perfName', perfName), ('perfIpAddr', perfIpAddr)]))
+    literal(f"""csRo-manage.cs --svcName="{svcName}" --perfName="{perfName}" --rosmu="{rosmu}"  -i ro_fps list""")
+
+
+####+BEGIN: b:py3:cs:cmnd/classHead :cmndName "inv_sapCreate" :ro "noCli" :comment "" :parsMand "perfName perfIpAddr rosmu svcName" :parsOpt "" :argsMin 0 :argsMax 0
+""" #+begin_org
+*  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  CmndSvc-   [[elisp:(outline-show-subtree+toggle)][||]] <<inv_sapCreate>>  =verify= parsMand=perfName perfIpAddr rosmu svcName ro=noCli   [[elisp:(org-cycle)][| ]]
+#+end_org """
+class inv_sapCreate(cs.Cmnd):
+    cmndParamsMandatory = [ 'perfName', 'perfIpAddr', 'rosmu', 'svcName', ]
+    cmndParamsOptional = [ ]
+    cmndArgsLen = {'Min': 0, 'Max': 0,}
+    rtInvConstraints = cs.rtInvoker.RtInvoker.new_noRo() # NO RO From CLI
+
+    @cs.track(fnLoc=True, fnEntry=True, fnExit=True)
+    def cmnd(self,
+             rtInv: cs.RtInvoker,
+             cmndOutcome: b.op.Outcome,
+             perfName: typing.Optional[str]=None,  # Cs Mandatory Param
+             perfIpAddr: typing.Optional[str]=None,  # Cs Mandatory Param
+             rosmu: typing.Optional[str]=None,  # Cs Mandatory Param
+             svcName: typing.Optional[str]=None,  # Cs Mandatory Param
+    ) -> b.op.Outcome:
+
+        failed = b_io.eh.badOutcome
+        callParamsDict = {'perfName': perfName, 'perfIpAddr': perfIpAddr, 'rosmu': rosmu, 'svcName': svcName, }
+        if self.invocationValidate(rtInv, cmndOutcome, callParamsDict, None).isProblematic():
+            return failed(cmndOutcome)
+        perfName = csParam.mappedValue('perfName', perfName)
+        perfIpAddr = csParam.mappedValue('perfIpAddr', perfIpAddr)
+        rosmu = csParam.mappedValue('rosmu', rosmu)
+        svcName = csParam.mappedValue('svcName', svcName)
+####+END:
+        """\
+***** [[elisp:(org-cycle)][| *CmndDesc:* | ]] Invoked both by invoker and performer. Creates path for ro_sap and updates FPs
+        """
+        self.captureRunStr(""" #+begin_org
+#+begin_src sh :results output :session shared
+  svcInvSiteRegBox.cs --rosmu svcSiteRegistrars.cs -i reg_sapCreateBox
+#+end_src
+#+RESULTS:
+#+begin_example
+
+FileParam.writeTo path=/bisos/var/cs/ro/sap/svcSiteRegistrars.cs/siteRegistrar/rpyc/default/perfIpAddr/value value=localhost
+#+end_example
+
+#+begin_src sh :results output :session shared
+  svcSiteRegistrars.cs -i reg_sapCreateBox
+#+end_src
+#+RESULTS:
+:
+: bash: svcSiteRegistrars.cs: command not found
+        #+end_org """)
+        if self.justCaptureP(): return cmndOutcome
+
+        if (sapPath := cs.ro.ro_sapCreate().pyWCmnd(
+                cmndOutcome,
+                rosmu=rosmu,
+                svcName=svcName,
+                perfName=perfName,
+                perfIpAddr=perfIpAddr,
+        ).results) is None : return failed(cmndOutcome)
+
+        return cmndOutcome.set(opResults=sapPath,)
+
+
+
 ####+BEGIN: b:py3:cs:framework/endOfFile :basedOn "classification"
 """ #+begin_org
 * *[[elisp:(org-cycle)][| ~End-Of-Editable-Text~ |]]* :: emacs and org variables and control parameters
 #+end_org """
 
 #+STARTUP: showall
```

### Comparing `bisos.b-0.2/bisos/b/cs/rpyc.py` & `bisos.b-0.3/bisos/b/cs/rpyc.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/cs/rtInvoker.py` & `bisos.b-0.3/bisos/b/cs/rtInvoker.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/cs/runArgs.py` & `bisos.b-0.3/bisos/b/cs/runArgs.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/cs/track.py` & `bisos.b-0.3/bisos/b/cs/track.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/dir.py` & `bisos.b-0.3/bisos/b/dir.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/exception.py` & `bisos.b-0.3/bisos/b/exception.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/fp.py` & `bisos.b-0.3/bisos/b/fp.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/fpCls.py` & `bisos.b-0.3/bisos/b/fpCls.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,15 +557,15 @@
 
         for each in formatTypes:    # type: ignore
             if each == 'values':
                 FP_listIcmParams(fps_namesWithAbsPath,)
             elif each == 'getExamples':
                 menu_getExamples(fpBaseInst,)
             elif each == 'setExamples':
-                print("Set Examples Come Here")
+                # print("Set Examples Come Here")
                 menu_setExamples(fpBaseInst,)
             else:
                 io.eh.problem_usageError(f"Unknown {each}")
 
         return cmndOutcome
 
 ####+BEGIN: b:py3:cs:method/args :methodName "cmndArgsSpec" :methodType "anyOrNone" :retType "bool" :deco "default" :argsList "self"
@@ -1113,16 +1113,18 @@
 
 
     csMainName = G.icmMyName()
 
     cmndFrontStr = f"""{csMainName} --fpBase="{fpBaseInst.fileTreeBaseGet()}" --cls="{fpBaseInst.__class__.__name__}" -i fpParamSetWithNameValue """
 
     for eachParam, eachDest  in fps_namesWithAbsPath.items():
-        thisCsParam = csParams.parNameFind(eachParam)   # type: ignore
-        print(f"{cmndFrontStr} {thisCsParam.parNameGet()} __VOID__")
+        # thisCsParam = csParams.parNameFind(eachParam)   # type: ignore
+        # print(f"{cmndFrontStr} {thisCsParam.parNameGet()} __VOID__")
+        print(f"{cmndFrontStr} {eachParam}  __VOID__")
+
 
 ####+BEGIN: b:py3:cs:func/typing :funcName "menu_getExamples" :deco ""
 """ #+begin_org
 *  _[[elisp:(blee:menu-sel:outline:popupMenu)][±]]_ _[[elisp:(blee:menu-sel:navigation:popupMenu)][Ξ]]_ [[elisp:(outline-show-branches+toggle)][|=]] [[elisp:(bx:orgm:indirectBufOther)][|>]] *[[elisp:(blee:ppmm:org-mode-toggle)][|N]]*  F-T-       [[elisp:(outline-show-subtree+toggle)][||]] /menu_getExamples/ deco=    [[elisp:(org-cycle)][| ]]
 #+end_org """
 def menu_getExamples(
 ####+END:
@@ -1134,16 +1136,18 @@
     fps_namesWithAbsPath = fpBaseInst.fps_manifestDictBuild()
 
     csMainName = G.icmMyName()
 
     cmndFrontStr = f"""{csMainName} --fpBase="{fpBaseInst.fileTreeBaseGet()}" --cls="{fpBaseInst.__class__.__name__}" -i fpParamGetWithName """
 
     for eachParam, eachDest  in fps_namesWithAbsPath.items():
-        thisCsParam = csParams.parNameFind(eachParam)   # type: ignore
-        print(f"{cmndFrontStr} {thisCsParam.parNameGet()}")
+        #thisCsParam = csParams.parNameFind(eachParam)   # type: ignore
+        #print(f"{cmndFrontStr} {thisCsParam.parNameGet()}")
+        #print(f"{cmndFrontStr} {eachDest.cmndParam.parNameGet()}")
+        print(f"{cmndFrontStr} {eachParam}")
 
 
 ####+BEGIN: b:prog:file/endOfFile :extraParams nil
 """ #+begin_org
 * *[[elisp:(org-cycle)][| END-OF-FILE |]]* :: emacs and org variables and control parameters
 #+end_org """
 ### local variables:
```

### Comparing `bisos.b-0.2/bisos/b/fpath.py` & `bisos.b-0.3/bisos/b/fpath.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/fto.py` & `bisos.b-0.3/bisos/b/fto.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/fv.py` & `bisos.b-0.3/bisos/b/fv.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/importFile.py` & `bisos.b-0.3/bisos/b/importFile.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/niche.py` & `bisos.b-0.3/bisos/b/niche.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/op.py` & `bisos.b-0.3/bisos/b/op.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,16 @@
 
         return self
 
     def isProblematic(self):
         if self.error:
             if self.error == b.OpError.Success:
                 return False
-            print(f"isProblematic: error={self.error}")
+            # NOTYET, these should be logged
+            # print(f"isProblematic: error={self.error}")
             b.cs.globalContext.get().__class__.lastOutcome = self
             return True
         else:
             return False
 
 
     def log(self):
```

### Comparing `bisos.b-0.2/bisos/b/pyRunAs.py` & `bisos.b-0.3/bisos/b/pyRunAs.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/subProc.py` & `bisos.b-0.3/bisos/b/subProc.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos/b/types.py` & `bisos.b-0.3/bisos/b/types.py`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/bisos.b.egg-info/PKG-INFO` & `bisos.b-0.3/bisos.b.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.b
-Version: 0.2
+Version: 0.3
 Summary: bisos.bx-bases: python scripts (Interactive Command Modules -- ICM) are used for bootstrapping the BISOS (ByStar Internet Services OS) environment.
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
```

### Comparing `bisos.b-0.2/bisos.b.egg-info/SOURCES.txt` & `bisos.b-0.3/bisos.b.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/lh-agpl3-LICENSE.txt` & `bisos.b-0.3/lh-agpl3-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bisos.b-0.2/setup.py` & `bisos.b-0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 
 
 # from setuphelpers import get_version, require_python
 # from setuptools import setup
 
 
 # __version__ = get_version('unisos/icm/__init__.py')
-__version__ = '0.2'
+__version__ = '0.3'
 
 
 requires = [
     'rpyc',
+    'bisos',
+    'bisos.transit',
 ]
 
 
 # print('Setting up under python version %s' % sys.version)
 # print('Requirements: %s' % ','.join(requires))
 
 scripts = [
```

