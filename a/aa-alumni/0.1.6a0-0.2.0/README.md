# Comparing `tmp/aa_alumni-0.1.6a0.tar.gz` & `tmp/aa_alumni-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_alumni-0.1.6a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_alumni-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_alumni-0.1.6a0.tar` & `aa_alumni-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1069 2023-08-02 06:02:38.418779 aa_alumni-0.1.6a0/LICENSE
--rw-r--r--   0        0        0     1765 2023-10-11 09:45:29.537102 aa_alumni-0.1.6a0/README.md
--rw-r--r--   0        0        0      187 2023-10-11 10:20:11.106849 aa_alumni-0.1.6a0/alumni/__init__.py
--rw-r--r--   0        0        0      754 2023-05-19 01:48:27.000000 aa_alumni-0.1.6a0/alumni/admin.py
--rw-r--r--   0        0        0      174 2021-12-29 10:05:29.000000 aa_alumni-0.1.6a0/alumni/app_settings.py
--rw-r--r--   0        0        0      236 2023-10-08 05:17:48.592333 aa_alumni-0.1.6a0/alumni/apps.py
--rw-r--r--   0        0        0        0 2021-12-29 10:05:29.000000 aa_alumni-0.1.6a0/alumni/management/commands/__init__.py
--rw-r--r--   0        0        0      759 2023-04-04 01:33:41.000000 aa_alumni-0.1.6a0/alumni/management/commands/alumni_state.py
--rw-r--r--   0        0        0     3283 2021-12-30 06:12:41.000000 aa_alumni-0.1.6a0/alumni/migrations/0001_initial.py
--rw-r--r--   0        0        0      626 2021-12-30 01:47:27.000000 aa_alumni-0.1.6a0/alumni/migrations/0002_auto_20211230_0147.py
--rw-r--r--   0        0        0        0 2021-12-29 10:05:29.000000 aa_alumni-0.1.6a0/alumni/migrations/__init__.py
--rw-r--r--   0        0        0     2432 2022-09-18 05:25:56.000000 aa_alumni-0.1.6a0/alumni/models.py
--rw-r--r--   0        0        0      999 2023-10-11 09:32:04.127200 aa_alumni-0.1.6a0/alumni/providers.py
--rw-r--r--   0        0        0      789 2023-06-14 03:11:03.120792 aa_alumni-0.1.6a0/alumni/signals.py
--rw-r--r--   0        0        0     8058 2023-10-11 09:05:15.547395 aa_alumni-0.1.6a0/alumni/tasks.py
--rw-r--r--   0        0        0        0 2022-09-07 05:35:45.000000 aa_alumni-0.1.6a0/alumni/tests/__init__.py
--rw-r--r--   0        0        0     1892 2023-10-08 03:57:01.796059 aa_alumni-0.1.6a0/pyproject.toml
--rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 aa_alumni-0.1.6a0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 10:48:49.633332 aa_alumni-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1767 2024-05-11 10:48:49.633332 aa_alumni-0.2.0/README.md
+-rw-r--r--   0        0        0      186 2024-05-11 10:48:49.633332 aa_alumni-0.2.0/alumni/__init__.py
+-rw-r--r--   0        0        0      737 2024-05-11 10:48:49.633332 aa_alumni-0.2.0/alumni/admin.py
+-rw-r--r--   0        0        0      172 2024-05-11 10:48:49.634332 aa_alumni-0.2.0/alumni/app_settings.py
+-rw-r--r--   0        0        0      239 2024-05-11 10:48:49.634332 aa_alumni-0.2.0/alumni/apps.py
+-rw-r--r--   0        0        0     1249 2024-05-11 10:48:49.634332 aa_alumni-0.2.0/alumni/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-05-11 10:48:49.665331 aa_alumni-0.2.0/alumni/management/commands/__init__.py
+-rw-r--r--   0        0        0      759 2024-05-11 10:48:49.634332 aa_alumni-0.2.0/alumni/management/commands/alumni_state.py
+-rw-r--r--   0        0        0     3283 2024-05-11 10:48:49.634332 aa_alumni-0.2.0/alumni/migrations/0001_initial.py
+-rw-r--r--   0        0        0      626 2024-05-11 10:48:49.634332 aa_alumni-0.2.0/alumni/migrations/0002_auto_20211230_0147.py
+-rw-r--r--   0        0        0     1012 2024-05-11 10:48:49.634332 aa_alumni-0.2.0/alumni/migrations/0003_alter_alumnisetup_options_and_more.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:48:49.666331 aa_alumni-0.2.0/alumni/migrations/__init__.py
+-rw-r--r--   0        0        0     2206 2024-05-11 10:48:49.634332 aa_alumni-0.2.0/alumni/models.py
+-rw-r--r--   0        0        0      999 2024-05-11 10:48:49.635331 aa_alumni-0.2.0/alumni/providers.py
+-rw-r--r--   0        0        0      789 2024-05-11 10:48:49.635331 aa_alumni-0.2.0/alumni/signals.py
+-rw-r--r--   0        0        0     8058 2024-05-11 10:48:49.635331 aa_alumni-0.2.0/alumni/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:48:49.666331 aa_alumni-0.2.0/alumni/tests/__init__.py
+-rw-r--r--   0        0        0     1995 2024-05-11 10:48:49.635331 aa_alumni-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 aa_alumni-0.2.0/PKG-INFO
```

### Comparing `aa_alumni-0.1.6a0/LICENSE` & `aa_alumni-0.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Joel Falknau
+Copyright (c) 2021 Joel Falknau
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `aa_alumni-0.1.6a0/README.md` & `aa_alumni-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ### Step 1 - Prepare Auth
 
 Remove/Promote any state with a priority of `1`, Alumni is considered slightly better than the built in Guest State.
 
 ### Step 2 - Install from pip
 
-```bash
+```shell
 pip install aa-alumni
 ```
 
 ### Step 3 - Configure Auth settings
 
 Configure your Auth settings (`local.py`) as follows:
 
