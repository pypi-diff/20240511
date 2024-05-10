# Comparing `tmp/gantry_logger-0.0.2a6.tar.gz` & `tmp/gantry_logger-0.0.2a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantry_logger-0.0.2a6.tar", last modified: Tue Apr 23 23:48:47 2024, max compression
+gzip compressed data, was "gantry_logger-0.0.2a7.tar", last modified: Fri May 10 22:47:21 2024, max compression
```

## Comparing `gantry_logger-0.0.2a6.tar` & `gantry_logger-0.0.2a7.tar`

### file list

```diff
@@ -1,82 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.414418 gantry_logger-0.0.2a6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.414418 gantry_logger-0.0.2a6/src/gantry/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/evaluations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.414418 gantry_logger-0.0.2a6/src/gantry/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/eval_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/eval_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/log_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.414418 gantry_logger-0.0.2a6/src/gantry/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.422418 gantry_logger-0.0.2a6/src/gantry/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/createragevaluationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/criteriafeedback.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/criteriaresultcapture.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/criteriastats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/criteriastatuscount.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/customstep.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evalcriteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evalstats.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationcriteriastatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrecordstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrun.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunjobstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunpreupload.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunpreuploadresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/functionstep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/getlogssummaryrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/getragevaluationresultsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/getragevaluationresultsresponseresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/llmevaluationcriteriatype.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/llmevaluationerrortype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/llmstep.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordresponseresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/organizationtier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/orguser.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/passfailunsurerubricscalevalues.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/ragcriteriaresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/ragevaluationresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/ragrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/recordstatuscount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/retrievalstep.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/stepformat.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/summarynotesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/topicstats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.422418 gantry_logger-0.0.2a6/src/gantry/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/src/gantry/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/operations/create_evaluation_run_pre_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/operations/create_rag_evaluation_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/operations/get_rag_evaluation_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/operations/log_rag_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/src/gantry/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    29680 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-23 23:48:47.000000 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-23 23:48:47.000000 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:48:47.000000 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 23:48:47.000000 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 23:48:47.000000 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:47:21.477571 gantry_logger-0.0.2a7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-10 22:47:21.477571 gantry_logger-0.0.2a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-10 22:47:21.477571 gantry_logger-0.0.2a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:47:21.461571 gantry_logger-0.0.2a7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:47:21.465571 gantry_logger-0.0.2a7/src/gantry/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:47:21.465571 gantry_logger-0.0.2a7/src/gantry/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/evaluations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:47:21.465571 gantry_logger-0.0.2a7/src/gantry/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/logger/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/logger/eval_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/logger/eval_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/logger/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/logger/log_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/logger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:47:21.465571 gantry_logger-0.0.2a7/src/gantry/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:47:21.473571 gantry_logger-0.0.2a7/src/gantry/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/createragevaluationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/criteriafeedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/criteriaresultcapture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/criteriastats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/criteriastatuscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/customstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/evalcriteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/evalstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/evaluationcriteriastatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/evaluationrecordstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/evaluationrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/evaluationrunjobstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/evaluationrunpreupload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/evaluationrunpreuploadresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/evaluationrunresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/functionstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/getlogssummaryrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/getragevaluationresultsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/getragevaluationresultsresponseresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/llmevaluationcriteriatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/llmevaluationerrortype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/llmstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/logerrorrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/logerrorresponseresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/logragrecordrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/logragrecordresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/logragrecordresponseresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/organizationtier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/orguser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/passfailunsurerubricscalevalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/ragcriteriaresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/ragevaluationresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/ragrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/recordstatuscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/retrievalstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/stepformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/summarynotesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/topicstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/unsupportedquestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/components/unsupportedquestiontype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:47:21.473571 gantry_logger-0.0.2a7/src/gantry/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:47:21.477571 gantry_logger-0.0.2a7/src/gantry/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/operations/create_evaluation_run_pre_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/operations/create_rag_evaluation_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/operations/get_rag_evaluation_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/operations/log_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/models/operations/log_rag_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:47:21.477571 gantry_logger-0.0.2a7/src/gantry/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-10 22:47:14.000000 gantry_logger-0.0.2a7/src/gantry/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:47:21.477571 gantry_logger-0.0.2a7/src/gantry_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-10 22:47:21.000000 gantry_logger-0.0.2a7/src/gantry_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-10 22:47:21.000000 gantry_logger-0.0.2a7/src/gantry_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:47:21.000000 gantry_logger-0.0.2a7/src/gantry_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 22:47:21.000000 gantry_logger-0.0.2a7/src/gantry_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 22:47:21.000000 gantry_logger-0.0.2a7/src/gantry_logger.egg-info/top_level.txt
```

### Comparing `gantry_logger-0.0.2a6/PKG-INFO` & `gantry_logger-0.0.2a7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry-logger
-Version: 0.0.2a6
+Version: 0.0.2a7
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `gantry_logger-0.0.2a6/setup.py` & `gantry_logger-0.0.2a7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-version = "0.0.2a6"
+version = "0.0.2a7"
 
 
 install_requires = [
     "pydantic",
     "certifi>=2023.7.22",
     "charset-normalizer>=3.2.0",
     "dataclasses-json>=0.6.1",
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/evaluations.py` & `gantry_logger-0.0.2a7/src/gantry/logs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,139 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
+import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from gantry import utils
+from gantry._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from gantry.models import components, errors, operations
 from typing import Optional
 
-class Evaluations:
+class Logs:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create_evaluation_run_pre_upload(self) -> operations.CreateEvaluationRunPreUploadResponse:
-        r"""Generate a pre-signed URL to upload an evaluation dataset"""
+    def log_rag_records(self, request: components.LogRagRecordRequest) -> operations.LogRagRecordsResponse:
+        r"""An endpoint to log RAG records"""
+        hook_ctx = HookContext(operation_id='log_rag_records', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/api/v2/evaluation_runs/pre-upload'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
+        url = base_url + '/api/v2/logs/rag'
         
         if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
-        
-        http_res = client.request('POST', url, headers=headers)
-        content_type = http_res.headers.get('Content-Type')
-        
-        res = operations.CreateEvaluationRunPreUploadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[components.EvaluationRunPreUploadResponse])
-                res.evaluation_run_pre_upload_response = out
-            else:
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
-    def create_rag_evaluation_run(self, request: components.CreateRAGEvaluationRequest) -> operations.CreateRagEvaluationRunResponse:
-        r"""Create a new RAG evaluation and kick off the workflow. Returns the created evaluation run"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = base_url + '/api/v2/rag_evaluation_runs'
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, components.CreateRAGEvaluationRequest, "request", False, False, 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+        req_content_type, data, form = utils.serialize_request_body(request, components.LogRagRecordRequest, "request", False, False, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
-        if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+        try:
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.CreateRagEvaluationRunResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.LogRagRecordsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[components.EvaluationRunResponse])
-                res.evaluation_run_response = out
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.LogRagRecordResponseResponse])
+                res.log_rag_record_response_response = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_rag_evaluation_results(self, request: operations.GetRagEvaluationResultsRequest) -> operations.GetRagEvaluationResultsResponse:
-        r"""Get a list of evaluation run results"""
+    def log_error(self, request: components.LogErrorRequest) -> operations.LogErrorResponse:
+        r"""Log an error to Sentry and DataDog. This is called by the SDK so we can better
+        debug client side issues.
+        """
+        hook_ctx = HookContext(operation_id='log_error', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetRagEvaluationResultsRequest, base_url, '/api/v2/rag_evaluation_runs/{evaluation_run_id}/results', request)
-        headers = {}
-        query_params = utils.get_query_params(operations.GetRagEvaluationResultsRequest, request)
+        url = base_url + '/api/v2/logs/error'
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        req_content_type, data, form = utils.serialize_request_body(request, components.LogErrorRequest, "request", False, False, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
         
-        if callable(self.sdk_configuration.security):
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security())
+        try:
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
         else:
-            client = utils.configure_security_client(self.sdk_configuration.client, self.sdk_configuration.security)
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
-        content_type = http_res.headers.get('Content-Type')
         
-        res = operations.GetRagEvaluationResultsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.LogErrorResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[components.GetRagEvaluationResultsResponseResponse])
-                res.get_rag_evaluation_results_response_response = out
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.LogErrorResponseResponse])
+                res.log_error_response_response = out
             else:
+                content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/logger/consumer.py` & `gantry_logger-0.0.2a7/src/gantry/logger/consumer.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/logger/eval_logger.py` & `gantry_logger-0.0.2a7/src/gantry/logger/eval_logger.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/logger/eval_reports.py` & `gantry_logger-0.0.2a7/src/gantry/logger/eval_reports.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/logger/langchain_callback.py` & `gantry_logger-0.0.2a7/src/gantry/logger/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/logger/log_location.py` & `gantry_logger-0.0.2a7/src/gantry/logger/log_location.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 import json
 import logging
+import traceback
 from abc import ABC, abstractmethod
 from queue import Queue
 from typing import Dict, List, Optional
 
 import requests
 from gantry.logger.consumer import BatchConsumer
 from gantry.logger.eval_reports import EvaluationReport
 from gantry.logger.utils import _init_gantry
 from gantry.models.components.createragevaluationrequest import (
     CreateRAGEvaluationRequest,
 )
+from gantry.models.components.logerrorrequest import LogErrorRequest
 from gantry.models.components.logragrecordrequest import LogRagRecordRequest
 
 logger = logging.getLogger(__name__)
 
 
 class EvalReportAlreadyCreated(Exception):
     pass
@@ -157,26 +159,31 @@
         # for thread consumer to continue running.
         try:
             self._sdk.logs.log_rag_records(
                 LogRagRecordRequest(records=batch, source_name=self._source_name)
             )
         except Exception as e:
             logger.error("Internal error sending batches: %s", e)
+            self._sdk.logs.log_error(
+                LogErrorRequest(
+                    exception_type=type(e).__name__,
+                    exception_value=str(e),
+                    exception_traceback="\n".join(traceback.format_exception(e)),
+                )
+            )
 
     def open(self):
         pass
 
     def write(self, data):
         """Push the record to the logs api."""
         if self.send_in_background:
             self.queue.put(data)
         else:
-            self._sdk.logs.log_rag_records(
-                LogRagRecordRequest(records=[data], source_name=self._source_name)
-            )
+            self.consumer_func([data])
 
     def close(self):
         for consumer in self.consumers:
             consumer.pause()
             try:
                 consumer.join()
             except RuntimeError:
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/logger/utils.py` & `gantry_logger-0.0.2a7/src/gantry/logger/utils.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/__init__.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from .functionstep import *
 from .getlogssummaryrequest import *
 from .getragevaluationresultsresponse import *
 from .getragevaluationresultsresponseresponse import *
 from .llmevaluationcriteriatype import *
 from .llmevaluationerrortype import *
 from .llmstep import *
+from .logerrorrequest import *
+from .logerrorresponseresponse import *
 from .logragrecordrequest import *
 from .logragrecordresponse import *
 from .logragrecordresponseresponse import *
 from .message import *
 from .organizationtier import *
 from .orguser import *
 from .passfailunsurerubricscalevalues import *
@@ -34,10 +36,13 @@
 from .ragevaluationresult import *
 from .ragrecord import *
 from .recordstatuscount import *
 from .retrievalstep import *
 from .security import *
 from .stepformat import *
 from .summarynotesresponse import *
+from .topic import *
 from .topicstats import *
+from .unsupportedquestion import *
+from .unsupportedquestiontype import *
 
-__all__ = ["Args","CreateRAGEvaluationRequest","CriteriaFeedback","CriteriaResultCapture","CriteriaStats","CriteriaStatusCount","CustomStep","CustomStepType","Document","EvalCriteria","EvalStats","EvaluationCriteriaStatus","EvaluationRecordStatus","EvaluationRun","EvaluationRunJobStatus","EvaluationRunPreUpload","EvaluationRunPreUploadResponse","EvaluationRunResponse","FunctionCall","FunctionStep","FunctionStepType","GetLogsSummaryRequest","GetRagEvaluationResultsResponse","GetRagEvaluationResultsResponseResponse","Inputs","LLMEvaluationCriteriaType","LLMEvaluationErrorType","LLMStep","LLMStepType","LogRagRecordRequest","LogRagRecordResponse","LogRagRecordResponseResponse","Message","Metadata","OrgUser","OrganizationTier","Outputs","Params","PassFailUnsureRubricScaleValues","RagCriteriaResult","RagCriteriaStepType","RagEvaluationResult","RagRecord","RagRecordMetadata","RecordStatusCount","Response2","RetrievalStep","Security","StepFormat","SummaryNotesResponse","ToolCalls","TopicStats","Two","Type"]
+__all__ = ["Args","CreateRAGEvaluationRequest","CriteriaFeedback","CriteriaResultCapture","CriteriaStats","CriteriaStatusCount","CustomStep","CustomStepType","Document","EvalCriteria","EvalStats","EvaluationCriteriaStatus","EvaluationRecordStatus","EvaluationRun","EvaluationRunJobStatus","EvaluationRunPreUpload","EvaluationRunPreUploadResponse","EvaluationRunResponse","FunctionCall","FunctionStep","FunctionStepType","GetLogsSummaryRequest","GetRagEvaluationResultsResponse","GetRagEvaluationResultsResponseResponse","Inputs","LLMEvaluationCriteriaType","LLMEvaluationErrorType","LLMStep","LLMStepType","LogErrorRequest","LogErrorResponseResponse","LogRagRecordRequest","LogRagRecordResponse","LogRagRecordResponseResponse","Message","Metadata","OrgUser","OrganizationTier","Outputs","Params","PassFailUnsureRubricScaleValues","RagCriteriaResult","RagCriteriaStepType","RagEvaluationResult","RagRecord","RagRecordMetadata","RecordStatusCount","Response2","RetrievalStep","Security","StepFormat","SummaryNotesResponse","ToolCalls","Topic","TopicStats","Two","Type","UnsupportedQuestion","UnsupportedQuestionType"]
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/createragevaluationrequest.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/createragevaluationrequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 @dataclasses.dataclass
 class CreateRAGEvaluationRequest:
     r"""Base Pydantic model to use when validating API request data instead
     of pydantic.BaseModel.
     This raises validation errors as GantryRequestValidationError so they can
     be caught and returned as 400s.
     """
-    concepts_mapping: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('concepts_mapping') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    copy_dataset_from_run_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('copy_dataset_from_run_id'), 'exclude': lambda f: f is None }})
-    custom_criteria_ids: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom_criteria_ids'), 'exclude': lambda f: f is None }})
+    concepts_mapping: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('concepts_mapping') }})
+    pending_dataset_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pending_dataset_id'), 'exclude': lambda f: f is None }})
     logs_query: Optional[GetLogsSummaryRequest] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logs_query'), 'exclude': lambda f: f is None }})
     r"""Base Pydantic model to use when validating API request data instead
     of pydantic.BaseModel.
     This raises validation errors as GantryRequestValidationError so they can
     be caught and returned as 400s.
     """
-    pending_dataset_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pending_dataset_id'), 'exclude': lambda f: f is None }})
+    custom_criteria_ids: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom_criteria_ids'), 'exclude': lambda f: f is None }})
     prompt_version_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt_version_id'), 'exclude': lambda f: f is None }})
+    copy_dataset_from_run_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('copy_dataset_from_run_id'), 'exclude': lambda f: f is None }})
+    topic_ids: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topic_ids'), 'exclude': lambda f: f is None }})
+    unsupported_question_ids: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unsupported_question_ids'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/criteriafeedback.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/criteriafeedback.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from dataclasses_json import Undefined, dataclass_json
 from gantry import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CriteriaFeedback:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     comment: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('comment') }})
     current: CriteriaResultCapture = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})
     r"""CriteriaResultCapture stores current and update values in CriteriaFeedback"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     update: CriteriaResultCapture = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('update') }})
     r"""CriteriaResultCapture stores current and update values in CriteriaFeedback"""
     updated_at: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updated_at') }})
     updated_by: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updated_by') }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/criteriaresultcapture.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/criteriaresultcapture.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/criteriastats.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/criteriastats.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 from dataclasses_json import Undefined, dataclass_json
 from gantry import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CriteriaStats:
-    criteria_eval_instruction: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_eval_instruction') }})
     criteria_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_id') }})
     criteria_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_name') }})
+    criteria_eval_instruction: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_eval_instruction') }})
     score_count: CriteriaStatusCount = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('score_count') }})
     r"""Criteria status aggregated at record level"""
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/criteriastatuscount.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/criteriastatuscount.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CriteriaStatusCount:
     r"""Criteria status aggregated at record level"""
-    error: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ERROR'), 'exclude': lambda f: f is None }})
-    fail: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('FAIL'), 'exclude': lambda f: f is None }})
-    feedback: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('FEEDBACK'), 'exclude': lambda f: f is None }})
-    not_applicable: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('NOT_APPLICABLE'), 'exclude': lambda f: f is None }})
     pass_: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('PASS'), 'exclude': lambda f: f is None }})
+    fail: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('FAIL'), 'exclude': lambda f: f is None }})
     unsure: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('UNSURE'), 'exclude': lambda f: f is None }})
+    not_applicable: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('NOT_APPLICABLE'), 'exclude': lambda f: f is None }})
+    error: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ERROR'), 'exclude': lambda f: f is None }})
+    feedback: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('FEEDBACK'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/customstep.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/customstep.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/document.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/document.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/evalcriteria.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/evalcriteria.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 @dataclasses.dataclass
 class EvalCriteria:
     r"""Criteria that was used in running an evaluation
     These are stored on the evaluation object itself
     so that we know what criteria was used to run the evaluation. This
     is to future proof the eval in case the criteria is changed after the eval
     """
-    criteria_type: LLMEvaluationCriteriaType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_type') }})
-    r"""An enumeration."""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    criteria_type: LLMEvaluationCriteriaType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_type') }})
+    r"""An enumeration."""
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/evalstats.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/evalstats.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from gantry import utils
 from typing import Dict, List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class EvalStats:
+    total_record_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total_record_count') }})
+    record_status_count: RecordStatusCount = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('record_status_count') }})
     all_criteria_stats: CriteriaStatusCount = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('all_criteria_stats') }})
     r"""Criteria status aggregated at record level"""
-    record_status_count: RecordStatusCount = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('record_status_count') }})
-    total_record_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total_record_count') }})
     criteria_stats: Optional[Dict[str, CriteriaStats]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_stats'), 'exclude': lambda f: f is None }})
     ordered_criteria_stats: Optional[List[CriteriaStats]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ordered_criteria_stats'), 'exclude': lambda f: f is None }})
     topic_stats: Optional[List[TopicStats]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topic_stats'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrun.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/evaluationrun.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,40 +3,45 @@
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from .evalcriteria import EvalCriteria
 from .evalstats import EvalStats
 from .evaluationrunjobstatus import EvaluationRunJobStatus
 from .getlogssummaryrequest import GetLogsSummaryRequest
+from .topic import Topic
+from .unsupportedquestion import UnsupportedQuestion
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from gantry import utils
 from typing import Dict, List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class EvaluationRun:
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
-    evaluation_job_status: EvaluationRunJobStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('evaluation_job_status') }})
-    r"""An enumeration."""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     organization_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('organization_id') }})
+    evaluation_job_status: EvaluationRunJobStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('evaluation_job_status') }})
+    r"""An enumeration."""
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     column_mapping: Optional[Dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('column_mapping'), 'exclude': lambda f: f is None }})
-    completed_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('completed_at'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
-    created_by: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_by'), 'exclude': lambda f: f is None }})
-    is_draft: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_draft'), 'exclude': lambda f: f is None }})
-    llm_evaluation_criterias: Optional[List[EvalCriteria]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('llm_evaluation_criterias'), 'exclude': lambda f: f is None }})
+    pending_dataset_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pending_dataset_id'), 'exclude': lambda f: f is None }})
+    raw_dataset_path: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raw_dataset_path'), 'exclude': lambda f: f is None }})
     logs_query: Optional[GetLogsSummaryRequest] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logs_query'), 'exclude': lambda f: f is None }})
     r"""Base Pydantic model to use when validating API request data instead
     of pydantic.BaseModel.
     This raises validation errors as GantryRequestValidationError so they can
     be caught and returned as 400s.
     """
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    llm_evaluation_criterias: Optional[List[EvalCriteria]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('llm_evaluation_criterias'), 'exclude': lambda f: f is None }})
+    created_by: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_by'), 'exclude': lambda f: f is None }})
+    completed_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('completed_at'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+    is_draft: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_draft'), 'exclude': lambda f: f is None }})
     num_records: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_records'), 'exclude': lambda f: f is None }})
     num_tokens: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_tokens'), 'exclude': lambda f: f is None }})
-    pending_dataset_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pending_dataset_id'), 'exclude': lambda f: f is None }})
+    bookmarked: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bookmarked'), 'exclude': lambda f: f is None }})
+    topics: Optional[List[Topic]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topics'), 'exclude': lambda f: f is None }})
+    unsupported_questions: Optional[List[UnsupportedQuestion]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unsupported_questions'), 'exclude': lambda f: f is None }})
     rag_stats: Optional[EvalStats] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rag_stats'), 'exclude': lambda f: f is None }})
-    raw_dataset_path: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raw_dataset_path'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunpreupload.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/evaluationrunpreupload.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunpreuploadresponse.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/evaluationrunpreuploadresponse.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunresponse.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/evaluationrunresponse.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/functionstep.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/functionstep.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class Args:
     pass
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class FunctionStep:
-    args: Args = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('args') }})
+    type: FunctionStepType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    args: Args = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('args') }})
     output: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('output') }})
-    type: FunctionStepType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     format: Optional[StepFormat] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format'), 'exclude': lambda f: f is None }})
     r"""An enumeration."""
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/getlogssummaryrequest.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/getlogssummaryrequest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 class GetLogsSummaryRequest:
     r"""Base Pydantic model to use when validating API request data instead
     of pydantic.BaseModel.
     This raises validation errors as GantryRequestValidationError so they can
     be caught and returned as 400s.
     """
     source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source_id') }})
+    start_time: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_time'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     end_time: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_time'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     relative_time_range: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('relative_time_range'), 'exclude': lambda f: f is None }})
     sample_percentage: Optional[int] = dataclasses.field(default=100, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sample_percentage'), 'exclude': lambda f: f is None }})
-    start_time: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_time'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/getragevaluationresultsresponse.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/getragevaluationresultsresponse.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     r"""Base Pydantic model to use when validating API request data instead
     of pydantic.BaseModel.
     This raises validation errors as GantryRequestValidationError so they can
     be caught and returned as 400s.
     """
     evaluation_results: List[RagEvaluationResult] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('evaluation_results') }})
     summary_notes: SummaryNotesResponse = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('summary_notes') }})
-    has_next: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has_next'), 'exclude': lambda f: f is None }})
     start: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start'), 'exclude': lambda f: f is None }})
+    has_next: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has_next'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/getragevaluationresultsresponseresponse.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/getragevaluationresultsresponseresponse.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/llmstep.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/llmstep.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class Response2:
     pass
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class LLMStep:
+    type: LLMStepType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     messages: List[Message] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages') }})
     response: Union[str, Response2] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('response') }})
-    type: LLMStepType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     format: Optional[StepFormat] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format'), 'exclude': lambda f: f is None }})
     r"""An enumeration."""
     params: Optional[Params] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('params'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordrequest.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/logragrecordrequest.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordresponse.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/logragrecordresponse.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 @dataclasses.dataclass
 class LogRagRecordResponse:
     r"""Base Pydantic model to use when validating API request data instead
     of pydantic.BaseModel.
     This raises validation errors as GantryRequestValidationError so they can
     be caught and returned as 400s.
     """
-    num_failure: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_failure'), 'exclude': lambda f: f is None }})
     num_success: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_success'), 'exclude': lambda f: f is None }})
+    num_failure: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_failure'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordresponseresponse.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/logragrecordresponseresponse.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/message.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/message.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,14 @@
     pass
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Message:
     type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
     format: Optional[StepFormat] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format'), 'exclude': lambda f: f is None }})
     r"""An enumeration."""
+    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
     function_call: Optional[FunctionCall] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('function_call'), 'exclude': lambda f: f is None }})
     tool_calls: Optional[List[ToolCalls]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tool_calls'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/orguser.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/orguser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from gantry import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class OrgUser:
-    email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    auth0_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth0_id'), 'exclude': lambda f: f is None }})
+    email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    auth0_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth0_id'), 'exclude': lambda f: f is None }})
     org_ids: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org_ids'), 'exclude': lambda f: f is None }})
     org_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org_name'), 'exclude': lambda f: f is None }})
     org_tier: Optional[OrganizationTier] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org_tier'), 'exclude': lambda f: f is None }})
     r"""Represents the different tiers an organization can have."""
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/ragcriteriaresult.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/ragcriteriaresult.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class RagCriteriaResult:
     r"""Stores an evaluation criteria generation's parsed score and
     reasoning for a particular RAG step.
     """
-    criteria_eval_instruction: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_eval_instruction') }})
     criteria_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_id') }})
     criteria_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_name') }})
-    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error_message'), 'exclude': lambda f: f is None }})
-    error_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error_type'), 'exclude': lambda f: f is None }})
+    criteria_eval_instruction: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_eval_instruction') }})
+    status: Optional[EvaluationCriteriaStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    r"""An enumeration."""
     feedback: Optional[List[CriteriaFeedback]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('feedback'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    steps: Optional[List[int]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('steps'), 'exclude': lambda f: f is None }})
     include_input_step: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('include_input_step'), 'exclude': lambda f: f is None }})
     include_output_step: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('include_output_step'), 'exclude': lambda f: f is None }})
-    reasoning: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reasoning'), 'exclude': lambda f: f is None }})
     relevant_step: Optional[RagCriteriaStepType] = dataclasses.field(default=RagCriteriaStepType.OUTPUT, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('relevant_step'), 'exclude': lambda f: f is None }})
     score: Optional[PassFailUnsureRubricScaleValues] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('score'), 'exclude': lambda f: f is None }})
     r"""An enumeration."""
-    status: Optional[EvaluationCriteriaStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    r"""An enumeration."""
-    steps: Optional[List[int]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('steps'), 'exclude': lambda f: f is None }})
+    reasoning: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reasoning'), 'exclude': lambda f: f is None }})
+    error_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error_type'), 'exclude': lambda f: f is None }})
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error_message'), 'exclude': lambda f: f is None }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/ragevaluationresult.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/ragevaluationresult.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,19 +17,19 @@
     r"""RagEvaluationResult stores both in-flight and completed evaluation result values.
 
     Completed evaluation results are mapped to EvaluationResults Dynamo model and stored in
     DynamoDB.
 
     TODO: Create class inheritance based on the in-flight status of the evaluation result.
     """
-    criteria_results: List[RagCriteriaResult] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_results') }})
-    record: RagRecord = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('record') }})
     record_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('record_id') }})
+    timestamp: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp') }})
     status: EvaluationRecordStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     r"""An enumeration."""
-    timestamp: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp') }})
+    record: RagRecord = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('record') }})
+    criteria_results: List[RagCriteriaResult] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria_results') }})
     topics: List[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topics') }})
-    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error_message'), 'exclude': lambda f: f is None }})
     error_type: Optional[LLMEvaluationErrorType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error_type'), 'exclude': lambda f: f is None }})
     r"""An enumeration."""
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error_message'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/ragrecord.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/ragrecord.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,12 +31,12 @@
 @dataclasses.dataclass
 class RagRecord:
     inputs: Inputs = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs') }})
     outputs: Outputs = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('outputs') }})
     steps: List[Union[RetrievalStep, LLMStep, FunctionStep, CustomStep]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('steps') }})
     format: Optional[StepFormat] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format'), 'exclude': lambda f: f is None }})
     r"""An enumeration."""
-    labels: Optional[Dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('labels'), 'exclude': lambda f: f is None }})
     metadata: Optional[RagRecordMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    labels: Optional[Dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('labels'), 'exclude': lambda f: f is None }})
     session_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('session_id'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/recordstatuscount.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/recordstatuscount.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 from gantry import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class RecordStatusCount:
-    failed: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('FAILED'), 'exclude': lambda f: f is None }})
     running: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RUNNING'), 'exclude': lambda f: f is None }})
+    failed: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('FAILED'), 'exclude': lambda f: f is None }})
     succeeded: Optional[int] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('SUCCEEDED'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/retrievalstep.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/retrievalstep.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class Metadata:
     pass
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class RetrievalStep:
-    documents: List[Document] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('documents') }})
-    query: Union[str, Two] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query') }})
     type: Type = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    query: Union[str, Two] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query') }})
+    documents: List[Document] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('documents') }})
     format: Optional[StepFormat] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format'), 'exclude': lambda f: f is None }})
     r"""An enumeration."""
     metadata: Optional[Metadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/summarynotesresponse.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/summarynotesresponse.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/components/topicstats.py` & `gantry_logger-0.0.2a7/src/gantry/models/components/topicstats.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/errors/sdkerror.py` & `gantry_logger-0.0.2a7/src/gantry/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/operations/create_evaluation_run_pre_upload.py` & `gantry_logger-0.0.2a7/src/gantry/models/operations/create_evaluation_run_pre_upload.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateEvaluationRunPreUploadResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
-    raw_response: requests_http.Response = dataclasses.field()
-    r"""Raw HTTP response; suitable for custom response parsing"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
+    raw_response: requests_http.Response = dataclasses.field()
+    r"""Raw HTTP response; suitable for custom response parsing"""
     evaluation_run_pre_upload_response: Optional[components_evaluationrunpreuploadresponse.EvaluationRunPreUploadResponse] = dataclasses.field(default=None)
     r"""OK"""
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/operations/create_rag_evaluation_run.py` & `gantry_logger-0.0.2a7/src/gantry/models/operations/create_rag_evaluation_run.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateRagEvaluationRunResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
-    raw_response: requests_http.Response = dataclasses.field()
-    r"""Raw HTTP response; suitable for custom response parsing"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
+    raw_response: requests_http.Response = dataclasses.field()
+    r"""Raw HTTP response; suitable for custom response parsing"""
     evaluation_run_response: Optional[components_evaluationrunresponse.EvaluationRunResponse] = dataclasses.field(default=None)
     r"""OK"""
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/operations/get_rag_evaluation_results.py` & `gantry_logger-0.0.2a7/src/gantry/models/operations/get_rag_evaluation_results.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 class Two(str, Enum):
     NAN = 'nan'
 
 
 @dataclasses.dataclass
 class GetRagEvaluationResultsRequest:
     evaluation_run_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'evaluation_run_id', 'style': 'simple', 'explode': False }})
-    criteria_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'criteria_id', 'style': 'form', 'explode': False }})
+    start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': False }})
     limit: Optional[int] = dataclasses.field(default=10, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': False }})
     search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': False }})
-    start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': False }})
+    criteria_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'criteria_id', 'style': 'form', 'explode': False }})
     winner_version: Optional[Union[str, Two]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'winner_version', 'style': 'form', 'explode': False }})
     
 
 
 
 @dataclasses.dataclass
 class GetRagEvaluationResultsResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
-    raw_response: requests_http.Response = dataclasses.field()
-    r"""Raw HTTP response; suitable for custom response parsing"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
+    raw_response: requests_http.Response = dataclasses.field()
+    r"""Raw HTTP response; suitable for custom response parsing"""
     get_rag_evaluation_results_response_response: Optional[components_getragevaluationresultsresponseresponse.GetRagEvaluationResultsResponseResponse] = dataclasses.field(default=None)
     r"""OK"""
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/models/operations/log_rag_records.py` & `gantry_logger-0.0.2a7/src/gantry/models/operations/log_rag_records.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class LogRagRecordsResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
-    raw_response: requests_http.Response = dataclasses.field()
-    r"""Raw HTTP response; suitable for custom response parsing"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
+    raw_response: requests_http.Response = dataclasses.field()
+    r"""Raw HTTP response; suitable for custom response parsing"""
     log_rag_record_response_response: Optional[components_logragrecordresponseresponse.LogRagRecordResponseResponse] = dataclasses.field(default=None)
     r"""OK"""
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/sdk.py` & `gantry_logger-0.0.2a7/src/gantry/sdk.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,79 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .evaluations import Evaluations
 from .logs import Logs
 from .sdkconfiguration import SDKConfiguration
+from .utils.retries import RetryConfig
 from gantry import utils
+from gantry._hooks import SDKHooks
 from gantry.models import components
-from typing import Dict
+from typing import Callable, Dict, Optional, Union
 
 class Gantry:
     evaluations: Evaluations
     logs: Logs
 
     sdk_configuration: SDKConfiguration
 
     def __init__(self,
-                 api_key_auth: str ,
-                 server_idx: int = None,
-                 server_url: str = None,
-                 url_params: Dict[str, str] = None,
-                 client: requests_http.Session = None,
-                 retry_config: utils.RetryConfig = None
+                 api_key_auth: Union[str, Callable[[], str]],
+                 server_idx: Optional[int] = None,
+                 server_url: Optional[str] = None,
+                 url_params: Optional[Dict[str, str]] = None,
+                 client: Optional[requests_http.Session] = None,
+                 retry_config: Optional[RetryConfig] = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
-        
+
         :param api_key_auth: The api_key_auth required for authentication
-        :type api_key_auth: Union[str,Callable[[], str]]
+        :type api_key_auth: Union[str, Callable[[], str]]
         :param server_idx: The index of the server to use for all operations
         :type server_idx: int
         :param server_url: The server URL to use for all operations
         :type server_url: str
         :param url_params: Parameters to optionally template the server URL with
         :type url_params: Dict[str, str]
         :param client: The requests.Session HTTP client to use for all operations
         :type client: requests_http.Session
         :param retry_config: The utils.RetryConfig to use globally
-        :type retry_config: utils.RetryConfig
+        :type retry_config: RetryConfig
         """
         if client is None:
             client = requests_http.Session()
-        
-        security = components.Security(api_key_auth = api_key_auth)
-        
+
+        if callable(api_key_auth):
+            def security():
+                return components.Security(api_key_auth = api_key_auth())
+        else:
+            security = components.Security(api_key_auth = api_key_auth)
+
         if server_url is not None:
             if url_params is not None:
                 server_url = utils.template_url(server_url, url_params)
+    
+
+        self.sdk_configuration = SDKConfiguration(
+            client,
+            security,
+            server_url,
+            server_idx,
+            retry_config=retry_config
+        )
+
+        hooks = SDKHooks()
+
+        current_server_url, *_ = self.sdk_configuration.get_server_details()
+        server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
+        if current_server_url != server_url:
+            self.sdk_configuration.server_url = server_url
+
+        # pylint: disable=protected-access
+        self.sdk_configuration.__dict__['_hooks'] = hooks
 
-        self.sdk_configuration = SDKConfiguration(client, security, server_url, server_idx, retry_config=retry_config)
-       
         self._init_sdks()
-    
+
+
     def _init_sdks(self):
         self.evaluations = Evaluations(self.sdk_configuration)
         self.logs = Logs(self.sdk_configuration)
-
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/sdkconfiguration.py` & `gantry_logger-0.0.2a7/src/gantry/sdkconfiguration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests
-from dataclasses import dataclass
-from typing import Dict, Tuple, Callable, Union
-from .utils.retries import RetryConfig
+
+import requests as requests_http
+from ._hooks import SDKHooks
 from .utils import utils
+from .utils.retries import RetryConfig
+from dataclasses import dataclass
 from gantry.models import components
+from typing import Callable, Dict, Optional, Tuple, Union
 
 
 SERVERS = [
     'https://app.gantry.io',
     # Gantry
 ]
 """Contains the list of servers available to the SDK"""
 
 @dataclass
 class SDKConfiguration:
-    client: requests.Session
+    client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
-    server_url: str = ''
-    server_idx: int = 0
+    server_url: Optional[str] = ''
+    server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '2.0.0'
-    sdk_version: str = '0.1.3'
-    gen_version: str = '2.231.0'
-    user_agent: str = 'speakeasy-sdk/python 0.1.3 2.231.0 2.0.0 gantry-logger'
-    retry_config: RetryConfig = None
+    sdk_version: str = '0.3.0'
+    gen_version: str = '2.326.3'
+    user_agent: str = 'speakeasy-sdk/python 0.3.0 2.326.3 2.0.0 gantry-logger'
+    retry_config: Optional[RetryConfig] = None
+
+    def __post_init__(self):
+        self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
-        if self.server_url:
+        if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
 
         return SERVERS[self.server_idx], {}
+
+
+    def get_hooks(self) -> SDKHooks:
+        return self._hooks
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/utils/retries.py` & `gantry_logger-0.0.2a7/src/gantry/utils/retries.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,20 +71,20 @@
                             raise TemporaryError(res)
                     else:
                         parsed_code = int(code)
 
                         if res.status_code == parsed_code:
                             raise TemporaryError(res)
             except requests.exceptions.ConnectionError as exception:
-                if not retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except requests.exceptions.Timeout as exception:
-                if not retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except TemporaryError:
                 raise
             except Exception as exception:
                 raise PermanentError(exception) from exception
@@ -110,11 +110,10 @@
             if now - start > max_elapsed_time:
                 if isinstance(exception, TemporaryError):
                     return exception.response
 
                 raise
             sleep = ((initial_interval/1000) *
                      exponent**retries + random.uniform(0, 1))
-            if sleep > max_interval/1000:
-                sleep = max_interval/1000
+            sleep = min(sleep, max_interval / 1000)
             time.sleep(sleep)
             retries += 1
```

