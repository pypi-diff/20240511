# Comparing `tmp/dolphie-5.0.1.tar.gz` & `tmp/dolphie-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolphie-5.0.1.tar", max compression
+gzip compressed data, was "dolphie-5.0.2.tar", max compression
```

## Comparing `dolphie-5.0.1.tar` & `dolphie-5.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-5.0.1/LICENSE
--rw-r--r--   0        0        0    10793 2024-04-26 06:15:38.607085 dolphie-5.0.1/README.md
--rw-r--r--   0        0        0     7743 2024-04-24 08:27:31.216691 dolphie-5.0.1/dolphie/DataTypes.py
--rw-r--r--   0        0        0     8998 2024-04-24 08:27:31.216991 dolphie-5.0.1/dolphie/Dolphie.css
--rw-r--r--   0        0        0    21811 2024-04-26 06:15:38.607944 dolphie-5.0.1/dolphie/Modules/ArgumentParser.py
--rw-r--r--   0        0        0     6769 2024-04-24 08:32:49.079123 dolphie-5.0.1/dolphie/Modules/Functions.py
--rw-r--r--   0        0        0      975 2024-02-26 06:55:52.585216 dolphie-5.0.1/dolphie/Modules/ManualException.py
--rw-r--r--   0        0        0    38471 2024-04-24 08:27:31.218418 dolphie-5.0.1/dolphie/Modules/MetricManager.py
--rw-r--r--   0        0        0     8204 2024-04-29 08:16:25.745454 dolphie-5.0.1/dolphie/Modules/MySQL.py
--rw-r--r--   0        0        0    18980 2024-04-29 08:07:57.617395 dolphie-5.0.1/dolphie/Modules/Queries.py
--rw-r--r--   0        0        0    25493 2024-04-24 08:27:31.219824 dolphie-5.0.1/dolphie/Modules/TabManager.py
--rw-r--r--   0        0        0     9429 2024-04-29 08:32:25.955658 dolphie-5.0.1/dolphie/Panels/dashboard_panel.py
--rw-r--r--   0        0        0     1559 2024-02-26 06:55:52.588164 dolphie-5.0.1/dolphie/Panels/ddl_panel.py
--rw-r--r--   0        0        0     2893 2024-02-26 06:55:52.588611 dolphie-5.0.1/dolphie/Panels/innodb_trx_locks_panel.py
--rw-r--r--   0        0        0     7360 2024-04-24 08:27:31.220949 dolphie-5.0.1/dolphie/Panels/metadata_locks_panel.py
--rw-r--r--   0        0        0     9917 2024-04-29 08:20:11.637840 dolphie-5.0.1/dolphie/Panels/processlist_panel.py
--rw-r--r--   0        0        0     3925 2024-04-24 08:27:31.221888 dolphie-5.0.1/dolphie/Panels/proxysql_command_stats_panel.py
--rw-r--r--   0        0        0     5766 2024-04-25 17:40:15.854128 dolphie-5.0.1/dolphie/Panels/proxysql_dashboard_panel.py
--rw-r--r--   0        0        0     4949 2024-04-24 08:27:31.222954 dolphie-5.0.1/dolphie/Panels/proxysql_hostgroup_summary_panel.py
--rw-r--r--   0        0        0     4086 2024-04-24 08:27:31.223282 dolphie-5.0.1/dolphie/Panels/proxysql_mysql_query_rules_panel.py
--rw-r--r--   0        0        0     6839 2024-04-24 08:27:31.223666 dolphie-5.0.1/dolphie/Panels/proxysql_processlist_panel.py
--rw-r--r--   0        0        0    26275 2024-04-29 09:08:12.751007 dolphie-5.0.1/dolphie/Panels/replication_panel.py
--rw-r--r--   0        0        0     1050 2024-02-12 13:50:32.934971 dolphie-5.0.1/dolphie/Widgets/command_screen.py
--rw-r--r--   0        0        0     6319 2024-02-26 06:55:52.590441 dolphie-5.0.1/dolphie/Widgets/event_log_screen.py
--rw-r--r--   0        0        0     9388 2024-04-26 06:15:38.608277 dolphie-5.0.1/dolphie/Widgets/help.py
--rw-r--r--   0        0        0    13960 2024-03-15 01:09:17.039272 dolphie-5.0.1/dolphie/Widgets/host_setup.py
--rw-r--r--   0        0        0    12034 2024-04-24 08:27:31.224413 dolphie-5.0.1/dolphie/Widgets/modal.py
--rw-r--r--   0        0        0     3873 2024-04-24 08:27:31.224676 dolphie-5.0.1/dolphie/Widgets/proxysql_thread_screen.py
--rw-r--r--   0        0        0      563 2024-02-26 06:55:52.591220 dolphie-5.0.1/dolphie/Widgets/spinner.py
--rw-r--r--   0        0        0     5997 2024-04-24 08:27:31.225002 dolphie-5.0.1/dolphie/Widgets/thread_screen.py
--rw-r--r--   0        0        0     1125 2024-02-12 13:50:32.936036 dolphie-5.0.1/dolphie/Widgets/topbar.py
--rw-r--r--   0        0        0    13455 2024-04-29 07:10:07.370077 dolphie-5.0.1/dolphie/__init__.py
--rwxr-xr-x   0        0        0    79546 2024-04-29 08:40:21.156862 dolphie-5.0.1/dolphie/app.py
--rw-r--r--   0        0        0      679 2024-04-29 08:58:05.522159 dolphie-5.0.1/pyproject.toml
--rw-r--r--   0        0        0    11861 1970-01-01 00:00:00.000000 dolphie-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-5.0.2/LICENSE
+-rw-r--r--   0        0        0    10798 2024-05-11 07:11:57.734402 dolphie-5.0.2/README.md
+-rw-r--r--   0        0        0     7743 2024-04-30 21:07:23.598756 dolphie-5.0.2/dolphie/DataTypes.py
+-rw-r--r--   0        0        0     8998 2024-04-24 08:27:31.216991 dolphie-5.0.2/dolphie/Dolphie.css
+-rw-r--r--   0        0        0    21811 2024-04-26 06:15:38.607944 dolphie-5.0.2/dolphie/Modules/ArgumentParser.py
+-rw-r--r--   0        0        0     6769 2024-04-30 21:09:29.587679 dolphie-5.0.2/dolphie/Modules/Functions.py
+-rw-r--r--   0        0        0      975 2024-02-26 06:55:52.585216 dolphie-5.0.2/dolphie/Modules/ManualException.py
+-rw-r--r--   0        0        0    38471 2024-04-24 08:27:31.218418 dolphie-5.0.2/dolphie/Modules/MetricManager.py
+-rw-r--r--   0        0        0     8204 2024-04-30 20:48:05.867910 dolphie-5.0.2/dolphie/Modules/MySQL.py
+-rw-r--r--   0        0        0    19438 2024-04-30 05:21:06.394645 dolphie-5.0.2/dolphie/Modules/Queries.py
+-rw-r--r--   0        0        0    25493 2024-04-24 08:27:31.219824 dolphie-5.0.2/dolphie/Modules/TabManager.py
+-rw-r--r--   0        0        0     9429 2024-04-29 08:32:25.955658 dolphie-5.0.2/dolphie/Panels/dashboard_panel.py
+-rw-r--r--   0        0        0     1559 2024-02-26 06:55:52.588164 dolphie-5.0.2/dolphie/Panels/ddl_panel.py
+-rw-r--r--   0        0        0     2893 2024-02-26 06:55:52.588611 dolphie-5.0.2/dolphie/Panels/innodb_trx_locks_panel.py
+-rw-r--r--   0        0        0     7360 2024-04-24 08:27:31.220949 dolphie-5.0.2/dolphie/Panels/metadata_locks_panel.py
+-rw-r--r--   0        0        0     9917 2024-04-29 08:20:11.637840 dolphie-5.0.2/dolphie/Panels/processlist_panel.py
+-rw-r--r--   0        0        0     3925 2024-04-24 08:27:31.221888 dolphie-5.0.2/dolphie/Panels/proxysql_command_stats_panel.py
+-rw-r--r--   0        0        0     5766 2024-04-25 17:40:15.854128 dolphie-5.0.2/dolphie/Panels/proxysql_dashboard_panel.py
+-rw-r--r--   0        0        0     4949 2024-04-24 08:27:31.222954 dolphie-5.0.2/dolphie/Panels/proxysql_hostgroup_summary_panel.py
+-rw-r--r--   0        0        0     4086 2024-04-24 08:27:31.223282 dolphie-5.0.2/dolphie/Panels/proxysql_mysql_query_rules_panel.py
+-rw-r--r--   0        0        0     6839 2024-04-24 08:27:31.223666 dolphie-5.0.2/dolphie/Panels/proxysql_processlist_panel.py
+-rw-r--r--   0        0        0    30811 2024-04-30 05:49:22.567668 dolphie-5.0.2/dolphie/Panels/replication_panel.py
+-rw-r--r--   0        0        0     1050 2024-02-12 13:50:32.934971 dolphie-5.0.2/dolphie/Widgets/command_screen.py
+-rw-r--r--   0        0        0     6319 2024-02-26 06:55:52.590441 dolphie-5.0.2/dolphie/Widgets/event_log_screen.py
+-rw-r--r--   0        0        0     9388 2024-04-26 06:15:38.608277 dolphie-5.0.2/dolphie/Widgets/help.py
+-rw-r--r--   0        0        0    13983 2024-04-29 09:32:40.864207 dolphie-5.0.2/dolphie/Widgets/host_setup.py
+-rw-r--r--   0        0        0    12034 2024-04-24 08:27:31.224413 dolphie-5.0.2/dolphie/Widgets/modal.py
+-rw-r--r--   0        0        0     3873 2024-04-24 08:27:31.224676 dolphie-5.0.2/dolphie/Widgets/proxysql_thread_screen.py
+-rw-r--r--   0        0        0      563 2024-02-26 06:55:52.591220 dolphie-5.0.2/dolphie/Widgets/spinner.py
+-rw-r--r--   0        0        0     5997 2024-04-24 08:27:31.225002 dolphie-5.0.2/dolphie/Widgets/thread_screen.py
+-rw-r--r--   0        0        0     1125 2024-02-12 13:50:32.936036 dolphie-5.0.2/dolphie/Widgets/topbar.py
+-rw-r--r--   0        0        0    13455 2024-04-29 07:10:07.370077 dolphie-5.0.2/dolphie/__init__.py
+-rwxr-xr-x   0        0        0    80400 2024-04-30 21:15:44.679230 dolphie-5.0.2/dolphie/app.py
+-rw-r--r--   0        0        0      687 2024-05-09 17:20:22.795392 dolphie-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11874 1970-01-01 00:00:00.000000 dolphie-5.0.2/PKG-INFO
```

### Comparing `dolphie-5.0.1/LICENSE` & `dolphie-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/README.md` & `dolphie-5.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 Note: Use `admin` user instead of `stats` user so you can use all features
 
 ## Supported MariaDB versions
 - MariaDB 5.5/10.0/11.0+
 - RDS MariaDB
 
 ## Supported MySQL versions
