# Comparing `tmp/python_spartan-0.2.5.tar.gz` & `tmp/python_spartan-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_spartan-0.2.5.tar", max compression
+gzip compressed data, was "python_spartan-0.2.6.tar", max compression
```

## Comparing `python_spartan-0.2.5.tar` & `python_spartan-0.2.6.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0      349 2023-12-15 09:36:48.322632 python_spartan-0.2.5/README.md
--rw-r--r--   0        0        0     1007 2023-12-20 01:44:07.442473 python_spartan-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-15 09:36:48.323633 python_spartan-0.2.5/python_spartan/__init__.py
--rw-r--r--   0        0        0    13891 2023-12-15 10:02:13.967365 python_spartan-0.2.5/python_spartan/main.py
--rw-r--r--   0        0        0        0 2023-12-15 09:36:48.323867 python_spartan-0.2.5/python_spartan/services/__init__.py
--rw-r--r--   0        0        0     3745 2023-12-15 10:02:13.967531 python_spartan-0.2.5/python_spartan/services/application.py
--rw-r--r--   0        0        0      705 2023-12-15 10:02:13.967682 python_spartan-0.2.5/python_spartan/services/deployment.py
--rw-r--r--   0        0        0     4734 2023-12-15 10:02:13.967812 python_spartan-0.2.5/python_spartan/services/handler.py
--rw-r--r--   0        0        0     3971 2023-12-15 10:02:13.967935 python_spartan-0.2.5/python_spartan/services/infrastructure.py
--rw-r--r--   0        0        0     3010 2023-12-15 10:02:13.968052 python_spartan-0.2.5/python_spartan/services/inspire.py
--rw-r--r--   0        0        0     2475 2023-12-15 10:02:13.968170 python_spartan-0.2.5/python_spartan/services/migrate.py
--rw-r--r--   0        0        0     2863 2023-12-15 10:02:13.968289 python_spartan-0.2.5/python_spartan/services/model.py
--rw-r--r--   0        0        0     2869 2023-12-15 10:02:13.968357 python_spartan-0.2.5/python_spartan/services/parser.py
--rw-r--r--   0        0        0     2875 2023-12-15 10:02:13.968418 python_spartan-0.2.5/python_spartan/services/plotter.py
--rw-r--r--   0        0        0     2875 2023-12-15 10:02:13.968543 python_spartan-0.2.5/python_spartan/services/request.py
--rw-r--r--   0        0        0     3052 2023-12-15 10:02:13.968659 python_spartan-0.2.5/python_spartan/services/response.py
--rw-r--r--   0        0        0     3045 2023-12-19 22:17:53.325956 python_spartan-0.2.5/python_spartan/services/route.py
--rw-r--r--   0        0        0     3187 2023-12-15 10:02:13.968809 python_spartan-0.2.5/python_spartan/services/service.py
--rw-r--r--   0        0        0      736 2023-12-15 10:02:13.968914 python_spartan-0.2.5/python_spartan/services/test.py
--rw-r--r--   0        0        0      364 2023-12-15 09:36:48.325067 python_spartan-0.2.5/python_spartan/stubs/handler/alexa_skill_kit_subscribe.stub
--rw-r--r--   0        0        0      206 2023-12-15 09:36:48.325146 python_spartan-0.2.5/python_spartan/stubs/handler/amazon_appsync_subsribe.stub
--rw-r--r--   0        0        0      251 2023-12-15 09:36:48.325220 python_spartan-0.2.5/python_spartan/stubs/handler/amazon_kinesis_subscribe.stub
--rw-r--r--   0        0        0      484 2023-12-15 09:36:48.325295 python_spartan-0.2.5/python_spartan/stubs/handler/amazon_lex_subscribe.stub
--rw-r--r--   0        0        0      233 2023-12-15 09:36:48.325368 python_spartan-0.2.5/python_spartan/stubs/handler/amazon_mq_subscribe.stub
--rw-r--r--   0        0        0      271 2023-12-15 09:36:48.325437 python_spartan-0.2.5/python_spartan/stubs/handler/amazon_msk_subscribe.stub
--rw-r--r--   0        0        0      261 2023-12-15 09:36:48.325502 python_spartan-0.2.5/python_spartan/stubs/handler/amazon_redshift_subscribe.stub
--rw-r--r--   0        0        0      229 2023-12-15 09:36:48.325581 python_spartan-0.2.5/python_spartan/stubs/handler/amazon_timestream_subscribe.stub
--rw-r--r--   0        0        0      133 2023-12-15 09:36:48.325662 python_spartan-0.2.5/python_spartan/stubs/handler/api_subscribe.stub
--rw-r--r--   0        0        0      334 2023-12-15 09:36:48.325747 python_spartan-0.2.5/python_spartan/stubs/handler/aws_codecommit_subscribe.stub
--rw-r--r--   0        0        0      341 2023-12-15 09:36:48.325854 python_spartan-0.2.5/python_spartan/stubs/handler/aws_config_subscribe.stub
--rw-r--r--   0        0        0      205 2023-12-15 09:36:48.325936 python_spartan-0.2.5/python_spartan/stubs/handler/aws_iot_button_subscribe.stub
--rw-r--r--   0        0        0      230 2023-12-15 09:36:48.326071 python_spartan-0.2.5/python_spartan/stubs/handler/aws_iot_core_subscribe.stub
--rw-r--r--   0        0        0      226 2023-12-15 09:36:48.326159 python_spartan-0.2.5/python_spartan/stubs/handler/aws_secrets_manager_rotation_subscribe.stub
--rw-r--r--   0        0        0      187 2023-12-15 09:36:48.326227 python_spartan-0.2.5/python_spartan/stubs/handler/aws_step_function_subscribe.stub
--rw-r--r--   0        0        0      271 2023-12-15 09:36:48.326290 python_spartan-0.2.5/python_spartan/stubs/handler/cloudtrail_subscribe.stub
--rw-r--r--   0        0        0      108 2023-12-15 09:36:48.326377 python_spartan-0.2.5/python_spartan/stubs/handler/cloudwatch_logs_subscribe.stub
--rw-r--r--   0        0        0      247 2023-12-15 09:36:48.326464 python_spartan-0.2.5/python_spartan/stubs/handler/cognito_subscribe.stub
--rw-r--r--   0        0        0      108 2023-12-15 09:36:48.326533 python_spartan-0.2.5/python_spartan/stubs/handler/default.stub
--rw-r--r--   0        0        0      339 2023-12-15 09:36:48.326605 python_spartan-0.2.5/python_spartan/stubs/handler/elastic_load_balancer_subscribe.stub
--rw-r--r--   0        0        0      409 2023-12-15 09:36:48.326682 python_spartan-0.2.5/python_spartan/stubs/handler/lambda_ws.stub
--rw-r--r--   0        0        0      186 2023-12-15 09:36:48.326783 python_spartan-0.2.5/python_spartan/stubs/handler/mqtt_over_ws_subscribe.stub
--rw-r--r--   0        0        0      273 2023-12-15 09:36:48.326856 python_spartan-0.2.5/python_spartan/stubs/handler/s3_subscribe.stub
--rw-r--r--   0        0        0      224 2023-12-15 09:36:48.326928 python_spartan-0.2.5/python_spartan/stubs/handler/ses_subscribe.stub
--rw-r--r--   0        0        0      202 2023-12-15 09:36:48.327009 python_spartan-0.2.5/python_spartan/stubs/handler/sns_subscribe.stub
--rw-r--r--   0        0        0     1075 2023-12-15 09:36:48.327105 python_spartan-0.2.5/python_spartan/stubs/handler/sqs_both.stub
--rw-r--r--   0        0        0      122 2023-12-15 09:36:48.327208 python_spartan-0.2.5/python_spartan/stubs/handler/sqs_listen.stub
--rw-r--r--   0        0        0      275 2023-12-15 09:36:48.327290 python_spartan-0.2.5/python_spartan/stubs/handler/sqs_publish.stub
--rw-r--r--   0        0        0      942 2023-12-15 09:36:48.327366 python_spartan-0.2.5/python_spartan/stubs/handler/sqs_subscribe.stub
--rw-r--r--   0        0        0      111 2023-12-15 09:36:48.327437 python_spartan-0.2.5/python_spartan/stubs/handler/sqs_trigger.stub
--rw-r--r--   0        0        0      179 2023-12-15 09:36:48.327686 python_spartan-0.2.5/python_spartan/stubs/infrastructure/fifo_dlq.stub
--rw-r--r--   0        0        0      178 2023-12-15 09:36:48.327751 python_spartan-0.2.5/python_spartan/stubs/infrastructure/fifo_sqs.stub
--rw-r--r--   0        0        0      334 2023-12-15 09:36:48.327832 python_spartan-0.2.5/python_spartan/stubs/infrastructure/fifo_with_dlq.stub
--rw-r--r--   0        0        0       70 2023-12-15 09:36:48.327921 python_spartan-0.2.5/python_spartan/stubs/infrastructure/iamrole_lambda.stub
--rw-r--r--   0        0        0      189 2023-12-15 09:36:48.328001 python_spartan-0.2.5/python_spartan/stubs/infrastructure/iamrole_sqs.stub
--rw-r--r--   0        0        0      219 2023-12-15 09:36:48.328094 python_spartan-0.2.5/python_spartan/stubs/infrastructure/lambda_triggered_by_http.stub
--rw-r--r--   0        0        0      147 2023-12-15 09:36:48.328179 python_spartan-0.2.5/python_spartan/stubs/infrastructure/lambda_triggered_by_sns.stub
--rw-r--r--   0        0        0      147 2023-12-15 09:36:48.328249 python_spartan-0.2.5/python_spartan/stubs/infrastructure/lambda_triggered_by_sqs.stub
--rw-r--r--   0        0        0      147 2023-12-15 09:36:48.328310 python_spartan-0.2.5/python_spartan/stubs/infrastructure/lambda_triggered_by_ws.stub
--rw-r--r--   0        0        0     1461 2023-12-15 10:02:13.969047 python_spartan-0.2.5/python_spartan/stubs/infrastructure/serverless.stub
--rw-r--r--   0        0        0      124 2023-12-15 09:36:48.328459 python_spartan-0.2.5/python_spartan/stubs/infrastructure/standard_dlq.stub
--rw-r--r--   0        0        0      123 2023-12-15 09:36:48.328519 python_spartan-0.2.5/python_spartan/stubs/infrastructure/standard_sqs.stub
--rw-r--r--   0        0        0      279 2023-12-15 09:36:48.328582 python_spartan-0.2.5/python_spartan/stubs/infrastructure/standard_with_dlq.stub
--rw-r--r--   0        0        0      537 2023-12-15 09:36:48.328652 python_spartan-0.2.5/python_spartan/stubs/infrastructure/ws.stub
--rw-r--r--   0        0        0     3298 2023-12-15 09:36:48.328779 python_spartan-0.2.5/python_spartan/stubs/migration/mssql_alembic.stub
--rw-r--r--   0        0        0     3278 2023-12-15 09:36:48.328895 python_spartan-0.2.5/python_spartan/stubs/migration/mysql_alembic.stub
--rw-r--r--   0        0        0     3282 2023-12-15 09:36:48.328973 python_spartan-0.2.5/python_spartan/stubs/migration/psql_alembic.stub
--rw-r--r--   0        0        0     3363 2023-12-15 09:36:48.329054 python_spartan-0.2.5/python_spartan/stubs/migration/sqlite_alembic.stub
--rw-r--r--   0        0        0      624 2023-12-15 10:02:13.969180 python_spartan-0.2.5/python_spartan/stubs/model/default.stub
--rw-r--r--   0        0        0      615 2023-12-15 10:02:13.969292 python_spartan-0.2.5/python_spartan/stubs/parser/default.stub
--rw-r--r--   0        0        0     2471 2023-12-15 10:02:13.969406 python_spartan-0.2.5/python_spartan/stubs/plotter/default.stub
--rw-r--r--   0        0        0     1711 2023-12-15 10:02:13.969520 python_spartan-0.2.5/python_spartan/stubs/request/default.stub
--rw-r--r--   0        0        0     2343 2023-12-15 10:02:13.969643 python_spartan-0.2.5/python_spartan/stubs/response/default.stub
--rw-r--r--   0        0        0     8860 2023-12-19 22:26:20.121918 python_spartan-0.2.5/python_spartan/stubs/route/default.stub
--rw-r--r--   0        0        0    13651 2023-12-19 22:39:02.726813 python_spartan-0.2.5/python_spartan/stubs/service/default.stub
--rw-r--r--   0        0        0     1471 2023-12-15 09:36:48.329744 python_spartan-0.2.5/python_spartan/stubs/service/elastic_search.stub
--rw-r--r--   0        0        0     1003 2023-12-15 09:36:48.329813 python_spartan-0.2.5/python_spartan/stubs/service/email.stub
--rw-r--r--   0        0        0      833 2023-12-15 09:36:48.329877 python_spartan-0.2.5/python_spartan/stubs/service/queue.stub
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 python_spartan-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      349 2023-12-15 09:36:48.322632 python_spartan-0.2.6/README.md
+-rw-r--r--   0        0        0     1026 2024-05-11 05:32:08.737606 python_spartan-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-15 09:36:48.323633 python_spartan-0.2.6/python_spartan/__init__.py
+-rw-r--r--   0        0        0    13834 2024-05-11 05:28:06.392053 python_spartan-0.2.6/python_spartan/main.py
+-rw-r--r--   0        0        0        0 2023-12-15 09:36:48.323867 python_spartan-0.2.6/python_spartan/services/__init__.py
+-rw-r--r--   0        0        0     3817 2024-05-11 05:01:38.116827 python_spartan-0.2.6/python_spartan/services/application.py
+-rw-r--r--   0        0        0      706 2023-12-28 08:30:29.954066 python_spartan-0.2.6/python_spartan/services/deployment.py
+-rw-r--r--   0        0        0     4735 2024-01-12 08:40:04.024573 python_spartan-0.2.6/python_spartan/services/handler.py
+-rw-r--r--   0        0        0     3301 2024-01-12 08:54:06.655173 python_spartan-0.2.6/python_spartan/services/infrastructure.py
+-rw-r--r--   0        0        0     3010 2024-01-12 08:42:45.991604 python_spartan-0.2.6/python_spartan/services/inspire.py
+-rw-r--r--   0        0        0     2135 2024-01-26 22:38:24.808491 python_spartan-0.2.6/python_spartan/services/migrate.py
+-rw-r--r--   0        0        0     2863 2023-12-28 08:30:29.954829 python_spartan-0.2.6/python_spartan/services/model.py
+-rw-r--r--   0        0        0     2869 2023-12-28 08:30:29.954897 python_spartan-0.2.6/python_spartan/services/parser.py
+-rw-r--r--   0        0        0     2794 2024-01-12 08:52:53.433982 python_spartan-0.2.6/python_spartan/services/plotter.py
+-rw-r--r--   0        0        0     2794 2024-01-12 08:26:24.708132 python_spartan-0.2.6/python_spartan/services/request.py
+-rw-r--r--   0        0        0     3109 2024-01-12 07:44:06.917540 python_spartan-0.2.6/python_spartan/services/response.py
+-rw-r--r--   0        0        0     3134 2024-01-12 08:54:06.659673 python_spartan-0.2.6/python_spartan/services/route.py
+-rw-r--r--   0        0        0     3289 2024-05-11 04:50:23.016686 python_spartan-0.2.6/python_spartan/services/service.py
+-rw-r--r--   0        0        0      737 2024-01-12 09:44:01.656607 python_spartan-0.2.6/python_spartan/services/test.py
+-rw-r--r--   0        0        0      364 2023-12-15 09:36:48.325067 python_spartan-0.2.6/python_spartan/stubs/handler/alexa_skill_kit_subscribe.stub
+-rw-r--r--   0        0        0      206 2023-12-15 09:36:48.325146 python_spartan-0.2.6/python_spartan/stubs/handler/amazon_appsync_subsribe.stub
+-rw-r--r--   0        0        0      251 2023-12-15 09:36:48.325220 python_spartan-0.2.6/python_spartan/stubs/handler/amazon_kinesis_subscribe.stub
+-rw-r--r--   0        0        0      484 2023-12-15 09:36:48.325295 python_spartan-0.2.6/python_spartan/stubs/handler/amazon_lex_subscribe.stub
+-rw-r--r--   0        0        0      233 2023-12-15 09:36:48.325368 python_spartan-0.2.6/python_spartan/stubs/handler/amazon_mq_subscribe.stub
+-rw-r--r--   0        0        0      271 2023-12-15 09:36:48.325437 python_spartan-0.2.6/python_spartan/stubs/handler/amazon_msk_subscribe.stub
+-rw-r--r--   0        0        0      261 2023-12-15 09:36:48.325502 python_spartan-0.2.6/python_spartan/stubs/handler/amazon_redshift_subscribe.stub
+-rw-r--r--   0        0        0      229 2023-12-15 09:36:48.325581 python_spartan-0.2.6/python_spartan/stubs/handler/amazon_timestream_subscribe.stub
+-rw-r--r--   0        0        0      133 2023-12-15 09:36:48.325662 python_spartan-0.2.6/python_spartan/stubs/handler/api_subscribe.stub
+-rw-r--r--   0        0        0      334 2023-12-15 09:36:48.325747 python_spartan-0.2.6/python_spartan/stubs/handler/aws_codecommit_subscribe.stub
+-rw-r--r--   0        0        0      341 2023-12-15 09:36:48.325854 python_spartan-0.2.6/python_spartan/stubs/handler/aws_config_subscribe.stub
+-rw-r--r--   0        0        0      205 2023-12-15 09:36:48.325936 python_spartan-0.2.6/python_spartan/stubs/handler/aws_iot_button_subscribe.stub
+-rw-r--r--   0        0        0      230 2023-12-15 09:36:48.326071 python_spartan-0.2.6/python_spartan/stubs/handler/aws_iot_core_subscribe.stub
+-rw-r--r--   0        0        0      226 2023-12-15 09:36:48.326159 python_spartan-0.2.6/python_spartan/stubs/handler/aws_secrets_manager_rotation_subscribe.stub
+-rw-r--r--   0        0        0      187 2023-12-15 09:36:48.326227 python_spartan-0.2.6/python_spartan/stubs/handler/aws_step_function_subscribe.stub
+-rw-r--r--   0        0        0      271 2023-12-15 09:36:48.326290 python_spartan-0.2.6/python_spartan/stubs/handler/cloudtrail_subscribe.stub
+-rw-r--r--   0        0        0      108 2023-12-15 09:36:48.326377 python_spartan-0.2.6/python_spartan/stubs/handler/cloudwatch_logs_subscribe.stub
+-rw-r--r--   0        0        0      247 2023-12-15 09:36:48.326464 python_spartan-0.2.6/python_spartan/stubs/handler/cognito_subscribe.stub
+-rw-r--r--   0        0        0      108 2023-12-15 09:36:48.326533 python_spartan-0.2.6/python_spartan/stubs/handler/default.stub
+-rw-r--r--   0        0        0      339 2023-12-15 09:36:48.326605 python_spartan-0.2.6/python_spartan/stubs/handler/elastic_load_balancer_subscribe.stub
+-rw-r--r--   0        0        0      409 2023-12-15 09:36:48.326682 python_spartan-0.2.6/python_spartan/stubs/handler/lambda_ws.stub
+-rw-r--r--   0        0        0      186 2023-12-15 09:36:48.326783 python_spartan-0.2.6/python_spartan/stubs/handler/mqtt_over_ws_subscribe.stub
+-rw-r--r--   0        0        0      273 2023-12-15 09:36:48.326856 python_spartan-0.2.6/python_spartan/stubs/handler/s3_subscribe.stub
+-rw-r--r--   0        0        0      224 2023-12-15 09:36:48.326928 python_spartan-0.2.6/python_spartan/stubs/handler/ses_subscribe.stub
+-rw-r--r--   0        0        0      202 2023-12-15 09:36:48.327009 python_spartan-0.2.6/python_spartan/stubs/handler/sns_subscribe.stub
+-rw-r--r--   0        0        0     1075 2023-12-15 09:36:48.327105 python_spartan-0.2.6/python_spartan/stubs/handler/sqs_both.stub
+-rw-r--r--   0        0        0      122 2023-12-15 09:36:48.327208 python_spartan-0.2.6/python_spartan/stubs/handler/sqs_listen.stub
+-rw-r--r--   0        0        0      275 2023-12-15 09:36:48.327290 python_spartan-0.2.6/python_spartan/stubs/handler/sqs_publish.stub
+-rw-r--r--   0        0        0      942 2023-12-15 09:36:48.327366 python_spartan-0.2.6/python_spartan/stubs/handler/sqs_subscribe.stub
+-rw-r--r--   0        0        0      111 2023-12-15 09:36:48.327437 python_spartan-0.2.6/python_spartan/stubs/handler/sqs_trigger.stub
+-rw-r--r--   0        0        0      330 2023-12-28 08:25:44.489306 python_spartan-0.2.6/python_spartan/stubs/infrastructure/default.stub
+-rw-r--r--   0        0        0      179 2023-12-15 09:36:48.327686 python_spartan-0.2.6/python_spartan/stubs/infrastructure/fifo_dlq.stub
+-rw-r--r--   0        0        0      178 2023-12-15 09:36:48.327751 python_spartan-0.2.6/python_spartan/stubs/infrastructure/fifo_sqs.stub
+-rw-r--r--   0        0        0      334 2023-12-15 09:36:48.327832 python_spartan-0.2.6/python_spartan/stubs/infrastructure/fifo_with_dlq.stub
+-rw-r--r--   0        0        0       70 2023-12-15 09:36:48.327921 python_spartan-0.2.6/python_spartan/stubs/infrastructure/iamrole_lambda.stub
+-rw-r--r--   0        0        0      189 2023-12-15 09:36:48.328001 python_spartan-0.2.6/python_spartan/stubs/infrastructure/iamrole_sqs.stub
+-rw-r--r--   0        0        0      219 2023-12-15 09:36:48.328094 python_spartan-0.2.6/python_spartan/stubs/infrastructure/lambda_triggered_by_http.stub
+-rw-r--r--   0        0        0      147 2023-12-15 09:36:48.328179 python_spartan-0.2.6/python_spartan/stubs/infrastructure/lambda_triggered_by_sns.stub
+-rw-r--r--   0        0        0      147 2023-12-15 09:36:48.328249 python_spartan-0.2.6/python_spartan/stubs/infrastructure/lambda_triggered_by_sqs.stub
+-rw-r--r--   0        0        0      147 2023-12-15 09:36:48.328310 python_spartan-0.2.6/python_spartan/stubs/infrastructure/lambda_triggered_by_ws.stub
+-rw-r--r--   0        0        0     1567 2024-05-11 04:33:36.659978 python_spartan-0.2.6/python_spartan/stubs/infrastructure/serverless.stub
+-rw-r--r--   0        0        0      124 2023-12-15 09:36:48.328459 python_spartan-0.2.6/python_spartan/stubs/infrastructure/standard_dlq.stub
+-rw-r--r--   0        0        0      123 2023-12-15 09:36:48.328519 python_spartan-0.2.6/python_spartan/stubs/infrastructure/standard_sqs.stub
+-rw-r--r--   0        0        0      279 2023-12-15 09:36:48.328582 python_spartan-0.2.6/python_spartan/stubs/infrastructure/standard_with_dlq.stub
+-rw-r--r--   0        0        0      537 2023-12-15 09:36:48.328652 python_spartan-0.2.6/python_spartan/stubs/infrastructure/ws.stub
+-rw-r--r--   0        0        0     3298 2023-12-15 09:36:48.328779 python_spartan-0.2.6/python_spartan/stubs/migration/mssql_alembic.stub
+-rw-r--r--   0        0        0     3278 2023-12-15 09:36:48.328895 python_spartan-0.2.6/python_spartan/stubs/migration/mysql_alembic.stub
+-rw-r--r--   0        0        0     3282 2023-12-15 09:36:48.328973 python_spartan-0.2.6/python_spartan/stubs/migration/psql_alembic.stub
+-rw-r--r--   0        0        0     3363 2023-12-15 09:36:48.329054 python_spartan-0.2.6/python_spartan/stubs/migration/sqlite_alembic.stub
+-rw-r--r--   0        0        0      624 2023-12-28 08:30:29.956043 python_spartan-0.2.6/python_spartan/stubs/model/default.stub
+-rw-r--r--   0        0        0      615 2023-12-28 08:30:29.956207 python_spartan-0.2.6/python_spartan/stubs/parser/default.stub
+-rw-r--r--   0        0        0     2471 2023-12-28 08:30:29.956365 python_spartan-0.2.6/python_spartan/stubs/plotter/default.stub
+-rw-r--r--   0        0        0     1711 2023-12-28 08:30:29.956527 python_spartan-0.2.6/python_spartan/stubs/request/default.stub
+-rw-r--r--   0        0        0     2401 2024-01-26 22:28:40.133551 python_spartan-0.2.6/python_spartan/stubs/response/default.stub
+-rw-r--r--   0        0        0     9294 2024-05-11 04:32:09.898588 python_spartan-0.2.6/python_spartan/stubs/route/default.stub
+-rw-r--r--   0        0        0    14331 2024-05-11 04:41:29.363756 python_spartan-0.2.6/python_spartan/stubs/service/default.stub
+-rw-r--r--   0        0        0     1471 2023-12-15 09:36:48.329744 python_spartan-0.2.6/python_spartan/stubs/service/elastic_search.stub
+-rw-r--r--   0        0        0     1003 2023-12-15 09:36:48.329813 python_spartan-0.2.6/python_spartan/stubs/service/email.stub
+-rw-r--r--   0        0        0      833 2023-12-15 09:36:48.329877 python_spartan-0.2.6/python_spartan/stubs/service/queue.stub
+-rw-r--r--   0        0        0     1397 1970-01-01 00:00:00.000000 python_spartan-0.2.6/PKG-INFO
```

### Comparing `python_spartan-0.2.5/pyproject.toml` & `python_spartan-0.2.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-spartan"
-version = "0.2.5"
+version = "0.2.6"
 description = "Spartan, often referred to as \"The swiss army knife for serverless development,\" is a tool that simplifies the creation of serverless applications on popular cloud providers by generating Python code for classes and more. It streamlines your development process, saving you time and ensuring code consistency in your serverless projects."
 authors = ["nerdmonkey <sydel.palinlin@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -12,14 +12,15 @@
 isort = "^5.12.0"
 requests = "^2.31.0"
 alembic = "^1.12.0"
 poetry = "^1.7.0"
 pyyaml = "^6.0.1"
 pymysql = "^1.1.0"
 faker = "^20.1.0"
+inflect = "^7.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest-cov = "^4.1.0"
 faker = "^20.1.0"
 pytest = "^7.4.3"
 black = "^23.11.0"
```

### Comparing `python_spartan-0.2.5/python_spartan/main.py` & `python_spartan-0.2.6/python_spartan/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,53 @@
+import os
+import shutil
 import subprocess
-import typer
+import sys
 from typing import Optional
-from pathlib import Path
-import shutil
-import os
-from alembic import command
+
+import typer
 from alembic.config import Config
+
 from python_spartan.services.application import ApplicationService
-from python_spartan.services.response import ResponseService
-from python_spartan.services.request import RequestService
+from python_spartan.services.deployment import DeploymentService
+from python_spartan.services.handler import HandlerService
+from python_spartan.services.infrastructure import InfrastructureService
+from python_spartan.services.inspire import InspireService
+from python_spartan.services.migrate import MigrateService
 from python_spartan.services.model import ModelService
-from python_spartan.services.service import ServiceService
-from python_spartan.services.route import RouteService
 from python_spartan.services.parser import ParserService
 from python_spartan.services.plotter import PlotterService
-from python_spartan.services.handler import HandlerService
-from python_spartan.services.migrate import MigrateService
+from python_spartan.services.request import RequestService
+from python_spartan.services.response import ResponseService
+from python_spartan.services.route import RouteService
+from python_spartan.services.service import ServiceService
 from python_spartan.services.test import TestService
-from python_spartan.services.inspire import InspireService
-from python_spartan.services.deployment import DeploymentService
-from python_spartan.services.infrastructure import InfrastructureService
-import sys
 
 alembic_cfg = Config("alembic.ini")
 
 app = typer.Typer()
 
 model_app = typer.Typer()
 app.add_typer(
-    model_app,
-    name="model",
-    help="Manages the creation and deletion of model classes."
+    model_app, name="model", help="Manages the creation and deletion of model classes."
 )
 
 parser_app = typer.Typer()
 app.add_typer(
     parser_app,
     name="parser",
-    help="Manages the creation and deletion of parser classes."
+    help="Manages the creation and deletion of parser classes.",
 )
 
 
 plotter_app = typer.Typer()
 app.add_typer(
     plotter_app,
     name="plotter",
-    help="Manages the creation and deletion of plotter classes."
+    help="Manages the creation and deletion of plotter classes.",
 )
 
 
 handler_app = typer.Typer()
 app.add_typer(
     handler_app,
     name="handler",
@@ -236,15 +234,15 @@
         print(f"Error upgrading database: {e}")
 
 
 @migrate_app.command(
     "create", help="Create a new database migration with an optional message."
 )
 def migrate_create(
-    message: str = typer.Option("", "--message", "-m", help="Message option."),
+    message: str = typer.Option("", "--comment", "-c", help="Message option."),
 ):
     try:
         migrate_service = MigrateService(alembic_cfg)
         migrate_service.migrate_create(message=message)
     except Exception as e:
         print(f"Error creating database migration: {e}")
```

### Comparing `python_spartan-0.2.5/python_spartan/services/application.py` & `python_spartan-0.2.6/python_spartan/services/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-import os
-import requests
-import zipfile
 import io
+import os
 import shutil
+import zipfile
+
+import requests
 
 
 class ApplicationService:
     def __init__(self, project_name: str):
         self.project_name = project_name
         self.repository_name = "spartan-framework"
 
     def is_valid_folder_name(self):
-        return self.project_name.isidentifier() and not self.project_name[0].isdigit()
+        return (
+            all(c.isidentifier() for c in self.project_name)
+            and not self.project_name[0].isdigit()
+        )
 
     def download_zip(self):
         release_url = f"https://github.com/nerdmonkey/{self.repository_name}/archive/refs/heads/main.zip"
         try:
             response = requests.get(release_url)
             response.raise_for_status()
             return io.BytesIO(response.content)
@@ -52,43 +56,50 @@
             print(f"{self.project_name} is not a valid project name. Aborting.")
             return
 
         zip_data = self.download_zip()
         if zip_data:
             temp_folder = self.extract_zip(zip_data)
             if temp_folder and self.setup_project(temp_folder):
-                print("\n")
-                ascii_art = [
-                    ".d8888. d8888b.  .d8b.  d8888b. d888888b  .d8b.  d8b   db",
-                    "88'  YP 88  `8D d8' `8b 88  `8D `~~88~~' d8' `8b 888o  88",
-                    "`8bo.   88oodD' 88ooo88 88oobY'    88    88ooo88 88V8o 88",
-                    "  `Y8b. 88~~~   88~~~88 88`8b      88    88~~~88 88 V8o88",
-                    "db   8D 88      88   88 88 `88.    88    88   88 88  V888",
-                    "`8888Y' 88      YP   YP 88   YD    YP    YP   YP VP   V8P",
-                ]
-
-                for line in ascii_art:
-                    print(line)
-
-                message = [
-                    "Embark on your cloud software journey with Spartan determination and simplicity."
-                    "Build your digital empire with unwavering focus and minimalism,"
-                    "just like the warriors of ancient Sparta."
-                ]
-
-                for line in message:
-                    print("\n")
-                    print(line)
-
-                print(
-                    f"\nSuccessfully setup the project to {self.project_name} folder."
-                )
-                print(f"\nYour First Mission:")
-                print(f"---------------")
-                print(f"cd {self.project_name}")
-                print(f"pip install -r requirements.txt")
-                print(f"copy the .env.example and name it as .env")
-                print(f"spartan migrate init -d sqlite")
-                print(f"spartan migrate upgrade")
-                print(f"spartan serve")
+                self.print_ascii_art()
+                self.print_message()
+                self.print_success_message()
+                self.print_first_mission()
             else:
                 print("Error: The ZIP file should contain a single top-level folder.")
+
+    def print_ascii_art(self):
+        ascii_art = [
+            ".d8888. d8888b.  .d8b.  d8888b. d888888b  .d8b.  d8b   db",
+            "88'  YP 88  `8D d8' `8b 88  `8D `~~88~~' d8' `8b 888o  88",
+            "`8bo.   88oodD' 88ooo88 88oobY'    88    88ooo88 88V8o 88",
+            "  `Y8b. 88~~~   88~~~88 88`8b      88    88~~~88 88 V8o88",
+            "db   8D 88      88   88 88 `88.    88    88   88 88  V888",
+            "`8888Y' 88      YP   YP 88   YD    YP    YP   YP VP   V8P",
+        ]
+
+        for line in ascii_art:
+            print(line)
+
+    def print_message(self):
+        message = [
+            "Embark on your cloud software journey with Spartan determination and simplicity.",
+            "Build your digital empire with unwavering focus and minimalism,",
+            "just like the warriors of ancient Sparta.",
+        ]
+
+        for line in message:
+            print("\n")
+            print(line)
+
+    def print_success_message(self):
+        print(f"\nSuccessfully setup the project to {self.project_name} folder.")
+
+    def print_first_mission(self):
+        print(f"\nYour First Mission:")
+        print(f"---------------")
+        print(f"cd {self.project_name}")
+        print(f"pip install -r requirements.txt")
+        print(f"copy the .env.example and name it as .env")
+        print(f"spartan migrate init -d sqlite")
+        print(f"spartan migrate upgrade")
+        print(f"spartan serve")
```

### Comparing `python_spartan-0.2.5/python_spartan/services/deployment.py` & `python_spartan-0.2.6/python_spartan/services/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import shutil
-import typer
 from pathlib import Path
 
+import typer
+
 
 class DeploymentService:
     def __init__(self):
         self.current_directory = Path.cwd()
 
     def config(self, source: str):
         source_path = Path(source)
```

### Comparing `python_spartan-0.2.5/python_spartan/services/handler.py` & `python_spartan-0.2.6/python_spartan/services/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import re
 
+
 class HandlerService:
     def __init__(self, name: str, subscribe: str = None, publish: str = None):
         self.name = name
         self.subscribe = subscribe
         self.publish = publish
         self.home_directory = os.path.dirname(
             os.path.dirname(os.path.abspath(__file__))
```

### Comparing `python_spartan-0.2.5/python_spartan/services/inspire.py` & `python_spartan-0.2.6/python_spartan/services/inspire.py`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/services/migrate.py` & `python_spartan-0.2.6/python_spartan/services/migrate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,50 @@
-import os
-from pathlib import Path
 import shutil
+from pathlib import Path
+
 from alembic import command
 
 
 class MigrateService:
     def __init__(self, alembic_cfg):
         self.alembic_cfg = alembic_cfg
 
     def migrate_initialize(self, db_type: str):
-        # Create a 'database' folder in the current directory if it doesn't exist
         database_dir = Path.cwd() / "database"
         database_dir.mkdir(exist_ok=True)
         print(f"Ensured 'database' folder exists in the current directory.")
 
-        # Create 'spartan.db' in the 'database' folder if it doesn't exist
         db_path = database_dir / "spartan.db"
         if not db_path.exists():
             db_path.touch()
             print("Created 'spartan.db' in the 'database' folder.")
         else:
             print("'spartan.db' already exists in the 'database' folder.")
 
-        # Define the destination path for alembic.ini
         destination_path = Path.cwd() / "alembic.ini"
 
-        # Check if alembic.ini already exists
         if destination_path.exists():
             print(
                 "alembic.ini already exists in the current directory. Operation aborted to prevent overwriting."
             )
             return
 
-        # Define the source path based on db_type
         stub_mapping = {
             "psql": "psql_alembic.stub",
             "mysql": "mysql_alembic.stub",
             "sqlite": "sqlite_alembic.stub",
         }
 
         stub_file = stub_mapping.get(db_type)
         if not stub_file:
             print(f"Unsupported or unnecessary database type for stub: {db_type}")
             return
 
         source_path = Path(__file__).parent.parent / "stubs" / "migration" / stub_file
 
-        # Copy the file
         try:
             shutil.copyfile(source_path, destination_path)
             print(f"New alembic.ini has been created in the current directory.")
         except Exception as e:
             print(f"Error occurred while copying the file: {e}")
 
     def migrate_create(self, message=""):
```

### Comparing `python_spartan-0.2.5/python_spartan/services/model.py` & `python_spartan-0.2.6/python_spartan/services/model.py`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/services/parser.py` & `python_spartan-0.2.6/python_spartan/services/parser.py`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/services/plotter.py` & `python_spartan-0.2.6/python_spartan/services/plotter.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,32 +19,15 @@
             self.current_directory,
             self.parent_folder,
             self.destination_folder,
             self.file_name,
         )
 
     def create_plotter_file(self):
-        if not os.path.exists(
-            os.path.join(
-                self.current_directory, self.parent_folder, self.destination_folder
-            )
-        ):
-            try:
-                os.makedirs(
-                    os.path.join(
-                        self.current_directory,
-                        self.parent_folder,
-                        self.destination_folder,
-                    )
-                )
-                print(f"Created '{self.destination_folder}' folder.")
-            except OSError as e:
-                print(f"Error creating directory: {e}")
-                return
-
+        self.create_destination_folder()
         if not os.path.exists(self.file_path):
             try:
                 with open(self.source_stub, "r") as source_file:
                     handler_stub_content = source_file.read()
             except FileNotFoundError:
                 print(f"Stub file '{self.source_stub}' not found.")
                 return
@@ -71,7 +54,19 @@
             try:
                 os.remove(self.file_path)
                 print(f'File "{self.file_path}" deleted successfully.')
             except Exception as e:
                 print(f"An error occurred while trying to delete the file: {e}")
         else:
             print(f'File "{self.file_path}" does not exist. No deletion needed.')
+
+    def create_destination_folder(self):
+        destination_folder_path = os.path.join(
+            self.current_directory, self.parent_folder, self.destination_folder
+        )
+        if not os.path.exists(destination_folder_path):
+            try:
+                os.makedirs(destination_folder_path)
+                print(f"Created '{self.destination_folder}' folder.")
+            except OSError as e:
+                print(f"Error creating directory: {e}")
+                return
```

### Comparing `python_spartan-0.2.5/python_spartan/services/request.py` & `python_spartan-0.2.6/python_spartan/services/request.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,32 +19,15 @@
             self.current_directory,
             self.parent_folder,
             self.destination_folder,
             self.file_name,
         )
 
     def create_request_file(self):
-        if not os.path.exists(
-            os.path.join(
-                self.current_directory, self.parent_folder, self.destination_folder
-            )
-        ):
-            try:
-                os.makedirs(
-                    os.path.join(
-                        self.current_directory,
-                        self.parent_folder,
-                        self.destination_folder,
-                    )
-                )
-                print(f"Created '{self.destination_folder}' folder.")
-            except OSError as e:
-                print(f"Error creating directory: {e}")
-                return
-
+        self.create_destination_folder()
         if not os.path.exists(self.file_path):
             try:
                 with open(self.source_stub, "r") as source_file:
                     handler_stub_content = source_file.read()
             except FileNotFoundError:
                 print(f"Stub file '{self.source_stub}' not found.")
                 return
@@ -71,7 +54,19 @@
             try:
                 os.remove(self.file_path)
                 print(f'File "{self.file_path}" deleted successfully.')
             except Exception as e:
                 print(f"An error occurred while trying to delete the file: {e}")
         else:
             print(f'File "{self.file_path}" does not exist. No deletion needed.')
+
+    def create_destination_folder(self):
+        destination_folder_path = os.path.join(
+            self.current_directory, self.parent_folder, self.destination_folder
+        )
+        if not os.path.exists(destination_folder_path):
+            try:
+                os.makedirs(destination_folder_path)
+                print(f"Created '{self.destination_folder}' folder.")
+            except OSError as e:
+                print(f"Error creating directory: {e}")
+                return
```

### Comparing `python_spartan-0.2.5/python_spartan/services/response.py` & `python_spartan-0.2.6/python_spartan/services/response.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,50 +19,27 @@
             self.current_directory,
             self.parent_folder,
             self.destination_folder,
             self.file_name,
         )
 
     def create_response_file(self):
