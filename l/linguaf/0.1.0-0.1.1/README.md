# Comparing `tmp/linguaf-0.1.0.tar.gz` & `tmp/linguaf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/alex/LinguaF/dist/tmpo2d3_8a5/linguaf-0.1.0.tar", last modified: Sat Jun 12 19:02:46 2021, max compression
+gzip compressed data, was "linguaf-0.1.1.tar", last modified: Fri May 10 09:52:40 2024, max compression
```

## Comparing `linguaf-0.1.0.tar` & `linguaf-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-06-12 19:02:46.000000 linguaf-0.1.0/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-06-12 19:02:46.000000 linguaf-0.1.0/linguaf.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      542 2021-06-12 19:02:46.000000 linguaf-0.1.0/linguaf.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       47 2021-06-12 19:02:46.000000 linguaf-0.1.0/linguaf.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2021-06-12 19:02:46.000000 linguaf-0.1.0/linguaf.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       14 2021-06-12 19:02:46.000000 linguaf-0.1.0/linguaf.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)     4494 2021-06-12 19:02:46.000000 linguaf-0.1.0/linguaf.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2021-06-12 19:02:46.000000 linguaf-0.1.0/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)     1076 2021-05-09 17:40:36.000000 linguaf-0.1.0/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)     3699 2021-06-12 19:02:20.000000 linguaf-0.1.0/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-06-12 19:02:46.000000 linguaf-0.1.0/tests/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2021-05-16 14:51:24.000000 linguaf-0.1.0/tests/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)    12108 2021-05-20 15:33:08.000000 linguaf-0.1.0/tests/test_descriptive_statistics.py
--rw-r--r--   0 alex      (1000) alex      (1000)    13369 2021-06-12 19:02:20.000000 linguaf-0.1.0/tests/test_lexical_diversity.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2715 2021-06-12 19:02:20.000000 linguaf-0.1.0/tests/test_syntactical_complexity.py
--rw-r--r--   0 alex      (1000) alex      (1000)    16148 2021-05-20 11:49:49.000000 linguaf-0.1.0/tests/test_readability.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-06-12 19:02:46.000000 linguaf-0.1.0/linguaf/
--rw-r--r--   0 alex      (1000) alex      (1000)     1348 2021-06-12 19:02:20.000000 linguaf-0.1.0/linguaf/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4343 2021-06-12 19:02:20.000000 linguaf-0.1.0/linguaf/lexical_diversity.py
--rw-r--r--   0 alex      (1000) alex      (1000)    11896 2021-06-12 19:02:20.000000 linguaf-0.1.0/linguaf/descriptive_statistics.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-06-12 19:02:46.000000 linguaf-0.1.0/linguaf/resources/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-06-12 19:02:46.000000 linguaf-0.1.0/linguaf/resources/stopwords/
--rw-r--r--   0 alex      (1000) alex      (1000)     2294 2021-05-11 16:04:49.000000 linguaf-0.1.0/linguaf/resources/stopwords/ru.json
--rw-r--r--   0 alex      (1000) alex      (1000)     2191 2021-05-11 16:05:00.000000 linguaf-0.1.0/linguaf/resources/stopwords/en.json
--rw-r--r--   0 alex      (1000) alex      (1000)     1528 2021-06-12 19:02:20.000000 linguaf-0.1.0/linguaf/syntactical_complexity.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5558 2021-06-12 19:02:20.000000 linguaf-0.1.0/linguaf/readability.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4494 2021-06-12 19:02:46.000000 linguaf-0.1.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     1499 2021-06-12 19:02:20.000000 linguaf-0.1.0/setup.py
+drwxrwxr-x   0 ins-alex  (1000) ins-alex  (1000)        0 2024-05-10 09:52:40.714142 linguaf-0.1.1/
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     5319 2024-05-10 09:52:40.710142 linguaf-0.1.1/PKG-INFO
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     3459 2024-05-10 09:50:05.000000 linguaf-0.1.1/README.md
+drwxrwxr-x   0 ins-alex  (1000) ins-alex  (1000)        0 2024-05-10 09:52:40.706142 linguaf-0.1.1/linguaf/
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     1485 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/__init__.py
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)    15986 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/descriptive_statistics.py
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     4343 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/lexical_diversity.py
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     5545 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/readability.py
+drwxrwxr-x   0 ins-alex  (1000) ins-alex  (1000)        0 2024-05-10 09:52:40.706142 linguaf-0.1.1/linguaf/resources/
+drwxrwxr-x   0 ins-alex  (1000) ins-alex  (1000)        0 2024-05-10 09:52:40.710142 linguaf-0.1.1/linguaf/resources/stopwords/
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)      786 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/resources/stopwords/be.json
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     2989 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/resources/stopwords/de.json
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     2191 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/resources/stopwords/en.json
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     4370 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/resources/stopwords/es.json
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     1915 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/resources/stopwords/fr.json
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     2294 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/resources/stopwords/ru.json
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)    11450 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/resources/stopwords/zh.json
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     1528 2024-05-10 09:50:05.000000 linguaf-0.1.1/linguaf/syntactical_complexity.py
+drwxrwxr-x   0 ins-alex  (1000) ins-alex  (1000)        0 2024-05-10 09:52:40.706142 linguaf-0.1.1/linguaf.egg-info/
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     5319 2024-05-10 09:52:40.000000 linguaf-0.1.1/linguaf.egg-info/PKG-INFO
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)      714 2024-05-10 09:52:40.000000 linguaf-0.1.1/linguaf.egg-info/SOURCES.txt
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)        1 2024-05-10 09:52:40.000000 linguaf-0.1.1/linguaf.egg-info/dependency_links.txt
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)      125 2024-05-10 09:52:40.000000 linguaf-0.1.1/linguaf.egg-info/requires.txt
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)       14 2024-05-10 09:52:40.000000 linguaf-0.1.1/linguaf.egg-info/top_level.txt
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)       38 2024-05-10 09:52:40.714142 linguaf-0.1.1/setup.cfg
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     1527 2024-05-10 09:52:23.000000 linguaf-0.1.1/setup.py
+drwxrwxr-x   0 ins-alex  (1000) ins-alex  (1000)        0 2024-05-10 09:52:40.710142 linguaf-0.1.1/tests/
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)        0 2024-05-10 09:50:05.000000 linguaf-0.1.1/tests/__init__.py
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)    32095 2024-05-10 09:50:05.000000 linguaf-0.1.1/tests/test_descriptive_statistics.py
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)    13369 2024-05-10 09:50:05.000000 linguaf-0.1.1/tests/test_lexical_diversity.py
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)    16150 2024-05-10 09:50:05.000000 linguaf-0.1.1/tests/test_readability.py
+-rw-rw-r--   0 ins-alex  (1000) ins-alex  (1000)     2715 2024-05-10 09:50:05.000000 linguaf-0.1.1/tests/test_syntactical_complexity.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `linguaf-0.1.0/linguaf.egg-info/SOURCES.txt` & `linguaf-0.1.1/linguaf.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-LICENSE
 README.md
 setup.py
 linguaf/__init__.py
 linguaf/descriptive_statistics.py
 linguaf/lexical_diversity.py
 linguaf/readability.py
 linguaf/syntactical_complexity.py
 linguaf.egg-info/PKG-INFO
 linguaf.egg-info/SOURCES.txt
 linguaf.egg-info/dependency_links.txt
 linguaf.egg-info/requires.txt
 linguaf.egg-info/top_level.txt
+linguaf/resources/stopwords/be.json
+linguaf/resources/stopwords/de.json
 linguaf/resources/stopwords/en.json
+linguaf/resources/stopwords/es.json
+linguaf/resources/stopwords/fr.json
 linguaf/resources/stopwords/ru.json
+linguaf/resources/stopwords/zh.json
 tests/__init__.py
 tests/test_descriptive_statistics.py
 tests/test_lexical_diversity.py
 tests/test_readability.py
 tests/test_syntactical_complexity.py
```

