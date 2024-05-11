# Comparing `tmp/plex_fuse-0.7.1.tar.gz` & `tmp/plex_fuse-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex_fuse-0.7.1.tar", last modified: Mon Apr 29 18:18:43 2024, max compression
+gzip compressed data, was "plex_fuse-0.8.0.tar", last modified: Sat May 11 11:27:48 2024, max compression
```

## Comparing `plex_fuse-0.7.1.tar` & `plex_fuse-0.8.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:18:43.093331 plex_fuse-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-29 18:18:43.093331 plex_fuse-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:18:43.089331 plex_fuse-0.7.1/plex_fuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-29 18:18:43.000000 plex_fuse-0.7.1/plex_fuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-29 18:18:43.000000 plex_fuse-0.7.1/plex_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:18:43.000000 plex_fuse-0.7.1/plex_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 18:18:43.000000 plex_fuse-0.7.1/plex_fuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 18:18:43.000000 plex_fuse-0.7.1/plex_fuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 18:18:43.000000 plex_fuse-0.7.1/plex_fuse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:18:43.085331 plex_fuse-0.7.1/plexfuse/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/TimeoutLock.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:18:43.085331 plex_fuse-0.7.1/plexfuse/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/cache/CacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/cache/CachedPropertyCacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/cache/DelayedPropertyCacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/cache/FileCache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/cache/HttpCache.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/cache/UserDictCacheControl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:18:43.085331 plex_fuse-0.7.1/plexfuse/control/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/control/Control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/control/ControlListener.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/control/ControlVFS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:18:43.085331 plex_fuse-0.7.1/plexfuse/fs/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/fs/FsOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/fs/PlexDirectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/fs/PlexFS.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/fs/PlexFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/fs/RefCountedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/fs/Timestampable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/fs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/fs/plex_errno.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:18:43.089331 plex_fuse-0.7.1/plexfuse/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/plex/Monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/plex/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:18:43.089331 plex_fuse-0.7.1/plexfuse/vfs/
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/ChunkedFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/Playable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/PlexVFS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:18:43.089331 plex_fuse-0.7.1/plexfuse/vfs/entry/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/AttrEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/ControlSockEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/DirEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/EpisodeEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/FileEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/LibraryEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/MovieEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/PathEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/PlexMatchEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/SeasonEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/SectionEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/SubtitleEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/plexfuse/vfs/entry/SymlinkEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:18:43.093331 plex_fuse-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:18:43.089331 plex_fuse-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/tests/test_RefCountedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/tests/test_chunk_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/tests/test_chunk_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/tests/test_file_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/tests/test_file_copy_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/tests/test_socket_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-29 18:18:39.000000 plex_fuse-0.7.1/tests/test_timeout_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/plex_fuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.536728 plex_fuse-0.8.0/plexfuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/TimeoutLock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.536728 plex_fuse-0.8.0/plexfuse/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/CacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/CachedPropertyCacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/DelayedPropertyCacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/FileCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/HttpCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/UserDictCacheControl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.536728 plex_fuse-0.8.0/plexfuse/control/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/control/Control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/control/ControlListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/control/ControlVFS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.536728 plex_fuse-0.8.0/plexfuse/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/FsOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/PlexDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/PlexFS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/PlexFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/RefCountedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/Timestampable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/plex_errno.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.536728 plex_fuse-0.8.0/plexfuse/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/plex/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/plexfuse/vfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/ChunkedFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/Playable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/PlexVFS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/plexfuse/vfs/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/AttrEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/ControlSockEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/DirEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/EpisodeEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/FileEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/LibraryEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/MovieEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/PathEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/PlexMatchEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/SeasonEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/SectionEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/SubtitleEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/SymlinkEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_RefCountedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_chunk_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_chunk_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_file_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_file_copy_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_socket_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_timeout_lock.py
```

### Comparing `plex_fuse-0.7.1/LICENSE` & `plex_fuse-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/PKG-INFO` & `plex_fuse-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-fuse
-Version: 0.7.1
+Version: 0.8.0
 Summary: Plex FUSE Filesystem - Mount Remote Plex Media Server contents as local filesystem
 Author-email: Elan Ruusamäe <glen@pld-linux.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Elan Ruusamäe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `plex_fuse-0.7.1/README.md` & `plex_fuse-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plex_fuse.egg-info/PKG-INFO` & `plex_fuse-0.8.0/plex_fuse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-fuse
-Version: 0.7.1
+Version: 0.8.0
 Summary: Plex FUSE Filesystem - Mount Remote Plex Media Server contents as local filesystem
 Author-email: Elan Ruusamäe <glen@pld-linux.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Elan Ruusamäe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `plex_fuse-0.7.1/plex_fuse.egg-info/SOURCES.txt` & `plex_fuse-0.8.0/plex_fuse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/TimeoutLock.py` & `plex_fuse-0.8.0/plexfuse/TimeoutLock.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/cache/CacheControl.py` & `plex_fuse-0.8.0/plexfuse/cache/CacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/cache/CachedPropertyCacheControl.py` & `plex_fuse-0.8.0/plexfuse/cache/CachedPropertyCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/cache/DelayedPropertyCacheControl.py` & `plex_fuse-0.8.0/plexfuse/cache/DelayedPropertyCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/cache/FileCache.py` & `plex_fuse-0.8.0/plexfuse/cache/FileCache.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/cache/HttpCache.py` & `plex_fuse-0.8.0/plexfuse/cache/HttpCache.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/cache/UserDictCacheControl.py` & `plex_fuse-0.8.0/plexfuse/cache/UserDictCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/control/Control.py` & `plex_fuse-0.8.0/plexfuse/control/Control.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/control/ControlListener.py` & `plex_fuse-0.8.0/plexfuse/control/ControlListener.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/control/ControlVFS.py` & `plex_fuse-0.8.0/plexfuse/control/ControlVFS.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/fs/PlexFS.py` & `plex_fuse-0.8.0/plexfuse/fs/PlexFS.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
         self.options = FsOptions()
         self.control = None
         self.monitor = None
         self.file_map = RefCountedDict()
