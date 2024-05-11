# Comparing `tmp/airfly-0.9.0.tar.gz` & `tmp/airfly-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airfly-0.9.0.tar", last modified: Sat Mar 23 12:20:54 2024, max compression
+gzip compressed data, was "airfly-1.0.0.tar", last modified: Sat May 11 15:18:48 2024, max compression
```

## Comparing `airfly-0.9.0.tar` & `airfly-1.0.0.tar`

### file list

```diff
@@ -1,647 +1,472 @@
--rw-r--r--   0        0        0     1062 2024-03-23 08:58:10.696397 airfly-0.9.0/LICENSE
--rw-r--r--   0        0        0     9754 2024-03-23 08:58:10.700398 airfly-0.9.0/README.md
--rw-r--r--   0        0        0      719 2024-03-23 12:20:54.119238 airfly-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      123 2024-03-23 08:58:10.708398 airfly-0.9.0/src/airfly/__init__.py
--rw-r--r--   0        0        0      441 2024-03-23 12:13:54.293047 airfly-0.9.0/src/airfly/_meta.py
--rw-r--r--   0        0        0      617 2024-03-23 08:58:10.708398 airfly-0.9.0/src/airfly/_vendor/__init__.py
--rw-r--r--   0        0        0       22 2024-03-23 11:48:43.898146 airfly-0.9.0/src/airfly/_vendor/airflow/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/__init__.py
--rw-r--r--   0        0        0      219 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/adls_to_gcs.py
--rw-r--r--   0        0        0      184 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/awsbatch_operator.py
--rw-r--r--   0        0        0      222 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/bigquery_operator.py
--rw-r--r--   0        0        0      231 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/bigquery_table_delete_operator.py
--rw-r--r--   0        0        0      229 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/bigquery_to_gcs.py
--rw-r--r--   0        0        0      239 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/cassandra_to_gcs.py
--rw-r--r--   0        0        0      456 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/dataflow_operator.py
--rw-r--r--   0        0        0     1557 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/dataproc_operator.py
--rw-r--r--   0        0        0      246 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/datastore_export_operator.py
--rw-r--r--   0        0        0      246 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/datastore_import_operator.py
--rw-r--r--   0        0        0      242 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/file_to_gcs.py
--rw-r--r--   0        0        0      908 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_bigtable_operator.py
--rw-r--r--   0        0        0      899 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_compute_operator.py
--rw-r--r--   0        0        0      409 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_container_operator.py
--rw-r--r--   0        0        0      559 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_dlp_operator.py
--rw-r--r--   0        0        0      368 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_function_operator.py
--rw-r--r--   0        0        0      754 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_natural_language_operator.py
--rw-r--r--   0        0        0      929 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_spanner_operator.py
--rw-r--r--   0        0        0      274 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_speech_to_text_operator.py
--rw-r--r--   0        0        0     1317 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_sql_operator.py
--rw-r--r--   0        0        0      259 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_text_to_speech_operator.py
--rw-r--r--   0        0        0     1712 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_transfer_operator.py
--rw-r--r--   0        0        0      240 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_translate_speech_operator.py
--rw-r--r--   0        0        0     1512 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcp_vision_operator.py
--rw-r--r--   0        0        0      388 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcs_acl_operator.py
--rw-r--r--   0        0        0      225 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcs_delete_operator.py
--rw-r--r--   0        0        0      244 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcs_download_operator.py
--rw-r--r--   0        0        0      219 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcs_list_operator.py
--rw-r--r--   0        0        0      229 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcs_operator.py
--rw-r--r--   0        0        0      235 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcs_to_bq.py
--rw-r--r--   0        0        0      230 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcs_to_gcs.py
--rw-r--r--   0        0        0      209 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/gcs_to_s3.py
--rw-r--r--   0        0        0      584 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/mlengine_operator.py
--rw-r--r--   0        0        0      223 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/mssql_to_gcs.py
--rw-r--r--   0        0        0      223 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/mysql_to_gcs.py
--rw-r--r--   0        0        0      218 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/oracle_to_oracle_transfer.py
--rw-r--r--   0        0        0      235 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/postgres_to_gcs_operator.py
--rw-r--r--   0        0        0      675 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/pubsub_operator.py
--rw-r--r--   0        0        0      227 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/sql_to_gcs.py
--rw-r--r--   0        0        0      219 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/vertica_to_hive.py
--rw-r--r--   0        0        0      217 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/operators/vertica_to_mysql.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/sensors/__init__.py
--rw-r--r--   0        0        0      223 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/sensors/bigquery_sensor.py
--rw-r--r--   0        0        0      288 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/sensors/gcp_transfer_sensor.py
--rw-r--r--   0        0        0      586 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/sensors/gcs_sensor.py
--rw-r--r--   0        0        0      263 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/contrib/sensors/hdfs_sensor.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/decorators/__init__.py
--rw-r--r--   0        0        0      359 2024-03-23 11:39:56.908920 airfly-0.9.0/src/airfly/_vendor/airflow/decorators/base.py
--rw-r--r--   0        0        0      387 2024-03-23 11:39:58.700968 airfly-0.9.0/src/airfly/_vendor/airflow/decorators/branch_external_python.py
--rw-r--r--   0        0        0      357 2024-03-23 11:39:59.132979 airfly-0.9.0/src/airfly/_vendor/airflow/decorators/branch_python.py
--rw-r--r--   0        0        0      398 2024-03-23 11:39:59.532990 airfly-0.9.0/src/airfly/_vendor/airflow/decorators/branch_virtualenv.py
--rw-r--r--   0        0        0      369 2024-03-23 11:40:00.001002 airfly-0.9.0/src/airfly/_vendor/airflow/decorators/external_python.py
--rw-r--r--   0        0        0      323 2024-03-23 11:39:57.832945 airfly-0.9.0/src/airfly/_vendor/airflow/decorators/python.py
--rw-r--r--   0        0        0      375 2024-03-23 11:40:00.421013 airfly-0.9.0/src/airfly/_vendor/airflow/decorators/python_virtualenv.py
--rw-r--r--   0        0        0      171 2024-03-23 11:40:01.249035 airfly-0.9.0/src/airfly/_vendor/airflow/decorators/sensor.py
--rw-r--r--   0        0        0      357 2024-03-23 11:40:01.685046 airfly-0.9.0/src/airfly/_vendor/airflow/decorators/short_circuit.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/example_dags/__init__.py
--rw-r--r--   0        0        0      167 2024-03-23 11:40:04.257114 airfly-0.9.0/src/airfly/_vendor/airflow/example_dags/example_dag_decorator.py
--rw-r--r--   0        0        0      226 2024-03-23 11:40:04.669125 airfly-0.9.0/src/airfly/_vendor/airflow/example_dags/example_dynamic_task_mapping_with_no_taskflow_operators.py
--rw-r--r--   0        0        0     1951 2024-03-23 11:40:08.105216 airfly-0.9.0/src/airfly/_vendor/airflow/example_dags/example_skip_dag.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/models/__init__.py
--rw-r--r--   0        0        0      234 2024-03-23 11:39:54.324852 airfly-0.9.0/src/airfly/_vendor/airflow/models/abstractoperator.py
--rw-r--r--   0        0        0       69 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/models/base.py
--rw-r--r--   0        0        0     1958 2024-03-23 11:39:54.804865 airfly-0.9.0/src/airfly/_vendor/airflow/models/baseoperator.py
--rw-r--r--   0        0        0      169 2024-03-23 11:39:55.216876 airfly-0.9.0/src/airfly/_vendor/airflow/models/skipmixin.py
--rw-r--r--   0        0        0      119 2024-03-23 11:39:53.892841 airfly-0.9.0/src/airfly/_vendor/airflow/models/taskmixin.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/__init__.py
--rw-r--r--   0        0        0      361 2024-03-23 11:40:02.093057 airfly-0.9.0/src/airfly/_vendor/airflow/operators/bash.py
--rw-r--r--   0        0        0     2081 2024-03-23 11:39:58.276956 airfly-0.9.0/src/airfly/_vendor/airflow/operators/branch.py
--rw-r--r--   0        0        0      449 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/check_operator.py
--rw-r--r--   0        0        0      460 2024-03-23 11:40:02.981080 airfly-0.9.0/src/airfly/_vendor/airflow/operators/datetime.py
--rw-r--r--   0        0        0      156 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/dummy.py
--rw-r--r--   0        0        0      426 2024-03-23 11:40:03.813102 airfly-0.9.0/src/airfly/_vendor/airflow/operators/email.py
--rw-r--r--   0        0        0     1947 2024-03-23 11:40:02.549069 airfly-0.9.0/src/airfly/_vendor/airflow/operators/empty.py
--rw-r--r--   0        0        0      323 2024-03-23 11:40:08.965238 airfly-0.9.0/src/airfly/_vendor/airflow/operators/generic_transfer.py
--rw-r--r--   0        0        0      219 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/google_api_to_s3_transfer.py
--rw-r--r--   0        0        0      212 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/hive_to_druid.py
--rw-r--r--   0        0        0      211 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/hive_to_mysql.py
--rw-r--r--   0        0        0     1961 2024-03-23 11:40:05.561149 airfly-0.9.0/src/airfly/_vendor/airflow/operators/latest_only.py
--rw-r--r--   0        0        0      211 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/mssql_to_hive.py
--rw-r--r--   0        0        0      211 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/mysql_to_hive.py
--rw-r--r--   0        0        0      368 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/presto_check_operator.py
--rw-r--r--   0        0        0      213 2024-03-23 08:58:10.724398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/presto_to_mysql.py
--rw-r--r--   0        0        0     3469 2024-03-23 11:39:57.396933 airfly-0.9.0/src/airfly/_vendor/airflow/operators/python.py
--rw-r--r--   0        0        0      214 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/redshift_to_s3_operator.py
--rw-r--r--   0        0        0      199 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/s3_to_hive_operator.py
--rw-r--r--   0        0        0      214 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/s3_to_redshift_operator.py
--rw-r--r--   0        0        0     1543 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/sql.py
--rw-r--r--   0        0        0      164 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/operators/sql_branch_operator.py
--rw-r--r--   0        0        0      287 2024-03-23 11:39:56.072898 airfly-0.9.0/src/airfly/_vendor/airflow/operators/subdag.py
--rw-r--r--   0        0        0      474 2024-03-23 11:40:08.549227 airfly-0.9.0/src/airfly/_vendor/airflow/operators/trigger_dagrun.py
--rw-r--r--   0        0        0      404 2024-03-23 11:40:03.381091 airfly-0.9.0/src/airfly/_vendor/airflow/operators/weekday.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/airbyte/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/airbyte/operators/__init__.py
--rw-r--r--   0        0        0      330 2024-03-23 11:40:09.393249 airfly-0.9.0/src/airfly/_vendor/airflow/providers/airbyte/operators/airbyte.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/airbyte/sensors/__init__.py
--rw-r--r--   0        0        0      254 2024-03-23 11:40:09.817261 airfly-0.9.0/src/airfly/_vendor/airflow/providers/airbyte/sensors/airbyte.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/alibaba/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/operators/__init__.py
--rw-r--r--   0        0        0     1055 2024-03-23 11:40:10.245272 airfly-0.9.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/operators/analyticdb_spark.py
--rw-r--r--   0        0        0      919 2024-03-23 11:40:10.701284 airfly-0.9.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/operators/oss.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/sensors/__init__.py
--rw-r--r--   0        0        0      232 2024-03-23 11:40:11.145296 airfly-0.9.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/sensors/analyticdb_spark.py
--rw-r--r--   0        0        0      251 2024-03-23 11:40:11.561307 airfly-0.9.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/sensors/oss_key.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0        0        0     1293 2024-03-23 11:40:13.261351 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0        0        0      542 2024-03-23 11:40:13.689363 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0        0        0      380 2024-03-23 11:40:12.813340 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/base_aws.py
--rw-r--r--   0        0        0     1237 2024-03-23 11:40:14.125374 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0        0        0      419 2024-03-23 11:40:14.553386 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0        0        0      722 2024-03-23 11:40:14.985397 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0        0        0      889 2024-03-23 11:40:15.409408 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0        0        0     1389 2024-03-23 11:40:15.877420 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0        0        0     1727 2024-03-23 11:40:16.325432 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0        0        0     4513 2024-03-23 11:40:16.833446 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0        0        0      395 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/emr_add_steps.py
--rw-r--r--   0        0        0      335 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/emr_create_job_flow.py
--rw-r--r--   0        0        0      207 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/emr_terminate_job_flow.py
--rw-r--r--   0        0        0      741 2024-03-23 11:40:17.273457 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/eventbridge.py
--rw-r--r--   0        0        0      405 2024-03-23 11:40:17.697468 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0        0        0      747 2024-03-23 11:40:18.141480 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0        0        0      310 2024-03-23 11:40:18.569491 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0        0        0      284 2024-03-23 11:40:18.977502 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/glue_databrew.py
--rw-r--r--   0        0        0      768 2024-03-23 11:40:19.409513 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0        0        0      523 2024-03-23 11:40:19.841525 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/neptune.py
--rw-r--r--   0        0        0      333 2024-03-23 11:40:20.253536 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0        0        0     2863 2024-03-23 11:40:20.725548 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0        0        0     2711 2024-03-23 11:40:21.201561 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0        0        0      552 2024-03-23 11:40:21.649572 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0        0        0     2275 2024-03-23 11:40:22.101584 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0        0        0      486 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/s3_copy_object.py
--rw-r--r--   0        0        0      334 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/s3_delete_objects.py
--rw-r--r--   0        0        0      539 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/s3_file_transform.py
--rw-r--r--   0        0        0      276 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/s3_list.py
--rw-r--r--   0        0        0     4301 2024-03-23 11:40:22.613598 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0        0        0      197 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sagemaker_base.py
--rw-r--r--   0        0        0      364 2024-03-23 08:58:10.728398 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sagemaker_endpoint.py
--rw-r--r--   0        0        0      237 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sagemaker_endpoint_config.py
--rw-r--r--   0        0        0      230 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sagemaker_model.py
--rw-r--r--   0        0        0      429 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sagemaker_training.py
--rw-r--r--   0        0        0      344 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sagemaker_transform.py
--rw-r--r--   0        0        0      341 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sagemaker_tuning.py
--rw-r--r--   0        0        0      292 2024-03-23 11:40:23.049609 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0        0        0      333 2024-03-23 11:40:23.477621 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0        0        0      468 2024-03-23 11:40:23.897632 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/step_function.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0        0        0      248 2024-03-23 11:40:24.785655 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0        0        0      383 2024-03-23 11:40:24.357644 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/base_aws.py
--rw-r--r--   0        0        0      623 2024-03-23 11:40:25.229667 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0        0        0      348 2024-03-23 11:40:25.633678 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0        0        0      356 2024-03-23 11:40:26.065689 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0        0        0      390 2024-03-23 11:40:26.501700 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-r--r--   0        0        0      291 2024-03-23 11:40:26.905711 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0        0        0      757 2024-03-23 11:40:27.341723 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0        0        0      652 2024-03-23 11:40:27.777734 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0        0        0     1280 2024-03-23 11:40:28.225746 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0        0        0      175 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/emr_base.py
--rw-r--r--   0        0        0      325 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/emr_job_flow.py
--rw-r--r--   0        0        0      341 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/emr_step.py
--rw-r--r--   0        0        0      260 2024-03-23 11:40:28.657757 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0        0        0      240 2024-03-23 11:40:29.077768 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0        0        0      342 2024-03-23 11:40:29.477779 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0        0        0      210 2024-03-23 11:40:29.901790 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0        0        0      265 2024-03-23 11:40:30.313801 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0        0        0      217 2024-03-23 11:40:30.721812 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0        0        0      706 2024-03-23 11:40:31.157823 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0        0        0      241 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/redshift.py
--rw-r--r--   0        0        0      268 2024-03-23 11:40:31.557834 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0        0        0      687 2024-03-23 11:40:31.989845 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0        0        0      317 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/s3_key.py
--rw-r--r--   0        0        0      286 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/s3_prefix.py
--rw-r--r--   0        0        0      718 2024-03-23 11:40:32.421856 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0        0        0      181 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/sagemaker_base.py
--rw-r--r--   0        0        0      232 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/sagemaker_endpoint.py
--rw-r--r--   0        0        0      251 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/sagemaker_training.py
--rw-r--r--   0        0        0      225 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/sagemaker_transform.py
--rw-r--r--   0        0        0      222 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/sagemaker_tuning.py
--rw-r--r--   0        0        0      494 2024-03-23 11:40:32.881868 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0        0        0      206 2024-03-23 11:40:33.297879 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/step_function.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0        0        0      280 2024-03-23 11:40:33.725891 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0        0        0      512 2024-03-23 11:40:34.157902 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0        0        0      430 2024-03-23 11:40:34.577913 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0        0        0      434 2024-03-23 11:40:35.001924 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0        0        0      626 2024-03-23 11:40:35.437936 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0        0        0      375 2024-03-23 11:40:35.865947 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0        0        0      704 2024-03-23 11:40:36.297958 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0        0        0      502 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0        0        0      681 2024-03-23 11:40:36.749970 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/http_to_s3.py
--rw-r--r--   0        0        0      395 2024-03-23 11:40:37.157981 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0        0        0      379 2024-03-23 11:40:37.589993 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0        0        0      451 2024-03-23 11:40:38.006003 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0        0        0      566 2024-03-23 11:40:38.426015 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0        0        0      269 2024-03-23 11:40:38.854026 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0        0        0      507 2024-03-23 11:40:39.286037 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0        0        0      264 2024-03-23 11:40:39.702048 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0        0        0      428 2024-03-23 11:40:40.154060 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0        0        0      521 2024-03-23 11:40:40.602072 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0        0        0      282 2024-03-23 11:40:41.010083 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0        0        0      548 2024-03-23 11:40:41.450094 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/sql_to_s3.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0        0        0      128 2024-03-23 11:40:12.389328 airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/utils/mixins.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/cassandra/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/cassandra/sensors/__init__.py
--rw-r--r--   0        0        0      240 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/cassandra/sensors/record.py
--rw-r--r--   0        0        0      205 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/cassandra/sensors/table.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/druid/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/druid/operators/__init__.py
--rw-r--r--   0        0        0      260 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/druid/operators/druid.py
--rw-r--r--   0        0        0      186 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/druid/operators/druid_check.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/druid/transfers/__init__.py
--rw-r--r--   0        0        0      798 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/druid/transfers/hive_to_druid.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hdfs/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hdfs/sensors/__init__.py
--rw-r--r--   0        0        0      529 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hdfs/sensors/hdfs.py
--rw-r--r--   0        0        0      199 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hdfs/sensors/web_hdfs.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/operators/__init__.py
--rw-r--r--   0        0        0      554 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/operators/hive.py
--rw-r--r--   0        0        0      559 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/operators/hive_stats.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/sensors/__init__.py
--rw-r--r--   0        0        0      292 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/sensors/hive_partition.py
--rw-r--r--   0        0        0      230 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/sensors/metastore_partition.py
--rw-r--r--   0        0        0      280 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/sensors/named_hive_partition.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/transfers/__init__.py
--rw-r--r--   0        0        0      429 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/transfers/hive_to_mysql.py
--rw-r--r--   0        0        0      256 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/transfers/hive_to_samba.py
--rw-r--r--   0        0        0      414 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/transfers/mssql_to_hive.py
--rw-r--r--   0        0        0      524 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/transfers/mysql_to_hive.py
--rw-r--r--   0        0        0      645 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/transfers/s3_to_hive.py
--rw-r--r--   0        0        0      351 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/transfers/vertica_to_hive.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/pig/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/pig/operators/__init__.py
--rw-r--r--   0        0        0      269 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/pig/operators/pig.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/spark/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/spark/operators/__init__.py
--rw-r--r--   0        0        0     1426 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/spark/operators/spark_jdbc.py
--rw-r--r--   0        0        0      641 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/spark/operators/spark_sql.py
--rw-r--r--   0        0        0     1317 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/spark/operators/spark_submit.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/sqoop/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/sqoop/operators/__init__.py
--rw-r--r--   0        0        0     1552 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/sqoop/operators/sqoop.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/arangodb/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/arangodb/operators/__init__.py
--rw-r--r--   0        0        0      230 2024-03-23 11:40:41.882106 airfly-0.9.0/src/airfly/_vendor/airflow/providers/arangodb/operators/arangodb.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/arangodb/sensors/__init__.py
--rw-r--r--   0        0        0      193 2024-03-23 11:40:42.282116 airfly-0.9.0/src/airfly/_vendor/airflow/providers/arangodb/sensors/arangodb.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/asana/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/asana/operators/__init__.py
--rw-r--r--   0        0        0      540 2024-03-23 11:40:42.710127 airfly-0.9.0/src/airfly/_vendor/airflow/providers/asana/operators/asana_tasks.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/celery/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/celery/sensors/__init__.py
--rw-r--r--   0        0        0      213 2024-03-23 11:40:43.134139 airfly-0.9.0/src/airfly/_vendor/airflow/providers/celery/sensors/celery_queue.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/cncf/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/cncf/kubernetes/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.736399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0        0        0     2806 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/cohere/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/cohere/operators/__init__.py
--rw-r--r--   0        0        0      266 2024-03-23 11:40:43.546149 airfly-0.9.0/src/airfly/_vendor/airflow/providers/cohere/operators/embedding.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/common/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/common/sql/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/common/sql/operators/__init__.py
--rw-r--r--   0        0        0     1625 2024-03-23 11:40:44.922186 airfly-0.9.0/src/airfly/_vendor/airflow/providers/common/sql/operators/sql.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/operators/__init__.py
--rw-r--r--   0        0        0     2552 2024-03-23 11:40:44.022162 airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks.py
--rw-r--r--   0        0        0      876 2024-03-23 11:40:44.474174 airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks_repos.py
--rw-r--r--   0        0        0     1395 2024-03-23 11:40:45.350197 airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks_sql.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/sensors/__init__.py
--rw-r--r--   0        0        0      539 2024-03-23 11:40:45.786208 airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/sensors/databricks_partition.py
--rw-r--r--   0        0        0      489 2024-03-23 11:40:46.234220 airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/sensors/databricks_sql.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/datadog/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/datadog/sensors/__init__.py
--rw-r--r--   0        0        0      385 2024-03-23 11:40:46.642231 airfly-0.9.0/src/airfly/_vendor/airflow/providers/datadog/sensors/datadog.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/dingding/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/dingding/operators/__init__.py
--rw-r--r--   0        0        0      289 2024-03-23 11:40:47.070242 airfly-0.9.0/src/airfly/_vendor/airflow/providers/dingding/operators/dingding.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/discord/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/discord/operators/__init__.py
--rw-r--r--   0        0        0      347 2024-03-23 11:40:47.926265 airfly-0.9.0/src/airfly/_vendor/airflow/providers/discord/operators/discord_webhook.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/docker/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/docker/decorators/__init__.py
--rw-r--r--   0        0        0      343 2024-03-23 11:40:48.798288 airfly-0.9.0/src/airfly/_vendor/airflow/providers/docker/decorators/docker.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/docker/operators/__init__.py
--rw-r--r--   0        0        0     1593 2024-03-23 11:40:48.374277 airfly-0.9.0/src/airfly/_vendor/airflow/providers/docker/operators/docker.py
--rw-r--r--   0        0        0      481 2024-03-23 11:40:49.202298 airfly-0.9.0/src/airfly/_vendor/airflow/providers/docker/operators/docker_swarm.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/exasol/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/exasol/operators/__init__.py
--rw-r--r--   0        0        0      267 2024-03-23 11:40:49.630310 airfly-0.9.0/src/airfly/_vendor/airflow/providers/exasol/operators/exasol.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/ftp/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/ftp/operators/__init__.py
--rw-r--r--   0        0        0      532 2024-03-23 11:40:50.062321 airfly-0.9.0/src/airfly/_vendor/airflow/providers/ftp/operators/ftp.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/ftp/sensors/__init__.py
--rw-r--r--   0        0        0      331 2024-03-23 11:40:50.478331 airfly-0.9.0/src/airfly/_vendor/airflow/providers/ftp/sensors/ftp.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/github/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/github/operators/__init__.py
--rw-r--r--   0        0        0      277 2024-03-23 11:40:50.906341 airfly-0.9.0/src/airfly/_vendor/airflow/providers/github/operators/github.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/github/sensors/__init__.py
--rw-r--r--   0        0        0      563 2024-03-23 11:40:51.338352 airfly-0.9.0/src/airfly/_vendor/airflow/providers/github/sensors/github.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/ads/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/ads/operators/__init__.py
--rw-r--r--   0        0        0      358 2024-03-23 11:40:51.758362 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/ads/operators/ads.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/ads/transfers/__init__.py
--rw-r--r--   0        0        0      437 2024-03-23 11:40:52.182373 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/ads/transfers/ads_to_gcs.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/__init__.py
--rw-r--r--   0        0        0     4425 2024-03-23 11:40:53.566406 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/automl.py
--rw-r--r--   0        0        0     7146 2024-03-23 11:40:54.150421 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigquery.py
--rw-r--r--   0        0        0     1337 2024-03-23 11:40:54.586431 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigquery_dts.py
--rw-r--r--   0        0        0     2226 2024-03-23 11:40:55.042442 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigtable.py
--rw-r--r--   0        0        0     1957 2024-03-23 11:40:53.058394 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_base.py
--rw-r--r--   0        0        0     1194 2024-03-23 11:40:55.490454 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_batch.py
--rw-r--r--   0        0        0     3913 2024-03-23 11:40:55.990466 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_build.py
--rw-r--r--   0        0        0     2461 2024-03-23 11:40:56.462477 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_composer.py
--rw-r--r--   0        0        0     6664 2024-03-23 11:40:56.994490 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_memorystore.py
--rw-r--r--   0        0        0     1346 2024-03-23 11:40:57.442501 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_run.py
--rw-r--r--   0        0        0     2934 2024-03-23 11:40:57.914513 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_sql.py
--rw-r--r--   0        0        0     3106 2024-03-23 11:40:58.406525 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_storage_transfer_service.py
--rw-r--r--   0        0        0     4766 2024-03-23 11:40:58.910537 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/compute.py
--rw-r--r--   0        0        0     8132 2024-03-23 11:40:59.494551 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datacatalog.py
--rw-r--r--   0        0        0     2087 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataflow.py
--rw-r--r--   0        0        0     5491 2024-03-23 11:41:00.054565 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataform.py
--rw-r--r--   0        0        0     3256 2024-03-23 11:41:00.534577 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datafusion.py
--rw-r--r--   0        0        0      518 2024-03-23 11:41:00.954587 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datapipeline.py
--rw-r--r--   0        0        0     8061 2024-03-23 11:41:01.570602 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataplex.py
--rw-r--r--   0        0        0     1107 2024-03-23 11:41:01.994613 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataprep.py
--rw-r--r--   0        0        0     8001 2024-03-23 11:41:02.598627 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataproc.py
--rw-r--r--   0        0        0     4105 2024-03-23 11:41:03.090639 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataproc_metastore.py
--rw-r--r--   0        0        0     2225 2024-03-23 11:41:03.538650 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datastore.py
--rw-r--r--   0        0        0    11576 2024-03-23 11:41:04.170666 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dlp.py
--rw-r--r--   0        0        0      923 2024-03-23 11:41:04.602676 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/functions.py
--rw-r--r--   0        0        0     2849 2024-03-23 11:41:05.066688 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/gcs.py
--rw-r--r--   0        0        0      999 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/kubernetes_engine.py
--rw-r--r--   0        0        0      229 2024-03-23 11:41:05.494698 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/life_sciences.py
--rw-r--r--   0        0        0      411 2024-03-23 11:41:05.926709 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/looker.py
--rw-r--r--   0        0        0     1039 2024-03-23 11:41:06.338719 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/mlengine.py
--rw-r--r--   0        0        0     1386 2024-03-23 11:41:06.802730 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/natural_language.py
--rw-r--r--   0        0        0     2675 2024-03-23 11:41:07.270742 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/pubsub.py
--rw-r--r--   0        0        0     1635 2024-03-23 11:41:07.722753 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/spanner.py
--rw-r--r--   0        0        0      461 2024-03-23 11:41:08.138763 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/speech_to_text.py
--rw-r--r--   0        0        0     3407 2024-03-23 11:41:08.634775 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/stackdriver.py
--rw-r--r--   0        0        0     4488 2024-03-23 11:41:09.150788 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/tasks.py
--rw-r--r--   0        0        0      571 2024-03-23 11:41:09.590798 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/text_to_speech.py
--rw-r--r--   0        0        0      419 2024-03-23 11:41:10.030809 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/translate.py
--rw-r--r--   0        0        0      482 2024-03-23 11:41:10.438819 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/translate_speech.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/__init__.py
--rw-r--r--   0        0        0     4846 2024-03-23 11:41:10.970832 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/auto_ml.py
--rw-r--r--   0        0        0     2216 2024-03-23 11:41:11.446844 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/batch_prediction_job.py
--rw-r--r--   0        0        0     3758 2024-03-23 11:41:11.946856 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/custom_job.py
--rw-r--r--   0        0        0     2569 2024-03-23 11:41:12.426868 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/dataset.py
--rw-r--r--   0        0        0     2648 2024-03-23 11:41:12.902880 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/endpoint_service.py
--rw-r--r--   0        0        0     2326 2024-03-23 11:41:13.366891 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/hyperparameter_tuning_job.py
--rw-r--r--   0        0        0     3446 2024-03-23 11:41:13.850903 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/model_service.py
--rw-r--r--   0        0        0     1844 2024-03-23 11:41:14.290913 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/pipeline_job.py
--rw-r--r--   0        0        0     1308 2024-03-23 11:41:14.738925 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/video_intelligence.py
--rw-r--r--   0        0        0     5923 2024-03-23 11:41:15.278938 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vision.py
--rw-r--r--   0        0        0     3270 2024-03-23 11:41:15.766950 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/workflows.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/__init__.py
--rw-r--r--   0        0        0      768 2024-03-23 11:41:16.218961 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/bigquery.py
--rw-r--r--   0        0        0      562 2024-03-23 11:41:16.654971 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/bigquery_dts.py
--rw-r--r--   0        0        0      468 2024-03-23 11:41:17.074982 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/bigtable.py
--rw-r--r--   0        0        0      178 2024-03-23 11:41:17.494992 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/cloud_composer.py
--rw-r--r--   0        0        0      344 2024-03-23 11:41:17.927003 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/cloud_storage_transfer_service.py
--rw-r--r--   0        0        0      437 2024-03-23 11:41:18.347013 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataform.py
--rw-r--r--   0        0        0      477 2024-03-23 11:41:18.783024 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/datafusion.py
--rw-r--r--   0        0        0     1238 2024-03-23 11:41:19.235035 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataplex.py
--rw-r--r--   0        0        0      229 2024-03-23 11:41:19.635044 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataprep.py
--rw-r--r--   0        0        0      454 2024-03-23 11:41:20.063055 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataproc.py
--rw-r--r--   0        0        0      336 2024-03-23 11:41:20.491066 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataproc_metastore.py
--rw-r--r--   0        0        0     1176 2024-03-23 11:41:20.923076 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/gcs.py
--rw-r--r--   0        0        0      247 2024-03-23 11:41:21.339086 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/looker.py
--rw-r--r--   0        0        0      457 2024-03-23 11:41:21.767097 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/pubsub.py
--rw-r--r--   0        0        0      314 2024-03-23 11:40:52.622383 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/tasks.py
--rw-r--r--   0        0        0      549 2024-03-23 11:41:22.191107 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/workflows.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/__init__.py
--rw-r--r--   0        0        0      556 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/adls_to_gcs.py
--rw-r--r--   0        0        0      491 2024-03-23 11:41:22.631118 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_bigquery.py
--rw-r--r--   0        0        0      674 2024-03-23 11:41:23.075129 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_gcs.py
--rw-r--r--   0        0        0      368 2024-03-23 11:41:23.923150 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_mysql.py
--rw-r--r--   0        0        0      281 2024-03-23 11:41:24.363160 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_postgres.py
--rw-r--r--   0        0        0      495 2024-03-23 11:41:23.491139 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_sql.py
--rw-r--r--   0        0        0      852 2024-03-23 11:41:24.787171 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/calendar_to_gcs.py
--rw-r--r--   0        0        0      555 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/cassandra_to_gcs.py
--rw-r--r--   0        0        0      456 2024-03-23 11:41:25.223182 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/facebook_ads_to_gcs.py
--rw-r--r--   0        0        0     1335 2024-03-23 11:41:25.675193 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_bigquery.py
--rw-r--r--   0        0        0      642 2024-03-23 11:41:26.103203 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_gcs.py
--rw-r--r--   0        0        0      368 2024-03-23 11:41:26.523213 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_local.py
--rw-r--r--   0        0        0      391 2024-03-23 11:41:26.951224 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_sftp.py
--rw-r--r--   0        0        0      357 2024-03-23 11:41:27.379234 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gdrive_to_gcs.py
--rw-r--r--   0        0        0      329 2024-03-23 11:41:27.799245 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gdrive_to_local.py
--rw-r--r--   0        0        0      342 2024-03-23 11:41:28.231255 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/local_to_gcs.py
--rw-r--r--   0        0        0      229 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/mssql_to_gcs.py
--rw-r--r--   0        0        0      254 2024-03-23 11:41:29.083276 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/mysql_to_gcs.py
--rw-r--r--   0        0        0      256 2024-03-23 11:41:29.515287 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/oracle_to_gcs.py
--rw-r--r--   0        0        0      302 2024-03-23 11:41:29.915297 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/postgres_to_gcs.py
--rw-r--r--   0        0        0      228 2024-03-23 11:41:30.339307 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/presto_to_gcs.py
--rw-r--r--   0        0        0      512 2024-03-23 11:41:30.779318 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/s3_to_gcs.py
--rw-r--r--   0        0        0      437 2024-03-23 11:41:31.187328 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/salesforce_to_gcs.py
--rw-r--r--   0        0        0      428 2024-03-23 11:41:31.619338 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/sftp_to_gcs.py
--rw-r--r--   0        0        0      364 2024-03-23 11:41:32.055349 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/sheets_to_gcs.py
--rw-r--r--   0        0        0      704 2024-03-23 11:41:28.663266 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/sql_to_gcs.py
--rw-r--r--   0        0        0      226 2024-03-23 11:41:32.467359 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/trino_to_gcs.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/firebase/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/firebase/operators/__init__.py
--rw-r--r--   0        0        0      339 2024-03-23 11:41:32.895370 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/firebase/operators/firestore.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/__init__.py
--rw-r--r--   0        0        0      772 2024-03-23 11:41:33.343381 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/analytics.py
--rw-r--r--   0        0        0     2388 2024-03-23 11:41:33.803392 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/analytics_admin.py
--rw-r--r--   0        0        0     2025 2024-03-23 11:41:34.251403 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/campaign_manager.py
--rw-r--r--   0        0        0     2228 2024-03-23 11:41:34.715414 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/display_video.py
--rw-r--r--   0        0        0      632 2024-03-23 11:41:35.147425 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/search_ads.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/sensors/__init__.py
--rw-r--r--   0        0        0      405 2024-03-23 11:41:35.579436 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/sensors/campaign_manager.py
--rw-r--r--   0        0        0      622 2024-03-23 11:41:35.999446 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/sensors/display_video.py
--rw-r--r--   0        0        0      358 2024-03-23 11:41:36.435457 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/sensors/search_ads.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/suite/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/suite/operators/__init__.py
--rw-r--r--   0        0        0      312 2024-03-23 11:41:36.839467 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/suite/operators/sheets.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/suite/sensors/__init__.py
--rw-r--r--   0        0        0      345 2024-03-23 11:41:37.271477 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/suite/sensors/drive.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/suite/transfers/__init__.py
--rw-r--r--   0        0        0      379 2024-03-23 11:41:37.707488 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/suite/transfers/gcs_to_gdrive.py
--rw-r--r--   0        0        0      337 2024-03-23 11:41:38.131498 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/suite/transfers/gcs_to_sheets.py
--rw-r--r--   0        0        0      506 2024-03-23 11:41:38.559509 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/suite/transfers/local_to_drive.py
--rw-r--r--   0        0        0      461 2024-03-23 11:41:39.015520 airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/suite/transfers/sql_to_sheets.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/grpc/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/grpc/operators/__init__.py
--rw-r--r--   0        0        0      418 2024-03-23 11:41:39.499532 airfly-0.9.0/src/airfly/_vendor/airflow/providers/grpc/operators/grpc.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/http/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/http/operators/__init__.py
--rw-r--r--   0        0        0      749 2024-03-23 11:40:47.514254 airfly-0.9.0/src/airfly/_vendor/airflow/providers/http/operators/http.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.740399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/http/sensors/__init__.py
--rw-r--r--   0        0        0      587 2024-03-23 11:41:40.023545 airfly-0.9.0/src/airfly/_vendor/airflow/providers/http/sensors/http.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/imap/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/imap/sensors/__init__.py
--rw-r--r--   0        0        0      289 2024-03-23 11:41:40.495556 airfly-0.9.0/src/airfly/_vendor/airflow/providers/imap/sensors/imap_attachment.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/influxdb/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/influxdb/operators/__init__.py
--rw-r--r--   0        0        0      193 2024-03-23 11:41:40.931567 airfly-0.9.0/src/airfly/_vendor/airflow/providers/influxdb/operators/influxdb.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jdbc/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jdbc/operators/__init__.py
--rw-r--r--   0        0        0      201 2024-03-23 11:41:41.359578 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jdbc/operators/jdbc.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jenkins/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jenkins/operators/__init__.py
--rw-r--r--   0        0        0      351 2024-03-23 11:41:41.791588 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jenkins/operators/jenkins_job_trigger.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jenkins/sensors/__init__.py
--rw-r--r--   0        0        0      283 2024-03-23 11:41:42.227599 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jenkins/sensors/jenkins.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jira/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jira/operators/__init__.py
--rw-r--r--   0        0        0      382 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jira/operators/jira.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jira/sensors/__init__.py
--rw-r--r--   0        0        0      574 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/jira/sensors/jira.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/operators/__init__.py
--rw-r--r--   0        0        0      217 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/operators/adls_list.py
--rw-r--r--   0        0        0     1054 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/operators/azure_container_instances.py
--rw-r--r--   0        0        0      272 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/operators/azure_cosmos.py
--rw-r--r--   0        0        0      311 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/sensors/__init__.py
--rw-r--r--   0        0        0      271 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/sensors/azure_cosmos.py
--rw-r--r--   0        0        0      438 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/sensors/wasb.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/transfers/__init__.py
--rw-r--r--   0        0        0      293 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/transfers/file_to_wasb.py
--rw-r--r--   0        0        0      419 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/mssql/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/mssql/operators/__init__.py
--rw-r--r--   0        0        0      328 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/mssql/operators/mssql.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/winrm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/winrm/operators/__init__.py
--rw-r--r--   0        0        0      471 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/microsoft/winrm/operators/winrm.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/mongo/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/mongo/sensors/__init__.py
--rw-r--r--   0        0        0      238 2024-03-23 11:41:42.655609 airfly-0.9.0/src/airfly/_vendor/airflow/providers/mongo/sensors/mongo.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/mysql/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/mysql/operators/__init__.py
--rw-r--r--   0        0        0      202 2024-03-23 11:41:43.079620 airfly-0.9.0/src/airfly/_vendor/airflow/providers/mysql/operators/mysql.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/mysql/transfers/__init__.py
--rw-r--r--   0        0        0      280 2024-03-23 11:41:43.515631 airfly-0.9.0/src/airfly/_vendor/airflow/providers/mysql/transfers/presto_to_mysql.py
--rw-r--r--   0        0        0      363 2024-03-23 11:41:43.939641 airfly-0.9.0/src/airfly/_vendor/airflow/providers/mysql/transfers/s3_to_mysql.py
--rw-r--r--   0        0        0      278 2024-03-23 11:41:44.371652 airfly-0.9.0/src/airfly/_vendor/airflow/providers/mysql/transfers/trino_to_mysql.py
--rw-r--r--   0        0        0      341 2024-03-23 11:41:44.823663 airfly-0.9.0/src/airfly/_vendor/airflow/providers/mysql/transfers/vertica_to_mysql.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/neo4j/operators/__init__.py
--rw-r--r--   0        0        0      241 2024-03-23 11:41:45.251673 airfly-0.9.0/src/airfly/_vendor/airflow/providers/neo4j/operators/neo4j.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/openai/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/openai/operators/__init__.py
--rw-r--r--   0        0        0      293 2024-03-23 11:41:45.707685 airfly-0.9.0/src/airfly/_vendor/airflow/providers/openai/operators/openai.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/opensearch/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/opensearch/operators/__init__.py
--rw-r--r--   0        0        0      636 2024-03-23 11:41:46.175696 airfly-0.9.0/src/airfly/_vendor/airflow/providers/opensearch/operators/opensearch.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/opsgenie/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/opsgenie/operators/__init__.py
--rw-r--r--   0        0        0      971 2024-03-23 11:41:46.643708 airfly-0.9.0/src/airfly/_vendor/airflow/providers/opsgenie/operators/opsgenie.py
--rw-r--r--   0        0        0      771 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/opsgenie/operators/opsgenie_alert.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/oracle/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/oracle/operators/__init__.py
--rw-r--r--   0        0        0      408 2024-03-23 11:41:47.095719 airfly-0.9.0/src/airfly/_vendor/airflow/providers/oracle/operators/oracle.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/oracle/transfers/__init__.py
--rw-r--r--   0        0        0      337 2024-03-23 11:41:47.531729 airfly-0.9.0/src/airfly/_vendor/airflow/providers/oracle/transfers/oracle_to_oracle.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/papermill/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/papermill/operators/__init__.py
--rw-r--r--   0        0        0      353 2024-03-23 11:41:47.967740 airfly-0.9.0/src/airfly/_vendor/airflow/providers/papermill/operators/papermill.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/pgvector/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/pgvector/operators/__init__.py
--rw-r--r--   0        0        0      211 2024-03-23 11:41:48.431752 airfly-0.9.0/src/airfly/_vendor/airflow/providers/pgvector/operators/pgvector.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/pinecone/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/pinecone/operators/__init__.py
--rw-r--r--   0        0        0      313 2024-03-23 11:41:48.883763 airfly-0.9.0/src/airfly/_vendor/airflow/providers/pinecone/operators/pinecone.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/postgres/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/postgres/operators/__init__.py
--rw-r--r--   0        0        0      205 2024-03-23 11:41:49.351774 airfly-0.9.0/src/airfly/_vendor/airflow/providers/postgres/operators/postgres.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/presto/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/presto/transfers/__init__.py
--rw-r--r--   0        0        0      404 2024-03-23 11:41:49.799785 airfly-0.9.0/src/airfly/_vendor/airflow/providers/presto/transfers/gcs_to_presto.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/qubole/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/qubole/operators/__init__.py
--rw-r--r--   0        0        0      174 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/qubole/operators/qubole.py
--rw-r--r--   0        0        0      701 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/qubole/operators/qubole_check.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/qubole/sensors/__init__.py
--rw-r--r--   0        0        0      299 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/qubole/sensors/qubole.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/redis/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/redis/operators/__init__.py
--rw-r--r--   0        0        0      217 2024-03-23 11:41:50.239796 airfly-0.9.0/src/airfly/_vendor/airflow/providers/redis/operators/redis_publish.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/redis/sensors/__init__.py
--rw-r--r--   0        0        0      193 2024-03-23 11:41:50.659806 airfly-0.9.0/src/airfly/_vendor/airflow/providers/redis/sensors/redis_key.py
--rw-r--r--   0        0        0      213 2024-03-23 11:41:51.091817 airfly-0.9.0/src/airfly/_vendor/airflow/providers/redis/sensors/redis_pub_sub.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/salesforce/operators/__init__.py
--rw-r--r--   0        0        0      383 2024-03-23 11:41:51.531828 airfly-0.9.0/src/airfly/_vendor/airflow/providers/salesforce/operators/bulk.py
--rw-r--r--   0        0        0      248 2024-03-23 11:41:51.963838 airfly-0.9.0/src/airfly/_vendor/airflow/providers/salesforce/operators/salesforce_apex_rest.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/samba/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/samba/transfers/__init__.py
--rw-r--r--   0        0        0      393 2024-03-23 11:41:52.395849 airfly-0.9.0/src/airfly/_vendor/airflow/providers/samba/transfers/gcs_to_samba.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/segment/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/segment/operators/__init__.py
--rw-r--r--   0        0        0      283 2024-03-23 11:41:52.827860 airfly-0.9.0/src/airfly/_vendor/airflow/providers/segment/operators/segment_track_event.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/sftp/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/sftp/decorators/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/sftp/decorators/sensors/__init__.py
--rw-r--r--   0        0        0      177 2024-03-23 11:41:53.679881 airfly-0.9.0/src/airfly/_vendor/airflow/providers/sftp/decorators/sensors/sftp.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/sftp/operators/__init__.py
--rw-r--r--   0        0        0      425 2024-03-23 11:41:54.115891 airfly-0.9.0/src/airfly/_vendor/airflow/providers/sftp/operators/sftp.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/sftp/sensors/__init__.py
--rw-r--r--   0        0        0      375 2024-03-23 11:41:53.247870 airfly-0.9.0/src/airfly/_vendor/airflow/providers/sftp/sensors/sftp.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/singularity/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/singularity/operators/__init__.py
--rw-r--r--   0        0        0      469 2024-03-23 11:41:54.543902 airfly-0.9.0/src/airfly/_vendor/airflow/providers/singularity/operators/singularity.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/slack/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.744399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/slack/operators/__init__.py
--rw-r--r--   0        0        0      806 2024-03-23 11:41:54.963912 airfly-0.9.0/src/airfly/_vendor/airflow/providers/slack/operators/slack.py
--rw-r--r--   0        0        0      473 2024-03-23 11:41:55.403923 airfly-0.9.0/src/airfly/_vendor/airflow/providers/slack/operators/slack_webhook.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/slack/transfers/__init__.py
--rw-r--r--   0        0        0      403 2024-03-23 11:41:55.843934 airfly-0.9.0/src/airfly/_vendor/airflow/providers/slack/transfers/base_sql_to_slack.py
--rw-r--r--   0        0        0      804 2024-03-23 11:41:56.695955 airfly-0.9.0/src/airfly/_vendor/airflow/providers/slack/transfers/sql_to_slack.py
--rw-r--r--   0        0        0      467 2024-03-23 11:41:56.259944 airfly-0.9.0/src/airfly/_vendor/airflow/providers/slack/transfers/sql_to_slack_webhook.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.716092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/smtp/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/smtp/operators/__init__.py
--rw-r--r--   0        0        0      448 2024-03-23 11:41:57.127966 airfly-0.9.0/src/airfly/_vendor/airflow/providers/smtp/operators/smtp.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/snowflake/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0        0        0     2011 2024-03-23 11:41:57.599977 airfly-0.9.0/src/airfly/_vendor/airflow/providers/snowflake/operators/snowflake.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0        0        0      630 2024-03-23 11:41:58.023988 airfly-0.9.0/src/airfly/_vendor/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/sqlite/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/sqlite/operators/__init__.py
--rw-r--r--   0        0        0      203 2024-03-23 11:41:58.451998 airfly-0.9.0/src/airfly/_vendor/airflow/providers/sqlite/operators/sqlite.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/ssh/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/ssh/operators/__init__.py
--rw-r--r--   0        0        0      467 2024-03-23 11:41:58.900009 airfly-0.9.0/src/airfly/_vendor/airflow/providers/ssh/operators/ssh.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/tableau/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/tableau/operators/__init__.py
--rw-r--r--   0        0        0      335 2024-03-23 11:41:59.356020 airfly-0.9.0/src/airfly/_vendor/airflow/providers/tableau/operators/tableau.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/tableau/sensors/__init__.py
--rw-r--r--   0        0        0      232 2024-03-23 11:41:59.856033 airfly-0.9.0/src/airfly/_vendor/airflow/providers/tableau/sensors/tableau.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/telegram/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/telegram/operators/__init__.py
--rw-r--r--   0        0        0      279 2024-03-23 11:42:00.364045 airfly-0.9.0/src/airfly/_vendor/airflow/providers/telegram/operators/telegram.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/trino/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/trino/operators/__init__.py
--rw-r--r--   0        0        0      202 2024-03-23 11:42:00.804056 airfly-0.9.0/src/airfly/_vendor/airflow/providers/trino/operators/trino.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/trino/transfers/__init__.py
--rw-r--r--   0        0        0      401 2024-03-23 11:42:01.252067 airfly-0.9.0/src/airfly/_vendor/airflow/providers/trino/transfers/gcs_to_trino.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/vertica/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/providers/vertica/operators/__init__.py
--rw-r--r--   0        0        0      204 2024-03-23 11:42:01.700078 airfly-0.9.0/src/airfly/_vendor/airflow/providers/vertica/operators/vertica.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/weaviate/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/weaviate/operators/__init__.py
--rw-r--r--   0        0        0      735 2024-03-23 11:42:02.144089 airfly-0.9.0/src/airfly/_vendor/airflow/providers/weaviate/operators/weaviate.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/yandex/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/providers/yandex/operators/__init__.py
--rw-r--r--   0        0        0     3577 2024-03-23 11:42:02.640101 airfly-0.9.0/src/airfly/_vendor/airflow/providers/yandex/operators/yandexcloud_dataproc.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/__init__.py
--rw-r--r--   0        0        0      432 2024-03-23 11:39:55.644887 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/base.py
--rw-r--r--   0        0        0      258 2024-03-23 11:40:05.969159 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/bash.py
--rw-r--r--   0        0        0      209 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/date_time.py
--rw-r--r--   0        0        0      847 2024-03-23 11:40:05.097136 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/external_task.py
--rw-r--r--   0        0        0      221 2024-03-23 11:40:06.393170 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/filesystem.py
--rw-r--r--   0        0        0      286 2024-03-23 11:40:00.817023 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/python.py
--rw-r--r--   0        0        0      388 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/smart_sensor.py
--rw-r--r--   0        0        0      285 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/sql.py
--rw-r--r--   0        0        0      241 2024-03-23 11:40:06.821182 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/time_delta.py
--rw-r--r--   0        0        0      246 2024-03-23 11:40:07.217192 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/time_sensor.py
--rw-r--r--   0        0        0      289 2024-03-23 11:40:07.641203 airfly-0.9.0/src/airfly/_vendor/airflow/sensors/weekday.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/serialization/__init__.py
--rw-r--r--   0        0        0      220 2024-03-23 11:39:56.484909 airfly-0.9.0/src/airfly/_vendor/airflow/serialization/serialized_objects.py
--rw-r--r--   0        0        0        0 2024-03-23 11:31:51.712092 airfly-0.9.0/src/airfly/_vendor/airflow/template/__init__.py
--rw-r--r--   0        0        0      169 2024-03-23 11:39:53.500831 airfly-0.9.0/src/airfly/_vendor/airflow/template/templater.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/_vendor/airflow/utils/log/__init__.py
--rw-r--r--   0        0        0       86 2024-03-23 11:39:53.072819 airfly-0.9.0/src/airfly/_vendor/airflow/utils/log/logging_mixin.py
--rw-r--r--   0        0        0       68 2024-03-23 11:40:11.973317 airfly-0.9.0/src/airfly/_vendor/typing.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/cli/__init__.py
--rw-r--r--   0        0        0     2885 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/cli/main.py
--rw-r--r--   0        0        0     1689 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/cli/utils.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/model/__init__.py
--rw-r--r--   0        0        0     9057 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/model/airflow.py
--rw-r--r--   0        0        0     2695 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/model/base.py
--rw-r--r--   0        0        0     4220 2024-03-23 08:58:10.748399 airfly-0.9.0/src/airfly/utils.py
--rw-r--r--   0        0        0        0 2024-03-23 09:08:57.065001 airfly-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/tests/_gutt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/tests/_gutt/airfly/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/tests/_gutt/airfly/cli/__init__.py
--rw-r--r--   0        0        0       64 2024-03-23 08:58:10.748399 airfly-0.9.0/tests/_gutt/airfly/cli/test_main.py
--rw-r--r--   0        0        0      853 2024-03-23 08:58:10.748399 airfly-0.9.0/tests/_gutt/airfly/cli/test_utils.py
--rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-0.9.0/tests/_gutt/airfly/model/__init__.py
--rw-r--r--   0        0        0     1284 2024-03-23 08:58:10.748399 airfly-0.9.0/tests/_gutt/airfly/model/test_airflow.py
--rw-r--r--   0        0        0     1713 2024-03-23 08:58:10.748399 airfly-0.9.0/tests/_gutt/airfly/model/test_base.py
--rw-r--r--   0        0        0     1019 2024-03-23 08:58:10.748399 airfly-0.9.0/tests/_gutt/airfly/test_utils.py
--rw-r--r--   0        0        0    10157 1970-01-01 00:00:00.000000 airfly-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-03-23 08:58:10.696397 airfly-1.0.0/LICENSE
+-rw-r--r--   0        0        0    16021 2024-05-11 15:05:09.839409 airfly-1.0.0/README.md
+-rw-r--r--   0        0        0     1020 2024-05-11 15:18:48.701513 airfly-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      123 2024-03-23 08:58:10.708398 airfly-1.0.0/src/airfly/__init__.py
+-rw-r--r--   0        0        0      609 2024-05-11 15:05:09.871410 airfly-1.0.0/src/airfly/_meta.py
+-rw-r--r--   0        0        0      617 2024-05-11 15:05:09.875410 airfly-1.0.0/src/airfly/_vendor/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-23 17:02:59.099106 airfly-1.0.0/src/airfly/_vendor/airflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/decorators/__init__.py
+-rw-r--r--   0        0        0      359 2024-03-24 06:31:17.967011 airfly-1.0.0/src/airfly/_vendor/airflow/decorators/base.py
+-rw-r--r--   0        0        0      387 2024-03-24 06:31:19.755069 airfly-1.0.0/src/airfly/_vendor/airflow/decorators/branch_external_python.py
+-rw-r--r--   0        0        0      357 2024-03-24 06:31:20.175083 airfly-1.0.0/src/airfly/_vendor/airflow/decorators/branch_python.py
+-rw-r--r--   0        0        0      393 2024-03-24 12:21:24.418761 airfly-1.0.0/src/airfly/_vendor/airflow/decorators/branch_virtualenv.py
+-rw-r--r--   0        0        0      369 2024-03-24 06:31:20.987109 airfly-1.0.0/src/airfly/_vendor/airflow/decorators/external_python.py
+-rw-r--r--   0        0        0      323 2024-03-24 06:31:18.863040 airfly-1.0.0/src/airfly/_vendor/airflow/decorators/python.py
+-rw-r--r--   0        0        0      375 2024-03-24 06:31:21.419123 airfly-1.0.0/src/airfly/_vendor/airflow/decorators/python_virtualenv.py
+-rw-r--r--   0        0        0      171 2024-03-24 06:31:22.251149 airfly-1.0.0/src/airfly/_vendor/airflow/decorators/sensor.py
+-rw-r--r--   0        0        0      357 2024-03-24 06:31:22.667163 airfly-1.0.0/src/airfly/_vendor/airflow/decorators/short_circuit.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.064900 airfly-1.0.0/src/airfly/_vendor/airflow/example_dags/__init__.py
+-rw-r--r--   0        0        0      167 2024-03-24 06:31:25.199244 airfly-1.0.0/src/airfly/_vendor/airflow/example_dags/example_dag_decorator.py
+-rw-r--r--   0        0        0      226 2024-03-24 06:31:25.643258 airfly-1.0.0/src/airfly/_vendor/airflow/example_dags/example_dynamic_task_mapping_with_no_taskflow_operators.py
+-rw-r--r--   0        0        0     1951 2024-03-24 06:31:29.123371 airfly-1.0.0/src/airfly/_vendor/airflow/example_dags/example_skip_dag.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/models/__init__.py
+-rw-r--r--   0        0        0      234 2024-03-24 06:31:15.218923 airfly-1.0.0/src/airfly/_vendor/airflow/models/abstractoperator.py
+-rw-r--r--   0        0        0     1958 2024-03-24 06:31:15.758940 airfly-1.0.0/src/airfly/_vendor/airflow/models/baseoperator.py
+-rw-r--r--   0        0        0      169 2024-03-24 06:31:16.186954 airfly-1.0.0/src/airfly/_vendor/airflow/models/skipmixin.py
+-rw-r--r--   0        0        0      119 2024-03-24 06:31:14.726907 airfly-1.0.0/src/airfly/_vendor/airflow/models/taskmixin.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/operators/__init__.py
+-rw-r--r--   0        0        0      361 2024-03-24 06:31:23.079176 airfly-1.0.0/src/airfly/_vendor/airflow/operators/bash.py
+-rw-r--r--   0        0        0     2081 2024-03-24 06:31:19.339056 airfly-1.0.0/src/airfly/_vendor/airflow/operators/branch.py
+-rw-r--r--   0        0        0      460 2024-03-24 06:31:23.947204 airfly-1.0.0/src/airfly/_vendor/airflow/operators/datetime.py
+-rw-r--r--   0        0        0      426 2024-03-24 06:31:24.795231 airfly-1.0.0/src/airfly/_vendor/airflow/operators/email.py
+-rw-r--r--   0        0        0     1947 2024-03-24 06:31:23.531190 airfly-1.0.0/src/airfly/_vendor/airflow/operators/empty.py
+-rw-r--r--   0        0        0      323 2024-03-24 06:31:29.955397 airfly-1.0.0/src/airfly/_vendor/airflow/operators/generic_transfer.py
+-rw-r--r--   0        0        0     1961 2024-03-24 06:31:26.535287 airfly-1.0.0/src/airfly/_vendor/airflow/operators/latest_only.py
+-rw-r--r--   0        0        0     3469 2024-03-24 06:31:18.439026 airfly-1.0.0/src/airfly/_vendor/airflow/operators/python.py
+-rw-r--r--   0        0        0      287 2024-03-24 06:31:17.102983 airfly-1.0.0/src/airfly/_vendor/airflow/operators/subdag.py
+-rw-r--r--   0        0        0      474 2024-03-24 06:31:29.527383 airfly-1.0.0/src/airfly/_vendor/airflow/operators/trigger_dagrun.py
+-rw-r--r--   0        0        0      404 2024-03-24 06:31:24.359217 airfly-1.0.0/src/airfly/_vendor/airflow/operators/weekday.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/airbyte/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/airbyte/operators/__init__.py
+-rw-r--r--   0        0        0      330 2024-03-24 06:31:30.363410 airfly-1.0.0/src/airfly/_vendor/airflow/providers/airbyte/operators/airbyte.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/airbyte/sensors/__init__.py
+-rw-r--r--   0        0        0      254 2024-03-24 06:31:30.771423 airfly-1.0.0/src/airfly/_vendor/airflow/providers/airbyte/sensors/airbyte.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/alibaba/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/operators/__init__.py
+-rw-r--r--   0        0        0     1055 2024-03-24 06:31:31.211438 airfly-1.0.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/operators/analyticdb_spark.py
+-rw-r--r--   0        0        0      919 2024-03-24 06:31:31.643451 airfly-1.0.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/operators/oss.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.064900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/sensors/__init__.py
+-rw-r--r--   0        0        0      232 2024-03-24 06:31:32.039464 airfly-1.0.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/sensors/analyticdb_spark.py
+-rw-r--r--   0        0        0      251 2024-03-24 06:31:32.455478 airfly-1.0.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/sensors/oss_key.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0        0        0     1293 2024-03-24 06:31:34.203534 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0        0        0      542 2024-03-24 06:31:34.775552 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0        0        0      380 2024-03-24 06:31:33.719518 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/base_aws.py
+-rw-r--r--   0        0        0     1237 2024-03-24 06:31:35.223566 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0        0        0      419 2024-03-24 06:31:35.643580 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0        0        0      722 2024-03-24 06:31:36.067593 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0        0        0      889 2024-03-24 06:31:36.479607 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0        0        0     1389 2024-03-24 06:31:36.907620 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0        0        0     1727 2024-03-24 06:31:37.355635 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0        0        0     4513 2024-03-24 06:31:37.871651 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0        0        0      741 2024-03-24 06:31:38.295665 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/eventbridge.py
+-rw-r--r--   0        0        0      405 2024-03-24 06:31:38.691678 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0        0        0      747 2024-03-24 06:31:39.119691 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0        0        0      310 2024-03-24 06:31:39.523704 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0        0        0      284 2024-03-24 06:31:39.939718 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/glue_databrew.py
+-rw-r--r--   0        0        0      768 2024-03-24 06:31:40.367731 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0        0        0      523 2024-03-24 06:31:40.779744 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/neptune.py
+-rw-r--r--   0        0        0      333 2024-03-24 06:31:41.191758 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0        0        0     2863 2024-03-24 06:31:41.703774 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0        0        0     2711 2024-03-24 06:31:42.155789 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0        0        0      552 2024-03-24 06:31:42.555801 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0        0        0     2275 2024-03-24 06:31:43.019816 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0        0        0     4301 2024-03-24 06:31:43.523832 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0        0        0      292 2024-03-24 06:31:43.943846 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0        0        0      333 2024-03-24 06:31:44.343859 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0        0        0      468 2024-03-24 06:31:44.767872 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/step_function.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0        0        0      248 2024-03-24 06:31:45.591899 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0        0        0      383 2024-03-24 06:31:45.179885 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/base_aws.py
+-rw-r--r--   0        0        0      623 2024-03-24 06:31:46.059913 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0        0        0      348 2024-03-24 06:31:46.463926 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0        0        0      356 2024-03-24 06:31:46.915941 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0        0        0      390 2024-03-24 06:31:47.371955 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0        0        0      291 2024-03-24 06:31:47.883972 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0        0        0      757 2024-03-24 06:31:48.383988 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0        0        0      652 2024-03-24 06:31:48.848003 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0        0        0     1280 2024-03-24 06:31:49.288017 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0        0        0      260 2024-03-24 06:31:49.696030 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0        0        0      240 2024-03-24 06:31:50.112043 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0        0        0      342 2024-03-24 06:31:50.520056 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0        0        0      210 2024-03-24 06:31:50.940070 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0        0        0      265 2024-03-24 06:31:51.348083 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0        0        0      217 2024-03-24 06:31:51.752096 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0        0        0      706 2024-03-24 06:31:52.320114 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0        0        0      268 2024-03-24 06:31:52.872131 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0        0        0      687 2024-03-24 06:31:53.452150 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0        0        0      718 2024-03-24 06:31:53.892164 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0        0        0      494 2024-03-24 06:31:54.308177 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0        0        0      206 2024-03-24 06:31:54.736191 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/step_function.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0        0        0      280 2024-03-24 06:31:55.196205 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0        0        0      512 2024-03-24 06:31:55.616219 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0        0        0      430 2024-03-24 06:31:56.072233 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0        0        0      434 2024-03-24 06:31:56.496247 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0        0        0      626 2024-03-24 06:31:56.916260 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0        0        0      375 2024-03-24 06:31:57.340274 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0        0        0      704 2024-03-24 06:31:57.780288 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0        0        0      681 2024-03-24 06:31:58.204301 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/http_to_s3.py
+-rw-r--r--   0        0        0      395 2024-03-24 06:31:58.628315 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0        0        0      379 2024-03-24 06:31:59.060329 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0        0        0      451 2024-03-24 06:31:59.472342 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0        0        0      566 2024-03-24 06:31:59.948357 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0        0        0      269 2024-03-24 06:32:00.360370 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0        0        0      507 2024-03-24 06:32:00.828385 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0        0        0      264 2024-03-24 06:32:01.260399 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0        0        0      428 2024-03-24 06:32:01.680412 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0        0        0      521 2024-03-24 06:32:02.120426 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0        0        0      282 2024-03-24 06:32:02.536440 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0        0        0      548 2024-03-24 06:32:03.008454 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.064900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0        0        0      128 2024-03-24 06:31:33.283504 airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/utils/mixins.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/arangodb/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.064900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/arangodb/operators/__init__.py
+-rw-r--r--   0        0        0      230 2024-03-24 06:32:03.428468 airfly-1.0.0/src/airfly/_vendor/airflow/providers/arangodb/operators/arangodb.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/arangodb/sensors/__init__.py
+-rw-r--r--   0        0        0      193 2024-03-24 06:32:03.836481 airfly-1.0.0/src/airfly/_vendor/airflow/providers/arangodb/sensors/arangodb.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/asana/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/asana/operators/__init__.py
+-rw-r--r--   0        0        0      540 2024-03-24 06:32:04.284495 airfly-1.0.0/src/airfly/_vendor/airflow/providers/asana/operators/asana_tasks.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/celery/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/celery/sensors/__init__.py
+-rw-r--r--   0        0        0      213 2024-03-24 06:32:04.708509 airfly-1.0.0/src/airfly/_vendor/airflow/providers/celery/sensors/celery_queue.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/cohere/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/cohere/operators/__init__.py
+-rw-r--r--   0        0        0      266 2024-03-24 06:32:05.160523 airfly-1.0.0/src/airfly/_vendor/airflow/providers/cohere/operators/embedding.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/common/sql/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/common/sql/operators/__init__.py
+-rw-r--r--   0        0        0     1625 2024-03-24 06:32:06.692572 airfly-1.0.0/src/airfly/_vendor/airflow/providers/common/sql/operators/sql.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/operators/__init__.py
+-rw-r--r--   0        0        0     2552 2024-03-24 06:32:05.732541 airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks.py
+-rw-r--r--   0        0        0      876 2024-03-24 06:32:06.216557 airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks_repos.py
+-rw-r--r--   0        0        0     1395 2024-03-24 06:32:07.148586 airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks_sql.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/sensors/__init__.py
+-rw-r--r--   0        0        0      539 2024-03-24 06:32:07.564600 airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/sensors/databricks_partition.py
+-rw-r--r--   0        0        0      489 2024-03-24 06:32:07.988613 airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/sensors/databricks_sql.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/datadog/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/datadog/sensors/__init__.py
+-rw-r--r--   0        0        0      385 2024-03-24 06:32:08.392626 airfly-1.0.0/src/airfly/_vendor/airflow/providers/datadog/sensors/datadog.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/dingding/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.064900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/dingding/operators/__init__.py
+-rw-r--r--   0        0        0      289 2024-03-24 06:32:08.812639 airfly-1.0.0/src/airfly/_vendor/airflow/providers/dingding/operators/dingding.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/discord/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/discord/operators/__init__.py
+-rw-r--r--   0        0        0      347 2024-03-24 06:32:09.632665 airfly-1.0.0/src/airfly/_vendor/airflow/providers/discord/operators/discord_webhook.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.064900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/docker/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/docker/decorators/__init__.py
+-rw-r--r--   0        0        0      343 2024-03-24 06:32:10.484692 airfly-1.0.0/src/airfly/_vendor/airflow/providers/docker/decorators/docker.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/docker/operators/__init__.py
+-rw-r--r--   0        0        0     1593 2024-03-24 06:32:10.096680 airfly-1.0.0/src/airfly/_vendor/airflow/providers/docker/operators/docker.py
+-rw-r--r--   0        0        0      481 2024-03-24 06:32:10.916706 airfly-1.0.0/src/airfly/_vendor/airflow/providers/docker/operators/docker_swarm.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/exasol/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/exasol/operators/__init__.py
+-rw-r--r--   0        0        0      267 2024-03-24 06:32:11.348720 airfly-1.0.0/src/airfly/_vendor/airflow/providers/exasol/operators/exasol.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/ftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/ftp/operators/__init__.py
+-rw-r--r--   0        0        0      532 2024-03-24 06:32:11.776733 airfly-1.0.0/src/airfly/_vendor/airflow/providers/ftp/operators/ftp.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/ftp/sensors/__init__.py
+-rw-r--r--   0        0        0      331 2024-03-24 06:32:12.212747 airfly-1.0.0/src/airfly/_vendor/airflow/providers/ftp/sensors/ftp.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/github/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/github/operators/__init__.py
+-rw-r--r--   0        0        0      277 2024-03-24 06:32:12.644761 airfly-1.0.0/src/airfly/_vendor/airflow/providers/github/operators/github.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/github/sensors/__init__.py
+-rw-r--r--   0        0        0      563 2024-03-24 06:32:13.068775 airfly-1.0.0/src/airfly/_vendor/airflow/providers/github/sensors/github.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/ads/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/ads/operators/__init__.py
+-rw-r--r--   0        0        0      358 2024-03-24 06:32:13.496788 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/ads/operators/ads.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/ads/transfers/__init__.py
+-rw-r--r--   0        0        0      437 2024-03-24 06:32:13.928802 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/ads/transfers/ads_to_gcs.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/__init__.py
+-rw-r--r--   0        0        0     4425 2024-03-24 06:32:15.624856 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/automl.py
+-rw-r--r--   0        0        0     7146 2024-03-24 06:32:16.300877 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigquery.py
+-rw-r--r--   0        0        0     1337 2024-03-24 06:32:16.800893 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigquery_dts.py
+-rw-r--r--   0        0        0     2226 2024-03-24 06:32:17.304909 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigtable.py
+-rw-r--r--   0        0        0     1957 2024-03-24 06:32:14.784829 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_base.py
+-rw-r--r--   0        0        0     1194 2024-03-24 06:32:17.720922 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_batch.py
+-rw-r--r--   0        0        0     3913 2024-03-24 06:32:18.200937 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_build.py
+-rw-r--r--   0        0        0     2461 2024-03-24 06:32:18.652952 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_composer.py
+-rw-r--r--   0        0        0     6664 2024-03-24 06:32:19.200969 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_memorystore.py
+-rw-r--r--   0        0        0     1346 2024-03-24 06:32:19.660984 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_run.py
+-rw-r--r--   0        0        0     2934 2024-03-24 06:32:20.136999 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_sql.py
+-rw-r--r--   0        0        0     3106 2024-03-24 06:32:20.605014 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_storage_transfer_service.py
+-rw-r--r--   0        0        0     4766 2024-03-24 06:32:21.121030 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/compute.py
+-rw-r--r--   0        0        0     8132 2024-03-24 06:32:21.701048 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datacatalog.py
+-rw-r--r--   0        0        0     5491 2024-03-24 06:32:22.225065 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataform.py
+-rw-r--r--   0        0        0     3256 2024-03-24 06:32:22.717080 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datafusion.py
+-rw-r--r--   0        0        0      518 2024-03-24 06:32:23.157095 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datapipeline.py
+-rw-r--r--   0        0        0     8061 2024-03-24 06:32:23.737113 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataplex.py
+-rw-r--r--   0        0        0     1107 2024-03-24 06:32:24.181127 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataprep.py
+-rw-r--r--   0        0        0     8001 2024-03-24 06:32:24.761145 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataproc.py
+-rw-r--r--   0        0        0     4105 2024-03-24 06:32:25.261161 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataproc_metastore.py
+-rw-r--r--   0        0        0     2225 2024-03-24 06:32:25.713175 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datastore.py
+-rw-r--r--   0        0        0    11576 2024-03-24 06:32:26.365196 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dlp.py
+-rw-r--r--   0        0        0      923 2024-03-24 06:32:26.809210 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/functions.py
+-rw-r--r--   0        0        0     2849 2024-03-24 06:32:27.289225 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/gcs.py
+-rw-r--r--   0        0        0      229 2024-03-24 06:32:27.785241 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/life_sciences.py
+-rw-r--r--   0        0        0      411 2024-03-24 06:32:28.213255 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/looker.py
+-rw-r--r--   0        0        0     1039 2024-03-24 06:32:28.661269 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/mlengine.py
+-rw-r--r--   0        0        0     1386 2024-03-24 06:32:29.145284 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/natural_language.py
+-rw-r--r--   0        0        0     2675 2024-03-24 06:32:29.721302 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/pubsub.py
+-rw-r--r--   0        0        0     1635 2024-03-24 06:32:30.173317 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/spanner.py
+-rw-r--r--   0        0        0      461 2024-03-24 06:32:30.601330 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/speech_to_text.py
+-rw-r--r--   0        0        0     3407 2024-03-24 06:32:31.069345 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/stackdriver.py
+-rw-r--r--   0        0        0     4488 2024-03-24 06:32:31.581361 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/tasks.py
+-rw-r--r--   0        0        0      571 2024-03-24 06:32:31.997374 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/text_to_speech.py
+-rw-r--r--   0        0        0      419 2024-03-24 06:32:32.421388 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/translate.py
+-rw-r--r--   0        0        0      482 2024-03-24 06:32:32.849401 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/translate_speech.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/__init__.py
+-rw-r--r--   0        0        0     4846 2024-03-24 06:32:33.369418 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/auto_ml.py
+-rw-r--r--   0        0        0     2216 2024-03-24 06:32:33.845433 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/batch_prediction_job.py
+-rw-r--r--   0        0        0     3758 2024-03-24 06:32:34.345448 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/custom_job.py
+-rw-r--r--   0        0        0     2569 2024-03-24 06:32:34.865465 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/dataset.py
+-rw-r--r--   0        0        0     2648 2024-03-24 06:32:35.325479 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/endpoint_service.py
+-rw-r--r--   0        0        0     2326 2024-03-24 06:32:35.793494 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/hyperparameter_tuning_job.py
+-rw-r--r--   0        0        0     3446 2024-03-24 06:32:36.281509 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/model_service.py
+-rw-r--r--   0        0        0     1844 2024-03-24 06:32:36.737524 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/pipeline_job.py
+-rw-r--r--   0        0        0     1308 2024-03-24 06:32:37.165537 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/video_intelligence.py
+-rw-r--r--   0        0        0     5923 2024-03-24 06:32:37.709555 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vision.py
+-rw-r--r--   0        0        0     3270 2024-03-24 06:32:38.405577 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/workflows.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/__init__.py
+-rw-r--r--   0        0        0      768 2024-03-24 06:32:38.921593 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/bigquery.py
+-rw-r--r--   0        0        0      562 2024-03-24 06:32:39.385608 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/bigquery_dts.py
+-rw-r--r--   0        0        0      468 2024-03-24 06:32:39.845622 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/bigtable.py
+-rw-r--r--   0        0        0      178 2024-03-24 06:32:40.325637 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/cloud_composer.py
+-rw-r--r--   0        0        0      344 2024-03-24 06:32:40.721650 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/cloud_storage_transfer_service.py
+-rw-r--r--   0        0        0      437 2024-03-24 06:32:41.145663 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataform.py
+-rw-r--r--   0        0        0      477 2024-03-24 06:32:41.573677 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/datafusion.py
+-rw-r--r--   0        0        0     1238 2024-03-24 06:32:42.017691 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataplex.py
+-rw-r--r--   0        0        0      229 2024-03-24 06:32:42.417703 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataprep.py
+-rw-r--r--   0        0        0      454 2024-03-24 06:32:42.861717 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataproc.py
+-rw-r--r--   0        0        0      336 2024-03-24 06:32:43.253729 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataproc_metastore.py
+-rw-r--r--   0        0        0     1176 2024-03-24 06:32:43.841748 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/gcs.py
+-rw-r--r--   0        0        0      247 2024-03-24 06:32:44.305763 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/looker.py
+-rw-r--r--   0        0        0      457 2024-03-24 06:32:44.773777 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/pubsub.py
+-rw-r--r--   0        0        0      314 2024-03-24 06:32:14.328815 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/tasks.py
+-rw-r--r--   0        0        0      549 2024-03-24 06:32:45.257793 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/workflows.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/__init__.py
+-rw-r--r--   0        0        0      491 2024-03-24 06:32:45.709807 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_bigquery.py
+-rw-r--r--   0        0        0      674 2024-03-24 06:32:46.189822 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_gcs.py
+-rw-r--r--   0        0        0      368 2024-03-24 06:32:47.081850 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_mysql.py
+-rw-r--r--   0        0        0      281 2024-03-24 06:32:47.533864 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_postgres.py
+-rw-r--r--   0        0        0      495 2024-03-24 06:32:46.645836 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_sql.py
+-rw-r--r--   0        0        0      852 2024-03-24 06:32:48.001879 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/calendar_to_gcs.py
+-rw-r--r--   0        0        0      456 2024-03-24 06:32:48.429893 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/facebook_ads_to_gcs.py
+-rw-r--r--   0        0        0     1335 2024-03-24 06:32:48.873906 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_bigquery.py
+-rw-r--r--   0        0        0      642 2024-03-24 06:32:49.301920 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_gcs.py
+-rw-r--r--   0        0        0      368 2024-03-24 06:32:49.773935 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_local.py
+-rw-r--r--   0        0        0      391 2024-03-24 06:32:50.257950 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_sftp.py
+-rw-r--r--   0        0        0      357 2024-03-24 06:32:50.717965 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gdrive_to_gcs.py
+-rw-r--r--   0        0        0      329 2024-03-24 06:32:51.213980 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gdrive_to_local.py
+-rw-r--r--   0        0        0      342 2024-03-24 06:32:51.701995 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/local_to_gcs.py
+-rw-r--r--   0        0        0      254 2024-03-24 06:32:52.926034 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/mysql_to_gcs.py
+-rw-r--r--   0        0        0      256 2024-03-24 06:32:53.430050 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/oracle_to_gcs.py
+-rw-r--r--   0        0        0      302 2024-03-24 06:32:53.918065 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/postgres_to_gcs.py
+-rw-r--r--   0        0        0      228 2024-03-24 06:32:54.374080 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/presto_to_gcs.py
+-rw-r--r--   0        0        0      512 2024-03-24 06:32:54.834094 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/s3_to_gcs.py
+-rw-r--r--   0        0        0      437 2024-03-24 06:32:55.298109 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/salesforce_to_gcs.py
+-rw-r--r--   0        0        0      428 2024-03-24 06:32:55.754123 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/sftp_to_gcs.py
+-rw-r--r--   0        0        0      364 2024-03-24 06:32:56.206137 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/sheets_to_gcs.py
+-rw-r--r--   0        0        0      704 2024-03-24 06:32:52.410018 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/sql_to_gcs.py
+-rw-r--r--   0        0        0      226 2024-03-24 06:32:56.678152 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/trino_to_gcs.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/firebase/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/firebase/operators/__init__.py
+-rw-r--r--   0        0        0      339 2024-03-24 06:32:57.198168 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/firebase/operators/firestore.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/__init__.py
+-rw-r--r--   0        0        0      772 2024-03-24 06:32:57.654183 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/analytics.py
+-rw-r--r--   0        0        0     2388 2024-03-24 06:32:58.134198 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/analytics_admin.py
+-rw-r--r--   0        0        0     2025 2024-03-24 06:32:58.610213 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/campaign_manager.py
+-rw-r--r--   0        0        0     2228 2024-03-24 06:32:59.086228 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/display_video.py
+-rw-r--r--   0        0        0      632 2024-03-24 06:32:59.542242 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/search_ads.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/sensors/__init__.py
+-rw-r--r--   0        0        0      405 2024-03-24 06:32:59.982256 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/sensors/campaign_manager.py
+-rw-r--r--   0        0        0      622 2024-03-24 06:33:00.430270 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/sensors/display_video.py
+-rw-r--r--   0        0        0      358 2024-03-24 06:33:00.878284 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/sensors/search_ads.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/suite/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/suite/operators/__init__.py
+-rw-r--r--   0        0        0      312 2024-03-24 06:33:01.318298 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/suite/operators/sheets.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/suite/sensors/__init__.py
+-rw-r--r--   0        0        0      345 2024-03-24 06:33:01.782312 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/suite/sensors/drive.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/suite/transfers/__init__.py
+-rw-r--r--   0        0        0      379 2024-03-24 06:33:02.226326 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/suite/transfers/gcs_to_gdrive.py
+-rw-r--r--   0        0        0      337 2024-03-24 06:33:02.690341 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/suite/transfers/gcs_to_sheets.py
+-rw-r--r--   0        0        0      506 2024-03-24 06:33:03.182356 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/suite/transfers/local_to_drive.py
+-rw-r--r--   0        0        0      461 2024-03-24 06:33:03.638371 airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/suite/transfers/sql_to_sheets.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/grpc/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/grpc/operators/__init__.py
+-rw-r--r--   0        0        0      418 2024-03-24 06:33:04.134386 airfly-1.0.0/src/airfly/_vendor/airflow/providers/grpc/operators/grpc.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/http/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/http/operators/__init__.py
+-rw-r--r--   0        0        0      749 2024-03-24 06:32:09.216652 airfly-1.0.0/src/airfly/_vendor/airflow/providers/http/operators/http.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/http/sensors/__init__.py
+-rw-r--r--   0        0        0      587 2024-03-24 06:33:04.598401 airfly-1.0.0/src/airfly/_vendor/airflow/providers/http/sensors/http.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/imap/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/imap/sensors/__init__.py
+-rw-r--r--   0        0        0      289 2024-03-24 06:33:05.082416 airfly-1.0.0/src/airfly/_vendor/airflow/providers/imap/sensors/imap_attachment.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/influxdb/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/influxdb/operators/__init__.py
+-rw-r--r--   0        0        0      193 2024-03-24 06:33:05.578431 airfly-1.0.0/src/airfly/_vendor/airflow/providers/influxdb/operators/influxdb.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/jdbc/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/jdbc/operators/__init__.py
+-rw-r--r--   0        0        0      201 2024-03-24 06:33:06.242452 airfly-1.0.0/src/airfly/_vendor/airflow/providers/jdbc/operators/jdbc.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/jenkins/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/jenkins/operators/__init__.py
+-rw-r--r--   0        0        0      351 2024-03-24 06:33:06.750468 airfly-1.0.0/src/airfly/_vendor/airflow/providers/jenkins/operators/jenkins_job_trigger.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/jenkins/sensors/__init__.py
+-rw-r--r--   0        0        0      283 2024-03-24 06:33:07.198482 airfly-1.0.0/src/airfly/_vendor/airflow/providers/jenkins/sensors/jenkins.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/mongo/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/mongo/sensors/__init__.py
+-rw-r--r--   0        0        0      238 2024-03-24 06:33:07.650496 airfly-1.0.0/src/airfly/_vendor/airflow/providers/mongo/sensors/mongo.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/mysql/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/mysql/operators/__init__.py
+-rw-r--r--   0        0        0      202 2024-03-24 06:33:08.102511 airfly-1.0.0/src/airfly/_vendor/airflow/providers/mysql/operators/mysql.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/mysql/transfers/__init__.py
+-rw-r--r--   0        0        0      280 2024-03-24 06:33:08.550525 airfly-1.0.0/src/airfly/_vendor/airflow/providers/mysql/transfers/presto_to_mysql.py
+-rw-r--r--   0        0        0      363 2024-03-24 06:33:09.038540 airfly-1.0.0/src/airfly/_vendor/airflow/providers/mysql/transfers/s3_to_mysql.py
+-rw-r--r--   0        0        0      278 2024-03-24 06:33:09.494554 airfly-1.0.0/src/airfly/_vendor/airflow/providers/mysql/transfers/trino_to_mysql.py
+-rw-r--r--   0        0        0      341 2024-03-24 06:33:09.930568 airfly-1.0.0/src/airfly/_vendor/airflow/providers/mysql/transfers/vertica_to_mysql.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/neo4j/operators/__init__.py
+-rw-r--r--   0        0        0      241 2024-03-24 06:33:10.398582 airfly-1.0.0/src/airfly/_vendor/airflow/providers/neo4j/operators/neo4j.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/openai/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/openai/operators/__init__.py
+-rw-r--r--   0        0        0      293 2024-03-24 06:33:11.022602 airfly-1.0.0/src/airfly/_vendor/airflow/providers/openai/operators/openai.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/opensearch/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/opensearch/operators/__init__.py
+-rw-r--r--   0        0        0      636 2024-03-24 06:33:11.714624 airfly-1.0.0/src/airfly/_vendor/airflow/providers/opensearch/operators/opensearch.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/opsgenie/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/opsgenie/operators/__init__.py
+-rw-r--r--   0        0        0      971 2024-03-24 06:33:12.170638 airfly-1.0.0/src/airfly/_vendor/airflow/providers/opsgenie/operators/opsgenie.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/oracle/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/oracle/operators/__init__.py
+-rw-r--r--   0        0        0      408 2024-03-24 06:33:12.686654 airfly-1.0.0/src/airfly/_vendor/airflow/providers/oracle/operators/oracle.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.064900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/oracle/transfers/__init__.py
+-rw-r--r--   0        0        0      337 2024-03-24 06:33:13.206670 airfly-1.0.0/src/airfly/_vendor/airflow/providers/oracle/transfers/oracle_to_oracle.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/papermill/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/papermill/operators/__init__.py
+-rw-r--r--   0        0        0      353 2024-03-24 06:33:13.698686 airfly-1.0.0/src/airfly/_vendor/airflow/providers/papermill/operators/papermill.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/pgvector/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/pgvector/operators/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-24 06:33:14.202701 airfly-1.0.0/src/airfly/_vendor/airflow/providers/pgvector/operators/pgvector.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/pinecone/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/pinecone/operators/__init__.py
+-rw-r--r--   0        0        0      313 2024-03-24 06:33:14.694717 airfly-1.0.0/src/airfly/_vendor/airflow/providers/pinecone/operators/pinecone.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/postgres/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/postgres/operators/__init__.py
+-rw-r--r--   0        0        0      205 2024-03-24 06:33:15.170732 airfly-1.0.0/src/airfly/_vendor/airflow/providers/postgres/operators/postgres.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.064900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/presto/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/presto/transfers/__init__.py
+-rw-r--r--   0        0        0      404 2024-03-24 06:33:15.750750 airfly-1.0.0/src/airfly/_vendor/airflow/providers/presto/transfers/gcs_to_presto.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/redis/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/redis/operators/__init__.py
+-rw-r--r--   0        0        0      217 2024-03-24 06:33:16.242765 airfly-1.0.0/src/airfly/_vendor/airflow/providers/redis/operators/redis_publish.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/redis/sensors/__init__.py
+-rw-r--r--   0        0        0      193 2024-03-24 06:33:16.706780 airfly-1.0.0/src/airfly/_vendor/airflow/providers/redis/sensors/redis_key.py
+-rw-r--r--   0        0        0      213 2024-03-24 06:33:17.146793 airfly-1.0.0/src/airfly/_vendor/airflow/providers/redis/sensors/redis_pub_sub.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/salesforce/operators/__init__.py
+-rw-r--r--   0        0        0      383 2024-03-24 06:33:17.598808 airfly-1.0.0/src/airfly/_vendor/airflow/providers/salesforce/operators/bulk.py
+-rw-r--r--   0        0        0      248 2024-03-24 06:33:18.078823 airfly-1.0.0/src/airfly/_vendor/airflow/providers/salesforce/operators/salesforce_apex_rest.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/samba/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/samba/transfers/__init__.py
+-rw-r--r--   0        0        0      393 2024-03-24 06:33:18.578838 airfly-1.0.0/src/airfly/_vendor/airflow/providers/samba/transfers/gcs_to_samba.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/segment/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/segment/operators/__init__.py
+-rw-r--r--   0        0        0      283 2024-03-24 06:33:19.090854 airfly-1.0.0/src/airfly/_vendor/airflow/providers/segment/operators/segment_track_event.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/sftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/sftp/decorators/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/sftp/decorators/sensors/__init__.py
+-rw-r--r--   0        0        0      177 2024-03-24 06:33:20.126887 airfly-1.0.0/src/airfly/_vendor/airflow/providers/sftp/decorators/sensors/sftp.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/sftp/operators/__init__.py
+-rw-r--r--   0        0        0      425 2024-03-24 06:33:20.706905 airfly-1.0.0/src/airfly/_vendor/airflow/providers/sftp/operators/sftp.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/sftp/sensors/__init__.py
+-rw-r--r--   0        0        0      375 2024-03-24 06:33:19.646872 airfly-1.0.0/src/airfly/_vendor/airflow/providers/sftp/sensors/sftp.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/singularity/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/singularity/operators/__init__.py
+-rw-r--r--   0        0        0      469 2024-03-24 06:33:21.258922 airfly-1.0.0/src/airfly/_vendor/airflow/providers/singularity/operators/singularity.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/slack/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/slack/operators/__init__.py
+-rw-r--r--   0        0        0      806 2024-03-24 06:33:21.890942 airfly-1.0.0/src/airfly/_vendor/airflow/providers/slack/operators/slack.py
+-rw-r--r--   0        0        0      473 2024-03-24 06:33:22.482960 airfly-1.0.0/src/airfly/_vendor/airflow/providers/slack/operators/slack_webhook.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/slack/transfers/__init__.py
+-rw-r--r--   0        0        0      403 2024-03-24 06:33:22.958975 airfly-1.0.0/src/airfly/_vendor/airflow/providers/slack/transfers/base_sql_to_slack.py
+-rw-r--r--   0        0        0      804 2024-03-24 06:33:23.935006 airfly-1.0.0/src/airfly/_vendor/airflow/providers/slack/transfers/sql_to_slack.py
+-rw-r--r--   0        0        0      467 2024-03-24 06:33:23.474991 airfly-1.0.0/src/airfly/_vendor/airflow/providers/slack/transfers/sql_to_slack_webhook.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/smtp/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/smtp/operators/__init__.py
+-rw-r--r--   0        0        0      448 2024-03-24 06:33:24.379020 airfly-1.0.0/src/airfly/_vendor/airflow/providers/smtp/operators/smtp.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0        0        0     2011 2024-03-24 06:33:24.867035 airfly-1.0.0/src/airfly/_vendor/airflow/providers/snowflake/operators/snowflake.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0        0        0      630 2024-03-24 06:33:25.363050 airfly-1.0.0/src/airfly/_vendor/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/sqlite/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/sqlite/operators/__init__.py
+-rw-r--r--   0        0        0      203 2024-03-24 06:33:25.847065 airfly-1.0.0/src/airfly/_vendor/airflow/providers/sqlite/operators/sqlite.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/ssh/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/ssh/operators/__init__.py
+-rw-r--r--   0        0        0      467 2024-03-24 06:33:26.363081 airfly-1.0.0/src/airfly/_vendor/airflow/providers/ssh/operators/ssh.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/tableau/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/tableau/operators/__init__.py
+-rw-r--r--   0        0        0      335 2024-03-24 06:33:26.847097 airfly-1.0.0/src/airfly/_vendor/airflow/providers/tableau/operators/tableau.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/tableau/sensors/__init__.py
+-rw-r--r--   0        0        0      232 2024-03-24 06:33:27.343112 airfly-1.0.0/src/airfly/_vendor/airflow/providers/tableau/sensors/tableau.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/telegram/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.064900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/telegram/operators/__init__.py
+-rw-r--r--   0        0        0      279 2024-03-24 06:33:27.819127 airfly-1.0.0/src/airfly/_vendor/airflow/providers/telegram/operators/telegram.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/trino/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/trino/operators/__init__.py
+-rw-r--r--   0        0        0      202 2024-03-24 06:33:28.255140 airfly-1.0.0/src/airfly/_vendor/airflow/providers/trino/operators/trino.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/trino/transfers/__init__.py
+-rw-r--r--   0        0        0      401 2024-03-24 06:33:28.699154 airfly-1.0.0/src/airfly/_vendor/airflow/providers/trino/transfers/gcs_to_trino.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/vertica/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/vertica/operators/__init__.py
+-rw-r--r--   0        0        0      204 2024-03-24 06:33:29.135168 airfly-1.0.0/src/airfly/_vendor/airflow/providers/vertica/operators/vertica.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/weaviate/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/weaviate/operators/__init__.py
+-rw-r--r--   0        0        0      735 2024-03-24 06:33:29.607183 airfly-1.0.0/src/airfly/_vendor/airflow/providers/weaviate/operators/weaviate.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/yandex/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/providers/yandex/operators/__init__.py
+-rw-r--r--   0        0        0     3577 2024-03-24 06:33:30.115198 airfly-1.0.0/src/airfly/_vendor/airflow/providers/yandex/operators/yandexcloud_dataproc.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/sensors/__init__.py
+-rw-r--r--   0        0        0      432 2024-03-24 06:31:16.626968 airfly-1.0.0/src/airfly/_vendor/airflow/sensors/base.py
+-rw-r--r--   0        0        0      258 2024-03-24 06:31:26.931300 airfly-1.0.0/src/airfly/_vendor/airflow/sensors/bash.py
+-rw-r--r--   0        0        0      847 2024-03-24 06:31:26.083273 airfly-1.0.0/src/airfly/_vendor/airflow/sensors/external_task.py
+-rw-r--r--   0        0        0      221 2024-03-24 06:31:27.379314 airfly-1.0.0/src/airfly/_vendor/airflow/sensors/filesystem.py
+-rw-r--r--   0        0        0      286 2024-03-24 06:31:21.835136 airfly-1.0.0/src/airfly/_vendor/airflow/sensors/python.py
+-rw-r--r--   0        0        0      241 2024-03-24 06:31:27.799328 airfly-1.0.0/src/airfly/_vendor/airflow/sensors/time_delta.py
+-rw-r--r--   0        0        0      246 2024-03-24 06:31:28.199341 airfly-1.0.0/src/airfly/_vendor/airflow/sensors/time_sensor.py
+-rw-r--r--   0        0        0      289 2024-03-24 06:31:28.619354 airfly-1.0.0/src/airfly/_vendor/airflow/sensors/weekday.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/serialization/__init__.py
+-rw-r--r--   0        0        0      220 2024-03-24 06:31:17.522997 airfly-1.0.0/src/airfly/_vendor/airflow/serialization/serialized_objects.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/template/__init__.py
+-rw-r--r--   0        0        0      169 2024-03-24 06:31:14.190889 airfly-1.0.0/src/airfly/_vendor/airflow/template/templater.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.060900 airfly-1.0.0/src/airfly/_vendor/airflow/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:00:06.056900 airfly-1.0.0/src/airfly/_vendor/airflow/utils/log/__init__.py
+-rw-r--r--   0        0        0       86 2024-03-24 06:31:13.738875 airfly-1.0.0/src/airfly/_vendor/airflow/utils/log/logging_mixin.py
+-rw-r--r--   0        0        0       68 2024-03-24 06:31:32.835490 airfly-1.0.0/src/airfly/_vendor/typing.py
+-rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-1.0.0/src/airfly/cli/__init__.py
+-rw-r--r--   0        0        0     2784 2024-05-11 15:05:09.875410 airfly-1.0.0/src/airfly/cli/main.py
+-rw-r--r--   0        0        0     1337 2024-05-11 15:05:09.875410 airfly-1.0.0/src/airfly/cli/utils.py
+-rw-r--r--   0        0        0      109 2024-05-11 15:05:09.887410 airfly-1.0.0/src/airfly/model/__init__.py
+-rw-r--r--   0        0        0    32117 2024-05-11 15:05:09.887410 airfly-1.0.0/src/airfly/model/v1.py
+-rw-r--r--   0        0        0     4546 2024-05-11 15:05:09.891410 airfly-1.0.0/src/airfly/utils.py
+-rw-r--r--   0        0        0        0 2024-03-23 09:08:57.065001 airfly-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-1.0.0/tests/_gutt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-1.0.0/tests/_gutt/airfly/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-1.0.0/tests/_gutt/airfly/cli/__init__.py
+-rw-r--r--   0        0        0      766 2024-05-11 15:05:09.899411 airfly-1.0.0/tests/_gutt/airfly/cli/test_main.py
+-rw-r--r--   0        0        0     1477 2024-05-11 15:05:09.903411 airfly-1.0.0/tests/_gutt/airfly/cli/test_utils.py
+-rw-r--r--   0        0        0        0 2024-03-23 08:58:10.748399 airfly-1.0.0/tests/_gutt/airfly/model/__init__.py
+-rw-r--r--   0        0        0    18545 2024-05-11 15:05:09.907411 airfly-1.0.0/tests/_gutt/airfly/model/test_v1.py
+-rw-r--r--   0        0        0     2891 2024-05-11 15:05:09.907411 airfly-1.0.0/tests/_gutt/airfly/test_utils.py
+-rw-r--r--   0        0        0    16721 1970-01-01 00:00:00.000000 airfly-1.0.0/PKG-INFO
```

### Comparing `airfly-0.9.0/LICENSE` & `airfly-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/__init__.py` & `airfly-1.0.0/src/airfly/_vendor/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import importlib
 from functools import lru_cache
 from typing import Dict, Type
 
 from airfly._vendor import airflow