### Comparing `linguaf-0.1.0/README.md` & `linguaf-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -122,16 +122,10 @@
 pip install .
 ```
 
 ## Language Support
 
 At the moment, library supports English and Russian languages for all the methods.
 
-## Open API
-
-The Swagger UI of the API is located here: http://webengineering.ins.hs-anhalt.de:41008/docs
-
-There is currently a request limit set up for 50 requests per minute. If you are beyond the limit, requests are moved to the queue.
-
 ## Citation
 
 TBD
```

### Comparing `linguaf-0.1.0/tests/test_lexical_diversity.py` & `linguaf-0.1.1/tests/test_lexical_diversity.py`

 * *Files identical despite different names*

### Comparing `linguaf-0.1.0/tests/test_syntactical_complexity.py` & `linguaf-0.1.1/tests/test_syntactical_complexity.py`

 * *Files identical despite different names*

### Comparing `linguaf-0.1.0/tests/test_readability.py` & `linguaf-0.1.1/tests/test_readability.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,33 +168,33 @@
 def test_coleman_readability():
     read_data_ru = [
         ([
              "Дивергенция — дифференциальный оператор, отображающий векторное поле на скалярное.",
              "То есть, в результате применения к векторному полю операции дифференцирования получается скалярное поле.",
              "Она определяет (для каждой точки), «насколько расходится входящее и исходящее из малой окрестности данной точки поле»",
              "Точнее, насколько расходятся входящий и исходящий потоки."
-         ], 20),
+         ], -9),
         ([
              "«Лунтик и его друзья» — российский мультсериал, ориентированный на семейную и детскую аудиторию.",
              "Транслируется на телевидении с 1 сентября 2006 года по настоящее время.",
              "Ключевой темой стали приключения маленького пушистого существа Лунтика — космического пришельца, который родился на Луне."
-         ], 24)
+         ], -3)
     ]
 
     read_data_en = [
         ([
              "In vector calculus, divergence is a vector operator that operates on a vector field, producing a scalar field giving the quantity of the vector field's source at each point.",
              "More technically, the divergence represents the volume density of the outward flux of a vector field from an infinitesimal volume around a given point."
-         ], 69),
+         ], 42),
         ([
              "Luntik and his friends (Russian: Лунтик и его друзья) or simply Luntik (Russian: Лунтик), in its English version better known as Moonzy, is a Russian animated series for children.",
              "The title character is a purple furry alien named Luntik/Moonzy.",
              "In the first episode Moonzy is shown hatching from an egg on the moon and then falling to Earth.",
              "All of the following series take place at a forest glade near a pond where Moonzy finds a new home."
-         ], 80)
+         ], 65)
     ]
 
     for d in read_data_ru:
         score = d[1]
         res = int(r.coleman_readability(d[0], 'ru', False))
 
         assert score == res
