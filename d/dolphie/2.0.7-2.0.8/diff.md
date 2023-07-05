# Comparing `tmp/dolphie-2.0.7.tar.gz` & `tmp/dolphie-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolphie-2.0.7.tar", max compression
+gzip compressed data, was "dolphie-2.0.8.tar", max compression
```

## Comparing `dolphie-2.0.7.tar` & `dolphie-2.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-2.0.7/LICENSE
--rw-r--r--   0        0        0     7167 2023-07-04 03:13:04.900371 dolphie-2.0.7/README.md
--rw-r--r--   0        0        0     1574 2023-07-04 07:09:03.000115 dolphie-2.0.7/dolphie/Database.py
--rw-r--r--   0        0        0     2826 2023-07-03 06:21:35.269967 dolphie-2.0.7/dolphie/Functions.py
--rw-r--r--   0        0        0     2002 2023-07-02 09:17:46.754079 dolphie-2.0.7/dolphie/KBHit.py
--rw-r--r--   0        0        0    16417 2023-07-03 06:53:04.526750 dolphie-2.0.7/dolphie/Panels/dashboard_panel.py
--rw-r--r--   0        0        0    11491 2023-07-03 01:59:19.386574 dolphie-2.0.7/dolphie/Panels/innodb_io_panel.py
--rw-r--r--   0        0        0     5316 2023-07-04 07:06:37.671790 dolphie-2.0.7/dolphie/Panels/innodb_locks_panel.py
--rw-r--r--   0        0        0    10056 2023-07-04 07:07:44.990022 dolphie-2.0.7/dolphie/Panels/processlist_panel.py
--rw-r--r--   0        0        0    11948 2023-07-04 03:00:00.226598 dolphie-2.0.7/dolphie/Panels/replica_panel.py
--rw-r--r--   0        0        0     8209 2023-07-03 06:52:07.577508 dolphie-2.0.7/dolphie/Queries.py
--rw-r--r--   0        0        0    51168 2023-07-04 07:26:33.046048 dolphie-2.0.7/dolphie/__init__.py
--rwxr-xr-x   0        0        0    15809 2023-07-04 07:00:32.285625 dolphie-2.0.7/dolphie/app.py
--rw-r--r--   0        0        0      521 2023-07-04 07:27:31.273098 dolphie-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     7933 1970-01-01 00:00:00.000000 dolphie-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-2.0.8/LICENSE
+-rw-r--r--   0        0        0     7136 2023-07-05 06:43:11.352701 dolphie-2.0.8/README.md
+-rw-r--r--   0        0        0     1673 2023-07-05 04:28:57.836097 dolphie-2.0.8/dolphie/Database.py
+-rw-r--r--   0        0        0     2826 2023-07-03 06:21:35.269967 dolphie-2.0.8/dolphie/Functions.py
+-rw-r--r--   0        0        0     2002 2023-07-02 09:17:46.754079 dolphie-2.0.8/dolphie/KBHit.py
+-rw-r--r--   0        0        0    16417 2023-07-03 06:53:04.526750 dolphie-2.0.8/dolphie/Panels/dashboard_panel.py
+-rw-r--r--   0        0        0    11491 2023-07-03 01:59:19.386574 dolphie-2.0.8/dolphie/Panels/innodb_io_panel.py
+-rw-r--r--   0        0        0     5316 2023-07-04 07:06:37.671790 dolphie-2.0.8/dolphie/Panels/innodb_locks_panel.py
+-rw-r--r--   0        0        0    10056 2023-07-04 07:07:44.990022 dolphie-2.0.8/dolphie/Panels/processlist_panel.py
+-rw-r--r--   0        0        0    11948 2023-07-04 03:00:00.226598 dolphie-2.0.8/dolphie/Panels/replica_panel.py
+-rw-r--r--   0        0        0     8209 2023-07-03 06:52:07.577508 dolphie-2.0.8/dolphie/Queries.py
+-rw-r--r--   0        0        0    51188 2023-07-05 06:41:45.858342 dolphie-2.0.8/dolphie/__init__.py
+-rwxr-xr-x   0        0        0    15809 2023-07-04 07:00:32.285625 dolphie-2.0.8/dolphie/app.py
+-rw-r--r--   0        0        0      521 2023-07-05 06:42:16.979477 dolphie-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7902 1970-01-01 00:00:00.000000 dolphie-2.0.8/PKG-INFO
```

### Comparing `dolphie-2.0.7/LICENSE` & `dolphie-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.7/README.md` & `dolphie-2.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Dolphie
 <p align="center">
 <img src="https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-4f9c-ada5-a153cdcf4070.png" width="120"><br>
 An intuitive feature-rich top tool for monitoring MySQL in real time
 </p>
 
 ## Installation