-        if not os.path.exists(
-            os.path.join(
-                self.current_directory, self.parent_folder, self.destination_folder
-            )
-        ):
-            try:
-                os.makedirs(
-                    os.path.join(
-                        self.current_directory,
-                        self.parent_folder,
-                        self.destination_folder,
-                    )
-                )
-                print(f"Created '{self.destination_folder}' folder.")
-            except OSError as e:
-                print(f"Error creating directory: {e}")
-                return
-
+        self.create_destination_folder()
         if not os.path.exists(self.file_path):
             try:
                 with open(self.source_stub, "r") as source_file:
                     handler_stub_content = source_file.read()
             except FileNotFoundError:
                 print(f"Stub file '{self.source_stub}' not found.")
                 return
             except Exception as e:
                 print(f"An error occurred while reading the stub file: {e}")
                 return
 
-            updated_content = handler_stub_content.replace("{{file_name}}", self.name)
-            updated_content = updated_content.replace(
-                "{{class_name_title_case_singular}}", self.name.capitalize()
-            )
-            updated_content = updated_content.replace(
-                "{{class_name_lower_case_plural}}", self.name.lower() + "s"
-            )
+            updated_content = self.update_stub_content(handler_stub_content)
 
             try:
                 with open(self.file_path, "w") as destination_file:
                     destination_file.write(updated_content)
                 print(f"File '{self.file_path}' created successfully.")
             except Exception as e:
                 print(f"An error occurred while writing the new response file: {e}")
