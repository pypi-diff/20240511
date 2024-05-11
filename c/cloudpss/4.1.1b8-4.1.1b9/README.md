# Comparing `tmp/cloudpss-4.1.1b8.tar.gz` & `tmp/cloudpss-4.1.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpss-4.1.1b8.tar", last modified: Fri Jan 12 06:55:01 2024, max compression
+gzip compressed data, was "dist\cloudpss-4.1.1b9.tar", last modified: Tue Apr  2 10:11:25 2024, max compression
```

## Comparing `cloudpss-4.1.1b8.tar` & `cloudpss-4.1.1b9.tar`

### file list

```diff
@@ -1,108 +1,120 @@
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/
--rw-rw-rw-   0        0        0     2103 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/PKG-INFO
--rw-rw-rw-   0        0        0     1760 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/
--rw-rw-rw-   0        0        0      835 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/dslab/
--rw-rw-rw-   0        0        0       45 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/dslab/__init__.py
--rw-rw-rw-   0        0        0    11527 2024-01-12 06:54:44.000000 cloudpss-4.1.1b8/cloudpss/dslab/dataManageModel.py
--rw-rw-rw-   0        0        0     8856 2024-01-12 06:52:55.000000 cloudpss-4.1.1b8/cloudpss/dslab/dslab.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/dslab/files/
--rw-rw-rw-   0        0        0       58 2024-01-12 06:52:49.000000 cloudpss-4.1.1b8/cloudpss/dslab/files/__init__.py
--rw-rw-rw-   0        0        0  4291778 2024-01-12 06:54:44.000000 cloudpss-4.1.1b8/cloudpss/dslab/files/curveData.py
--rw-rw-rw-   0        0        0      934 2024-01-12 06:54:44.000000 cloudpss-4.1.1b8/cloudpss/dslab/files/files.py
--rw-rw-rw-   0        0        0     5062 2024-01-12 06:52:55.000000 cloudpss-4.1.1b8/cloudpss/dslab/financialAnalysisModel.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/function/
--rw-rw-rw-   0        0        0     1629 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/function/__init__.py
--rw-rw-rw-   0        0        0       29 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/function/function.py
--rw-rw-rw-   0        0        0    14645 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/function/functionExecution.py
--rw-rw-rw-   0        0        0    13162 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/function/job.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/ieslab/
--rw-rw-rw-   0        0        0    19445 2023-12-27 10:11:11.000000 cloudpss-4.1.1b8/cloudpss/ieslab/DataManageModel.py
--rw-rw-rw-   0        0        0     6721 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/ieslab/EvaluationModel.py
--rw-rw-rw-   0        0        0     4940 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/ieslab/IESLabPlan.py
--rw-rw-rw-   0        0        0     3090 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/ieslab/IESLabSimulation.py
--rw-rw-rw-   0        0        0     4790 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/ieslab/PlanModel.py
--rw-rw-rw-   0        0        0      186 2023-07-10 05:15:47.000000 cloudpss-4.1.1b8/cloudpss/ieslab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/job/
--rw-rw-rw-   0        0        0       51 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/__init__.py
--rw-rw-rw-   0        0        0     8600 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/job.py
--rw-rw-rw-   0        0        0      268 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/jobMachine.py
--rw-rw-rw-   0        0        0     4083 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/jobPolicy.py
--rw-rw-rw-   0        0        0      416 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/jobQueue.py
--rw-rw-rw-   0        0        0      740 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/jobReceiver.py
--rw-rw-rw-   0        0        0      148 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/jobTres.py
--rw-rw-rw-   0        0        0     6048 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/messageStreamReceiver.py
--rw-rw-rw-   0        0        0     3797 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/messageStreamSender.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/job/view/
--rw-rw-rw-   0        0        0     6838 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/view/EMTView.py
--rw-rw-rw-   0        0        0       76 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/view/IESLabSimulationView.py
--rw-rw-rw-   0        0        0     1168 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/view/IESLabTypicalDayView.py
--rw-rw-rw-   0        0        0     3842 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/view/IESView.py
--rw-rw-rw-   0        0        0     2089 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/view/PowerFlowView.py
--rw-rw-rw-   0        0        0     1466 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/view/__init__.py
--rw-rw-rw-   0        0        0     3453 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/job/view/view.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/model/
--rw-rw-rw-   0        0        0      151 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/model/implements/
--rw-rw-rw-   0        0        0       67 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/model/implements/__init__.py
--rw-rw-rw-   0        0        0      734 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/model/implements/component.py
--rw-rw-rw-   0        0        0     1063 2024-01-12 06:52:49.000000 cloudpss-4.1.1b8/cloudpss/model/implements/diagram.py
--rw-rw-rw-   0        0        0      954 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/model/implements/implement.py
--rw-rw-rw-   0        0        0     3770 2023-07-10 05:15:47.000000 cloudpss-4.1.1b8/cloudpss/model/jobDefinitions.py
--rw-rw-rw-   0        0        0    26562 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/model/model.py
--rw-rw-rw-   0        0        0     4183 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/model/revision.py
--rw-rw-rw-   0        0        0     2516 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/model/topology.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/project/
--rw-rw-rw-   0        0        0       51 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/project/__init__.py
--rw-rw-rw-   0        0        0    17698 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/project/project.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/runner/
--rw-rw-rw-   0        0        0     3422 2024-01-12 06:52:55.000000 cloudpss-4.1.1b8/cloudpss/runner/DSLabResult.py
--rw-rw-rw-   0        0        0     5841 2023-07-10 05:15:47.000000 cloudpss-4.1.1b8/cloudpss/runner/IESLabEvaluationResult.py
--rw-rw-rw-   0        0        0     6862 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/runner/IESLabPlanResult.py
--rw-rw-rw-   0        0        0     8001 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/runner/IESLabTypicalDayResult.py
--rw-rw-rw-   0        0        0     5883 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/runner/MessageStreamReceiver.py
--rw-rw-rw-   0        0        0      341 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/runner/__init__.py
--rw-rw-rw-   0        0        0     4162 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/runner/receiver.py
--rw-rw-rw-   0        0        0    13125 2023-07-10 05:15:47.000000 cloudpss-4.1.1b8/cloudpss/runner/result.py
--rw-rw-rw-   0        0        0     7820 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/runner/runner.py
--rw-rw-rw-   0        0        0     4162 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/runner/storage.py
--rw-rw-rw-   0        0        0    11613 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/runner/transform.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss/utils/
--rw-rw-rw-   0        0        0      781 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/utils/AsyncIterable.py
--rw-rw-rw-   0        0        0     5314 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/utils/IO.py
--rw-rw-rw-   0        0        0      326 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/utils/__init__.py
--rw-rw-rw-   0        0        0      885 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/utils/dataEncoder.py
--rw-rw-rw-   0        0        0      255 2023-11-29 02:43:45.000000 cloudpss-4.1.1b8/cloudpss/utils/graphqlUtil.py
--rw-rw-rw-   0        0        0     2689 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/utils/httpAsyncRequest.py
--rw-rw-rw-   0        0        0     1733 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/utils/httprequests.py
--rw-rw-rw-   0        0        0      795 2023-01-12 12:36:01.000000 cloudpss-4.1.1b8/cloudpss/utils/matlab.py
--rw-rw-rw-   0        0        0     2677 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/utils/yamlLoader.py
--rw-rw-rw-   0        0        0     1498 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/cloudpss/verify.py
--rw-rw-rw-   0        0        0       28 2024-01-12 06:54:50.000000 cloudpss-4.1.1b8/cloudpss/version.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/cloudpss.egg-info/
--rw-rw-rw-   0        0        0     2103 2024-01-12 06:55:00.000000 cloudpss-4.1.1b8/cloudpss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2535 2024-01-12 06:55:00.000000 cloudpss-4.1.1b8/cloudpss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-12 06:55:00.000000 cloudpss-4.1.1b8/cloudpss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2024-01-12 06:55:00.000000 cloudpss-4.1.1b8/cloudpss.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-01-12 06:55:00.000000 cloudpss-4.1.1b8/cloudpss.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/setup.cfg
--rw-rw-rw-   0        0        0      880 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-12 06:55:01.000000 cloudpss-4.1.1b8/test/
--rw-rw-rw-   0        0        0      523 2023-12-27 12:07:35.000000 cloudpss-4.1.1b8/test/test-async.py
--rw-rw-rw-   0        0        0     1719 2023-12-27 12:10:15.000000 cloudpss-4.1.1b8/test/test-async2.py
--rw-rw-rw-   0        0        0      846 2023-12-28 08:14:48.000000 cloudpss-4.1.1b8/test/test-async3.py
--rw-rw-rw-   0        0        0     1097 2023-05-30 02:30:39.000000 cloudpss-4.1.1b8/test/test-sdk.py
--rw-rw-rw-   0        0        0     1359 2023-12-14 10:07:50.000000 cloudpss-4.1.1b8/test/test-sdk1.py
--rw-rw-rw-   0        0        0     3091 2023-05-30 02:30:39.000000 cloudpss-4.1.1b8/test/test-snapshot.py
--rw-rw-rw-   0        0        0     1064 2023-11-28 11:24:47.000000 cloudpss-4.1.1b8/test/test-topology.py
--rw-rw-rw-   0        0        0     1083 2024-01-12 06:54:39.000000 cloudpss-4.1.1b8/test/test.py
--rw-rw-rw-   0        0        0     1142 2023-09-27 07:50:35.000000 cloudpss-4.1.1b8/test/test7950.py
--rw-rw-rw-   0        0        0      854 2023-09-20 03:47:30.000000 cloudpss-4.1.1b8/test/testAsync.py
--rw-rw-rw-   0        0        0     1569 2023-09-25 06:50:28.000000 cloudpss-4.1.1b8/test/testEvent.py
--rw-rw-rw-   0        0        0     3127 2023-09-21 07:38:49.000000 cloudpss-4.1.1b8/test/testRt copy.py
--rw-rw-rw-   0        0        0     5065 2023-09-25 06:50:27.000000 cloudpss-4.1.1b8/test/testRt.py
--rw-rw-rw-   0        0        0     1382 2023-09-22 02:14:32.000000 cloudpss-4.1.1b8/test/testSend.py
--rw-rw-rw-   0        0        0     5350 2023-07-31 07:18:47.000000 cloudpss-4.1.1b8/test/test_in_new_web_1.py
--rw-rw-rw-   0        0        0     2217 2023-12-28 10:14:00.000000 cloudpss-4.1.1b8/test/test_ws.py
--rw-rw-rw-   0        0        0      302 2023-09-21 09:28:41.000000 cloudpss-4.1.1b8/test/testb.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/
+-rw-rw-rw-   0        0        0     2103 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/PKG-INFO
+-rw-rw-rw-   0        0        0     1760 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/
+-rw-rw-rw-   0        0        0      835 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/asyncio/
+-rw-rw-rw-   0        0        0      198 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/asyncio/job/
+-rw-rw-rw-   0        0        0       51 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/job/__init__.py
+-rw-rw-rw-   0        0        0     3891 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/job/job.py
+-rw-rw-rw-   0        0        0     3864 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/job/messageStreamReceiver.py
+-rw-rw-rw-   0        0        0     1594 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/job/messageStreamSender.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/asyncio/model/
+-rw-rw-rw-   0        0        0      151 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/model/__init__.py
+-rw-rw-rw-   0        0        0     8627 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/model/model.py
+-rw-rw-rw-   0        0        0     1568 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/model/revision.py
+-rw-rw-rw-   0        0        0     1192 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/model/topology.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/asyncio/utils/
+-rw-rw-rw-   0        0        0      781 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/utils/AsyncIterable.py
+-rw-rw-rw-   0        0        0       84 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/utils/__init__.py
+-rw-rw-rw-   0        0        0     2692 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/asyncio/utils/httpAsyncRequest.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/dslab/
+-rw-rw-rw-   0        0        0       45 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/dslab/__init__.py
+-rw-rw-rw-   0        0        0    11527 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/dslab/dataManageModel.py
+-rw-rw-rw-   0        0        0    13511 2024-04-02 03:51:35.000000 cloudpss-4.1.1b9/cloudpss/dslab/dslab.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/dslab/files/
+-rw-rw-rw-   0        0        0       58 2024-04-02 03:50:52.000000 cloudpss-4.1.1b9/cloudpss/dslab/files/__init__.py
+-rw-rw-rw-   0        0        0  4291778 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/dslab/files/curveData.py
+-rw-rw-rw-   0        0        0      934 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/dslab/files/files.py
+-rw-rw-rw-   0        0        0     5062 2024-04-02 03:50:52.000000 cloudpss-4.1.1b9/cloudpss/dslab/financialAnalysisModel.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/function/
+-rw-rw-rw-   0        0        0     1629 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/cloudpss/function/__init__.py
+-rw-rw-rw-   0        0        0       29 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/cloudpss/function/function.py
+-rw-rw-rw-   0        0        0    14894 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/function/functionExecution.py
+-rw-rw-rw-   0        0        0    13162 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/cloudpss/function/job.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/ieslab/
+-rw-rw-rw-   0        0        0    21921 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/ieslab/DataManageModel.py
+-rw-rw-rw-   0        0        0     6721 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/ieslab/EvaluationModel.py
+-rw-rw-rw-   0        0        0     8329 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/ieslab/IESLabPlan.py
+-rw-rw-rw-   0        0        0     4046 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/ieslab/IESLabSimulation.py
+-rw-rw-rw-   0        0        0     4883 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/ieslab/PlanModel.py
+-rw-rw-rw-   0        0        0      186 2023-07-10 05:15:47.000000 cloudpss-4.1.1b9/cloudpss/ieslab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/job/
+-rw-rw-rw-   0        0        0       51 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/job/__init__.py
+-rw-rw-rw-   0        0        0     7930 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/job/job.py
+-rw-rw-rw-   0        0        0      919 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/job/jobReceiver.py
+-rw-rw-rw-   0        0        0     4133 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/job/messageStreamReceiver.py
+-rw-rw-rw-   0        0        0     2371 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/job/messageStreamSender.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/job/view/
+-rw-rw-rw-   0        0        0     6933 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/job/view/EMTView.py
+-rw-rw-rw-   0        0        0       76 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/job/view/IESLabSimulationView.py
+-rw-rw-rw-   0        0        0     7817 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/job/view/IESLabTypicalDayView.py
+-rw-rw-rw-   0        0        0     3842 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/job/view/IESView.py
+-rw-rw-rw-   0        0        0     2089 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/job/view/PowerFlowView.py
+-rw-rw-rw-   0        0        0     1466 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/job/view/__init__.py
+-rw-rw-rw-   0        0        0     4280 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/job/view/view.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/model/
+-rw-rw-rw-   0        0        0      151 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/cloudpss/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/model/implements/
+-rw-rw-rw-   0        0        0       67 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/cloudpss/model/implements/__init__.py
+-rw-rw-rw-   0        0        0      734 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/cloudpss/model/implements/component.py
+-rw-rw-rw-   0        0        0     4582 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/model/implements/diagram.py
+-rw-rw-rw-   0        0        0      954 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/cloudpss/model/implements/implement.py
+-rw-rw-rw-   0        0        0     3749 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/model/jobDefinitions.py
+-rw-rw-rw-   0        0        0    25540 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/model/model.py
+-rw-rw-rw-   0        0        0     3966 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/model/revision.py
+-rw-rw-rw-   0        0        0     2313 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/model/topology.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/project/
+-rw-rw-rw-   0        0        0       51 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/cloudpss/project/__init__.py
+-rw-rw-rw-   0        0        0    17698 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/project/project.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/runner/
+-rw-rw-rw-   0        0        0     3422 2024-04-02 03:50:52.000000 cloudpss-4.1.1b9/cloudpss/runner/DSLabResult.py
+-rw-rw-rw-   0        0        0     5841 2023-07-10 05:15:47.000000 cloudpss-4.1.1b9/cloudpss/runner/IESLabEvaluationResult.py
+-rw-rw-rw-   0        0        0     6862 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/runner/IESLabPlanResult.py
+-rw-rw-rw-   0        0        0     8001 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/runner/IESLabTypicalDayResult.py
+-rw-rw-rw-   0        0        0     5953 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/runner/MessageStreamReceiver.py
+-rw-rw-rw-   0        0        0      341 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/runner/__init__.py
+-rw-rw-rw-   0        0        0     4162 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/runner/receiver.py
+-rw-rw-rw-   0        0        0    13125 2024-04-02 02:00:51.000000 cloudpss-4.1.1b9/cloudpss/runner/result.py
+-rw-rw-rw-   0        0        0     7820 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/runner/runner.py
+-rw-rw-rw-   0        0        0     4162 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/cloudpss/runner/storage.py
+-rw-rw-rw-   0        0        0    11613 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/cloudpss/runner/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss/utils/
+-rw-rw-rw-   0        0        0     5314 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/utils/IO.py
+-rw-rw-rw-   0        0        0      326 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/utils/__init__.py
+-rw-rw-rw-   0        0        0      885 2024-04-02 03:50:05.000000 cloudpss-4.1.1b9/cloudpss/utils/dataEncoder.py
+-rw-rw-rw-   0        0        0      255 2024-04-02 03:50:08.000000 cloudpss-4.1.1b9/cloudpss/utils/graphqlUtil.py
+-rw-rw-rw-   0        0        0     1750 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/utils/httprequests.py
+-rw-rw-rw-   0        0        0      795 2023-01-12 12:36:01.000000 cloudpss-4.1.1b9/cloudpss/utils/matlab.py
+-rw-rw-rw-   0        0        0     2677 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/utils/yamlLoader.py
+-rw-rw-rw-   0        0        0     1498 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/cloudpss/verify.py
+-rw-rw-rw-   0        0        0       29 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/cloudpss/version.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/cloudpss.egg-info/
+-rw-rw-rw-   0        0        0     2103 2024-04-02 10:11:24.000000 cloudpss-4.1.1b9/cloudpss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2832 2024-04-02 10:11:24.000000 cloudpss-4.1.1b9/cloudpss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 10:11:24.000000 cloudpss-4.1.1b9/cloudpss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2024-04-02 10:11:24.000000 cloudpss-4.1.1b9/cloudpss.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 10:11:24.000000 cloudpss-4.1.1b9/cloudpss.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/setup.cfg
+-rw-rw-rw-   0        0        0      880 2024-04-02 03:51:28.000000 cloudpss-4.1.1b9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:11:25.000000 cloudpss-4.1.1b9/test/
+-rw-rw-rw-   0        0        0      523 2023-12-27 12:07:35.000000 cloudpss-4.1.1b9/test/test-async.py
+-rw-rw-rw-   0        0        0     1719 2023-12-27 12:10:15.000000 cloudpss-4.1.1b9/test/test-async2.py
+-rw-rw-rw-   0        0        0      846 2023-12-28 08:14:48.000000 cloudpss-4.1.1b9/test/test-async3.py
+-rw-rw-rw-   0        0        0      519 2024-03-07 08:20:22.000000 cloudpss-4.1.1b9/test/test-plot.py
+-rw-rw-rw-   0        0        0     1097 2023-05-30 02:30:39.000000 cloudpss-4.1.1b9/test/test-sdk.py
+-rw-rw-rw-   0        0        0     1359 2023-12-14 10:07:50.000000 cloudpss-4.1.1b9/test/test-sdk1.py
+-rw-rw-rw-   0        0        0     3091 2023-05-30 02:30:39.000000 cloudpss-4.1.1b9/test/test-snapshot.py
+-rw-rw-rw-   0        0        0     1247 2024-01-17 08:11:57.000000 cloudpss-4.1.1b9/test/test-topology.py
+-rw-rw-rw-   0        0        0     1238 2024-04-02 06:24:12.000000 cloudpss-4.1.1b9/test/test.py
+-rw-rw-rw-   0        0        0     1142 2023-09-27 07:50:35.000000 cloudpss-4.1.1b9/test/test7950.py
+-rw-rw-rw-   0        0        0      854 2023-09-20 03:47:30.000000 cloudpss-4.1.1b9/test/testAsync.py
+-rw-rw-rw-   0        0        0     1569 2023-09-25 06:50:28.000000 cloudpss-4.1.1b9/test/testEvent.py
+-rw-rw-rw-   0        0        0     6556 2024-02-05 08:35:40.000000 cloudpss-4.1.1b9/test/testRt.py
+-rw-rw-rw-   0        0        0     5127 2024-02-02 10:25:09.000000 cloudpss-4.1.1b9/test/testRt2.py
+-rw-rw-rw-   0        0        0     2030 2024-01-24 08:48:01.000000 cloudpss-4.1.1b9/test/testSend.py
+-rw-rw-rw-   0        0        0     5350 2023-07-31 07:18:47.000000 cloudpss-4.1.1b9/test/test_in_new_web_1.py
+-rw-rw-rw-   0        0        0     2045 2024-01-18 02:22:57.000000 cloudpss-4.1.1b9/test/test_ws.py
+-rw-rw-rw-   0        0        0     3542 2024-01-18 04:05:57.000000 cloudpss-4.1.1b9/test/test_ws2.py
+-rw-rw-rw-   0        0        0      302 2023-09-21 09:28:41.000000 cloudpss-4.1.1b9/test/testb.py
```

### Comparing `cloudpss-4.1.1b8/PKG-INFO` & `cloudpss-4.1.1b9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpss
-Version: 4.1.1b8
+Version: 4.1.1b9
 Summary: cloudpss sdk
 Home-page: https://www.cloudpss.net
 Author: cloudpss
 Author-email: zhangdaming@cloudpss.net
 License: MIT Licence
 Keywords: cloudpss,cloudpss-sdk
 Platform: any
