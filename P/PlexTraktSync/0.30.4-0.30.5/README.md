# Comparing `tmp/plextraktsync-0.30.4.tar.gz` & `tmp/plextraktsync-0.30.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plextraktsync-0.30.4.tar", last modified: Sun May  5 18:12:47 2024, max compression
+gzip compressed data, was "plextraktsync-0.30.5.tar", last modified: Fri May 10 16:01:02 2024, max compression
```

## Comparing `plextraktsync-0.30.4.tar` & `plextraktsync-0.30.5.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.986604 plextraktsync-0.30.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    30216 2024-05-05 18:12:47.986604 plextraktsync-0.30.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.986604 plextraktsync-0.30.4/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30216 2024-05-05 18:12:47.000000 plextraktsync-0.30.4/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-05 18:12:47.000000 plextraktsync-0.30.4/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:12:47.000000 plextraktsync-0.30.4/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 18:12:47.000000 plextraktsync-0.30.4/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-05 18:12:47.000000 plextraktsync-0.30.4/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 18:12:47.000000 plextraktsync-0.30.4/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26812 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.966604 plextraktsync-0.30.4/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.970604 plextraktsync-0.30.4/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.970604 plextraktsync-0.30.4/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/config/ServerConfigFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.970604 plextraktsync-0.30.4/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/decorators/coro.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.970604 plextraktsync-0.30.4/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/logger/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.970604 plextraktsync-0.30.4/plextraktsync/media/
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/media/Media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/media/MediaFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.974604 plextraktsync-0.30.4/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/mixin/RichMarkup.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/mixin/SetWindowTitle.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.974604 plextraktsync-0.30.4/plextraktsync/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plan/WalkConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plan/WalkPlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plan/WalkPlanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plan/Walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.974604 plextraktsync-0.30.4/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexGuidProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexGuidProviderIMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexGuidProviderLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexGuidProviderMbid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexGuidProviderTMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexGuidProviderTVDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexIdFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexPlaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexPlaylistCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexSectionPager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plex/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.978603 plextraktsync-0.30.4/plextraktsync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.978603 plextraktsync-0.30.4/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/queue/TraktScrobbleWorker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.978603 plextraktsync-0.30.4/plextraktsync/rich/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/rich/RichHighlighter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/rich/RichProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.978603 plextraktsync-0.30.4/plextraktsync/sync/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/AddCollectionPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/ClearCollectedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/LikedListsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/Sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/SyncRatingsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/SyncWatchedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/TraktListsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/WatchListPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/WatchProgressPlugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.978603 plextraktsync-0.30.4/plextraktsync/sync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/plugin/SyncPluginInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/plugin/SyncPluginManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/sync/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.982603 plextraktsync-0.30.4/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/TraktUserList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/TraktUserListCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/WatchProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/trakt/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.982603 plextraktsync-0.30.4/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/Rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/util/remove_empty_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.986604 plextraktsync-0.30.4/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-05 18:12:45.000000 plextraktsync-0.30.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-05 18:12:47.986604 plextraktsync-0.30.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:12:47.986604 plextraktsync-0.30.4/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_plex_id.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_rating.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-05-05 18:12:44.000000 plextraktsync-0.30.4/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.394349 plextraktsync-0.30.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    30223 2024-05-10 16:01:02.394349 plextraktsync-0.30.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.394349 plextraktsync-0.30.5/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30223 2024-05-10 16:01:02.000000 plextraktsync-0.30.5/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-10 16:01:02.000000 plextraktsync-0.30.5/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:01:02.000000 plextraktsync-0.30.5/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-10 16:01:02.000000 plextraktsync-0.30.5/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-10 16:01:02.000000 plextraktsync-0.30.5/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 16:01:02.000000 plextraktsync-0.30.5/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26819 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.370349 plextraktsync-0.30.5/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.374349 plextraktsync-0.30.5/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.374349 plextraktsync-0.30.5/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/config/ServerConfigFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.378349 plextraktsync-0.30.5/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/decorators/coro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.378349 plextraktsync-0.30.5/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/logger/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.378349 plextraktsync-0.30.5/plextraktsync/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/media/Media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/media/MediaFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.378349 plextraktsync-0.30.5/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/mixin/RichMarkup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/mixin/SetWindowTitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.378349 plextraktsync-0.30.5/plextraktsync/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plan/WalkConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plan/WalkPlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plan/WalkPlanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plan/Walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.382349 plextraktsync-0.30.5/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexGuidProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexGuidProviderIMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexGuidProviderLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexGuidProviderMbid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexGuidProviderTMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexGuidProviderTVDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexIdFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexPlaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexPlaylistCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexSectionPager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.382349 plextraktsync-0.30.5/plextraktsync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.382349 plextraktsync-0.30.5/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/queue/TraktScrobbleWorker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.382349 plextraktsync-0.30.5/plextraktsync/rich/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/rich/RichHighlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/rich/RichProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.386349 plextraktsync-0.30.5/plextraktsync/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/AddCollectionPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/ClearCollectedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/LikedListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/Sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/SyncRatingsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/SyncWatchedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/TraktListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/WatchListPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/WatchProgressPlugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.386349 plextraktsync-0.30.5/plextraktsync/sync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/plugin/SyncPluginInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/plugin/SyncPluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/sync/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.390349 plextraktsync-0.30.5/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/TraktUserList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/TraktUserListCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/WatchProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/trakt/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.390349 plextraktsync-0.30.5/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/Rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/util/remove_empty_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.390349 plextraktsync-0.30.5/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-10 16:01:00.000000 plextraktsync-0.30.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-10 16:01:02.394349 plextraktsync-0.30.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:02.394349 plextraktsync-0.30.5/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_plex_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_rating.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-05-10 16:00:58.000000 plextraktsync-0.30.5/tests/test_walker.py
```

### Comparing `plextraktsync-0.30.4/LICENSE` & `plextraktsync-0.30.5/LICENSE`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/PKG-INFO` & `plextraktsync-0.30.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.4
+Version: 0.30.5
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,15 +34,15 @@
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: platformdirs==4.2.1; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: plexapi==4.15.12; python_version >= "3.8"
 Requires-Dist: pluggy==1.5.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
-Requires-Dist: pygments==2.17.2; python_version >= "3.7"
+Requires-Dist: pygments==2.18.0; python_version >= "3.8"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
 Requires-Dist: pytrakt==3.4.32
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
 Requires-Dist: requests==2.31.0; python_version >= "3.7"
 Requires-Dist: requests-cache==1.2.0; python_version >= "3.8"
@@ -765,15 +765,15 @@
 Now create instances based on server names from `servers.yml`, in this example `SERVER_NAME`.
 
 1. `systemctl --user start "plextraktsync@SERVER_NAME.service"`
 1. `systemctl --user status "plextraktsync@SERVER_NAME.service"`
 
 for complete logs, you can use `journalctl` (add `-f` to follow logs):
 
-1. `journalctl -u "plextraktsync@SERVER_NAME.service"`
+1. `journalctl --user -u "plextraktsync@SERVER_NAME.service"`
 
 If all works, enable it for auto-start on host reboot
 
 1. `systemctl --user enable "plextraktsync@SERVER_NAME.service"`
 
 For systemd --user session to start without having to log in you need to enable [systemd-linger]:
```

