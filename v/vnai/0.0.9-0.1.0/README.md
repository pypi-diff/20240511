# Comparing `tmp/vnai-0.0.9.tar.gz` & `tmp/vnai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnai-0.0.9.tar", last modified: Tue May  7 13:05:00 2024, max compression
+gzip compressed data, was "vnai-0.1.0.tar", last modified: Sat May 11 13:54:06 2024, max compression
```

## Comparing `vnai-0.0.9.tar` & `vnai-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-07 13:05:00.385245 vnai-0.0.9/
--rw-r--r--   0 mrthinh    (501) staff       (20)      573 2024-05-07 13:05:00.385183 vnai-0.0.9/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)      140 2024-05-06 15:49:50.000000 vnai-0.0.9/pyproject.toml
--rw-r--r--   0 mrthinh    (501) staff       (20)      568 2024-05-07 13:05:00.385498 vnai-0.0.9/setup.cfg
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-07 13:05:00.383847 vnai-0.0.9/vnai/
--rw-r--r--   0 mrthinh    (501) staff       (20)    17531 2024-05-07 13:01:44.000000 vnai-0.0.9/vnai/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-07 13:05:00.384877 vnai-0.0.9/vnai.egg-info/
--rw-r--r--   0 mrthinh    (501) staff       (20)      573 2024-05-07 13:05:00.000000 vnai-0.0.9/vnai.egg-info/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)      180 2024-05-07 13:05:00.000000 vnai-0.0.9/vnai.egg-info/SOURCES.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-07 13:05:00.000000 vnai-0.0.9/vnai.egg-info/dependency_links.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)       47 2024-05-07 13:05:00.000000 vnai-0.0.9/vnai.egg-info/requires.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        5 2024-05-07 13:05:00.000000 vnai-0.0.9/vnai.egg-info/top_level.txt
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-11 13:54:06.904052 vnai-0.1.0/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      586 2024-05-11 13:54:06.903829 vnai-0.1.0/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)      140 2024-05-06 15:49:50.000000 vnai-0.1.0/pyproject.toml
+-rw-r--r--   0 mrthinh    (501) staff       (20)       38 2024-05-11 13:54:06.904102 vnai-0.1.0/setup.cfg
+-rw-r--r--   0 mrthinh    (501) staff       (20)      697 2024-05-11 13:46:39.000000 vnai-0.1.0/setup.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-11 13:54:06.902342 vnai-0.1.0/vnai/
+-rw-r--r--   0 mrthinh    (501) staff       (20)    17618 2024-05-11 13:52:00.000000 vnai-0.1.0/vnai/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-11 13:54:06.903501 vnai-0.1.0/vnai.egg-info/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      586 2024-05-11 13:54:06.000000 vnai-0.1.0/vnai.egg-info/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)      179 2024-05-11 13:54:06.000000 vnai-0.1.0/vnai.egg-info/SOURCES.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-11 13:54:06.000000 vnai-0.1.0/vnai.egg-info/dependency_links.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)       47 2024-05-11 13:54:06.000000 vnai-0.1.0/vnai.egg-info/requires.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        5 2024-05-11 13:54:06.000000 vnai-0.1.0/vnai.egg-info/top_level.txt
```

### Comparing `vnai-0.0.9/PKG-INFO` & `vnai-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: vnai
-Version: 0.0.9
+Version: 0.1.0
+Summary: :))
 Author: Vnstock HQ
 Author-email: support@vnstock.site
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnai-0.0.9/vnai/__init__.py` & `vnai-0.1.0/vnai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import json
 import base64
 from cryptography.fernet import Fernet
 
 TC_VAR = "ACCEPT_TC"
 TC_VAL = "tôi đồng ý"
 
+lmt = os.path.sep
 HOME_DIR = pathlib.Path.home()
 PROJECT_DIR = HOME_DIR / ".vnstock"
 ID_DIR = PROJECT_DIR / 'id'
 TG = b'gAAAAABmOPXPmFYXs94INEralMxhR38geFp91TZRLP29C41OoO0k7D7QiXIR2nWl5PCEoQCKECZw8b-Xeek3oqT6LcpcpJsAPyOGOBTX5cw_r5Mv0o8SBLa53jOeuVAwCAhId_BpMtOO'
 TC_PATH = ID_DIR / "terms_agreement.txt"
 
 TERMS_AND_CONDITIONS = """
@@ -78,23 +79,24 @@
 class VnstockInitializer:
     def __init__(self, target, tc=TERMS_AND_CONDITIONS):
         self.terms_and_conditions = tc
         self.home_dir = HOME_DIR
         self.project_dir = PROJECT_DIR
         self.id_dir = ID_DIR
         self.terms_file_path = TC_PATH
+        self.env_config = ID_DIR / "environment.json"
         self.RH = 'asejruyy^&%$#W2vX>NfwrevDRESWR'
         self.LH = 'YMAnhuytr%$59u90y7j-mjhgvyFTfbiuUYH'
 
         # Create the project directory if it doesn't exist
         self.project_dir.mkdir(exist_ok=True)
         self.id_dir.mkdir(exist_ok=True)
         self.target = target
 
-        kb = (str(self.project_dir).split("/")[-1] + str(self.id_dir).split("/")[-1] + str(self.terms_file_path).split("/")[-1]).ljust(32)[:32].encode('utf-8')
+        kb = (str(self.project_dir).split(lmt)[-1] + str(self.id_dir).split(lmt)[-1] + str(self.terms_file_path).split(lmt)[-1]).ljust(32)[:32].encode('utf-8')
         kb64 = base64.urlsafe_b64encode(kb)
         self.cph = Fernet(kb64)
 
     def system_info(self):
         """
         Gathers information about the environment and system.
         """
@@ -224,27 +226,27 @@
         data = {
             "systems": HARDWARE,
             "accepted_agreement": True,
             "installed_packages": self.packages_installed(),
         }
 
         # save data to a json file in id folder
-        with open(self.id_dir / "environment.json", "w", encoding="utf-8") as f:
+        with open(self.env_config, "w", encoding="utf-8") as f:
             f.write(json.dumps(data, indent=4))
 
         try:
             response = requests.post(WH, json=data)
         except:
             raise SystemExit("Không thể gửi dữ liệu phân tích. Vui lòng kiểm tra kết nối mạng và thử lại sau.")
 
     def check_terms_accepted(self):
         """
         Checks if terms and conditions are accepted.
         """
-        if not self.terms_file_path.exists():
+        if not self.env_config.exists() or not self.terms_file_path.exists():
             # If not, ask for acceptance
             accepted = self.show_terms_and_conditions()
             if not accepted:
                 raise SystemExit("Điều khoản và điều kiện không được chấp nhận. Không thể tiếp tục.")
             else:
                 self.log_analytics_data()
```

### Comparing `vnai-0.0.9/vnai.egg-info/PKG-INFO` & `vnai-0.1.0/vnai.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: vnai
-Version: 0.0.9
+Version: 0.1.0
+Summary: :))
 Author: Vnstock HQ
 Author-email: support@vnstock.site
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