-- MySQL/Percona Server 5.6/5.7/8.0+
+- MySQL/Percona Server 5.6/5.7/8.0+/8.4+
 - RDS MySQL & Aurora + Azure
 
 ## MySQL Grants required
 #### Least privilege
 1. PROCESS (only if you switch to using processlist via `P` command)
 2. SELECT to `performance_schema` + `pt-heartbeat table` (if used)
 3. REPLICATION CLIENT/REPLICATION SLAVE
```

#### html2text {}

```diff
@@ -76,17 +76,17 @@
 (str) ssl_cert (str) ssl_key (str) mycnf_file (str) login_path (str)
 host_cache_file (str) host_setup_file (int) refresh_interval (str)
 heartbeat_table (str) startup_panels (str) graph_marker (str) pypi_repository
 (str) hostgroup (bool) show_trxs_only (bool) show_additional_query_columns ```
 ## Supported ProxySQL versions - ProxySQL 2.6+ (could work on previous versions
 but not tested) Note: Use `admin` user instead of `stats` user so you can use
 all features ## Supported MariaDB versions - MariaDB 5.5/10.0/11.0+ - RDS
-MariaDB ## Supported MySQL versions - MySQL/Percona Server 5.6/5.7/8.0+ - RDS
-MySQL & Aurora + Azure ## MySQL Grants required #### Least privilege 1. PROCESS
-(only if you switch to using processlist via `P` command) 2. SELECT to
+MariaDB ## Supported MySQL versions - MySQL/Percona Server 5.6/5.7/8.0+/8.4+ -
+RDS MySQL & Aurora + Azure ## MySQL Grants required #### Least privilege 1.
+PROCESS (only if you switch to using processlist via `P` command) 2. SELECT to
 `performance_schema` + `pt-heartbeat table` (if used) 3. REPLICATION CLIENT/
 REPLICATION SLAVE 4. BACKUP_ADMIN (MySQL 8 only) #### Recommended 1. PROCESS
 (only if you switch to using processlist via `P` command) 2. Global SELECT
 access (good for explaining queries, listing all databases, etc) 4. REPLICATION
 CLIENT/REPLICATION SLAVE 5. SUPER (required if you want to kill queries) 6.
 BACKUP_ADMIN (MySQL 8 only) ## Features - Tabs docked at the top to seamlessly
 switch between connected hosts - Hostgroups to make it easy for connecting to
```

