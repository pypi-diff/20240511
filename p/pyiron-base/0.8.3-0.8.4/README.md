# Comparing `tmp/pyiron_base-0.8.3.tar.gz` & `tmp/pyiron_base-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_base-0.8.3.tar", last modified: Tue Apr 30 13:32:13 2024, max compression
+gzip compressed data, was "pyiron_base-0.8.4.tar", last modified: Sat May 11 19:29:02 2024, max compression
```

## Comparing `pyiron_base-0.8.3.tar` & `pyiron_base-0.8.4.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.517540 pyiron_base-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-30 13:32:13.517540 pyiron_base-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.497539 pyiron_base-0.8.3/pyiron_base/
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-30 13:32:13.517540 pyiron_base-0.8.3/pyiron_base/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.497539 pyiron_base-0.8.3/pyiron_base/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/reloadfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.501539 pyiron_base-0.8.3/pyiron_base/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24876 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/filetable.py
--rw-r--r--   0 runner    (1001) docker     (127)    36818 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/jobtable.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/sqlcolumnlength.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.501539 pyiron_base-0.8.3/pyiron_base/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/has_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/has_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/has_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/lockable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.501539 pyiron_base-0.8.3/pyiron_base/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29278 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/datamining.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.501539 pyiron_base-0.8.3/pyiron_base/jobs/flex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/flex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/flex/executablecontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/flex/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/flex/pythonfunctioncontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.505539 pyiron_base-0.8.3/pyiron_base/jobs/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39577 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.505539 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10855 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/jobstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.505539 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/queuestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/runmode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    61634 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/jobtype.py
--rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    29036 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/runfunction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)    19730 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.505539 pyiron_base-0.8.3/pyiron_base/jobs/master/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/flexible.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/list.py
--rw-r--r--   0 runner    (1001) docker     (127)    32984 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/submissionstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/script.py
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.509539 pyiron_base-0.8.3/pyiron_base/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.509539 pyiron_base-0.8.3/pyiron_base/project/archiving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/archiving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/archiving/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/archiving/import_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/archiving/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/condaenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/external.py
--rw-r--r--   0 runner    (1001) docker     (127)    74335 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/jobloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/size.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.509539 pyiron_base-0.8.3/pyiron_base/project/update/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/update/pyiron_base_03x_to_04x.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.513539 pyiron_base-0.8.3/pyiron_base/state/
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/publications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/queue_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    25130 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.513539 pyiron_base-0.8.3/pyiron_base/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34122 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/datacontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/filedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)    43875 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/flattenedstorage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/has_stored_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    49006 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/hdfio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/hdfstub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/inputlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    33000 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.513539 pyiron_base-0.8.3/pyiron_base/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/jedi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29090 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/safetar.py
--rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.517540 pyiron_base-0.8.3/pyiron_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-30 13:32:11.000000 pyiron_base-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:32:13.517540 pyiron_base-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.513539 pyiron_base-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/tests/test_testwithproject.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/tests/test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.526921 pyiron_base-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-05-11 19:29:02.526921 pyiron_base-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.510921 pyiron_base-0.8.4/pyiron_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-11 19:29:02.526921 pyiron_base-0.8.4/pyiron_base/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.510921 pyiron_base-0.8.4/pyiron_base/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/cli/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/cli/reloadfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/cli/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.510921 pyiron_base-0.8.4/pyiron_base/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24876 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/database/filetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36818 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/database/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/database/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/database/jobtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/database/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/database/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/database/sqlcolumnlength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.514921 pyiron_base-0.8.4/pyiron_base/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/interfaces/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/interfaces/has_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/interfaces/has_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/interfaces/has_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/interfaces/lockable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/interfaces/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/interfaces/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.514921 pyiron_base-0.8.4/pyiron_base/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29278 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.514921 pyiron_base-0.8.4/pyiron_base/jobs/flex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/flex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/flex/executablecontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/flex/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/flex/pythonfunctioncontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.518921 pyiron_base-0.8.4/pyiron_base/jobs/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39577 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.518921 pyiron_base-0.8.4/pyiron_base/jobs/job/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10855 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/extension/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/extension/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/extension/jobstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.518921 pyiron_base-0.8.4/pyiron_base/jobs/job/extension/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/extension/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/extension/server/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/extension/server/queuestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/extension/server/runmode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61634 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/jobtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29036 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/runfunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19730 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/job/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.518921 pyiron_base-0.8.4/pyiron_base/jobs/master/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/master/flexible.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/master/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/master/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/master/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32984 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/master/submissionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/jobs/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.522921 pyiron_base-0.8.4/pyiron_base/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.522921 pyiron_base-0.8.4/pyiron_base/project/archiving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/archiving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/archiving/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/archiving/import_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/archiving/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/condaenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74335 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/jobloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.522921 pyiron_base-0.8.4/pyiron_base/project/update/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/project/update/pyiron_base_03x_to_04x.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.522921 pyiron_base-0.8.4/pyiron_base/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/state/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/state/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/state/publications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/state/queue_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25130 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/state/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/state/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/state/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.526921 pyiron_base-0.8.4/pyiron_base/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34122 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/storage/datacontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/storage/filedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/storage/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43875 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/storage/flattenedstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/storage/has_stored_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49006 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/storage/hdfio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/storage/hdfstub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/storage/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/storage/inputlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33000 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/storage/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.526921 pyiron_base-0.8.4/pyiron_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/utils/jedi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29090 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/utils/safetar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/pyiron_base/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.526921 pyiron_base-0.8.4/pyiron_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-05-11 19:29:02.000000 pyiron_base-0.8.4/pyiron_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-11 19:29:02.000000 pyiron_base-0.8.4/pyiron_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 19:29:02.000000 pyiron_base-0.8.4/pyiron_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-11 19:29:02.000000 pyiron_base-0.8.4/pyiron_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-11 19:29:02.000000 pyiron_base-0.8.4/pyiron_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 19:29:02.000000 pyiron_base-0.8.4/pyiron_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-11 19:29:00.000000 pyiron_base-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 19:29:02.526921 pyiron_base-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:29:02.526921 pyiron_base-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/tests/test_testwithproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-11 19:28:07.000000 pyiron_base-0.8.4/tests/test_toolkit.py
```

### Comparing `pyiron_base-0.8.3/LICENSE` & `pyiron_base-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/__init__.py` & `pyiron_base-0.8.4/pyiron_base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/_tests.py` & `pyiron_base-0.8.4/pyiron_base/_tests.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/cli/control.py` & `pyiron_base-0.8.4/pyiron_base/cli/control.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/cli/install.py` & `pyiron_base-0.8.4/pyiron_base/cli/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/cli/ls.py` & `pyiron_base-0.8.4/pyiron_base/cli/ls.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/cli/reloadfile.py` & `pyiron_base-0.8.4/pyiron_base/cli/reloadfile.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/cli/rm.py` & `pyiron_base-0.8.4/pyiron_base/cli/rm.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/cli/wrapper.py` & `pyiron_base-0.8.4/pyiron_base/cli/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/database/filetable.py` & `pyiron_base-0.8.4/pyiron_base/database/filetable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/database/generic.py` & `pyiron_base-0.8.4/pyiron_base/database/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/database/interface.py` & `pyiron_base-0.8.4/pyiron_base/database/interface.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/database/jobtable.py` & `pyiron_base-0.8.4/pyiron_base/database/jobtable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/database/manager.py` & `pyiron_base-0.8.4/pyiron_base/database/manager.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/database/performance.py` & `pyiron_base-0.8.4/pyiron_base/database/performance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/database/tables.py` & `pyiron_base-0.8.4/pyiron_base/database/tables.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/interfaces/factory.py` & `pyiron_base-0.8.4/pyiron_base/interfaces/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/interfaces/has_dict.py` & `pyiron_base-0.8.4/pyiron_base/interfaces/has_dict.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/interfaces/has_groups.py` & `pyiron_base-0.8.4/pyiron_base/interfaces/has_groups.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/interfaces/has_hdf.py` & `pyiron_base-0.8.4/pyiron_base/interfaces/has_hdf.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/interfaces/lockable.py` & `pyiron_base-0.8.4/pyiron_base/interfaces/lockable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/interfaces/object.py` & `pyiron_base-0.8.4/pyiron_base/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/interfaces/singleton.py` & `pyiron_base-0.8.4/pyiron_base/interfaces/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/datamining.py` & `pyiron_base-0.8.4/pyiron_base/jobs/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/dynamic.py` & `pyiron_base-0.8.4/pyiron_base/jobs/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/flex/executablecontainer.py` & `pyiron_base-0.8.4/pyiron_base/jobs/flex/executablecontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/flex/factory.py` & `pyiron_base-0.8.4/pyiron_base/jobs/flex/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/flex/pythonfunctioncontainer.py` & `pyiron_base-0.8.4/pyiron_base/jobs/flex/pythonfunctioncontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/core.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/core.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/executable.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/extension/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/files.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/extension/files.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/jobstatus.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/extension/jobstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/generic.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/extension/server/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/queuestatus.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/extension/server/queuestatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/runmode.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/extension/server/runmode.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/factory.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/generic.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/interactive.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/jobtype.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/jobtype.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/path.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/runfunction.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/runfunction.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/template.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/template.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/toolkit.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/util.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/job/wrapper.py` & `pyiron_base-0.8.4/pyiron_base/jobs/job/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/master/flexible.py` & `pyiron_base-0.8.4/pyiron_base/jobs/master/flexible.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/master/generic.py` & `pyiron_base-0.8.4/pyiron_base/jobs/master/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/master/interactivewrapper.py` & `pyiron_base-0.8.4/pyiron_base/jobs/master/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/master/list.py` & `pyiron_base-0.8.4/pyiron_base/jobs/master/list.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/master/parallel.py` & `pyiron_base-0.8.4/pyiron_base/jobs/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/master/submissionstatus.py` & `pyiron_base-0.8.4/pyiron_base/jobs/master/submissionstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/script.py` & `pyiron_base-0.8.4/pyiron_base/jobs/script.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/jobs/worker.py` & `pyiron_base-0.8.4/pyiron_base/jobs/worker.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/archiving/export_archive.py` & `pyiron_base-0.8.4/pyiron_base/project/archiving/export_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/archiving/import_archive.py` & `pyiron_base-0.8.4/pyiron_base/project/archiving/import_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/condaenv.py` & `pyiron_base-0.8.4/pyiron_base/project/condaenv.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/data.py` & `pyiron_base-0.8.4/pyiron_base/project/data.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/external.py` & `pyiron_base-0.8.4/pyiron_base/project/external.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/generic.py` & `pyiron_base-0.8.4/pyiron_base/project/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/gui.py` & `pyiron_base-0.8.4/pyiron_base/project/gui.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/jobloader.py` & `pyiron_base-0.8.4/pyiron_base/project/jobloader.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/maintenance.py` & `pyiron_base-0.8.4/pyiron_base/project/maintenance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/path.py` & `pyiron_base-0.8.4/pyiron_base/project/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/size.py` & `pyiron_base-0.8.4/pyiron_base/project/size.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/project/update/pyiron_base_03x_to_04x.py` & `pyiron_base-0.8.4/pyiron_base/project/update/pyiron_base_03x_to_04x.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/state/__init__.py` & `pyiron_base-0.8.4/pyiron_base/state/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/state/install.py` & `pyiron_base-0.8.4/pyiron_base/state/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/state/logger.py` & `pyiron_base-0.8.4/pyiron_base/state/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/state/publications.py` & `pyiron_base-0.8.4/pyiron_base/state/publications.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/state/queue_adapter.py` & `pyiron_base-0.8.4/pyiron_base/state/queue_adapter.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/state/settings.py` & `pyiron_base-0.8.4/pyiron_base/state/settings.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/state/signal.py` & `pyiron_base-0.8.4/pyiron_base/state/signal.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/state/update.py` & `pyiron_base-0.8.4/pyiron_base/state/update.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/storage/datacontainer.py` & `pyiron_base-0.8.4/pyiron_base/storage/datacontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/storage/filedata.py` & `pyiron_base-0.8.4/pyiron_base/storage/filedata.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/storage/fileio.py` & `pyiron_base-0.8.4/pyiron_base/storage/fileio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/storage/flattenedstorage.py` & `pyiron_base-0.8.4/pyiron_base/storage/flattenedstorage.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/storage/has_stored_traits.py` & `pyiron_base-0.8.4/pyiron_base/storage/has_stored_traits.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/storage/hdfio.py` & `pyiron_base-0.8.4/pyiron_base/storage/hdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/storage/hdfstub.py` & `pyiron_base-0.8.4/pyiron_base/storage/hdfstub.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/storage/helper_functions.py` & `pyiron_base-0.8.4/pyiron_base/storage/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/storage/parameters.py` & `pyiron_base-0.8.4/pyiron_base/storage/parameters.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/utils/deprecate.py` & `pyiron_base-0.8.4/pyiron_base/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/utils/error.py` & `pyiron_base-0.8.4/pyiron_base/utils/error.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/utils/instance.py` & `pyiron_base-0.8.4/pyiron_base/utils/instance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/utils/jedi.py` & `pyiron_base-0.8.4/pyiron_base/utils/jedi.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/utils/parser.py` & `pyiron_base-0.8.4/pyiron_base/utils/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/utils/safetar.py` & `pyiron_base-0.8.4/pyiron_base/utils/safetar.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base/utils/units.py` & `pyiron_base-0.8.4/pyiron_base/utils/units.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/pyiron_base.egg-info/SOURCES.txt` & `pyiron_base-0.8.4/pyiron_base.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 pyproject.toml
 setup.py
 pyiron_base/__init__.py
 pyiron_base/_tests.py
 pyiron_base/_version.py
 pyiron_base.egg-info/PKG-INFO
 pyiron_base.egg-info/SOURCES.txt
