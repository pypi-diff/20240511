# Comparing `tmp/aliyun-python-sdk-live-3.9.8.tar.gz` & `tmp/aliyun-python-sdk-live-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-live-3.9.8.tar", last modified: Thu Jun 10 07:33:23 2021, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-live-3.9.9.tar", last modified: Thu Jul  8 02:32:30 2021, max compression
```

## Comparing `aliyun-python-sdk-live-3.9.8.tar` & `aliyun-python-sdk-live-3.9.9.tar`

### file list

```diff
@@ -1,263 +1,268 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-10 07:33:23.000000 aliyun-python-sdk-live-3.9.8/
--rw-r--r--   0 root         (0) root         (0)      575 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2021-06-10 07:33:23.000000 aliyun-python-sdk-live-3.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyun_python_sdk_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyun_python_sdk_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16532 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyun_python_sdk_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyun_python_sdk_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyun_python_sdk_live.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyun_python_sdk_live.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/
--rw-r--r--   0 root         (0) root         (0)       21 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3612 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-10 07:33:23.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/
--rw-r--r--   0 root         (0) root         (0)     3515 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterComponentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1783 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterEpisodeGroupContentRequest.py
--rw-r--r--   0 root         (0) root         (0)     2916 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterEpisodeGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2905 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterEpisodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     4317 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterLayoutRequest.py
--rw-r--r--   0 root         (0) root         (0)     3043 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterProgramRequest.py
--rw-r--r--   0 root         (0) root         (0)     3361 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterVideoResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     4005 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCustomLiveStreamTranscodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2401 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddDRMCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2601 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveASRConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3884 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveAppRecordConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3081 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveAppSnapshotConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2603 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveAudioAuditConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1993 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveAudioAuditNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1973 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveDetectNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1969 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveDomainMappingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1787 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveDomainPlayMappingRequest.py
--rw-r--r--   0 root         (0) root         (0)     2809 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2433 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLivePullStreamInfoConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2359 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveRecordNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3001 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveRecordVodConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2893 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveSnapshotDetectPornConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2227 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveStreamTranscodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2539 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddMultiRateConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2127 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddPlaylistItemsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4325 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddRtsLiveStreamTranscodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3005 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddStudioLayoutRequest.py
--rw-r--r--   0 root         (0) root         (0)     2501 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddTrancodeSEIRequest.py
--rw-r--r--   0 root         (0) root         (0)     1715 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AllowPushStreamRequest.py
--rw-r--r--   0 root         (0) root         (0)     1869 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ApplyBoardTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     1569 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ApplyRecordTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     2193 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/BatchDeleteLiveDomainConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2163 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/BatchSetLiveDomainConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2151 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CheckServiceForRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1921 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CloseLiveShiftRequest.py
--rw-r--r--   0 root         (0) root         (0)     1889 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CompleteBoardRecordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1717 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CompleteBoardRequest.py
--rw-r--r--   0 root         (0) root         (0)     2097 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ControlHtmlResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1943 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CopyCasterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1941 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CopyCasterSceneConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1707 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateBoardRequest.py
--rw-r--r--   0 root         (0) root         (0)     2653 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateCasterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2086 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateLiveRealTimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2977 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateLiveStreamRecordIndexFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2339 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateMixStreamRequest.py
--rw-r--r--   0 root         (0) root         (0)     2245 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateRoomRequest.py
--rw-r--r--   0 root         (0) root         (0)     1713 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteBoardRequest.py
--rw-r--r--   0 root         (0) root         (0)     1775 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterComponentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1609 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterEpisodeGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1759 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterEpisodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1751 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterLayoutRequest.py
--rw-r--r--   0 root         (0) root         (0)     1593 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterProgramRequest.py
--rw-r--r--   0 root         (0) root         (0)     1579 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1891 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterSceneConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1777 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterVideoResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1941 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteHtmlResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1931 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveASRConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2133 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveAppRecordConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1965 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveAppSnapshotConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1945 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveAudioAuditConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1631 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveAudioAuditNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1813 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveDetectNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1975 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveDomainMappingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1793 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveDomainPlayMappingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1973 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1789 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveLazyPullStreamInfoConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2143 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLivePullStreamInfoConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1914 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveRealTimeLogLogstoreRequest.py
--rw-r--r--   0 root         (0) root         (0)     2086 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1813 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveRecordNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1943 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveRecordVodConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1979 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveSnapshotDetectPornConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1979 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveSpecificStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2073 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveStreamTranscodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1631 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveStreamsNotifyUrlConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2101 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteMixStreamRequest.py
--rw-r--r--   0 root         (0) root         (0)     2225 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteMultiRateConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1795 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeletePlaylistItemsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1589 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeletePlaylistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1705 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteRoomRequest.py
--rw-r--r--   0 root         (0) root         (0)     1751 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteStudioLayoutRequest.py
--rw-r--r--   0 root         (0) root         (0)     2049 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeBoardEventsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1733 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeBoardSnapshotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1879 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeBoardsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1599 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterChannelsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1781 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterComponentsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1595 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1757 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterLayoutsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2723 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterProgramRequest.py
--rw-r--r--   0 root         (0) root         (0)     1597 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterRtcInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1757 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterSceneAudioRequest.py
--rw-r--r--   0 root         (0) root         (0)     1749 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterScenesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1601 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterStreamUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     1601 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterSyncGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1611 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterVideoResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2539 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCastersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1747 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeDRMCertListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2507 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeDomainUsageDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2057 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeForbidPushStreamRoomListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1774 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeHlsLiveStreamRealTimeBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1945 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeHtmlResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1935 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveAsrConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1949 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveAudioAuditConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1635 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveAudioAuditNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1803 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveCertificateDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1811 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveCertificateListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1817 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDetectNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2791 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDetectPornDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2155 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainBpsDataByTimeStampRequest.py
--rw-r--r--   0 root         (0) root         (0)     2459 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1633 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainCertificateInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1997 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1805 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1815 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainFrameRateAndBitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainLimitRequest.py
--rw-r--r--   0 root         (0) root         (0)     1616 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainMappingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1795 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainOnlineUserNumRequest.py
--rw-r--r--   0 root         (0) root         (0)     2467 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainPushBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2475 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainPushTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1939 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainPvUvDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2314 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2325 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2323 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1640 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2115 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainRecordDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1947 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainSnapshotDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1819 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2263 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainStreamTranscodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2109 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainTimeShiftDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2467 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1949 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainTranscodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1785 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveLazyPullStreamConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1623 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLivePullStreamConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2251 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveRealtimeDeliveryAccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1680 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveRealtimeLogAuthorizedRequest.py
--rw-r--r--   0 root         (0) root         (0)     2587 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveRecordConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1817 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveRecordNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2263 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveRecordVodConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1615 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveShiftConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2419 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveSnapshotConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2439 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveSnapshotDetectPornConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1437 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStagingIpRequest.py
--rw-r--r--   0 root         (0) root         (0)     2461 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamBitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1612 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1625 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamDelayConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2467 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamHistoryUserNumRequest.py
--rw-r--r--   0 root         (0) root         (0)     1819 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamOptimizedFeatureConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2465 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordContentRequest.py
--rw-r--r--   0 root         (0) root         (0)     2309 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordIndexFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     2927 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordIndexFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2747 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamSnapshotInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1683 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamTranscodeInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1639 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamTranscodeStreamNumRequest.py
--rw-r--r--   0 root         (0) root         (0)     2127 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamsBlockListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2107 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamsControlHistoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1635 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamsNotifyUrlConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2603 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamsOnlineListRequest.py
--rw-r--r--   0 root         (0) root         (0)     3097 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamsPublishListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2317 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1913 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveTopDomainsByFlowRequest.py
--rw-r--r--   0 root         (0) root         (0)     3295 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveUserDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1435 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveUserTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1617 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveVerifyContentRequest.py
--rw-r--r--   0 root         (0) root         (0)     2741 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeMixStreamListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1725 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeRecordRequest.py
--rw-r--r--   0 root         (0) root         (0)     2059 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2195 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeRoomKickoutUserListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2825 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeRoomListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1721 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeRoomStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1757 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeStudioLayoutsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2113 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeUpBpsPeakDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2253 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeUpBpsPeakOfLineRequest.py
--rw-r--r--   0 root         (0) root         (0)     2133 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeUpPeakPublishStreamDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1626 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DisableLiveRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2263 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/EditHtmlResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1959 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/EditPlaylistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1745 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/EffectCasterUrgentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1931 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/EffectCasterVideoResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1624 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/EnableLiveRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2447 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ForbidLiveStreamRequest.py
--rw-r--r--   0 root         (0) root         (0)     2031 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ForbidPushStreamRequest.py
--rw-r--r--   0 root         (0) root         (0)     1611 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/GetMultiRateConfigListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1887 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/GetMultiRateConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/JoinBoardRequest.py
--rw-r--r--   0 root         (0) root         (0)     1924 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1678 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryInfosRequest.py
--rw-r--r--   0 root         (0) root         (0)     1668 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1791 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ListPlaylistItemsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1881 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ListPlaylistRequest.py
--rw-r--r--   0 root         (0) root         (0)     3147 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyCasterComponentRequest.py
--rw-r--r--   0 root         (0) root         (0)     2899 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyCasterEpisodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     4483 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyCasterLayoutRequest.py
--rw-r--r--   0 root         (0) root         (0)     3209 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyCasterProgramRequest.py
--rw-r--r--   0 root         (0) root         (0)     3207 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyCasterVideoResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1789 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyLiveDomainSchdmByPropertyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2086 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyLiveRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2999 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyStudioLayoutRequest.py
--rw-r--r--   0 root         (0) root         (0)     2227 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/OpenLiveShiftRequest.py
--rw-r--r--   0 root         (0) root         (0)     1823 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/PublishLiveStagingConfigToProductionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2089 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/RealTimeRecordCommandRequest.py
--rw-r--r--   0 root         (0) root         (0)     2389 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/RealTimeSnapshotCommandRequest.py
--rw-r--r--   0 root         (0) root         (0)     2311 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ResumeLiveStreamRequest.py
--rw-r--r--   0 root         (0) root         (0)     1801 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/RollbackLiveStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2169 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SendRoomNotificationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2337 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SendRoomUserNotificationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2465 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetBoardCallbackRequest.py
--rw-r--r--   0 root         (0) root         (0)     2269 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetCasterChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     3591 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetCasterConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2207 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetCasterSceneConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2620 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetCasterSyncGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2759 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveDomainCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1785 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveDomainStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2341 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveLazyPullStreamInfoConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2587 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveStreamDelayConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2171 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveStreamOptimizedFeatureConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1791 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveStreamsNotifyUrlConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1889 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartBoardRecordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1577 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartCasterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1741 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartCasterSceneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1787 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartLiveDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     3077 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartLiveIndexRequest.py
--rw-r--r--   0 root         (0) root         (0)     2085 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartPlaylistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1575 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StopCasterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1739 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StopCasterSceneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1785 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StopLiveDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2067 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StopLiveIndexRequest.py
--rw-r--r--   0 root         (0) root         (0)     1585 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StopPlaylistRequest.py
--rw-r--r--   0 root         (0) root         (0)     2301 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/TagLiveResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2293 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UnTagLiveResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2471 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateBoardCallbackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1725 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateBoardRequest.py
--rw-r--r--   0 root         (0) root         (0)     2918 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateCasterSceneAudioRequest.py
--rw-r--r--   0 root         (0) root         (0)     2213 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateCasterSceneConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2607 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveASRConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3087 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveAppSnapshotConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2609 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveAudioAuditConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1999 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveAudioAuditNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1979 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveDetectNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2365 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveRecordNotifyConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2899 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveSnapshotDetectPornConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1847 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveTopLevelDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2137 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateMixStreamRequest.py
--rw-r--r--   0 root         (0) root         (0)     1781 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/VerifyLiveDomainOwnerRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-06-10 07:33:23.000000 aliyun-python-sdk-live-3.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2021-06-10 07:33:22.000000 aliyun-python-sdk-live-3.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyun_python_sdk_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyun_python_sdk_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16883 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyun_python_sdk_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyun_python_sdk_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyun_python_sdk_live.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyun_python_sdk_live.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3606 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/
+-rw-r--r--   0 root         (0) root         (0)     3515 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterComponentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterEpisodeGroupContentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterEpisodeGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterEpisodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4317 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterLayoutRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterProgramRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3361 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterVideoResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4623 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCustomLiveStreamTranscodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddDRMCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2601 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveASRConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3884 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveAppRecordConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3081 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveAppSnapshotConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveAudioAuditConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveAudioAuditNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveDetectNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveDomainMappingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveDomainPlayMappingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2809 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLivePullStreamInfoConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveRecordNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3001 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveRecordVodConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveSnapshotDetectPornConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveStreamTranscodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddMultiRateConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddPlaylistItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4325 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddRtsLiveStreamTranscodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddStudioLayoutRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddTrancodeSEIRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AllowPushStreamRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ApplyBoardTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ApplyRecordTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/BatchDeleteLiveDomainConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/BatchSetLiveDomainConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CheckServiceForRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CloseLiveShiftRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CompleteBoardRecordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CompleteBoardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ControlHtmlResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CopyCasterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CopyCasterSceneConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateBoardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2653 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateCasterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateLiveRealTimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2977 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateLiveStreamRecordIndexFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateMixStreamRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateRoomRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteBoardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterComponentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1609 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterEpisodeGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterEpisodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterLayoutRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterProgramRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterSceneConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterVideoResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteHtmlResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveASRConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveAppRecordConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveAppSnapshotConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveAudioAuditConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveAudioAuditNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveDetectNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1975 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveDomainMappingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveDomainPlayMappingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveLazyPullStreamInfoConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLivePullStreamInfoConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveRealTimeLogLogstoreRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveRecordNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveRecordVodConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveSnapshotDetectPornConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveSpecificStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveStreamTranscodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveStreamsNotifyUrlConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteMixStreamRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteMultiRateConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeletePlaylistItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeletePlaylistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteRoomRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteStudioLayoutRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeBoardEventsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeBoardSnapshotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeBoardsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterChannelsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterComponentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterLayoutsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterProgramRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterRtcInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterSceneAudioRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterScenesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterStreamUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterSyncGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterVideoResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCastersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeDRMCertListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2507 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeDomainUsageDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeForbidPushStreamRoomListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeHlsLiveStreamRealTimeBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeHtmlResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveAsrConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveAudioAuditConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveAudioAuditNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveCertificateDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveCertificateListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDetectNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDetectPornDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainBpsDataByTimeStampRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainCertificateInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainFrameRateAndBitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainLimitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainMappingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainOnlineUserNumRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainPushBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainPushTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainPvUvDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainRecordDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainRecordUsageDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainSnapshotDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainStreamTranscodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainTimeShiftDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainTranscodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDrmUsageDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1785 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveLazyPullStreamConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1623 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLivePullStreamConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveRealtimeDeliveryAccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveRealtimeLogAuthorizedRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveRecordConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveRecordNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveRecordVodConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveShiftConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveSnapshotConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2439 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveSnapshotDetectPornConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStagingIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2461 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamBitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamDelayConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamHistoryUserNumRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamOptimizedFeatureConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordContentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordIndexFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordIndexFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamSnapshotInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamTranscodeInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamTranscodeStreamNumRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamsBlockListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamsControlHistoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamsNotifyUrlConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamsOnlineListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamsPublishListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2317 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveTopDomainsByFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3295 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveUserDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveUserTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveVerifyContentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeMixStreamListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeRecordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeRoomKickoutUserListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeRoomListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeRoomStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeStudioLayoutsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeToutiaoLivePlayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeToutiaoLivePublishRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeUpBpsPeakDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeUpBpsPeakOfLineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeUpPeakPublishStreamDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DisableLiveRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/EditHtmlResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/EditPlaylistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/EffectCasterUrgentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/EffectCasterVideoResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/EnableLiveRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2447 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ForbidLiveStreamRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ForbidPushStreamRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/GetMultiRateConfigListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/GetMultiRateConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/JoinBoardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryInfosRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ListPlaylistItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ListPlaylistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyCasterComponentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2899 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyCasterEpisodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyCasterLayoutRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3209 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyCasterProgramRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3207 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyCasterVideoResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyLiveDomainSchdmByPropertyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyLiveRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyStudioLayoutRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/OpenLiveShiftRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/PublishLiveStagingConfigToProductionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/RealTimeRecordCommandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/RealTimeSnapshotCommandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ResumeLiveStreamRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/RollbackLiveStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SendRoomNotificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SendRoomUserNotificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetBoardCallbackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetCasterChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetCasterConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetCasterSceneConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetCasterSyncGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveDomainCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1785 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveDomainStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2341 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveLazyPullStreamInfoConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveStreamDelayConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveStreamOptimizedFeatureConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveStreamsNotifyUrlConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartBoardRecordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartCasterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartCasterSceneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartLiveDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartLiveIndexRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartPlaylistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StopCasterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StopCasterSceneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1785 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StopLiveDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StopLiveIndexRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StopPlaylistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/TagLiveResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UnTagLiveResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateBoardCallbackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateBoardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateCasterSceneAudioRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateCasterSceneConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveASRConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveAppSnapshotConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveAudioAuditConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveAudioAuditNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveDetectNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLivePullStreamInfoConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2365 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveRecordNotifyConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2899 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveSnapshotDetectPornConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveTopLevelDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateMixStreamRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/VerifyLiveDomainOwnerRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2021-07-08 02:32:30.000000 aliyun-python-sdk-live-3.9.9/setup.py
```

### Comparing `aliyun-python-sdk-live-3.9.8/LICENSE` & `aliyun-python-sdk-live-3.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/PKG-INFO` & `aliyun-python-sdk-live-3.9.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-live
-Version: 3.9.8
+Version: 3.9.9
 Summary: The live module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-live
