# Comparing `tmp/geotify-0.1.0.tar.gz` & `tmp/geotify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotify-0.1.0.tar", last modified: Sat May 11 03:02:26 2024, max compression
+gzip compressed data, was "geotify-0.2.0.tar", last modified: Sat May 11 18:06:30 2024, max compression
```

## Comparing `geotify-0.1.0.tar` & `geotify-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 jungmir    (501) staff       (20)        0 2024-05-11 03:02:26.571494 geotify-0.1.0/
-drwxr-xr-x   0 jungmir    (501) staff       (20)        0 2024-05-11 03:02:26.566232 geotify-0.1.0/.github/
-drwxr-xr-x   0 jungmir    (501) staff       (20)        0 2024-05-11 03:02:26.567427 geotify-0.1.0/.github/workflows/
--rw-r--r--   0 jungmir    (501) staff       (20)      655 2024-05-09 10:36:39.000000 geotify-0.1.0/.github/workflows/unittest.yaml
--rw-r--r--   0 jungmir    (501) staff       (20)       54 2024-05-11 02:48:51.000000 geotify-0.1.0/.gitignore
--rw-r--r--   0 jungmir    (501) staff       (20)      634 2024-05-09 10:36:39.000000 geotify-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 jungmir    (501) staff       (20)     1521 2024-05-09 10:36:39.000000 geotify-0.1.0/CONVENTION.md
--rw-r--r--   0 jungmir    (501) staff       (20)     4303 2024-05-11 03:02:26.571151 geotify-0.1.0/PKG-INFO
--rw-r--r--   0 jungmir    (501) staff       (20)     1442 2024-05-09 10:36:39.000000 geotify-0.1.0/README.md
--rw-r--r--   0 jungmir    (501) staff       (20)        6 2024-05-09 10:36:39.000000 geotify-0.1.0/VERSION
-drwxr-xr-x   0 jungmir    (501) staff       (20)        0 2024-05-11 03:02:26.567923 geotify-0.1.0/geotify/
--rw-r--r--   0 jungmir    (501) staff       (20)        0 2024-05-09 10:36:39.000000 geotify-0.1.0/geotify/__init__.py
--rw-r--r--   0 jungmir    (501) staff       (20)      756 2024-05-09 10:36:39.000000 geotify-0.1.0/geotify/command.py
-drwxr-xr-x   0 jungmir    (501) staff       (20)        0 2024-05-11 03:02:26.570378 geotify-0.1.0/geotify/datasets/
--rw-r--r--   0 jungmir    (501) staff       (20)    37830 2024-05-09 10:36:39.000000 geotify-0.1.0/geotify/datasets/Map_Korea.json
--rw-r--r--   0 jungmir    (501) staff       (20)   327424 2024-05-09 10:36:39.000000 geotify-0.1.0/geotify/datasets/TL_SCCO_CTPRVN.json
--rw-r--r--   0 jungmir    (501) staff       (20)     2782 2024-05-09 10:36:39.000000 geotify-0.1.0/geotify/datasets/aaa.csv
--rw-r--r--   0 jungmir    (501) staff       (20)   375223 2024-05-09 10:36:39.000000 geotify-0.1.0/geotify/datasets/base_korea_map.json
--rw-r--r--   0 jungmir    (501) staff       (20)      872 2024-05-09 10:36:39.000000 geotify-0.1.0/geotify/datasets/강원도.csv
--rw-r--r--   0 jungmir    (501) staff       (20)     1303 2024-05-09 10:36:39.000000 geotify-0.1.0/geotify/datasets/서울_인구밀도.csv
--rw-r--r--   0 jungmir    (501) staff       (20)     1741 2024-05-09 10:36:39.000000 geotify-0.1.0/geotify/datasets/전북특별자치도_인구밀도.csv
--rw-r--r--   0 jungmir    (501) staff       (20)    10591 2024-05-09 10:36:39.000000 geotify-0.1.0/geotify/map.py
--rw-r--r--   0 jungmir    (501) staff       (20)      651 2024-05-09 10:36:39.000000 geotify-0.1.0/geotify/utils.py
-drwxr-xr-x   0 jungmir    (501) staff       (20)        0 2024-05-11 03:02:26.570703 geotify-0.1.0/geotify.egg-info/
--rw-r--r--   0 jungmir    (501) staff       (20)     4303 2024-05-11 03:02:26.000000 geotify-0.1.0/geotify.egg-info/PKG-INFO
--rw-r--r--   0 jungmir    (501) staff       (20)      677 2024-05-11 03:02:26.000000 geotify-0.1.0/geotify.egg-info/SOURCES.txt
--rw-r--r--   0 jungmir    (501) staff       (20)        1 2024-05-11 03:02:26.000000 geotify-0.1.0/geotify.egg-info/dependency_links.txt
--rw-r--r--   0 jungmir    (501) staff       (20)       49 2024-05-11 03:02:26.000000 geotify-0.1.0/geotify.egg-info/entry_points.txt
--rw-r--r--   0 jungmir    (501) staff       (20)     1372 2024-05-11 03:02:26.000000 geotify-0.1.0/geotify.egg-info/requires.txt
--rw-r--r--   0 jungmir    (501) staff       (20)        8 2024-05-11 03:02:26.000000 geotify-0.1.0/geotify.egg-info/top_level.txt
--rw-r--r--   0 jungmir    (501) staff       (20)     1710 2024-05-11 03:02:18.000000 geotify-0.1.0/pyproject.toml
--rw-r--r--   0 jungmir    (501) staff       (20)       33 2024-05-09 10:36:39.000000 geotify-0.1.0/requirements.in
--rw-r--r--   0 jungmir    (501) staff       (20)     1372 2024-05-09 10:52:02.000000 geotify-0.1.0/requirements.txt
--rw-r--r--   0 jungmir    (501) staff       (20)       38 2024-05-11 03:02:26.571557 geotify-0.1.0/setup.cfg
-drwxr-xr-x   0 jungmir    (501) staff       (20)        0 2024-05-11 03:02:26.570517 geotify-0.1.0/test/
--rw-r--r--   0 jungmir    (501) staff       (20)     1005 2024-05-11 02:48:51.000000 geotify-0.1.0/test/test.py
+drwxr-xr-x   0 songle     (501) staff       (20)        0 2024-05-11 18:06:30.934651 geotify-0.2.0/
+drwxr-xr-x   0 songle     (501) staff       (20)        0 2024-05-11 18:06:30.922755 geotify-0.2.0/.github/
+drwxr-xr-x   0 songle     (501) staff       (20)        0 2024-05-11 18:06:30.924955 geotify-0.2.0/.github/workflows/
+-rw-r--r--   0 songle     (501) staff       (20)      655 2024-05-09 09:38:01.000000 geotify-0.2.0/.github/workflows/unittest.yaml
+-rw-r--r--   0 songle     (501) staff       (20)       54 2024-05-10 18:24:07.000000 geotify-0.2.0/.gitignore
+-rw-r--r--   0 songle     (501) staff       (20)      634 2024-05-09 09:38:01.000000 geotify-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 songle     (501) staff       (20)     1521 2024-05-09 09:38:01.000000 geotify-0.2.0/CONVENTION.md
+-rw-r--r--   0 songle     (501) staff       (20)     4366 2024-05-11 18:06:30.934190 geotify-0.2.0/PKG-INFO
+-rw-r--r--   0 songle     (501) staff       (20)     1442 2024-05-09 10:40:29.000000 geotify-0.2.0/README.md
+-rw-r--r--   0 songle     (501) staff       (20)        6 2024-05-11 18:05:50.000000 geotify-0.2.0/VERSION
+drwxr-xr-x   0 songle     (501) staff       (20)        0 2024-05-11 18:06:30.926396 geotify-0.2.0/geotify/
+-rw-r--r--   0 songle     (501) staff       (20)        0 2024-05-09 09:38:01.000000 geotify-0.2.0/geotify/__init__.py
+-rw-r--r--   0 songle     (501) staff       (20)      756 2024-05-09 09:38:01.000000 geotify-0.2.0/geotify/command.py
+drwxr-xr-x   0 songle     (501) staff       (20)        0 2024-05-11 18:06:30.932473 geotify-0.2.0/geotify/datasets/
+-rw-r--r--   0 songle     (501) staff       (20)    37830 2024-05-09 09:38:01.000000 geotify-0.2.0/geotify/datasets/Map_Korea.json
+-rw-r--r--   0 songle     (501) staff       (20)   327424 2024-05-09 09:38:01.000000 geotify-0.2.0/geotify/datasets/TL_SCCO_CTPRVN.json
+-rw-r--r--   0 songle     (501) staff       (20)     2782 2024-05-09 09:38:01.000000 geotify-0.2.0/geotify/datasets/aaa.csv
+-rw-r--r--   0 songle     (501) staff       (20)   375223 2024-04-30 03:17:28.000000 geotify-0.2.0/geotify/datasets/base_korea_map.json
+-rw-r--r--   0 songle     (501) staff       (20)      872 2024-05-09 09:38:01.000000 geotify-0.2.0/geotify/datasets/강원도.csv
+-rw-r--r--   0 songle     (501) staff       (20)     1303 2024-04-30 03:17:28.000000 geotify-0.2.0/geotify/datasets/서울_인구밀도.csv
+-rw-r--r--   0 songle     (501) staff       (20)     1741 2024-05-09 07:40:32.000000 geotify-0.2.0/geotify/datasets/전북특별자치도_인구밀도.csv
+-rw-r--r--   0 songle     (501) staff       (20)    10591 2024-05-09 09:38:01.000000 geotify-0.2.0/geotify/map.py
+-rw-r--r--   0 songle     (501) staff       (20)      651 2024-05-09 09:38:01.000000 geotify-0.2.0/geotify/utils.py
+drwxr-xr-x   0 songle     (501) staff       (20)        0 2024-05-11 18:06:30.933486 geotify-0.2.0/geotify.egg-info/
+-rw-r--r--   0 songle     (501) staff       (20)     4366 2024-05-11 18:06:30.000000 geotify-0.2.0/geotify.egg-info/PKG-INFO
+-rw-r--r--   0 songle     (501) staff       (20)      686 2024-05-11 18:06:30.000000 geotify-0.2.0/geotify.egg-info/SOURCES.txt
+-rw-r--r--   0 songle     (501) staff       (20)        1 2024-05-11 18:06:30.000000 geotify-0.2.0/geotify.egg-info/dependency_links.txt
+-rw-r--r--   0 songle     (501) staff       (20)       49 2024-05-11 18:06:30.000000 geotify-0.2.0/geotify.egg-info/entry_points.txt
+-rw-r--r--   0 songle     (501) staff       (20)     1372 2024-05-11 18:06:30.000000 geotify-0.2.0/geotify.egg-info/requires.txt
+-rw-r--r--   0 songle     (501) staff       (20)        8 2024-05-11 18:06:30.000000 geotify-0.2.0/geotify.egg-info/top_level.txt
+-rw-r--r--   0 songle     (501) staff       (20)     1565 2024-05-11 17:47:38.000000 geotify-0.2.0/pyproject.toml
+-rw-r--r--   0 songle     (501) staff       (20)       33 2024-05-09 09:38:01.000000 geotify-0.2.0/requirements.in
+-rw-r--r--   0 songle     (501) staff       (20)     1372 2024-05-09 10:46:35.000000 geotify-0.2.0/requirements.txt
+-rw-r--r--   0 songle     (501) staff       (20)       38 2024-05-11 18:06:30.934753 geotify-0.2.0/setup.cfg
+-rw-r--r--   0 songle     (501) staff       (20)      805 2024-05-11 17:40:35.000000 geotify-0.2.0/setup.py
+drwxr-xr-x   0 songle     (501) staff       (20)        0 2024-05-11 18:06:30.932860 geotify-0.2.0/test/
+-rw-r--r--   0 songle     (501) staff       (20)     1005 2024-05-09 11:39:19.000000 geotify-0.2.0/test/test.py
```

### Comparing `geotify-0.1.0/.github/workflows/unittest.yaml` & `geotify-0.2.0/.github/workflows/unittest.yaml`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/.pre-commit-config.yaml` & `geotify-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/CONVENTION.md` & `geotify-0.2.0/CONVENTION.md`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/PKG-INFO` & `geotify-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: geotify
-Version: 0.1.0
+Version: 0.2.0
 Summary: geotify