@@ -34,15 +34,15 @@
     'task': 'alumni.tasks.update_all_models',
     'schedule': crontab(minute=0, hour=0, day_of_week=3),
 }
 ```
 
 ### Step 4 - Update AA's State system
 
-```bash
+```shell
 python myauth/manage.py alumni_state
 ```
 
 ### Step 5 - Maintain Alliance Auth
 
 - Run migrations `python manage.py migrate`
 - Gather your staticfiles `python manage.py collectstatic`
```

### Comparing `aa_alumni-0.1.6a0/alumni/admin.py` & `aa_alumni-0.2.0/alumni/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,15 @@
     AlumniSetup, CharacterCorporationHistory, CorporationAllianceHistory,
 )
 
 
 @admin.register(AlumniSetup)
 class AlumniSetupAdmin(admin.ModelAdmin):
     search_fields = ['alumni_corporations', ]
-    filter_horizontal = [
-        "alumni_corporations",
-        "alumni_alliances"]
+    filter_horizontal = ["alumni_corporations", "alumni_alliances"]
 
 
 @admin.register(CorporationAllianceHistory)
 class CorporationAllianceHistoryAdmin(admin.ModelAdmin):
     search_fields = ['corporation_id', 'alliance_id']
     list_display = ('corporation_id', 'alliance_id')
```

### Comparing `aa_alumni-0.1.6a0/alumni/management/commands/alumni_state.py` & `aa_alumni-0.2.0/alumni/management/commands/alumni_state.py`

 * *Files identical despite different names*

### Comparing `aa_alumni-0.1.6a0/alumni/migrations/0001_initial.py` & `aa_alumni-0.2.0/alumni/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_alumni-0.1.6a0/alumni/migrations/0002_auto_20211230_0147.py` & `aa_alumni-0.2.0/alumni/migrations/0002_auto_20211230_0147.py`

 * *Files identical despite different names*

### Comparing `aa_alumni-0.1.6a0/alumni/models.py` & `aa_alumni-0.2.0/alumni/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,56 @@
-from django.core.exceptions import ValidationError
+from solo.models import SingletonModel
+
 from django.db import models
+from django.utils.translation import gettext as _
 
 from allianceauth.eveonline.models import (
     EveAllianceInfo, EveCharacter, EveCorporationInfo,
 )
 
 
-class AlumniSetup(models.Model):
+class AlumniSetup(SingletonModel):
     alumni_corporations = models.ManyToManyField(
         EveCorporationInfo,
         blank=True,
-        help_text="Characters with these Corps in their History will be given Alumni Status")
+        help_text=_("Characters with these Corps in their History will be given Alumni Status"))
     alumni_alliances = models.ManyToManyField(
         EveAllianceInfo,
         blank=True,
-        help_text="Characters with these Alliances in their History will be given Alumni Status")
+        help_text=_("Characters with these Alliances in their History will be given Alumni Status"))
 
-    def save(self, *args, **kwargs):
-        if not self.pk and AlumniSetup.objects.exists():
-            # Force a single object
-            raise ValidationError('There is can be only one \
-                                AlumniCorp instance')
-        self.pk = self.id = 1  # If this happens to be deleted and recreated, force it to be 1
-        return super().save(*args, **kwargs)
+    def __str__(self):
+        return _("Alumni Config")
 
     class Meta:
-        verbose_name_plural = "Alumni Config"
+        verbose_name = _("Alumni Config")
+        verbose_name_plural = _("Alumni Config")
 
 
 class CorporationAllianceHistory(models.Model):
     class Meta:
         constraints = [
             models.UniqueConstraint(fields=['corporation_id', 'record_id'], name="CorporationAllianceRecord"),
         ]
     corporation_id = models.PositiveIntegerField(db_index=True)
     alliance_id = models.PositiveIntegerField(blank=True, null=True, db_index=True)
     is_deleted = models.BooleanField(
         default=False,
-        help_text='True if the corporation has been deleted')
-    record_id = models.IntegerField(
-        help_text='An incrementing ID that can be used to canonically establish order of records in cases where dates may be ambiguous')
+        help_text=_("True if the corporation has been deleted"))
+    record_id = models.PositiveIntegerField(
+        help_text=_("An incrementing ID that can be used to canonically establish order of records in cases where dates may be ambiguous"))
     start_date = models.DateTimeField()
 
 
 class CharacterCorporationHistory(models.Model):
     class Meta:
         constraints = [
             models.UniqueConstraint(fields=['character', 'record_id'], name="CharacterCorporationRecord"),
         ]
