# Comparing `tmp/epyxid-0.1.4.tar.gz` & `tmp/epyxid-0.2.0.tar.gz`

## Comparing `epyxid-0.1.4.tar` & `epyxid-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 epyxid-0.1.4/Cargo.toml
--rw-r--r--   0     1001      127      270 2024-05-10 13:39:34.000000 epyxid-0.1.4/.editorconfig
--rw-r--r--   0     1001      127     4131 2024-05-10 13:39:34.000000 epyxid-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0     1001      127     1511 2024-05-10 13:39:34.000000 epyxid-0.1.4/.gitignore
--rw-r--r--   0     1001      127      516 2024-05-10 13:39:34.000000 epyxid-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1036 2024-05-10 13:39:34.000000 epyxid-0.1.4/LICENSE.txt
--rw-r--r--   0     1001      127      490 2024-05-10 13:39:34.000000 epyxid-0.1.4/README.md
--rw-r--r--   0     1001      127     1390 2024-05-10 13:39:34.000000 epyxid-0.1.4/epyxid.pyi
--rwxr-xr-x   0     1001      127      135 2024-05-10 13:39:34.000000 epyxid-0.1.4/justfile
--rw-r--r--   0     1001      127      118 2024-05-10 13:39:34.000000 epyxid-0.1.4/src/errors.rs
--rw-r--r--   0     1001      127      595 2024-05-10 13:39:34.000000 epyxid-0.1.4/src/lib.rs
--rw-r--r--   0     1001      127      926 2024-05-10 13:39:34.000000 epyxid-0.1.4/src/utils.rs
--rw-r--r--   0     1001      127     1746 2024-05-10 13:39:34.000000 epyxid-0.1.4/src/wrapper.rs
--rw-r--r--   0     1001      127      913 2024-05-10 13:39:34.000000 epyxid-0.1.4/test_xid.py
--rw-r--r--   0     1001      127    13608 2024-05-10 13:39:40.000000 epyxid-0.1.4/Cargo.lock
--rw-r--r--   0     1001      127     1168 2024-05-10 13:39:34.000000 epyxid-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1371 1970-01-01 00:00:00.000000 epyxid-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 epyxid-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      127      270 2024-05-10 20:25:37.000000 epyxid-0.2.0/.editorconfig
+-rw-r--r--   0     1001      127     3526 2024-05-10 20:25:37.000000 epyxid-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     1511 2024-05-10 20:25:37.000000 epyxid-0.2.0/.gitignore
+-rw-r--r--   0     1001      127      516 2024-05-10 20:25:37.000000 epyxid-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1036 2024-05-10 20:25:37.000000 epyxid-0.2.0/LICENSE.txt
+-rw-r--r--   0     1001      127      490 2024-05-10 20:25:37.000000 epyxid-0.2.0/README.md
+-rw-r--r--   0     1001      127     1444 2024-05-10 20:25:37.000000 epyxid-0.2.0/epyxid.pyi
+-rwxr-xr-x   0     1001      127      274 2024-05-10 20:25:37.000000 epyxid-0.2.0/justfile
+-rw-r--r--   0     1001      127      118 2024-05-10 20:25:37.000000 epyxid-0.2.0/src/errors.rs
+-rw-r--r--   0     1001      127      675 2024-05-10 20:25:37.000000 epyxid-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      127      944 2024-05-10 20:25:37.000000 epyxid-0.2.0/src/utils.rs
+-rw-r--r--   0     1001      127     1928 2024-05-10 20:25:37.000000 epyxid-0.2.0/src/wrapper.rs
+-rw-r--r--   0     1001      127     1014 2024-05-10 20:25:37.000000 epyxid-0.2.0/test_xid.py
+-rw-r--r--   0     1001      127    13608 2024-05-10 20:25:43.000000 epyxid-0.2.0/Cargo.lock
+-rw-r--r--   0     1001      127     1168 2024-05-10 20:25:37.000000 epyxid-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1371 1970-01-01 00:00:00.000000 epyxid-0.2.0/PKG-INFO
```

### Comparing `epyxid-0.1.4/.gitignore` & `epyxid-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `epyxid-0.1.4/.pre-commit-config.yaml` & `epyxid-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `epyxid-0.1.4/LICENSE.txt` & `epyxid-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `epyxid-0.1.4/epyxid.pyi` & `epyxid-0.2.0/epyxid.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from datetime import datetime
 
+__version__: str
+
 
 class XID:
     """
     Globally unique sortable id.
     """
 
     def as_bytes(self) -> bytes:
@@ -36,14 +38,16 @@
 
     @property
     def counter(self) -> int:
         """
         Extract the incrementing counter.
         """
 
+    def __hash__(self) -> int: ...
+
     def __bytes__(self) -> bytes: ...
 
     def __str__(self) -> str: ...
 
     def __repr__(self) -> str: ...
 
     def __eq__(self, object: 'XID') -> bool: ...
```