@@ -209,39 +209,39 @@
 def test_easy_listening():
     read_data_ru = [
         ([
              "Дивергенция — дифференциальный оператор, отображающий векторное поле на скалярное.",
              "То есть, в результате применения к векторному полю операции дифференцирования получается скалярное поле.",
              "Она определяет (для каждой точки), «насколько расходится входящее и исходящее из малой окрестности данной точки поле»",
              "Точнее, насколько расходятся входящий и исходящий потоки."
-         ], 2),
+         ], 8),
         ([
              "«Лунтик и его друзья» — российский мультсериал, ориентированный на семейную и детскую аудиторию.",
              "Транслируется на телевидении с 1 сентября 2006 года по настоящее время.",
              "Ключевой темой стали приключения маленького пушистого существа Лунтика — космического пришельца, который родился на Луне."
-         ], 2)
+         ], 9)
     ]
 
     read_data_en = [
         ([
              "In vector calculus, divergence is a vector operator that operates on a vector field, producing a scalar field giving the quantity of the vector field's source at each point.",
              "More technically, the divergence represents the volume density of the outward flux of a vector field from an infinitesimal volume around a given point."
-         ], 5),
+         ], 10),
         ([
              "Luntik and his friends (Russian: Лунтик и его друзья) or simply Luntik (Russian: Лунтик), in its English version better known as Moonzy, is a Russian animated series for children.",
              "The title character is a purple furry alien named Luntik/Moonzy.",
              "In the first episode Moonzy is shown hatching from an egg on the moon and then falling to Earth.",
              "All of the following series take place at a forest glade near a pond where Moonzy finds a new home."
-         ], 2)
+         ], 3)
     ]
 
     for d in read_data_ru:
         score = d[1]
         res = int(r.easy_listening(d[0], 'ru', False))
 
         assert score == res
 
     for d in read_data_en:
         score = d[1]
         res = int(r.easy_listening(d[0], 'en', False))
 