```

### Comparing `cloudpss-4.1.1b8/README.md` & `cloudpss-4.1.1b9/README.md`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/__init__.py` & `cloudpss-4.1.1b9/cloudpss/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/dslab/dataManageModel.py` & `cloudpss-4.1.1b9/cloudpss/dslab/dataManageModel.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/dslab/dslab.py` & `cloudpss-4.1.1b9/cloudpss/ieslab/IESLabPlan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,210 +1,210 @@
 import json
+
+from cloudpss.ieslab.DataManageModel import IESPlanDataManageModel
+from cloudpss.ieslab.EvaluationModel import IESLabEvaluationModel
+from cloudpss.ieslab.PlanModel import IESLabPlanModel
+from cloudpss.runner.IESLabTypicalDayResult import IESLabTypicalDayResult
 from ..utils import request
 from ..model.model import Model
-from .dataManageModel import DSLabDataManageModel
-from .financialAnalysisModel import DSLabFinancialAnalysisModel
-from cloudpss.runner.DSLabResult import DSLabResult
-from cloudpss.runner.runner import Runner
-from cloudpss.runner.result import IESResult, EMTResult
+from cloudpss.runner.runner import  Runner
+from cloudpss.runner.IESLabPlanResult import IESLabPlanResult
+from cloudpss.runner.IESLabEvaluationResult import IESLabEvaluationResult
 
-class DSLab(object):
+class IESLabPlan(object):
     def __init__(self, project={}):
         '''
             初始化
         '''
         self.id = project.get('id', None)
-        self.resource = project.get('resource', None)
         self.name = project.get('name', None)
         self.__modelRid = project.get('model', None)
+        self.project_group = project.get('project_group', None)
         if self.__modelRid is not None:
             self.model = Model.fetch(self.__modelRid)
-        self.dataManageModel = DSLabDataManageModel(self.resource)
-        self.financialAnalysisModel = DSLabFinancialAnalysisModel(self.resource)
-        self.currentEvaluationResult = DSLabResult(self.resource)
+        self.dataManageModel = IESPlanDataManageModel(self.id)
+        self.planModel = IESLabPlanModel(self.id)
+        self.evaluationModel = IESLabEvaluationModel(self.id)
+        self.currentPlanResult = IESLabPlanResult(self.id)
+        self.currentEvaluationResult = IESLabEvaluationResult(self.id)
 
     @staticmethod
     def fetch(simulationId):
         '''
             获取算例信息
 
             :params: simulationId string类型，代表数据项的算例id
 
-            :return: DSLab
+            :return: IESLabPlan
         '''
         try:
-            r = request(
-                'GET', 'api/dslab/rest/simulation/{0}'.format(simulationId))
+            r = request('GET',
+                        'api/ieslab-plan/rest/simu/{0}/'.format(simulationId))
             project = json.loads(r.text)
-            return DSLab(project)
-        except Exception as e:
-            if 'Unauthorized' in str(e): 
-                raise Exception('token 无效')
-            else:
-                raise Exception('未查询到当前算例')
+            return IESLabPlan(project)
+        except:
+            raise Exception('未查询到当前算例')
 
-    def run(self, job=None, name=None):
+    def __run(self, job=None, name=None):
         '''
             调用仿真 
 
             :params job:  调用仿真时使用的计算方案，不指定将使用算例保存时选中的计算方案
             :params name:  任务名称，为空时使用项目的参数方案名称和计算方案名称
 
             :return: 返回一个运行实例
         '''
         if job is None:
             currentJob = self.model.context['currentJob']
             job = self.model.jobs[currentJob]
-
-        job['args']['simulationId'] = self.resource
+        job['args']['simulationId'] = self.id
         return self.model.run(job, name=name)
-    
-    def dsLabRun(self):
-        '''
-            生成方案优选算例
-
-            :return: 方案优选运行实例
-        '''
-    pass
-
-    def dsLabFinancialRun(self, planID):
-        '''
-            运行技术经济分析
-            :param planID int 类型，表示优化方案的ID，数值位于0~优化方案数量之间
-
-            :return: 技术经济分析实例
 
+    def iesLabTypicalDayRun(self, job=None, name=None, **kwargs)->Runner[IESLabTypicalDayResult]:
         '''
-        return self.financialAnalysisModel.run(planID)
-    
+            运行典型日计算 
 
-    def runIESLoadPrediction(self,job=None,name=None, **kwargs)->Runner[IESResult]:
-        '''
-            运行 负荷预测方案 内核，如果当前 model 没有创建  Job 时报错，默认使用第一个计算方案，进行仿真。
-            
-            :param: job 计算方案名称，可选，字符串类型或者字典类型,默认使用第一个计算方案，如果同名使用最靠前一个
+            :params job:  调用仿真时使用的计算方案，不指定将使用算例保存时选中的计算方案
             :params name:  任务名称，为空时使用项目的参数方案名称和计算方案名称
 
-            :return: runner Runner[IESResult]
+            :return: Runner[IESLabTypicalDayResult]
         '''
         if job is None:
             currentJob = self.model.context['currentJob']
             job = self.model.jobs[currentJob]
-            if job['rid'] != 'job-definition/ies/ies-load-prediction':
+            if job['rid'] != 'function/CloudPSS/ieslab-gmm':
                 for j in self.model.jobs:
-                    if j['rid'] == 'job-definition/ies/ies-load-prediction':
+                    if j['rid'] == 'job-definition/ies/ies-gmm' or j['rid'] == 'job-definition/cloudpss/ieslab-gmm':
+                        j['rid'] = 'function/CloudPSS/ieslab-gmm'
                         job = j
         if job is None:
-            raise Exception("找不到负荷预测方案内核运行的计算方案")
-        if job['rid'] != 'job-definition/ies/ies-load-prediction':
-            raise Exception("不是负荷预测方案内核运行生成算法的计算方案")
-        return self.run(job=job, name=name)
-    
-    def runIESPowerFlow(self,job=None,name=None, **kwargs)->Runner[IESResult]:
+            raise Exception("找不到默认的综合能源系统规划典型日生成算法的计算方案")
+        if job['rid'] != 'function/CloudPSS/ieslab-gmm':
+            raise Exception("不是综合能源系统规划典型日生成算法的计算方案")
+        return self.__run(job=job, name=name)
+
+    def iesLabEvaluationRun(self, planId, type=None):
         '''
-            运行 时序潮流方案 内核，如果当前 model 没有创建  Job 时报错，默认使用第一个计算方案，进行仿真。
-            
-            :param: job 计算方案名称，可选，字符串类型或者字典类型,默认使用第一个计算方案，如果同名使用最靠前一个
-            :params name:  任务名称，为空时使用项目的参数方案名称和计算方案名称
+            运行方案评估
+
+            :param planID int类型，表示优化方案的ID，数值位于0~优化方案数量之间
+            :param type string类型，表示评估类型，可选值为：能效评价、环保评价
+
+            :return: 方案评估运行实例
 
-            :return: runner Runner[IESResult]
         '''
-        if job is None:
-            currentJob = self.model.context['currentJob']
-            job = self.model.jobs[currentJob]
-            if job['rid'] != 'job-definition/ies/ies-power-flow':
-                for j in self.model.jobs:
-                    if j['rid'] == 'job-definition/ies/ies-power-flow':
-                        job = j
-        if job is None:
-            raise Exception("找不到时序潮流方案内核运行的计算方案")
-        if job['rid'] != 'job-definition/ies/ies-power-flow':
-            raise Exception("不是时序潮流方案内核运行生成算法的计算方案")
-        return self.run(job=job, name=name)
-
-    def runIESEnergyStoragePlan(self,job=None,name=None, **kwargs)->Runner[IESResult]:
-        '''
-            运行 储能规划方案 内核，如果当前 model 没有创建  Job 时报错，默认使用第一个计算方案，进行仿真。
-            
-            :param: job 计算方案名称，可选，字符串类型或者字典类型,默认使用第一个计算方案，如果同名使用最靠前一个
-            :params name:  任务名称，为空时使用项目的参数方案名称和计算方案名称
+        return self.evaluationModel.run(planId, type)
 
-            :return: runner Runner[IESResult]
+    def iesLabEnergyEvaluationRun(self, planId):
         '''
-        if job is None:
-            currentJob = self.model.context['currentJob']
-            job = self.model.jobs[currentJob]
-            if job['rid'] != 'job-definition/ies/ies-energy-storage-plan':
-                for j in self.model.jobs:
-                    if j['rid'] == 'job-definition/ies/ies-energy-storage-plan':
-                        job = j
-        if job is None:
-            raise Exception("找不到储能规划方案内核运行的计算方案")
-        if job['rid'] != 'job-definition/ies/ies-energy-storage-plan':
-            raise Exception("不是储能规划方案内核运行生成算法的计算方案")
-        return self.run(job=job, name=name)
+            运行能效评价
+
+            :param planID int类型，表示优化方案的ID，数值位于0~优化方案数量之间
+
+            :return: 能效评价运行实例
+
+        '''
+        return self.evaluationModel.EnergyEvaluationRun(planId)
+
+    def iesLabEnvironmentalEvaluationRun(self, planId):
+        '''
+            运行环保评价
+
+            :param planID int类型，表示优化方案的ID，数值位于0~优化方案数量之间
+
+            :return: 环保评价运行实例
+        '''
+        return self.evaluationModel.EnvironmentalEvaluationRun(planId)
+
+    def iesLabPlanRun(self):
+        '''
+            生成方案优选算例
+
+            :return: 方案优选运行实例
+        '''
+        return self.planModel.run()
+    
+    def iesLabPlanKill(self):
+        '''
+            停止并删除方案优选算例
+
+            :return: Boolean
+        '''
+        return self.planModel.kill()
 
     @staticmethod
-    def createProjectGroup(name, description=None, createById=None):
+    def createProjectGroup(group_name, desc=None, createById=None):
         '''
             创建项目组
 
-            :params name: String 项目组名称 
-            :params description: String 项目组描述 可选参数
+            :params group_name: String 项目组名称 
+            :params desc: String 项目组描述 可选参数
             :params createById Int 父项目组id  可选参数，如果是从已有项目组导入的项目组，必填此项
 
             :return: Int 返回创建的项目组id
         '''
         try:
             if createById is None: 
                 isImport = 0
             else:
                 isImport = 1
             payload = {
-                'name': name,
-                'description': description,
+                'group_name': group_name,
+                'desc': desc,
                 'isImport': isImport,
                 'createById': createById,
             }
             r = request(
-                'POST', 'api/dslab/rest/group', data=json.dumps(payload))
-            if r.ok:
-                r = request('GET', 'api/dslab/rest/group')
-                groupList = json.loads(r.text)
-                id = groupList[len(groupList) -1].get('id', None)
-                return id
+                'POST', 'api/ieslab-plan/rest/projectgroup/', data=json.dumps(payload))
+            project = json.loads(r.text)
+            return project.get('id', None)
         except Exception as e:
             raise Exception('创建项目组失败')
-        
-    @staticmethod
-    def createProject(name, gid, description=None, initialTerm=None, build=None, operate=None, yearsInOperation=None):
+
+    @staticmethod  
+    def createProject(name, project_group, start_date, end_date, construction_cycle, desc=None, createById=None):
         '''
             创建项目
 
             :params name: String 项目名称 
-            :params gid: Int 父项目组id,
-            :params description: String 项目描述, 可选参数
-            :params initialTerm: String 项目起始年限，可选参数
-            :params build: String 项目建设期（年），可选参数
-            :params operate: String 项目生命周期（年），可选参数
-            :params yearsInOperation: String 已投运年限，可选参数
+            :params project_group: Int 父项目组id
+            :param start_date: Int 项目开始年限，范围在[1500,3000]之间
+            :param end_date: Int 项目结束年限，范围在项目开始时间之后且不超过五十年
+            :param construction_cycle: Int 项目建设周期(年), 必须小于等于 项目结束年限 - 项目开始年限
+            :params desc: String 项目描述, 可选参数
+            :params createById Int 父项目id, 可选参数, 如果是从已有项目导入的项目，必填此项
 
             :return: Int 返回创建的项目id
         '''
         try:
-            payload = {
-                'name': name,
-                'gid': gid,
-                'description': description,
-                'config': {
-                    'initialTerm': initialTerm,
-                    'build': build,
-                    'operate': operate,
-                    'yearsInOperation': yearsInOperation,
+            if start_date < 1500 or start_date > 3000:
+                raise Exception('项目开始年限错误，范围在[1500,3000]之间')
+            if end_date < start_date or end_date > start_date + 50:
+                raise Exception('项目结束年限错误，范围在项目开始时间之后且不超过五十年')
+            if construction_cycle > end_date - start_date:
+                raise Exception('项目建设周期错误，必须小于等于 项目结束年限 - 项目开始年限')
+            if createById is None: 
+                payload = {
+                    'name': name,
+                    'project_group': project_group,
+                    'start_date': start_date,
+                    'end_date': end_date,
+                    'construction_cycle': construction_cycle,
+                    'desc': desc
+                }
+            else:
+                payload = {
+                    'name': name,
+                    'project_group': project_group,
+                    'start_date': start_date,
+                    'end_date': end_date,
+                    'construction_cycle': construction_cycle,
+                    'desc': desc,
+                    'createById': createById
                 }
-            }
             r = request(
-                'POST', 'api/dslab/rest/simulation', data=json.dumps(payload))
+                'POST', 'api/ieslab-plan/rest/simu/', data=json.dumps(payload))
             project = json.loads(r.text)
-            return project.get('resource', None)
+            return project.get('id', None)
         except Exception as e:
             raise Exception('创建项目失败')
+
```

