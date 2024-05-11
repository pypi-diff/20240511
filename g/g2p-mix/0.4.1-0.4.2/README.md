# Comparing `tmp/g2p-mix-0.4.1.tar.gz` & `tmp/g2p-mix-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p-mix-0.4.1.tar", last modified: Thu Apr 25 15:28:30 2024, max compression
+gzip compressed data, was "g2p-mix-0.4.2.tar", last modified: Sat May 11 10:41:10 2024, max compression
```

## Comparing `g2p-mix-0.4.1.tar` & `g2p-mix-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.910365 g2p-mix-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 15:28:30.910365 g2p-mix-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.902364 g2p-mix-0.4.1/g2p_mix/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/g2p_eng.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/g2p_mix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.902364 g2p-mix-0.4.1/g2p_mix/nltk_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.906365 g2p-mix-0.4.1/g2p_mix/nltk_data/corpora/
--rw-r--r--   0 runner    (1001) docker     (127)   896069 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/nltk_data/corpora/cmudict.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.906365 g2p-mix-0.4.1/g2p_mix/nltk_data/taggers/
--rw-r--r--   0 runner    (1001) docker     (127)  2526731 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/tone_sandhi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.906365 g2p-mix-0.4.1/g2p_mix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:28:30.910365 g2p-mix-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.368895 g2p-mix-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-11 10:41:10.368895 g2p-mix-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.360895 g2p-mix-0.4.2/g2p_mix/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/g2p_eng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/g2p_jyut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/g2p_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/g2p_pth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.360895 g2p-mix-0.4.2/g2p_mix/nltk_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.360895 g2p-mix-0.4.2/g2p_mix/nltk_data/corpora/
+-rw-r--r--   0 runner    (1001) docker     (127)   896069 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/nltk_data/corpora/cmudict.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.364895 g2p-mix-0.4.2/g2p_mix/nltk_data/taggers/
+-rw-r--r--   0 runner    (1001) docker     (127)  2526731 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/tone_sandhi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.360895 g2p-mix-0.4.2/g2p_mix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 10:41:10.368895 g2p-mix-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/setup.py
```

### Comparing `g2p-mix-0.4.1/LICENSE` & `g2p-mix-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.1/PKG-INFO` & `g2p-mix-0.4.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.4.1
+Version: 0.4.2
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,33 +12,60 @@
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 Provides-Extra: g2pw
 License-File: LICENSE
 
 # g2p-mix
 