```

### Comparing `aliyun-python-sdk-live-3.9.8/README.rst` & `aliyun-python-sdk-live-3.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyun_python_sdk_live.egg-info/PKG-INFO` & `aliyun-python-sdk-live-3.9.9/aliyun_python_sdk_live.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-live
-Version: 3.9.8
+Version: 3.9.9
 Summary: The live module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-live
```

### Comparing `aliyun-python-sdk-live-3.9.8/aliyun_python_sdk_live.egg-info/SOURCES.txt` & `aliyun-python-sdk-live-3.9.9/aliyun_python_sdk_live.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -132,20 +132,22 @@
 aliyunsdklive/request/v20161101/DescribeLiveDomainPushTrafficDataRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainPvUvDataRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeBpsDataRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeHttpCodeDataRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeTrafficDataRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainRealtimeLogDeliveryRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainRecordDataRequest.py
+aliyunsdklive/request/v20161101/DescribeLiveDomainRecordUsageDataRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainSnapshotDataRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainStagingConfigRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainStreamTranscodeDataRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainTimeShiftDataRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainTrafficDataRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveDomainTranscodeDataRequest.py
+aliyunsdklive/request/v20161101/DescribeLiveDrmUsageDataRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveLazyPullStreamConfigRequest.py
 aliyunsdklive/request/v20161101/DescribeLivePullStreamConfigRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveRealtimeDeliveryAccRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveRealtimeLogAuthorizedRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveRecordConfigRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveRecordNotifyConfigRequest.py
 aliyunsdklive/request/v20161101/DescribeLiveRecordVodConfigsRequest.py