### Comparing `plextraktsync-0.30.4/PlexTraktSync.egg-info/PKG-INFO` & `plextraktsync-0.30.5/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.4
+Version: 0.30.5
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,15 +34,15 @@
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: platformdirs==4.2.1; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: plexapi==4.15.12; python_version >= "3.8"
 Requires-Dist: pluggy==1.5.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
-Requires-Dist: pygments==2.17.2; python_version >= "3.7"
+Requires-Dist: pygments==2.18.0; python_version >= "3.8"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
 Requires-Dist: pytrakt==3.4.32
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
 Requires-Dist: requests==2.31.0; python_version >= "3.7"
 Requires-Dist: requests-cache==1.2.0; python_version >= "3.8"
@@ -765,15 +765,15 @@
 Now create instances based on server names from `servers.yml`, in this example `SERVER_NAME`.
 
 1. `systemctl --user start "plextraktsync@SERVER_NAME.service"`
 1. `systemctl --user status "plextraktsync@SERVER_NAME.service"`
 
 for complete logs, you can use `journalctl` (add `-f` to follow logs):
 
-1. `journalctl -u "plextraktsync@SERVER_NAME.service"`
+1. `journalctl --user -u "plextraktsync@SERVER_NAME.service"`
 
 If all works, enable it for auto-start on host reboot
 
 1. `systemctl --user enable "plextraktsync@SERVER_NAME.service"`
 
 For systemd --user session to start without having to log in you need to enable [systemd-linger]:
```

### Comparing `plextraktsync-0.30.4/PlexTraktSync.egg-info/SOURCES.txt` & `plextraktsync-0.30.5/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/PlexTraktSync.egg-info/requires.txt` & `plextraktsync-0.30.5/PlexTraktSync.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 oauthlib==3.2.2
 pyyaml==6.0.1
 
 [:python_version >= "3.7"]
 attrs==23.2.0
 click==8.1.7
 mdurl==0.1.2
-pygments==2.17.2
 requests==2.31.0
 tqdm==4.66.4
 
 [:python_version >= "3.7" and python_version < "4.0"]
 inquirerpy==0.3.4
 pfzy==0.3.4
 
@@ -56,12 +55,13 @@
 platformdirs==4.2.1
 
 [:python_version >= "3.8"]
 apluggy==0.9.4
 humanize==4.9.0
 plexapi==4.15.12
 pluggy==1.5.0
+pygments==2.18.0
 python-dotenv==1.0.1
 requests-cache==1.2.0
 types-decorator==5.1.8.20240310
 urllib3==2.2.1
 websocket-client==1.8.0
```

### Comparing `plextraktsync-0.30.4/README.md` & `plextraktsync-0.30.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -705,15 +705,15 @@
 Now create instances based on server names from `servers.yml`, in this example `SERVER_NAME`.
 
 1. `systemctl --user start "plextraktsync@SERVER_NAME.service"`
 1. `systemctl --user status "plextraktsync@SERVER_NAME.service"`
 
 for complete logs, you can use `journalctl` (add `-f` to follow logs):
 
-1. `journalctl -u "plextraktsync@SERVER_NAME.service"`
+1. `journalctl --user -u "plextraktsync@SERVER_NAME.service"`
 
 If all works, enable it for auto-start on host reboot
 
 1. `systemctl --user enable "plextraktsync@SERVER_NAME.service"`
 
 For systemd --user session to start without having to log in you need to enable [systemd-linger]:
```

### Comparing `plextraktsync-0.30.4/plextraktsync/cli.py` & `plextraktsync-0.30.5/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/bug_report.py` & `plextraktsync-0.30.5/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/cache.py` & `plextraktsync-0.30.5/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/clear_collections.py` & `plextraktsync-0.30.5/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/config.py` & `plextraktsync-0.30.5/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/download.py` & `plextraktsync-0.30.5/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/imdb_import.py` & `plextraktsync-0.30.5/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/info.py` & `plextraktsync-0.30.5/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/inspect.py` & `plextraktsync-0.30.5/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/login.py` & `plextraktsync-0.30.5/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/plex_login.py` & `plextraktsync-0.30.5/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/self_update.py` & `plextraktsync-0.30.5/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/sync.py` & `plextraktsync-0.30.5/plextraktsync/commands/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 from plextraktsync.decorators.measure_time import measure_time
 from plextraktsync.factory import factory, logging
 
 logger = logging.getLogger(__name__)
 
 
 @coro