-        assert score == res
+        assert score == res
```

### Comparing `linguaf-0.1.0/linguaf/__init__.py` & `linguaf-0.1.1/linguaf/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 
-SUPPORTED_LANGS = ['en', 'ru']
-__version__ = '0.1.0'
+SUPPORTED_LANGS = ['en', 'ru', 'de', 'fr', 'es', 'zh', # stopwords from nltk
+                   'lt', 'be', 'uk', 'hy'] # stopwords from other sources
+__version__ = '0.1.1'
 
 
 def __load_json(filepath):
     data = None
-    with open(filepath) as f:
+    with open(filepath, encoding="utf8") as f:
         data = json.load(f)
     return data
 
 
 def __check_documents_param(param):
     if type(param) != list:
         raise TypeError(f"The documents parameter has to be list. Now: {type(param)}")
```

### Comparing `linguaf-0.1.0/linguaf/lexical_diversity.py` & `linguaf-0.1.1/linguaf/lexical_diversity.py`

 * *Files identical despite different names*

### Comparing `linguaf-0.1.0/linguaf/resources/stopwords/ru.json` & `linguaf-0.1.1/linguaf/resources/stopwords/ru.json`

 * *Files identical despite different names*

### Comparing `linguaf-0.1.0/linguaf/resources/stopwords/en.json` & `linguaf-0.1.1/linguaf/resources/stopwords/en.json`

 * *Files identical despite different names*

### Comparing `linguaf-0.1.0/linguaf/syntactical_complexity.py` & `linguaf-0.1.1/linguaf/syntactical_complexity.py`

 * *Files identical despite different names*

### Comparing `linguaf-0.1.0/linguaf/readability.py` & `linguaf-0.1.1/linguaf/readability.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     remove_stopwords -- boolean flag that shows if the function should exclude stopwords
     """
     __check_documents_param(documents)
     __check_lang_param(lang)
     __check_bool_param(remove_stopwords)
 
     words = get_words(documents, lang, remove_stopwords)
-    nws_one = number_of_n_syllable_words(words, lang, (1, 2))
+    nws_one = number_of_n_syllable_words(documents, lang, (1, 2), remove_stopwords)
 
     return 1.29*(100*nws_one/len(words)) - 38.45
 
 
 def easy_listening(documents: list, lang: str = 'en', remove_stopwords: bool = False) -> float:
     """Calculates Easy Listening score based on a list of textual documents.
     Publication: Fang 1966
@@ -125,11 +125,10 @@
     remove_stopwords -- boolean flag that shows if the function should exclude stopwords
     """
     __check_documents_param(documents)
     __check_lang_param(lang)
     __check_bool_param(remove_stopwords)
 
     nst = sentence_count(documents)
-    words = get_words(documents, lang, remove_stopwords)
-    nws_more_two = number_of_n_syllable_words(words, lang, (2, 15))
+    nws_more_two = number_of_n_syllable_words(documents, lang, (2, 15), remove_stopwords)
 
     return nws_more_two/nst
```

### Comparing `linguaf-0.1.0/setup.py` & `linguaf-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,28 +17,28 @@
     for req in reqs:
         names.append(req)
     return {'install_requires': names}
 
 
 setuptools.setup(
     name="linguaf",
-    version="0.1.0",
-    author="Aleksandr Perevalov",
+    version="0.1.1",
+    author="Aleksandr Perevalov, Paul Heinze, Andreas Both",
     author_email="perevalovproduction@gmail.com",
     description="Python package for calculating famous measures in computational linguistics",
     long_description=long_description,
     license="MIT",
     long_description_content_type="text/markdown",
     url="https://github.com/Perevalov/LinguaF",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     packages=setuptools.find_packages(),
     package_data={"": ["resources/stopwords/*.json"]},
     keywords="language features computational linguistics quantitative text analysis",
```

