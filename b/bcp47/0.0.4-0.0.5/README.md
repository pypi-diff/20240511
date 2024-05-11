# Comparing `tmp/bcp47-0.0.4.tar.gz` & `tmp/bcp47-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bcp47-0.0.4.tar", last modified: Fri Nov 13 13:50:56 2020, max compression
+gzip compressed data, was "bcp47-0.0.5.tar", last modified: Sat May 11 16:04:40 2024, max compression
```

## Comparing `bcp47-0.0.4.tar` & `bcp47-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2020-11-13 13:50:56.854728 bcp47-0.0.4/
--rw-rw-rw-   0        0        0     2314 2020-11-13 13:50:56.853731 bcp47-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1553 2020-11-13 13:47:41.000000 bcp47-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2020-11-13 13:50:56.848745 bcp47-0.0.4/bcp47/
--rw-rw-rw-   0        0        0       21 2019-09-27 15:05:49.000000 bcp47-0.0.4/bcp47/__init__.py
--rw-rw-rw-   0        0        0    28864 2020-11-13 13:46:07.000000 bcp47-0.0.4/bcp47/bcp47.py
--rw-rw-rw-   0        0        0     3294 2020-11-13 13:46:03.000000 bcp47-0.0.4/bcp47/generate-bcp47.py
-drwxrwxrwx   0        0        0        0 2020-11-13 13:50:56.852733 bcp47-0.0.4/bcp47.egg-info/
--rw-rw-rw-   0        0        0     2314 2020-11-13 13:50:56.000000 bcp47-0.0.4/bcp47.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2020-11-13 13:50:56.000000 bcp47-0.0.4/bcp47.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-11-13 13:50:56.000000 bcp47-0.0.4/bcp47.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2020-11-13 13:50:56.000000 bcp47-0.0.4/bcp47.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-11-13 13:50:56.854728 bcp47-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      640 2020-11-13 13:48:43.000000 bcp47-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 16:04:40.744073 bcp47-0.0.5/
+-rw-rw-rw-   0        0        0     1092 2019-09-27 15:01:21.000000 bcp47-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1971 2024-05-11 16:04:40.742991 bcp47-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1553 2020-11-13 13:47:41.000000 bcp47-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 16:04:40.736019 bcp47-0.0.5/bcp47/
+-rw-rw-rw-   0        0        0       21 2019-09-27 15:05:49.000000 bcp47-0.0.5/bcp47/__init__.py
+-rw-rw-rw-   0        0        0    28864 2020-11-13 13:46:07.000000 bcp47-0.0.5/bcp47/bcp47.py
+-rw-rw-rw-   0        0        0     3294 2020-11-13 13:46:03.000000 bcp47-0.0.5/bcp47/generate-bcp47.py
+drwxrwxrwx   0        0        0        0 2024-05-11 16:04:40.740990 bcp47-0.0.5/bcp47.egg-info/
+-rw-rw-rw-   0        0        0     1971 2024-05-11 16:04:40.000000 bcp47-0.0.5/bcp47.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-05-11 16:04:40.000000 bcp47-0.0.5/bcp47.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 16:04:40.000000 bcp47-0.0.5/bcp47.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 16:04:40.000000 bcp47-0.0.5/bcp47.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 16:04:40.744073 bcp47-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      640 2024-05-11 16:04:22.000000 bcp47-0.0.5/setup.py
```

### Comparing `bcp47-0.0.4/PKG-INFO` & `bcp47-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 Metadata-Version: 2.1
 Name: bcp47
-Version: 0.0.4
+Version: 0.0.5
 Summary: Language tags made easy
 Home-page: https://github.com/highfestiva/bcp47.py
 Author: Jonas Byström
 Author-email: highfestiva@gmail.com