### Comparing `dolphie-5.0.1/dolphie/DataTypes.py` & `dolphie-5.0.2/dolphie/DataTypes.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Dolphie.css` & `dolphie-5.0.2/dolphie/Dolphie.css`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Modules/ArgumentParser.py` & `dolphie-5.0.2/dolphie/Modules/ArgumentParser.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Modules/Functions.py` & `dolphie-5.0.2/dolphie/Modules/Functions.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Modules/ManualException.py` & `dolphie-5.0.2/dolphie/Modules/ManualException.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Modules/MetricManager.py` & `dolphie-5.0.2/dolphie/Modules/MetricManager.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Modules/MySQL.py` & `dolphie-5.0.2/dolphie/Modules/MySQL.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Modules/Queries.py` & `dolphie-5.0.2/dolphie/Modules/Queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,24 @@
     """
     heartbeat_replica_lag: str = """
         SELECT
             TIMESTAMPDIFF(SECOND, MAX(ts), NOW()) AS Seconds_Behind_Master
         FROM
             $1
     """
+    mariadb_find_replicas: str = """
+        SELECT
+            t.THREAD_ID AS id,
+            t.PROCESSLIST_USER AS user,
+            t.PROCESSLIST_HOST AS host
+        FROM
+            `performance_schema`.threads AS t
+        WHERE
+            t.PROCESSLIST_COMMAND LIKE 'Binlog Dump%'
+    """
     ps_find_replicas: str = """
         SELECT
             t.THREAD_ID AS id,
             t.PROCESSLIST_USER AS user,
             t.PROCESSLIST_HOST AS host,
             CONVERT (
                 CAST( CONVERT ( uvt.VARIABLE_VALUE USING latin1 ) AS BINARY ) USING utf8
@@ -528,11 +538,14 @@
             log_type = 'BINARY' AND
             compression_type = 'ZSTD'
         LIMIT
             1
     """
     status: str = "SHOW GLOBAL STATUS"
     variables: str = "SHOW GLOBAL VARIABLES"
-    binlog_status: str = "SHOW MASTER STATUS"
-    replication_status: str = "SHOW SLAVE STATUS"
+    show_master_status: str = "SHOW MASTER STATUS"
+    show_binary_log_status: str = "SHOW BINARY LOG STATUS"
+    show_slave_status: str = "SHOW SLAVE STATUS"
+    show_replica_status: str = "SHOW REPLICA STATUS"
     innodb_status: str = "SHOW ENGINE INNODB STATUS"
-    get_replicas: str = "SHOW SLAVE HOSTS"
+    show_replicas: str = "SHOW REPLICAS"
+    show_slave_hosts: str = "SHOW SLAVE HOSTS"
```

### Comparing `dolphie-5.0.1/dolphie/Modules/TabManager.py` & `dolphie-5.0.2/dolphie/Modules/TabManager.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Panels/dashboard_panel.py` & `dolphie-5.0.2/dolphie/Panels/dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Panels/ddl_panel.py` & `dolphie-5.0.2/dolphie/Panels/ddl_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Panels/innodb_trx_locks_panel.py` & `dolphie-5.0.2/dolphie/Panels/innodb_trx_locks_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Panels/metadata_locks_panel.py` & `dolphie-5.0.2/dolphie/Panels/metadata_locks_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Panels/processlist_panel.py` & `dolphie-5.0.2/dolphie/Panels/processlist_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Panels/proxysql_command_stats_panel.py` & `dolphie-5.0.2/dolphie/Panels/proxysql_command_stats_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Panels/proxysql_dashboard_panel.py` & `dolphie-5.0.2/dolphie/Panels/proxysql_dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Panels/proxysql_hostgroup_summary_panel.py` & `dolphie-5.0.2/dolphie/Panels/proxysql_hostgroup_summary_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Panels/proxysql_mysql_query_rules_panel.py` & `dolphie-5.0.2/dolphie/Panels/proxysql_mysql_query_rules_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Panels/proxysql_processlist_panel.py` & `dolphie-5.0.2/dolphie/Panels/proxysql_processlist_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Panels/replication_panel.py` & `dolphie-5.0.2/dolphie/Panels/replication_panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import socket
 
 from dolphie.DataTypes import ConnectionSource, Replica
 from dolphie.Modules.Functions import format_number, format_time
 from dolphie.Modules.ManualException import ManualException
 from dolphie.Modules.MySQL import Database
 from dolphie.Modules.Queries import MySQLQueries
 from dolphie.Modules.TabManager import Tab
@@ -153,27 +154,34 @@
             tab.replication_thread_applier.update(table_thread_applier_status)
             tab.replication_thread_applier_container.display = True
         else:
             tab.replication_thread_applier_container.display = False
 
         if tab.dolphie.connection_source_alt == ConnectionSource.mariadb:
             available_replication_variables = {
-                "gtid_domain_id": "gtid_domain_id",
                 "slave_parallel_mode": "parallel_mode",
                 "slave_parallel_workers": "parallel_workers",
                 "slave_parallel_threads": "parallel_threads",
-                "slave_domain_parallel_threads": "domain_parallel_threads",
+                "log_slave_updates": "log_slave_updates",
             }
         else:
-            available_replication_variables = {
-                "binlog_transaction_dependency_tracking": "dependency_tracking",
-                "slave_parallel_type": "parallel_type",
-                "slave_parallel_workers": "parallel_workers",
-                "slave_preserve_commit_order": "preserve_commit_order",
-            }
+            if dolphie.is_mysql_version_at_least("8.0"):
+                available_replication_variables = {
+                    "replica_parallel_type": "parallel_type",
+                    "replica_parallel_workers": "parallel_workers",
+                    "replica_preserve_commit_order": "preserve_commit_order",
+                    "log_replica_updates": "log_replica_updates",
+                }
+            else:
+                available_replication_variables = {
+                    "slave_parallel_type": "parallel_type",
+                    "slave_parallel_workers": "parallel_workers",
+                    "slave_preserve_commit_order": "preserve_commit_order",
+                    "log_slave_updates": "log_slave_updates",
+                }
 
         replication_variables = ""
         for setting_variable, setting_display_name in available_replication_variables.items():
             value = dolphie.global_variables.get(setting_variable, "N/A")
             replication_variables += f"[b light_blue]{setting_display_name}[/b light_blue] {value}  "
         replication_variables = replication_variables.strip()
 
@@ -263,25 +271,58 @@
         if replica_lag >= 20:
             lag_color = "red"
         elif replica_lag >= 10:
             lag_color = "yellow"
 
         lag = f"[{lag_color}]{format_time(replica_lag)}[/{lag_color}]"
 
-    data["Master_Host"] = dolphie.get_hostname(data["Master_Host"])
+    if dolphie.is_mysql_version_at_least("8.0") and dolphie.connection_source_alt != ConnectionSource.mariadb:
+        primary_uuid = data.get("Source_UUID")
+        primary_host = dolphie.get_hostname(data.get("Source_Host"))
+        primary_user = data.get("Source_User")
+        primary_log_file = data.get("Source_Log_File")
+        primary_ssl_allowed = data.get("Source_SSL_Allowed")
+        relay_primary_log_file = data.get("Relay_Source_Log_File")
+        replica_sql_running_state = data.get("Replica_SQL_Running_State")
+        replica_io_state = data.get("Replica_IO_State")
+        read_primary_log_pos = data.get("Read_Source_Log_Pos")
+        exec_primary_log_pos = data.get("Exec_Source_Log_Pos")
+
+        io_thread_running = "[green]ON[/green]" if data.get("Replica_IO_Running").lower() == "yes" else "[red]OFF[/red]"
+        sql_thread_running = (
+            "[green]ON[/green]" if data.get("Replica_SQL_Running").lower() == "yes" else "[red]OFF[/red]"
+        )
+
+    else:
+        primary_uuid = data.get("Master_UUID")
+        primary_host = dolphie.get_hostname(data.get("Master_Host"))
+        primary_user = data.get("Master_User")
+        primary_log_file = data.get("Master_Log_File")
+        primary_ssl_allowed = data.get("Master_SSL_Allowed")
+        relay_primary_log_file = data.get("Relay_Master_Log_File")
+        replica_sql_running_state = data.get("Slave_SQL_Running_State")
+        replica_io_state = data.get("Slave_IO_State")
+        read_primary_log_pos = data.get("Read_Master_Log_Pos")
+        exec_primary_log_pos = data.get("Exec_Master_Log_Pos")
+
+        io_thread_running = "[green]ON[/green]" if data.get("Slave_IO_Running").lower() == "yes" else "[red]OFF[/red]"
+        sql_thread_running = "[green]ON[/green]" if data.get("Slave_SQL_Running").lower() == "yes" else "[red]OFF[/red]"
+
     mysql_gtid_enabled = False
     mariadb_gtid_enabled = False
     gtid_status = "OFF"
-    if "Executed_Gtid_Set" in data and data["Executed_Gtid_Set"]:
+
+    using_gtid = data.get("Using_Gtid")
+    if using_gtid and using_gtid != "No":
+        mariadb_gtid_enabled = True
+        gtid_status = using_gtid
+    elif data.get("Executed_Gtid_Set"):
         mysql_gtid_enabled = True
-        auto_position = "ON" if data["Auto_Position"] == 1 else "OFF"
+        auto_position = "ON" if data.get("Auto_Position") == 1 else "OFF"
         gtid_status = f"ON [label]Auto Position[/label] {auto_position}"
-    if "Using_Gtid" in data and data["Using_Gtid"] != "No":
-        mariadb_gtid_enabled = True
-        gtid_status = data["Using_Gtid"]
 
     table = Table(show_header=False, box=None)
     if dashboard_table:
         table = Table(
             show_header=False,
             box=None,
             expand=True,
@@ -296,71 +337,65 @@
         table.add_column()
         table.add_column(overflow="fold")
 
     if replica:
         table.add_row("[b][light_blue]Host", "[light_blue]%s" % replica.host)
         table.add_row("[label]Version", "%s" % replica.mysql_version)
     else:
-        table.add_row("[label]Primary", "%s" % data["Master_Host"])
+        table.add_row("[label]Primary", "%s" % primary_host)
 
     if not dashboard_table:
-        table.add_row("[label]User", "%s" % data["Master_User"])
+        table.add_row("[label]User", "%s" % primary_user)
 
-    io_thread_running = "[green]ON[/green]" if data.get("Slave_IO_Running").lower() == "yes" else "[red]OFF[/red]"
-    sql_thread_running = "[green]ON[/green]" if data.get("Slave_SQL_Running").lower() == "yes" else "[red]OFF[/red]"
     table.add_row(
         "[label]Thread",
         f"[label]IO[/label] {io_thread_running} [label]SQL[/label] {sql_thread_running}",
     )
 
     replication_delay = ""
     if data["SQL_Delay"]:
         if dashboard_table:
             replication_delay = "[dark_yellow](delayed)"
         else:
             replication_delay = f"[dark_yellow]Delay[/dark_yellow] {format_time(data['SQL_Delay'])}"
 
     lag_source = f"Lag ({replica_sbm_source})" if replica_sbm_source else "Lag"
-    if lag is None or data["Slave_SQL_Running"].lower() == "no":
+    if lag is None or sql_thread_running == "[red]OFF[/red]":
         table.add_row(f"[label]{lag_source}", "")
     else:
         table.add_row(
             "[label]%s" % lag_source,
             "%s [label]Speed[/label] %s %s" % (lag, speed, replication_delay),
         )
 
     if dashboard_table:
-        table.add_row("[label]Binlog IO", "%s" % (data["Master_Log_File"]))
-        table.add_row("[label]Binlog SQL", "%s" % (data["Relay_Master_Log_File"]))
-        table.add_row("[label]Relay Log ", "%s" % (data["Relay_Log_File"]))
+        table.add_row("[label]Binlog IO", "%s" % primary_log_file)
+        table.add_row("[label]Binlog SQL", "%s" % relay_primary_log_file)
+        table.add_row("[label]Relay Log ", "%s" % data["Relay_Log_File"])
         table.add_row("[label]GTID", "%s" % gtid_status)
-        table.add_row("[label]State", "%s" % data["Slave_SQL_Running_State"])
+        table.add_row("[label]State", "%s" % replica_sql_running_state)
     else:
         table.add_row(
             "[label]Binlog IO",
-            "%s ([dark_gray]%s[/dark_gray])" % (data["Master_Log_File"], data["Read_Master_Log_Pos"]),
+            "%s ([dark_gray]%s[/dark_gray])" % (primary_log_file, read_primary_log_pos),
         )
         table.add_row(
             "[label]Binlog SQL",
-            "%s ([dark_gray]%s[/dark_gray])"
-            % (
-                data["Relay_Master_Log_File"],
-                data["Exec_Master_Log_Pos"],
-            ),
+            "%s ([dark_gray]%s[/dark_gray])" % (relay_primary_log_file, exec_primary_log_pos),
         )
         table.add_row(
             "[label]Relay Log",
             "%s ([dark_gray]%s[/dark_gray])" % (data["Relay_Log_File"], data["Relay_Log_Pos"]),
         )
 
     if dashboard_table:
         table.add_row("[label]GTID", "%s" % gtid_status)
-        table.add_row("[label]State", "%s" % data["Slave_SQL_Running_State"])
+        table.add_row("[label]State", "%s" % replica_sql_running_state)
     else:
-        ssl_enabled = "ON" if data.get("Master_SSL_Allowed") == "Yes" else "OFF"
+        ssl_enabled = "ON" if primary_ssl_allowed == "Yes" else "OFF"
         table.add_row("[label]SSL", "%s" % ssl_enabled)
 
         replication_status_filtering = [
             "Replicate_Do_DB",
             "Replicate_Ignore_Table",
             "Replicate_Ignore_DB",
             "Replicate_Do_Table",
@@ -379,19 +414,18 @@
         error_types = ["Last_IO_Error", "Last_SQL_Error"]
         errors = [(error_type, data[error_type]) for error_type in error_types if data[error_type]]
 
         if errors:
             for error_type, error_message in errors:
                 table.add_row("[label]%s" % error_type.replace("_", " "), "[red]%s[/red]" % error_message)
         else:
-            table.add_row("[label]IO State", "%s" % data["Slave_IO_State"])
-            table.add_row("[label]SQL State", "%s" % data["Slave_SQL_Running_State"])
+            table.add_row("[label]IO State", "%s" % replica_io_state)
+            table.add_row("[label]SQL State", "%s" % replica_sql_running_state)
 
         if mysql_gtid_enabled:
-            primary_uuid = data["Master_UUID"]
             executed_gtid_set = data["Executed_Gtid_Set"]
             retrieved_gtid_set = data["Retrieved_Gtid_Set"]
 
             table.add_row("[label]GTID", "%s" % gtid_status)
 
             if replica:
                 replica_primary_server_uuid = None
@@ -452,15 +486,42 @@
             pattern = re.compile(r"\b(\w+(?:-\w+){4}):(.+)\b")
             retrieved_gtid_set = pattern.sub(color_gtid_set, retrieved_gtid_set.replace(",", ""))
             executed_gtid_set = pattern.sub(color_gtid_set, executed_gtid_set.replace(",", ""))
 
             table.add_row("[label]Retrieved GTID", "%s" % retrieved_gtid_set)
             table.add_row("[label]Executed GTID", "%s" % executed_gtid_set)
         elif mariadb_gtid_enabled:
-            table.add_row("[label]GTID IO Pos", "%s" % data.get("Gtid_IO_Pos"))
+            primary_id = data.get("Master_Server_Id")
+
+            table.add_row("[label]GTID", gtid_status)
+
+            # Check if GTID IO position exists
+            gtid_io_pos = data.get("Gtid_IO_Pos")
+            # gtid_io_pos = "1-1-3323,1-2-32,1-3-5543,1-4-554454"
+            if gtid_io_pos:
+                # If this is a replica, use its primary server ID, else use its own server ID
+                if replica:
+                    replica_primary_server_id = dolphie.replication_status.get("Master_Server_Id")
+                    if replica_primary_server_id:
+                        primary_id = replica_primary_server_id
+                    else:
+                        primary_id = dolphie.global_variables.get("server_id")
+
+                gtids = gtid_io_pos.split(",")
+                for idx, gtid in enumerate(gtids):
+                    server_id = gtid.split("-")[1]
+
+                    if str(server_id) == str(primary_id):
+                        # Highlight GTID if it matches the primary ID
+                        gtids[idx] = f"[highlight]{gtid}[/highlight]"
+                    else:
+                        # Otherwise, darken GTID
+                        gtids[idx] = f"[dark_gray]{gtid}[/dark_gray]"
+
+                table.add_row("[label]GTID IO Pos", "\n".join(gtids))
 
     return table
 
 
 def create_group_replication_member_table(tab: Tab):
     dolphie = tab.dolphie
 
@@ -525,34 +586,47 @@
 
 
 def fetch_replication_data(tab: Tab, replica: Replica = None) -> tuple:
     dolphie = tab.dolphie
 
     connection = dolphie.main_db_connection if not replica else replica.connection
 
+    # Determine which query to use based on MySQL version and connection source
+    replication_status_query = (
+        MySQLQueries.show_replica_status
+        if dolphie.is_mysql_version_at_least("8.0") and dolphie.connection_source_alt != ConnectionSource.mariadb
+        else MySQLQueries.show_slave_status
+    )
+
     # Determine which replication lag source and query to use
     if dolphie.heartbeat_table:
         replica_lag_source = "HB"
         replica_lag_query = MySQLQueries.heartbeat_replica_lag
     else:
         replica_lag_source = None
-        replica_lag_query = MySQLQueries.replication_status
+        replica_lag_query = replication_status_query
 
-    connection.execute(MySQLQueries.replication_status)
+    connection.execute(replication_status_query)
     replica_lag_data = connection.fetchone()
     replication_status = replica_lag_data
 
     # Use an alternative method to detect replication lag if available
     if replication_status and replica_lag_source:
         connection.execute(replica_lag_query)
         replica_lag_data = connection.fetchone()
 
-    # Extract lag value from fetched data
-    replica_lag = replica_lag_data.get("Seconds_Behind_Master") if replica_lag_data else None
-    replica_lag = int(replica_lag) if replica_lag is not None else 0
+    # Determine which key to use for fetching the seconds behind
+    seconds_behind_key = (
+        "Seconds_Behind_Source"
+        if dolphie.is_mysql_version_at_least("8.0") and dolphie.connection_source_alt != ConnectionSource.mariadb
+        else "Seconds_Behind_Master"
+    )
+
+    seconds_behind = replica_lag_data.get(seconds_behind_key)
+    replica_lag = int(seconds_behind) if seconds_behind is not None else 0
 
     return replica_lag_source, replica_lag, replication_status
 
 
 def fetch_replicas(tab: Tab):
     dolphie = tab.dolphie
 
@@ -566,15 +640,39 @@
 
     for row in dolphie.replica_manager.available_replicas:
         replica_error = None
 
         thread_id = row["id"]
 
         host = dolphie.get_hostname(row["host"].split(":")[0])
-        port = dolphie.replica_manager.ports.get(row["replica_uuid"], 3306)
+
+        # MariaDB has no way of knowing what port a replica is using, so we have to manage it ourselves
+        if dolphie.connection_source_alt == ConnectionSource.mariadb:
+            # Loop through available ports
+            for port_data in dolphie.replica_manager.ports.values():
+                port = port_data.get("port", 3306)
+
+                # If the port is not in use, check to see if we can connect to it
+                if not port_data.get("in_use"):
+                    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+                    sock.settimeout(2)
+
+                    try:
+                        # Try to connect to the host and port
+                        sock.connect((host, port))
+                        port_data["in_use"] = True
+                        break
+                    except (socket.timeout, socket.error, ConnectionRefusedError):
+                        continue  # Continue to the next available port
+                    finally:
+                        sock.close()
+                else:
+                    break
+        else:
+            port = dolphie.replica_manager.ports.get(row["replica_uuid"], {}).get("port", 3306)
 
         # This lets us connect to replicas on the same host as the primary if we're connecting remotely
         if host == "localhost" or host == "127.0.0.1":
             host = dolphie.host
 
         host_and_port = "%s:%s" % (host, port)
```

### Comparing `dolphie-5.0.1/dolphie/Widgets/command_screen.py` & `dolphie-5.0.2/dolphie/Widgets/command_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Widgets/event_log_screen.py` & `dolphie-5.0.2/dolphie/Widgets/event_log_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Widgets/help.py` & `dolphie-5.0.2/dolphie/Widgets/help.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Widgets/host_setup.py` & `dolphie-5.0.2/dolphie/Widgets/host_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,19 @@
             layout: horizontal;
         }
         HostSetupModal AutoComplete {
             width: 100%;
             height: auto;
         }
         HostSetupModal #password {
-            width: 84%;
+            width: 88%;
         }
         HostSetupModal #show_password {
-            max-width: 12%;
+            max-width: 13%;
+            height: 3;
             background:  #262c4b;
             border: blank #344063;
         }
         HostSetupModal #show_password:hover {
             background:  #313960;
             border: blank #344063;
         }
```

### Comparing `dolphie-5.0.1/dolphie/Widgets/modal.py` & `dolphie-5.0.2/dolphie/Widgets/modal.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Widgets/proxysql_thread_screen.py` & `dolphie-5.0.2/dolphie/Widgets/proxysql_thread_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Widgets/spinner.py` & `dolphie-5.0.2/dolphie/Widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Widgets/thread_screen.py` & `dolphie-5.0.2/dolphie/Widgets/thread_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/Widgets/topbar.py` & `dolphie-5.0.2/dolphie/Widgets/topbar.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/__init__.py` & `dolphie-5.0.2/dolphie/__init__.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.1/dolphie/app.py` & `dolphie-5.0.2/dolphie/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,28 +275,43 @@
         dolphie = tab.dolphie
 
         dolphie.global_variables = dolphie.main_db_connection.fetch_status_and_variables("variables")
         dolphie.global_status = dolphie.main_db_connection.fetch_status_and_variables("status")
         dolphie.innodb_metrics = dolphie.main_db_connection.fetch_status_and_variables("innodb_metrics")
 
         if dolphie.performance_schema_enabled and dolphie.is_mysql_version_at_least("5.7"):
-            find_replicas_query = MySQLQueries.ps_find_replicas
+            if dolphie.connection_source_alt == ConnectionSource.mariadb:
+                find_replicas_query = MySQLQueries.mariadb_find_replicas
+            else:
+                find_replicas_query = MySQLQueries.ps_find_replicas
         else:
             find_replicas_query = MySQLQueries.pl_find_replicas
 
         dolphie.main_db_connection.execute(find_replicas_query)
         available_replicas = dolphie.main_db_connection.fetchall()
         # We update the replica ports used if the number of replicas have changed
         if len(available_replicas) != len(dolphie.replica_manager.available_replicas):
             dolphie.replica_manager.ports = {}
 
-            dolphie.main_db_connection.execute(MySQLQueries.get_replicas)
+            if dolphie.is_mysql_version_at_least("8.0") and dolphie.connection_source_alt != ConnectionSource.mariadb:
+                dolphie.main_db_connection.execute(MySQLQueries.show_replicas)
+            else:
+                dolphie.main_db_connection.execute(MySQLQueries.show_slave_hosts)
+
             replica_data = dolphie.main_db_connection.fetchall()
             for row in replica_data:
-                dolphie.replica_manager.ports[row["Slave_UUID"]] = row["Port"]
+                if dolphie.connection_source_alt == ConnectionSource.mariadb:
+                    key = "Server_id"
+                else:
+                    if dolphie.is_mysql_version_at_least("8.0"):
+                        key = "Replica_UUID"
+                    else:
+                        key = "Slave_UUID"
+
+                dolphie.replica_manager.ports[row.get(key)] = {"port": row.get("Port"), "in_use": False}
 
             dolphie.replica_manager.available_replicas = available_replicas
 
         dolphie.main_db_connection.execute(MySQLQueries.ps_disk_io)
         dolphie.disk_io_metrics = dolphie.main_db_connection.fetchone()
 
         dolphie.previous_replica_sbm = dolphie.replica_lag
@@ -304,15 +319,15 @@
             replication_panel.fetch_replication_data(tab)
         )
 
         # If using MySQL 8, fetch the replication applier status data
         if (
             dolphie.is_mysql_version_at_least("8.0")
             and dolphie.panels.replication.visible
-            and dolphie.global_variables.get("slave_parallel_workers", 0) > 1
+            and dolphie.global_variables.get("replica_parallel_workers", 0) > 1
         ):
             dolphie.main_db_connection.execute(MySQLQueries.replication_applier_status)
             dolphie.replication_applier_status = dolphie.main_db_connection.fetchall()
 
         dolphie.massage_metrics_data()
 
         if dolphie.group_replication or dolphie.innodb_cluster:
@@ -327,15 +342,18 @@
                     member_role_data.get("MEMBER_ID") == dolphie.server_uuid
                     and member_role_data.get("MEMBER_ROLE") == "PRIMARY"
                 ):
                     dolphie.is_group_replication_primary = True
                     break
 
         if dolphie.panels.dashboard.visible:
-            dolphie.main_db_connection.execute(MySQLQueries.binlog_status)
+            if dolphie.is_mysql_version_at_least("8.2.0") and dolphie.connection_source_alt != ConnectionSource.mariadb:
+                dolphie.main_db_connection.execute(MySQLQueries.show_binary_log_status)
+            else:
+                dolphie.main_db_connection.execute(MySQLQueries.show_master_status)
             dolphie.binlog_status = dolphie.main_db_connection.fetchone()
 
             # This can cause MySQL to crash: https://perconadev.atlassian.net/browse/PS-9066
             # if dolphie.global_variables.get("binlog_transaction_compression") == "ON":
             #     dolphie.main_db_connection.execute(MySQLQueries.get_binlog_transaction_compression_percentage)
             #     dolphie.binlog_transaction_compression_percentage = dolphie.main_db_connection.fetchone().get(
             #         "compression_percentage"
@@ -1604,22 +1622,20 @@
 
                     if transaction_history:
                         transaction_history_table = Table(box=None)
                         transaction_history_table.add_column("Start Time")
                         transaction_history_table.add_column("Query", overflow="fold")
 
                         for query in transaction_history:
-                            trx_history_formatted_query = query["sql_text"]
-                            if trx_history_formatted_query:
-                                trx_history_formatted_query = sqlformat(
-                                    trx_history_formatted_query, reindent_aligned=True
+                            trx_history_formatted_query = ""
+                            if query["sql_text"]:
+                                trx_history_formatted_query = format_query(
+                                    sqlformat(query["sql_text"], reindent_aligned=True), minify=False
                                 )
 
-                            trx_history_formatted_query = format_query(trx_history_formatted_query, minify=False)
-
                             transaction_history_table.add_row(
                                 query["start_time"].strftime("%Y-%m-%d %H:%M:%S"), trx_history_formatted_query
                             )
 
                 self.call_from_thread(show_thread_screen)
 
             elif key == "u":
```

### Comparing `dolphie-5.0.1/pyproject.toml` & `dolphie-5.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "dolphie"
-version = "5.0.1"
+version = "5.0.2"
 license = "GPL-3.0-or-later"
-description = "Your single pane of glass for real-time analytics into MySQL & ProxySQL"
+description = "Your single pane of glass for real-time analytics into MySQL/MariaDB & ProxySQL"
 authors = ["Charles Thompson <01charles.t@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^13.7.1"
 pymysql = "^1.1.0"
 myloginpath = "^0.0.4"
 packaging = "^24.0"
 requests = "^2.31.0"
 sqlparse = "^0.4.4"
-textual = {extras = ["syntax"], version = "^0.57.1"}
+textual = {extras = ["syntax"], version = "^0.58.1"}
 textual-autocomplete = "^2.1.0b0"
 charset-normalizer = "^3.3.2"
 plotext = "^5.2.8"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dolphie-5.0.1/PKG-INFO` & `dolphie-5.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dolphie
-Version: 5.0.1
-Summary: Your single pane of glass for real-time analytics into MySQL & ProxySQL
+Version: 5.0.2
+Summary: Your single pane of glass for real-time analytics into MySQL/MariaDB & ProxySQL
 License: GPL-3.0-or-later
 Author: Charles Thompson
 Author-email: 01charles.t@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: plotext (>=5.2.8,<6.0.0)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
 Requires-Dist: textual-autocomplete (>=2.1.0b0,<3.0.0)
-Requires-Dist: textual[syntax] (>=0.57.1,<0.58.0)
+Requires-Dist: textual[syntax] (>=0.58.1,<0.59.0)
 Description-Content-Type: text/markdown
 
 # Dolphie
 <p align="center">
   <img src="https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-4f9c-ada5-a153cdcf4070.png" width="120"><br>
   Your single pane of glass for real-time analytics into MySQL/MariaDB & ProxySQL<br><br>
   <img src="https://github.com/charles-001/dolphie/assets/13244625/88a41290-f52c-4b8e-97f8-3b7ef5096eae" width="30">
@@ -182,15 +182,15 @@
 Note: Use `admin` user instead of `stats` user so you can use all features
 
 ## Supported MariaDB versions
 - MariaDB 5.5/10.0/11.0+
 - RDS MariaDB
 
 ## Supported MySQL versions
-- MySQL/Percona Server 5.6/5.7/8.0+
+- MySQL/Percona Server 5.6/5.7/8.0+/8.4+
 - RDS MySQL & Aurora + Azure
 
 ## MySQL Grants required
 #### Least privilege
 1. PROCESS (only if you switch to using processlist via `P` command)
 2. SELECT to `performance_schema` + `pt-heartbeat table` (if used)
 3. REPLICATION CLIENT/REPLICATION SLAVE
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: dolphie Version: 5.0.1 Summary: Your single pane of
-glass for real-time analytics into MySQL & ProxySQL License: GPL-3.0-or-later
-Author: Charles Thompson Author-email: 01charles.t@gmail.com Requires-Python:
->=3.8,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
-or later (GPLv3+) Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: charset-normalizer
-(>=3.3.2,<4.0.0) Requires-Dist: myloginpath (>=0.0.4,<0.0.5) Requires-Dist:
-packaging (>=24.0,<25.0) Requires-Dist: plotext (>=5.2.8,<6.0.0) Requires-Dist:
-pymysql (>=1.1.0,<2.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-
-Dist: rich (>=13.7.1,<14.0.0) Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
-Requires-Dist: textual-autocomplete (>=2.1.0b0,<3.0.0) Requires-Dist: textual
-[syntax] (>=0.57.1,<0.58.0) Description-Content-Type: text/markdown # Dolphie
+Metadata-Version: 2.1 Name: dolphie Version: 5.0.2 Summary: Your single pane of
+glass for real-time analytics into MySQL/MariaDB & ProxySQL License: GPL-3.0-
+or-later Author: Charles Thompson Author-email: 01charles.t@gmail.com Requires-
+Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: GNU General Public
+License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: charset-
+normalizer (>=3.3.2,<4.0.0) Requires-Dist: myloginpath (>=0.0.4,<0.0.5)
+Requires-Dist: packaging (>=24.0,<25.0) Requires-Dist: plotext (>=5.2.8,<6.0.0)
+Requires-Dist: pymysql (>=1.1.0,<2.0.0) Requires-Dist: requests
+(>=2.31.0,<3.0.0) Requires-Dist: rich (>=13.7.1,<14.0.0) Requires-Dist:
+sqlparse (>=0.4.4,<0.5.0) Requires-Dist: textual-autocomplete
+(>=2.1.0b0,<3.0.0) Requires-Dist: textual[syntax] (>=0.58.1,<0.59.0)
+Description-Content-Type: text/markdown # Dolphie
  [https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-
                           4f9c-ada5-a153cdcf4070.png]
 Your single pane of glass for real-time analytics into MySQL/MariaDB & ProxySQL
 
   [https://github.com/charles-001/dolphie/assets/13244625/88a41290-f52c-4b8e-
   97f8-3b7ef5096eae][https://github.com/charles-001/dolphie/assets/13244625/
  1d94502a-9abf-4436-a7d0-cb2b08c105c1][https://github.com/charles-001/dolphie/
@@ -89,17 +90,17 @@
 (str) ssl_cert (str) ssl_key (str) mycnf_file (str) login_path (str)
 host_cache_file (str) host_setup_file (int) refresh_interval (str)
 heartbeat_table (str) startup_panels (str) graph_marker (str) pypi_repository
 (str) hostgroup (bool) show_trxs_only (bool) show_additional_query_columns ```
 ## Supported ProxySQL versions - ProxySQL 2.6+ (could work on previous versions
 but not tested) Note: Use `admin` user instead of `stats` user so you can use
 all features ## Supported MariaDB versions - MariaDB 5.5/10.0/11.0+ - RDS
-MariaDB ## Supported MySQL versions - MySQL/Percona Server 5.6/5.7/8.0+ - RDS
-MySQL & Aurora + Azure ## MySQL Grants required #### Least privilege 1. PROCESS
-(only if you switch to using processlist via `P` command) 2. SELECT to
+MariaDB ## Supported MySQL versions - MySQL/Percona Server 5.6/5.7/8.0+/8.4+ -
+RDS MySQL & Aurora + Azure ## MySQL Grants required #### Least privilege 1.
+PROCESS (only if you switch to using processlist via `P` command) 2. SELECT to
 `performance_schema` + `pt-heartbeat table` (if used) 3. REPLICATION CLIENT/
 REPLICATION SLAVE 4. BACKUP_ADMIN (MySQL 8 only) #### Recommended 1. PROCESS
 (only if you switch to using processlist via `P` command) 2. Global SELECT
 access (good for explaining queries, listing all databases, etc) 4. REPLICATION
 CLIENT/REPLICATION SLAVE 5. SUPER (required if you want to kill queries) 6.
 BACKUP_ADMIN (MySQL 8 only) ## Features - Tabs docked at the top to seamlessly
 switch between connected hosts - Hostgroups to make it easy for connecting to
```