### Comparing `gantry_logger-0.0.2a6/src/gantry/utils/utils.py` & `gantry_logger-0.0.2a7/src/gantry/utils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,507 +1,636 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import base64
 import json
 import re
 import sys
-from dataclasses import Field, dataclass, fields, is_dataclass, make_dataclass
+from dataclasses import Field, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from email.message import Message
 from enum import Enum
-from typing import (Any, Callable, Dict, List, Optional, Tuple, Union,
-                    get_args, get_origin)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    get_args,
+    get_origin,
+)
 from xmlrpc.client import boolean
 from typing_inspect import is_optional_type
 import dateutil.parser
-import requests
 from dataclasses_json import DataClassJsonMixin
 
 
-class SecurityClient:
-    client: requests.Session
+def get_security(security: Any) -> Tuple[Dict[str, str], Dict[str, str]]:
+    headers: Dict[str, str] = {}
     query_params: Dict[str, str] = {}
 
-    def __init__(self, client: requests.Session):
-        self.client = client
-
-    def request(self, method, url, **kwargs):
-        params = kwargs.get('params', {})
-        kwargs["params"] = {**self.query_params, **params}
-
-        return self.client.request(method, url, **kwargs)
-
-
-def configure_security_client(client: requests.Session, security: dataclass):
-    client = SecurityClient(client)
-
     if security is None:
