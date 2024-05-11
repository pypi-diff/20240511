# Comparing `tmp/django_admin_reset-0.7.0-py3-none-any.whl.zip` & `tmp/django_admin_reset-0.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9214 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Aug-06 20:15 django_admin_reset/__init__.py
--rw-r--r--  2.0 unx     6191 b- defN 23-Aug-06 20:15 django_admin_reset/admin.py
--rw-r--r--  2.0 unx     1819 b- defN 23-Aug-06 20:16 django_admin_reset/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--  2.0 unx     2056 b- defN 23-Aug-06 20:15 django_admin_reset/locale/hu/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      317 b- defN 23-Aug-06 20:15 django_admin_reset/templates/admin/add_user_form.html
--rw-r--r--  2.0 unx      264 b- defN 23-Aug-06 20:15 django_admin_reset/templates/admin/change_user.html
--rw-r--r--  2.0 unx      545 b- defN 23-Aug-06 20:15 django_admin_reset/templates/admin/password_reset_url.html
--rw-r--r--  2.0 unx     1476 b- defN 23-Aug-06 20:16 django_admin_reset-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2522 b- defN 23-Aug-06 20:16 django_admin_reset-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 20:16 django_admin_reset-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Aug-06 20:16 django_admin_reset-0.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1154 b- defN 23-Aug-06 20:16 django_admin_reset-0.7.0.dist-info/RECORD
-12 files, 16477 bytes uncompressed, 7214 bytes compressed:  56.2%
+Zip file size: 9222 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 24-May-11 21:42 django_admin_reset/__init__.py
+-rw-r--r--  2.0 unx     6191 b- defN 24-May-11 21:42 django_admin_reset/admin.py
+-rw-r--r--  2.0 unx     1819 b- defN 24-May-11 21:43 django_admin_reset/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--  2.0 unx     2056 b- defN 24-May-11 21:42 django_admin_reset/locale/hu/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      317 b- defN 24-May-11 21:42 django_admin_reset/templates/admin/add_user_form.html
+-rw-r--r--  2.0 unx      264 b- defN 24-May-11 21:42 django_admin_reset/templates/admin/change_user.html
+-rw-r--r--  2.0 unx      545 b- defN 24-May-11 21:42 django_admin_reset/templates/admin/password_reset_url.html
+-rw-r--r--  2.0 unx     1476 b- defN 24-May-11 21:43 django_admin_reset-0.7.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2543 b- defN 24-May-11 21:43 django_admin_reset-0.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-11 21:43 django_admin_reset-0.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-11 21:43 django_admin_reset-0.7.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1154 b- defN 24-May-11 21:43 django_admin_reset-0.7.1.dist-info/RECORD
+12 files, 16498 bytes uncompressed, 7222 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: django_admin_reset/templates/admin/change_user.html
 Comment: 
 
 Filename: django_admin_reset/templates/admin/password_reset_url.html
 Comment: 
 
-Filename: django_admin_reset-0.7.0.dist-info/LICENSE
+Filename: django_admin_reset-0.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: django_admin_reset-0.7.0.dist-info/METADATA
+Filename: django_admin_reset-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: django_admin_reset-0.7.0.dist-info/WHEEL
+Filename: django_admin_reset-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: django_admin_reset-0.7.0.dist-info/top_level.txt
+Filename: django_admin_reset-0.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: django_admin_reset-0.7.0.dist-info/RECORD
+Filename: django_admin_reset-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_admin_reset/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.7.0'
+__version__ = '0.7.1'
```

## Comparing `django_admin_reset-0.7.0.dist-info/LICENSE` & `django_admin_reset-0.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_admin_reset-0.7.0.dist-info/METADATA` & `django_admin_reset-0.7.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: django-admin-reset
-Version: 0.7.0
+Version: 0.7.1
 Summary: Django admin password reset
 Home-page: https://github.com/tiborhari/django-admin-reset/
 Author: Tibor Hári
 Author-email: hartib@gmail.com
 Requires-Python: >=3.8, <4
 License-File: LICENSE
-Requires-Dist: django (!=4.0,<4.3,>=3.2)
+Requires-Dist: django !=4.0,<5.1,>=3.2
 Provides-Extra: babel
-Requires-Dist: babel (~=2.12.1) ; extra == 'babel'
+Requires-Dist: babel ~=2.12.1 ; extra == 'babel'
 Provides-Extra: docs