@@ -74,7 +51,29 @@
             try:
                 os.remove(self.file_path)
                 print(f'File "{self.file_path}" deleted successfully.')
             except Exception as e:
                 print(f"An error occurred while trying to delete the file: {e}")
         else:
             print(f'File "{self.file_path}" does not exist. No deletion needed.')
+
+    def create_destination_folder(self):
+        destination_folder_path = os.path.join(
+            self.current_directory, self.parent_folder, self.destination_folder
+        )
+        if not os.path.exists(destination_folder_path):
+            try:
+                os.makedirs(destination_folder_path)
+                print(f"Created '{self.destination_folder}' folder.")
+            except OSError as e:
+                print(f"Error creating directory: {e}")
+                return
+
+    def update_stub_content(self, handler_stub_content):
+        updated_content = handler_stub_content.replace("{{file_name}}", self.name)
+        updated_content = updated_content.replace(
+            "{{class_name_title_case_singular}}", self.name.capitalize()
+        )
+        updated_content = updated_content.replace(
+            "{{class_name_lower_case_plural}}", self.name.lower() + "s"
+        )
+        return updated_content
```

### Comparing `python_spartan-0.2.5/python_spartan/services/route.py` & `python_spartan-0.2.6/python_spartan/services/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,83 @@
 import os
 import re