-Must be using Python 3.8+
+Requires Python 3.8+
 
 Using PyPi:
 ```shell
 pip install dolphie
 ```
 
 Using Poetry:
@@ -19,53 +19,14 @@
 poetry install
 ```
 
 ## Using Docker container
 1. `docker pull ghcr.io/charles-001/dolphie:latest`
 2. `docker run -dit --name dolphie ghcr.io/charles-001/dolphie:latest`
 3. `docker exec -it dolphie dolphie -h host.docker.internal -u root --ask-pass` (pass any additional parameters you'd like)
-5. Enjoy!
-
-## Supported MySQL versions
-- MySQL/Percona Server 5.5/5.6/5.7/8.0
-- MariaDB 10+
-- RDS/Aurora
-
-## Grants required
-#### Least privilege
-1. PROCESS
-2. SELECT to `performance_schema` (if used) + `pt-heartbeat table` (if used)
-3. REPLICATION CLIENT
-
-#### Recommended
-1. PROCESS
-2. Global SELECT access (good for explaining queries, listing all databases, etc)
-4. REPLICATION CLIENT
-5. SUPER (only required if you want to kill queries)
-
-## Features
-- Dolphie uses panels to present groups of data. They can all be turned on/off to have a view of your database server that you prefer (see Help screenshot for panels available)
-- Prefers Performance Schema over Processlist if it's turned on for listing queries. Can be switched to use Processlist by pressing key "1" (or using parameter) since P_S can truncate query length for explaining queries
-- 3 options for finding replica lag in this order of precedence: 
-  - `Performance Schema` (MySQL 8 only - most accurate, especially for multi-threaded replication)
-  - `pt-heartbeat table` (specified by parameter)
-  - `SHOW SLAVE STATUS`
-- Host cache file. This provides users a way to specify hostnames for IPs when their network's DNS can't resolve them. An example use case for this is when you connect to your work's VPN and DNS isn't available to resolve IPs. In my opinion, it's a lot easier to look at hostnames than IPs!
-- Supports encrypted login credentials via `mysql_config_editor`
-- Automatic conversion of large numbers & bytes to human-readable
-- Notifies when new version is available
-- Many commands at your fingertips (see Help screenshot)
-- Many valuable statisitics across the available panels that can help you troubleshoot issues and be proactive against them
-
-## Things to note
-Order of precedence for variables passed to Dolphie:
-1. Parameters via command-line
-2. Environment variables
-3. ~/.mylogin.cnf (`mysql_config_editor`)
-4. ~/.my.cnf
 
 ## Usage
 ```
 options:
   --help                show this help message and exit
   -u USER, --user USER  Username for MySQL
   -p PASSWORD, --password PASSWORD