-from airfly.utils import collect_objects, load_module_by_name, qualname
+from airfly.utils import collect_objects, qualname
 
 
 @lru_cache()
 def collect_airflow_operators() -> Dict[str, Type]:
 
-    vendor = load_module_by_name(qualname(airflow))
+    vendor = importlib.import_module(qualname(airflow))
     collected = {}
 
     for item in collect_objects(vendor, lambda obj: isinstance(obj, type)):
 
         basename = qualname(item, level=1)
         if basename not in collected:
             collected[basename] = []
```

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/example_dags/example_skip_dag.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/example_dags/example_skip_dag.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/models/baseoperator.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/models/baseoperator.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/operators/branch.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/operators/branch.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/operators/empty.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/operators/latest_only.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/operators/latest_only.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/operators/python.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/operators/python.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/operators/analyticdb_spark.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/operators/analyticdb_spark.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/operators/oss.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/alibaba/cloud/operators/oss.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/appflow.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/athena.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/batch.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/batch.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/datasync.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/dms.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/ec2.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/ecs.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/emr.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/emr.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/eventbridge.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/eventbridge.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/glue.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/lambda_function.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/neptune.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/neptune.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/rds.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/rds.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/redshift_data.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/s3.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/s3_file_transform.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/search_ads.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 # Auto generated by 'inv collect-airflow'
 from airfly._vendor.airflow.models.baseoperator import BaseOperator
 
 
-class S3FileTransformOperator(BaseOperator):
-    source_s3_key: "str"
-    dest_s3_key: "str"
-    transform_script: "typing.Union[str, NoneType]"
-    select_expression: "_empty"
-    script_args: "typing.Union[typing.Sequence[str], NoneType]"
-    source_aws_conn_id: "str"
-    source_verify: "typing.Union[bool, str, NoneType]"
-    dest_aws_conn_id: "str"
-    dest_verify: "typing.Union[bool, str, NoneType]"
-    replace: "bool"
+class GoogleSearchAdsInsertReportOperator(BaseOperator):
+    report: "dict[str, Any]"
+    api_version: "str"
+    gcp_conn_id: "str"
+    delegate_to: "str | None"
+    impersonation_chain: "str | Sequence[str] | None"
+
+
+class GoogleSearchAdsDownloadReportOperator(BaseOperator):
+    report_id: "str"
+    bucket_name: "str"
+    report_name: "str | None"
+    gzip: "bool"
+    chunk_size: "int"
+    api_version: "str"
+    gcp_conn_id: "str"
+    delegate_to: "str | None"
+    impersonation_chain: "str | Sequence[str] | None"
```

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sagemaker.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/batch.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/ecs.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/eks.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/emr.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/rds.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/s3.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/sagemaker.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/http_to_s3.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/http_to_s3.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/apache/hive/transfers/mysql_to_hive.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/weaviate/operators/weaviate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 # Auto generated by 'inv collect-airflow'
 from airfly._vendor.airflow.models.baseoperator import BaseOperator
 
 