-        self.iolock = TimeoutLock(60)
+        self.iolock = TimeoutLock(300)
 
     @cached_property
     def plex(self):
         return PlexApi()
 
     @cached_property
     def vfs(self):
```

### Comparing `plex_fuse-0.7.1/plexfuse/fs/RefCountedDict.py` & `plex_fuse-0.8.0/plexfuse/fs/RefCountedDict.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/fs/main.py` & `plex_fuse-0.8.0/plexfuse/fs/main.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/fs/plex_errno.py` & `plex_fuse-0.8.0/plexfuse/fs/plex_errno.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,24 @@
     handle exceptions from plex setting appropriate errno
     """
 
     @wraps(f)
     def decorated(*args, **kwargs):
         try:
             return f(*args, **kwargs)
-        except (urllib3.exceptions.ReadTimeoutError, requests.exceptions.ReadTimeout, TimeoutError) as e:
+        except (urllib3.exceptions.ReadTimeoutError,
+                requests.exceptions.ConnectionError,
+                requests.exceptions.ReadTimeout,
+                TimeoutError) as e:
             print(f"ERROR: Plex: {f.__module__}.{f.__name__}({args[1:]}, {kwargs}): {type(e)}: {e}")
             return -errno.ETIMEDOUT
         except plexapi.exceptions.BadRequest as e:
             print(f"ERROR: Plex: {f.__module__}.{f.__name__}({args[1:]}, {kwargs}): {e}")
             return -errno.ENETUNREACH
         except KeyError as e:
             print(f"ERROR: Plex: {f.__module__}.{f.__name__}: Unsupported path: {e}")
             return -errno.ENOENT
+        except Exception as e:
+            print(f"ERROR: Plex: Unknown error {type(e)}: {e}")
+            return -errno.ENOENT
 
     return decorated
```

### Comparing `plex_fuse-0.7.1/plexfuse/plex/Monitor.py` & `plex_fuse-0.8.0/plexfuse/plex/Monitor.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/plex/PlexApi.py` & `plex_fuse-0.8.0/plexfuse/plex/PlexApi.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 class PlexApi:
     CACHE_PATH = Path("cache")
     CACHE_VERSION = str(2)
     CHUNK_SIZE = 1024 * 1024 * 16
     HTTP_CACHE = False
-    PLEX_TIMEOUT = 3
+    PLEX_TIMEOUT = 30
     PLEX_READ_TIMEOUT = 10
 
     @cached_property
     def server(self):
         session = None
         if self.HTTP_CACHE:
             http_cache = HttpCache(self.CACHE_PATH / "http_cache")
```

### Comparing `plex_fuse-0.7.1/plexfuse/vfs/ChunkedFile.py` & `plex_fuse-0.8.0/plexfuse/vfs/ChunkedFile.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/vfs/Playable.py` & `plex_fuse-0.8.0/plexfuse/vfs/Playable.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/vfs/PlexVFS.py` & `plex_fuse-0.8.0/plexfuse/vfs/PlexVFS.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/vfs/entry/FileEntry.py` & `plex_fuse-0.8.0/plexfuse/vfs/entry/FileEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/vfs/entry/LibraryEntry.py` & `plex_fuse-0.8.0/plexfuse/vfs/entry/LibraryEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/vfs/entry/PlexMatchEntry.py` & `plex_fuse-0.8.0/plexfuse/vfs/entry/PlexMatchEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/vfs/entry/SectionEntry.py` & `plex_fuse-0.8.0/plexfuse/vfs/entry/SectionEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/plexfuse/vfs/entry/SubtitleEntry.py` & `plex_fuse-0.8.0/plexfuse/vfs/entry/SubtitleEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/pyproject.toml` & `plex_fuse-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/tests/test_RefCountedDict.py` & `plex_fuse-0.8.0/tests/test_RefCountedDict.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/tests/test_chunk_calc.py` & `plex_fuse-0.8.0/tests/test_chunk_calc.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/tests/test_chunk_read.py` & `plex_fuse-0.8.0/tests/test_chunk_read.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/tests/test_file_copy_partial.py` & `plex_fuse-0.8.0/tests/test_file_copy_partial.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/tests/test_socket_control.py` & `plex_fuse-0.8.0/tests/test_socket_control.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.7.1/tests/test_timeout_lock.py` & `plex_fuse-0.8.0/tests/test_timeout_lock.py`

 * *Files identical despite different names*