@@ -177,14 +179,16 @@
 aliyunsdklive/request/v20161101/DescribeMixStreamListRequest.py
 aliyunsdklive/request/v20161101/DescribeRecordRequest.py
 aliyunsdklive/request/v20161101/DescribeRecordsRequest.py
 aliyunsdklive/request/v20161101/DescribeRoomKickoutUserListRequest.py
 aliyunsdklive/request/v20161101/DescribeRoomListRequest.py
 aliyunsdklive/request/v20161101/DescribeRoomStatusRequest.py
 aliyunsdklive/request/v20161101/DescribeStudioLayoutsRequest.py
+aliyunsdklive/request/v20161101/DescribeToutiaoLivePlayRequest.py
+aliyunsdklive/request/v20161101/DescribeToutiaoLivePublishRequest.py
 aliyunsdklive/request/v20161101/DescribeUpBpsPeakDataRequest.py
 aliyunsdklive/request/v20161101/DescribeUpBpsPeakOfLineRequest.py
 aliyunsdklive/request/v20161101/DescribeUpPeakPublishStreamDataRequest.py
 aliyunsdklive/request/v20161101/DisableLiveRealtimeLogDeliveryRequest.py
 aliyunsdklive/request/v20161101/EditHtmlResourceRequest.py
 aliyunsdklive/request/v20161101/EditPlaylistRequest.py
 aliyunsdklive/request/v20161101/EffectCasterUrgentRequest.py