-        return client
+        return headers, query_params
 
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
-        metadata = sec_field.metadata.get('security')
+        metadata = sec_field.metadata.get("security")
         if metadata is None:
             continue
-        if metadata.get('option'):
-            _parse_security_option(client, value)
-            return client
-        if metadata.get('scheme'):
+        if metadata.get("option"):
+            _parse_security_option(headers, query_params, value)
+            return headers, query_params
+        if metadata.get("scheme"):
             # Special case for basic auth which could be a flattened struct
             if metadata.get("sub_type") == "basic" and not is_dataclass(value):
-                _parse_security_scheme(client, metadata, security)
+                _parse_security_scheme(headers, query_params, metadata, security)
             else:
-                _parse_security_scheme(client, metadata, value)
+                _parse_security_scheme(headers, query_params, metadata, value)
 
-    return client
+    return headers, query_params
 
 
-def _parse_security_option(client: SecurityClient, option: dataclass):
+def _parse_security_option(
+    headers: Dict[str, str], query_params: Dict[str, str], option: Any
+):
     opt_fields: Tuple[Field, ...] = fields(option)
     for opt_field in opt_fields:
-        metadata = opt_field.metadata.get('security')
-        if metadata is None or metadata.get('scheme') is None:
+        metadata = opt_field.metadata.get("security")
+        if metadata is None or metadata.get("scheme") is None:
             continue
         _parse_security_scheme(
-            client, metadata, getattr(option, opt_field.name))
+            headers, query_params, metadata, getattr(option, opt_field.name)
+        )
 
 
-def _parse_security_scheme(client: SecurityClient, scheme_metadata: Dict, scheme: any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    scheme: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
     if is_dataclass(scheme):
-        if scheme_type == 'http' and sub_type == 'basic':
-            _parse_basic_auth_scheme(client, scheme)
+        if scheme_type == "http" and sub_type == "basic":
+            _parse_basic_auth_scheme(headers, scheme)
             return
 
         scheme_fields: Tuple[Field, ...] = fields(scheme)
         for scheme_field in scheme_fields:
-            metadata = scheme_field.metadata.get('security')
-            if metadata is None or metadata.get('field_name') is None:
+            metadata = scheme_field.metadata.get("security")
+            if metadata is None or metadata.get("field_name") is None:
                 continue
 
             value = getattr(scheme, scheme_field.name)
 
             _parse_security_scheme_value(
-                client, scheme_metadata, metadata, value)
+                headers, query_params, scheme_metadata, metadata, value
+            )
     else:
         _parse_security_scheme_value(
-            client, scheme_metadata, scheme_metadata, scheme)
+            headers, query_params, scheme_metadata, scheme_metadata, scheme
+        )
 
 
-def _parse_security_scheme_value(client: SecurityClient, scheme_metadata: Dict, security_metadata: Dict, value: any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme_value(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    security_metadata: Dict,
+    value: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
-    header_name = security_metadata.get('field_name')
+    header_name = str(security_metadata.get("field_name"))
 
     if scheme_type == "apiKey":
-        if sub_type == 'header':
-            client.client.headers[header_name] = value
-        elif sub_type == 'query':
-            client.query_params[header_name] = value
-        elif sub_type == 'cookie':
-            client.client.cookies[header_name] = value
+        if sub_type == "header":
+            headers[header_name] = value
+        elif sub_type == "query":
+            query_params[header_name] = value
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     elif scheme_type == "openIdConnect":
-        client.client.headers[header_name] = value
-    elif scheme_type == 'oauth2':
-        client.client.headers[header_name] = value
-    elif scheme_type == 'http':
-        if sub_type == 'bearer':
-            client.client.headers[header_name] = value.lower().startswith(
-                'bearer ') and value or f'Bearer {value}'
+        headers[header_name] = _apply_bearer(value)
+    elif scheme_type == "oauth2":
+        if sub_type != "client_credentials":
+            headers[header_name] = _apply_bearer(value)
+    elif scheme_type == "http":
+        if sub_type == "bearer":
+            headers[header_name] = _apply_bearer(value)
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     else:
-        raise Exception('not supported')
+        raise Exception("not supported")
+
+
+def _apply_bearer(token: str) -> str:
+    return token.lower().startswith("bearer ") and token or f"Bearer {token}"
 
 
-def _parse_basic_auth_scheme(client: SecurityClient, scheme: dataclass):
+def _parse_basic_auth_scheme(headers: Dict[str, str], scheme: Any):
     username = ""
     password = ""
 
     scheme_fields: Tuple[Field, ...] = fields(scheme)
     for scheme_field in scheme_fields:
-        metadata = scheme_field.metadata.get('security')
-        if metadata is None or metadata.get('field_name') is None:
+        metadata = scheme_field.metadata.get("security")
+        if metadata is None or metadata.get("field_name") is None:
             continue
 
-        field_name = metadata.get('field_name')
+        field_name = metadata.get("field_name")
         value = getattr(scheme, scheme_field.name)
 
-        if field_name == 'username':
+        if field_name == "username":
             username = value
-        if field_name == 'password':
+        if field_name == "password":
             password = value
 
-    data = f'{username}:{password}'.encode()
-    client.client.headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
+    data = f"{username}:{password}".encode()
+    headers["Authorization"] = f"Basic {base64.b64encode(data).decode()}"
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass,
-                 gbls: Dict[str, Dict[str, Dict[str, Any]]] = None) -> str:
-    path_param_fields: Tuple[Field, ...] = fields(clazz)
+def generate_url(
+    server_url: str,
+    path: str,
+    path_params: Any,
+    gbls: Optional[Any] = None,
+) -> str:
+    path_param_values: Dict[str, str] = {}
+
+    globals_already_populated = _populate_path_params(
+        path_params, gbls, path_param_values, []
+    )
+    if gbls is not None:
+        _populate_path_params(gbls, None, path_param_values, globals_already_populated)
+
+    for key, value in path_param_values.items():
+        path = path.replace("{" + key + "}", value, 1)
+
+    return remove_suffix(server_url, "/") + path
+
+
+def _populate_path_params(
+    path_params: Any,
+    gbls: Any,
+    path_param_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    path_param_fields: Tuple[Field, ...] = fields(path_params)
     for field in path_param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        param_metadata = field.metadata.get('path_param')
+        param_metadata = field.metadata.get("path_param")
         if param_metadata is None:
             continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+        param = getattr(path_params, field.name) if path_params is not None else None
+        param, global_found = _populate_from_globals(
+            field.name, param, "path_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
 
         if param is None:
             continue
 
         f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
+        serialization = param_metadata.get("serialization", "")
+        if serialization != "":
             serialized_params = _get_serialized_params(
-                param_metadata, field.type, f_name, param)
+                param_metadata, field.type, f_name, param
+            )
             for key, value in serialized_params.items():
-                path = path.replace(
-                    '{' + key + '}', value, 1)
+                path_param_values[key] = value
         else:
-            if param_metadata.get('style', 'simple') == 'simple':
+            if param_metadata.get("style", "simple") == "simple":
                 if isinstance(param, List):
                     pp_vals: List[str] = []
                     for pp_val in param:
                         if pp_val is None:
                             continue
                         pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif isinstance(param, Dict):
                     pp_vals: List[str] = []
                     for pp_key in param:
                         if param[pp_key] is None:
                             continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        if param_metadata.get("explode"):
+                            pp_vals.append(f"{pp_key}={_val_to_string(param[pp_key])}")
                         else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                            pp_vals.append(f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif not isinstance(param, (str, int, float, complex, bool, Decimal)):
                     pp_vals: List[str] = []
                     param_fields: Tuple[Field, ...] = fields(param)
                     for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
+                        param_value_metadata = param_field.metadata.get("path_param")
                         if not param_value_metadata:
                             continue
 
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
+                        param_name = param_value_metadata.get("field_name", field.name)
 
                         param_field_val = getattr(param, param_field.name)
                         if param_field_val is None:
                             continue
-                        if param_metadata.get('explode'):
+                        if param_metadata.get("explode"):
                             pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
+                                f"{param_name}={_val_to_string(param_field_val)}"
+                            )
                         else:
                             pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                                f"{param_name},{_val_to_string(param_field_val)}"
+                            )
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        _val_to_string(param)
+                    )
 