### Comparing `epyxid-0.1.4/src/lib.rs` & `epyxid-0.2.0/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-use std::str::FromStr;
-
-use pyo3::prelude::{pymodule, PyModule, PyResult, Python};
-use pyo3::wrap_pyfunction;
+use pyo3::prelude::{pymodule, wrap_pyfunction, Bound, PyModule, PyResult, Python};
 
 use crate::errors::XIDError;
 use crate::utils::{xid_create, xid_from_bytes, xid_from_str};
 use crate::wrapper::XID;
 
+const PY_MODULE_VERSION: &str = "0.2.0";
+
 mod errors;
 mod utils;
 mod wrapper;
 
 #[pymodule]
-fn epyxid(_py: Python, m: &PyModule) -> PyResult<()> {
+fn epyxid(py: Python<'_>, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<XID>()?;
     m.add_function(wrap_pyfunction!(xid_create, m)?)?;
     m.add_function(wrap_pyfunction!(xid_from_str, m)?)?;
     m.add_function(wrap_pyfunction!(xid_from_bytes, m)?)?;
-    m.add("XIDError", _py.get_type::<XIDError>())?;
+    m.add("XIDError", py.get_type_bound::<XIDError>())?;
+    m.add("__version__", PY_MODULE_VERSION)?;
     Ok(())
 }
```

### Comparing `epyxid-0.1.4/src/utils.rs` & `epyxid-0.2.0/src/utils.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 use std::str::FromStr;
 
+use pyo3::prelude::PyBytesMethods;
 use pyo3::types::PyBytes;
-use pyo3::{pyfunction, PyResult};
+use pyo3::{pyfunction, Bound, PyResult};
 use xid::{Id, ParseIdError};
 
 use crate::errors::XIDError;
 use crate::wrapper::XID;
 
 #[pyfunction]
 pub fn xid_create() -> PyResult<XID> {
-    Ok(XID { inner: xid::new() })
+    Ok(XID(xid::new()))
 }
 
 #[pyfunction]
 pub fn xid_from_str(s: &str) -> PyResult<XID> {
     match Id::from_str(s) {
-        Ok(id) => Ok(XID { inner: id }),
+        Ok(id) => Ok(XID(id)),
         Err(error) => Err(XIDError::new_err(error.to_string())),
     }
 }
 
 #[pyfunction]
-pub fn xid_from_bytes(b: &PyBytes) -> PyResult<XID> {
+pub fn xid_from_bytes(b: Bound<PyBytes>) -> PyResult<XID> {
     match id_from_bytes(b.as_bytes()) {
-        Ok(value) => Ok(XID { inner: value }),
+        Ok(value) => Ok(XID(value)),
         Err(error) => Err(XIDError::new_err(error.to_string())),
     }
 }
 
 fn id_from_bytes(s: &[u8]) -> Result<Id, ParseIdError> {
     if s.len() != 12 {
         return Err(ParseIdError::InvalidLength(s.len()));
```

### Comparing `epyxid-0.1.4/src/wrapper.rs` & `epyxid-0.2.0/src/wrapper.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-use std::str::FromStr;
+use std::hash::{DefaultHasher, Hash, Hasher};
 
 use pyo3::types::{PyBytes, PyDateTime};
-use pyo3::{pyclass, pymethods, PyResult, Python};
+use pyo3::{pyclass, pymethods, Bound, PyResult, Python};
 use xid::Id;
 
 #[pyclass]
-pub struct XID {
-    pub inner: Id,
-}
+pub struct XID(pub Id);
 
 #[pymethods]
 impl XID {
-    fn as_bytes<'p>(&self, _py: Python<'p>) -> &'p PyBytes {
-        PyBytes::new(_py, self.inner.as_bytes())
+    fn as_bytes<'p>(&self, _py: Python<'p>) -> Bound<'p, PyBytes> {
+        PyBytes::new_bound(_py, self.0.as_bytes())
     }
 
     fn to_str(&self) -> String {
-        self.inner.to_string()
+        self.0.to_string()
     }
 
     #[getter]
-    fn machine<'p>(&self, _py: Python<'p>) -> &'p PyBytes {
-        PyBytes::new(_py, &self.inner.machine())
+    fn machine<'p>(&self, _py: Python<'p>) -> Bound<'p, PyBytes> {
+        PyBytes::new_bound(_py, &self.0.machine())
     }
 
     #[getter]
     fn pid(&self) -> u16 {
-        self.inner.pid()
+        self.0.pid()
     }
 
     #[getter]
