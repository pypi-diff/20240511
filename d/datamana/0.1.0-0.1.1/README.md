# Comparing `tmp/datamana-0.1.0.tar.gz` & `tmp/datamana-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamana-0.1.0.tar", last modified: Thu May  9 11:55:20 2024, max compression
+gzip compressed data, was "datamana-0.1.1.tar", last modified: Fri May 10 14:31:22 2024, max compression
```

## Comparing `datamana-0.1.0.tar` & `datamana-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:55:20.624034 datamana-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-09 11:55:14.000000 datamana-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-09 11:55:14.000000 datamana-0.1.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-09 11:55:14.000000 datamana-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 11:55:14.000000 datamana-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-09 11:55:20.624034 datamana-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:55:14.000000 datamana-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:55:20.620034 datamana-0.1.0/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-09 11:55:14.000000 datamana-0.1.0/csrc/mqueue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-09 11:55:14.000000 datamana-0.1.0/csrc/python.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-09 11:55:14.000000 datamana-0.1.0/csrc/semaphore.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-09 11:55:14.000000 datamana-0.1.0/csrc/shared_memory.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:55:20.624034 datamana-0.1.0/datamana/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:55:14.000000 datamana-0.1.0/datamana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-09 11:55:14.000000 datamana-0.1.0/datamana/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-09 11:55:14.000000 datamana-0.1.0/datamana/ipc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-09 11:55:14.000000 datamana-0.1.0/datamana/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-09 11:55:14.000000 datamana-0.1.0/datamana/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:55:20.624034 datamana-0.1.0/datamana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-09 11:55:20.000000 datamana-0.1.0/datamana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 11:55:20.000000 datamana-0.1.0/datamana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:55:20.000000 datamana-0.1.0/datamana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 11:55:20.000000 datamana-0.1.0/datamana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 11:55:20.000000 datamana-0.1.0/datamana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-09 11:55:14.000000 datamana-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:55:20.624034 datamana-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-09 11:55:14.000000 datamana-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:31:22.260938 datamana-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-10 14:31:14.000000 datamana-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-10 14:31:14.000000 datamana-0.1.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 14:31:14.000000 datamana-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-10 14:31:14.000000 datamana-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-10 14:31:22.260938 datamana-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:31:14.000000 datamana-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:31:22.256937 datamana-0.1.1/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-10 14:31:14.000000 datamana-0.1.1/csrc/mqueue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-10 14:31:14.000000 datamana-0.1.1/csrc/python.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-10 14:31:14.000000 datamana-0.1.1/csrc/semaphore.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-10 14:31:14.000000 datamana-0.1.1/csrc/shared_memory.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:31:22.260938 datamana-0.1.1/datamana/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:31:14.000000 datamana-0.1.1/datamana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 14:31:14.000000 datamana-0.1.1/datamana/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-10 14:31:14.000000 datamana-0.1.1/datamana/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-10 14:31:14.000000 datamana-0.1.1/datamana/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-10 14:31:14.000000 datamana-0.1.1/datamana/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:31:22.260938 datamana-0.1.1/datamana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-10 14:31:22.000000 datamana-0.1.1/datamana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-10 14:31:22.000000 datamana-0.1.1/datamana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:31:22.000000 datamana-0.1.1/datamana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 14:31:22.000000 datamana-0.1.1/datamana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 14:31:22.000000 datamana-0.1.1/datamana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-10 14:31:14.000000 datamana-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:31:22.260938 datamana-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-10 14:31:14.000000 datamana-0.1.1/setup.py
```

### Comparing `datamana-0.1.0/.gitignore` & `datamana-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `datamana-0.1.0/CMakeLists.txt` & `datamana-0.1.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `datamana-0.1.0/LICENSE` & `datamana-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datamana-0.1.0/PKG-INFO` & `datamana-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.1.0/csrc/mqueue.hpp` & `datamana-0.1.1/csrc/mqueue.hpp`

 * *Files identical despite different names*

### Comparing `datamana-0.1.0/csrc/semaphore.hpp` & `datamana-0.1.1/csrc/semaphore.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -27,18 +27,22 @@
     }
     int py_sem_post() {
         return sem_post(sem);
     }
     int py_sem_wait() {
         return sem_wait(sem);
     }
+    int py_sem_trywait() {
+        return sem_trywait(sem);
+    }
 };
 
 void DEFINE_SEMAPHORE_MODULE(nb::module_ & (m)) {
     nb::class_<Semaphore>(m, "Semaphore")
         .def(nb::init<>())
         .def("open", &Semaphore::py_sem_open)
         .def("close", &Semaphore::py_sem_close)
         .def("unlink", &Semaphore::py_sem_unlink)
         .def("wait", &Semaphore::py_sem_wait)
+        .def("trywait", &Semaphore::py_sem_trywait)
         .def("post", &Semaphore::py_sem_post);
 }
```

### Comparing `datamana-0.1.0/csrc/shared_memory.hpp` & `datamana-0.1.1/csrc/shared_memory.hpp`

 * *Files identical despite different names*

### Comparing `datamana-0.1.0/datamana/base.py` & `datamana-0.1.1/datamana/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 
 class Base():
     def __init__(self, name):
         self.data_name = f'datamana{name}'
         self.data_meta_name = f'{self.data_name}meta'
         self.data_share_name = f'{self.data_name}share'
         self.data_sem_name = f'{self.data_name}sem'