```

### Comparing `pyiron_base-0.8.3/pyproject.toml` & `pyiron_base-0.8.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pyiron_base"
 description = "Core components of the pyiron integrated development environment (IDE) for computational materials science"
 authors = [
     { name = "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department", email = "pyiron@mpie.de" },
 ]
-readme = "README.rst"
+readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["pyiron"]
 requires-python = ">=3.9, <3.13"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering :: Physics",
     "License :: OSI Approved :: BSD License",
@@ -24,26 +24,26 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "cloudpickle>=2.0.0,<=3.0.0",
     "gitpython>=3.1.23,<=3.1.43",
     "h5io_browser>=0.0.6,<=0.0.12",
     "h5py>=3.6.0,<=3.11.0",
-    "jinja2>=2.11.3,<=3.1.3",
+    "jinja2>=2.11.3,<=3.1.4",
     "numpy>=1.23.5,<=1.26.4",
     "monty>=2021.3.3,<=2024.4.17",
     "pandas>=2.0.0,<=2.2.2",
     "pint>=0.18,<=0.23",
     "psutil>=5.8.0,<=5.9.8",
     "pyfileindex>=0.0.16,<=0.0.24",
-    "pympipool>=0.8.0,<=0.8.1",
-    "pysqa>=0.1.12,<=0.1.19",
-    "sqlalchemy>=2.0.22,<=2.0.29",
+    "pympipool>=0.8.0,<=0.8.2",
+    "pysqa>=0.1.12,<=0.1.20",
+    "sqlalchemy>=2.0.22,<=2.0.30",
     "tables>=3.6.1,<=3.9.2",
-    "tqdm>=4.44.0,<=4.66.2",
+    "tqdm>=4.44.0,<=4.66.4",
     "traitlets>=5.1.1,<=5.14.3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/pyiron/pyiron_base"
 Documentation = "https://github.com/pyiron/pyiron_base"
```

### Comparing `pyiron_base-0.8.3/tests/test_testwithproject.py` & `pyiron_base-0.8.4/tests/test_testwithproject.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.3/tests/test_toolkit.py` & `pyiron_base-0.8.4/tests/test_toolkit.py`

 * *Files identical despite different names*