-License: UNKNOWN
-Description: # BCP47
-        Language tags are not your everyday ISO standard, but instead composed of an ISO-639 language code, and an ISO-3166 country/region code
-        (and occationally an ISO-15924 script tag for the written language).
-        
-        The file is generated from Microsoft's seminal piece, [MS-LCID].pdf.
-        
-        
-        ## Easy installation
-        
-        ```bash
-        $ pip install bcp47
-        ```
-        
-        
-        ## Example
-        
-        ```python
-        >>> import bcp47
-        
-        >>> 'dje' in bcp47.tags and 'es-DO' in bcp47.tags
-        True
-        
-        >>> [v for k,v in bcp47.languages.items() if 'English' in k]
-        ['en', 'en-AS', 'en-AI', 'en-AG', 'en-AU', 'en-AT', 'en-BS', 'en-BB', 'en-BE', 'en-BZ', 'en-BM', 'en-BW', 'en-IO', ...]
-        ```
-        
-        
-        ## Discontentment
-        
-        This package only lists the most common language codes. If you want a package to parse, validate and simplify full BCP47 language tags,
-        have a look at [langcodes](https://github.com/LuminosoInsight/langcodes) or [langtags](https://github.com/jsommers/langtags).
-        
-        The BCP47 standard is 84 pages catering to specificity (such as `de-CH-1996` and `zh-CN-a-myext-x-private`) while this package currently
-        does not. Instead a highly pragmatic approach is used (some say [overly simplified](https://github.com/highfestiva/bcp47.py/issues/2))
-        where only the most common 900 or so language codes are listed, such as `fo-DK` and `iu-Cans-CA`.
-        
-        Microsoft's language codes are used to ensure some level of pragmatism, [KISS](https://en.wikipedia.org/wiki/KISS_principle). Validation you
-        will have to do yourself, see above for a trivial example.
-        
-        Enjoy at the best of your ability!
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# BCP47
+Language tags are not your everyday ISO standard, but instead composed of an ISO-639 language code, and an ISO-3166 country/region code
+(and occationally an ISO-15924 script tag for the written language).
+
+The file is generated from Microsoft's seminal piece, [MS-LCID].pdf.
+
+
+## Easy installation
+
+```bash
+$ pip install bcp47
+```
+
+
+## Example
+
+```python
+>>> import bcp47
+
+>>> 'dje' in bcp47.tags and 'es-DO' in bcp47.tags
+True
+
+>>> [v for k,v in bcp47.languages.items() if 'English' in k]
+['en', 'en-AS', 'en-AI', 'en-AG', 'en-AU', 'en-AT', 'en-BS', 'en-BB', 'en-BE', 'en-BZ', 'en-BM', 'en-BW', 'en-IO', ...]
+```
+
+
+## Discontentment
+
+This package only lists the most common language codes. If you want a package to parse, validate and simplify full BCP47 language tags,
+have a look at [langcodes](https://github.com/LuminosoInsight/langcodes) or [langtags](https://github.com/jsommers/langtags).
+
+The BCP47 standard is 84 pages catering to specificity (such as `de-CH-1996` and `zh-CN-a-myext-x-private`) while this package currently
+does not. Instead a highly pragmatic approach is used (some say [overly simplified](https://github.com/highfestiva/bcp47.py/issues/2))
+where only the most common 900 or so language codes are listed, such as `fo-DK` and `iu-Cans-CA`.
+
+Microsoft's language codes are used to ensure some level of pragmatism, [KISS](https://en.wikipedia.org/wiki/KISS_principle). Validation you
+will have to do yourself, see above for a trivial example.
+
+Enjoy at the best of your ability!
```

### Comparing `bcp47-0.0.4/README.md` & `bcp47-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bcp47-0.0.4/bcp47/bcp47.py` & `bcp47-0.0.5/bcp47/bcp47.py`

 * *Files identical despite different names*

### Comparing `bcp47-0.0.4/bcp47/generate-bcp47.py` & `bcp47-0.0.5/bcp47/generate-bcp47.py`

 * *Files identical despite different names*

### Comparing `bcp47-0.0.4/bcp47.egg-info/PKG-INFO` & `bcp47-0.0.5/bcp47.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 Metadata-Version: 2.1
 Name: bcp47
-Version: 0.0.4
+Version: 0.0.5
 Summary: Language tags made easy
 Home-page: https://github.com/highfestiva/bcp47.py
 Author: Jonas Byström
 Author-email: highfestiva@gmail.com
-License: UNKNOWN
-Description: # BCP47
-        Language tags are not your everyday ISO standard, but instead composed of an ISO-639 language code, and an ISO-3166 country/region code
-        (and occationally an ISO-15924 script tag for the written language).
-        
-        The file is generated from Microsoft's seminal piece, [MS-LCID].pdf.
-        
-        
-        ## Easy installation
-        
-        ```bash
-        $ pip install bcp47
-        ```
-        
-        
-        ## Example
-        
-        ```python
-        >>> import bcp47
-        
-        >>> 'dje' in bcp47.tags and 'es-DO' in bcp47.tags
-        True
-        
-        >>> [v for k,v in bcp47.languages.items() if 'English' in k]
-        ['en', 'en-AS', 'en-AI', 'en-AG', 'en-AU', 'en-AT', 'en-BS', 'en-BB', 'en-BE', 'en-BZ', 'en-BM', 'en-BW', 'en-IO', ...]
-        ```
-        
-        
-        ## Discontentment
-        
-        This package only lists the most common language codes. If you want a package to parse, validate and simplify full BCP47 language tags,
-        have a look at [langcodes](https://github.com/LuminosoInsight/langcodes) or [langtags](https://github.com/jsommers/langtags).
-        
-        The BCP47 standard is 84 pages catering to specificity (such as `de-CH-1996` and `zh-CN-a-myext-x-private`) while this package currently
-        does not. Instead a highly pragmatic approach is used (some say [overly simplified](https://github.com/highfestiva/bcp47.py/issues/2))
-        where only the most common 900 or so language codes are listed, such as `fo-DK` and `iu-Cans-CA`.
-        
-        Microsoft's language codes are used to ensure some level of pragmatism, [KISS](https://en.wikipedia.org/wiki/KISS_principle). Validation you
-        will have to do yourself, see above for a trivial example.
-        
-        Enjoy at the best of your ability!
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# BCP47
+Language tags are not your everyday ISO standard, but instead composed of an ISO-639 language code, and an ISO-3166 country/region code
+(and occationally an ISO-15924 script tag for the written language).
+
+The file is generated from Microsoft's seminal piece, [MS-LCID].pdf.
+
+
+## Easy installation
+
+```bash
+$ pip install bcp47
+```
+
+
+## Example
+
+```python
+>>> import bcp47
+
+>>> 'dje' in bcp47.tags and 'es-DO' in bcp47.tags
+True
+
+>>> [v for k,v in bcp47.languages.items() if 'English' in k]
+['en', 'en-AS', 'en-AI', 'en-AG', 'en-AU', 'en-AT', 'en-BS', 'en-BB', 'en-BE', 'en-BZ', 'en-BM', 'en-BW', 'en-IO', ...]
+```
+
+
+## Discontentment
+
+This package only lists the most common language codes. If you want a package to parse, validate and simplify full BCP47 language tags,
+have a look at [langcodes](https://github.com/LuminosoInsight/langcodes) or [langtags](https://github.com/jsommers/langtags).
+
+The BCP47 standard is 84 pages catering to specificity (such as `de-CH-1996` and `zh-CN-a-myext-x-private`) while this package currently
+does not. Instead a highly pragmatic approach is used (some say [overly simplified](https://github.com/highfestiva/bcp47.py/issues/2))
+where only the most common 900 or so language codes are listed, such as `fo-DK` and `iu-Cans-CA`.
+
+Microsoft's language codes are used to ensure some level of pragmatism, [KISS](https://en.wikipedia.org/wiki/KISS_principle). Validation you
+will have to do yourself, see above for a trivial example.
+
+Enjoy at the best of your ability!
```

### Comparing `bcp47-0.0.4/setup.py` & `bcp47-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='bcp47',
-    version='0.0.4',
+    version='0.0.5',
     author='Jonas Byström',
     author_email='highfestiva@gmail.com',
     description='Language tags made easy',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/highfestiva/bcp47.py',
     packages=['bcp47'],
```