### Comparing `cloudpss-4.1.1b8/cloudpss/dslab/files/curveData.py` & `cloudpss-4.1.1b9/cloudpss/dslab/files/curveData.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/dslab/files/files.py` & `cloudpss-4.1.1b9/cloudpss/dslab/files/files.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/dslab/financialAnalysisModel.py` & `cloudpss-4.1.1b9/cloudpss/dslab/financialAnalysisModel.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/function/__init__.py` & `cloudpss-4.1.1b9/cloudpss/function/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/function/functionExecution.py` & `cloudpss-4.1.1b9/cloudpss/function/functionExecution.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,8 +392,18 @@
                 'title': title,
                 'traces':
                 [self.__plotlyDataToTrace(trace) for trace in traces],
                 'xAxis': layout.get('xaxis', {}),
                 'yAxis': layout.get('yaxis', {}),
             }
         }
+        self.print(result)
+        
+    def custom(self, data, key=None,verb='replace'):
+        result = {
+            'key': key,
+            'version': 1,
+            'verb': verb,
+            'type': 'custom',
+            'data': data
+        }
         self.print(result)
```

### Comparing `cloudpss-4.1.1b8/cloudpss/function/job.py` & `cloudpss-4.1.1b9/cloudpss/function/job.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/ieslab/DataManageModel.py` & `cloudpss-4.1.1b9/cloudpss/ieslab/DataManageModel.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,34 +79,58 @@
     
     def _getAllData(self):
         '''
             私有方法，获取数据管理模块全部数据，函数初始化时调用
             
             :return: 无
         '''
-        list = ['thermalLoads', 'electricLoads', 'fuels', 'typhoon', 'rainfall', 'earthquake', 'extremeCold']
-        for kind,value in self._kindUrlMap.items():
-            try:
+        try:
+            r = request('GET',
+                    self._dataManageUrl,
+                    params={
+                        "simulationId": self.simulationId
+                        ,
+                    })
+            data = json.loads(r.text)
+            info = data['info']
+            for kind,value in info.items():
+                if kind =='Weather':
+                    continue
+                
+                for k,data in value.items():
+                    self._kindItemDataMap[k]=value
+                    for val in data:
+                        self._itemDataMap[str(val['timeid'])]=val
+                        self._itemDataMap[str(val['id'])]=val
+                        self._kindIdMap[str(val['timeid'])]=k
+                        self._kindIdMap[str(val['id'])]=k
+        except Exception as e:
+            print('获取数据失败',e)
+            pass
+
+        # list = ['thermalLoads', 'electricLoads', 'fuels', 'typhoon', 'rainfall', 'earthquake', 'extremeCold']
+        # for kind,value in self._kindUrlMap.items():
+        #     try:
             
-                if kind in list:
-                    dataList = self._fetchItemData(self._kindUrlMap[kind], None)
-                else:
-                    dataList = self._fetchItemData(self._kindUrlMap[kind], kind)
-            except Exception as e:
-                pass
-            self._kindItemDataMap[kind]=dataList
-            for val in dataList:
-                self._itemDataMap[str(val['timeid'])]=val
-                self._itemDataMap[str(val['id'])]=val
-                self._kindIdMap[str(val['timeid'])]=kind
-                self._kindIdMap[str(val['id'])]=kind
+        #         if kind in list:
+        #             dataList = self._fetchItemData(self._kindUrlMap[kind], None)
+        #         else:
+        #             dataList = self._fetchItemData(self._kindUrlMap[kind], kind)
+        #     except Exception as e:
+        #         pass
+        #     self._kindItemDataMap[kind]=dataList
+        #     for val in dataList:
+        #         self._itemDataMap[str(val['timeid'])]=val
+        #         self._itemDataMap[str(val['id'])]=val
+        #         self._kindIdMap[str(val['timeid'])]=kind
+        #         self._kindIdMap[str(val['id'])]=kind
 
     def GetDataItem(self, ID: str):
         '''
-            获取ID对应的元素信息
+            获取ID对应的数据信息
             
             :params: ID string类型，代表数据项的标识符，可以在所有类型的数据项中实现唯一标识
             
             :return: dict类型，为源数据的引用，返回该数据项的信息
         '''
         data = self._itemDataMap.get(str(ID),None)
         
@@ -277,19 +301,43 @@
                         params={
                             "time_after": startDate,
                             "time_before": endDate,
                             "sid": self.simulationId,
                         })
             weatherData = json.loads(r.text)
             return weatherData['results']
+        
+    def UpdateAtmosData(self, data):
+        '''
+            更新气象数据
+            :data:  list类型，表示数据内容，其数据结构应满足对应数据项的满足如下结构要求：
+                        "lat": string类型 坐标纬度
+                        "lng": string类型 坐标经度
+                        "time": string类型 表示时间 需满足格式YYYY-MM-DD hh:mm:ss 如"2016-01-01 00:00:00"
+                        "t10m": string类型 表示环境温度（℃）
+                        "lwgab_swgdn": string类型 表示太阳辐射强度（W/m2）
+                        "u10m": string类型 距地面10m处东向风速（m/s）
+                        "u50m": string类型 距地面50m处东向风速（m/s）
+                        "v10m": string类型 距地面10m处北向风速（m/s）
+                        "v50m": string类型 距地面50m处北向风速（m/s）
+                        "adj_sfc_sw_direct_all_1h": string类型 短波直射强度（W/m²）
+                        "adj_sfc_sw_diff_all_1h": string类型 短波散射强度（W/m²）
+                        "solar_zen_angle_1h": string类型 太阳天顶角°
+            :return: bool 类型，返回True 更新成功
+        '''
+        r = request('POST',
+                    self._weatherUrl,
+                    data=json.dumps({"sid":self.simulationId, "data":data}))
+        return r.ok
 
 
 class IESSimulationDataManageModel(DataManageModel):
     _baseUri = 'api/ieslab-simulation/'
     _weatherUrl = 'api/ieslab-simulation/rest/weather_data/'
+    _dataManageUrl = 'api/ieslab-simulation/editor/data_manage/'
     _kindNameMap = {
         "光伏": "PhotovoltaicSys",
         "风机": "WindPowerGenerator",
         "燃气轮机": "GasTurbine",
         "热泵": "HeatPump",
         "燃气锅炉": "GasBoiler",
         "热管式太阳能集热器": "HPSolarCollector",
@@ -348,14 +396,15 @@
     }
     pass
 
 
 class IESPlanDataManageModel(DataManageModel):
     _baseUri = 'api/ieslab-plan/'
     _weatherUrl = 'api/ieslab-plan/rest/weather_data/'