+import inflect
 
-
-class RouteService:
+class ServiceService:
     def __init__(self, name: str):
         self.name = name
+        self.p = inflect.engine()
         self.home_directory = os.path.dirname(
             os.path.dirname(os.path.abspath(__file__))
         )
         self.current_directory = os.getcwd()
-        self.destination_folder = "routes"
+        self.parent_folder = "app"
+        self.destination_folder = "services"
         self.source_stub = os.path.join(
-            self.home_directory, "stubs", "route", "default.stub"
+            self.home_directory, "stubs", "service", "default.stub"
         )
-        self.file_name = re.sub(r"\d", "", f"{self.name}s.py").lower()
+        self.file_name = re.sub(r"\d", "", f"{self.name}.py").lower()
         self.file_path = os.path.join(
             self.current_directory,
+            self.parent_folder,
             self.destination_folder,
             self.file_name,
         )
 
-    def create_route_file(self):
-        if not os.path.exists(
-            os.path.join(
-                self.current_directory, self.destination_folder
-            )
-        ):
-            try:
-                os.makedirs(
-                    os.path.join(
-                        self.current_directory,
-                        self.destination_folder,
-                    )
-                )
-                print(f"Created '{self.destination_folder}' folder.")
-            except OSError as e:
-                print(f"Error creating directory: {e}")
-                return
-
+    def create_service_file(self):
+        self.create_destination_folder()
         if not os.path.exists(self.file_path):
             try:
                 with open(self.source_stub, "r") as source_file:
                     handler_stub_content = source_file.read()
             except FileNotFoundError:
                 print(f"Stub file '{self.source_stub}' not found.")
                 return
             except Exception as e:
                 print(f"An error occurred while reading the stub file: {e}")
                 return
 