-        self.data_mq_tx_name =f'{self.data_name}mqtx'
-        self.data_mq_rx_name =f'{self.data_name}mqrx'
+        self.data_event_name =f'{self.data_name}event'
         self.sem = Semaphore(self.data_sem_name)
-        self.mq_tx = MQueue(self.data_mq_tx_name)
-        self.mq_rx = MQueue(self.data_mq_rx_name)
+        self.event = Semaphore(self.data_event_name)
         self.name2shm = {}
 
     def get_shm(self, shm_name, size, **kwargs):
         if shm_name in self.name2shm:
             shm = self.name2shm[shm_name]
             if size > 0: shm.resize(size)
         else:
@@ -26,19 +24,7 @@
     def write_byte(self, shm, data, size):
         shm.resize(size)
         shm.buf[:size] = data[:]
 
     def write_numpy(self, shm, data):
         np_shm = np.ndarray(data.shape, dtype=data.dtype, buffer=shm.buf)
         np_shm[:] = data[:]
-
-    def server_send(self, msg, msg_prio=0):
-        return self.mq_tx.send(msg, msg_prio)
-
-    def server_recv(self):
-        return self.mq_rx.receive()
-
-    def client_send(self, msg, msg_prio=0):
-        return self.mq_rx.send(msg, msg_prio)
-
-    def client_recv(self):
-        return self.mq_tx.receive()
```

### Comparing `datamana-0.1.0/datamana/ipc.py` & `datamana-0.1.1/datamana/ipc.py`

 * *Files identical despite different names*

### Comparing `datamana-0.1.0/datamana/numpy.py` & `datamana-0.1.1/datamana/numpy.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,72 +5,78 @@
 
 class Server(Base):
     def __init__(self, name, dataloader: Iterable):
         super().__init__(name)
         self.dataloader = dataloader
         self.iterloader = iter(self.dataloader)
         self.oflags = os.O_CREAT | os.O_RDWR
+        self.data_id = 0
+        self.max_data_id = 2**31 - 1
 
     def next(self):
         try:
             data = next(self.iterloader)
         except StopIteration:
             self.iterloader = iter(self.dataloader)
             data = next(self.iterloader)
-        shm = self.get_shm(self.data_share_name, data.nbytes, oflags=self.oflags)
+        shm = self.get_shm(self.data_share_name, data.nbytes, oflag=self.oflags)
         self.write_numpy(shm, data)
 
         meta_data = {
             'shape': data.shape,
             'dtype': data.dtype.name,
-            'pids': set(),
+            'id': self.data_id,
         }
         meta_data_pkl = pickle.dumps(meta_data)
         pkl_size = len(meta_data_pkl)
-        shm = self.get_shm(self.data_meta_name, pkl_size, oflags=self.oflags)
+        shm = self.get_shm(self.data_meta_name, pkl_size, oflag=self.oflags)
         self.write_byte(shm, meta_data_pkl, pkl_size)
+        self.data_id += 1
+        if self.data_id >= self.max_data_id:
+            self.data_id = 0
 
     def serve(self):
         self.next()
 
         while True:
-            ret, msg, msg_prio = self.server_recv()
+            # wait client signal
+            ret = self.event.wait()
+            loop = ret
+            # clean all signal
+            while loop == 0:
+                loop = self.event.trywait()
+
             if ret == 0:
                 self.sem.wait()
                 self.next()
-                self.server_send("")
                 self.sem.post()
             else:
                 print(os.strerror(ret))
                 time.sleep(1)
 
 class Client(Base):
     def __init__(self, name):
         super().__init__(name)
         self.pid = os.getpid()
         self.oflags = os.O_RDWR
+        self.data_id = -1
 
     def next(self):
         while True:
             self.sem.wait()
 
             shm_meta = self.get_shm(self.data_meta_name, 0, oflag=self.oflags)
             meta_data = pickle.loads(shm_meta.buf)
 
-            if self.pid not in meta_data['pids']:
+            if self.data_id != meta_data['id']:
+                self.data_id = meta_data['id']
                 shape = meta_data['shape']
                 dtype = np.dtype(meta_data['dtype'])
 
                 shm_data = self.get_shm(self.data_share_name, 0, oflag=self.oflags)
                 data = np.ndarray(shape, dtype=dtype, buffer=shm_data.buf).copy()
 
-                meta_data['pids'].add(self.pid)
-                meta_data_pkl = pickle.dumps(meta_data)
-                pkl_size = len(meta_data_pkl)
-                shm_meta = self.get_shm(self.data_meta_name, pkl_size, oflags=self.oflags)
-                self.write_byte(shm_meta, meta_data_pkl, pkl_size)
                 self.sem.post()
                 return data
             else:
-                self.client_send("")
                 self.sem.post()
-                self.client_recv()
+                self.event.post()
```

### Comparing `datamana-0.1.0/datamana/torch.py` & `datamana-0.1.1/datamana/torch.py`

 * *Files identical despite different names*

### Comparing `datamana-0.1.0/datamana.egg-info/PKG-INFO` & `datamana-0.1.1/datamana.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.1.0/pyproject.toml` & `datamana-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "cmake >= 3.15",
     "nanobind >= 1.9.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamana"
-version = "0.1.0"
+version = "0.1.1"
 description = "Dataset Manager"
 readme = "README.md"
 authors = [
     {name = "Jiau Zhang", email = "jiauzhang@163.com"},
 ]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `datamana-0.1.0/setup.py` & `datamana-0.1.1/setup.py`

 * *Files identical despite different names*