-    return remove_suffix(server_url, '/') + path
+    return globals_already_populated
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
 
 def template_url(url_with_params: str, params: Dict[str, str]) -> str:
     for key, value in params.items():
-        url_with_params = url_with_params.replace(
-            '{' + key + '}', value)
+        url_with_params = url_with_params.replace("{" + key + "}", value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: dataclass, gbls: Dict[str, Dict[str, Dict[str, Any]]] = None) -> Dict[
-        str, List[str]]:
+def get_query_params(
+    query_params: Any,
+    gbls: Optional[Any] = None,
+) -> Dict[str, List[str]]:
     params: Dict[str, List[str]] = {}
 
-    param_fields: Tuple[Field, ...] = fields(clazz)
+    globals_already_populated = _populate_query_params(query_params, gbls, params, [])
+    if gbls is not None:
+        _populate_query_params(gbls, None, params, globals_already_populated)
+
+    return params
+
+
+def _populate_query_params(
+    query_params: Any,
+    gbls: Any,
+    query_param_values: Dict[str, List[str]],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(query_params)
     for field in param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        metadata = field.metadata.get('query_param')
+        metadata = field.metadata.get("query_param")
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(
-            query_params, param_name) if query_params is not None else None
+        value = getattr(query_params, param_name) if query_params is not None else None
 
-        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
+        value, global_found = _populate_from_globals(
+            param_name, value, "query_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(param_name)
 
         f_name = metadata.get("field_name")
-        serialization = metadata.get('serialization', '')
-        if serialization != '':
-            serialized_parms = _get_serialized_params(metadata, field.type, f_name, value)
+        serialization = metadata.get("serialization", "")
+        if serialization != "":
+            serialized_parms = _get_serialized_params(
+                metadata, field.type, f_name, value
+            )
             for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
+                if key in query_param_values:
+                    query_param_values[key].extend(value)
                 else:
-                    params[key] = [value]
+                    query_param_values[key] = [value]
         else:
-            style = metadata.get('style', 'form')
-            if style == 'deepObject':
-                params = {**params, **_get_deep_object_query_params(
-                    metadata, f_name, value)}
-            elif style == 'form':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, ",")}
-            elif style == 'pipeDelimited':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, "|")}
+            style = metadata.get("style", "form")
+            if style == "deepObject":
+                _populate_deep_object_query_params(
+                    metadata, f_name, value, query_param_values
+                )
+            elif style == "form":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, ",", query_param_values
+                )
+            elif style == "pipeDelimited":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, "|", query_param_values
+                )
             else:
-                raise Exception('not yet implemented')
-    return params
+                raise Exception("not yet implemented")
 
+    return globals_already_populated
 
-def get_headers(headers_params: dataclass) -> Dict[str, str]:
-    if headers_params is None:
-        return {}
 
+def get_headers(headers_params: Any, gbls: Optional[Any] = None) -> Dict[str, str]:
     headers: Dict[str, str] = {}
 
-    param_fields: Tuple[Field, ...] = fields(headers_params)
-    for field in param_fields:
-        metadata = field.metadata.get('header')
-        if not metadata:
-            continue
+    globals_already_populated = []
+    if headers_params is not None:
+        globals_already_populated = _populate_headers(headers_params, gbls, headers, [])
+    if gbls is not None:
+        _populate_headers(gbls, None, headers, globals_already_populated)
 
-        value = _serialize_header(metadata.get(
-            'explode', False), getattr(headers_params, field.name))
+    return headers
 
-        if value != '':
-            headers[metadata.get('field_name', field.name)] = value
 
-    return headers
+def _populate_headers(
+    headers_params: Any,
+    gbls: Any,
+    header_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(headers_params)
+    for field in param_fields:
+        if field.name in skip_fields:
+            continue
 
+        metadata = field.metadata.get("header")
+        if not metadata:
+            continue
 
-def _get_serialized_params(metadata: Dict, field_type: type, field_name: str, obj: any) -> Dict[str, str]:
+        value, global_found = _populate_from_globals(
+            field.name, getattr(headers_params, field.name), "header", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
+        value = _serialize_header(metadata.get("explode", False), value)
+
+        if value != "":
+            header_values[metadata.get("field_name", field.name)] = value
+
+    return globals_already_populated
+
+
+def _get_serialized_params(
+    metadata: Dict, field_type: type, field_name: str, obj: Any
+) -> Dict[str, str]:
     params: Dict[str, str] = {}
 
-    serialization = metadata.get('serialization', '')
-    if serialization == 'json':
+    serialization = metadata.get("serialization", "")
+    if serialization == "json":
         params[metadata.get("field_name", field_name)] = marshal_json(obj, field_type)
 
     return params
 
 
-def _get_deep_object_query_params(metadata: Dict, field_name: str, obj: any) -> Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_deep_object_query_params(
+    metadata: Dict, field_name: str, obj: Any, params: Dict[str, List[str]]
+):
     if obj is None:
-        return params
+        return
 
     if is_dataclass(obj):
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('query_param')
+            obj_param_metadata = obj_field.metadata.get("query_param")
             if not obj_param_metadata:
                 continue
 
             obj_val = getattr(obj, obj_field.name)
             if obj_val is None:
                 continue
 
             if isinstance(obj_val, List):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                    if (
+                        params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        )
+                        is None
+                    ):
                         params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                        ]
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        ] = []
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                    ].append(_val_to_string(val))
             else:
                 params[
-                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                    _val_to_string(obj_val)]
+                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                ] = [_val_to_string(obj_val)]
     elif isinstance(obj, Dict):
         for key, value in obj.items():
             if value is None:
                 continue
 
             if isinstance(value, List):
                 for val in value:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{key}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                        ]