@@ -245,13 +249,14 @@
 aliyunsdklive/request/v20161101/UpdateCasterSceneAudioRequest.py
 aliyunsdklive/request/v20161101/UpdateCasterSceneConfigRequest.py
 aliyunsdklive/request/v20161101/UpdateLiveASRConfigRequest.py
 aliyunsdklive/request/v20161101/UpdateLiveAppSnapshotConfigRequest.py
 aliyunsdklive/request/v20161101/UpdateLiveAudioAuditConfigRequest.py
 aliyunsdklive/request/v20161101/UpdateLiveAudioAuditNotifyConfigRequest.py
 aliyunsdklive/request/v20161101/UpdateLiveDetectNotifyConfigRequest.py
+aliyunsdklive/request/v20161101/UpdateLivePullStreamInfoConfigRequest.py
 aliyunsdklive/request/v20161101/UpdateLiveRecordNotifyConfigRequest.py
 aliyunsdklive/request/v20161101/UpdateLiveSnapshotDetectPornConfigRequest.py
 aliyunsdklive/request/v20161101/UpdateLiveTopLevelDomainRequest.py
 aliyunsdklive/request/v20161101/UpdateMixStreamRequest.py
 aliyunsdklive/request/v20161101/VerifyLiveDomainOwnerRequest.py
 aliyunsdklive/request/v20161101/__init__.py