@@ -121,14 +82,52 @@
     DOLPHIE_PASSWORD
     DOLPHIE_HOST
     DOLPHIE_PORT
     DOLPHIE_SOCKET
 
 ```
 
+## Supported MySQL versions
+- MySQL/Percona Server 5.5/5.6/5.7/8.0
+- MariaDB 10+
+- RDS/Aurora
+
+## Grants required
+#### Least privilege
+1. PROCESS
+2. SELECT to `performance_schema` (if used) + `pt-heartbeat table` (if used)
+3. REPLICATION CLIENT
+
+#### Recommended
+1. PROCESS
+2. Global SELECT access (good for explaining queries, listing all databases, etc)
+4. REPLICATION CLIENT
+5. SUPER (only required if you want to kill queries)
+
+## Features
+- Dolphie uses panels to present groups of data. They can all be turned on/off to have a view of your database server that you prefer (see Help screenshot for panels available)
+- Prefers Performance Schema over Processlist if it's turned on for listing queries. Can be switched to use Processlist by pressing key "1" (or using parameter) since P_S can truncate query length for explaining queries
+- 3 options for finding replica lag in this order of precedence:
+  - `Performance Schema` (MySQL 8 only - most accurate, especially for multi-threaded replication)
+  - `pt-heartbeat table` (specified by parameter)
+  - `SHOW SLAVE STATUS`
+- Host cache file. This provides users a way to specify hostnames for IPs when their network's DNS can't resolve them. An example use case for this is when you connect to your work's VPN and DNS isn't available to resolve IPs. In my opinion, it's a lot easier to look at hostnames than IPs!
+- Supports encrypted login credentials via `mysql_config_editor`
+- Automatic conversion of large numbers & bytes to human-readable
+- Notifies when new version is available
+- Many commands at your fingertips (see Help screenshot)
+- Many valuable statisitics across the available panels that can help you troubleshoot issues and be proactive against them
+
+## Things to note
+Order of precedence for variables passed to Dolphie:
+1. Command-line
+2. Environment variables
+3. ~/.mylogin.cnf (`mysql_config_editor`)
+4. ~/.my.cnf
+
 ## Feedback
 I welcome all questions, bug reports, and requests. If you enjoy Dolphie, please let me know! I'd love to hear from you :smiley:
 
 ## Dashboard with processlist
 <img width="1706" alt="dashboard_processlist" src="https://user-images.githubusercontent.com/13244625/188236477-4ede6b72-d643-4037-b9a7-c2acfdf0c0b9.png">
 
 ## Dashboard with InnoDB statisitics + processlist
```

### Comparing `dolphie-2.0.7/dolphie/Database.py` & `dolphie-2.0.8/dolphie/Database.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,16 +33,19 @@
         self.cursor.execute(query, tuple(values))
         data = self.cursor.fetchone()
         if isinstance(data[field], (bytes, bytearray)):
             return data[field].decode()
         else:
             return data[field]
 
-    def execute(self, query, values=None):
+    def execute(self, query, values=None, ignore_error=False):
         try:
-            self.cursor.execute(query, values)
+            return self.cursor.execute(query, values)
         except Exception as e:
-            raise Exception("Failed to execute query %s - Reason: %s" % (query, e.args[1]))
+            if ignore_error:
+                pass
+            else:
+                raise Exception("Failed to execute query %s - Reason: %s" % (query, e.args[1]))
 
     def close(self):
         if self.connection:
             self.connection.close()
```

### Comparing `dolphie-2.0.7/dolphie/Functions.py` & `dolphie-2.0.8/dolphie/Functions.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.7/dolphie/KBHit.py` & `dolphie-2.0.8/dolphie/KBHit.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.7/dolphie/Panels/dashboard_panel.py` & `dolphie-2.0.8/dolphie/Panels/dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.7/dolphie/Panels/innodb_io_panel.py` & `dolphie-2.0.8/dolphie/Panels/innodb_io_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.7/dolphie/Panels/innodb_locks_panel.py` & `dolphie-2.0.8/dolphie/Panels/innodb_locks_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.7/dolphie/Panels/processlist_panel.py` & `dolphie-2.0.8/dolphie/Panels/processlist_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.7/dolphie/Panels/replica_panel.py` & `dolphie-2.0.8/dolphie/Panels/replica_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.7/dolphie/Queries.py` & `dolphie-2.0.8/dolphie/Queries.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.7/dolphie/__init__.py` & `dolphie-2.0.8/dolphie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         self.processlist_threads: dict = {}
         self.pause_refresh: bool = False
         self.first_loop: bool = True
         self.saved_status: bool = None
         self.previous_binlog_position: int = 0
         self.previous_replica_sbm: int = 0
         self.host_cache: dict = {}