-async def sync(
+async def run_async(runner, **kwargs):
+    await runner.sync(**kwargs)
+
+
+def sync(
     sync_option: str,
     library: str,
     show: str,
     movie: str,
     ids: list[str],
     server: str,
     batch_delay: int,
@@ -65,8 +69,8 @@
 
     with measure_time("Completed full sync"):
         runner = factory.sync
         if runner.config.need_library_walk:
             w.print_plan(print=logger.info)
         if dry_run:
             logger.info("Enabled dry-run mode: not making actual changes")
-        await runner.sync(walker=w, dry_run=config.dry_run)
+        run_async(runner, walker=w, dry_run=config.dry_run)
```

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/trakt_login.py` & `plextraktsync-0.30.5/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/unmatched.py` & `plextraktsync-0.30.5/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/watch.py` & `plextraktsync-0.30.5/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/commands/watched_shows.py` & `plextraktsync-0.30.5/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/config/Config.py` & `plextraktsync-0.30.5/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/config/ConfigLoader.py` & `plextraktsync-0.30.5/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/config/HttpCacheConfig.py` & `plextraktsync-0.30.5/plextraktsync/config/HttpCacheConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/config/PlexServerConfig.py` & `plextraktsync-0.30.5/plextraktsync/config/PlexServerConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/config/ServerConfigFactory.py` & `plextraktsync-0.30.5/plextraktsync/config/ServerConfigFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/config/SyncConfig.py` & `plextraktsync-0.30.5/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/config.default.yml` & `plextraktsync-0.30.5/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/decorators/measure_time.py` & `plextraktsync-0.30.5/plextraktsync/decorators/measure_time.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/decorators/rate_limit.py` & `plextraktsync-0.30.5/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/decorators/retry.py` & `plextraktsync-0.30.5/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/logger/filter.py` & `plextraktsync-0.30.5/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/logger/init.py` & `plextraktsync-0.30.5/plextraktsync/logger/init.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/media/Media.py` & `plextraktsync-0.30.5/plextraktsync/media/Media.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/media/MediaFactory.py` & `plextraktsync-0.30.5/plextraktsync/media/MediaFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/mixin/ChangeNotifier.py` & `plextraktsync-0.30.5/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plan/WalkConfig.py` & `plextraktsync-0.30.5/plextraktsync/plan/WalkConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plan/WalkPlanner.py` & `plextraktsync-0.30.5/plextraktsync/plan/WalkPlanner.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plan/Walker.py` & `plextraktsync-0.30.5/plextraktsync/plan/Walker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexApi.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexAudioCodec.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexGuid.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexGuidProvider.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexGuidProvider.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexGuidProviderMbid.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexGuidProviderMbid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexGuidProviderTMDB.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexGuidProviderTMDB.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexId.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexId.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexIdFactory.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexIdFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexLibraryItem.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexLibraryItem.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexLibrarySection.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexPlaylist.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexPlaylist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexRatings.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexSectionPager.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexSectionPager.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexServerConnection.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/PlexWatchList.py` & `plextraktsync-0.30.5/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/plex/SessionCollection.py` & `plextraktsync-0.30.5/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/pytrakt_extensions.py` & `plextraktsync-0.30.5/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/queue/BackgroundTask.py` & `plextraktsync-0.30.5/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/queue/Queue.py` & `plextraktsync-0.30.5/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/queue/TraktBatchWorker.py` & `plextraktsync-0.30.5/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/queue/TraktMarkWatchedWorker.py` & `plextraktsync-0.30.5/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/queue/TraktScrobbleWorker.py` & `plextraktsync-0.30.5/plextraktsync/queue/TraktScrobbleWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/rich/RichHighlighter.py` & `plextraktsync-0.30.5/plextraktsync/rich/RichHighlighter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/rich/RichProgressBar.py` & `plextraktsync-0.30.5/plextraktsync/rich/RichProgressBar.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/sync/AddCollectionPlugin.py` & `plextraktsync-0.30.5/plextraktsync/sync/AddCollectionPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/sync/ClearCollectedPlugin.py` & `plextraktsync-0.30.5/plextraktsync/sync/ClearCollectedPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/sync/LikedListsPlugin.py` & `plextraktsync-0.30.5/plextraktsync/sync/LikedListsPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/sync/Sync.py` & `plextraktsync-0.30.5/plextraktsync/sync/Sync.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/sync/SyncRatingsPlugin.py` & `plextraktsync-0.30.5/plextraktsync/sync/SyncRatingsPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/sync/SyncWatchedPlugin.py` & `plextraktsync-0.30.5/plextraktsync/sync/SyncWatchedPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/sync/TraktListsPlugin.py` & `plextraktsync-0.30.5/plextraktsync/sync/TraktListsPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/sync/WatchListPlugin.py` & `plextraktsync-0.30.5/plextraktsync/sync/WatchListPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/sync/WatchProgressPlugin.py` & `plextraktsync-0.30.5/plextraktsync/sync/WatchProgressPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/sync/plugin/SyncPluginInterface.py` & `plextraktsync-0.30.5/plextraktsync/sync/plugin/SyncPluginInterface.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/sync/plugin/SyncPluginManager.py` & `plextraktsync-0.30.5/plextraktsync/sync/plugin/SyncPluginManager.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/trakt/ScrobblerCollection.py` & `plextraktsync-0.30.5/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/trakt/ScrobblerProxy.py` & `plextraktsync-0.30.5/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/trakt/TraktApi.py` & `plextraktsync-0.30.5/plextraktsync/trakt/TraktApi.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/trakt/TraktLookup.py` & `plextraktsync-0.30.5/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/trakt/TraktRatingCollection.py` & `plextraktsync-0.30.5/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/trakt/TraktUserList.py` & `plextraktsync-0.30.5/plextraktsync/trakt/TraktUserList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/trakt/TraktUserListCollection.py` & `plextraktsync-0.30.5/plextraktsync/trakt/TraktUserListCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/trakt/TraktWatchlist.py` & `plextraktsync-0.30.5/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/trakt/WatchProgress.py` & `plextraktsync-0.30.5/plextraktsync/trakt/WatchProgress.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/util/Factory.py` & `plextraktsync-0.30.5/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/util/Path.py` & `plextraktsync-0.30.5/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/util/Rating.py` & `plextraktsync-0.30.5/plextraktsync/util/Rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/util/Timer.py` & `plextraktsync-0.30.5/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/util/Version.py` & `plextraktsync-0.30.5/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/util/local_url.py` & `plextraktsync-0.30.5/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/util/openurl.py` & `plextraktsync-0.30.5/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/util/packaging.py` & `plextraktsync-0.30.5/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/util/remove_empty_values.py` & `plextraktsync-0.30.5/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/watch/EventDispatcher.py` & `plextraktsync-0.30.5/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/watch/EventFactory.py` & `plextraktsync-0.30.5/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/watch/ProgressBar.py` & `plextraktsync-0.30.5/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/watch/WatchStateUpdater.py` & `plextraktsync-0.30.5/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/watch/WebSocketListener.py` & `plextraktsync-0.30.5/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/plextraktsync/watch/events.py` & `plextraktsync-0.30.5/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/requirements.txt` & `plextraktsync-0.30.5/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 mdurl==0.1.2; python_version >= '3.7'
 oauthlib==3.2.2; python_version >= '3.6'
 pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 platformdirs==4.2.1; python_version >= '3.7' and python_version >= '3.8'
 plexapi==4.15.12; python_version >= '3.8'
 pluggy==1.5.0; python_version >= '3.8'
 prompt-toolkit==3.0.43; python_full_version >= '3.7.0'
-pygments==2.17.2; python_version >= '3.7'
+pygments==2.18.0; python_version >= '3.8'
 python-dotenv==1.0.1; python_version >= '3.8'
 python-git-info==0.8.3
 pytimeparse==1.1.8
 pytrakt==3.4.32
 pyyaml==6.0.1; python_version >= '3.6'
 requests==2.31.0; python_version >= '3.7'
 requests-cache==1.2.0; python_version >= '3.8'
```

### Comparing `plextraktsync-0.30.4/setup.cfg` & `plextraktsync-0.30.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/tests/test_collection_metadata.py` & `plextraktsync-0.30.5/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/tests/test_config.py` & `plextraktsync-0.30.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/tests/test_events.py` & `plextraktsync-0.30.5/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/tests/test_new_agent.py` & `plextraktsync-0.30.5/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/tests/test_plex_id.py` & `plextraktsync-0.30.5/tests/test_plex_id.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/tests/test_rating.py` & `plextraktsync-0.30.5/tests/test_rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/tests/test_timer.py` & `plextraktsync-0.30.5/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/tests/test_trakt_progress.py` & `plextraktsync-0.30.5/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/tests/test_tv_lookup.py` & `plextraktsync-0.30.5/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.4/tests/test_walker.py` & `plextraktsync-0.30.5/tests/test_walker.py`

 * *Files identical despite different names*