```

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/endpoint.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/endpoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,56 +28,59 @@
 			"cn-hangzhou-internal-prod-1": "live.aliyuncs.com",
 			"cn-north-2-gov-1": "live.aliyuncs.com",
 			"cn-yushanfang": "live.aliyuncs.com",
 			"cn-qingdao-nebula": "live.aliyuncs.com",
 			"cn-beijing-finance-pop": "live.aliyuncs.com",
 			"cn-wuhan": "live.aliyuncs.com",
 			"cn-zhangjiakou": "live.aliyuncs.com",
-			"us-west-1": "live.ap-southeast-1.aliyuncs.com",
-			"rus-west-1-pop": "live.ap-southeast-1.aliyuncs.com",
+			"us-west-1": "live.aliyuncs.com",
+			"cn-zhangbei": "live.aliyuncs.com",
+			"rus-west-1-pop": "live.aliyuncs.com",
 			"cn-shanghai-et15-b01": "live.aliyuncs.com",
 			"cn-hangzhou-bj-b01": "live.aliyuncs.com",
 			"cn-zhangbei-na61-b01": "live.aliyuncs.com",
 			"ap-northeast-1": "live.aliyuncs.com",
+			"cn-huhehaote-nebula-1": "live.aliyuncs.com",
 			"cn-shanghai-et2-b01": "live.aliyuncs.com",
 			"ap-southeast-1": "live.aliyuncs.com",
-			"ap-southeast-2": "live.ap-southeast-1.aliyuncs.com",
-			"ap-southeast-3": "live.ap-southeast-1.aliyuncs.com",
+			"ap-southeast-2": "live.aliyuncs.com",
+			"ap-southeast-3": "live.aliyuncs.com",
 			"ap-southeast-5": "live.aliyuncs.com",
-			"us-east-1": "live.ap-southeast-1.aliyuncs.com",
+			"us-east-1": "live.aliyuncs.com",
 			"cn-shenzhen-inner": "live.aliyuncs.com",
 			"cn-zhangjiakou-na62-a01": "live.aliyuncs.com",
 			"cn-beijing-gov-1": "live.aliyuncs.com",
+			"cn-wulanchabu": "live.aliyuncs.com",
 			"ap-south-1": "live.aliyuncs.com",
 			"cn-shenzhen-st4-d01": "live.aliyuncs.com",
 			"cn-haidian-cm12-c01": "live.aliyuncs.com",
 			"cn-qingdao": "live.aliyuncs.com",
 			"cn-hongkong-finance-pop": "live.aliyuncs.com",
 			"cn-shanghai": "live.aliyuncs.com",
 			"cn-shanghai-finance-1": "live.aliyuncs.com",
 			"cn-hongkong": "live.aliyuncs.com",
 			"eu-central-1": "live.aliyuncs.com",
 			"cn-shenzhen": "live.aliyuncs.com",
 			"cn-zhengzhou-nebula-1": "live.aliyuncs.com",
-			"eu-west-1": "live.ap-southeast-1.aliyuncs.com",
+			"eu-west-1": "live.aliyuncs.com",
 			"cn-hangzhou-internal-test-1": "live.aliyuncs.com",
-			"eu-west-1-oxs": "live.ap-southeast-1.aliyuncs.com",
+			"eu-west-1-oxs": "live.aliyuncs.com",
 			"cn-beijing-finance-1": "live.aliyuncs.com",
 			"cn-hangzhou-internal-test-3": "live.aliyuncs.com",
 			"cn-hangzhou-internal-test-2": "live.aliyuncs.com",
 			"cn-shenzhen-finance-1": "live.aliyuncs.com",
-			"me-east-1": "live.ap-southeast-1.aliyuncs.com",
+			"me-east-1": "live.aliyuncs.com",
 			"cn-chengdu": "live.aliyuncs.com",
 			"cn-hangzhou-test-306": "live.aliyuncs.com",
 			"cn-hangzhou-finance": "live.aliyuncs.com",
 			"cn-beijing-nu16-b01": "live.aliyuncs.com",
 			"cn-edge-1": "live.aliyuncs.com",
 			"cn-huhehaote": "live.aliyuncs.com",
 			"cn-fujian": "live.aliyuncs.com",
-			"ap-northeast-2-pop": "live.ap-southeast-1.aliyuncs.com",
+			"ap-northeast-2-pop": "live.aliyuncs.com",
 			"cn-hangzhou": "live.aliyuncs.com",
 		}
 		self.endpoint_regional = "regional"
 
 	def getEndpointMap(self):
 		return self.endpoint_map
```

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterComponentRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterComponentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterEpisodeGroupContentRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterEpisodeGroupContentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterEpisodeGroupRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterEpisodeGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterEpisodeRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterEpisodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterLayoutRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterLayoutRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterProgramRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterProgramRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCasterVideoResourceRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCasterVideoResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddCustomLiveStreamTranscodeRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddCustomLiveStreamTranscodeRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,32 +33,38 @@
 
 	def get_Template(self):
 		return self.get_query_params().get('Template')
 
 	def set_Template(self,Template):
 		self.add_query_param('Template',Template)
 