-            updated_content = handler_stub_content.replace("{{file_name}}", self.name)
-            updated_content = updated_content.replace(
-                "{{class_name_title_case_singular}}", self.name.capitalize()
-            )
-            updated_content = updated_content.replace(
-                "{{class_name_lower_case_singular}}", self.name.lower()
-            )
-            updated_content = updated_content.replace(
-                "{{class_name_lower_case_plural}}", self.name.lower() + "s"
-            )
+            updated_content = self.update_stub_content(handler_stub_content)
 
             try:
                 with open(self.file_path, "w") as destination_file:
                     destination_file.write(updated_content)
                 print(f"File '{self.file_path}' created successfully.")
             except Exception as e:
-                print(f"An error occurred while writing the new route file: {e}")
+                print(f"An error occurred while writing the new service file: {e}")
         else:
             print(f"File '{self.file_path}' already exists. Skipping creation.")
 
-    def delete_route_file(self):
+    def delete_service_file(self):
         if os.path.exists(self.file_path):
             try:
                 os.remove(self.file_path)
                 print(f'File "{self.file_path}" deleted successfully.')
             except Exception as e:
                 print(f"An error occurred while trying to delete the file: {e}")
         else:
             print(f'File "{self.file_path}" does not exist. No deletion needed.')
+
+    def create_destination_folder(self):
+        destination_folder_path = os.path.join(
+            self.current_directory, self.parent_folder, self.destination_folder
+        )
+        if not os.path.exists(destination_folder_path):
+            try:
+                os.makedirs(destination_folder_path)
+                print(f"Created '{self.destination_folder}' folder.")
+            except OSError as e:
+                print(f"Error creating directory: {e}")
+                return
+
+    def update_stub_content(self, handler_stub_content):
+        updated_content = handler_stub_content.replace("{{file_name}}", self.name)
+        updated_content = updated_content.replace(
+            "{{class_name_title_case_singular}}", self.name.capitalize()
+        )
+        updated_content = updated_content.replace(
+            "{{class_name_lower_case_singular}}", self.name.lower()
+        )
+        updated_content = updated_content.replace(
+            "{{class_name_lower_case_plural}}", self.p.plural(self.name.lower())
+        )
+        return updated_content
```

### Comparing `python_spartan-0.2.5/python_spartan/services/service.py` & `python_spartan-0.2.6/python_spartan/services/route.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,80 @@
 import os
 import re
 
 