-class MySqlToHiveOperator(BaseOperator):
-    sql: "str"
-    hive_table: "str"
-    create: "bool"
-    recreate: "bool"
-    partition: "typing.Union[typing.Dict, NoneType]"
-    delimiter: "str"
-    quoting: "typing.Union[str, NoneType]"
-    quotechar: "str"
-    escapechar: "typing.Union[str, NoneType]"
-    mysql_conn_id: "str"
-    hive_cli_conn_id: "str"
-    tblproperties: "typing.Union[typing.Dict, NoneType]"
+class WeaviateIngestOperator(BaseOperator):
+    conn_id: "str"
+    class_name: "str"
+    input_json: "list[dict[str, Any]] | pd.DataFrame | None"
+    input_data: "list[dict[str, Any]] | pd.DataFrame | None"
+    vector_col: "str"
+    uuid_column: "str"
+    tenant: "str | None"
+
+
+class WeaviateDocumentIngestOperator(BaseOperator):
+    conn_id: "str"
+    input_data: "pd.DataFrame | list[dict[str, Any]] | list[pd.DataFrame]"
+    class_name: "str"
+    document_column: "str"
+    existing: "str"
+    uuid_column: "str"
+    vector_col: "str"
+    batch_config_params: "dict | None"
+    tenant: "str | None"
+    verbose: "bool"
```

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/asana/operators/asana_tasks.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/asana/operators/asana_tasks.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/common/sql/operators/sql.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/common/sql/operators/sql.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks_repos.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks_repos.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks_sql.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/operators/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/databricks/sensors/databricks_partition.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/databricks/sensors/databricks_partition.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/docker/operators/docker.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/docker/operators/docker.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/ftp/operators/ftp.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/ftp/operators/ftp.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/github/sensors/github.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/github/sensors/github.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/automl.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/automl.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigquery.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigquery_dts.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigquery_dts.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigtable.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/bigtable.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_base.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_base.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_batch.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_batch.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_build.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_build.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_composer.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_composer.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_memorystore.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_memorystore.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_run.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_run.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_sql.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_sql.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_storage_transfer_service.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/cloud_storage_transfer_service.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/compute.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/compute.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datacatalog.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datacatalog.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataform.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataform.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datafusion.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datafusion.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datapipeline.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datapipeline.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataplex.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataplex.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataprep.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataprep.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataproc.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataproc.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataproc_metastore.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dataproc_metastore.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datastore.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/datastore.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dlp.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/dlp.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/functions.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/functions.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/gcs.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/gcs.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/mlengine.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/mlengine.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/natural_language.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/natural_language.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/pubsub.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/pubsub.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/spanner.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/spanner.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/stackdriver.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/stackdriver.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/tasks.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/tasks.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/text_to_speech.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/text_to_speech.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/auto_ml.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/auto_ml.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/batch_prediction_job.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/custom_job.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/custom_job.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/dataset.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/dataset.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/endpoint_service.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/endpoint_service.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/hyperparameter_tuning_job.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/hyperparameter_tuning_job.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/model_service.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/model_service.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/pipeline_job.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vertex_ai/pipeline_job.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/video_intelligence.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/video_intelligence.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vision.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/vision.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/workflows.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/operators/workflows.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/bigquery.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/bigquery.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/bigquery_dts.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/bigquery_dts.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataplex.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/dataplex.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/gcs.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/gcs.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/workflows.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/sensors/workflows.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_gcs.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/bigquery_to_gcs.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/calendar_to_gcs.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/calendar_to_gcs.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_bigquery.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_gcs.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/gcs_to_gcs.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/s3_to_gcs.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/s3_to_gcs.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/sql_to_gcs.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/cloud/transfers/sql_to_gcs.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/analytics.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/analytics.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/analytics_admin.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/analytics_admin.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/campaign_manager.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/campaign_manager.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/display_video.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/display_video.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/operators/search_ads.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/google/marketing_platform/sensors/display_video.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # Auto generated by 'inv collect-airflow'
-from airfly._vendor.airflow.models.baseoperator import BaseOperator
+from airfly._vendor.airflow.sensors.base import BaseSensorOperator
 
 
-class GoogleSearchAdsInsertReportOperator(BaseOperator):
-    report: "dict[str, Any]"
+class GoogleDisplayVideo360GetSDFDownloadOperationSensor(BaseSensorOperator):
+    operation_name: "str"
     api_version: "str"
     gcp_conn_id: "str"
     delegate_to: "str | None"
+    mode: "str"
+    poke_interval: "int"
     impersonation_chain: "str | Sequence[str] | None"
 
 
-class GoogleSearchAdsDownloadReportOperator(BaseOperator):
+class GoogleDisplayVideo360RunQuerySensor(BaseSensorOperator):
+    query_id: "str"
     report_id: "str"
-    bucket_name: "str"
-    report_name: "str | None"
-    gzip: "bool"
-    chunk_size: "int"
     api_version: "str"
     gcp_conn_id: "str"
     delegate_to: "str | None"
     impersonation_chain: "str | Sequence[str] | None"
```

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/http/operators/http.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/http/operators/http.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/http/sensors/http.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/http/sensors/http.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/opensearch/operators/opensearch.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/opensearch/operators/opensearch.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/opsgenie/operators/opsgenie.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/opsgenie/operators/opsgenie.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/slack/operators/slack.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/slack/operators/slack.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/slack/transfers/sql_to_slack.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/slack/transfers/sql_to_slack.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/snowflake/operators/snowflake.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/snowflake/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/providers/yandex/operators/yandexcloud_dataproc.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/providers/yandex/operators/yandexcloud_dataproc.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/_vendor/airflow/sensors/external_task.py` & `airfly-1.0.0/src/airfly/_vendor/airflow/sensors/external_task.py`

 * *Files identical despite different names*

### Comparing `airfly-0.9.0/src/airfly/cli/main.py` & `airfly-1.0.0/src/airfly/cli/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+import importlib
 import os
 
 import click
