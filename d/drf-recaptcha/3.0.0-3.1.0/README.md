# Comparing `tmp/drf-recaptcha-3.0.0.tar.gz` & `tmp/drf_recaptcha-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-recaptcha-3.0.0.tar", last modified: Sat Jul  1 15:24:36 2023, max compression
+gzip compressed data, was "drf_recaptcha-3.1.0.tar", last modified: Sat May 11 10:03:11 2024, max compression
```

## Comparing `drf-recaptcha-3.0.0.tar` & `drf_recaptcha-3.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:24:36.166619 drf-recaptcha-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-01 15:24:36.166619 drf-recaptcha-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:24:36.162618 drf-recaptcha-3.0.0/drf_recaptcha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:24:36.162618 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-01 15:24:36.166619 drf-recaptcha-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:24:36.166619 drf-recaptcha-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_secret_key_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:03:11.670037 drf_recaptcha-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-11 10:03:11.670037 drf_recaptcha-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:03:11.670037 drf_recaptcha-3.1.0/drf_recaptcha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/drf_recaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/drf_recaptcha/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/drf_recaptcha/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/drf_recaptcha/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/drf_recaptcha/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/drf_recaptcha/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/drf_recaptcha/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:03:11.670037 drf_recaptcha-3.1.0/drf_recaptcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-11 10:03:11.000000 drf_recaptcha-3.1.0/drf_recaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-11 10:03:11.000000 drf_recaptcha-3.1.0/drf_recaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 10:03:11.000000 drf_recaptcha-3.1.0/drf_recaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 10:03:11.000000 drf_recaptcha-3.1.0/drf_recaptcha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-11 10:03:11.000000 drf_recaptcha-3.1.0/drf_recaptcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-11 10:03:11.000000 drf_recaptcha-3.1.0/drf_recaptcha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-11 10:03:11.670037 drf_recaptcha-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:03:11.670037 drf_recaptcha-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/tests/test_secret_key_priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-11 10:03:06.000000 drf_recaptcha-3.1.0/tests/test_validator.py
```

### Comparing `drf-recaptcha-3.0.0/LICENSE.md` & `drf_recaptcha-3.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-3.0.0/PKG-INFO` & `drf_recaptcha-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-recaptcha
-Version: 3.0.0
+Version: 3.1.0
 Summary: Django rest framework recaptcha field serializer.
 Home-page: https://github.com/llybin/drf-recaptcha
 Author: Lev Lybin
 Author-email: lev.lybin@gmail.com
 License: MIT
 Keywords: django,drf,rest,django-rest-framework,reCAPTCHA,reCAPTCHA v2,reCAPTCHA v3
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,31 +12,35 @@
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: django>=3.2
+Requires-Dist: djangorestframework>=3.11
+Requires-Dist: django-ipware>=2.1
 
 # Django REST reCAPTCHA
 
 **Django REST reCAPTCHA v2 and v3 field serializer**
 
 [![CI](https://github.com/llybin/drf-recaptcha/workflows/tests/badge.svg)](https://github.com/llybin/drf-recaptcha/actions)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/a9b44d24cba74c75bca6472b2ee8da67)](https://www.codacy.com/app/llybin/drf-recaptcha?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=llybin/drf-recaptcha&amp;utm_campaign=Badge_Grade)
@@ -44,17 +48,17 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - License](https://img.shields.io/pypi/l/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 
 ## Requirements
 
-*   Python: 3.7, 3.8, 3.9, 3.10, 3.11
-*   Django: 3.2, 4.0, 4.1, 4.2
-*   DRF: 3.11, 3.12, 3.13, 3.14
+*   Python: 3.8, 3.9, 3.10, 3.11, 3.12
+*   Django: 3.2, 4.0, 4.1, 4.2, 5.0
+*   DRF: 3.11, 3.12, 3.13, 3.14, 3.15
 
 ## Installation
 
 1.  [Sign up for reCAPTCHA](https://www.google.com/recaptcha/)
 2.  Install with `pip install drf-recaptcha`
 3.  Add `"drf_recaptcha"` to your `INSTALLED_APPS` settings.
 4.  Set in settings `DRF_RECAPTCHA_SECRET_KEY`
@@ -171,14 +175,22 @@
 
 ### Priority of secret_key value
 
 1.  settings `DRF_RECAPTCHA_SECRET_KEY`
 2.  the argument `secret_key` of field
 3.  request.context["recaptcha_secret_key"]
 
+### Silence the check error
+
+If you need to disable the error, you can do so using the django settings.
+
+```python
+SILENCED_SYSTEM_CHECKS = ['drf_recaptcha.checks.recaptcha_system_check']
+```
+
 ## reCAPTCHA v3
 
 Validation is passed if the score value returned by Google is greater than or equal to required score.
 
 Required score value: `0.0 - 1.0`
 
 ### Priority of score value
```

### Comparing `drf-recaptcha-3.0.0/README.md` & `drf_recaptcha-3.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - License](https://img.shields.io/pypi/l/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 
 ## Requirements
 
-*   Python: 3.7, 3.8, 3.9, 3.10, 3.11
-*   Django: 3.2, 4.0, 4.1, 4.2
-*   DRF: 3.11, 3.12, 3.13, 3.14
+*   Python: 3.8, 3.9, 3.10, 3.11, 3.12
+*   Django: 3.2, 4.0, 4.1, 4.2, 5.0
+*   DRF: 3.11, 3.12, 3.13, 3.14, 3.15
 
 ## Installation
 
 1.  [Sign up for reCAPTCHA](https://www.google.com/recaptcha/)
 2.  Install with `pip install drf-recaptcha`
 3.  Add `"drf_recaptcha"` to your `INSTALLED_APPS` settings.
 4.  Set in settings `DRF_RECAPTCHA_SECRET_KEY`
@@ -135,14 +135,22 @@
 
 ### Priority of secret_key value
 
 1.  settings `DRF_RECAPTCHA_SECRET_KEY`
 2.  the argument `secret_key` of field
 3.  request.context["recaptcha_secret_key"]
 
+### Silence the check error
+
+If you need to disable the error, you can do so using the django settings.
+
+```python
+SILENCED_SYSTEM_CHECKS = ['drf_recaptcha.checks.recaptcha_system_check']
+```
+
 ## reCAPTCHA v3
 
 Validation is passed if the score value returned by Google is greater than or equal to required score.
 
 Required score value: `0.0 - 1.0`
 
 ### Priority of score value
```

### Comparing `drf-recaptcha-3.0.0/drf_recaptcha/checks.py` & `drf_recaptcha-3.1.0/drf_recaptcha/checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.conf import settings
-from django.core.checks import Tags, Warning, register
+from django.core.checks import Tags, Error, Warning, register
 from django.core.exceptions import ImproperlyConfigured
 
 from drf_recaptcha.constants import TEST_V2_SECRET_KEY
 
 
 @register(Tags.security)
 def recaptcha_system_check(app_configs, **kwargs):
@@ -11,17 +11,19 @@
 
     is_testing = getattr(settings, "DRF_RECAPTCHA_TESTING", False)
     if is_testing:
         return errors
 
     secret_key = getattr(settings, "DRF_RECAPTCHA_SECRET_KEY", None)
     if not secret_key:
-        raise ImproperlyConfigured("settings.DRF_RECAPTCHA_SECRET_KEY must be set.")
+        errors.append(
+            Error("settings.DRF_RECAPTCHA_SECRET_KEY must be set."),
+        )
 
-    if secret_key == TEST_V2_SECRET_KEY:
+    elif secret_key == TEST_V2_SECRET_KEY:
         errors.append(
             Warning(
                 "Google test key for reCAPTCHA v2 is used now.\n"
                 "If you use reCAPTCHA v2 - you will always get No CAPTCHA and all"
                 " verification requests will pass.\n"
                 "If you use reCAPTCHA v3 - all verification requests will fail.",
                 hint="Update settings.DRF_RECAPTCHA_SECRET_KEY",
```

### Comparing `drf-recaptcha-3.0.0/drf_recaptcha/client.py` & `drf_recaptcha-3.1.0/drf_recaptcha/client.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-3.0.0/drf_recaptcha/constants.py` & `drf_recaptcha-3.1.0/drf_recaptcha/constants.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-3.0.0/drf_recaptcha/fields.py` & `drf_recaptcha-3.1.0/drf_recaptcha/fields.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-3.0.0/drf_recaptcha/validators.py` & `drf_recaptcha-3.1.0/drf_recaptcha/validators.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-3.0.0/drf_recaptcha.egg-info/PKG-INFO` & `drf_recaptcha-3.1.0/drf_recaptcha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-recaptcha
-Version: 3.0.0
+Version: 3.1.0
 Summary: Django rest framework recaptcha field serializer.
 Home-page: https://github.com/llybin/drf-recaptcha
 Author: Lev Lybin
 Author-email: lev.lybin@gmail.com
 License: MIT
 Keywords: django,drf,rest,django-rest-framework,reCAPTCHA,reCAPTCHA v2,reCAPTCHA v3
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,31 +12,35 @@
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: django>=3.2
+Requires-Dist: djangorestframework>=3.11
+Requires-Dist: django-ipware>=2.1
 
 # Django REST reCAPTCHA
 
 **Django REST reCAPTCHA v2 and v3 field serializer**
 
 [![CI](https://github.com/llybin/drf-recaptcha/workflows/tests/badge.svg)](https://github.com/llybin/drf-recaptcha/actions)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/a9b44d24cba74c75bca6472b2ee8da67)](https://www.codacy.com/app/llybin/drf-recaptcha?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=llybin/drf-recaptcha&amp;utm_campaign=Badge_Grade)
@@ -44,17 +48,17 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - License](https://img.shields.io/pypi/l/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 
 ## Requirements
 
-*   Python: 3.7, 3.8, 3.9, 3.10, 3.11
-*   Django: 3.2, 4.0, 4.1, 4.2
-*   DRF: 3.11, 3.12, 3.13, 3.14
+*   Python: 3.8, 3.9, 3.10, 3.11, 3.12
+*   Django: 3.2, 4.0, 4.1, 4.2, 5.0
+*   DRF: 3.11, 3.12, 3.13, 3.14, 3.15
 
 ## Installation
 
 1.  [Sign up for reCAPTCHA](https://www.google.com/recaptcha/)
 2.  Install with `pip install drf-recaptcha`
 3.  Add `"drf_recaptcha"` to your `INSTALLED_APPS` settings.
 4.  Set in settings `DRF_RECAPTCHA_SECRET_KEY`
@@ -171,14 +175,22 @@
 
 ### Priority of secret_key value
 
 1.  settings `DRF_RECAPTCHA_SECRET_KEY`
 2.  the argument `secret_key` of field
 3.  request.context["recaptcha_secret_key"]
 
+### Silence the check error
+
+If you need to disable the error, you can do so using the django settings.
+
+```python
+SILENCED_SYSTEM_CHECKS = ['drf_recaptcha.checks.recaptcha_system_check']
+```
+
 ## reCAPTCHA v3
 
 Validation is passed if the score value returned by Google is greater than or equal to required score.
 
 Required score value: `0.0 - 1.0`
 
 ### Priority of score value
```

### Comparing `drf-recaptcha-3.0.0/drf_recaptcha.egg-info/SOURCES.txt` & `drf_recaptcha-3.1.0/drf_recaptcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-3.0.0/setup.cfg` & `drf_recaptcha-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-3.0.0/setup.py` & `drf_recaptcha-3.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 
 def read(f):
     return open(f, encoding="utf-8").read()
 
 
 setup(
     name="drf-recaptcha",
-    version="3.0.0",
+    version="3.1.0",
     description="Django rest framework recaptcha field serializer.",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="Lev Lybin",
     author_email="lev.lybin@gmail.com",
     license="MIT",
     url="https://github.com/llybin/drf-recaptcha",
     packages=find_packages(exclude=["tests*"]),
     install_requires=[
         "django>=3.2",
         "djangorestframework>=3.11",
         "django-ipware>=2.1",
     ],
     setup_requires=["pytest-runner"],
-    tests_require=["pytest", "pytest-django", "pytest-cov", "pytest-mock"],
-    python_requires=">=3.7",
+    tests_require=["pytest", "pytest-django", "pytest-cov", "pytest-mock", "pytz"],
+    python_requires=">=3.8",
     include_package_data=True,
     zip_safe=False,
     keywords=[
         "django",
         "drf",
         "rest",
         "django-rest-framework",
@@ -41,23 +41,24 @@
         "Environment :: Plugins",
         "Intended Audience :: Developers",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
+        "Framework :: Django :: 5.0",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Security",
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `drf-recaptcha-3.0.0/tests/test_checks.py` & `drf_recaptcha-3.1.0/tests/test_checks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-import pytest
-from django.core.exceptions import ImproperlyConfigured
-
 from drf_recaptcha.checks import recaptcha_system_check
 from drf_recaptcha.constants import TEST_V2_SECRET_KEY
 
 
 def test_warning_no_secret_key(settings):
     settings.DRF_RECAPTCHA_SECRET_KEY = None
 
-    with pytest.raises(ImproperlyConfigured) as exc_info:
-        recaptcha_system_check(None)
-
-    assert str(exc_info.value) == "settings.DRF_RECAPTCHA_SECRET_KEY must be set."
+    errors = recaptcha_system_check(None)
+    assert len(errors) == 1
+    assert errors[0].msg == "settings.DRF_RECAPTCHA_SECRET_KEY must be set."
 
 
 def test_silent_testing(settings):
     settings.DRF_RECAPTCHA_TESTING = True
     settings.DRF_RECAPTCHA_SECRET_KEY = None
 
     assert recaptcha_system_check(None) == []
```

### Comparing `drf-recaptcha-3.0.0/tests/test_fields.py` & `drf_recaptcha-3.1.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-3.0.0/tests/test_secret_key_priority.py` & `drf_recaptcha-3.1.0/tests/test_secret_key_priority.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-3.0.0/tests/test_serializers.py` & `drf_recaptcha-3.1.0/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-3.0.0/tests/test_testing.py` & `drf_recaptcha-3.1.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-3.0.0/tests/test_validator.py` & `drf_recaptcha-3.1.0/tests/test_validator.py`

 * *Files identical despite different names*