+        self.host_cache_from_file: dict = {}
         self.variables: dict = {}
         self.statuses: dict = {}
         self.primary_status: dict = {}
         self.replica_status: dict = {}
         self.innodb_status: dict = {}
         self.replica_connections: dict = {}
 
@@ -1067,104 +1068,103 @@
 
         return valid_key
 
     def create_user_stats_table(self):
         table = Table(header_style="bold white", box=box.ROUNDED, style="grey70")
         columns = {}
 
-        if self.db.execute("SELECT @@userstat") == 1:
-            userstat_enabled = self.db.cursor.fetchone()["@@userstat"] == 1
+        userstat_enabled = 0
+        if self.db.execute("SELECT @@userstat", ignore_error=True) == 1:
+            userstat_enabled = self.db.cursor.fetchone()["@@userstat"]
+
+        if userstat_enabled:
+            self.db.execute(Queries["userstat_user_statisitics"])
+        elif self.performance_schema_enabled:
+            self.db.execute(Queries["ps_user_statisitics"])
+        else:
+            return False
 
-            if userstat_enabled:
-                self.db.execute(Queries["userstat_user_statisitics"])
-            elif self.performance_schema_enabled:
-                self.db.execute(Queries["ps_user_statisitics"])
-            else:
-                return False
+        users = self.db.cursor.fetchall()
+        user_stats = {}
 
-            users = self.db.cursor.fetchall()
-            user_stats = {}
+        for user in users:
+            username = user["user"].decode()
+            user_stats.setdefault(username, {}).update(
+                user=user["user"].decode(),
+                total_connections=user["total_connections"],
+                concurrent_connections=user.get("concurrent_connections"),
+                denied_connections=user.get("denied_connections"),
+                binlog_bytes_written=user.get("binlog_bytes_written"),
+                rows_fetched=user.get("rows_fetched"),
+                rows_updated=user.get("rows_updated"),
+                table_rows_read=user.get("table_rows_read"),
+                select_commands=user.get("select_commands"),
+                update_commands=user.get("update_commands"),
+                other_commands=user.get("other_commands"),
+                commit_transactions=user.get("commit_transactions"),
+                rollback_transactions=user.get("rollback_transactions"),
+                access_denied=user.get("access_denied"),
+                current_connections=user.get("current_connections"),
+                rows_affected=user.get("sum_rows_affected"),
+                rows_sent=user.get("sum_rows_sent"),
+                rows_read=user.get("sum_rows_examined"),
+                created_tmp_disk_tables=user.get("sum_created_tmp_disk_tables"),
+                created_tmp_tables=user.get("sum_created_tmp_tables"),
+            )
 