-from airfly.model.airflow import AirflowDAG, AirflowTask
-from airfly.model.base import TaskTree, collect_taskpairs, collect_taskset
-from airfly.utils import load_module_by_name
+
+from airfly.model import AirFly, TaskTree
+from airfly.utils import qualname
 
 from .utils import (
-    InvalidModule,
     convert_dag_params,
+    convert_task_group,
     expand_sys_path,
     print_version,
-    should_exclude,
     validate_includes,
 )
 
 
 @click.command()
 @click.option(
     "--version",
@@ -67,46 +67,49 @@
         "Parameters to construct DAG object,"
         " defined by a dictionary in a python file."
         " Pass this option with <python-file>:<variable> form,"
         " the <variable> should be the dictionary"
         " which will be passed to DAG as keyword arguments."
     ),
 )
-def main(name, modname, path, exclude_pattern, includes, dag_params):
+@click.option(
+    "--task-class",
+    "-t",
+    default="airfly.model.AirFly",
+    help=f"Target task class to search, default: '{qualname(AirFly)}'",
+)
+@click.option(
+    "--task-group",
+    "-g",
+    callback=convert_task_group,
+    default=True,
+    help="Whether to enable TaskGroup, default: True",
+)
+def main(
+    name, modname, path, exclude_pattern, includes, dag_params, task_class, task_group
+):
 
     with expand_sys_path(*path):
