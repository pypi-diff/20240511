# Comparing `tmp/jphrase-0.0.0.tar.gz` & `tmp/jphrase-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jphrase-0.0.0.tar", last modified: Fri May 10 06:03:12 2024, max compression
+gzip compressed data, was "jphrase-0.0.1.tar", last modified: Sat May 11 14:25:59 2024, max compression
```

## Comparing `jphrase-0.0.0.tar` & `jphrase-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-10 06:03:12.195637 jphrase-0.0.0/
--rw-r--r--   0 jiro       (501) staff       (20)     1069 2024-05-09 08:54:48.000000 jphrase-0.0.0/LICENSE
--rw-r--r--   0 jiro       (501) staff       (20)      522 2024-05-10 06:03:12.195368 jphrase-0.0.0/PKG-INFO
--rw-r--r--   0 jiro       (501) staff       (20)       27 2024-05-09 08:54:48.000000 jphrase-0.0.0/README.md
--rw-r--r--   0 jiro       (501) staff       (20)       38 2024-05-10 06:03:12.195698 jphrase-0.0.0/setup.cfg
--rw-r--r--   0 jiro       (501) staff       (20)      874 2024-05-10 05:43:28.000000 jphrase-0.0.0/setup.py
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-10 06:03:12.192581 jphrase-0.0.0/src/
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-10 06:03:12.193576 jphrase-0.0.0/src/jphrase/
--rw-r--r--   0 jiro       (501) staff       (20)       74 2024-05-09 14:29:27.000000 jphrase-0.0.0/src/jphrase/__init__.py
--rw-r--r--   0 jiro       (501) staff       (20)     6259 2024-05-10 05:38:27.000000 jphrase-0.0.0/src/jphrase/phrase_splitter.py
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-10 06:03:12.195081 jphrase-0.0.0/src/jphrase.egg-info/
--rw-r--r--   0 jiro       (501) staff       (20)      522 2024-05-10 06:03:12.000000 jphrase-0.0.0/src/jphrase.egg-info/PKG-INFO
--rw-r--r--   0 jiro       (501) staff       (20)      285 2024-05-10 06:03:12.000000 jphrase-0.0.0/src/jphrase.egg-info/SOURCES.txt
--rw-r--r--   0 jiro       (501) staff       (20)        1 2024-05-10 06:03:12.000000 jphrase-0.0.0/src/jphrase.egg-info/dependency_links.txt
--rw-r--r--   0 jiro       (501) staff       (20)       21 2024-05-10 06:03:12.000000 jphrase-0.0.0/src/jphrase.egg-info/requires.txt
--rw-r--r--   0 jiro       (501) staff       (20)        8 2024-05-10 06:03:12.000000 jphrase-0.0.0/src/jphrase.egg-info/top_level.txt
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-10 06:03:12.194655 jphrase-0.0.0/tests/
--rw-r--r--   0 jiro       (501) staff       (20)     3340 2024-05-10 05:32:58.000000 jphrase-0.0.0/tests/test_phrase_splitter.py
+drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-11 14:25:59.994780 jphrase-0.0.1/
+-rw-r--r--   0 jiro       (501) staff       (20)     1069 2024-05-09 08:54:48.000000 jphrase-0.0.1/LICENSE
+-rw-r--r--   0 jiro       (501) staff       (20)     7497 2024-05-11 14:25:59.993900 jphrase-0.0.1/PKG-INFO
+-rw-r--r--   0 jiro       (501) staff       (20)     7054 2024-05-11 14:21:45.000000 jphrase-0.0.1/README.md
+-rw-r--r--   0 jiro       (501) staff       (20)       38 2024-05-11 14:25:59.994833 jphrase-0.0.1/setup.cfg
+-rw-r--r--   0 jiro       (501) staff       (20)      827 2024-05-11 13:51:45.000000 jphrase-0.0.1/setup.py
+drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-11 14:25:59.991541 jphrase-0.0.1/src/
+drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-11 14:25:59.992464 jphrase-0.0.1/src/jphrase/
+-rw-r--r--   0 jiro       (501) staff       (20)       74 2024-05-09 14:29:27.000000 jphrase-0.0.1/src/jphrase/__init__.py
+-rw-r--r--   0 jiro       (501) staff       (20)     6860 2024-05-11 14:03:55.000000 jphrase-0.0.1/src/jphrase/phrase_splitter.py
+drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-11 14:25:59.993623 jphrase-0.0.1/src/jphrase.egg-info/
+-rw-r--r--   0 jiro       (501) staff       (20)     7497 2024-05-11 14:25:59.000000 jphrase-0.0.1/src/jphrase.egg-info/PKG-INFO
+-rw-r--r--   0 jiro       (501) staff       (20)      251 2024-05-11 14:25:59.000000 jphrase-0.0.1/src/jphrase.egg-info/SOURCES.txt
+-rw-r--r--   0 jiro       (501) staff       (20)        1 2024-05-11 14:25:59.000000 jphrase-0.0.1/src/jphrase.egg-info/dependency_links.txt
+-rw-r--r--   0 jiro       (501) staff       (20)        8 2024-05-11 14:25:59.000000 jphrase-0.0.1/src/jphrase.egg-info/top_level.txt
+drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-11 14:25:59.993269 jphrase-0.0.1/tests/
+-rw-r--r--   0 jiro       (501) staff       (20)     3340 2024-05-10 05:32:58.000000 jphrase-0.0.1/tests/test_phrase_splitter.py
```

### Comparing `jphrase-0.0.0/LICENSE` & `jphrase-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jphrase-0.0.0/setup.py` & `jphrase-0.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="jphrase",  # PyPIに登録するパッケージ名
-    version="0.0.0",
+    version="0.0.1",
     packages=find_packages(where='src'),  # パッケージはsrcディレクトリ内にある
     package_dir={'': 'src'},  # パッケージのルートディレクトリをsrcに設定