-Requires-Dist: sphinx (~=6.2.1) ; extra == 'docs'
-Requires-Dist: sphinx-rtd-theme (~=1.2.1) ; extra == 'docs'
+Requires-Dist: sphinx ~=7.3.7 ; extra == 'docs'
+Requires-Dist: sphinx-rtd-theme ~=2.0.0 ; extra == 'docs'
 Provides-Extra: testing
-Requires-Dist: flake8 (~=6.0.0) ; extra == 'testing'
-Requires-Dist: pytest (~=7.3.1) ; extra == 'testing'
-Requires-Dist: pytest-cov (~=4.1.0) ; extra == 'testing'
-Requires-Dist: pytest-django (~=4.5.2) ; extra == 'testing'
-Requires-Dist: tox (~=4.5.2) ; extra == 'testing'
+Requires-Dist: flake8 ~=6.0.0 ; extra == 'testing'
+Requires-Dist: pytest ~=7.3.1 ; extra == 'testing'
+Requires-Dist: pytest-cov ~=4.1.0 ; extra == 'testing'
+Requires-Dist: pytest-django ~=4.5.2 ; extra == 'testing'
+Requires-Dist: tox ~=4.5.2 ; extra == 'testing'
 
 Password reset for the Django admin interface
 =============================================
 
 This package provides views, to use the built-in Django password reset
 functionality from inside the admin interface.
 
@@ -76,9 +76,10 @@
 Compatible Django and Python versions:
 
 ==============  ========================
 Django version  Python versions
 ==============  ========================
 3.2 LTS         3.8, 3.9, 3.10
 4.1             3.8, 3.9, 3.10, 3.11
-4.2             3.8, 3.9, 3.10, 3.11
+4.2             3.8, 3.9, 3.10, 3.11, 3.12
+5.0             3.10, 3.11, 3.12
 ==============  ========================
```

## Comparing `django_admin_reset-0.7.0.dist-info/RECORD` & `django_admin_reset-0.7.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-django_admin_reset/__init__.py,sha256=09hol5ovL6ArILJIJZ-MiscnOjKa6RjaETmtdgJpW2c,22
+django_admin_reset/__init__.py,sha256=x2pOclYRECzfJMAd4sw67W_FEUEXKPUoISgurYPhSRg,22
 django_admin_reset/admin.py,sha256=_dFId_HljRyTroHLp04_z73EtnOKKH6Y8fIIOa0yk8g,6191
 django_admin_reset/locale/hu/LC_MESSAGES/django.mo,sha256=CJeEZsyr6bkk-Bsnq2TZXWFX3VP8y75lA3APOaqBwIo,1819
 django_admin_reset/locale/hu/LC_MESSAGES/django.po,sha256=lfjlvVkgYf6_oksEzL4W-7f-iMAw4pBEpGD3worI2Gk,2056
 django_admin_reset/templates/admin/add_user_form.html,sha256=tgdIIpA2zvlxs38lMvEZBCm4hsMiHPPpwMWQ73KMcjo,317
 django_admin_reset/templates/admin/change_user.html,sha256=9HqSy-1Elm2j2P6VWCJzuiPokrKNIyTmNdOVjSKXQHU,264
 django_admin_reset/templates/admin/password_reset_url.html,sha256=O_zg5XBc0YrBN4UaQPnp6Z6sb5xa1-PANbqvE7QuRn0,545
-django_admin_reset-0.7.0.dist-info/LICENSE,sha256=HUeCDOHFhxmzf_23dAKJJ5KOcMMLnnod30PvvTG9R_A,1476
-django_admin_reset-0.7.0.dist-info/METADATA,sha256=36x8sGY2gdsrmlgb1JAbnJIpF_ZecObDcs1ZxUwarRA,2522
-django_admin_reset-0.7.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-django_admin_reset-0.7.0.dist-info/top_level.txt,sha256=Ccyn6m1bbjFU-uqeAgvw8FwXpKY1q0pj1MB-LTXAPKU,19
-django_admin_reset-0.7.0.dist-info/RECORD,,
+django_admin_reset-0.7.1.dist-info/LICENSE,sha256=HUeCDOHFhxmzf_23dAKJJ5KOcMMLnnod30PvvTG9R_A,1476
+django_admin_reset-0.7.1.dist-info/METADATA,sha256=S8MVVQgQj_DgKbxhE35ZKU_DV1XoZgpk7ppCbn25Pro,2543
+django_admin_reset-0.7.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+django_admin_reset-0.7.1.dist-info/top_level.txt,sha256=Ccyn6m1bbjFU-uqeAgvw8FwXpKY1q0pj1MB-LTXAPKU,19
+django_admin_reset-0.7.1.dist-info/RECORD,,
```

