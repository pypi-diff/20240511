# Comparing `tmp/sonatoki-0.1.4.tar.gz` & `tmp/sonatoki-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonatoki-0.1.4.tar", last modified: Thu May  9 15:18:28 2024, max compression
+gzip compressed data, was "sonatoki-0.1.5.tar", last modified: Sat May 11 17:49:31 2024, max compression
```

## Comparing `sonatoki-0.1.4.tar` & `sonatoki-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    34523 2024-05-09 15:18:10.812224 sonatoki-0.1.4/LICENSE
--rw-r--r--   0        0        0     4765 2024-05-09 15:18:10.812224 sonatoki-0.1.4/README.md
--rw-r--r--   0        0        0     2013 2024-05-09 15:18:28.876055 sonatoki-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1160 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Cleaners.py
--rw-r--r--   0        0        0     1935 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Configs.py
--rw-r--r--   0        0        0     4190 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Filters.py
--rw-r--r--   0        0        0     4205 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Preprocessors.py
--rw-r--r--   0        0        0     4129 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Scorers.py
--rw-r--r--   0        0        0     1942 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/Tokenizers.py
--rw-r--r--   0        0        0        0 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/__init__.py
--rw-r--r--   0        0        0       82 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/__main__.py
--rw-r--r--   0        0        0     1647 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/constants.py
--rw-r--r--   0        0        0     4343 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/ilo.py
--rw-r--r--   0        0        0   271013 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/linku.json
--rw-r--r--   0        0        0    77650 2024-05-09 15:18:10.816224 sonatoki-0.1.4/src/sonatoki/sandbox.json
--rw-r--r--   0        0        0        0 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      680 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_cleaners.py
--rw-r--r--   0        0        0     2530 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_filters.py
--rw-r--r--   0        0        0     4063 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_ilo.py
--rw-r--r--   0        0        0     4145 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_preprocessors.py
--rw-r--r--   0        0        0     1062 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_scorers.py
--rw-r--r--   0        0        0     3039 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_tokenize.py
--rw-r--r--   0        0        0      821 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/test_utils.py
--rw-r--r--   0        0        0      151 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/tokenize_cases/tokenize_sentences.yml
--rw-r--r--   0        0        0      743 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/tokenize_cases/tokenize_sentences_tok.yml
--rw-r--r--   0        0        0      440 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/tokenize_cases/tokenize_words.yml
--rw-r--r--   0        0        0     1522 2024-05-09 15:18:10.816224 sonatoki-0.1.4/tests/tokenize_cases/tokenize_words_tok.yml
--rw-r--r--   0        0        0     5225 1970-01-01 00:00:00.000000 sonatoki-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-11 17:49:19.493311 sonatoki-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4765 2024-05-11 17:49:19.493311 sonatoki-0.1.5/README.md
+-rw-r--r--   0        0        0     2013 2024-05-11 17:49:31.721320 sonatoki-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1160 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Cleaners.py
+-rw-r--r--   0        0        0     1935 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Configs.py
+-rw-r--r--   0        0        0     4470 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Filters.py
+-rw-r--r--   0        0        0     4441 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Preprocessors.py
+-rw-r--r--   0        0        0     3658 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Scorers.py
+-rw-r--r--   0        0        0     2310 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Tokenizers.py
+-rw-r--r--   0        0        0        0 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/__main__.py
+-rw-r--r--   0        0        0     4883 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/constants.py
+-rw-r--r--   0        0        0     3849 2024-05-11 17:49:19.497311 sonatoki-0.1.5/src/sonatoki/ilo.py
+-rw-r--r--   0        0        0   271013 2024-05-11 17:49:19.497311 sonatoki-0.1.5/src/sonatoki/linku.json
+-rw-r--r--   0        0        0    77650 2024-05-11 17:49:19.497311 sonatoki-0.1.5/src/sonatoki/sandbox.json
+-rw-r--r--   0        0        0        0 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      680 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_cleaners.py
+-rw-r--r--   0        0        0     2315 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_filters.py
+-rw-r--r--   0        0        0     4029 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_ilo.py
+-rw-r--r--   0        0        0     4145 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_preprocessors.py
+-rw-r--r--   0        0        0     1062 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_scorers.py
+-rw-r--r--   0        0        0     3039 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_tokenize.py
+-rw-r--r--   0        0        0      821 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_utils.py
+-rw-r--r--   0        0        0      151 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/tokenize_cases/tokenize_sentences.yml
+-rw-r--r--   0        0        0     1112 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/tokenize_cases/tokenize_sentences_tok.yml
+-rw-r--r--   0        0        0      440 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/tokenize_cases/tokenize_words.yml
+-rw-r--r--   0        0        0     1522 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/tokenize_cases/tokenize_words_tok.yml
+-rw-r--r--   0        0        0     5225 1970-01-01 00:00:00.000000 sonatoki-0.1.5/PKG-INFO
```

### Comparing `sonatoki-0.1.4/LICENSE` & `sonatoki-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/README.md` & `sonatoki-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/pyproject.toml` & `sonatoki-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sonatoki"
-version = "0.1.4"
+version = "0.1.5"
 description = "ilo li moku e toki li pana e sona ni: ni li toki ala toki pona?"
 authors = [
     { name = "jan Kekan San (@gregdan3)", email = "gregory.danielson3@gmail.com" },
 ]
 dependencies = [
     "unidecode>=1.3.6",
     "regex>=2023.12.25",
```

### Comparing `sonatoki-0.1.4/src/sonatoki/Cleaners.py` & `sonatoki-0.1.5/src/sonatoki/Cleaners.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/src/sonatoki/Configs.py` & `sonatoki-0.1.5/src/sonatoki/Configs.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/src/sonatoki/Filters.py` & `sonatoki-0.1.5/src/sonatoki/Filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # STL
+import re
 from abc import ABC, abstractmethod
 from typing import Set
 from functools import lru_cache as cache  # cache comes in 3.9
 
 # PDM
-import regex as re
+import regex
 from typing_extensions import override
 
 # LOCAL
 from sonatoki.constants import (
     VOWELS,
     CONSONANTS,
     NIMI_PU_SET,
     ALPHABET_SET,
+    UNICODE_PUNCT,
     ALLOWABLES_SET,
     NIMI_LINKU_SET,
     NIMI_PU_ALE_SET,
     NIMI_LINKU_ALE_SET,
+    PRUNED_POSIX_PUNCT,
     NIMI_LINKU_SANDBOX_SET,
 )
 
-re.DEFAULT_VERSION = re.VERSION1
+regex.DEFAULT_VERSION = regex.VERSION1
 
 
 class Filter(ABC):
     @classmethod
     @abstractmethod
     @cache(maxsize=None)
     def filter(cls, token: str) -> bool:
@@ -37,14 +40,24 @@
     @classmethod
     @override
     @cache(maxsize=None)
     def filter(cls, token: str) -> bool:
         return not not re.fullmatch(cls.pattern, token)
 
 
+class Regex1Filter(Filter):
+    pattern: "regex.Pattern[str]"
+
+    @classmethod
+    @override
+    @cache(maxsize=None)
+    def filter(cls, token: str) -> bool:
+        return not not regex.fullmatch(cls.pattern, token)
+
+
 class SetFilter(Filter):
     tokens: Set[str]
 
     @classmethod
     @override
     @cache(maxsize=None)
     def filter(cls, token: str) -> bool:
@@ -144,15 +157,15 @@
     @override
     @cache(maxsize=None)
     def filter(cls, msg: str) -> bool:
         return msg.isnumeric()
 
 
 class Punctuation(RegexFilter):
-    pattern = re.compile(r"[\p{Punctuation}\p{posix_punct}]+")
+    pattern = re.compile(rf"[{PRUNED_POSIX_PUNCT}{UNICODE_PUNCT}]+")
 
 
 __all__ = [
     "NimiPu",
     "NimiLinku",
     "NimiLinkuAle",
     "Phonotactic",
```

### Comparing `sonatoki-0.1.4/src/sonatoki/Preprocessors.py` & `sonatoki-0.1.5/src/sonatoki/Preprocessors.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,21 +13,22 @@
   - ArrowQuote
 
 Order does not generally matter, but if there were two overlapping containers such as in the string "|| spoiler ` monospace || `", order would matter.
 It is up to the user to order them appropriately.
 """
 
 # STL
+import re
 from abc import ABC, abstractmethod
 
 # PDM
-import regex as re
+import regex
 from typing_extensions import override
 
-re.DEFAULT_VERSION = re.VERSION1
+regex.DEFAULT_VERSION = regex.VERSION1
 
 
 class Preprocessor(ABC):
     @classmethod  # order matters
     @abstractmethod
     def process(cls, msg: str) -> str:
         raise NotImplementedError
@@ -39,14 +40,24 @@
 
     @classmethod
     @override
     def process(cls, msg: str) -> str:
         return re.sub(cls.pattern, cls.replace, msg)
 
 
+class Regex1Preprocessor(Preprocessor):
+    pattern: "regex.Pattern[str]"
+    replace: str = " "
+
+    @classmethod
+    @override
+    def process(cls, msg: str) -> str:
+        return regex.sub(cls.pattern, cls.replace, msg)
+
+
 """
 The following classes are Ignorables.
 
 Ignorables are tokens which do not count toward the accepted number of tokens
 or the total number of tokens.
 This is generally because they are considered external to Toki Pona.
```

### Comparing `sonatoki-0.1.4/src/sonatoki/Scorers.py` & `sonatoki-0.1.5/src/sonatoki/Scorers.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 # PDM
 from typing_extensions import override
 
 # LOCAL
 from sonatoki.Filters import Filter
 
-LOG = logging.getLogger(__name__)
-
 Number = Union[int, float]
 Weights = Dict[str, Number]
 
 
 def sigmoid(n: int) -> Number:
     return 1 / (1 + math.exp(-(0.30 * (n - 1))))
     # n-1 makes sigmoid(1) == 0.5
@@ -33,20 +31,15 @@
 class PassFail(Scorer):
     """The token passes any filter or fails all of them, scoring 1 or 0 respectively."""
 
     @classmethod
     def score_token(cls, token: str, filters: List[Type[Filter]]) -> Number:
         for f in filters:
             if f.filter(token):
-                score = 1
-                LOG.debug(
-                    "%12s.%s('%s') = %.2f", cls.__name__, f.__name__, token, score
-                )
-                return score
-        LOG.debug("%12s('%s') = 0.00", cls.__name__, token)
+                return 1
         return 0
 
     @classmethod
     @override
     def score(cls, tokens: List[str], filters: List[Type[Filter]]) -> Number:
         if not tokens:
             return 1
@@ -82,20 +75,15 @@
     This is desirable to avoid messages which would only match weaker filters, as these are less likely to be Toki Pona.
     """
 
     @classmethod
     def score_token(cls, token: str, filters: List[Type[Filter]], scale: int):
         for i, f in enumerate(filters):
             if f.filter(token):
-                score = scale - i
-                LOG.debug(
-                    "%12s.%s('%s') = %.2f", cls.__name__, f.__name__, token, score
-                )
-                return score
-        LOG.debug("%12s('%s') = 0.00", cls.__name__, token)
+                return scale - i
         return 0
 
     @classmethod
     @override
     def score(cls, tokens: List[str], filters: List[Type[Filter]]) -> Number:
         if not tokens:
             return 1
```

### Comparing `sonatoki-0.1.4/src/sonatoki/Tokenizers.py` & `sonatoki-0.1.5/src/sonatoki/Tokenizers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # STL
+import re
 from abc import ABC, abstractmethod
 from typing import List
 
 # PDM
-import regex as re
+import regex
 from typing_extensions import override
 
+# LOCAL
+from sonatoki.constants import UNICODE_PUNCT, PRUNED_POSIX_PUNCT
+
 try:
     # PDM
     import nltk
     from nltk.tokenize import sent_tokenize as __sent_tokenize_nltk
     from nltk.tokenize import word_tokenize as __word_tokenize_nltk
 except ImportError as e:
     nltk = e
 
 
-LANGUAGE = "english"  # for NLTK
+regex.DEFAULT_VERSION = regex.VERSION1
 
 
 class Tokenizer(ABC):
     @classmethod
     @abstractmethod
     def tokenize(cls, s: str) -> List[str]: ...
 
@@ -38,23 +42,34 @@
 
     @classmethod
     @override
     def tokenize(cls, s: str) -> List[str]:
         return [clean for word in re.split(cls.pattern, s) if (clean := word.strip())]
 
 
+class Regex1Tokenizer(Tokenizer):
+    pattern: "regex.Pattern[str]"
+
+    @classmethod
+    @override
+    def tokenize(cls, s: str) -> List[str]:
+        return [
+            clean for word in regex.split(cls.pattern, s) if (clean := word.strip())
+        ]
+
+
 class WordTokenizerTok(RegexTokenizer):
-    pattern = re.compile(r"""([\p{Punctuation}\p{posix_punct}]+|\s+)""")
-    # TODO: are <> or {} that common as *sentence* delims? [] are already a stretch
-    # TODO: do the typography characters matter?
-    # NOTE: | / and , are *not* sentence delimiters for my purpose
+    pattern = re.compile(rf"""([{PRUNED_POSIX_PUNCT}{UNICODE_PUNCT}]+|\s+)""")
 
 
 class SentTokenizerTok(RegexTokenizer):
-    pattern = re.compile(r"""(?<=[.?!:;·…“”"'()\[\]\-]|$)""")
+    pattern = re.compile(r"""(?<=[.?!:;·…“”"'()\[\]\-])|$""", flags=re.MULTILINE)
+    # TODO: are <> or {} that common as *sentence* delims? [] are already a stretch
+    # TODO: do the typography characters matter?
+    # NOTE: | / and , are *not* sentence delimiters for my purpose
 
 
 class WordTokenizerRe(RegexTokenizer):
     pattern = re.compile(r"""(?<=[.?!;:'"-])""")
 
 
 class SentTokenizerRe(RegexTokenizer):
```

### Comparing `sonatoki-0.1.4/src/sonatoki/ilo.py` & `sonatoki-0.1.5/src/sonatoki/ilo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # STL
-import logging
 from typing import List, Type, Tuple
 
 # LOCAL
 from sonatoki.Filters import Filter
 from sonatoki.Scorers import Number, Scorer
 from sonatoki.Cleaners import Cleaner
 from sonatoki.Tokenizers import Tokenizer
 from sonatoki.Preprocessors import Preprocessor
 
-LOG = logging.getLogger(__name__)
-
 
 class Ilo:
     __preprocessors: List[Type[Preprocessor]]
     __word_tokenizer: Type[Tokenizer]
     __cleaners: List[Type[Cleaner]]
     __ignoring_filters: List[Type[Filter]]
     __scoring_filters: List[Type[Filter]]
     __scorer: Type[Scorer]
     __passing_score: Number
-    logging_threshold: Number = -1
 
     def __init__(
         self,
         preprocessors: List[Type[Preprocessor]],
         cleaners: List[Type[Cleaner]],
         ignoring_filters: List[Type[Filter]],
         scoring_filters: List[Type[Filter]],
@@ -100,21 +96,13 @@
         preprocessed = self.preprocess(message)
         tokenized = self.word_tokenize(preprocessed)
         filtered = self.filter_tokens(tokenized)
         cleaned = self.clean_tokens(filtered)
         score = self.score_tokens(cleaned)
         result = score >= self.__passing_score
 
-        if score <= self.logging_threshold:
-            LOG.debug("msg: %.2f  %s", score, repr(message))
-            LOG.debug("preproc:   %s", repr(preprocessed))
-            LOG.debug("tokenized: %s", tokenized)
-            LOG.debug("filtered:  %s", filtered)
-            LOG.debug("cleaned:   %s", cleaned)
-        # TODO: Move to each function? Loses ability to control when logging occurs by threshold
-
         return preprocessed, tokenized, filtered, cleaned, score, result
 
     def is_toki_pona(self, message: str) -> bool:
         """Determines whether a single statement is or is not Toki Pona."""
         *_, result = self._is_toki_pona(message)
         return result
```

### Comparing `sonatoki-0.1.4/src/sonatoki/linku.json` & `sonatoki-0.1.5/src/sonatoki/linku.json`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/src/sonatoki/sandbox.json` & `sonatoki-0.1.5/src/sonatoki/sandbox.json`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/tests/test_cleaners.py` & `sonatoki-0.1.5/tests/test_cleaners.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/tests/test_filters.py` & `sonatoki-0.1.5/tests/test_filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -78,24 +78,23 @@
 
 @given(st.from_regex(PROPER_NAME_RE, fullmatch=True))
 def test_ProperName(s: str):
     res = ProperName.filter(s)
     assert res, repr(s)
 
 
-# I use `regex`'s Unicode property feature, which Hypothesis doesn't understand
-# So I have to provide a different regex tha doesn't technically match
-@given(st.from_regex(r"[^\w\s]+", fullmatch=True))
+@given(st.from_regex(Punctuation.pattern.pattern, fullmatch=True))
+@example("[]")
+@example(r"\\")
+@example(r"\"")
 @example("⟨·⟩")
 @example("…")
-@example("「　」")
+@example("「」")  # `　`
 @example(string.punctuation)
-@settings(suppress_health_check=[HealthCheck.filter_too_much])  # FIXME
 def test_Punctuation(s: str):
-    _ = assume(re.fullmatch(Punctuation.pattern.pattern, s))
     res = Punctuation.filter(s)
     assert res, repr(s)
 
 
 @given(st.from_regex(r"\d+", fullmatch=True))
 @example("124125")
 @example("99990000")
```

### Comparing `sonatoki-0.1.4/tests/test_ilo.py` & `sonatoki-0.1.5/tests/test_ilo.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from sonatoki.ilo import Ilo
 from sonatoki.Configs import LazyConfig, PrefConfig
 
 
 @pytest.fixture
 def ilo():
     ilo = Ilo(**PrefConfig)
-    # ilo.logging_threshold = 0.8
     return ilo
 
 
 @pytest.fixture()
 def lazy_ilo():
     ilo = Ilo(**LazyConfig)
     # ilo.logging_threshold = 0.8
```

### Comparing `sonatoki-0.1.4/tests/test_preprocessors.py` & `sonatoki-0.1.5/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/tests/test_scorers.py` & `sonatoki-0.1.5/tests/test_scorers.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/tests/test_tokenize.py` & `sonatoki-0.1.5/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/tests/test_utils.py` & `sonatoki-0.1.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/tests/tokenize_cases/tokenize_sentences_tok.yml` & `sonatoki-0.1.5/tests/tokenize_cases/tokenize_sentences_tok.yml`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,32 @@
     - "mu?"
     - "mu?"
 - name: "basic4"
   input: "mi mu. mi wawa."
   output:
     - "mi mu."
     - "mi wawa."
+- name: "empty"
+  input: ""
+  output: []
+- name: "whitespace"
+  input: "  \n  "
+  output: []
+- name: "newline basic"
+  input: "sina lon seme?\nmi wile lon poka...\n"
+  output:
+    - "sina lon seme?"
+    - "mi wile lon poka."
+    - "."
+    - "."
+- name: "newline alone"
+  input: "sina lon seme\nmi wile lon poka"
+  output:
+    - "sina lon seme"
+    - "mi wile lon poka"
 - name: "dash"
   input: "mi sona ala e ni- sina seme a"
   output:
     - "mi sona ala e ni-"
     - "sina seme a"
 - name: "comma"
   input: "mi mu tawa sina, mi wawa e sina."
```

### Comparing `sonatoki-0.1.4/tests/tokenize_cases/tokenize_words_tok.yml` & `sonatoki-0.1.5/tests/tokenize_cases/tokenize_words_tok.yml`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.4/PKG-INFO` & `sonatoki-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonatoki
-Version: 0.1.4
+Version: 0.1.5
 Summary: ilo li moku e toki li pana e sona ni: ni li toki ala toki pona?
 Author-Email: "jan Kekan San (@gregdan3)" <gregory.danielson3@gmail.com>
 License: AGPL-3.0-or-later
 Requires-Python: >=3.8
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: regex>=2023.12.25
 Requires-Dist: typing-extensions>=4.11.0
```