-    install_requires=[
-        'mecab-python3',
-        'ipadic'
-    ],
+    install_requires=[],
     author="shimajiroxyz",
     author_email="shimaya.jiro@irl.sys.es.osaka-u.ac.jp",
     description="A Japanese phrase tokenizer",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/jiroshimaya/jphrase",
     classifiers=[
```

### Comparing `jphrase-0.0.0/src/jphrase/phrase_splitter.py` & `jphrase-0.0.1/src/jphrase/phrase_splitter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,55 @@
-import MeCab
-import ipadic
 
 class PhraseSplitter:
     OUTPUT_SURFACE = 'surface'
     OUTPUT_DETAILED = 'detailed'
     OUTPUT_CONCATENATED = 'concatenated'
 
-    def __init__(self, output_type=OUTPUT_SURFACE, consider_non_independent_nouns_as_breaks=True):
-        self.m = MeCab.Tagger(ipadic.MECAB_ARGS)  # MeCabのタグ付けオブジェクトを宣言
+    def __init__(self
+                 , output_type=OUTPUT_SURFACE
+                 , consider_non_independent_nouns_and_verbs_as_breaks=True):
+        import MeCab, ipadic
+        self.__tokenize = self.create_tokenizer_from_mecab_ipadic(MeCab.Tagger(ipadic.MECAB_ARGS))
         self.output_type = output_type
-        self.consider_non_independent_nouns_as_breaks = consider_non_independent_nouns_as_breaks
+        self.consider_non_independent_nouns_and_verbs_as_breaks = consider_non_independent_nouns_and_verbs_as_breaks
+    
+    def create_tokenizer_from_mecab_ipadic(self, tagger) -> callable:
+        
+        def tokenize(text: str) -> list[dict]:
+            mecab_result = tagger.parse(text).splitlines()
+            mecab_result = mecab_result[:-1]  # Remove the last line as it is unnecessary
+            tokens = []
+            for line in mecab_result:
+                if '\t' not in line:
+                    continue
+                parts = line.split('\t')
+                word_surface = parts[0]  # Surface form of the word
+                pos_info = parts[1].split(',')  # Part of speech and other grammatical information
+                token = {
+                    'surface_form': word_surface,
+                    'pos': pos_info[0],
+                    'pos_detail_1': pos_info[1] if len(pos_info) > 1 else '*',
+                    'pos_detail_2': pos_info[2] if len(pos_info) > 2 else '*',
+                    'pos_detail_3': pos_info[3] if len(pos_info) > 3 else '*',
+                    'conjugated_type': pos_info[4] if len(pos_info) > 4 else '*',
+                    'conjugated_form': pos_info[5] if len(pos_info) > 5 else '*',
+                    'basic_form': pos_info[6] if len(pos_info) > 6 else word_surface,
+                    'reading': pos_info[7] if len(pos_info) > 7 else '',
+                    'pronunciation': pos_info[8] if len(pos_info) > 8 else ''
+                }
+                tokens.append(token)
+            return tokens
+        
+        return tokenize
 
+    # This method is intended to be replaced by the tokenizer defined in __init__, so it is left empty here.
     def __tokenize(self, text: str) -> list[dict]:
-        mecab_result = self.m.parse(text).splitlines()
-        mecab_result = mecab_result[:-1]  # 最後の行は不要なので削除
-        tokens = []
-        for line in mecab_result:
-            if '\t' not in line:
-                continue
-            parts = line.split('\t')
-            word_surface = parts[0]  # 単語の表層形
-            pos_info = parts[1].split(',')  # 品詞やその他の文法情報
-            token = {
-                'surface_form': word_surface,
-                'pos': pos_info[0],
-                'pos_detail_1': pos_info[1] if len(pos_info) > 1 else '*',
-                'pos_detail_2': pos_info[2] if len(pos_info) > 2 else '*',
-                'pos_detail_3': pos_info[3] if len(pos_info) > 3 else '*',
-                'conjugated_type': pos_info[4] if len(pos_info) > 4 else '*',
-                'conjugated_form': pos_info[5] if len(pos_info) > 5 else '*',
-                'basic_form': pos_info[6] if len(pos_info) > 6 else word_surface,
-                'reading': pos_info[7] if len(pos_info) > 7 else '',
-                'pronunciation': pos_info[8] if len(pos_info) > 8 else ''
-            }
-            tokens.append(token)
-        return tokens
+        pass
     
-    def __should_break_before_token(self, token: dict, current_phrase: list[dict], consider_non_independent_nouns_as_breaks: bool = True) -> bool:
+    def __should_break_before_token(self, token: dict, current_phrase: list[dict], consider_non_independent_nouns_and_verbs_as_breaks: bool = True) -> bool:
 
         if not current_phrase:
             return False
         if all(_token['pos'] == '記号' for _token in current_phrase):
             return False
                     
         phrase_break_pos_tags = ['名詞', '動詞', '接頭詞', '副詞', '感動詞', '形容詞', '形容動詞', '連体詞']
@@ -53,15 +62,15 @@
         previous_pos_detail = ','.join([previous_token['pos_detail_1'], previous_token['pos_detail_2'], previous_token['pos_detail_3']])
 
 
         if pos_info == '記号':
             return False
         
         is_phrase_break_pos = pos_info in phrase_break_pos_tags
-        if not consider_non_independent_nouns_as_breaks and '非自立' in pos_detail:
+        if not consider_non_independent_nouns_and_verbs_as_breaks and '非自立' in pos_detail:
             is_phrase_break_pos = False
 
         if is_phrase_break_pos:
             if previous_pos_info == '接頭詞':
                 return False
             elif '接尾' in pos_detail:
                 return False
@@ -74,55 +83,55 @@
                 return True
             
             return False
                 
         return True
             
         
-    def __split_text_into_detailed_phrases(self, text: str, consider_non_independent_nouns_as_breaks: bool = True) -> list[list[dict]]:
+    def __split_text_into_detailed_phrases(self, text: str, consider_non_independent_nouns_and_verbs_as_breaks: bool = True) -> list[list[dict]]:
         tokens = self.__tokenize(text)
         segmented_text = []
         current_phrase = []
 
         for token in tokens:
-            should_break = self.__should_break_before_token(token, current_phrase, consider_non_independent_nouns_as_breaks)
+            should_break = self.__should_break_before_token(token, current_phrase, consider_non_independent_nouns_and_verbs_as_breaks)
             if should_break:
                 if current_phrase:
                     segmented_text.append(current_phrase)
                 current_phrase = []
             current_phrase.append(token)
 
         if current_phrase:
             segmented_text.append(current_phrase)
         return segmented_text
     
-    def __split_text_into_surface_phrases(self, text: str, consider_non_independent_nouns_as_breaks: bool = True) -> list[str]:
-        detailed_phrases = self.__split_text_into_detailed_phrases(text, consider_non_independent_nouns_as_breaks)
+    def __split_text_into_surface_phrases(self, text: str, consider_non_independent_nouns_and_verbs_as_breaks: bool = True) -> list[str]:
+        detailed_phrases = self.__split_text_into_detailed_phrases(text, consider_non_independent_nouns_and_verbs_as_breaks)
         surface_phrases = [''.join(token['surface_form'] for token in phrase) for phrase in detailed_phrases]
         return surface_phrases
     
-    def __split_text_into_concatenated_phrases(self, text: str, consider_non_independent_nouns_as_breaks: bool = True) -> list[dict]:
-        detailed_phrases = self.__split_text_into_detailed_phrases(text, consider_non_independent_nouns_as_breaks)
+    def __split_text_into_concatenated_phrases(self, text: str, consider_non_independent_nouns_and_verbs_as_breaks: bool = True) -> list[dict]:
+        detailed_phrases = self.__split_text_into_detailed_phrases(text, consider_non_independent_nouns_and_verbs_as_breaks)
         concatenated_phrases = []
         for phrase in detailed_phrases:
             concatenated_phrase = {
                 'surface_form': ''.join(token['surface_form'] for token in phrase),
                 'pronunciation': ''.join(token['pronunciation'] for token in phrase if token['pronunciation'] and token['pos'] != '記号'),
                 'reading': ''.join(token['reading'] for token in phrase if token['reading'] and token['pos'] != '記号')
             }
             concatenated_phrases.append(concatenated_phrase)
         return concatenated_phrases
-    def split_text(self, text: str, output_type: str = None, consider_non_independent_nouns_as_breaks: bool = None):
-        if consider_non_independent_nouns_as_breaks is None:
-            consider_non_independent_nouns_as_breaks = self.consider_non_independent_nouns_as_breaks
+    def split_text(self, text: str, output_type: str = None, consider_non_independent_nouns_and_verbs_as_breaks: bool = None):
+        if consider_non_independent_nouns_and_verbs_as_breaks is None:
+            consider_non_independent_nouns_and_verbs_as_breaks = self.consider_non_independent_nouns_and_verbs_as_breaks
         output_type = output_type or self.output_type
         split_methods = {
             self.OUTPUT_SURFACE: self.__split_text_into_surface_phrases,
             self.OUTPUT_DETAILED: self.__split_text_into_detailed_phrases,
             self.OUTPUT_CONCATENATED: self.__split_text_into_concatenated_phrases
         }
         if output_type in split_methods:
-            return split_methods[output_type](text, consider_non_independent_nouns_as_breaks)
+            return split_methods[output_type](text, consider_non_independent_nouns_and_verbs_as_breaks)
         else:
             valid_types = ', '.join(split_methods.keys())
             raise ValueError(f"Invalid output type specified. Choose {valid_types}.")
```

### Comparing `jphrase-0.0.0/tests/test_phrase_splitter.py` & `jphrase-0.0.1/tests/test_phrase_splitter.py`

 * *Files identical despite different names*