+Author: Yeogyeong, Song
+Author-email: challengef0802@gmail.com
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `geotify-0.1.0/README.md` & `geotify-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/geotify/command.py` & `geotify-0.2.0/geotify/command.py`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/geotify/datasets/Map_Korea.json` & `geotify-0.2.0/geotify/datasets/Map_Korea.json`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/geotify/datasets/TL_SCCO_CTPRVN.json` & `geotify-0.2.0/geotify/datasets/TL_SCCO_CTPRVN.json`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/geotify/datasets/aaa.csv` & `geotify-0.2.0/geotify/datasets/aaa.csv`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/geotify/datasets/base_korea_map.json` & `geotify-0.2.0/geotify/datasets/base_korea_map.json`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/geotify/datasets/강원도.csv` & `geotify-0.2.0/geotify/datasets/강원도.csv`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/geotify/datasets/서울_인구밀도.csv` & `geotify-0.2.0/geotify/datasets/서울_인구밀도.csv`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/geotify/datasets/전북특별자치도_인구밀도.csv` & `geotify-0.2.0/geotify/datasets/전북특별자치도_인구밀도.csv`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/geotify/map.py` & `geotify-0.2.0/geotify/map.py`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/geotify/utils.py` & `geotify-0.2.0/geotify/utils.py`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/geotify.egg-info/PKG-INFO` & `geotify-0.2.0/geotify.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: geotify
-Version: 0.1.0
+Version: 0.2.0
 Summary: geotify
+Author: Yeogyeong, Song
+Author-email: challengef0802@gmail.com
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `geotify-0.1.0/geotify.egg-info/SOURCES.txt` & `geotify-0.2.0/geotify.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .pre-commit-config.yaml
 CONVENTION.md
 README.md
 VERSION
 pyproject.toml
 requirements.in
 requirements.txt