-class ServiceService:
+class RouteService:
     def __init__(self, name: str):
         self.name = name
         self.home_directory = os.path.dirname(
             os.path.dirname(os.path.abspath(__file__))
         )
         self.current_directory = os.getcwd()
-        self.parent_folder = "app"
-        self.destination_folder = "services"
+        self.destination_folder = "routes"
         self.source_stub = os.path.join(
-            self.home_directory, "stubs", "service", "default.stub"
+            self.home_directory, "stubs", "route", "default.stub"
         )
-        self.file_name = re.sub(r"\d", "", f"{self.name}.py").lower()
+        self.file_name = re.sub(r"\d", "", f"{self.name}s.py").lower()
         self.file_path = os.path.join(
             self.current_directory,
-            self.parent_folder,
             self.destination_folder,
             self.file_name,
         )
 
-    def create_service_file(self):
-        if not os.path.exists(
-            os.path.join(
-                self.current_directory, self.parent_folder, self.destination_folder
-            )
-        ):
-            try:
-                os.makedirs(
-                    os.path.join(
-                        self.current_directory,
-                        self.parent_folder,
-                        self.destination_folder,
-                    )
-                )
-                print(f"Created '{self.destination_folder}' folder.")
-            except OSError as e:
-                print(f"Error creating directory: {e}")
-                return
-
+    def create_route_file(self):
+        self.create_destination_folder()
         if not os.path.exists(self.file_path):
             try:
                 with open(self.source_stub, "r") as source_file:
                     handler_stub_content = source_file.read()
             except FileNotFoundError:
                 print(f"Stub file '{self.source_stub}' not found.")
                 return
             except Exception as e:
                 print(f"An error occurred while reading the stub file: {e}")
                 return
 
-            updated_content = handler_stub_content.replace("{{file_name}}", self.name)
-            updated_content = updated_content.replace(
-                "{{class_name_title_case_singular}}", self.name.capitalize()
-            )
-            updated_content = updated_content.replace(
-                "{{class_name_lower_case_singular}}", self.name.lower()
-            )
-            updated_content = updated_content.replace(
-                "{{class_name_lower_case_plural}}", self.name.lower() + "s"
-            )
+            updated_content = self.update_stub_content(handler_stub_content)
 
             try:
                 with open(self.file_path, "w") as destination_file:
                     destination_file.write(updated_content)
                 print(f"File '{self.file_path}' created successfully.")
             except Exception as e:
-                print(f"An error occurred while writing the new service file: {e}")
+                print(f"An error occurred while writing the new route file: {e}")
         else:
             print(f"File '{self.file_path}' already exists. Skipping creation.")
 
-    def delete_service_file(self):
+    def delete_route_file(self):
         if os.path.exists(self.file_path):
             try:
                 os.remove(self.file_path)
                 print(f'File "{self.file_path}" deleted successfully.')
             except Exception as e:
                 print(f"An error occurred while trying to delete the file: {e}")
         else:
             print(f'File "{self.file_path}" does not exist. No deletion needed.')
+
+    def create_destination_folder(self):
+        destination_folder_path = os.path.join(
+            self.current_directory, self.destination_folder
+        )
+        if not os.path.exists(destination_folder_path):
+            try:
+                os.makedirs(destination_folder_path)
+                print(f"Created '{self.destination_folder}' folder.")
+            except OSError as e:
+                print(f"Error creating directory: {e}")
+                return
+
+    def update_stub_content(self, handler_stub_content):
+        updated_content = handler_stub_content.replace("{{file_name}}", self.name)
+        updated_content = updated_content.replace(
+            "{{class_name_title_case_singular}}", self.name.capitalize()
+        )
+        updated_content = updated_content.replace(
+            "{{class_name_lower_case_singular}}", self.name.lower()
+        )
+        updated_content = updated_content.replace(
+            "{{class_name_lower_case_plural}}", self.name.lower() + "s"
+        )
+        return updated_content
```

### Comparing `python_spartan-0.2.5/python_spartan/services/test.py` & `python_spartan-0.2.6/python_spartan/services/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import typer
 import subprocess
 
+import typer
+
 
 class TestService:
     def __init__(self, coverage: str = None, report: str = None):
         self.coverage = coverage
         self.report = report
 
     def run(self):
```

### Comparing `python_spartan-0.2.5/python_spartan/stubs/handler/sqs_both.stub` & `python_spartan-0.2.6/python_spartan/stubs/handler/sqs_both.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/handler/sqs_subscribe.stub` & `python_spartan-0.2.6/python_spartan/stubs/handler/sqs_subscribe.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/infrastructure/serverless.stub` & `python_spartan-0.2.6/python_spartan/stubs/infrastructure/serverless.stub`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
       - sg-<name>
     subnetIds:
       - subnet-<name>
       - subnet-<name>
       - subnet-<name>
    iam:
     role: arn:aws:iam::${aws:accountId}:role/<role_name>
+
 functions:
     validator:
         handler: public.main.handle
         timeout: 10
         memorySize: 512
         events:
         - http:
@@ -36,27 +37,34 @@
             method: any
             cors:
                 origin: ${env:ALLOWED_ORIGINS}
                 maxAge: 60
 plugins:
   - serverless-lift
   - serverless-python-requirements
-  - serverless-plugin-warmup
+
 package:
   patterns:
+    - "!__pycache__/**"
+    - "!.pytest_cache/**"
     - "!node_modules/**"
     - "!database/**"
+    - "!.serverless/**"
     - "!tests/**"
     - "!.venv**"
     - "!venv**"
+    - "!alembic.ini"
+    - "!*.ipynb"
+    - "!.vscode/**"
     - "!CHANGEDLOG.md"
     - "!CODE_OF_CONDUCT.md"
     - "!CONTRIBUTING.md"
     - "!requirements_dev.txt"
     - "!requirements_all.txt"
+
 resources:
     Resources:
 custom:
   pythonRequirements:
     usePoetry: true
     noDeploy:
       - boto3
```

### Comparing `python_spartan-0.2.5/python_spartan/stubs/infrastructure/ws.stub` & `python_spartan-0.2.6/python_spartan/stubs/infrastructure/ws.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/migration/mssql_alembic.stub` & `python_spartan-0.2.6/python_spartan/stubs/migration/mssql_alembic.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/migration/mysql_alembic.stub` & `python_spartan-0.2.6/python_spartan/stubs/migration/mysql_alembic.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/migration/psql_alembic.stub` & `python_spartan-0.2.6/python_spartan/stubs/migration/psql_alembic.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/migration/sqlite_alembic.stub` & `python_spartan-0.2.6/python_spartan/stubs/migration/sqlite_alembic.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/model/default.stub` & `python_spartan-0.2.6/python_spartan/stubs/model/default.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/parser/default.stub` & `python_spartan-0.2.6/python_spartan/stubs/parser/default.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/plotter/default.stub` & `python_spartan-0.2.6/python_spartan/stubs/plotter/default.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/request/default.stub` & `python_spartan-0.2.6/python_spartan/stubs/request/default.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/response/default.stub` & `python_spartan-0.2.6/python_spartan/stubs/response/default.stub`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 
     Attributes:
         current_page (int): The current page number.
         items_per_current_page (int): The number of items per page.
         total_items (int): The total number of items.
     """
     current_page: int
+    last_page: int
+    first_item: int
+    last_item: int
     items_per_page: int
     total: int
 
 class Paginated{{class_name_title_case_singular}}Response(BaseModel):
     """
     Pydantic model representing a paginated response for a list of users.