-
-                    params[
-                        f'{metadata.get("field_name", field_name)}[{key}]'].append(_val_to_string(val))
+                    if (
+                        params.get(f'{metadata.get("field_name", field_name)}[{key}]')
+                        is None
+                    ):
+                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = []
+
+                    params[f'{metadata.get("field_name", field_name)}[{key}]'].append(
+                        _val_to_string(val)
+                    )
             else:
                 params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                    _val_to_string(value)]
-    return params
+                    _val_to_string(value)
+                ]
 
 
 def _get_query_param_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('query_param')
+    obj_param_metadata = obj_field.metadata.get("query_param")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: Dict, field_name: str, obj: any, delimiter: str) -> Dict[
-        str, List[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
+def _populate_delimited_query_params(
+    metadata: Dict,
+    field_name: str,
+    obj: Any,
+    delimiter: str,
+    query_param_values: Dict[str, List[str]],
+):
+    _populate_form(
+        field_name,
+        metadata.get("explode", True),
+        obj,
+        _get_query_param_field_name,
+        delimiter,
+        query_param_values,
+    )
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
-    'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    "json": "application/json",
+    "form": "application/x-www-form-urlencoded",
+    "multipart": "multipart/form-data",
+    "raw": "application/octet-stream",
+    "string": "text/plain",
 }
 
 
-def serialize_request_body(request: dataclass, request_type: type, request_field_name: str, nullable: bool, optional: bool, serialization_method: str, encoder=None) -> Tuple[
-        str, any, any]:
+def serialize_request_body(
+    request: Any,
+    request_type: type,
+    request_field_name: str,
+    nullable: bool,
+    optional: bool,
+    serialization_method: str,
+    encoder=None,
+) -> Tuple[Optional[str], Optional[Any], Optional[Any]]:
     if request is None:
         if not nullable and optional:
             return None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, request_type, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request, encoder)