+setup.py
 .github/workflows/unittest.yaml
 geotify/__init__.py
 geotify/command.py
 geotify/map.py
 geotify/utils.py
 geotify.egg-info/PKG-INFO
 geotify.egg-info/SOURCES.txt
```

### Comparing `geotify-0.1.0/geotify.egg-info/requires.txt` & `geotify-0.2.0/geotify.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/pyproject.toml` & `geotify-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 # 프로젝트 정보 작성
 [project]
 name = "geotify"    # 패키지 이름
 description = "geotify"    # 패키지 간단 설명
 readme = "README.md"    # README.md 파일 경로
 requires-python = ">=3.10"    # 파이썬 최소 버전
 classifiers = [
-    'Environment :: Console',    # 실행환경 (GUI or Console)
-    'Environment :: MacOS X',    # 실행환경 (OS)
-    'Operating System :: POSIX :: Linux',    # 실행환경 (OS)
-    'Programming Language :: Python :: 3',    # 프로그래밍 언어와 버전
-    'Programming Language :: Python :: 3.10'    # 프로그래밍 언어와 버전
-]
+     "Environment :: Console",
+     'Environment :: MacOS X',
+     "Operating System :: POSIX :: Linux",
+     "Programming Language :: Python :: 3",
+     "Programming Language :: Python :: 3.10"
+]       
 dynamic = ["version", "dependencies"]    # 동적 메타데이터 항목 정의
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.dynamic]    # 동적 메타데이터 상세 정의
 version = {file = ["VERSION"]}    # VERSION 파일에서 가져옴
```

### Comparing `geotify-0.1.0/requirements.txt` & `geotify-0.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `geotify-0.1.0/test/test.py` & `geotify-0.2.0/test/test.py`

 * *Files identical despite different names*