-            for user in users:
-                username = user["user"].decode()
-                user_stats.setdefault(username, {}).update(
-                    user=user["user"].decode(),
-                    total_connections=user["total_connections"],
-                    concurrent_connections=user.get("concurrent_connections"),
-                    denied_connections=user.get("denied_connections"),
-                    binlog_bytes_written=user.get("binlog_bytes_written"),
-                    rows_fetched=user.get("rows_fetched"),
-                    rows_updated=user.get("rows_updated"),
-                    table_rows_read=user.get("table_rows_read"),
-                    select_commands=user.get("select_commands"),
-                    update_commands=user.get("update_commands"),
-                    other_commands=user.get("other_commands"),
-                    commit_transactions=user.get("commit_transactions"),
-                    rollback_transactions=user.get("rollback_transactions"),
-                    access_denied=user.get("access_denied"),
-                    current_connections=user.get("current_connections"),
-                    rows_affected=user.get("sum_rows_affected"),
-                    rows_sent=user.get("sum_rows_sent"),
-                    rows_read=user.get("sum_rows_examined"),
-                    created_tmp_disk_tables=user.get("sum_created_tmp_disk_tables"),
-                    created_tmp_tables=user.get("sum_created_tmp_tables"),
-                )
+        if userstat_enabled:
+            columns.update(
+                {
+                    "User": {"field": "user", "format_number": False},
+                    "Active": {"field": "concurrent_connections", "format_number": True},
+                    "Total": {"field": "total_connections", "format_number": True},
+                    "Binlog Data": {"field": "binlog_bytes_written", "format_number": False},
+                    "Rows Read": {"field": "table_rows_read", "format_number": True},
+                    "Rows Sent": {"field": "rows_fetched", "format_number": True},
+                    "Rows Updated": {"field": "rows_updated", "format_number": True},
+                    "Selects": {"field": "select_commands", "format_number": True},
+                    "Updates": {"field": "update_commands", "format_number": True},
+                    "Other": {"field": "other_commands", "format_number": True},
+                    "Commit": {"field": "commit_transactions", "format_number": True},
+                    "Rollback": {"field": "rollback_transactions", "format_number": True},
+                    "Access Denied": {"field": "access_denied", "format_number": True},
+                    "Conn Denied": {"field": "denied_connections", "format_number": True},
+                }
+            )
+        else:
+            columns.update(
+                {
+                    "User": {"field": "user", "format_number": False},
+                    "Active": {"field": "current_connections", "format_number": True},
+                    "Total": {"field": "total_connections", "format_number": True},
+                    "Rows Read": {"field": "rows_read", "format_number": True},
+                    "Rows Sent": {"field": "rows_sent", "format_number": True},
+                    "Rows Updated": {"field": "rows_affected", "format_number": True},
+                    "Tmp Tables": {"field": "created_tmp_tables", "format_number": True},
+                    "Tmp Disk Tables": {"field": "created_tmp_disk_tables", "format_number": True},
+                }
+            )
 
-            if userstat_enabled:
-                columns.update(
-                    {
-                        "User": {"field": "user", "format_number": False},
-                        "Active": {"field": "concurrent_connections", "format_number": True},
-                        "Total": {"field": "total_connections", "format_number": True},
-                        "Binlog Data": {"field": "binlog_bytes_written", "format_number": False},
-                        "Rows Read": {"field": "table_rows_read", "format_number": True},
-                        "Rows Sent": {"field": "rows_fetched", "format_number": True},
-                        "Rows Updated": {"field": "rows_updated", "format_number": True},
-                        "Selects": {"field": "select_commands", "format_number": True},
-                        "Updates": {"field": "update_commands", "format_number": True},
-                        "Other": {"field": "other_commands", "format_number": True},
-                        "Commit": {"field": "commit_transactions", "format_number": True},
-                        "Rollback": {"field": "rollback_transactions", "format_number": True},
-                        "Access Denied": {"field": "access_denied", "format_number": True},
-                        "Conn Denied": {"field": "denied_connections", "format_number": True},
-                    }
-                )
-            else:
-                columns.update(
-                    {
-                        "User": {"field": "user", "format_number": False},
-                        "Active": {"field": "current_connections", "format_number": True},
-                        "Total": {"field": "total_connections", "format_number": True},
-                        "Rows Read": {"field": "rows_read", "format_number": True},
-                        "Rows Sent": {"field": "rows_sent", "format_number": True},
-                        "Rows Updated": {"field": "rows_affected", "format_number": True},
-                        "Tmp Tables": {"field": "created_tmp_tables", "format_number": True},
-                        "Tmp Disk Tables": {"field": "created_tmp_disk_tables", "format_number": True},
-                    }
-                )
+        for column, data in columns.items():
+            table.add_column(column, no_wrap=True)
 
+        for user_data in user_stats.values():
+            row_values = []
             for column, data in columns.items():
-                table.add_column(column, no_wrap=True)
-
-            for user_data in user_stats.values():
-                row_values = []
-                for column, data in columns.items():
-                    value = user_data.get(data["field"])
-                    if column == "Binlog Data":
-                        row_values.append(format_bytes(value) if value else "")
-                    elif data["format_number"]:
-                        row_values.append(format_number(value) if value else "")
-                    else:
-                        row_values.append(value or "")
+                value = user_data.get(data["field"])
+                if column == "Binlog Data":
+                    row_values.append(format_bytes(value) if value else "")
+                elif data["format_number"]:
+                    row_values.append(format_number(value) if value else "")
+                else:
+                    row_values.append(value or "")
 
