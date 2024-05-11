# Comparing `tmp/sqlglotrs-0.2.0.tar.gz` & `tmp/sqlglotrs-0.2.5.tar.gz`

## Comparing `sqlglotrs-0.2.0.tar` & `sqlglotrs-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      146 1970-01-01 00:00:00.000000 sqlglotrs-0.2.0/Cargo.toml
--rw-r--r--   0     1001      127     2528 2024-04-02 18:59:05.000000 sqlglotrs-0.2.0/src/lib.rs
--rw-r--r--   0     1001      127     5129 2024-04-02 18:59:05.000000 sqlglotrs-0.2.0/src/settings.rs
--rw-r--r--   0     1001      127    24089 2024-04-02 18:59:05.000000 sqlglotrs-0.2.0/src/tokenizer.rs
--rw-r--r--   0     1001      127     1468 2024-04-02 18:59:05.000000 sqlglotrs-0.2.0/src/trie.rs
--rw-r--r--   0     1001      127     7619 2024-04-02 18:59:13.000000 sqlglotrs-0.2.0/Cargo.lock
--rw-r--r--   0     1001      127      390 2024-04-02 18:59:05.000000 sqlglotrs-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      258 1970-01-01 00:00:00.000000 sqlglotrs-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      146 1970-01-01 00:00:00.000000 sqlglotrs-0.2.5/Cargo.toml
+-rw-r--r--   0     1001      127     2528 2024-05-11 00:45:46.000000 sqlglotrs-0.2.5/src/lib.rs
+-rw-r--r--   0     1001      127     5129 2024-05-11 00:45:46.000000 sqlglotrs-0.2.5/src/settings.rs
+-rw-r--r--   0     1001      127    24273 2024-05-11 00:45:46.000000 sqlglotrs-0.2.5/src/tokenizer.rs
+-rw-r--r--   0     1001      127     1468 2024-05-11 00:45:46.000000 sqlglotrs-0.2.5/src/trie.rs
+-rw-r--r--   0     1001      127     7619 2024-05-11 00:45:46.000000 sqlglotrs-0.2.5/Cargo.lock
+-rw-r--r--   0     1001      127      390 2024-05-11 00:45:46.000000 sqlglotrs-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      258 1970-01-01 00:00:00.000000 sqlglotrs-0.2.5/PKG-INFO
```

### Comparing `sqlglotrs-0.2.0/src/lib.rs` & `sqlglotrs-0.2.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `sqlglotrs-0.2.0/src/settings.rs` & `sqlglotrs-0.2.5/src/settings.rs`

 * *Files identical despite different names*

### Comparing `sqlglotrs-0.2.0/src/tokenizer.rs` & `sqlglotrs-0.2.5/src/tokenizer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -479,14 +479,17 @@
         let mut decimal = false;
         let mut scientific = 0;
 
         loop {
             if self.peek_char.is_digit(10) {
                 self.advance(1)?;
             } else if self.peek_char == '.' && !decimal {
+                if self.tokens.last().map(|t| t.token_type) == Some(self.token_types.parameter) {
+                    return self.add(self.token_types.number, None);
+                }
                 decimal = true;
                 self.advance(1)?;
             } else if (self.peek_char == '-' || self.peek_char == '+') && scientific == 1 {
                 scientific += 1;
                 self.advance(1)?;
             } else if self.peek_char.to_ascii_uppercase() == 'E' && scientific == 0 {
                 scientific += 1;
```

### Comparing `sqlglotrs-0.2.0/src/trie.rs` & `sqlglotrs-0.2.5/src/trie.rs`

 * *Files identical despite different names*

### Comparing `sqlglotrs-0.2.0/Cargo.lock` & `sqlglotrs-0.2.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 name = "smallvec"
 version = "1.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
 
 [[package]]
 name = "sqlglotrs"
-version = "0.2.0"
+version = "0.2.5"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "syn"
 version = "2.0.41"
```