+        return serialize_content_type(
+            request_field_name,
+            request_type,
+            SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+            request,
+            encoder,
+        )
 
     request_val = getattr(request, request_field_name)
 
     if request_val is None:
         if not nullable and optional:
             return None, None, None
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
-            request_metadata = field.metadata.get('request')
+            request_metadata = field.metadata.get("request")
             break
 
     if request_metadata is None:
-        raise Exception('invalid request type')
+        raise Exception("invalid request type")
 
-    return serialize_content_type(request_field_name, request_type, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(
+        request_field_name,
+        request_type,
+        request_metadata.get("media_type", "application/octet-stream"),
+        request_val,
+    )
 
 
-def serialize_content_type(field_name: str, request_type: any, media_type: str, request: dataclass, encoder=None) -> Tuple[str, any, List[List[any]]]:
-    if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
+def serialize_content_type(
+    field_name: str, request_type: Any, media_type: str, request: Any, encoder=None
+) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
+    if re.match(r"(application|text)\/.*?\+*json.*", media_type) is not None:
         return media_type, marshal_json(request, request_type, encoder), None
-    if re.match(r'multipart\/.*', media_type) is not None:
+    if re.match(r"multipart\/.*", media_type) is not None:
         return serialize_multipart_form(media_type, request)
-    if re.match(r'application\/x-www-form-urlencoded.*', media_type) is not None:
+    if re.match(r"application\/x-www-form-urlencoded.*", media_type) is not None:
         return media_type, serialize_form_data(field_name, request), None
     if isinstance(request, (bytes, bytearray)):
         return media_type, request, None
     if isinstance(request, str):
         return media_type, request, None
 
     raise Exception(
-        f"invalid request body type {type(request)} for mediaType {media_type}")
+        f"invalid request body type {type(request)} for mediaType {media_type}"
+    )
 
 
-def serialize_multipart_form(media_type: str, request: dataclass) -> Tuple[str, any, List[List[any]]]:
-    form: List[List[any]] = []
+def serialize_multipart_form(
+    media_type: str, request: Any
+) -> Tuple[str, Any, List[List[Any]]]:
+    form: List[List[Any]] = []
     request_fields = fields(request)
 
     for field in request_fields:
         val = getattr(request, field.name)
         if val is None:
             continue
 
-        field_metadata = field.metadata.get('multipart_form')
+        field_metadata = field.metadata.get("multipart_form")
         if not field_metadata:
             continue
 
         if field_metadata.get("file") is True:
             file_fields = fields(val)
 
             file_name = ""
             field_name = ""
             content = bytes()
 
             for file_field in file_fields:
-                file_metadata = file_field.metadata.get('multipart_form')
+                file_metadata = file_field.metadata.get("multipart_form")
                 if file_metadata is None:
                     continue
 
                 if file_metadata.get("content") is True:
                     content = getattr(val, file_field.name)
                 else:
-                    field_name = file_metadata.get(
-                        "field_name", file_field.name)
+                    field_name = file_metadata.get("field_name", file_field.name)
                     file_name = getattr(val, file_field.name)
             if field_name == "" or file_name == "" or content == bytes():
-                raise Exception('invalid multipart/form-data file')
+                raise Exception("invalid multipart/form-data file")
 
             form.append([field_name, [file_name, content]])
         elif field_metadata.get("json") is True:
-            to_append = [field_metadata.get("field_name", field.name), [
-                None, marshal_json(val, field.type), "application/json"]]
+            to_append = [
+                field_metadata.get("field_name", field.name),
+                [None, marshal_json(val, field.type), "application/json"],
+            ]
             form.append(to_append)
         else:
-            field_name = field_metadata.get(
-                "field_name", field.name)
+            field_name = field_metadata.get("field_name", field.name)
             if isinstance(val, List):
                 for value in val:
                     if value is None:
                         continue
-                    form.append(
-                        [field_name + "[]", [None, _val_to_string(value)]])
+                    form.append([field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
-def serialize_dict(original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]) -> Dict[
-        str, List[str]]:
+def serialize_dict(
+    original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]
+) -> Dict[str, List[str]]:
     if existing is None:
-        existing = []
+        existing = {}
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
             existing[key].append(val)
     else:
@@ -511,225 +640,239 @@
             temp.append(str(val))
         if field_name not in existing:
             existing[field_name] = []
         existing[field_name].append(",".join(temp))
     return existing
 
 
-def serialize_form_data(field_name: str, data: dataclass) -> Dict[str, any]:
+def serialize_form_data(field_name: str, data: Any) -> Dict[str, Any]:
     form: Dict[str, List[str]] = {}
 
     if is_dataclass(data):
         for field in fields(data):
             val = getattr(data, field.name)
             if val is None:
                 continue
 
-            metadata = field.metadata.get('form')
+            metadata = field.metadata.get("form")
             if metadata is None:
                 continue
 
-            field_name = metadata.get('field_name', field.name)
+            field_name = metadata.get("field_name", field.name)
 
-            if metadata.get('json'):
+            if metadata.get("json"):
                 form[field_name] = [marshal_json(val, field.type)]
             else:
-                if metadata.get('style', 'form') == 'form':
-                    form = {**form, **_populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")}
+                if metadata.get("style", "form") == "form":
+                    _populate_form(
+                        field_name,
+                        metadata.get("explode", True),
+                        val,
+                        _get_form_field_name,
+                        ",",
+                        form,
+                    )
                 else:
-                    raise Exception(
-                        f'Invalid form style for field {field.name}')
+                    raise Exception(f"Invalid form style for field {field.name}")
     elif isinstance(data, Dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
-        raise Exception(f'Invalid request body type for field {field_name}')
+        raise Exception(f"Invalid request body type for field {field_name}")
 
     return form
 
 
 def _get_form_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('form')
+    obj_param_metadata = obj_field.metadata.get("form")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, delimiter: str) -> \
-        Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_form(
+    field_name: str,
+    explode: boolean,
+    obj: Any,
+    get_field_name_func: Callable,
+    delimiter: str,
+    form: Dict[str, List[str]],
+):
     if obj is None:
-        return params
+        return form
 
     if is_dataclass(obj):
         items = []
 
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
             obj_field_name = get_field_name_func(obj_field)
-            if obj_field_name == '':
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                params[obj_field_name] = [_val_to_string(val)]
+                form[obj_field_name] = [_val_to_string(val)]
             else:
-                items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                items.append(f"{obj_field_name}{delimiter}{_val_to_string(val)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, Dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                params[key] = _val_to_string(value)
+                form[key] = [_val_to_string(value)]
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f"{key}{delimiter}{_val_to_string(value)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             if explode:
-                if not field_name in params:
-                    params[field_name] = []
-                params[field_name].append(_val_to_string(value))
+                if not field_name in form:
+                    form[field_name] = []
+                form[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(
-                [str(item) for item in items])]
+            form[field_name] = [delimiter.join([str(item) for item in items])]
     else:
-        params[field_name] = [_val_to_string(obj)]
+        form[field_name] = [_val_to_string(obj)]
 
-    return params
+    return form
 
 
-def _serialize_header(explode: bool, obj: any) -> str:
+def _serialize_header(explode: bool, obj: Any) -> str:
     if obj is None:
-        return ''
+        return ""
 
     if is_dataclass(obj):
         items = []
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('header')
+            obj_param_metadata = obj_field.metadata.get("header")
 
             if not obj_param_metadata:
                 continue
 
-            obj_field_name = obj_param_metadata.get(
-                'field_name', obj_field.name)
-            if obj_field_name == '':
+            obj_field_name = obj_param_metadata.get("field_name", obj_field.name)
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                items.append(
-                    f'{obj_field_name}={_val_to_string(val)}')
+                items.append(f"{obj_field_name}={_val_to_string(val)}")
             else:
                 items.append(obj_field_name)
                 items.append(_val_to_string(val))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     elif isinstance(obj, Dict):
         items = []
 
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                items.append(f'{key}={_val_to_string(value)}')
+                items.append(f"{key}={_val_to_string(value)}")
             else:
                 items.append(key)
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join([str(item) for item in items])
+            return ",".join([str(item) for item in items])
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     else:
-        return f'{_val_to_string(obj)}'
+        return f"{_val_to_string(obj)}"
 
-    return ''
+    return ""
 
 
 def unmarshal_json(data, typ, decoder=None):
-    unmarshal = make_dataclass('Unmarshal', [('res', typ)],
-                               bases=(DataClassJsonMixin,))
+    unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
         out = unmarshal.from_dict({"res": json_dict})
     except AttributeError as attr_err:
         raise AttributeError(
-            f'unable to unmarshal {data} as {typ}') from attr_err
+            f"unable to unmarshal {data} as {typ} - {attr_err}"
+        ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
 
 
 def marshal_json(val, typ, encoder=None):
     if not is_optional_type(typ) and val is None:
         raise ValueError(f"Could not marshal None into non-optional type: {typ}")
 
-    marshal = make_dataclass('Marshal', [('res', typ)],
-                             bases=(DataClassJsonMixin,))
+    marshal = make_dataclass("Marshal", [("res", typ)], bases=(DataClassJsonMixin,))
     marshaller = marshal(res=val)
     json_dict = marshaller.to_dict()
     val = json_dict["res"] if encoder is None else encoder(json_dict["res"])
 
-    return json.dumps(val, separators=(',', ':'), sort_keys=True)
+    return json.dumps(val, separators=(",", ":"), sort_keys=True)
 
 
 def match_content_type(content_type: str, pattern: str) -> boolean:
     if pattern in (content_type, "*", "*/*"):
         return True
 
     msg = Message()
-    msg['content-type'] = content_type
+    msg["content-type"] = content_type
     media_type = msg.get_content_type()
 
     if media_type == pattern:
         return True
 
     parts = media_type.split("/")
     if len(parts) == 2:
-        if pattern in (f'{parts[0]}/*', f'*/{parts[1]}'):
+        if pattern in (f"{parts[0]}/*", f"*/{parts[1]}"):
+            return True
+
+    return False
+
+
+def match_status_codes(status_codes: List[str], status_code: int) -> bool:
+    for code in status_codes:
+        if code == str(status_code):
             return True
 
+        if code.endswith("XX") and code.startswith(str(status_code)[:1]):
+            return True
     return False
 
 
 def datetimeisoformat(optional: bool):
     def isoformatoptional(val):
         if optional and val is None:
             return None
@@ -761,14 +904,41 @@
 
 
 def bigintdecoder(val):
     if isinstance(val, float):
         raise ValueError(f"{val} is a float")
     return int(val)
 
+def integerstrencoder(optional: bool):
+    def integerstrencode(val: int):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return integerstrencode
+
+
+def integerstrdecoder(val):
+    if isinstance(val, float):
+        raise ValueError(f"{val} is a float")
+    return int(val)
+
+
+def numberstrencoder(optional: bool):
+    def numberstrencode(val: float):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return numberstrencode
+
+
+def numberstrdecoder(val):
+    return float(val)
+
 
 def decimalencoder(optional: bool, as_str: bool):
     def decimalencode(val: Decimal):
         if optional and val is None:
             return None
 
         if as_str:
@@ -828,67 +998,90 @@
         for value in val:
             decoded.append(value_decoder(value))
 
         return decoded
 
     return list_decode
 
+
 def union_encoder(all_encoders: Dict[str, Callable]):
-    def selective_encoder(val: any):
+    def selective_encoder(val: Any):
         if type(val) in all_encoders:
             return all_encoders[type(val)](val)
         return val
+
     return selective_encoder
 
+
 def union_decoder(all_decoders: List[Callable]):
-    def selective_decoder(val: any):
+    def selective_decoder(val: Any):
         decoded = val
         for decoder in all_decoders:
             try:
                 decoded = decoder(val)
                 break
             except (TypeError, ValueError):
                 continue
         return decoded
+
     return selective_decoder
 
+
 def get_field_name(name):
     def override(_, _field_name=name):
         return _field_name
 
     return override
 
 
-def _val_to_string(val):
+def _val_to_string(val) -> str:
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
-        return val.isoformat().replace('+00:00', 'Z')
+        return str(val.isoformat().replace("+00:00", "Z"))
     if isinstance(val, Enum):
         return str(val.value)
 
     return str(val)
 
 
-def _populate_from_globals(param_name: str, value: any, param_type: str, gbls: Dict[str, Dict[str, Dict[str, Any]]]):
-    if value is None and gbls is not None:
-        if 'parameters' in gbls:
-            if param_type in gbls['parameters']:
-                if param_name in gbls['parameters'][param_type]:
-                    global_value = gbls['parameters'][param_type][param_name]
-                    if global_value is not None:
-                        value = global_value
+def _populate_from_globals(
+    param_name: str, value: Any, param_type: str, gbls: Any
+) -> Tuple[Any, bool]:
+    if gbls is None:
+        return value, False
+
+    global_fields = fields(gbls)
+
+    found = False
+    for field in global_fields:
+        if field.name is not param_name:
+            continue
+
+        found = True
 
-    return value
+        if value is not None:
+            return value, True
+
+        global_value = getattr(gbls, field.name)
+
+        param_metadata = field.metadata.get(param_type)
+        if param_metadata is None:
+            return value, True
+
+        return global_value, True
+
+    return value, found
 
 
 def decoder_with_discriminator(field_name):
     def decode_fx(obj):
-        kls = getattr(sys.modules['sdk.models.components'], obj[field_name])
+        kls = getattr(sys.modules["sdk.models.components"], obj[field_name])
         return unmarshal_json(json.dumps(obj), kls)
+
     return decode_fx
 
 
 def remove_suffix(input_string, suffix):
     if suffix and input_string.endswith(suffix):
-        return input_string[:-len(suffix)]
+        return input_string[: -len(suffix)]
     return input_string
```

### Comparing `gantry_logger-0.0.2a6/src/gantry_logger.egg-info/PKG-INFO` & `gantry_logger-0.0.2a7/src/gantry_logger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry-logger
-Version: 0.0.2a6
+Version: 0.0.2a7
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `gantry_logger-0.0.2a6/src/gantry_logger.egg-info/SOURCES.txt` & `gantry_logger-0.0.2a7/src/gantry_logger.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 setup.cfg
 setup.py
 src/gantry/__init__.py
 src/gantry/evaluations.py
 src/gantry/logs.py
 src/gantry/sdk.py
 src/gantry/sdkconfiguration.py
+src/gantry/_hooks/__init__.py
+src/gantry/_hooks/sdkhooks.py
+src/gantry/_hooks/types.py
 src/gantry/logger/__init__.py
 src/gantry/logger/consumer.py
 src/gantry/logger/eval_logger.py
 src/gantry/logger/eval_reports.py
 src/gantry/logger/langchain_callback.py
 src/gantry/logger/log_location.py
 src/gantry/logger/utils.py
@@ -34,14 +37,16 @@
 src/gantry/models/components/functionstep.py
 src/gantry/models/components/getlogssummaryrequest.py
 src/gantry/models/components/getragevaluationresultsresponse.py
 src/gantry/models/components/getragevaluationresultsresponseresponse.py
 src/gantry/models/components/llmevaluationcriteriatype.py
 src/gantry/models/components/llmevaluationerrortype.py
 src/gantry/models/components/llmstep.py
+src/gantry/models/components/logerrorrequest.py
+src/gantry/models/components/logerrorresponseresponse.py
 src/gantry/models/components/logragrecordrequest.py
 src/gantry/models/components/logragrecordresponse.py
 src/gantry/models/components/logragrecordresponseresponse.py
 src/gantry/models/components/message.py
 src/gantry/models/components/organizationtier.py
 src/gantry/models/components/orguser.py
 src/gantry/models/components/passfailunsurerubricscalevalues.py
@@ -49,21 +54,25 @@
 src/gantry/models/components/ragevaluationresult.py
 src/gantry/models/components/ragrecord.py
 src/gantry/models/components/recordstatuscount.py
 src/gantry/models/components/retrievalstep.py
 src/gantry/models/components/security.py
 src/gantry/models/components/stepformat.py
 src/gantry/models/components/summarynotesresponse.py
+src/gantry/models/components/topic.py
 src/gantry/models/components/topicstats.py
+src/gantry/models/components/unsupportedquestion.py
+src/gantry/models/components/unsupportedquestiontype.py
 src/gantry/models/errors/__init__.py
 src/gantry/models/errors/sdkerror.py
 src/gantry/models/operations/__init__.py
 src/gantry/models/operations/create_evaluation_run_pre_upload.py
 src/gantry/models/operations/create_rag_evaluation_run.py
 src/gantry/models/operations/get_rag_evaluation_results.py
+src/gantry/models/operations/log_error.py
 src/gantry/models/operations/log_rag_records.py
 src/gantry/utils/__init__.py
 src/gantry/utils/retries.py
 src/gantry/utils/utils.py
 src/gantry_logger.egg-info/PKG-INFO
 src/gantry_logger.egg-info/SOURCES.txt
 src/gantry_logger.egg-info/dependency_links.txt
```