-	def get_Lazy(self):
-		return self.get_query_params().get('Lazy')
-
-	def set_Lazy(self,Lazy):
-		self.add_query_param('Lazy',Lazy)
-
 	def get_Gop(self):
 		return self.get_query_params().get('Gop')
 
 	def set_Gop(self,Gop):
 		self.add_query_param('Gop',Gop)
 
+	def get_KmsKeyExpireInterval(self):
+		return self.get_query_params().get('KmsKeyExpireInterval')
+
+	def set_KmsKeyExpireInterval(self,KmsKeyExpireInterval):
+		self.add_query_param('KmsKeyExpireInterval',KmsKeyExpireInterval)
+
 	def get_AudioCodec(self):
 		return self.get_query_params().get('AudioCodec')
 
 	def set_AudioCodec(self,AudioCodec):
 		self.add_query_param('AudioCodec',AudioCodec)
 
+	def get_KmsUID(self):
+		return self.get_query_params().get('KmsUID')
+
+	def set_KmsUID(self,KmsUID):
+		self.add_query_param('KmsUID',KmsUID)
+
 	def get_TemplateType(self):
 		return self.get_query_params().get('TemplateType')
 
 	def set_TemplateType(self,TemplateType):
 		self.add_query_param('TemplateType',TemplateType)
 
 	def get_AudioProfile(self):
@@ -75,14 +81,20 @@
 
 	def get_App(self):
 		return self.get_query_params().get('App')
 
 	def set_App(self,App):
 		self.add_query_param('App',App)
 
+	def get_EncryptParameters(self):
+		return self.get_query_params().get('EncryptParameters')
+
+	def set_EncryptParameters(self,EncryptParameters):
+		self.add_query_param('EncryptParameters',EncryptParameters)
+
 	def get_AudioChannelNum(self):
 		return self.get_query_params().get('AudioChannelNum')
 
 	def set_AudioChannelNum(self,AudioChannelNum):
 		self.add_query_param('AudioChannelNum',AudioChannelNum)
 
 	def get_Profile(self):
@@ -127,8 +139,14 @@
 	def set_Width(self,Width):
 		self.add_query_param('Width',Width)
 
 	def get_VideoBitrate(self):
 		return self.get_query_params().get('VideoBitrate')
 
 	def set_VideoBitrate(self,VideoBitrate):