-    fn time<'p>(&self, _py: Python<'p>) -> PyResult<&'p PyDateTime> {
-        let raw = self.inner.as_bytes();
+    fn time<'p>(&self, _py: Python<'p>) -> PyResult<Bound<'p, PyDateTime>> {
+        let raw = self.0.as_bytes();
         let unix_ts = u32::from_be_bytes([raw[0], raw[1], raw[2], raw[3]]);
-        PyDateTime::from_timestamp(_py, unix_ts as f64, None)
+        PyDateTime::from_timestamp_bound(_py, unix_ts as f64, None)
     }
 
     #[getter]
     fn counter(&self) -> u32 {
-        self.inner.counter()
+        self.0.counter()
     }
 
-    fn __bytes__<'p>(&self, _py: Python<'p>) -> &'p PyBytes {
+    fn __bytes__<'p>(&self, _py: Python<'p>) -> Bound<'p, PyBytes> {
         self.as_bytes(_py)
     }
 
     fn __str__(&self) -> String {
         self.to_str()
     }
 
@@ -72,8 +70,14 @@
     fn __gt__(&self, object: &XID) -> bool {
         self.to_str() > object.to_str()
     }
 
     fn __ge__(&self, object: &XID) -> bool {
         self.to_str() >= object.to_str()
     }
+
+    fn __hash__(&self) -> u64 {
+        let mut hasher = DefaultHasher::new();
+        self.0.hash(&mut hasher);
+        hasher.finish()
+    }
 }
```

### Comparing `epyxid-0.1.4/test_xid.py` & `epyxid-0.2.0/test_xid.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,10 +26,15 @@
 
 
 def test_from_bytes_valid() -> None:
     xid = xid_from_bytes(XID_BYTES)
     assert str(xid) == XID_STR
 
 
+def test_hash() -> None:
+    xid = xid_from_bytes(XID_BYTES)
+    assert isinstance(hash(xid), int)
+
+
 def test_from_bytes_invalid_length() -> None:
     with raises(ValueError):
         xid_from_bytes(bytes([0x4d, 0x88, 0xe1, 0x5b, 0x60, 0xf4, 0x86, 0xe4, 0x28, 0x41, 0x2d]))
```

### Comparing `epyxid-0.1.4/Cargo.lock` & `epyxid-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "epyxid"
-version = "0.0.0"
+version = "0.2.0"
 dependencies = [
  "pyo3",
  "xid",
 ]
 
 [[package]]
 name = "getrandom"
```

### Comparing `epyxid-0.1.4/pyproject.toml` & `epyxid-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "epyxid"
 description = "Python wrapper around Rust implementation of XID (Globally Unique ID Generator)"
 requires-python = ">=3.8"
 authors = [
   {name = "Aleksandr Shpak", email = "shpaker@gmail.com"},
 ]
-version = "0.1.4"
+version = "0.2.0"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 keywords = [
   "rust",
   "xid",
   "pyo3",
 ]
```

### Comparing `epyxid-0.1.4/PKG-INFO` & `epyxid-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: epyxid
-Version: 0.1.4
+Version: 0.2.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
```