-    character = models.ForeignKey(
-        EveCharacter,
-        on_delete=models.CASCADE)
+    character = models.ForeignKey(EveCharacter, on_delete=models.CASCADE)
     corporation_id = models.PositiveIntegerField()
     is_deleted = models.BooleanField(
         default=False,
-        help_text='True if the corporation has been deleted')
-    record_id = models.IntegerField(
-        help_text='An incrementing ID that can be used to canonically establish order of records in cases where dates may be ambiguous')
+        help_text=_("True if the corporation has been deleted"))
+    record_id = models.PositiveIntegerField(
+        help_text=_("An incrementing ID that can be used to canonically establish order of records in cases where dates may be ambiguous"))
     start_date = models.DateTimeField()
```

### Comparing `aa_alumni-0.1.6a0/alumni/providers.py` & `aa_alumni-0.2.0/alumni/providers.py`

 * *Files identical despite different names*

### Comparing `aa_alumni-0.1.6a0/alumni/signals.py` & `aa_alumni-0.2.0/alumni/signals.py`

 * *Files identical despite different names*

### Comparing `aa_alumni-0.1.6a0/alumni/tasks.py` & `aa_alumni-0.2.0/alumni/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_alumni-0.1.6a0/pyproject.toml` & `aa_alumni-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -16,32 +16,32 @@
     "eveonline",
 ]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Celery",
     "Framework :: Django",
     "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content"
 ]
 dependencies = [
     "allianceauth>=3.0.0,<5.0.0",
-    "django-eveuniverse",
-    "django-solo>=2.0.0,<3.0.0",
-    "py-cord>=2.0.0,<3.0.0"
+    "django-solo>=2.0.0,<3.0.0"
 ]
 
 [project.urls]
 Homepage = "https://gitlab.com/tactical-supremacy/aa-alumni"
 Source = "https://gitlab.com/tactical-supremacy/aa-alumni"
 Tracker = "https://gitlab.com/tactical-supremacy/aa-alumni/-/issues"
 
@@ -64,7 +64,12 @@
 skip_gitignore = true
 
 [tool.flake8]
 exclude = [".git", "*migrations*", ".tox", "dist", "htmlcov"]
 max-line-length = 119
 select = ["C", "E", "F", "W", "B", "B950"]
 ignore = ['E203', 'E231', 'E501', 'W503', 'W291', 'W293']
+
+[tool.djlint]
+max_attribute_length=119
+max_line_length=119
+max_blank_lines=1
```

### Comparing `aa_alumni-0.1.6a0/PKG-INFO` & `aa_alumni-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: aa_alumni
-Version: 0.1.6a0
+Version: 0.2.0
 Summary: Integration with Alliance Auths State System, creates and maintains an Alumni State for past members of an Alliance and/or Corporation
 Keywords: allianceauth,eveonline
 Author-email: Joel Falknau <joel.falknau@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Celery
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: allianceauth>=3.0.0,<5.0.0
-Requires-Dist: django-eveuniverse
 Requires-Dist: django-solo>=2.0.0,<3.0.0
-Requires-Dist: py-cord>=2.0.0,<3.0.0
 Project-URL: Homepage, https://gitlab.com/tactical-supremacy/aa-alumni
 Project-URL: Source, https://gitlab.com/tactical-supremacy/aa-alumni
 Project-URL: Tracker, https://gitlab.com/tactical-supremacy/aa-alumni/-/issues
 
 # Alliance Auth - Alumni
 
 ## Features
@@ -40,15 +40,15 @@
 
 ### Step 1 - Prepare Auth
 
 Remove/Promote any state with a priority of `1`, Alumni is considered slightly better than the built in Guest State.
 
 ### Step 2 - Install from pip
 
-```bash
+```shell
 pip install aa-alumni
 ```
 
 ### Step 3 - Configure Auth settings
 
 Configure your Auth settings (`local.py`) as follows:
 
@@ -66,15 +66,15 @@
     'task': 'alumni.tasks.update_all_models',
     'schedule': crontab(minute=0, hour=0, day_of_week=3),
 }
 ```
 
 ### Step 4 - Update AA's State system
 
-```bash
+```shell
 python myauth/manage.py alumni_state
 ```
 
 ### Step 5 - Maintain Alliance Auth
 
 - Run migrations `python manage.py migrate`
 - Gather your staticfiles `python manage.py collectstatic`
```