+- Cantonese: [pycantonese](https://github.com/jacksonllee/pycantonese)
+- English: [g2p_en](https://github.com/Kyubyong/g2p)
+- Mandarin: [pypinyin](https://github.com/mozillazg/python-pinyin)
+
+## Usage
+
 ```bash
 $ pip install g2p-mix
 $ python
 ```
 
+### Mandarin
+
 ```python
 >>> from g2p_mix import G2pMix
->>> G2pMix().g2p("你这个idea, 不太make sense。")
+>>> G2pMix().g2p("你这个idea, 不太make sense。", sandhi=True)
 ```
 
 ```json
 [
   { "word": "你", "phones": ["n", "i3"], "lang": "ZH" },
   { "word": "这", "phones": ["zh", "e4"], "lang": "ZH" },
   { "word": "个", "phones": ["g", "e4"], "lang": "ZH" },
   { "word": "idea", "phones": ["AY0", "D", "IY1", "AH0"], "lang": "EN" },
   { "word": ",", "phones": ",", "lang": "SYM" },
-  { "word": "不", "phones": ["b", "u4"], "lang": "ZH" },
+  { "word": "不", "phones": ["b", "u2"], "lang": "ZH" },
   { "word": "太", "phones": ["t", "ai4"], "lang": "ZH" },
   { "word": "make", "phones": ["M", "EY1", "K"], "lang": "EN" },
   { "word": "sense", "phones": ["S", "EH1", "N", "S"], "lang": "EN" },
   { "word": "。", "phones": "。", "lang": "SYM" }
 ]
 ```
 
+### Cantonese
+
+```python
+>>> G2pMix(jyut=True).g2p("你这个idea, 不太make sense。")
+```
+
+```json
+{"word": "你", "phones": ["n", "ei5"], "lang": "ZH"}
+{"word": "這", "phones": ["z", "e3"], "lang": "ZH"}
+{"word": "個", "phones": ["g", "o3"], "lang": "ZH"}
+{"word": "idea", "phones": ["AY0", "D", "IY1", "AH0"], "lang": "EN"}
+{"word": ",", "phones": ",", "lang": "SYM"}
+{"word": "不", "phones": ["b", "at1"], "lang": "ZH"}
+{"word": "太", "phones": ["t", "aai3"], "lang": "ZH"}
+{"word": "make", "phones": ["M", "EY1", "K"], "lang": "EN"}
+{"word": "sense", "phones": ["S", "EH1", "N", "S"], "lang": "EN"}
+{"word": "。", "phones": "。", "lang": "SYM"}
+```
+
```

### Comparing `g2p-mix-0.4.1/g2p_mix/__init__.py` & `g2p-mix-0.4.2/g2p_mix/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.1/g2p_mix/cli.py` & `g2p-mix-0.4.2/g2p_mix/cli.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.1/g2p_mix/constants.py` & `g2p-mix-0.4.2/g2p_mix/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -66,14 +66,34 @@
     (
         "a o e i u v er ai ei ao ou ia ie ua uo "
         "ve iao iou uai uei an ian uan van en in uen vn ang "
         "iang uang eng ing ueng ong iong ê ng mg io"
     ).split()
 )
 
+# https://www.ilc.cuhk.edu.hk/workshop/Chinese/Cantonese/Romanization/ch1_intro/1_history.aspx
+# 韵母分类：
+# - 单元音（单韵母）：i yu u e oe o a aa
+# - 复元音收 i、u 韵尾（复韵母）：iu ui ei eu eoi oi ou ai au aai aau
+# - 单元音收 m、n、ng 鼻音韵尾（鼻音韵母）：im in ing yun um un ung em en eng eon oeng on ong am an ang aam aan aang
+# - 单元音收 p、t、k 塞音韵尾（塞音韵母）：ip it ik yut up ut uk ep et ek eot oet oek ot ok ap at ak aap aat aak
+# - 鼻音 m、ng 单独成韵：m ng
+ONSETS = set("b p m f d t n l g k ng h gw kw z c s j w".split())
+NUCLEUS = set("a aa eo oe i yu o e u m ng".split())
+CODAS = set("m n ng p t k".split())
+CFINALS = set(
+    (
+        "i yu u e oe o a aa "
+        "iu ui ei eu eoi oi ou ai au aai aau "
+        "im in ing yun um un ung em en eng eon oeng on ong am an ang aam aan aang "
+        "ip it ik yut up ut uk ep et ek eot oet oek ot ok ap at ak aap aat aak "
+        "m ng"
+    ).split()
+)
+
 # http://www.speech.cs.cmu.edu/cgi-bin/cmudict
 STRESS = {"", "0", "1", "2"}
 
 # 39
 PHONES = set(
     (
         "AA AE AH AO AW AY B CH D DH EH ER EY F G HH IH IY "
```

### Comparing `g2p-mix-0.4.1/g2p_mix/g2p_eng.py` & `g2p-mix-0.4.2/g2p_mix/g2p_eng.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.1/g2p_mix/nltk_data/corpora/cmudict.zip` & `g2p-mix-0.4.2/g2p_mix/nltk_data/corpora/cmudict.zip`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.1/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip` & `g2p-mix-0.4.2/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.1/g2p_mix/token.py` & `g2p-mix-0.4.2/g2p_mix/token.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.1/g2p_mix/tone_sandhi.py` & `g2p-mix-0.4.2/g2p_mix/tone_sandhi.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.1/g2p_mix.egg-info/PKG-INFO` & `g2p-mix-0.4.2/g2p_mix.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.4.1
+Version: 0.4.2
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,33 +12,60 @@
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 Provides-Extra: g2pw
 License-File: LICENSE
 
 # g2p-mix
 
+- Cantonese: [pycantonese](https://github.com/jacksonllee/pycantonese)
+- English: [g2p_en](https://github.com/Kyubyong/g2p)
+- Mandarin: [pypinyin](https://github.com/mozillazg/python-pinyin)
+
+## Usage
+
 ```bash
 $ pip install g2p-mix
 $ python
 ```
 
+### Mandarin
+
 ```python
 >>> from g2p_mix import G2pMix
->>> G2pMix().g2p("你这个idea, 不太make sense。")
+>>> G2pMix().g2p("你这个idea, 不太make sense。", sandhi=True)
 ```
 
 ```json
 [
   { "word": "你", "phones": ["n", "i3"], "lang": "ZH" },
   { "word": "这", "phones": ["zh", "e4"], "lang": "ZH" },
   { "word": "个", "phones": ["g", "e4"], "lang": "ZH" },
   { "word": "idea", "phones": ["AY0", "D", "IY1", "AH0"], "lang": "EN" },
   { "word": ",", "phones": ",", "lang": "SYM" },
-  { "word": "不", "phones": ["b", "u4"], "lang": "ZH" },
+  { "word": "不", "phones": ["b", "u2"], "lang": "ZH" },
   { "word": "太", "phones": ["t", "ai4"], "lang": "ZH" },
   { "word": "make", "phones": ["M", "EY1", "K"], "lang": "EN" },
   { "word": "sense", "phones": ["S", "EH1", "N", "S"], "lang": "EN" },
   { "word": "。", "phones": "。", "lang": "SYM" }
 ]
 ```
 
+### Cantonese
+
+```python
+>>> G2pMix(jyut=True).g2p("你这个idea, 不太make sense。")
+```
+
+```json
+{"word": "你", "phones": ["n", "ei5"], "lang": "ZH"}
+{"word": "這", "phones": ["z", "e3"], "lang": "ZH"}
+{"word": "個", "phones": ["g", "o3"], "lang": "ZH"}
+{"word": "idea", "phones": ["AY0", "D", "IY1", "AH0"], "lang": "EN"}
+{"word": ",", "phones": ",", "lang": "SYM"}
+{"word": "不", "phones": ["b", "at1"], "lang": "ZH"}
+{"word": "太", "phones": ["t", "aai3"], "lang": "ZH"}
+{"word": "make", "phones": ["M", "EY1", "K"], "lang": "EN"}
+{"word": "sense", "phones": ["S", "EH1", "N", "S"], "lang": "EN"}
+{"word": "。", "phones": "。", "lang": "SYM"}
+```
+
```

### Comparing `g2p-mix-0.4.1/setup.py` & `g2p-mix-0.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup, find_packages
 
 
-with open("README.md", encoding="utf8") as fin:
-    long_description = fin.read()
-
 with open("requirements.txt", encoding="utf8") as f:
     requirements = f.readlines()
 extras_require = {"g2pw": ["torch", "modelscope", "pypinyin-g2pw"]}
 
 setup(
     name="g2p-mix",
     version=open("VERSION", encoding="utf8").read(),
     author="Zhendong Peng",
     author_email="pzd17@tsinghua.org.cn",
-    long_description=long_description,
+    long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     description="G2P mix",
     url="https://github.com/pengzhendong/g2p-mix",
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     extras_require=extras_require,
```