-                table.add_row(*row_values, style="grey93")
+            table.add_row(*row_values, style="grey93")
 
-            return table if user_stats else False
-        else:
-            return False
+        return table if user_stats else False
 
     def load_host_cache_file(self):
         if os.path.exists(self.host_cache_file):
             with open(self.host_cache_file) as file:
                 for line in file:
                     line = line.strip()
                     error_message = f"Host cache entry '{line}' is not properly formatted! Format: ip=hostname"
@@ -1175,21 +1175,26 @@
                     ip_address, hostname = line.split("=", maxsplit=1)
                     ip_address = ip_address.strip()
                     hostname = hostname.strip()
 
                     if not ip_address or not hostname:
                         raise Exception(error_message)
 
-                    self.host_cache[ip_address] = hostname
+                    self.host_cache_from_file[ip_address] = hostname
 
     def get_hostname(self, ip_address):
         if ip_address in self.host_cache:
             return self.host_cache[ip_address]
 
+        if self.host_cache_from_file and ip_address in self.host_cache_from_file:
+            self.host_cache[ip_address] = self.host_cache_from_file[ip_address]
+            return self.host_cache_from_file[ip_address]
+
         try:
             ipaddress.IPv4Network(ip_address)
             hostname = socket.gethostbyaddr(ip_address)[0]
             self.host_cache[ip_address] = hostname
         except (ValueError, socket.error):
+            self.host_cache[ip_address] = ip_address
             hostname = ip_address
 
         return hostname