```

### Comparing `python_spartan-0.2.5/python_spartan/stubs/route/default.stub` & `python_spartan-0.2.6/python_spartan/stubs/route/default.stub`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,81 @@
 import logging
-from typing import List, Optional
+from datetime import date
+from typing import Optional
 
 from fastapi import APIRouter, Depends, HTTPException, Query
 from sqlalchemy.orm import Session
 
-from app.models.{{class_name_lower_case_singular}} import {{class_name_title_case_singular}}
 from app.requests.{{class_name_lower_case_singular}} import {{class_name_title_case_singular}}CreateRequest, {{class_name_title_case_singular}}UpdateRequest
-from app.responses.{{class_name_lower_case_singular}} import (
-    Paginated{{class_name_title_case_singular}}Response,
-    Single{{class_name_title_case_singular}}Response
-)
+from app.responses.{{class_name_lower_case_singular}} import Paginated{{class_name_title_case_singular}}Response, Single{{class_name_title_case_singular}}Response
 from app.services.{{class_name_lower_case_singular}} import {{class_name_title_case_singular}}Service
 from config.database import get_session
-from datetime import date
 
 {{class_name_lower_case_singular}}_service = {{class_name_title_case_singular}}Service(db=None)
 
 route = APIRouter(
     prefix="/api", tags=["{{class_name_title_case_singular}}s"], responses={404: {"description": "Not found"}}
 )
 
 
-@route.get("/{{class_name_lower_case_singular}}s", status_code=200, response_model=Paginated{{class_name_title_case_singular}}Response)
+@route.get("/{{class_name_lower_case_plural}}", status_code=200, response_model=Paginated{{class_name_title_case_singular}}Response)
 async def get_{{class_name_lower_case_singular}}s(
     page: Optional[int] = Query(1, description="page number", gt=0),
     items_per_page: Optional[int] = Query(10, description="items per page", gt=0),
-    sort_type: Optional[str] = Query('asc', description="sort type (asc or desc)"),
-    sort_by: Optional[str] = Query('id', description="sort by field"),
-    first_field: Optional[str] = Query(None, description="first field filter"),
-    second_field: Optional[str] = Query(None, description="second field filter"),
+    sort_type: Optional[str] = Query("asc", description="sort type (asc or desc)"),
+    sort_by: Optional[str] = Query("id", description="sort by field"),
+    username: Optional[str] = Query(None, description="username filter"),
+    email: Optional[str] = Query(None, description="email filter"),
     start_date: Optional[date] = Query(None, description="start date filter"),
     end_date: Optional[date] = Query(None, description="end date filter"),
     db: Session = Depends(get_session),
 ):
     """
-    Get a list of {{class_name_lower_case_singular}}s with pagination and optional filters.
+    Get a list of {{class_name_lower_case_plural}} with pagination and optional filters.
 
     Args:
         page (int): The page number.
         items_per_page (int): Number of items per page.
         sort_by (str): Sort by field.
         sort_type (str): Sort type (asc or desc).
         start_date (date): Start date filter.
         end_date (date): End date filter.
-        first_field (str): First field filter.
-        second_field (str): Second field filter.
+        username (str): Username filter.
+        email (str): Email filter.
         db (Session): SQLAlchemy database session.
 
     Returns:
         List[{{class_name_title_case_singular}}Response]: List of {{class_name_lower_case_singular}} objects.
     """
     try:
         {{class_name_lower_case_singular}}_service.db = db
         items, total, last_page, first_item, last_item = {{class_name_lower_case_singular}}_service.all(
-            page, items_per_page, sort_type=sort_type, sort_by=sort_by,
-            start_date=start_date, end_date=end_date, first_field=first_field, second_field=second_field
+            page,
+            items_per_page,
+            sort_type=sort_type,
+            sort_by=sort_by,
+            start_date=start_date,
+            end_date=end_date,
+            username=username,
+            email=email,
         )
 
         if not items:
-            raise ValueError("No {{class_name_lower_case_singular}}s found")
+            return {
+                "data": [],
+                "meta": {
+                    "current_page": 0,
+                    "last_page": 0,
+                    "first_item": 0,
+                    "last_item": 0,
+                    "items_per_page": 0,
+                    "total": 0,
+                },
+                "status_code": 404,
+            }
 
         return {
             "data": items,
             "meta": {
                 "current_page": page,
                 "last_page": last_page,
                 "first_item": first_item,
@@ -75,15 +88,15 @@
     except ValueError as e:
         raise HTTPException(status_code=404, detail=f"{e}")
     except Exception as e:
         logging.error(e)
         raise HTTPException(status_code=500, detail="Internal server error")
 
 
-@route.get("/{{class_name_lower_case_singular}}s/{id}", status_code=200, response_model=Single{{class_name_title_case_singular}}Response)
+@route.get("/{{class_name_lower_case_plural}}/{id}", status_code=200, response_model=Single{{class_name_title_case_singular}}Response)
 async def get_{{class_name_lower_case_singular}}(id: int, db: Session = Depends(get_session)):
     """
     Get a {{class_name_lower_case_singular}} by their unique identifier.
 
     Args:
         id (int): The unique identifier of the {{class_name_lower_case_singular}}.
         db (Session): SQLAlchemy database session.
@@ -93,43 +106,48 @@
     """
     try:
         {{class_name_lower_case_singular}}_service.db = db
         {{class_name_lower_case_singular}} = {{class_name_lower_case_singular}}_service.find(id)
         if not {{class_name_lower_case_singular}}:
             raise HTTPException(status_code=404, detail="{{class_name_title_case_singular}} not found")
         return {"data": {{class_name_lower_case_singular}}, "status_code": 200}
+    except HTTPException as e:
+        logging.error(e)
+        raise HTTPException(status_code=404, detail="{{class_name_title_case_singular}} not found")
     except Exception as e:
+        logging.error(e)
         raise HTTPException(status_code=500, detail="Internal server error")
 
 
-@route.post("/{{class_name_lower_case_singular}}s", status_code=201, response_model=Single{{class_name_title_case_singular}}Response)
+@route.post("/{{class_name_lower_case_plural}}", status_code=201, response_model=Single{{class_name_title_case_singular}}Response)
 async def create_{{class_name_lower_case_singular}}({{class_name_lower_case_singular}}: {{class_name_title_case_singular}}CreateRequest, db: Session = Depends(get_session)):
     """
     Create a new {{class_name_lower_case_singular}}.
 
     Args:
         {{class_name_lower_case_singular}} ({{class_name_title_case_singular}}CreateRequest): {{class_name_title_case_singular}} creation request.
         db (Session): SQLAlchemy database session.
 
     Returns:
-        {{class_name_title_case_singular}}CreateResponse: Created {{class_name_lower_case_singular}} object.
+        UserCreateResponse: Created {{class_name_lower_case_singular}} object.
 
     Raises:
         HTTPException: If there is an internal server error.
 
     """
     try:
         {{class_name_lower_case_singular}}_service.db = db
         created_{{class_name_lower_case_singular}} = {{class_name_lower_case_singular}}_service.save({{class_name_lower_case_singular}})
         return {"data": created_{{class_name_lower_case_singular}}, "status_code": 201}
     except Exception as e:
+        logging.error(e)
         raise HTTPException(status_code=500, detail="Internal server error")
 
 
-@route.put("/{{class_name_lower_case_singular}}s/{id}", status_code=200, response_model=Single{{class_name_title_case_singular}}Response)
+@route.put("/{{class_name_lower_case_plural}}/{id}", status_code=200, response_model=Single{{class_name_title_case_singular}}Response)
 async def update_{{class_name_lower_case_singular}}(
     id: int, {{class_name_lower_case_singular}}: {{class_name_title_case_singular}}UpdateRequest, db: Session = Depends(get_session)
 ):
     """
     Update an existing {{class_name_lower_case_singular}}'s information.
 
     Args:
@@ -147,21 +165,23 @@
     """
     try:
         {{class_name_lower_case_singular}}_service.db = db
         updated_{{class_name_lower_case_singular}} = {{class_name_lower_case_singular}}_service.update(id, {{class_name_lower_case_singular}})
         if not updated_{{class_name_lower_case_singular}}:
             raise HTTPException(status_code=404, detail="{{class_name_title_case_singular}} not found")
         return {"data": updated_{{class_name_lower_case_singular}}, "status_code": 200}
-    except ValueError as e:
-        raise HTTPException(status_code=400, detail=str(e))
+    except HTTPException as e:
+        logging.error(e)
+        raise HTTPException(status_code=404, detail="{{class_name_title_case_singular}} not found")
     except Exception as e:
+        logging.error(e)
         raise HTTPException(status_code=500, detail="Internal server error")
 
 
-@route.delete("/{{class_name_lower_case_singular}}s/{id}", status_code=200, response_model=Single{{class_name_title_case_singular}}Response)
+@route.delete("/{{class_name_lower_case_plural}}/{id}", status_code=200, response_model=Single{{class_name_title_case_singular}}Response)
 async def delete_{{class_name_lower_case_singular}}(id: int, db: Session = Depends(get_session)):
     """
     Delete a {{class_name_lower_case_singular}} by their unique identifier.
 
     Args:
         id (int): The unique identifier of the {{class_name_lower_case_singular}} to delete.
         db (Session): SQLAlchemy database session.
@@ -174,14 +194,14 @@
     """
     try:
         {{class_name_lower_case_singular}}_service.db = db
 
         {{class_name_lower_case_singular}} = {{class_name_lower_case_singular}}_service.delete(id)
 
         if not {{class_name_lower_case_singular}}:
-            raise HTTPException(status_code=500, detail="Failed to delete {{class_name_lower_case_singular}}")
+            raise HTTPException(status_code=404, detail="{{class_name_title_case_singular}} not found")
 
         return {"data": {{class_name_lower_case_singular}}, "status_code": 200}
     except HTTPException as e:
         raise e
     except Exception as e:
         raise HTTPException(status_code=500, detail=f"Internal server error {e}")
```

### Comparing `python_spartan-0.2.5/python_spartan/stubs/service/default.stub` & `python_spartan-0.2.6/python_spartan/stubs/service/default.stub`

 * *Files 9% similar despite different names*

