# Comparing `tmp/databend_driver-0.9.4-cp37-abi3-win_amd64.whl.zip` & `tmp/databend_driver-0.9.5-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4335926 bytes, number of entries: 6
--rw-r--r--  4.6 unx     1509 b- defN 23-Oct-31 07:31 databend_driver-0.9.4.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Oct-31 07:31 databend_driver-0.9.4.dist-info/WHEEL
--rw-r--r--  4.6 unx      641 b- defN 23-Oct-31 07:31 databend_driver/__init__.py
--rw-r--r--  4.6 unx     2036 b- defN 23-Oct-31 07:31 databend_driver/__init__.pyi
--rwxr-xr-x  4.6 unx 12875264 b- defN 23-Oct-31 07:31 databend_driver/_databend_driver.pyd
--rw-r--r--  4.6 unx      495 b- defN 23-Oct-31 07:31 databend_driver-0.9.4.dist-info/RECORD
-6 files, 12880039 bytes uncompressed, 4335036 bytes compressed:  66.3%
+Zip file size: 4336313 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     1631 b- defN 23-Nov-02 07:53 databend_driver-0.9.5.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Nov-02 07:53 databend_driver-0.9.5.dist-info/WHEEL
+-rw-r--r--  4.6 unx      641 b- defN 23-Nov-02 07:53 databend_driver/__init__.py
+-rw-r--r--  4.6 unx     2036 b- defN 23-Nov-02 07:53 databend_driver/__init__.pyi
+-rwxr-xr-x  4.6 unx 12883456 b- defN 23-Nov-02 07:53 databend_driver/_databend_driver.pyd
+-rw-r--r--  4.6 unx      495 b- defN 23-Nov-02 07:53 databend_driver-0.9.5.dist-info/RECORD
+6 files, 12888353 bytes uncompressed, 4335423 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: databend_driver-0.9.4.dist-info/METADATA
+Filename: databend_driver-0.9.5.dist-info/METADATA
 Comment: 
 
-Filename: databend_driver-0.9.4.dist-info/WHEEL
+Filename: databend_driver-0.9.5.dist-info/WHEEL
 Comment: 
 
 Filename: databend_driver/__init__.py
 Comment: 
 
 Filename: databend_driver/__init__.pyi
 Comment: 
 
 Filename: databend_driver/_databend_driver.pyd
 Comment: 
 
-Filename: databend_driver-0.9.4.dist-info/RECORD
+Filename: databend_driver-0.9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `databend_driver-0.9.4.dist-info/METADATA` & `databend_driver-0.9.5.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-driver
-Version: 0.9.4
+Version: 0.9.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pdoc ; extra == 'docs'
 Requires-Dist: behave ; extra == 'test'
 Requires-Dist: black ; extra == 'lint'
 Requires-Dist: flake8 ; extra == 'lint'
@@ -15,60 +15,53 @@
 Author: Databend Authors <opensource@datafuselabs.com>
 Author-email: Databend Authors <opensource@datafuselabs.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/datafuselabs/bendsql
 
-## databend-driver
+# databend-driver
 
-### Build
+## Build
 
 ```shell
 cd bindings/python
 maturin develop
 ```
 
 ## Usage
 
 ```python
-import databend_driver
 import asyncio
+from databend_driver import AsyncDatabendClient
+
 async def main():
-	s = databend_driver.AsyncDatabendDriver('databend+http://root:root@localhost:8000/?sslmode=disable')
-	await s.exec("CREATE TABLE if not exists test_upload (x Int32,y VARCHAR)")
+    client = AsyncDatabendClient('databend+http://root:root@localhost:8000/?sslmode=disable')
+    conn = await client.get_conn()
+    await conn.exec(
+        """
+        CREATE TABLE test (
+            i64 Int64,
+            u64 UInt64,
+            f64 Float64,
+            s   String,
+            s2  String,
+            d   Date,
+            t   DateTime
+        )
+        """
+    )
+    rows = await conn.query_iter("SELECT * FROM test")
+    async for row in rows:
+        print(row.values())
 
 asyncio.run(main())
 ```
 
 ## Development
 
-Setup virtualenv:
-
-```shell
-python -m venv venv
-```
-
-Activate venv:
-
-```shell
-source venv/bin/activate
-````
-
-Install `maturin`:
-
-```shell
-pip install maturin[patchelf]
-```
-
-Build bindings:
-
 ```shell
+pipenv install --dev
 maturin develop
+pipenv run behave tests
 ```
-
-Run some tests:
-
-```shell
-maturin develop -E test
-behave tests
-```
+
```