+    _dataManageUrl = 'api/ieslab-plan/editor/data_manage/'
     _kindNameMap = {
         "光伏": "PhotovoltaicSys",
         "风机": "WindPowerGenerator",
         "燃气轮机": "GasTurbine",
         "热泵": "HeatPump",
         "燃气锅炉": "GasBoiler",
         "热管式太阳能集热器": "HPSolarCollector",
```

### Comparing `cloudpss-4.1.1b8/cloudpss/ieslab/EvaluationModel.py` & `cloudpss-4.1.1b9/cloudpss/ieslab/EvaluationModel.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/ieslab/IESLabSimulation.py` & `cloudpss-4.1.1b9/cloudpss/ieslab/IESLabSimulation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from ..utils import request
 from ..model.model import Model
 from .DataManageModel import IESSimulationDataManageModel
 
 
 class IESLabSimulation(object):
-    def __init__(self, project={},model=None):
+    def __init__(self, project={},model:Model=None):
         '''
             初始化
         '''
         self.id = project.get('id', None)
         self.name = project.get('name', None)
         self.__modelRid = project.get('model', None)
         self.project_group = project.get('project_group', None)
@@ -32,34 +32,15 @@
             modelRid = project.get('model', None)
             model=None
             if modelRid is not None:
                 model = Model.fetch(modelRid)
             return IESLabSimulation(project,model)
         except:
             raise Exception('未查询到当前算例')
-    @staticmethod
-    async def fetchAsync(simulationId):
-        '''
-            获取算例信息
-
-            :params: simulationId string类型，代表数据项的算例id
-
-            :return: IESLabSimulation
-        '''
-        try:
-            r = request(
-                'GET', 'api/ieslab-simulation/rest/simu/{0}/'.format(simulationId))
-            project = json.loads(r.text)
-            modelRid = project.get('model', None)
-            model=None
-            if modelRid is not None:
-                model =await Model.fetchAsync(modelRid)
-            return IESLabSimulation(project,model)
-        except:
-            raise Exception('未查询到当前算例')
+   
     def run(self, job=None, name=None):
         '''
             调用仿真 
 
             :params job:  调用仿真时使用的计算方案，不指定将使用算例保存时选中的计算方案
             :params name:  任务名称，为空时使用项目的参数方案名称和计算方案名称
 
@@ -67,23 +48,69 @@
         '''
         if job is None:
             currentJob = self.model.context['currentJob']
             job = self.model.jobs[currentJob]
 
         job['args']['simulationId'] = self.id
         return self.model.run(job, name=name)
-
-    async def runAsync(self, job=None, name=None):
+    
+    @staticmethod
+    def createProjectGroup(group_name, desc=None, createById=None):
         '''
-            调用仿真 
+            创建项目组
 
-            :params job:  调用仿真时使用的计算方案，不指定将使用算例保存时选中的计算方案
-            :params name:  任务名称，为空时使用项目的参数方案名称和计算方案名称
+            :params group_name: String 项目组名称 
+            :params desc: String 项目组描述 可选参数
+            :params createById Int 父项目组id  可选参数，如果是从已有项目组导入的项目组，必填此项
 
-            :return: 返回一个运行实例
+            :return: Int 返回创建的项目组id
         '''
-        if job is None:
-            currentJob = self.model.context['currentJob']
-            job = self.model.jobs[currentJob]
+        try:
+            if createById is None: 
+                isImport = 0
+            else:
+                isImport = 1
+            payload = {
+                'group_name': group_name,
+                'desc': desc,
+                'isImport': isImport,
+                'createById': createById,
+            }
+            r = request(
+                'POST', 'api/ieslab-simulation/rest/projectgroup/', data=json.dumps(payload))
+            project = json.loads(r.text)
+            return project.get('id', None)
+        except Exception as e:
+            raise Exception('创建项目组失败')
 
-        job['args']['simulationId'] = self.id
-        return await self.model.runAsync(job, name=name)
+    @staticmethod 
+    def createProject(name, project_group, desc=None, createById=None):
+        '''
+            创建项目
+
+            :params name: String 项目名称 
+            :params project_group: Int 父项目组id,
+            :params desc: String 项目描述, 可选参数
+            :params createById Int 父项目id, 可选参数, 如果是从已有项目导入的项目，必填此项
+
+            :return: Int 返回创建的项目id
+        '''
+        try:
+            if createById is None: 
+                payload = {
+                    'name': name,
+                    'project_group': project_group,
+                    'desc': desc
+                }
+            else:
+                payload = {
+                    'name': name,
+                    'project_group': project_group,
+                    'desc': desc,
+                    'createById': createById
+                }
+            r = request(
+                'POST', 'api/ieslab-simulation/rest/simu/', data=json.dumps(payload))
+            project = json.loads(r.text)
+            return project.get('id', None)
+        except Exception as e:
+            raise Exception('创建项目失败')
```

### Comparing `cloudpss-4.1.1b8/cloudpss/ieslab/PlanModel.py` & `cloudpss-4.1.1b9/cloudpss/ieslab/PlanModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             for e in OptimizationMode:
                 if (e.value == data['data']['optimizationpara']
                     ['OptimizationMode']):
                     return e
         except:
             return OptimizationMode['经济性']
 
-    def SetOptimizationInfo(self, optType):
+    def SetOptimizationInfo(self,   optType):
         '''
             无对应接口
             设置当前算例的优化目标
 
             :param optType: enum 类型，代表经济性优化和环保性优化的类型
         '''
         self.optimizationInfo = optType
@@ -124,20 +124,24 @@
         error = res.get('error', 0)
         if error == 0:
             data = res.get('data', {})
             if data is not None:
                 status = data.get('status', '')
                 if status == 'stop':
                     isRunning = False
-        logs = IESLabPlanResult(self.simulationId).GetLogs()
-        if logs is not None:
-            for log in logs:
-                if(log.get('data', '') == 'run ends'):
-                    isRunning = False
-                    break
+        try:
+            
+            logs = IESLabPlanResult(self.simulationId).GetLogs()
+            if logs is not None:
+                for log in logs:
+                    if(log.get('data', '') == 'run ends'):
+                        isRunning = False
+                        break
+        except:
+            return False
         return isRunning
 
 
 # @unique
 class OptimizationMode(IntEnum):
     经济性 = 0
     环保性 = 1
```

### Comparing `cloudpss-4.1.1b8/cloudpss/job/job.py` & `cloudpss-4.1.1b9/cloudpss/job/job.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,58 @@
 import asyncio
 import random
 import re
 import time
-from cloudpss.utils.AsyncIterable import CustomAsyncIterable
 
-from cloudpss.utils.httpAsyncRequest import graphql_fetch
+from cloudpss.job.view.view import View
 from .view import getViewClass
 
 from cloudpss.utils.IO import IO
 from .messageStreamReceiver import MessageStreamReceiver
 
 from cloudpss.utils.graphqlUtil import graphql_request
-from .jobPolicy import JobPolicy
-from .jobMachine import JobMachine
 from .messageStreamSender import MessageStreamSender
-from typing import Any, Callable, TypeVar
+from typing import Any, Callable, Generic, TypeVar
 F = TypeVar('F', bound=Callable[..., Any])
-class Job(object):
+T = TypeVar('T', bound=Callable[..., View])
+class Job(Generic[T]):
     """docstring for Job"""
-
+    __jobQuery = """query($_a:JobInput!){
+            job(input:$_a){
+                id
+                args
+                createTime
+                startTime
+                endTime
+                status
+                context
+                user
+                priority
+                policy  { 
+                    name
+                    queue
+                    tres {
+                        cpu
+                        ecpu
+                        mem
+                    } 
+                    priority 
+                    maxDuration 
+                }
+                machine {
+                    id
+                    name
+                }
+                input
+                output
+                position
+            }
+        }"""
+    
+    __createJobQuery = """mutation($input:CreateJobInput!){job:createJob(input:$input){id input output status position}}"""
     def __init__(
         self,
         id,
         args,
         createTime,
         startTime,
         endTime,
@@ -43,100 +73,50 @@
         self.startTime = startTime
         self.endTime = endTime
         self.job_status = status #这里的status字段与原本的status()冲突
         self.context = context
         self.user = user
         self.priority = priority
         self.policy = policy  # type: ignore
-        self.machine = JobMachine(**machine)  # type: ignore
+        self.machine = machine # type: ignore
         self.input = input
         self.output = output
         self.position = position
         self.__receiver = None
         self.__sender = None
         self._result = None
 
     @staticmethod
     def fetch(id):
-        return  asyncio.run(Job.fetchAsync(id))
-    @staticmethod
-    async def fetchAsync(id):
         """
         获取job信息
         """
         if id is None:
             raise Exception("id is None")
-        query = """query($_a:JobInput!){
-            job(input:$_a){
-                id
-                args
-                createTime
-                startTime
-                endTime
-                status
-                context
-                user
-                priority
-                policy  { 
-                    name
-                    queue
-                    tres {
-                        cpu
-                        ecpu
-                        mem
-                    } 
-                    priority 
-                    maxDuration 
-                }
-                machine {
-                    id
-                    name
-                    tres {
-                        cpu
-                        ecpu
-                        mem
-                    }
-                }
-                input
-                output
-                position
-            }
-        }"""
+       
         variables = {"_a": {"id": id}}
 
-        r = await graphql_fetch(query, variables)
+        r =  graphql_request(Job.__jobQuery, variables)
         if "errors" in r:
             raise Exception(r["errors"])
         return Job(**r["data"]["job"])
-
-    @staticmethod
-    def fetchMany(*args):
-        """
-        批量获取任务信息
-        """
-        jobs = CustomAsyncIterable(Job.fetchAsync,*args)
-        return jobs
+        
+    
+    # @staticmethod
+    # def fetchMany(*args):
+    #     """
+    #     批量获取任务信息
+    #     """
+    #     # jobs = CustomAsyncIterable(Job.fetch,*args)
+    #     # return jobs 
     
 
+    
     @staticmethod
-    async def create(revisionHash, job, config, name=None, rid="", policy=None, **kwargs):
-        """
-        创建一个运行任务
-
-        :params: revision 项目版本号
-        :params: job 调用仿真时使用的计算方案，为空时使用项目的第一个计算方案
-        :params: config 调用仿真时使用的参数方案，为空时使用项目的第一个参数方案
-        :params: name 任务名称，为空时使用项目的参数方案名称和计算方案名称
-        :params: rid 项目rid，可为空
-
-        :return: 返回一个运行实例
-
-        >>> runner = Runner.runRevision(revision,job,config,'')
-        """
-
+    def __createJobVariables(job, config, revisionHash, rid, policy, **kwargs):
         # 处理policy字段
         if policy is None:
             policy = {}
             if policy.get("tres", None) is None:
                 policy["tres"] = {}
             policy["queue"] = job["args"].get("@queue", 1)
             policy["priority"] = job["args"].get("@priority", 0)
@@ -144,145 +124,152 @@
             tresStr = job["args"].get("@tres", "")
             for t in re.split("\s+", tresStr):
                 if t == "":
                     continue
                 k, v = t.split("=")
                 tres[k] = float(v)  # type: ignore
             policy["tres"] = tres
-
-        query = """mutation($input:CreateJobInput!){job:createJob(input:$input){id input output status position}}"""
         function = job["rid"].replace("job-definition/cloudpss/", "function/CloudPSS/")
+        implement = kwargs.get("implement", None)
+        debug = job["args"].get("@debug", None )
+        debugargs={}
+        if debug is not None:
+            t= [ i.split('=') for i in re.split(r'\s+',debug) if i.find('=')>0]
+            for i in t:
+                debugargs[i[0]]=i[1]
         variables = {
             "input": {
                 "args": {
                     **job["args"],
                     "_ModelRevision": revisionHash,
                     "_ModelArgs": config["args"],
+                    "implement":implement
                 },
                 "context": [
                     function,
                     rid,
                     f"model/@sdk/{str(int(time.time() * random.random()))}",
                 ],
                 "policy": policy,
+                "debug":debugargs
             }
         }
-        r = await graphql_fetch(query, variables)
-        if "errors" in r:
-            raise Exception(r["errors"])
-        id = r["data"]["job"]["id"]
-        return await Job.fetchAsync(id)
-
+        return variables
     @staticmethod
-    async def abort(id, timeout):
+    def create(revisionHash, job, config, name=None, rid="", policy=None, **kwargs):
         """
-        结束当前运行的算例
+        创建一个运行任务
 
+        :params: revision 项目版本号
+        :params: job 调用仿真时使用的计算方案，为空时使用项目的第一个计算方案
+        :params: config 调用仿真时使用的参数方案，为空时使用项目的第一个参数方案
+        :params: name 任务名称，为空时使用项目的参数方案名称和计算方案名称
+        :params: rid 项目rid，可为空
+
+        :return: 返回一个运行实例
+
+        >>> runner = Runner.runRevision(revision,job,config,'')
         """
-        query = """mutation ($input: AbortJobInput!) {
-            job: abortJob(input: $input) {
-                id
-                status
-            }
-        }
-        """
-        variables = {"input": {"id": id, "timeout": timeout}}
-        await graphql_fetch(query, variables)
+        variables=Job.__createJobVariables(job, config, revisionHash, rid, policy)
+        r =  graphql_request(Job.__createJobQuery, variables)
+        if "errors" in r:
+            raise Exception(r["errors"])
+        id = r["data"]["job"]["id"]
+        return  Job.fetch(id)
+        
+    
 
     @staticmethod
     def load(file, format="yaml"):
         return IO.load(file, format)
 
     @staticmethod
     def dump(job, file, format="yaml", compress="gzip"):
         return IO.dump(job, file, format, compress)
 
-    async def read(self, receiver=None, dev=False, **kwargs):
-        """
-        使用接收器获取当前运行实例的输出
-        """
-        if receiver is not None:
-            self.__receiver = receiver
-        if self.__receiver is None:
-            self.__receiver = MessageStreamReceiver(self, dev)
-        await self.__receiver.connect(**kwargs)
-        return self.__receiver
+    
 
-    def read_legacy(self, receiver=None, dev=False, **kwargs):
+    def read(self, receiver=None, **kwargs):
         """
         使用接收器获取当前运行实例的输出
         """
         if receiver is not None:
             self.__receiver = receiver
         if self.__receiver is None:
-            self.__receiver = MessageStreamReceiver(self, dev)
-            self.__receiver.connect_legacy(**kwargs)
+            self.__receiver = MessageStreamReceiver(self)
+            self.__receiver.connect(**kwargs)
         return self.__receiver
 
-    async def write(self, sender=None, dev=False, **kwargs) -> MessageStreamSender:
-        """
-        使用发送器为当前运行实例输入
-        """
-
-        if sender is not None:
-            self.__sender = sender
-        if self.__sender is None:
-            self.__sender = MessageStreamSender(self, dev)
-        await self.__sender.connect(**kwargs)
-        return self.__sender
     
-    def write_legacy(self, sender=None, dev=False, **kwargs) -> MessageStreamSender:
+    
+    def write(self, sender=None,  **kwargs) -> MessageStreamSender:
         """
-        使用发送器为当前运行实例输入同步方法
+        使用发送器为当前运行实例输入
         """
 
         if sender is not None:
             self.__sender = sender
         if self.__sender is None:
-            self.__sender = MessageStreamSender(self, dev)
+            self.__sender = MessageStreamSender(self)
         self.__sender.connect_legacy(**kwargs)
         return self.__sender
     
     def status(self):
         """
         return: 0: 运行中 1: 运行完成 2: 运行失败
         """
-        
+        time.sleep(0)
         if self.__receiver is not None:
             return self.__receiver.status
         if self.__receiver is None:
-            self.__connect_legacy()
+            self.__connect()
+        
         return 0
     
-    def __connect_legacy(self):
+    def __connect(self):
         """
         连接接收器和发送器
         """
         viewType = getViewClass(self.context[0])
-        self._result = self.view_legacy(viewType)
+        self._result = self.view(viewType)
         
     @property
-    def result(self):
+    def result(self)->T:
         """
         获取当前运行实例的输出
         """
         if self._result is None:
-            self.__connect_legacy()
+            self.__connect()
         return self._result
    
     
-    def view_legacy(self, viewType:F)->F:
+    def view(self, viewType:F=None)->F:
         """
         获取当前运行实例的输出
         """
-        receiver =  self.read_legacy()
-        sender =  self.write_legacy()
+        receiver =  self.read()
+        sender =  self.write()
+        if viewType is None:
+            viewType = getViewClass(self.context[0])
+        
         return viewType(receiver, sender)
 
-    async def view(self, viewType:F)->F:
+    
+
+    def abort(self,timeout=3):
         """
-        获取当前运行实例的输出
+        中断当前运行实例
         """
-        receiver = await self.read()
-        sender = await self.write()
-        self._result= viewType(receiver, sender)
-        return self._result
+        query = '''mutation ($input: AbortJobInput!) {
+            job: abortJob(input: $input) {
+                id
+                status
+            }
+        }
+        '''
+        variables = {
+            'input': {
+                'id': self.taskId,
+                'timeout': timeout
+            }
+        }
+        graphql_request(query, variables)
```

### Comparing `cloudpss-4.1.1b8/cloudpss/job/jobReceiver.py` & `cloudpss-4.1.1b9/cloudpss/job/jobReceiver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from deprecated import deprecated
 class JobReceiver(object):
     messages = []
     index = 0
 
     def __init__(self):
         self.index = 0
         self.messages = []
@@ -26,8 +27,13 @@
 
             :params viewType: 视图类型
 
             :returns: 对应类型的视图数据
 
             >>> view= receiver.view(EMTView)
         """
-        return ViewType(self)
+        return ViewType(self)
+    
+    @property
+    @deprecated(version='3.0', reason="该方法将在 5.0 版本移除")
+    def message(self):
+        return self.messages
```

### Comparing `cloudpss-4.1.1b8/cloudpss/job/messageStreamSender.py` & `cloudpss-4.1.1b9/cloudpss/job/messageStreamSender.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 import asyncio
 import sys, os
 import threading
 from urllib.parse import urlparse
-
-import aiohttp
-
-
 sys.path.append(os.path.join(os.path.dirname(__file__), "../"))
 
 import websocket
 
 from cloudpss.utils.IO import IO
 import time
 import logging
 
 
 class MessageStreamSender:
-    def __init__(self, job, dev=False):
+    def __init__(self, job):
         super().__init__()
         self.job = job
-        self.dev = dev
         self.origin = os.environ.get("CLOUDPSS_API_URL", "https://cloudpss.net/")
         self.__hasOpen = False
 
     def __on_message(self, ws, message):
         logging.debug("on_message", message)
 
     def __on_error(self, ws, error):
@@ -52,27 +47,17 @@
         if self.session is not None:
             asyncio.run(self.session.close())
 
     @property
     def status(self):
         return self._status
 
-    async def write_async(self, message):
-        if self.websocket:
-            data = IO.serialize(message, "ubjson", None)
-            await self.websocket.send_bytes(data)
-        else:
-            logging.info("websocket is None")
-
     def write(self, message):
-        if self.ws:
-            data = IO.serialize(message, "ubjson", None)
-            self.ws.send(data,websocket.ABNF.OPCODE_BINARY)
-        else:
-            asyncio.run(self.write_async(message))
+        data = IO.serialize(message, "ubjson", None)
+        self.ws.send(data,websocket.ABNF.OPCODE_BINARY)
 
     def connect_legacy(self):
         """
         同步方法连接ws
         """
         self._status = 0
         if self.job.input is None:
@@ -95,32 +80,10 @@
         thread = threading.Thread(target=self.ws.run_forever, args=(None, None, 6, 3))
         thread.setDaemon(True)
         thread.start()
         while not self.__hasOpen:
             time.sleep(0.2)
         return self.ws
 
-    async def receive_data(self):
-        if self.websocket:
-            data = await self.websocket.receive()
-            if data.type == aiohttp.WSMsgType.TEXT:
-                self.__on_message(data.data)
-            elif data.type == aiohttp.WSMsgType.CLOSED:
-                self.__on_close()
-            elif data.type == aiohttp.WSMsgType.ERROR:
-                self.__on_error(data.data)
-        else:
-            logging.info("WebSocket connection not established")
+    
 
-    async def connect(self):
-        self._status = 0
-        if self.job.input is None:
-            raise Exception("id is None")
-        if self.job.input == "00000000-0000-0000-0000-000000000000":
-            return
-        u = list(urlparse(self.origin))
-        head = "wss" if u[0] == "https" else "ws"
-
-        path = head + "://" + str(u[1]) + "/api/streams/token/" + self.job.input
-        logging.info(f"MessageStreamSender data from websocket: {path}")
-        async with aiohttp.ClientSession() as session:
-            self.websocket = await session.ws_connect(path)
+
```

### Comparing `cloudpss-4.1.1b8/cloudpss/job/view/EMTView.py` & `cloudpss-4.1.1b9/cloudpss/job/view/EMTView.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 import uuid
-
+from deprecated import deprecated
 from .view import View
 class EMTView(View):
     """
         电磁暂态结果视图， 
 
         提供快捷 plot 数据的接口函数，获取到的 plot 数据为合并后的数据格式，不在是接收时分段的数据
 
@@ -32,15 +32,15 @@
                             v['x'])
                         self.result[key]['data']['traces'][i]['y'].extend(
                             v['y'])
         return self.result.values()
     
     def getPlot(self, index: int):
         '''
-            获取指定序号的数据分组
+            获取指定序号的曲线分组
 
             :params: index 图表位置
 
             >>> result.getPlot(0)
             {...}
         '''
         self.getPlots()
@@ -96,20 +96,21 @@
             前进到指定时步
         """
         if self._sender is not None:
             self._sender.write({'type': 'debug', 'step': step})
         else:
             raise Exception('sender is None')
     
+    
     def writeShm(self,path,buffer,offset):
         """
-            写内存接口
+            写内存接口 （未最终确定，后续版本进行修改，使用时注意版本）
         """
         if self._sender is not None:
-            self._sender.write({'type': 'memory', 'path': path,'value':buffer,'offset':offset})
+            self._sender.write({'type': 'memory', 'path': path,'buffer':buffer,'offset':offset})
         else:
             raise Exception('transmitter is None')
     
     def _writeEvent(self,eventType,eventTime,eventTimeType,defaultApp):
         if self._sender is  None:
             raise Exception('transmitter is None')
         event = {
@@ -132,43 +133,40 @@
             }
         }
         eventData = {}
         eventData = {'SimuCtrl': param}
 
         self._writeEvent('time','-1','1',{'SimuCtrl': eventData})
             
-        
     def _snapshotControl(self,ctrlType,snapshotNumber,log):
         """
             断面控制
         """
         param = {
             "ctrl_type": ctrlType,
             "snapshot_number": snapshotNumber,
             "uuid": str(uuid.uuid1()),
             'message': {
                 'log': log
             },
         }
         eventData = {}
         eventData = {'SnapshotCtrl': param}
-        self._writeEvent('time','-1','1',{'SnapshotCtrl': eventData})
-        
+        self._writeEvent('time','-1','1',{'SnapshotCtrl': eventData})  
     def saveSnapshot(self,snapshotNumber,log='保存断面成功'):
         """
             通过事件链保存断面
         """
         self._snapshotControl('0',snapshotNumber,log)
     def loadSnapshot(self,snapshotNumber,log='加载断面成功'):
         """
             通过事件链加载断面
         """
         self._snapshotControl('1',snapshotNumber,log)
         
-
     def control(self,controlParam,eventTime='-1',eventTimeType='1'):
         """
             控制仿真
         """    
 
         if type(controlParam) is not list:
             controlParam=[controlParam]
@@ -186,18 +184,18 @@
                 }
             }
         self._writeEvent('time',eventTime,eventTimeType,{'para': para})
         pass
     
     def monitor(self,monitorParam,eventTime='-1',eventTimeType='1'):
         
-        if type(controlParam) is not list:
-            controlParam=[controlParam]
+        if type(monitorParam) is not list:
+            monitorParam=[monitorParam]
         para={}
-        for param in controlParam:
+        for param in monitorParam:
             para[param['key']]={
                 'a': {
                     'uuid':param['uuid'] if param.get('uuid',None) is not None else str(uuid.uuid1()),
                     'function':param['function'],
                     'cmd':'add',
                     'period':param['period'],
                     'value':param['value'],
```

### Comparing `cloudpss-4.1.1b8/cloudpss/job/view/IESView.py` & `cloudpss-4.1.1b9/cloudpss/job/view/IESView.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/job/view/PowerFlowView.py` & `cloudpss-4.1.1b9/cloudpss/job/view/PowerFlowView.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/job/view/__init__.py` & `cloudpss-4.1.1b9/cloudpss/job/view/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/model/implements/component.py` & `cloudpss-4.1.1b9/cloudpss/model/implements/component.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/model/implements/diagram.py` & `cloudpss-4.1.1b9/cloudpss/model/implements/implement.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,40 @@
-from .component import Component
+from .diagram import DiagramImplement
 
 
-class DiagramImplement(object):
+class ModelImplement(object):
     """
-        拓扑实现
+        实现类
     """
-
-    def __init__(self, diagram: dict = {}):
+    def __init__(self, implements: dict = {}):
         """
             初始化
         """
-        for k, v in diagram.items():
-            if k == 'cells':
-                self.__dict__[k] = v
-                for key, val in v.items():
-                    v[key] = Component(val)
+        for k, v in implements.items():
+            if k == 'diagram':
+                self.__dict__[k] = DiagramImplement(v)
             else:
                 self.__dict__[k] = v
 
     def __getitem__(self, attr):
-        return super(DiagramImplement, self).__getattribute__(attr)
+        return super(ModelImplement, self).__getattribute__(attr)
 
     def toJSON(self):
         """
             类对象序列化为 dict
             :return: dict
 
-            >>>> diagram.toJSON()
+             >>> implement.toJSON()
         """
-        cells = {}
-        for key, val in self.cells.items():
-            cells[key] = val.toJSON()
-        diagram = {**self.__dict__, 'cells': cells}
-        return diagram
+        implements = {**self.__dict__, 'diagram': self.diagram.toJSON()}
+        return implements
 
-    def getAllComponents(self):
+    def getDiagram(self):
         """
-            获取所有元件
+            获取拓扑实现，不存在返回空
 
-            :return: dict<Component>
+            :return: 示意图实例
 
-            >>>> diagram.getAllComponents()
+            >>> implement.getDiagram()
         """
 
-        return self.cells
+        return getattr(self, 'diagram', None)
```

### Comparing `cloudpss-4.1.1b8/cloudpss/model/jobDefinitions.py` & `cloudpss-4.1.1b9/cloudpss/model/jobDefinitions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 JOB_DEFINITIONS = {
     "emtp": {
-        "rid": "job-definition/cloudpss/emtp",
+        "rid": "function/CloudPSS/emtp",
         "args": {
             "debug":
             "0",
             "n_cpu":
             "1",
             "solver":
             "0",
@@ -44,15 +44,15 @@
             "save_snapshot_time":
             "1"
         },
         "name": "电磁暂态仿真方案 1"
     },
     'sfemt': {
         "name": "移频电磁暂态仿真方案 1",
-        "rid": "job-definition/cloudpss/sfemt",
+        "rid": "function/CloudPSS/sfemt",
         "args": {
             "begin_time":
             "0",
             "end_time":
             "1",
             "step_time":
             "0.0001",
@@ -99,50 +99,50 @@
             "",
             "debug":
             "0"
         }
     },
     "powerFlow": {
         "name": "潮流计算方案 1",
-        "rid": "job-definition/cloudpss/power-flow",
+        "rid": "function/CloudPSS/power-flow",
         "args": {
             "UseBusVoltageAsInit": "1",
             "UseBusAngleAsInit": "1",
             "UseVoltageLimit": "1",
             "UseReactivePowerLimit": "1",
             "SkipPF": "0",
             "MaxIteration": "30"
         }
     },
     "iesLoadPrediction": {
         "name": "负荷预测方案 1",
-        "rid": "job-definition/ies/ies-load-prediction",
+        "rid": "function/CloudPSS/ies-load-prediction",
         "arcs": {
             "startTime": "2022 -01-01 00:00:00",
             "endTime": "2022 -12-31 23:00:00",
             "layer_forcast": "0",
             "forcast_algorithm": "0",
             "ratio_sub": [],
             "ratio_feeder": [],
             "ratio_trans": []
         }
     },
     "iesPowerFlow": {
         "name": "时序潮流方案 1",
-        "rid": "job-definition/ies/ies-power-flow",
+        "rid": "function/CloudPSS/ies-power-flow",
         "arcs": {
             "startTime": "2022 -01-01 00:00:00",
             "endTime": "2022 -12-31 23:00:00",
             "solveMethod": "0",
             "maxIteration": "30"
         }
     },
     "iesEnergyStoragePlan": {
         "name": "储能规划方案 1",
-        "rid": "job-definition/ies/ies-energy-storage-plan",
+        "rid": "function/CloudPSS/ies-energy-storage-plan",
         "arcs": {
             "Planyear": "15",
             "NetConfig": [],
             "SourceConfig": [],
             "LoadConfig": []
         }
     }
```

### Comparing `cloudpss-4.1.1b8/cloudpss/model/model.py` & `cloudpss-4.1.1b9/cloudpss/model/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import asyncio
 import os
 import re
 from copy import deepcopy
-
 from cloudpss.job.job import Job
+from cloudpss.job.view import EMTView, IESView, PowerFlowView
+from cloudpss.job.view.view import View
 from cloudpss.utils.IO import IO
-from cloudpss.utils.httpAsyncRequest import graphql_fetch
-
+from cloudpss.utils import graphql_request
 from .revision import ModelRevision
 from .jobDefinitions import JOB_DEFINITIONS
 from ..verify import userName
 
 from cloudpss.runner.result import IESResult
 from cloudpss.runner.runner import Runner
 
@@ -32,14 +31,42 @@
     configs     当前项目的所有参数方案
 
     jobs        当前项目的所有计算方案
 
     context     当前项目的上下文相关信息
 
     """
+    __models_query="""query($input:ModelsInput!){models(input:$input){cursor total count items{rid name description owner tags updatedAt }}}"""
+    
+    __model_query= """
+            query  t($rid:ResourceId!){
+                model(input:{rid: $rid}) {
+                    configs
+                    context
+                    description
+                    jobs
+                    name
+                    rid
+                    tags
+                    revision {
+                        author
+                        documentation
+                        graphic
+                        hash
+                        implements
+                        message
+                        parameters
+                        pins
+                        version
+                    }
+                }
+            }
+        """
+    __create_model= """mutation($a:CreateModelInput!){createModel(input:$a){rid}}"""
+    __update_model = """mutation($a:UpdateModelInput!){updateModel(input:$a){rid}}"""
 
     context: dict
     jobs: list
     configs: list
 
     def __init__(self, model: dict = {}):
         """
@@ -64,29 +91,69 @@
         """
         类对象序列化为 dict
         :return: dict
         """
         model = {**self.__dict__, "revision": self.revision.toJSON()}
         return model
 
-    def getAllComponents(self):
+    def getAllComponents(self)->dict:
         """
         获取实现
 
         :return: 所有元件信息
 
         >>> model.getAllComponents()
         {
             'canvas_0_2': Component 实例
         }
         """
         diagramImplement = self.revision.getImplements().getDiagram()
         if diagramImplement is None:
             raise ValueError("不存在拓扑实现")
         return diagramImplement.getAllComponents()
+    
+    def addComponent(self, definition, label, args, pins, canvas=None, position=None, size=None):
+        """
+        创建一个
+
+        :return: Component
+
+        >>>> model.addComponent(args)
+        """
+        diagramImplement = self.revision.getImplements().getDiagram()
+        if diagramImplement is None:
+            raise ValueError("不存在拓扑实现")
+        return diagramImplement.addComponent(definition, label, args, pins, canvas, position, size)
+    
+    def removeComponent(self, key):
+        """
+        删除元件实现
+
+        :return: boolean
+
+        >>>> model.removeComponent(key)
+        """
+        diagramImplement = self.revision.getImplements().getDiagram()
+        if diagramImplement is None:
+            raise ValueError("不存在拓扑实现")
+        return diagramImplement.removeComponent(key)
+    
+    def updateComponent(self, key, args):
+        """
+        更新元件实现
+
+        :return: bool
+
+        >>>> model.updateComponent(key, args)
+        """
+        diagramImplement = self.revision.getImplements().getDiagram()
+        if diagramImplement is None:
+            raise ValueError("不存在拓扑实现")
+        return diagramImplement.updateComponent(key, args)
+
 
     def getComponentsByRid(self, rid: str):
         """
         通过指定元件类型获取元件
 
         :params str: 元件类型
 
@@ -140,15 +207,15 @@
 
         for val in self.jobs:
             if val["name"] == name:
                 jobs.append(val)
 
         return jobs
 
-    def createJob(self, jobType: str, name):
+    def createJob(self, jobType:str, name:str):
         """
         创建一个计算方案
         创建出的方案默认不加入到项目中，需要加入请调用 addJob
 
         :params jobType:  方案类型
             电磁暂态仿真方案 emtp
             移频电磁暂态仿真方案 sfemt
@@ -220,138 +287,74 @@
             model.addConfig(config)
         """
 
         self.configs.append(config)
         return config
 
     @staticmethod
-    def fetchMany(name=None, cursor=[]):
-        return asyncio.run(Model.fetchManyAsync(name, cursor))
-
-    @staticmethod
-    async def fetchManyAsync(name=None, cursor=[]):
+    def fetchMany(name=None, cursor=[],pageSize=10,owner=None):
         """
         获取用户可以运行的项目列表
 
         :params name:  查询名称，模糊查询
         :params cursor:  游标
 
         :return: 按分页信息返回项目列表
 
-        >>> data= await Model.fetchManyAsync()
-        {
-            items: [
-                {'rid': 'model/admin/share-test', 'name': '1234', 'description': '1234'}
-                ...
-            ],
-            cursor: ["1699353593000"],
-
-        }
-
+        >>> data= await Model.fetchMany()
+        [
+            {'rid': 'model/demo/demo', 'name': 'demo', 'description': 'demo'}
+            ...
+        ]
 
         """
-        query = """query($input:ModelsInput!){models(input:$input){cursor total count items{rid name description owner tags updatedAt pages{pageId resource key path mode}access{permission role}}}}"""
+        if owner is None:
+            owner = userName()
+        elif owner == "*":
+            owner = None
         variables = {
             "cursor": cursor,
-            "limit": 10,
-            "orderBy": ["updatedAt<"],
-            "permissionEveryone": ["b_any", 2**16],
+            "limit": pageSize,
+            "orderBy": [
+                "updatedAt<",
+                "type",
+                "owner",
+                "key"
+            ],
+            "owner":owner,
         }
         if name is not None:
             variables["_search"] = name
 
-        data = await graphql_fetch(query, {"input": variables})
-
+        data = graphql_request(Model.__models_query, {"input": variables})
         if "errors" in data:
             raise Exception(data["errors"][0]["message"])
-
-        return data["data"]["models"]
+        return data["data"]["models"]['items']
 
     @staticmethod
     def fetch(rid):
-        return asyncio.run(Model.fetchAsync(rid))
-
-    @staticmethod
-    async def fetchAsync(rid):
         """
         获取项目
 
         :params rid:  项目 rid
 
         :return: 返回一个项目实例
 
         >>> model=Model.fetch('model/Demo/test')
 
         """
-        query = """
-            query  t($rid:ResourceId!){
-                model(input:{rid: $rid}) {
-                    configs
-                    context
-                    description
-                    jobs
-                    name
-                    rid
-                    tags
-                    
-                    revision {
-                        author
-                        documentation
-                        graphic
-                        hash
-                        implements
-                        message
-                        parameters
-                        pins
-                        version
-                    }
-                }
-            }
-        """
-        data = await graphql_fetch(query, {"rid": rid})
+        data = graphql_request(Model.__model_query, {"rid": rid})
         if "errors" in data:
             raise Exception(data["errors"][0]["message"])
         return Model(data["data"]["model"])
 
-    def run(self, job=None, config=None, name=None, policy=None,stop_on_entry=None, **kwargs):
-        
-        job= asyncio.run(self.runAsync(job, config, name, policy,stop_on_entry, **kwargs))
-        job._Job__connect_legacy()
-        return job
-
-    async def runAsync(self, job=None, config=None, name=None, policy=None,stop_on_entry=None, **kwargs):
-        """
-
-        调用仿真
-
-        :params job:  调用仿真时使用的计算方案，不指定将使用算例保存时选中的计算方案
-        :params config:  调用仿真时使用的参数方案，不指定将使用算例保存时选中的参数方案
-        :params name:  任务名称，为空时使用项目的参数方案名称和计算方案名称
-
-        :return: 返回一个Job实例
-
-        >>> job=model.run(job,config,'')
-        job
-
-        """
-        if job is None:
-            currentJob = self.context["currentJob"]
-            job = self.jobs[currentJob]
-        if config is None:
-            currentConfig = self.context["currentConfig"]
-            config = self.configs[currentConfig]
-        revision = await self.revision.run(
-            job, config, name, self.rid, policy, **kwargs
-        )
-        if stop_on_entry is not None:
-            job['args']['stop_on_entry'] = stop_on_entry
-        return await Job.create(
-            revision["hash"], job, config, name, self.rid, policy, **kwargs
-        )
+  
+    
 
+ 
     def iesSimulationRun(self, job=None, config=None, name=None, **kwargs):
         return self.run(job=job, config=config, name=name, kwargs=kwargs)
 
     @staticmethod
     def load(filePath, format="yaml"):
         """
         加载本地项目文件
@@ -385,25 +388,21 @@
 
         >>> Model.dump(model,file)
         """
 
         IO.dump(model, file, format, compress)
 
     def save(self, key=None):
-        return asyncio.run(self.saveAsync(key))
-
-    async def saveAsync(self, key=None):
         """
         保存/创建项目
 
         key 不为空时如果远程存在相同的资源名称时将覆盖远程项目。
         key 为空时如果项目 rid 不存在则抛异常，需要重新设置 key。
         如果保存时，当前用户不是该项目的拥有者时，将重新创建项目，重建项目时如果参数的 key 为空将使用当前当前项目的 key 作为资源的 key ，当资源的 key 和远程冲突时保存失败
 
-        :params: model 项目
         :params: key 资源 id 的唯一标识符，
 
         :return: 保存成功/保存失败
 
         >>> model.save(model)
             model.save(model,'newKey') # 另存为新的项目
 
@@ -411,39 +410,36 @@
         username = userName()
 
         if key is not None:
             matchObj = re.match(r"^[-_A-Za-z0-9]+$", key, re.I | re.S)
             if matchObj:
                 self.rid = "model/" + username + "/" + key
                 try:
-                    return await Model.updateAsync(self)
+                    return Model.update(self)
                 except:
-                    return await Model.createAsync(self)
+                    return Model.create(self)
             else:
                 raise Exception("key 能包含字母数子和下划线")
         else:
             t = "(?<=/)\\S+(?=/)"
             owner = re.search(t, self.rid)
             if owner is None:
                 raise Exception("rid 错误，请传入 key")
             elif owner[0] != username:
                 rid = re.sub(t, username, self.rid)
                 try:
-                    return await Model.createAsync(self)
+                    return Model.create(self)
                 except:
                     raise Exception(rid + " 该资源已存在，无法重复创建,请修改 key")
 
-        return await Model.updateAsync(self)
+        return Model.update(self)
 
-    @staticmethod
-    def create(model):
-        return asyncio.run(Model.createAsync(model))
 
     @staticmethod
-    async def createAsync(model):
+    def create(model):
         """
         新建项目
 
         :params: model 项目
 
         :return: 保存成功/保存失败
 
@@ -456,27 +452,21 @@
         owner = re.search(t, model.rid)
 
         if owner is None:
             raise Exception("rid 错误，无法保存")
         elif owner[0] != username:
             raise Exception("rid 错误，无法保存")
 
-        modelQuery = """
-                    mutation($a:CreateModelInput!){createModel(input:$a){
-                                         rid
-                                }}
-                """
         isPublic = model.context.get("auth", "") != "private"
-        isComponent = model.context.get("category", "") == "component"
         publicRead = model.context.get("publicRead", "") != False
         auth = (65539 if publicRead else 65537) if isPublic else 0
-        revision = await ModelRevision.createAsync(model.revision, model.revision.hash)
+        revision = ModelRevision.create(model.revision, model.revision.hash)
 
-        return await graphql_fetch(
-            modelQuery,
+        return graphql_request(
+            Model.__create_model,
             {
                 "a": {
                     "rid": model.rid,
                     "revision": revision["hash"],
                     "context": model.context,
                     "configs": model.configs,
                     "jobs": model.jobs,
@@ -488,20 +478,18 @@
                         "member": 1,
                         "everyone": auth,
                     },
                 }
             },
         )
 
-    @staticmethod
-    def update(model):
-        return asyncio.run(Model.updateAsync(model))
+    
 
     @staticmethod
-    async def updateAsync(model):
+    def update(model):
         """
         更新项目
 
         :params: model 项目
 
         :return: 保存成功/保存失败
 
@@ -513,32 +501,28 @@
         owner = re.search(t, model.rid)
 
         if owner is None:
             raise Exception("rid 错误，无法保存")
         elif owner[0] != username:
             raise Exception("rid 错误，无法保存")
 
-        modelQuery = """
-                    mutation($a:UpdateModelInput!){updateModel(input:$a){
-                                         rid
-                                }}
-                """
+        
         isPublic = model.context.get("auth", "") != "private"
         isComponent = model.context.get("category", "") == "component"
         publicRead = model.context.get("publicRead", "") != False
         auth = (65539 if publicRead else 65537) if isPublic else 0
-        revision = await ModelRevision.createAsync(model.revision, model.revision.hash)
+        revision = ModelRevision.create(model.revision, model.revision.hash)
 
         xVersion = int(float(os.environ.get("X_CLOUDPSS_VERSION", 4)))
         tags = {"replace": model.tags}
         if xVersion == 3:
             tags = model.tags
 
-        return await graphql_fetch(
-            modelQuery,
+        return graphql_request(
+            Model.__update_model,
             {
                 "a": {
                     "rid": model.rid,
                     "revision": revision["hash"],
                     "context": model.context,
                     "configs": model.configs,
                     "jobs": model.jobs,
@@ -550,14 +534,16 @@
                         "member": 1,
                         "everyone": auth,
                     },
                 }
             },
         )
 
+
+    
     def fetchTopology(
         self,
         implementType=None,
         config=None,
         maximumDepth=None,
     ):
         """
@@ -578,182 +564,184 @@
             if implementType is None:
                 implementType = "emtp"
             if config is None:
                 currentConfig = self.context["currentConfig"]
                 config = self.configs[currentConfig]
             return self.revision.fetchTopology(implementType, config, maximumDepth)
         return None
+    
+    def run(self, job=None, config=None, name=None, policy=None,stop_on_entry=None, **kwargs)-> Job[View]:
+        
+        """
+
+            运行仿真任务 
+
+            :params job:  调用仿真时使用的计算方案，不指定将使用算例保存时选中的计算方案
+            :params config:  调用仿真时使用的参数方案，不指定将使用算例保存时选中的参数方案
+            :params name:  任务名称，为空时使用项目的参数方案名称和计算方案名称
+
+            :return: 返回一个运行实例
+
+            >>> runner=model.run(job,config,'')
+            runner
 
-    def runEMT(self, job=None, config=None) -> Job:
         """
-        运行 emtp 内核，如果当前 model 没有创建  Job 时报错，默认使用第一个计算方案，进行仿真。
+        if job is None:
+            currentJob = self.context["currentJob"]
+            job = self.jobs[currentJob]
+        if config is None:
+            currentConfig = self.context["currentConfig"]
+            config = self.configs[currentConfig]
+        return self.revision.run(
+            job, config, name,  policy, stop_on_entry,self.rid,**kwargs
+        )
+        
+    def __findJob(self, jobType):
+        currentJob = self.context["currentJob"]
+        job = self.jobs[currentJob]
+        if job["rid"] != jobType:
+            for j in self.jobs:
+                if j["rid"] ==jobType:
+                    job = j
+        return job        
+        
+    def runEMT(self, job=None, config=None,**kwargs) -> Job[EMTView]:
+        """
+        运行 emtp 内核，如果当前 model 没有创建  Job 时报错，默认使用算例中选中的计算方案进行仿真，如果选中的计算方案不是 EMT 方案则选第一个EMT 计算方案，如果不存在计算方案则直接报错。
 
         :param: job 计算方案名称，可选，字符串类型或者字典类型,默认使用第一个计算方案，如果同名使用最靠前一个
         :param: config 参数方案，可选，字符串类型或者字典类型,默认使用保存时选中的参数方案
 
-        :return: job 运行结果
+        :return: 生成的任务
         """
         if job is None:
-            currentJob = self.context["currentJob"]
-            job = self.jobs[currentJob]
-            if job["rid"] != "job-definition/cloudpss/emtp":
-                for j in self.jobs:
-                    if j["rid"] == "job-definition/cloudpss/emtp":
-                        job = j
+            job = self.__findJob("function/CloudPSS/emtps")
         if job is None:
             raise Exception("找不到电磁暂态运行的计算方案")
-        if job["rid"] != "job-definition/cloudpss/emtp":
+        if job["rid"] != "function/CloudPSS/emtp" and job["rid"] != "function/CloudPSS/emtps":
             raise Exception("不是电磁暂态运行生成算法的计算方案")
         if config is None:
             currentConfig = self.context["currentConfig"]
             config = self.configs[currentConfig]
-        return self.run(job=job, config=config)
+        return self.run(job=job, config=config,**kwargs)
 
-    def runSFEMT(self, job=None, config=None) -> Job:
+    def runSFEMT(self, job=None, config=None,**kwargs) -> Job[EMTView]:
         """
         运行 移频电磁暂态 内核，如果当前 model 没有创建  Job 时报错，默认使用第一个计算方案，进行仿真。
 
         :param: job 计算方案名称，可选，字符串类型或者字典类型,默认使用第一个计算方案，如果同名使用最靠前一个
         :param: config 参数方案，可选，字符串类型或者字典类型,默认使用保存时选中的参数方案
 
-        :return: runner Runner[EMTResult]
+        :return: Job[EMTView]
         """
         if job is None:
-            currentJob = self.context["currentJob"]
-            job = self.jobs[currentJob]
-            if job["rid"] != "job-definition/cloudpss/sfemt":
-                for j in self.jobs:
-                    if j["rid"] == "job-definition/cloudpss/sfemt":
-                        job = j
+            job = self.__findJob("function/CloudPSS/sfemt")
         if job is None:
             raise Exception("找不到移频电磁暂态运行的计算方案")
-        if job["rid"] != "job-definition/cloudpss/sfemt":
+        if job["rid"] != "function/CloudPSS/sfemt":
             raise Exception("不是移频电磁暂态运行生成算法的计算方案")
         if config is None:
             currentConfig = self.context["currentConfig"]
             config = self.configs[currentConfig]
         return self.run(job=job, config=config)
 
-    def runPowerFlow(self, job=None, config=None) -> Job:
+    def runPowerFlow(self, job=None, config=None,**kwargs) -> Job[PowerFlowView]:
         """
         运行 潮流 内核，如果当前 model 没有创建  Job 时报错，默认使用第一个计算方案，进行仿真。
 
         :param: job 计算方案名称，可选，字符串类型或者字典类型,默认使用第一个计算方案，如果同名使用最靠前一个
         :param: config 参数方案，可选，字符串类型或者字典类型,默认使用保存时选中的参数方案
 
-        :return: runner Runner[PowerFlowResult]
+        :return: Job[EMTView]
         """
         if job is None:
-            currentJob = self.context["currentJob"]
-            job = self.jobs[currentJob]
-            if job["rid"] != "job-definition/cloudpss/power-flow":
-                for j in self.jobs:
-                    if j["rid"] == "job-definition/cloudpss/power-flow":
-                        job = j
+            job = self.__findJob("function/CloudPSS/power-flow")
         if job is None:
             raise Exception("找不到潮流内核运行的计算方案")
-        if job["rid"] != "job-definition/cloudpss/power-flow":
+        if job["rid"] != "function/CloudPSS/power-flow":
             raise Exception("不是潮流内核运行生成算法的计算方案")
         if config is None:
             currentConfig = self.context["currentConfig"]
             config = self.configs[currentConfig]
-        return self.run(job=job, config=config)
+        return self.run(job=job, config=config,**kwargs)
 
-    def runThreePhasePowerFlow(self, job=None, config=None) -> Job:
+    def runThreePhasePowerFlow(self, job=None, config=None,**kwargs) -> Job[PowerFlowView]:
         """
         运行 三相不平衡潮流 内核，如果当前 model 没有创建  Job 时报错，默认使用第一个计算方案，进行仿真。
 
         :param: job 计算方案名称，可选，字符串类型或者字典类型,默认使用第一个计算方案，如果同名使用最靠前一个
         :param: config 参数方案，可选，字符串类型或者字典类型,默认使用保存时选中的参数方案
 
-        :return: runner Runner[PowerFlowResult]
+        :return: Job[PowerFlowView]
         """
         if job is None:
-            currentJob = self.context["currentJob"]
-            job = self.jobs[currentJob]
-            if job["rid"] != "job-definition/cloudpss/three-phase-powerFlow":
-                for j in self.jobs:
-                    if j["rid"] == "job-definition/cloudpss/three-phase-powerFlow":
-                        job = j
+            job = self.__findJob("function/CloudPSS/three-phase-powerFlow")
         if job is None:
             raise Exception("找不到三相不平衡潮流内核运行的计算方案")
-        if job["rid"] != "job-definition/cloudpss/three-phase-powerFlow":
+        if job["rid"] != "function/CloudPSS/three-phase-powerFlow":
             raise Exception("不是三相不平衡潮流内核运行生成算法的计算方案")
         if config is None:
             currentConfig = self.context["currentConfig"]
             config = self.configs[currentConfig]
-        return self.run(job=job, config=config)
+        return self.run(job=job, config=config,**kwargs)
 
-    def runIESLoadPrediction(self, job=None, config=None) -> Runner[IESResult]:
+    def runIESLoadPrediction(self, job=None, config=None,**kwargs) -> Job[IESView]:
         """
         运行 负荷预测方案 内核，如果当前 model 没有创建  Job 时报错，默认使用第一个计算方案，进行仿真。
 
         :param: job 计算方案名称，可选，字符串类型或者字典类型,默认使用第一个计算方案，如果同名使用最靠前一个
         :param: config 参数方案，可选，字符串类型或者字典类型,默认使用保存时选中的参数方案
 
-        :return: runner Runner[IESResult]
+        :return: Job[IESView]
         """
         if job is None:
-            currentJob = self.context["currentJob"]
-            job = self.jobs[currentJob]
-            if job["rid"] != "job-definition/ies/ies-load-prediction":
-                for j in self.jobs:
-                    if j["rid"] == "job-definition/ies/ies-load-prediction":
-                        job = j
+            job = self.__findJob("job-definition/ies/ies-load-prediction")
         if job is None:
             raise Exception("找不到负荷预测方案内核运行的计算方案")
         if job["rid"] != "job-definition/ies/ies-load-prediction":
             raise Exception("不是负荷预测方案内核运行生成算法的计算方案")
         if config is None:
             currentConfig = self.context["currentConfig"]
             config = self.configs[currentConfig]
         return self.run(job=job, config=config)
 
-    def runIESPowerFlow(self, job=None, config=None) -> Runner[IESResult]:
+    def runIESPowerFlow(self, job=None, config=None,**kwargs) -> Job[IESView]:
         """
         运行 时序潮流方案 内核，如果当前 model 没有创建  Job 时报错，默认使用第一个计算方案，进行仿真。
 
         :param: job 计算方案名称，可选，字符串类型或者字典类型,默认使用第一个计算方案，如果同名使用最靠前一个
         :param: config 参数方案，可选，字符串类型或者字典类型,默认使用保存时选中的参数方案
 
-        :return: runner Runner[IESResult]
+        :return: Job[IESView]
         """
         if job is None:
-            currentJob = self.context["currentJob"]
-            job = self.jobs[currentJob]
-            if job["rid"] != "job-definition/ies/ies-power-flow":
-                for j in self.jobs:
-                    if j["rid"] == "job-definition/ies/ies-power-flow":
-                        job = j
+            job = self.__findJob("job-definition/ies/ies-power-flow")
         if job is None:
             raise Exception("找不到时序潮流方案内核运行的计算方案")
         if job["rid"] != "job-definition/ies/ies-power-flow":
             raise Exception("不是时序潮流方案内核运行生成算法的计算方案")
         if config is None:
             currentConfig = self.context["currentConfig"]
             config = self.configs[currentConfig]
-        return self.run(job=job, config=config)
+        return self.run(job=job, config=config,**kwargs)
 
-    def runIESEnergyStoragePlan(self, job=None, config=None) -> Runner[IESResult]:
+    def runIESEnergyStoragePlan(self, job=None, config=None,**kwargs) -> Job[IESView]:
         """
         运行 储能规划方案 内核，如果当前 model 没有创建  Job 时报错，默认使用第一个计算方案，进行仿真。
 
         :param: job 计算方案名称，可选，字符串类型或者字典类型,默认使用第一个计算方案，如果同名使用最靠前一个
         :param: config 参数方案，可选，字符串类型或者字典类型,默认使用保存时选中的参数方案
 
-        :return: runner Runner[IESResult]
+        :return: Job[IESView]
         """
         if job is None:
-            currentJob = self.context["currentJob"]
-            job = self.jobs[currentJob]
-            if job["rid"] != "job-definition/ies/ies-energy-storage-plan":
-                for j in self.jobs:
-                    if j["rid"] == "job-definition/ies/ies-energy-storage-plan":
-                        job = j
+            job = self.__findJob("job-definition/ies/ies-energy-storage-plan")
         if job is None:
             raise Exception("找不到储能规划方案内核运行的计算方案")
         if job["rid"] != "job-definition/ies/ies-energy-storage-plan":
             raise Exception("不是储能规划方案内核运行生成算法的计算方案")
         if config is None:
             currentConfig = self.context["currentConfig"]
             config = self.configs[currentConfig]
-        return self.run(job=job, config=config)
+        return self.run(job=job, config=config,**kwargs)
+
+
```

### Comparing `cloudpss-4.1.1b8/cloudpss/model/revision.py` & `cloudpss-4.1.1b9/cloudpss/model/revision.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import asyncio
-from cloudpss.utils.httpAsyncRequest import graphql_fetch
+from cloudpss.job.job import Job
 from .topology import ModelTopology
 from .implements import ModelImplement
-from ..utils import request, graphql_request
-from ..runner import Runner
+from ..utils import  graphql_request
 
 
 class ModelRevision(object):
+    
     """
         表示一个项目的版本数据
 
         实例变量说明：
 
         implements          项目当前版本的实现数据
 
@@ -19,14 +18,20 @@
         pins                项目当前版本的引脚信息
 
         documentation       项目当前版本的文档信息
 
 
 
     """
+    
+    __createModelRevisionQuery = """
+                    mutation($a:CreateModelRevisionInput!){createModelRevision(input:$a){
+                            hash
+                    }}
+                """
 
     def __init__(self, revision: dict = {}):
         """
             初始化
         """
         for k, v in revision.items():
             if k == 'implements':
@@ -52,73 +57,62 @@
 
             :return: 实现实例
 
             >>> revision.getImplements()
         """
 
         return self.implements
-
-    async def run(self, job, config, name=None, rid='', policy=None, **kwargs):
+    
+    def run(self, job, config, name=None, policy=None,stop_on_entry=None,rid=None, **kwargs):
         """
-            运行某个指定版本的项目
+            运行当前版本
 
             :params job:  调用仿真时使用的计算方案，为空时使用项目的第一个计算方案
             :params config:  调用仿真时使用的参数方案，为空时使用项目的第一个参数方案
             :params name:  任务名称，为空时使用项目的参数方案名称和计算方案名称
             :params rid:  项目rid，可为空
 
-            :return: 返回一个ModelRevision
+            :return: 返回一个运行实例
 
             >>> revision.run(revision,job,config,'')
         """
-        return await ModelRevision.createAsync(self)
+        revision= ModelRevision.create(self)
+        if stop_on_entry is not None:
+            job['args']['stop_on_entry'] = stop_on_entry
+        return Job.create(
+            revision["hash"], job, config, name, rid, policy, **kwargs
+        )
+    
 
     @staticmethod
     def create(revision, parentHash=None):
         """
             创建一个新版本
 
             :params: revision 版本数据
 
             :return: 项目版本hash
 
             >>> ModelRevision.create(model.revision)
             {hash:'4043acbddb9ce0c6174be65573c0380415bc48186c74a459f88865313743230c'}
         """
 
-        return  asyncio.run(ModelRevision.createAsync(revision, parentHash))
-        
-    @staticmethod
-    async def createAsync(revision, parentHash=None):
-        """
-            创建一个新版本
-
-            :params: revision 版本数据
-
-            :return: 项目版本hash
-
-            >>> ModelRevision.create(model.revision)
-            {hash:'4043acbddb9ce0c6174be65573c0380415bc48186c74a459f88865313743230c'}
-        """
-
-        query = """
-                    mutation($a:CreateModelRevisionInput!){createModelRevision(input:$a){
-                            hash
-                    }}
-                """
         r = revision.toJSON()
-        del r['hash']
+        if 'hash' in r:
+            del r['hash']
         variables = {'a': {**r, 'parent': parentHash}}
-
-        r = await graphql_fetch(query, variables)
+        r = graphql_request(ModelRevision.__createModelRevisionQuery, variables)
         if 'errors' in r:
             raise Exception(r['errors'])
+        
         return r['data']['createModelRevision']
+        
+    
 
-    async def fetchTopology(self, implementType, config, maximumDepth):
+    def fetchTopology(self, implementType, config, maximumDepth):
         """
             获取当前项目版本的拓扑数据
 
             :params implementType:  实现类型
             :params config:  项目参数
             :params maximumDepth:  最大递归深度，用于自定义项目中使用 diagram 实现元件展开情况
 
@@ -127,10 +121,11 @@
             >>> topology=revision.fetchTopology()
                 topology=revision.fetchTopology(implementType='powerFlow',config=config) # 获取潮流实现的拓扑数据
                 topology=revision.fetchTopology(maximumDepth=2) # 获取仅展开 2 层的拓扑数据
 
         """
 
         if self.hash is not None:
-            return await ModelTopology.fetch(self.hash, implementType, config,
+            return ModelTopology.fetch(self.hash, implementType, config,
                                        maximumDepth)
         return None
+
```

### Comparing `cloudpss-4.1.1b8/cloudpss/model/topology.py` & `cloudpss-4.1.1b9/cloudpss/model/topology.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 import json
 
-from cloudpss.utils.httpAsyncRequest import graphql_fetch
 from ..utils import request, graphql_request
 
 
 class ModelTopology():
     """
         项目拓扑类
 
@@ -15,14 +14,21 @@
 
         components 摊平后的拓扑元件，参数和引脚不再保留表达式的形式，如果元件为拓扑实现，并有读取权限时将被展开
 
         mappings   拓扑分析后的一些映射数据
 
 
     """
+    __modelTopologyQuery = """
+            query($a:ModelTopologyInput!){
+            modelTopology(input:$a){
+                components
+                mappings
+            }}
+        """
     __All__ = ['ModelTopology']
 
     def __init__(self, topology: dict = {}):
         self.__dict__.update(topology)
 
     def toJSON(self):
         """
@@ -44,46 +50,38 @@
         data = topology.toJSON()
         f = open(filePath, 'w', encoding='utf-8')
         json.dump(data, f, indent=indent)
         f.close()
         
     @staticmethod
     def fetch(hash, implementType, config, maximumDepth=None):
-       return asyncio.run(ModelTopology.fetchAsync(hash, implementType, config, maximumDepth))
-        
-    @staticmethod
-    async def fetchAsync(hash, implementType, config, maximumDepth=None):
         """
             获取拓扑
 
             :params: hash 
             :params: implementType 实现类型
             :params: config 参数方案
             :params: maximumDepth 最大递归深度，用于自定义项目中使用 diagram 实现元件展开情况
 
             : return: 拓扑实例
 
             >>> data = ModelTopology.fetch('','emtp',{})
 
         """
         args = {} if config is None else config['args']
-        query = """
-            query($a:ModelTopologyInput!){
-            modelTopology(input:$a){
-                components
-                mappings
-            }}
-        """
-
         variables = {
             "a": {
                 'hash': hash,
                 'args': args,
                 'acceptImplementType': implementType,
                 'maximumDepth': maximumDepth
             }
         }
-        data = await graphql_fetch(query, variables)
+        data = graphql_request(ModelTopology.__modelTopologyQuery, variables)
         if 'errors' in data:
             raise Exception(data['errors'][0]['message'])
 
         return ModelTopology(data['data']['modelTopology'])
+        
+    
+
+
```

### Comparing `cloudpss-4.1.1b8/cloudpss/project/project.py` & `cloudpss-4.1.1b9/cloudpss/project/project.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/runner/DSLabResult.py` & `cloudpss-4.1.1b9/cloudpss/runner/DSLabResult.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/runner/IESLabEvaluationResult.py` & `cloudpss-4.1.1b9/cloudpss/runner/IESLabEvaluationResult.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/runner/IESLabPlanResult.py` & `cloudpss-4.1.1b9/cloudpss/runner/IESLabPlanResult.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/runner/IESLabTypicalDayResult.py` & `cloudpss-4.1.1b9/cloudpss/runner/IESLabTypicalDayResult.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/runner/MessageStreamReceiver.py` & `cloudpss-4.1.1b9/cloudpss/runner/MessageStreamReceiver.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,16 @@
     ###下面是兼容Receiver部分功能实现
     def on_message(self, ws, message):
         data = IO.deserialize(message, 'ubjson')
         msg = IO.deserialize(data['data'], 'ubjson')
         if "when" not in msg:
             msg['when']= datetime.datetime.now()
         self.db.storeMessage(msg)
+        if(msg['type']=='terminate'):
+            self.close(self.ws)
 
     def on_error(self, ws, error):
         msg = {
             'type': 'log',
             'verb': 'create',
             'version': 1,
             'data': {
```

### Comparing `cloudpss-4.1.1b8/cloudpss/runner/receiver.py` & `cloudpss-4.1.1b9/cloudpss/runner/receiver.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/runner/result.py` & `cloudpss-4.1.1b9/cloudpss/runner/result.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/runner/runner.py` & `cloudpss-4.1.1b9/cloudpss/runner/runner.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/runner/storage.py` & `cloudpss-4.1.1b9/cloudpss/runner/storage.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/runner/transform.py` & `cloudpss-4.1.1b9/cloudpss/runner/transform.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/utils/AsyncIterable.py` & `cloudpss-4.1.1b9/cloudpss/asyncio/utils/AsyncIterable.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/utils/IO.py` & `cloudpss-4.1.1b9/cloudpss/utils/IO.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/utils/dataEncoder.py` & `cloudpss-4.1.1b9/cloudpss/utils/dataEncoder.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/utils/httpAsyncRequest.py` & `cloudpss-4.1.1b9/cloudpss/asyncio/utils/httpAsyncRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 from aiohttp import ClientSession, WSMsgType
 from urllib.parse import urljoin
 import logging
-from ..version import __version__
+from ...version import __version__
 
 
 def graphql_version_check(uri, response):
     if uri.startswith("graphql"):
         if "X-Cloudpss-Version" not in response.headers:
             raise Exception("当前SDK版本（ver 3.X.X）与服务器版本（3.0.0 以下）不兼容，请更换服务器地址或更换SDK版本。")
         os.environ["X_CLOUDPSS_VERSION"] = response.headers["X-Cloudpss-Version"]
@@ -50,15 +50,15 @@
             elif 500 <= response.status < 600:
                 raise Exception(f"请求失败，状态码：{response.status}")
             else:
                 return
 
 
 # graphql实现方法
-async def graphql_fetch(query, variables=None):
+async def graphql_request(query, variables=None):
     payload = {"query": query, "variables": variables}
     return await fetch_data("POST", "graphql", data=json.dumps(payload))
 
 
 # websocket
 async def websocket_connect(url, open_func):
     async with ClientSession() as session:
```

### Comparing `cloudpss-4.1.1b8/cloudpss/utils/httprequests.py` & `cloudpss-4.1.1b9/cloudpss/utils/httprequests.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,16 +29,17 @@
                 '当前SDK版本（ver 3.X.X）与服务器版本（3.0.0 以下）不兼容，请更换服务器地址或更换SDK版本。')
         os.environ['X_CLOUDPSS_VERSION'] = r.headers['X-Cloudpss-Version']
         if float(r.headers['X-Cloudpss-Version']) >= 5:
             raise Exception('当前SDK版本（ver '+__version__ +'）与服务器版本（ver ' +
                             r.headers['X-Cloudpss-Version'] +
                             '.X.X）不兼容，请更换服务器地址或更换SDK版本(pip 使用 pip install -U cloudpss 命令更新, conda 使用 conda update cloudpss 命令更新)。')
 
-    if r.ok:
-        return r
-    logging.debug(r.text)
-    if r.text =="":
-        r.raise_for_status()
+    # if r.ok:
+    #     return r
+    # logging.debug(r.text)
+    # if r.text =="":
+    r.raise_for_status()
     if "statusCode" in r.text:
         t = json.loads(r.text)
         raise  Exception(str(t['statusCode']) + " "+t['message'])
+    return r
```

### Comparing `cloudpss-4.1.1b8/cloudpss/utils/matlab.py` & `cloudpss-4.1.1b9/cloudpss/utils/matlab.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/utils/yamlLoader.py` & `cloudpss-4.1.1b9/cloudpss/utils/yamlLoader.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss/verify.py` & `cloudpss-4.1.1b9/cloudpss/verify.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/cloudpss.egg-info/PKG-INFO` & `cloudpss-4.1.1b9/cloudpss.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpss
-Version: 4.1.1b8
+Version: 4.1.1b9
 Summary: cloudpss sdk
 Home-page: https://www.cloudpss.net
 Author: cloudpss
 Author-email: zhangdaming@cloudpss.net
 License: MIT Licence
 Keywords: cloudpss,cloudpss-sdk
 Platform: any
```

### Comparing `cloudpss-4.1.1b8/cloudpss.egg-info/SOURCES.txt` & `cloudpss-4.1.1b9/cloudpss.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 cloudpss/verify.py
 cloudpss/version.py
 cloudpss.egg-info/PKG-INFO
 cloudpss.egg-info/SOURCES.txt
 cloudpss.egg-info/dependency_links.txt
 cloudpss.egg-info/requires.txt
 cloudpss.egg-info/top_level.txt
+cloudpss/asyncio/__init__.py
+cloudpss/asyncio/job/__init__.py
+cloudpss/asyncio/job/job.py
+cloudpss/asyncio/job/messageStreamReceiver.py
+cloudpss/asyncio/job/messageStreamSender.py
+cloudpss/asyncio/model/__init__.py
+cloudpss/asyncio/model/model.py
+cloudpss/asyncio/model/revision.py
+cloudpss/asyncio/model/topology.py
+cloudpss/asyncio/utils/AsyncIterable.py
+cloudpss/asyncio/utils/__init__.py
+cloudpss/asyncio/utils/httpAsyncRequest.py
 cloudpss/dslab/__init__.py
 cloudpss/dslab/dataManageModel.py
 cloudpss/dslab/dslab.py
 cloudpss/dslab/financialAnalysisModel.py
 cloudpss/dslab/files/__init__.py
 cloudpss/dslab/files/curveData.py
 cloudpss/dslab/files/files.py
@@ -23,19 +35,15 @@
 cloudpss/ieslab/EvaluationModel.py
 cloudpss/ieslab/IESLabPlan.py
 cloudpss/ieslab/IESLabSimulation.py
 cloudpss/ieslab/PlanModel.py
 cloudpss/ieslab/__init__.py
 cloudpss/job/__init__.py
 cloudpss/job/job.py
-cloudpss/job/jobMachine.py
-cloudpss/job/jobPolicy.py
-cloudpss/job/jobQueue.py
 cloudpss/job/jobReceiver.py
-cloudpss/job/jobTres.py
 cloudpss/job/messageStreamReceiver.py
 cloudpss/job/messageStreamSender.py
 cloudpss/job/view/EMTView.py
 cloudpss/job/view/IESLabSimulationView.py
 cloudpss/job/view/IESLabTypicalDayView.py
 cloudpss/job/view/IESView.py
 cloudpss/job/view/PowerFlowView.py
@@ -59,33 +67,33 @@
 cloudpss/runner/MessageStreamReceiver.py
 cloudpss/runner/__init__.py
 cloudpss/runner/receiver.py
 cloudpss/runner/result.py
 cloudpss/runner/runner.py
 cloudpss/runner/storage.py
 cloudpss/runner/transform.py
-cloudpss/utils/AsyncIterable.py
 cloudpss/utils/IO.py
 cloudpss/utils/__init__.py
 cloudpss/utils/dataEncoder.py
 cloudpss/utils/graphqlUtil.py
-cloudpss/utils/httpAsyncRequest.py
 cloudpss/utils/httprequests.py
 cloudpss/utils/matlab.py
 cloudpss/utils/yamlLoader.py
 test/test-async.py
 test/test-async2.py
 test/test-async3.py
+test/test-plot.py
 test/test-sdk.py
 test/test-sdk1.py
 test/test-snapshot.py
 test/test-topology.py
 test/test.py
 test/test7950.py
 test/testAsync.py
 test/testEvent.py
-test/testRt copy.py
 test/testRt.py
+test/testRt2.py
 test/testSend.py
 test/test_in_new_web_1.py
 test/test_ws.py
+test/test_ws2.py
 test/testb.py
```

### Comparing `cloudpss-4.1.1b8/setup.py` & `cloudpss-4.1.1b9/setup.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/test/test-async.py` & `cloudpss-4.1.1b9/test/test-async.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/test/test-async2.py` & `cloudpss-4.1.1b9/test/test-async2.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/test/test-async3.py` & `cloudpss-4.1.1b9/test/test-async3.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/test/test-sdk.py` & `cloudpss-4.1.1b9/test/test-sdk.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/test/test-sdk1.py` & `cloudpss-4.1.1b9/test/test-sdk1.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/test/test-snapshot.py` & `cloudpss-4.1.1b9/test/test-snapshot.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/test/test-topology.py` & `cloudpss-4.1.1b9/test/test-topology.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 if __name__ == '__main__':
     os.environ['CLOUDPSS_API_URL'] = 'http://10.101.10.45/'
     print('CLOUDPSS connected')
     cloudpss.setToken(
         'eyJhbGciOiJFUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MSwidXNlcm5hbWUiOiJhZG1pbiIsInNjb3BlcyI6WyJtb2RlbDo5ODMzNSIsImZ1bmN0aW9uOjk4MzM1IiwiYXBwbGljYXRpb246OTgzMzUiXSwicm9sZXMiOlsiYWRtaW4iXSwidHlwZSI6ImFwcGx5IiwiZXhwIjoxNzI0NTU3MDIzLCJub3RlIjoiYSIsImlhdCI6MTY5MzQ1MzAyM30._Xuyo62ESKLcIAFeNdnfBM44yPiiXli9OPKvXDzL2rPV4J1_qsGZP--bsS1tXAVy-x8ooUIIAAG1yhwmZuk7-Q')
     print('Token done')
     # project = cloudpss.Model.fetch('model/admin/7744b02b-0636-5a39-8c16-eca939259ee1')
-    topology = cloudpss.ModelTopology.fetch("zL4x-BbTkoaKGU1rhmXsr_1aBFtqDV8hTIyQ29uCTuuBIdAMBCbLpIANT4kpTGfO","emtp",{'args':{}})
+    t = time.time()
+    topology = cloudpss.ModelTopology.fetch("24sne1BQ_lLCRLBnVl7_9QdhR70HxKIWsmIpKMF4iBw6tTt-h6ZkB-vUgm-nfDp2","emtp",{'args':{}})
+    # topology = cloudpss.ModelTopology.fetch("JwHbZdjco9eC0nZw3fY7Iz9rqsQ4HFGJObiBW3bFuYLPCd0Vqb2vb8zNY28D1AXV","emtp",{'args':{}})
+    print(time.time()-t)
     
     
     
     # topology= project.fetchTopology(config={'args':{}})
 
-    topology.dump(topology,'test.json')
+    # topology.dump(topology,'test.json')
```

### Comparing `cloudpss-4.1.1b8/test/test.py` & `cloudpss-4.1.1b9/test/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 
 import time
 import sys
 import os
 
+import redis
+
 sys.path.append(os.path.join(os.path.dirname(__file__), '..\\'))
 import cloudpss
 import time
 import numpy as np
 import pandas as pd
 import json
 
 if __name__ == '__main__':
-    os.environ['CLOUDPSS_API_URL'] = 'http://10.101.10.45/'
-    print('CLOUDPSS connected')
-    cloudpss.setToken(
-        'eyJhbGciOiJFUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MSwidXNlcm5hbWUiOiJhZG1pbiIsInNjb3BlcyI6WyJtb2RlbDo5ODMzNSIsImZ1bmN0aW9uOjk4MzM1IiwiYXBwbGljYXRpb246OTgzMzUiXSwicm9sZXMiOlsiYWRtaW4iXSwidHlwZSI6ImFwcGx5IiwiZXhwIjoxNzI0NTU3MDIzLCJub3RlIjoiYSIsImlhdCI6MTY5MzQ1MzAyM30._Xuyo62ESKLcIAFeNdnfBM44yPiiXli9OPKvXDzL2rPV4J1_qsGZP--bsS1tXAVy-x8ooUIIAAG1yhwmZuk7-Q')
-    print('Token done')
-    # project = cloudpss.Model.fetch('model/admin/7744b02b-0636-5a39-8c16-eca939259ee1')
-    topology = cloudpss.ModelTopology.fetch("-xrS3SewFhpVYKBtIXLk-XDLCQRQnUmlIbXS3s4sdPUkPKeAMhXHjRgZD1JPjPfQ","emtp",{'args':{}})
+    
+    client = redis.Redis(host='10.101.10.46',port=6379)
+    client.publish('read','1')
+    ps = client.pubsub()
+    # os.environ['CLOUDPSS_API_URL'] = 'http://10.101.10.45/'
+    # print('CLOUDPSS connected')
+    # cloudpss.setToken(
+    #     'eyJhbGciOiJFUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MSwidXNlcm5hbWUiOiJhZG1pbiIsInNjb3BlcyI6WyJtb2RlbDo5ODMzNSIsImZ1bmN0aW9uOjk4MzM1IiwiYXBwbGljYXRpb246OTgzMzUiXSwicm9sZXMiOlsiYWRtaW4iXSwidHlwZSI6ImFwcGx5IiwiZXhwIjoxNzI0NTU3MDIzLCJub3RlIjoiYSIsImlhdCI6MTY5MzQ1MzAyM30._Xuyo62ESKLcIAFeNdnfBM44yPiiXli9OPKvXDzL2rPV4J1_qsGZP--bsS1tXAVy-x8ooUIIAAG1yhwmZuk7-Q')
+    # print('Token done')
+    # # project = cloudpss.Model.fetch('model/admin/7744b02b-0636-5a39-8c16-eca939259ee1')
+    # topology = cloudpss.ModelTopology.fetch("-xrS3SewFhpVYKBtIXLk-XDLCQRQnUmlIbXS3s4sdPUkPKeAMhXHjRgZD1JPjPfQ","emtp",{'args':{}})
     
     
     
-    # topology= project.fetchTopology(config={'args':{}})
+    # # topology= project.fetchTopology(config={'args':{}})
 
-    topology.dump(topology,'test.json')
+    # topology.dump(topology,'test.json')
```

### Comparing `cloudpss-4.1.1b8/test/test7950.py` & `cloudpss-4.1.1b9/test/test7950.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/test/testAsync.py` & `cloudpss-4.1.1b9/test/testAsync.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/test/testEvent.py` & `cloudpss-4.1.1b9/test/testEvent.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/test/testRt.py` & `cloudpss-4.1.1b9/test/testRt2.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,26 +20,22 @@
     def __init__(self, namespace=None, *args, **kwargs):
         super().__init__(namespace)
         
         setattr(self, 'on_data-panel', self.on_data_panel)
         setattr(self, 'on_start-job', self.on_start_job)
         setattr(self, 'on_stop-job', self.on_stop_job)
         setattr(self, 'on_close-job', self.on_close_job)
-        setattr(self, 'on_load-record-data', self.on_load_record_data)
-        setattr(self, 'on_real-time-data', self.on_real_time_data)
         self.numericValueCallBack = kwargs.get('numericValueCallBack',None)
         self.chartCallBack = kwargs.get('chartCallBack',None)
         
         
         
         
     def on_connect(self):
         self.emit('start-job', { 'type': 'start-job', 'context': 'real-time-data' })
-        self.emit('real-time-data', { 'type': 'real-time-data', 'context': 'real-time-data' })
-        self.emit('data-panel', { 'type': 'data-panel', 'context': 'real-time-data' })
         pass
 
     def on_disconnect(self):
         pass
 
     def on_data_panel(self, data):
         # self.numericValue=data
@@ -68,33 +64,36 @@
         print('on_close_job',flush=True)
         self.disconnect()
         self.end=True
     def on_recording(self,data):
         print( 'on_recording',data)
     def on_load_record_data(self,data):
         print( 'on_load_record_data',data)
-    def on_real_time_data(self,d):
-        
-        data =struct.unpack('d'*int(len(d)/8),d)
+    def on_real_time_data(self,msg):
+        display=self.config['display']
+        d ={}
+        for x,v in display.items():
+            d[v]=x
+        data =struct.unpack('d'*int(len(msg)/8),msg)
         i = 0
         runTime =0
+        self.series=[]
         channelLength=int(self.config['portNumber'])+1
         virtual_input=int(self.config['virtual_input'])
         for index in range(0,len(data)):
             val = data[index]
             if(index%channelLength==0):
                 i=0
                 runTime = val
             elif i>virtual_input:
                 serieIndex = i - virtual_input - 1
                 
                 if len(self.series)-1<serieIndex:
-                    
                     serie=  {
-                        'name':  'data%d'%serieIndex,
+                        'name':  d[i-1],
                         'type': 'scatter',
                         'x': [],
                         'y': []
                     }  
                     self.series.append(serie)
                 else:
                     serie=self.series[serieIndex]
@@ -103,48 +102,65 @@
                 serie['y'].append(val)
             i+=1
         if self.chartCallBack is not None:
             self.chartCallBack(self.series)
 
     def close(self):
         self.end =True
-        self.emit('close-job', { 'type': 'close-job', 'context': 'close-job' })
+        self.disconnect()
+        # self.emit('close-job', { 'type': 'close-job', 'context': 'close-job' })
     def write(self,data):
+        print('write',data,flush=True)
         self.emit('send-message', data)
     @staticmethod
     def connect(*args, **kwargs):
         sio = socketio.Client()
         stream = RealTimeSream('',*args, **kwargs)
         
         sio.register_namespace(stream)
-        sio.connect('ws://10.101.10.119/',socketio_path='/api/real-time/socket.io')
+        
+        url = os.environ.get('CLOUDPSS_API_URL')
+        
+        if url is None:
+            url = 'http://10.101.10.91/'
+        
+        sio.connect(url,socketio_path='/api/real-time/socket.io')
     
         thread = threading.Thread(target=sio.wait, args=())
         thread.setDaemon(True)
         thread.start()
         return stream
 
 if __name__ == '__main__':
     # logging.basicConfig(level=logging.DEBUG)
-    os.environ['CLOUDPSS_API_URL'] = 'ws://10.101.10.119/'
     job = cloudpss.currentJob()
     
+    remoteAddr= job.args.get('remoteAddr','http://10.101.10.91/')
+    
+    inputKey= job.args.get('inputKey',None)
+    inputValue= job.args.get('inputValue',None)
+    
+    print('inputKey',inputKey)
+    print('inputValue',inputValue)
+    if not remoteAddr.startswith('http://'):
+        remoteAddr='http://'+remoteAddr
+    
+    
+    
+    os.environ['CLOUDPSS_API_URL'] = remoteAddr
+    
     
-    def numericValueCallBack(inputNumericValue,outputNumericValue):
-        print(inputNumericValue,flush=True)
-        
-    def chartCallBack(series):
-        job.plot(series,key='test1')
-
-    stream = RealTimeSream.connect(numericValueCallBack=numericValueCallBack,chartCallBack=chartCallBack)
     def exitCallback():
         stream.close()
         time.sleep(1)
         print('exit')
         job.exit(0)
 
     job.on_abort(exitCallback, args=(), kwargs={})
     
-    print('start',flush=True)
-    while not stream.end :
-        time.sleep(1)
-        pass
+
+    stream = RealTimeSream.connect()
+    stream.write({inputKey:float(inputValue)})
+    time.sleep(1)
+    stream.close()
+   
+    job.exit(0)
```

### Comparing `cloudpss-4.1.1b8/test/test_in_new_web_1.py` & `cloudpss-4.1.1b9/test/test_in_new_web_1.py`

 * *Files identical despite different names*

### Comparing `cloudpss-4.1.1b8/test/test_ws.py` & `cloudpss-4.1.1b9/test/test_ws.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,63 +5,61 @@
 
     
 class WebsocketClient():
     message = []
     _status=0
     # __init__(self):
     def on_close(self):
-        time.sleep(0.5)
         self._status = 1
         print("close")
-    def on_error(self):
+    def on_error(self,msg):
         self._status = 1
         print("error")
     def on_open(self):
         self._status = 0
         print("open")
     # websocket
     async def websocket_connect(self,url):
         
         # session = await ClientSession()
         # ws = await session.ws_connect(url)
 
         async with ClientSession() as session:
             async with session.ws_connect(url) as ws:
                 self.on_open()
-                async for msg in ws:
-                    # print(msg.type)
+                # async for msg in ws:
+                while True:
+                    msg = await ws.receive()
                     if msg.type == WSMsgType.BINARY:
                         self.message.append(msg)
                     if msg.type == WSMsgType.TEXT:
                         self.message.append(msg)
                     elif msg.type == WSMsgType.CLOSED:
-                        self.on_error()
+                        self.on_close()
                         break
                     elif msg.type == WSMsgType.ERROR:
-                        self.on_close(msg.data)
+                        self.on_error(msg.data)
                         break
         self._status=1
+    @property
+    async def status(self):
+        await asyncio.sleep(0)
+        return self._status
     def count(self):
         # await asyncio.sleep(0.1)
         # while self._status == 0:
         #     await asyncio.sleep(0.5)
         print(len(self.message))
         return self._status
         
     async def create(self):
-       asyncio.create_task(self.websocket_connect('ws://10.101.10.45/api/streams/id/726dfbfa-dee4-4266-89f9-c6e18d8cc72b'))
+       asyncio.create_task(self.websocket_connect('ws://10.101.10.45/api/streams/id/bb30285a-7d11-484b-a8b0-4855cf8bf8ed'))
        
 async def main():
     ws=WebsocketClient()
     task=await ws.create()
-    # task= ws.websocket_connect('ws://10.101.10.45/api/streams/id/6f6ce77c-48a1-4043-8549-1eb72a1a45c7')
-    # print(task)
-    # await ws.count()
-    while ws.count() == 0:
-        # time.sleep(0.5)
-        await asyncio.sleep(0.5)
-    # task_list=[asyncio.create_task(ws.count())]
-    # await asyncio.wait(task_list)
-    # print(x[0].pop().result())
+    while (await ws.status == 0):
+        pass
+    ws.count()  
 if __name__ == '__main__':
     
     asyncio.run(main())
```