```diff
@@ -40,55 +40,55 @@
         {{class_name_lower_case_singular}} = self.db.query({{class_name_title_case_singular}}).filter({{class_name_title_case_singular}}.id == id).first()
         if not {{class_name_lower_case_singular}}:
             raise HTTPException(status_code=404, detail="{{class_name_title_case_singular}} not found")
         return {{class_name_lower_case_singular}}
 
     def all(self, page: int, items_per_page: int, sort_type: str = 'asc', sort_by: str = 'id', start_date: str = None, end_date: str = None, first_field: str = None, second_field: str = None) -> Tuple[List[{{class_name_title_case_singular}}Response], int, int, int, int]:
         """
-        Retrieve all {{class_name_lower_case_singular}}s with pagination and optional date, first_field, and second field filters.
+        Retrieve all {{class_name_lower_case_plural}} with pagination and optional date, first_field, and second field filters.
 
         Args:
             page (int): The page number.
             items_per_page (int): The number of items per page.
             sort_type (str): The sort type ('asc' or 'desc').
             sort_by (str): The field to sort by ('created_at' or 'first_field').
             start_date (str): The start date for the filter (YYYY-MM-DD).
             end_date (str): The end date for the filter (YYYY-MM-DD).
             first_field (str): The first field filter.
             second_field (str): The second field filter.
 
         Returns:
-            Tuple[List[{{class_name_title_case_singular}}Response], int, int, int, int]: A tuple containing the list of {{class_name_lower_case_singular}} responses, the total number of {{class_name_lower_case_singular}}s, the last page number, the first item number, and the last item number.
+            Tuple[List[{{class_name_title_case_singular}}Response], int, int, int, int]: A tuple containing the list of {{class_name_lower_case_singular}} responses, the total number of {{class_name_lower_case_plural}}, the last page number, the first item number, and the last item number.
 
         Raises:
             HTTPException: If there is an internal server error.
         """
         try:
             offset = (page - 1) * items_per_page
 
             sort_field = self.get_sort_field(sort_by)
 
             query = self.build_query(sort_field, sort_type, start_date, end_date, first_field, second_field)
 
-            {{class_name_lower_case_singular}}s = query.offset(offset).limit(items_per_page).all()
+            {{class_name_lower_case_plural}} = query.offset(offset).limit(items_per_page).all()
 
             responses = [{{class_name_title_case_singular}}Response(
                 id={{class_name_lower_case_singular}}.id,
                 first_field={{class_name_lower_case_singular}}.first_field,
                 second_field={{class_name_lower_case_singular}}.second_field,
                 created_at={{class_name_lower_case_singular}}.created_at.strftime("%Y-%m-%d %H:%M:%S"),
                 updated_at={{class_name_lower_case_singular}}.updated_at.strftime("%Y-%m-%d %H:%M:%S"),
-            ) for {{class_name_lower_case_singular}} in {{class_name_lower_case_singular}}s]
+            ) for {{class_name_lower_case_singular}} in {{class_name_lower_case_plural}}]
 
-            total_{{class_name_lower_case_singular}}s = query.count()
-            last_page = (total_{{class_name_lower_case_singular}}s - 1) // items_per_page + 1
+            total_{{class_name_lower_case_plural}} = query.count()
+            last_page = (total_{{class_name_lower_case_plural}} - 1) // items_per_page + 1
             first_item = offset + 1
-            last_item = min(offset + items_per_page, total_{{class_name_lower_case_singular}}s)
+            last_item = min(offset + items_per_page, total_{{class_name_lower_case_plural}})
 
-            return responses, total_{{class_name_lower_case_singular}}s, last_page, first_item, last_item
+            return responses, total_{{class_name_lower_case_plural}}, last_page, first_item, last_item
 
         except DatabaseError:
             raise HTTPException(status_code=500, detail="Internal server error")
 
     def get_sort_field(self, sort_by: str):
             """
             Returns the corresponding sort field based on the given sort_by parameter.
@@ -109,26 +109,26 @@
             elif sort_by == 'id':
                 return {{class_name_title_case_singular}}.id
             else:
                 raise HTTPException(status_code=400, detail="Invalid sort_by field")
 
     def build_query(self, sort_field, sort_type, start_date, end_date, first_field, second_field):
         """
-        Builds a query to retrieve {{class_name_lower_case_singular}}s based on the provided parameters.
+        Builds a query to retrieve {{class_name_lower_case_plural}} based on the provided parameters.
 
         Args:
-            sort_field (str): The field to sort the {{class_name_lower_case_singular}}s by.
+            sort_field (str): The field to sort the {{class_name_lower_case_plural}} by.
             sort_type (str): The type of sorting, either 'asc' or 'desc'.
-            start_date (str): The start date for filtering {{class_name_lower_case_singular}}s.
-            end_date (str): The end date for filtering {{class_name_lower_case_singular}}s.
-            first_field (str): The first field to filter {{class_name_lower_case_singular}}s by.
-            second_field (str): The second_field to filter {{class_name_lower_case_singular}}s by.
+            start_date (str): The start date for filtering {{class_name_lower_case_plural}}.
+            end_date (str): The end date for filtering {{class_name_lower_case_plural}}.
+            first_field (str): The first field to filter {{class_name_lower_case_plural}} by.
+            second_field (str): The second_field to filter {{class_name_lower_case_plural}} by.
 
         Returns:
-            sqlalchemy.orm.query.Query: The query object for retrieving {{class_name_lower_case_singular}}s.
+            sqlalchemy.orm.query.Query: The query object for retrieving {{class_name_lower_case_plural}}.
         """
         query = self.db.query({{class_name_title_case_singular}})
 
         if sort_type == 'asc':
             query = query.order_by(sort_field.asc())
         elif sort_type == 'desc':
             query = query.order_by(sort_field.desc())
@@ -147,18 +147,18 @@
         if second_field:
             query = query.filter({{class_name_title_case_singular}}.second_field.like(f'%{second_field}%'))
 
         return query
 
     def total(self) -> int:
             """
-            Get the total number of {{class_name_lower_case_singular}}s.
+            Get the total number of {{class_name_lower_case_plural}}.
 
             Returns:
-                int: The total number of {{class_name_lower_case_singular}}s.
+                int: The total number of {{class_name_lower_case_plural}}.
             """
             return self.db.query({{class_name_title_case_singular}}).count()
 
     def find(self, id: int) -> {{class_name_title_case_singular}}Response:
         """
         Find a {{class_name_lower_case_singular}} by their ID and return the {{class_name_lower_case_singular}} response.
 
@@ -196,15 +196,14 @@
         try:
             existing = self.db.query({{class_name_title_case_singular}}).filter({{class_name_title_case_singular}}.second_field == {{class_name_lower_case_singular}}.second_field).first()
             if existing:
                 raise HTTPException(
                     status_code=422, detail="{{class_name_title_case_singular}} with this second_field already exists"
                 )
             data = {{class_name_lower_case_singular}}.dict(exclude_unset=True)
-            data["password"] = "hashed_" + data["password"]
             item = {{class_name_title_case_singular}}(**data)
             self.db.add(item)
             self.db.commit()
             self.db.refresh(item)
 
             item = self.db.query({{class_name_title_case_singular}}).filter({{class_name_title_case_singular}}.id == item.id).first()
             response_data = {
@@ -230,17 +229,16 @@
         Returns:
             {{class_name_title_case_singular}}UpdateResponse: The response data of the updated {{class_name_lower_case_singular}}.
         """
         try:
             item = self.get_by_id(id)
             data = {{class_name_lower_case_singular}}.dict(exclude_unset=True)
             if "password" in data:
-                data["password"] = "hashed_" + data["password"]
-            for key, value in data.items():
-                setattr(item, key, value)
+                for key, value in data.items():
+                    setattr(item, key, value)
             self.db.commit()
             self.db.refresh(item)
             response_data = {
                 "id": item.id,
                 "first_field": item.first_field,
                 "second_field": item.second_field,
                 "created_at": item.created_at.strftime("%Y-%m-%d %H:%M:%S"),
@@ -275,7 +273,33 @@
                     "created_at": item.created_at.strftime("%Y-%m-%d %H:%M:%S"),
                     "updated_at": item.updated_at.strftime("%Y-%m-%d %H:%M:%S"),
                 }
                 return response_data
             except DatabaseError as e:
                 logging.error(f"Error occurred while deleting {{class_name_lower_case_singular}}: {str(e)}")
                 raise HTTPException(status_code=500, detail="Internal server error")
+
+
+    def bulk_delete(self, ids: Union[int, List[int]]):
+        if isinstance(ids, int):
+            ids = [ids]
+
+        deleted_{{class_name_lower_case_plural}} = []
+
+        for id in ids:
+            item = self.get_by_id(id)
+            if item:
+                self.db.delete(item)
+                response_data = {
+                    "id": item.id,
+                    "first_field": item.first_field,
+                    "second_field": item.second_field,
+                    "created_at": item.created_at.strftime("%Y-%m-%d %H:%M:%S"),
+                    "updated_at": item.updated_at.strftime("%Y-%m-%d %H:%M:%S"),
+                }
+                deleted_{{class_name_lower_case_plural}}.append(response_data)
+
+        self.db.commit()
+
+        response_data = deleted_{{class_name_lower_case_plural}}
+
+        return response_data
```

### Comparing `python_spartan-0.2.5/python_spartan/stubs/service/elastic_search.stub` & `python_spartan-0.2.6/python_spartan/stubs/service/elastic_search.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/service/email.stub` & `python_spartan-0.2.6/python_spartan/stubs/service/email.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/python_spartan/stubs/service/queue.stub` & `python_spartan-0.2.6/python_spartan/stubs/service/queue.stub`

 * *Files identical despite different names*

### Comparing `python_spartan-0.2.5/PKG-INFO` & `python_spartan-0.2.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: python-spartan
-Version: 0.2.5
+Version: 0.2.6
 Summary: Spartan, often referred to as "The swiss army knife for serverless development," is a tool that simplifies the creation of serverless applications on popular cloud providers by generating Python code for classes and more. It streamlines your development process, saving you time and ensuring code consistency in your serverless projects.
 Author: nerdmonkey
 Author-email: sydel.palinlin@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (>=1.12.0,<2.0.0)
 Requires-Dist: faker (>=20.1.0,<21.0.0)
+Requires-Dist: inflect (>=7.2.1,<8.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: poetry (>=1.7.0,<2.0.0)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