-        try:
-            module = load_module_by_name(modname)
-        except Exception:
-            raise InvalidModule(f'got: "{modname}"')
+        module = importlib.import_module(modname)
+
+        taskmodule, taskname = task_class.rsplit(".", 1)
+        taskmodule = importlib.import_module(taskmodule)
+        taskclass = taskmodule.__dict__[taskname]
 
     name = name or f"{modname}_dag"
 
-    if dag_params[0]:
+    if dag_params and dag_params[0]:
         if includes:
             includes.append(dag_params[0])
         else:
             includes = [dag_params[0]]
 
-    taskset = set(
-        collect_taskset(
-            module,
-            taskclass=AirflowTask,
-            predicate=lambda obj: not should_exclude(obj, exclude_pattern),
-        )
+    tree = TaskTree.from_module(
+        module, taskclass=taskclass, exclude_pattern=exclude_pattern
     )
 
-    taskpairs = set(
-        collect_taskpairs(
-            taskset,
-            taskclass=AirflowTask,
-            predicate=lambda pair: not (
-                should_exclude(pair.up, exclude_pattern, verbose=False)
-                or should_exclude(pair.down, exclude_pattern, verbose=False)
-            ),
-        )
+    print(
+        tree.to_dag(
+            name, includes=includes, dag_params=dag_params, task_group=task_group
+        ),
+        end="",
     )
-    tasktree = TaskTree(taskset=taskset, taskpairs=taskpairs)
-
-    dag = AirflowDAG(name, tasktree, includes=includes, dag_params=dag_params)
-
-    print(dag.render())
```

### Comparing `airfly-0.9.0/src/airfly/cli/utils.py` & `airfly-1.0.0/src/airfly/cli/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,25 @@
 import os
 import sys
 from contextlib import contextmanager
-from types import FunctionType
-from typing import Optional, Union
 
 import click
-import regex as re
-from airfly.utils import qualname
 
 
 def print_version(ctx, param, value):
-    if not value or ctx.resilient_parsing:
+    if (not value) or ctx.resilient_parsing:
         return
 
     from airfly import __version__
 
     click.echo(f"Version: {__version__}")
 
     ctx.exit()
 
 
-def should_exclude(
-    obj: Union[FunctionType, type], pattern: Optional[str] = None, verbose: bool = True
-):
-    if pattern and isinstance(pattern, str):
-        obj_name = qualname(obj)
-        if re.search(pattern, obj_name):
-            if verbose:
-                click.secho("excluding ", err=True, nl=False, fg="bright_white")
-                click.secho(obj_name, err=True, fg="bright_black")
-            return True
-
-    return False
-
-
 @contextmanager
 def expand_sys_path(*paths: str):
 
     num = len(paths)
 
     for p in paths[::-1]:
         if p and isinstance(p, str):
@@ -60,22 +42,32 @@
 
     return value
 
 
 def convert_dag_params(ctx, param, value):
 
     if not value:
-        return (None, None)
+        return None
 
     elif isinstance(value, tuple):
         return value
 
     try:
         pypath, _, varname = value.partition(":")
         return pypath, varname
 
     except ValueError:
         raise click.BadParameter("format must be '<python-file>:<variable>'")
 
 
-class InvalidModule(Exception):
-    pass
+def convert_task_group(ctx, param, value):
+
+    if isinstance(value, bool):
+        return value
+
+    if isinstance(value, int):
+        return value == 1
+
+    if isinstance(value, str):
+        return value.lower() == "true" or value == "1"
+
+    return False
```

### Comparing `airfly-0.9.0/src/airfly/utils.py` & `airfly-1.0.0/src/airfly/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+import importlib
 import io
 import os
 import pathlib
 import pkgutil
 import subprocess as sp
 import sys
 import tempfile
 from contextlib import contextmanager
-from importlib._bootstrap_external import SourceFileLoader
 from types import FunctionType, ModuleType
 from typing import Callable, Generator, Union
 
+import attr
+import loguru
+
+immutable = attr.s(auto_attribs=True, slots=True, frozen=True, kw_only=True)
+
 
 def qualname(obj: Union[FunctionType, ModuleType, type], level: int = -1) -> str:
     """Return the qualname of a class, a function or a module.
 
     >>> class Foo:
     ...     pass
 
@@ -35,59 +40,65 @@
 
     else:
         name = ""
 
     return ".".join(name.split(".")[-level:]) if level > 0 else name
 
 
+def issubclass_by_qualname(cls, class_or_tuple):
+    mro = {qualname(o) for o in cls.mro()}
+
+    if isinstance(class_or_tuple, type):
+        class_or_tuple = (class_or_tuple,)
+
+    for o in class_or_tuple:
+        if qualname(o) in mro:
+            return True
+
+    return False
+
+
 def blacking(source_code: str):
 
     with tempfile.NamedTemporaryFile("w", delete=False) as f:
         f.write(source_code)
         fname = f.name
 
-    p = sp.Popen(f"cat {fname}".split(), stdout=sp.PIPE)
-
-    out = sp.check_output("black -q -".split(), stdin=p.stdout)
-
-    p.wait()
+    with sp.Popen(["cat", fname], stdout=sp.PIPE) as p:
+        cmd = [sys.executable, "-m", "black", "-q", "-"]
+        out = sp.check_output(cmd, stdin=p.stdout)
 
     try:
         pathlib.Path(fname).unlink()
+
     except FileNotFoundError:
         pass
 
     return out.decode()
 
 
 def isorting(source_code: str):
 
     with tempfile.NamedTemporaryFile("w", delete=False) as f:
         f.write(source_code)
         fname = f.name
 
-    p = sp.Popen(f"cat {fname}".split(), stdout=sp.PIPE)
-
-    out = sp.check_output("isort -q -".split(), stdin=p.stdout)
-
-    p.wait()
+    with sp.Popen(["cat", fname], stdout=sp.PIPE) as p:
+        cmd = [sys.executable, "-m", "isort", "--profile", "black", "-q", "-"]
+        out = sp.check_output(cmd, stdin=p.stdout)
 
     try:
         pathlib.Path(fname).unlink()
+
     except FileNotFoundError:
         pass
 
     return out.decode()
 
 
-def load_module_by_name(modname: str) -> ModuleType:
-    loader: SourceFileLoader = pkgutil.get_loader(modname)
-    return loader.load_module(modname)
-
-
 def collect_objects(
     module: ModuleType,
     predicate: Callable[[Union[FunctionType, type]], bool] = lambda _: True,
 ) -> Generator[Union[FunctionType, type], None, None]:
 
     modname = qualname(module)
     cached = set()
@@ -129,52 +140,49 @@
 def _collect_from_package(
     package: ModuleType,
 ) -> Generator[Union[FunctionType, type], None, None]:
 
     for obj in _collect_from_module(package):
         yield obj
 
-    for finder, name, _ in pkgutil.walk_packages(
-        package.__path__, package.__name__ + "."
-    ):
+    for _, name, _ in pkgutil.walk_packages(package.__path__, package.__name__ + "."):
 
         with _escape_any_commandline_parser():
             try:
-                mod = finder.find_module(name).load_module(name)
+                mod = importlib.import_module(name)
 
-            except BaseException:
+            except Exception as e:
+                loguru.logger.warning(f"Ignore invalid module: '{name}'. Reason: {e}")
                 continue
 
         for obj in _collect_from_module(mod):
-
             yield obj
 
 
 def _collect_from_module(
     module: ModuleType,
 ) -> Generator[Union[FunctionType, type], None, None]:
+
     for _, obj in module.__dict__.items():
-        if isinstance(obj, (type, FunctionType)):
 
+        if isinstance(obj, (type, FunctionType)):
             yield obj
 
 
 def makefile(fullpath: str, content: Union[str, bytes] = "", overwrite: bool = False):
 
     if not os.path.isfile(fullpath):
-
         dirpath = os.path.dirname(fullpath)
 
         if not os.path.isdir(dirpath):
             os.makedirs(dirpath)
 
         _writefile(fullpath, content)
 
     elif overwrite:
-
         _writefile(fullpath, content)
 
 
 def _writefile(fullpath: str, content: Union[str, bytes] = ""):
 
     if not isinstance(content, (str, bytes)):
         raise TypeError(f"content must be str or bytes, got: {type(content)}")
```