-		self.add_query_param('VideoBitrate',VideoBitrate)
+		self.add_query_param('VideoBitrate',VideoBitrate)
+
+	def get_KmsKeyID(self):
+		return self.get_query_params().get('KmsKeyID')
+
+	def set_KmsKeyID(self,KmsKeyID):
+		self.add_query_param('KmsKeyID',KmsKeyID)
```

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddDRMCertificateRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddDRMCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveASRConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveASRConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveAppRecordConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveAppRecordConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveAppSnapshotConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveAppSnapshotConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveAudioAuditConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveAudioAuditConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveAudioAuditNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveAudioAuditNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveDetectNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveDetectNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveDomainMappingRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveDomainMappingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveDomainPlayMappingRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveDomainPlayMappingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveDomainRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLivePullStreamInfoConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLivePullStreamInfoConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveRecordNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveRecordNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveRecordVodConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveRecordVodConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveSnapshotDetectPornConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveSnapshotDetectPornConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddLiveStreamTranscodeRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddLiveStreamTranscodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddMultiRateConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddMultiRateConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddPlaylistItemsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddPlaylistItemsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddRtsLiveStreamTranscodeRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddRtsLiveStreamTranscodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddStudioLayoutRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddStudioLayoutRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AddTrancodeSEIRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AddTrancodeSEIRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/AllowPushStreamRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/AllowPushStreamRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ApplyBoardTokenRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ApplyBoardTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ApplyRecordTokenRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ApplyRecordTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/BatchDeleteLiveDomainConfigsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/BatchDeleteLiveDomainConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/BatchSetLiveDomainConfigsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/BatchSetLiveDomainConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CheckServiceForRoleRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CheckServiceForRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CloseLiveShiftRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CloseLiveShiftRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CompleteBoardRecordRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CompleteBoardRecordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CompleteBoardRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CompleteBoardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ControlHtmlResourceRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ControlHtmlResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CopyCasterRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CopyCasterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CopyCasterSceneConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CopyCasterSceneConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateBoardRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateBoardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateCasterRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateCasterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateLiveRealTimeLogDeliveryRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateLiveRealTimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateLiveStreamRecordIndexFilesRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateLiveStreamRecordIndexFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateMixStreamRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateMixStreamRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/CreateRoomRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/CreateRoomRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteBoardRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteBoardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterComponentRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterComponentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterEpisodeGroupRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterEpisodeGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterEpisodeRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterEpisodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterLayoutRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterLayoutRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterProgramRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterProgramRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterSceneConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterSceneConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteCasterVideoResourceRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteCasterVideoResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteHtmlResourceRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteHtmlResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveASRConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveASRConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveAppRecordConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveAppRecordConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveAppSnapshotConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveAppSnapshotConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveAudioAuditConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveAudioAuditConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveAudioAuditNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveAudioAuditNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveDetectNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveDetectNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveDomainMappingRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveDomainMappingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveDomainPlayMappingRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveDomainPlayMappingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveDomainRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveLazyPullStreamInfoConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveLazyPullStreamInfoConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLivePullStreamInfoConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLivePullStreamInfoConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveRealTimeLogLogstoreRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveRealTimeLogLogstoreRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveRecordNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveRecordNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveRecordVodConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveRecordVodConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveSnapshotDetectPornConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveSnapshotDetectPornConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveSpecificStagingConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveSpecificStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveStreamTranscodeRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveStreamTranscodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteLiveStreamsNotifyUrlConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteLiveStreamsNotifyUrlConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteMixStreamRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteMixStreamRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteMultiRateConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteMultiRateConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeletePlaylistItemsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeletePlaylistItemsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeletePlaylistRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeletePlaylistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteRoomRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteRoomRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DeleteStudioLayoutRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DeleteStudioLayoutRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeBoardEventsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeBoardEventsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeBoardSnapshotRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeBoardSnapshotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeBoardsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeBoardsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterChannelsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterChannelsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterComponentsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterComponentsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterLayoutsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterLayoutsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterProgramRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterProgramRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterRtcInfoRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterRtcInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterSceneAudioRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterSceneAudioRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterScenesRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterScenesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterStreamUrlRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterStreamUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterSyncGroupRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterSyncGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCasterVideoResourcesRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCasterVideoResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeCastersRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeCastersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeDRMCertListRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeDRMCertListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeDomainUsageDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeDomainUsageDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeForbidPushStreamRoomListRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeForbidPushStreamRoomListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeHlsLiveStreamRealTimeBpsDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeHlsLiveStreamRealTimeBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeHtmlResourceRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeHtmlResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveAsrConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveAsrConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveAudioAuditConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveAudioAuditConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveAudioAuditNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveAudioAuditNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveCertificateDetailRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveCertificateDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveCertificateListRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveCertificateListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDetectNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDetectNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDetectPornDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDetectPornDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainBpsDataByTimeStampRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainBpsDataByTimeStampRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainBpsDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainCertificateInfoRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainCertificateInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainConfigsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainDetailRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainFrameRateAndBitRateDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainFrameRateAndBitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainLimitRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainLimitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainMappingRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainMappingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainOnlineUserNumRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainOnlineUserNumRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainPushBpsDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainPushBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainPushTrafficDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainPushTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainPvUvDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainPvUvDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeBpsDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeHttpCodeDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeTrafficDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainRealTimeTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainRecordDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainRecordDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainSnapshotDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainSnapshotDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainStagingConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainStreamTranscodeDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainStreamTranscodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainTimeShiftDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainTimeShiftDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainTrafficDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveDomainTranscodeDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveDomainTranscodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveLazyPullStreamConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveLazyPullStreamConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLivePullStreamConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLivePullStreamConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveRealtimeDeliveryAccRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveRealtimeDeliveryAccRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,20 @@
 
 	def get_StartTime(self):
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self,StartTime):
 		self.add_query_param('StartTime',StartTime)
 
+	def get_DomainName(self):
+		return self.get_query_params().get('DomainName')
+
+	def set_DomainName(self,DomainName):
+		self.add_query_param('DomainName',DomainName)
+
 	def get_EndTime(self):
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self,EndTime):
 		self.add_query_param('EndTime',EndTime)
 
 	def get_OwnerId(self):
```

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveRealtimeLogAuthorizedRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveRealtimeLogAuthorizedRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveRecordConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveRecordConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveRecordNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveRecordNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveRecordVodConfigsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveRecordVodConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveShiftConfigsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveShiftConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveSnapshotConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveSnapshotConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveSnapshotDetectPornConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveSnapshotDetectPornConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStagingIpRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStagingIpRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamBitRateDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamBitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamCountRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamDelayConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamDelayConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamHistoryUserNumRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamHistoryUserNumRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamOptimizedFeatureConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamOptimizedFeatureConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordContentRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordContentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordIndexFileRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordIndexFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordIndexFilesRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamRecordIndexFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamSnapshotInfoRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamSnapshotInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamTranscodeInfoRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamTranscodeInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamTranscodeStreamNumRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamTranscodeStreamNumRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamsBlockListRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamsBlockListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamsControlHistoryRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamsControlHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamsNotifyUrlConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamsNotifyUrlConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamsOnlineListRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamsOnlineListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveStreamsPublishListRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveStreamsPublishListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveTagResourcesRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveTopDomainsByFlowRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveTopDomainsByFlowRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveUserDomainsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveUserDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveUserTagsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveUserTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeLiveVerifyContentRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeLiveVerifyContentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeMixStreamListRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeMixStreamListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeRecordRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeRecordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeRecordsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeRoomKickoutUserListRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeRoomKickoutUserListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeRoomListRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeRoomListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeRoomStatusRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeRoomStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeStudioLayoutsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeStudioLayoutsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeUpBpsPeakDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeUpBpsPeakDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeUpBpsPeakOfLineRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeUpBpsPeakOfLineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DescribeUpPeakPublishStreamDataRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DescribeUpPeakPublishStreamDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/DisableLiveRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/DisableLiveRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/EditHtmlResourceRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/EditHtmlResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/EditPlaylistRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/EditPlaylistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/EffectCasterUrgentRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/EffectCasterUrgentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/EffectCasterVideoResourceRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/EffectCasterVideoResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/EnableLiveRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/EnableLiveRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ForbidLiveStreamRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ForbidLiveStreamRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ForbidPushStreamRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ForbidPushStreamRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/GetMultiRateConfigListRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/GetMultiRateConfigListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/GetMultiRateConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/GetMultiRateConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/JoinBoardRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/JoinBoardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryDomainsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryInfosRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryInfosRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ListLiveRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ListPlaylistItemsRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ListPlaylistItemsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ListPlaylistRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ListPlaylistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyCasterComponentRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyCasterComponentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyCasterEpisodeRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyCasterEpisodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyCasterLayoutRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyCasterLayoutRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyCasterProgramRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyCasterProgramRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyCasterVideoResourceRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyCasterVideoResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyLiveDomainSchdmByPropertyRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyLiveDomainSchdmByPropertyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyLiveRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyLiveRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ModifyStudioLayoutRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ModifyStudioLayoutRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/OpenLiveShiftRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/OpenLiveShiftRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/PublishLiveStagingConfigToProductionRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/PublishLiveStagingConfigToProductionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/RealTimeRecordCommandRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/RealTimeRecordCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/RealTimeSnapshotCommandRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/RealTimeSnapshotCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/ResumeLiveStreamRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/ResumeLiveStreamRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/RollbackLiveStagingConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/RollbackLiveStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SendRoomNotificationRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SendRoomNotificationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SendRoomUserNotificationRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SendRoomUserNotificationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetBoardCallbackRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetBoardCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetCasterChannelRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetCasterChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetCasterConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetCasterConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetCasterSceneConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetCasterSceneConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetCasterSyncGroupRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetCasterSyncGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveDomainCertificateRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveDomainCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveDomainStagingConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveDomainStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveLazyPullStreamInfoConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveLazyPullStreamInfoConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveStreamDelayConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveStreamDelayConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveStreamOptimizedFeatureConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveStreamOptimizedFeatureConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/SetLiveStreamsNotifyUrlConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/SetLiveStreamsNotifyUrlConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartBoardRecordRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartBoardRecordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartCasterRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartCasterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartCasterSceneRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartCasterSceneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartLiveDomainRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartLiveDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartLiveIndexRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartLiveIndexRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StartPlaylistRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StartPlaylistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StopCasterRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StopCasterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StopCasterSceneRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StopCasterSceneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StopLiveDomainRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StopLiveDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StopLiveIndexRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StopLiveIndexRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/StopPlaylistRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/StopPlaylistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/TagLiveResourcesRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/TagLiveResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UnTagLiveResourcesRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UnTagLiveResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateBoardCallbackRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateBoardCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateBoardRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateBoardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateCasterSceneAudioRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateCasterSceneAudioRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateCasterSceneConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateCasterSceneConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveASRConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveASRConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveAppSnapshotConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveAppSnapshotConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveAudioAuditConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveAudioAuditConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveAudioAuditNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveAudioAuditNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveDetectNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveDetectNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveRecordNotifyConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveRecordNotifyConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveSnapshotDetectPornConfigRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveSnapshotDetectPornConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateLiveTopLevelDomainRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateLiveTopLevelDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/UpdateMixStreamRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/UpdateMixStreamRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/aliyunsdklive/request/v20161101/VerifyLiveDomainOwnerRequest.py` & `aliyun-python-sdk-live-3.9.9/aliyunsdklive/request/v20161101/VerifyLiveDomainOwnerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-live-3.9.8/setup.py` & `aliyun-python-sdk-live-3.9.9/setup.py`

 * *Files identical despite different names*