```

### Comparing `dolphie-2.0.7/dolphie/app.py` & `dolphie-2.0.8/dolphie/app.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.7/pyproject.toml` & `dolphie-2.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dolphie"
-version = "2.0.7"
+version = "2.0.8"
 description = "An intuitive feature-rich top tool for monitoring MySQL in real time"
 authors = ["Charles Thompson <01charles.t@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^13.4.2"
```

### Comparing `dolphie-2.0.7/PKG-INFO` & `dolphie-2.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolphie
-Version: 2.0.7
+Version: 2.0.8
 Summary: An intuitive feature-rich top tool for monitoring MySQL in real time
 Author: Charles Thompson
 Author-email: 01charles.t@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,15 +21,15 @@
 # Dolphie
 <p align="center">
 <img src="https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-4f9c-ada5-a153cdcf4070.png" width="120"><br>
 An intuitive feature-rich top tool for monitoring MySQL in real time
 </p>
 
 ## Installation
-Must be using Python 3.8+
+Requires Python 3.8+
 
 Using PyPi:
 ```shell
 pip install dolphie
 ```
 
 Using Poetry:
@@ -39,53 +39,14 @@
 poetry install
 ```
 
 ## Using Docker container
 1. `docker pull ghcr.io/charles-001/dolphie:latest`
 2. `docker run -dit --name dolphie ghcr.io/charles-001/dolphie:latest`
 3. `docker exec -it dolphie dolphie -h host.docker.internal -u root --ask-pass` (pass any additional parameters you'd like)
-5. Enjoy!
-
-## Supported MySQL versions
-- MySQL/Percona Server 5.5/5.6/5.7/8.0
-- MariaDB 10+
-- RDS/Aurora
-
-## Grants required
-#### Least privilege
-1. PROCESS
-2. SELECT to `performance_schema` (if used) + `pt-heartbeat table` (if used)
-3. REPLICATION CLIENT
-
-#### Recommended
-1. PROCESS
-2. Global SELECT access (good for explaining queries, listing all databases, etc)
-4. REPLICATION CLIENT
-5. SUPER (only required if you want to kill queries)
-
-## Features
-- Dolphie uses panels to present groups of data. They can all be turned on/off to have a view of your database server that you prefer (see Help screenshot for panels available)
-- Prefers Performance Schema over Processlist if it's turned on for listing queries. Can be switched to use Processlist by pressing key "1" (or using parameter) since P_S can truncate query length for explaining queries
-- 3 options for finding replica lag in this order of precedence: 
-  - `Performance Schema` (MySQL 8 only - most accurate, especially for multi-threaded replication)
-  - `pt-heartbeat table` (specified by parameter)
-  - `SHOW SLAVE STATUS`
-- Host cache file. This provides users a way to specify hostnames for IPs when their network's DNS can't resolve them. An example use case for this is when you connect to your work's VPN and DNS isn't available to resolve IPs. In my opinion, it's a lot easier to look at hostnames than IPs!
-- Supports encrypted login credentials via `mysql_config_editor`
-- Automatic conversion of large numbers & bytes to human-readable
-- Notifies when new version is available
-- Many commands at your fingertips (see Help screenshot)
-- Many valuable statisitics across the available panels that can help you troubleshoot issues and be proactive against them
-
-## Things to note
-Order of precedence for variables passed to Dolphie:
-1. Parameters via command-line
-2. Environment variables
-3. ~/.mylogin.cnf (`mysql_config_editor`)
-4. ~/.my.cnf
 
 ## Usage
 ```
 options:
   --help                show this help message and exit
   -u USER, --user USER  Username for MySQL
   -p PASSWORD, --password PASSWORD
@@ -141,14 +102,52 @@
     DOLPHIE_PASSWORD
     DOLPHIE_HOST
     DOLPHIE_PORT
     DOLPHIE_SOCKET
 
 ```
 
+## Supported MySQL versions
+- MySQL/Percona Server 5.5/5.6/5.7/8.0
+- MariaDB 10+
+- RDS/Aurora
+
+## Grants required
+#### Least privilege
+1. PROCESS
+2. SELECT to `performance_schema` (if used) + `pt-heartbeat table` (if used)
+3. REPLICATION CLIENT
+
+#### Recommended
+1. PROCESS
+2. Global SELECT access (good for explaining queries, listing all databases, etc)
+4. REPLICATION CLIENT
+5. SUPER (only required if you want to kill queries)
+
+## Features
+- Dolphie uses panels to present groups of data. They can all be turned on/off to have a view of your database server that you prefer (see Help screenshot for panels available)
+- Prefers Performance Schema over Processlist if it's turned on for listing queries. Can be switched to use Processlist by pressing key "1" (or using parameter) since P_S can truncate query length for explaining queries
+- 3 options for finding replica lag in this order of precedence:
+  - `Performance Schema` (MySQL 8 only - most accurate, especially for multi-threaded replication)
+  - `pt-heartbeat table` (specified by parameter)
+  - `SHOW SLAVE STATUS`
+- Host cache file. This provides users a way to specify hostnames for IPs when their network's DNS can't resolve them. An example use case for this is when you connect to your work's VPN and DNS isn't available to resolve IPs. In my opinion, it's a lot easier to look at hostnames than IPs!
+- Supports encrypted login credentials via `mysql_config_editor`
+- Automatic conversion of large numbers & bytes to human-readable
+- Notifies when new version is available
+- Many commands at your fingertips (see Help screenshot)
+- Many valuable statisitics across the available panels that can help you troubleshoot issues and be proactive against them
+
+## Things to note
+Order of precedence for variables passed to Dolphie:
+1. Command-line
+2. Environment variables
+3. ~/.mylogin.cnf (`mysql_config_editor`)
+4. ~/.my.cnf
+
 ## Feedback
 I welcome all questions, bug reports, and requests. If you enjoy Dolphie, please let me know! I'd love to hear from you :smiley:
 
 ## Dashboard with processlist
 <img width="1706" alt="dashboard_processlist" src="https://user-images.githubusercontent.com/13244625/188236477-4ede6b72-d643-4037-b9a7-c2acfdf0c0b9.png">
 
 ## Dashboard with InnoDB statisitics + processlist
```

